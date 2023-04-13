# Comparing `tmp/geo-espresso-0.2.1.dev0.tar.gz` & `tmp/geo-espresso-0.2.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geo-espresso-0.2.1.dev0.tar", last modified: Mon Mar  6 02:28:35 2023, max compression
+gzip compressed data, was "geo-espresso-0.2.1.dev1.tar", last modified: Sat Apr  1 01:50:48 2023, max compression
```

## Comparing `geo-espresso-0.2.1.dev0.tar` & `geo-espresso-0.2.1.dev1.tar`

### file list

```diff
@@ -1,116 +1,182 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:28:35.487293 geo-espresso-0.2.1.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-03-06 02:28:35.487293 geo-espresso-0.2.1.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 02:28:35.487293 geo-espresso-0.2.1.dev0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:28:35.471294 geo-espresso-0.2.1.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:28:35.475293 geo-espresso-0.2.1.dev0/src/espresso/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_espresso_problem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:28:35.475293 geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/_fmm_tomography.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:28:35.475293 geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)    38400 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/datasets/cbmod.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:28:35.479293 geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/datasets/ttimes/
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/datasets/ttimes/receivers_InLab_lrt_r36.dat
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/datasets/ttimes/receivers_crossb_nwt_r10.dat
--rw-r--r--   0 runner    (1001) docker     (123)    37500 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/datasets/ttimes/sources_InLab_lrt_s500.dat
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/datasets/ttimes/sources_crossb_nwt_s10.dat
--rw-r--r--   0 runner    (1001) docker     (123)  1350000 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/datasets/ttimes/ttimes_InLab_lrt_s500_r36.dat
--rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/datasets/ttimes/ttimes_crossb_nwt_s10_r10.dat
--rwxr-xr-x   0 runner    (1001) docker     (123)    88120 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/fm2dss.o
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:28:35.471294 geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/fmst/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:28:35.479293 geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/fmst/src/
--rw-r--r--   0 runner    (1001) docker     (123)    57221 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/fmst/src/fm2dss.f90
--rw-r--r--   0 runner    (1001) docker     (123)    20366 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/waveTracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:28:35.479293 geo-espresso-0.2.1.dev0/src/espresso/_gravity_density/
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_gravity_density/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_gravity_density/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_gravity_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21254 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_gravity_density/_gravity_density.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:28:35.479293 geo-espresso-0.2.1.dev0/src/espresso/_gravity_density/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_gravity_density/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_gravity_density/data/gravmodel1.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_gravity_density/data/testdata.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:28:35.479293 geo-espresso-0.2.1.dev0/src/espresso/_machine/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_machine/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:28:35.479293 geo-espresso-0.2.1.dev0/src/espresso/_machine/build_package/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_machine/build_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_machine/build_package/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_machine/build_package/check_requires.py
--rw-r--r--   0 runner    (1001) docker     (123)    13516 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_machine/build_package/criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)    12728 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_machine/build_package/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_machine/build_package/run_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_machine/build_package/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_machine/build_package/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:28:35.479293 geo-espresso-0.2.1.dev0/src/espresso/_machine/doc_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_machine/doc_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_machine/doc_utils/gen_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:28:35.479293 geo-espresso-0.2.1.dev0/src/espresso/_machine/new_contribution/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:28:35.479293 geo-espresso-0.2.1.dev0/src/espresso/_machine/new_contribution/_template/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_machine/new_contribution/_template/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_machine/new_contribution/_template/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_machine/new_contribution/_template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:28:35.479293 geo-espresso-0.2.1.dev0/src/espresso/_machine/new_contribution/_template/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_machine/new_contribution/_template/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_machine/new_contribution/_template/data/testdata.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_machine/new_contribution/_template/example_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_machine/new_contribution/create_new_contrib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:28:35.479293 geo-espresso-0.2.1.dev0/src/espresso/_magnetotelluric_1D/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_magnetotelluric_1D/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_magnetotelluric_1D/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_magnetotelluric_1D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11981 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_magnetotelluric_1D/_magnetotelluric_1D.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:28:35.479293 geo-espresso-0.2.1.dev0/src/espresso/_magnetotelluric_1D/data/
--rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_magnetotelluric_1D/data/16-A_KN2.dat
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_magnetotelluric_1D/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:28:35.483293 geo-espresso-0.2.1.dev0/src/espresso/_magnetotelluric_1D/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_magnetotelluric_1D/examples/example_01.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_magnetotelluric_1D/examples/field_MT.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_magnetotelluric_1D/examples/synthetic_AMT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:28:35.483293 geo-espresso-0.2.1.dev0/src/espresso/_pumping_test/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_pumping_test/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_pumping_test/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_pumping_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14893 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_pumping_test/_pumping_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:28:35.483293 geo-espresso-0.2.1.dev0/src/espresso/_simple_regression/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_simple_regression/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_simple_regression/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_simple_regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_simple_regression/_simple_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:28:35.483293 geo-espresso-0.2.1.dev0/src/espresso/_slug_test/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_slug_test/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_slug_test/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_slug_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_slug_test/_slug_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-06 02:28:35.000000 geo-espresso-0.2.1.dev0/src/espresso/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:28:35.483293 geo-espresso-0.2.1.dev0/src/espresso/_xray_tomography/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_xray_tomography/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_xray_tomography/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_xray_tomography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11238 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_xray_tomography/_xray_tomography.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:28:35.483293 geo-espresso-0.2.1.dev0/src/espresso/_xray_tomography/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_xray_tomography/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55535 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_xray_tomography/data/csiro_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   510434 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_xray_tomography/data/example1.dat
--rw-r--r--   0 runner    (1001) docker     (123)   166740 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_xray_tomography/data/example2.dat
--rw-r--r--   0 runner    (1001) docker     (123)   233604 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_xray_tomography/data/example3.dat
--rw-r--r--   0 runner    (1001) docker     (123)   312372 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/_xray_tomography/data/inlab_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/list_problems.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:28:35.487293 geo-espresso-0.2.1.dev0/src/espresso/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/utils/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/utils/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-06 02:28:21.000000 geo-espresso-0.2.1.dev0/src/espresso/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:28:35.487293 geo-espresso-0.2.1.dev0/src/geo_espresso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-03-06 02:28:35.000000 geo-espresso-0.2.1.dev0/src/geo_espresso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-03-06 02:28:35.000000 geo-espresso-0.2.1.dev0/src/geo_espresso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 02:28:35.000000 geo-espresso-0.2.1.dev0/src/geo_espresso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-06 02:28:35.000000 geo-espresso-0.2.1.dev0/src/geo_espresso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-06 02:28:35.000000 geo-espresso-0.2.1.dev0/src/geo_espresso.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.861014 geo-espresso-0.2.1.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-04-01 01:50:48.861014 geo-espresso-0.2.1.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.833013 geo-espresso-0.2.1.dev1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.837013 geo-espresso-0.2.1.dev1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.837013 geo-espresso-0.2.1.dev1/docs/source/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/_ext/generate_contrib_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.837013 geo-espresso-0.2.1.dev1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    16996 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/_static/contrib_edit1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/_static/contrib_fork.png
+-rw-r--r--   0 runner    (1001) docker     (123)    82278 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/_static/contrib_fork2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22274 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/_static/contrib_fork3.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35166 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/_static/contrib_fork4.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36057 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/_static/contrib_pr1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/_static/espresso_arch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/_static/inlab_logo_60px.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.837013 geo-espresso-0.2.1.dev1/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.837013 geo-espresso-0.2.1.dev1/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/_templates/autosummary/exception.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/_templates/autosummary/function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.841013 geo-espresso-0.2.1.dev1/docs/source/contributor_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/contributor_guide/documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/contributor_guide/github.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/contributor_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13396 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/contributor_guide/new_contrib.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/contributor_guide/setup.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.841013 geo-espresso-0.2.1.dev1/docs/source/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/developer_guide/build.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/developer_guide/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/developer_guide/deploy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/developer_guide/develop.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/developer_guide/licence.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/developer_guide/repository.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/developer_guide/sphinx.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.841013 geo-espresso-0.2.1.dev1/docs/source/user_guide/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.841013 geo-espresso-0.2.1.dev1/docs/source/user_guide/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/user_guide/api/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.841013 geo-espresso-0.2.1.dev1/docs/source/user_guide/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/user_guide/contrib/_index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/user_guide/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/user_guide/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/user_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/user_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/user_guide/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/docs/source/user_guide/why.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 01:50:48.861014 geo-espresso-0.2.1.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.833013 geo-espresso-0.2.1.dev1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.845013 geo-espresso-0.2.1.dev1/src/espresso/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_espresso_problem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.845013 geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/_fmm_tomography.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.845013 geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)    38400 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/datasets/cbmod.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.845013 geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/datasets/ttimes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/datasets/ttimes/receivers_InLab_lrt_r36.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/datasets/ttimes/receivers_crossb_nwt_r10.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    37500 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/datasets/ttimes/sources_InLab_lrt_s500.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/datasets/ttimes/sources_crossb_nwt_s10.dat
+-rw-r--r--   0 runner    (1001) docker     (123)  1350000 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/datasets/ttimes/ttimes_InLab_lrt_s500_r36.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/datasets/ttimes/ttimes_crossb_nwt_s10_r10.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.849013 geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/fmst/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1115 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/fmst/compile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.849013 geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/fmst/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    57221 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/fmst/src/fm2dss.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    20349 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/waveTracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.849013 geo-espresso-0.2.1.dev1/src/espresso/_gravity_density/
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_gravity_density/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_gravity_density/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_gravity_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21254 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_gravity_density/_gravity_density.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.849013 geo-espresso-0.2.1.dev1/src/espresso/_gravity_density/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_gravity_density/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_gravity_density/data/gravmodel1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_gravity_density/data/testdata.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_gravity_density/metadata.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.849013 geo-espresso-0.2.1.dev1/src/espresso/_machine/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_machine/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.853014 geo-espresso-0.2.1.dev1/src/espresso/_machine/build_package/
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_machine/build_package/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9335 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_machine/build_package/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_machine/build_package/check_requires.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_machine/build_package/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13630 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_machine/build_package/criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_machine/build_package/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_machine/build_package/run_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_machine/build_package/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_machine/build_package/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.853014 geo-espresso-0.2.1.dev1/src/espresso/_machine/doc_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_machine/doc_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_machine/doc_utils/gen_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.853014 geo-espresso-0.2.1.dev1/src/espresso/_machine/new_contribution/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.853014 geo-espresso-0.2.1.dev1/src/espresso/_machine/new_contribution/_template/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_machine/new_contribution/_template/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_machine/new_contribution/_template/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_machine/new_contribution/_template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.853014 geo-espresso-0.2.1.dev1/src/espresso/_machine/new_contribution/_template/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_machine/new_contribution/_template/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_machine/new_contribution/_template/data/testdata.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_machine/new_contribution/_template/example_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_machine/new_contribution/create_new_contrib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.853014 geo-espresso-0.2.1.dev1/src/espresso/_magnetotelluric_1D/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_magnetotelluric_1D/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_magnetotelluric_1D/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_magnetotelluric_1D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_magnetotelluric_1D/_magnetotelluric_1D.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.853014 geo-espresso-0.2.1.dev1/src/espresso/_magnetotelluric_1D/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_magnetotelluric_1D/data/16-A_KN2.dat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_magnetotelluric_1D/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.857014 geo-espresso-0.2.1.dev1/src/espresso/_magnetotelluric_1D/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)   125288 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_magnetotelluric_1D/examples/example_01.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_magnetotelluric_1D/examples/example_01.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101422 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_magnetotelluric_1D/examples/field_MT.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_magnetotelluric_1D/examples/field_MT.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146169 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_magnetotelluric_1D/examples/synthetic_AMT.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_magnetotelluric_1D/examples/synthetic_AMT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.857014 geo-espresso-0.2.1.dev1/src/espresso/_pumping_test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_pumping_test/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_pumping_test/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_pumping_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14893 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_pumping_test/_pumping_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.857014 geo-espresso-0.2.1.dev1/src/espresso/_simple_regression/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_simple_regression/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_simple_regression/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_simple_regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_simple_regression/_simple_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.857014 geo-espresso-0.2.1.dev1/src/espresso/_slug_test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_slug_test/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_slug_test/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_slug_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_slug_test/_slug_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-01 01:50:48.000000 geo-espresso-0.2.1.dev1/src/espresso/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.857014 geo-espresso-0.2.1.dev1/src/espresso/_xray_tomography/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_xray_tomography/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_xray_tomography/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_xray_tomography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11238 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_xray_tomography/_xray_tomography.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.861014 geo-espresso-0.2.1.dev1/src/espresso/_xray_tomography/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_xray_tomography/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55535 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_xray_tomography/data/csiro_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   510434 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_xray_tomography/data/example1.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   166740 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_xray_tomography/data/example2.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   233604 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_xray_tomography/data/example3.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   312372 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/_xray_tomography/data/inlab_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/list_problems.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.861014 geo-espresso-0.2.1.dev1/src/espresso/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/utils/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/utils/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-01 01:50:31.000000 geo-espresso-0.2.1.dev1/src/espresso/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:50:48.861014 geo-espresso-0.2.1.dev1/src/geo_espresso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-04-01 01:50:48.000000 geo-espresso-0.2.1.dev1/src/geo_espresso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-04-01 01:50:48.000000 geo-espresso-0.2.1.dev1/src/geo_espresso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 01:50:48.000000 geo-espresso-0.2.1.dev1/src/geo_espresso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-01 01:50:48.000000 geo-espresso-0.2.1.dev1/src/geo_espresso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-01 01:50:48.000000 geo-espresso-0.2.1.dev1/src/geo_espresso.egg-info/top_level.txt
```

### Comparing `geo-espresso-0.2.1.dev0/LICENCE` & `geo-espresso-0.2.1.dev1/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/PKG-INFO` & `geo-espresso-0.2.1.dev1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo-espresso
-Version: 0.2.1.dev0
+Version: 0.2.1.dev1
 Summary: Earth Science PRoblems for the Evaluation of Strategies, Solvers and Optimizers
 Author: InLab, Espresso development team
 Keywords: inversion,inference,python package,geoscience,geophysics
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
@@ -16,21 +16,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Fortran
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: Other/Proprietary License
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: doc
 License-File: LICENCE
 
 # Espresso
 
 [![PyPI version](https://img.shields.io/pypi/v/geo-espresso?logo=pypi&style=flat-square&color=bde0fe&labelColor=f8f9fa)](https://pypi.org/project/geo-espresso/)
+[![build](https://img.shields.io/github/actions/workflow/status/inlab-geo/espresso/build_wheels.yml?branch=main&logo=githubactions&style=flat-square&color=ccd5ae&labelColor=f8f9fa)](https://github.com/inlab-geo/espresso/actions/workflows/build_wheels.yml)
 [![Documentation Status](https://img.shields.io/readthedocs/geo-espresso?logo=readthedocs&style=flat-square&color=fed9b7&labelColor=f8f9fa&logoColor=eaac8b)](https://geo-espresso.readthedocs.io/en/latest/?badge=latest)
 [![Slack](https://img.shields.io/badge/Slack-InLab_community-4A154B?logo=slack&style=flat-square&color=cdb4db&labelColor=f8f9fa&logoColor=9c89b8)](https://join.slack.com/t/inlab-community/shared_invite/zt-1ejny069z-v5ZyvP2tDjBR42OAu~TkHg)
 
 ## Introduction
 
 **E**arth **S**cience **PR**oblems for the **E**valuation of **S**trategies, 
 **S**olvers and **O**ptimizers (Espresso) is a collection of datasets, and
```

### Comparing `geo-espresso-0.2.1.dev0/README.md` & `geo-espresso-0.2.1.dev1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Espresso
 
 [![PyPI version](https://img.shields.io/pypi/v/geo-espresso?logo=pypi&style=flat-square&color=bde0fe&labelColor=f8f9fa)](https://pypi.org/project/geo-espresso/)
+[![build](https://img.shields.io/github/actions/workflow/status/inlab-geo/espresso/build_wheels.yml?branch=main&logo=githubactions&style=flat-square&color=ccd5ae&labelColor=f8f9fa)](https://github.com/inlab-geo/espresso/actions/workflows/build_wheels.yml)
 [![Documentation Status](https://img.shields.io/readthedocs/geo-espresso?logo=readthedocs&style=flat-square&color=fed9b7&labelColor=f8f9fa&logoColor=eaac8b)](https://geo-espresso.readthedocs.io/en/latest/?badge=latest)
 [![Slack](https://img.shields.io/badge/Slack-InLab_community-4A154B?logo=slack&style=flat-square&color=cdb4db&labelColor=f8f9fa&logoColor=9c89b8)](https://join.slack.com/t/inlab-community/shared_invite/zt-1ejny069z-v5ZyvP2tDjBR42OAu~TkHg)
 
 ## Introduction
 
 **E**arth **S**cience **PR**oblems for the **E**valuation of **S**trategies, 
 **S**olvers and **O**ptimizers (Espresso) is a collection of datasets, and
```

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/__init__.py` & `geo-espresso-0.2.1.dev1/src/espresso/__init__.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -49,18 +49,18 @@
 
 # from .example_name import ExampleName
 
 # from .list_problems import list_problem_names, list_problems
 # __all__ += list_problem_names()
 # __all__ += ["list_problem_names", "list_problems"]
 
+from ._fmm_tomography import FmmTomography
+from ._pumping_test import PumpingTest
 from ._simple_regression import SimpleRegression
 from ._slug_test import SlugTest
-from ._fmm_tomography import FmmTomography
 from ._xray_tomography import XrayTomography
 from ._gravity_density import GravityDensity
 from ._magnetotelluric_1D import Magnetotelluric1D
-from ._pumping_test import PumpingTest
 
 from .list_problems import list_problem_names, list_problems
 __all__ += list_problem_names()
 __all__ += ['list_problem_names', 'list_problems']
```

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_espresso_problem.py` & `geo-espresso-0.2.1.dev1/src/espresso/_espresso_problem.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/CMakeLists.txt` & `geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/CMakeLists.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 if(SKBUILD)
   message(STATUS "The project is built using scikit-build")
+  enable_language(Fortran)
   set(fmm_fortran_src "${CMAKE_CURRENT_SOURCE_DIR}/fmst/src/fm2dss.f90")
   set_source_files_properties(${fmm_fortran_src} PROPERTIES LANGUAGE "Fortran")
   set(fmm_generated "fm2dss.o")
   add_executable(${fmm_generated} ${fmm_fortran_src})
   install(FILES 
     ${CMAKE_CURRENT_BINARY_DIR}/${fmm_generated} 
     ${CMAKE_CURRENT_BINARY_DIR}/globalp.mod
     ${CMAKE_CURRENT_BINARY_DIR}/traveltime.mod
-    DESTINATION _fmm_tomography/)
+    DESTINATION _fmm_tomography/build)
 else()
+  # Run "mkdir build; cd build; cmake ..; make"
   message(STATUS "The project is NOT built using scikit-build")
   cmake_minimum_required(VERSION 3.11.0)
   project(FMMTOMO Fortran)
   add_executable(fm2dss.o fmst/src/fm2dss.f90)
 endif()
```

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/LICENCE` & `geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/README.md` & `geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/README.md`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/__init__.py` & `geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/__init__.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/_fmm_tomography.py` & `geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/_fmm_tomography.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/datasets/cbmod.txt` & `geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/datasets/cbmod.txt`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/datasets/ttimes/receivers_InLab_lrt_r36.dat` & `geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/datasets/ttimes/receivers_InLab_lrt_r36.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/datasets/ttimes/receivers_crossb_nwt_r10.dat` & `geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/datasets/ttimes/receivers_crossb_nwt_r10.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/datasets/ttimes/sources_InLab_lrt_s500.dat` & `geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/datasets/ttimes/sources_InLab_lrt_s500.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/datasets/ttimes/sources_crossb_nwt_s10.dat` & `geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/datasets/ttimes/sources_crossb_nwt_s10.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/datasets/ttimes/ttimes_InLab_lrt_s500_r36.dat` & `geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/datasets/ttimes/ttimes_InLab_lrt_s500_r36.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/datasets/ttimes/ttimes_crossb_nwt_s10_r10.dat` & `geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/datasets/ttimes/ttimes_crossb_nwt_s10_r10.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/fmst/src/fm2dss.f90` & `geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/fmst/src/fm2dss.f90`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_fmm_tomography/waveTracker.py` & `geo-espresso-0.2.1.dev1/src/espresso/_fmm_tomography/waveTracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,21 +91,24 @@
         noncushion,nodemap = write_gridc(v,self.extent,wdir) # write data for input velocity model file gridc.txc
     
         write_otimes([[True]*len(recs)]*len(srcs),wdir) # write out rays to be calculated
     
         # run fmst wavefront tracker code from command line
         # see if the executable is there, otherwise do preparation for the executable
         out = run_fm2dss(wdir)
-        if out.returncode:      # re-compile if there's an error
-            compile_fm2dss()
-            out = run_fm2dss(wdir)
+        # if out.returncode:      # re-compile if there's an error
+        #     compile_fm2dss()
+        #     out = run_fm2dss(wdir)
         if out.returncode:      # add permission if there's a further error
             print("Trying to fix now...")
             try:
-                Path(wdir + "/fm2dss.o").chmod(0o774)
+                import stat
+                exe_file = Path(wdir + "/build/fm2dss.o")
+                st = os.stat(exe_file)
+                os.chmod(exe_file, st.st_mode | stat.S_IEXEC)
                 print("Execute permission given to fm2dss.o.")
             except:
                 print("Failed to fix. Check error message above.")
             out = run_fm2dss(wdir)
         if(verbose): print(' Message from fmm2dss:',out.stdout)
         if(out.returncode != 0):
             print(' The process returned with errorcode:',out.returncode)
@@ -454,26 +457,22 @@
         if surface[1] or surface[2]:
             out+=[[extent[1],extent[2]]]
         if surface[1] or surface[3]:
             out+=[[extent[1],extent[3]]]
     return np.array(out)
 
 def run_fm2dss(wdir):
-    command = "./fm2dss.o"
+    command = "./build/fm2dss.o"
     return subprocess.run(command,stdout=subprocess.PIPE, text=True,shell=True,cwd=wdir)
 
 def compile_fm2dss():
     # https://github.com/inlab-geo/espresso/blob/main/espresso_machine/build_package/validate.py#L170
-    build_dir = path(".")
-    res1 = subprocess.call(["cmake", "."], cwd=build_dir)
+    build_dir = path("./build")
+    res1 = subprocess.call(["cmake", ".."], cwd=build_dir)
     if res1:
         raise ChildProcessError(f"`cmake .` failed in {build_dir}")
     res2 = subprocess.call(["make"], cwd=build_dir)
     if res2:
         raise ChildProcessError(f"`make` failed in {build_dir}")
-    clean_cmake_files()
 
-def clean_cmake_files():
-    shutil.rmtree(path("CMakeFiles"))
-    files_to_rm = ["Makefile", "cmake_install.cmake", "CMakeCache.txt"]
-    for file in files_to_rm:
-        silent_remove(path(file))
+def clean_fm2dss():
+    shutil.rmtree(path("build"))
```

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_gravity_density/LICENCE` & `geo-espresso-0.2.1.dev1/src/espresso/_gravity_density/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_gravity_density/README.md` & `geo-espresso-0.2.1.dev1/src/espresso/_gravity_density/README.md`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_gravity_density/_gravity_density.py` & `geo-espresso-0.2.1.dev1/src/espresso/_gravity_density/_gravity_density.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_machine/README.md` & `geo-espresso-0.2.1.dev1/src/espresso/_machine/README.md`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_machine/build_package/build.py` & `geo-espresso-0.2.1.dev1/src/espresso/_machine/build_package/build.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,83 +1,83 @@
 """Build the Python package "espresso"
 
 1. clean "_esp_build/"
 2. "/<meta-data-files>" => "_esp_build/"
-3. "src/" => "_esp_build/src/"
-4. "contrib/" => "_esp_build/src/espresso/" + "__init__.py" + "list_problems.py"
-5. "_version.py" => "_esp_build/pyproject.toml"
-6. "espresso_machine/" => _esp_build/src/_machine"
-6. `pip install .`
+3. generate "_version.py"
+4. "src/" => "_esp_build/src/"
+5. "contrib/" => "_esp_build/src/espresso/" + "__init__.py" + "list_problems.py"
+6. remove `.core` from versioningit_config
+7. "espresso_machine/" => _esp_build/src/_machine"
+8. build capability_matrix
+9. `pip install .`      (can be disabled by `--no-install`)
 
+Usage: python build.py [--pre] [--post] [--no-install] [-c <example_name>]
 """
 
 import subprocess
 import sys
 import os
-import argparse
-import pytest
 from shutil import copytree, copy, rmtree, ignore_patterns
 from pathlib import Path
 import versioningit
+import json
+
+import _utils
+import report
+import validate
 
 
 # ------------------------ constants ------------------------
-PKG_NAME = "espresso"
+MODULE_NAME = "espresso"
+PKG_NAME = "geo-espresso"
 current_directory = Path(__file__).resolve().parent
 root = current_directory.parent.parent
 ROOT_DIR = str(root)
 BUILD_DIR = str(root / "_esp_build")
 PKG_SRC = str(root / "src")
 CONTRIB_SRC = str(root / "contrib")
 VCS_GIT = str(root / ".git")
 DOCS_SRC = str(root / "docs")
 MACHINE_SRC = str(root / "espresso_machine")
 META_FILES = [
     "README.md",
     "pyproject.toml",
+    "setup.py",
     "LICENCE",
+    "CMakeLists.txt",
     ".readthedocs.yml",
     ".gitignore",
     "CHANGELOG.md",
 ]
-
-# ------------------------ argument parser ------------------------
-def setup_parser():
-    parser = argparse.ArgumentParser(
-        description="Script to build Espresso, with/without pre/post-build validation"
-    )
-    parser.add_argument(
-        "--validate", "-v", "--checks", dest="validate", action="store_true", 
-        default=False, help="Run tests before and after building the package")
-    return parser
-
-args = setup_parser().parse_args()
+PROBLEMS_TO_COMPILE_FILE = "problems_to_compile.txt"
+validate_script = str(Path(__file__).resolve().parent / "validate.py")
 
 
 # ------------------------ helpers ------------------------
 def is_cache(file_name):
     return file_name.endswith(".pyc") or \
         file_name == "__pycache__" or \
             file_name == "cmake_install.cmake" or \
                 file_name.endswith(".mod") or \
                     file_name.endswith(".out") or \
                         file_name == "CMakeFiles" or \
-                            file_name == "Makefile"
+                            file_name == "Makefile" or \
+                                file_name == PROBLEMS_TO_COMPILE_FILE
 
-def move_folder_content(folder_path, dest_path, prefix=None):
+def move_folder_content(folder_path, dest_path, prefix=None, only_include=None):
     if prefix is None:
         copytree(
             folder_path, 
             dest_path, 
             # dirs_exist_ok=True, 
             ignore=ignore_patterns('*.pyc', 'tmp*', '__pycache__')
          )
     else:
         for f in os.listdir(folder_path):
-            if is_cache(f):
+            if is_cache(f) or (only_include is not None and f not in only_include):
                 continue
             src = f"{folder_path}/{f}"
             dst = f"{dest_path}/{prefix}{f}"
             copytree(src, dst, 
                 ignore=ignore_patterns(
                     "*.pyc", "__pycache__", "tmp*", "CMakeFiles", "Makefile", "*.mod", "*.out"
                 ))
@@ -104,153 +104,157 @@
 # 2
 def move_pkg_metadata():
     move_folder_content(DOCS_SRC, f"{BUILD_DIR}/docs")
     for f in META_FILES:
         copy(f"{ROOT_DIR}/{f}", f"{BUILD_DIR}/{f}")
 
 # 3
+def write_version():
+    versioningit_config = {
+        "format": {
+            "distance": "{base_version}+{distance}.{vcs}{rev}",
+            "dirty": "{base_version}+{distance}.{vcs}{rev}.dirty",
+            "distance-dirty": "{base_version}+{distance}.{vcs}{rev}.dirty",
+        },
+        "write": {
+            "file": "src/espresso/_version.py"
+        }
+    }
+    versioningit.get_version(root, versioningit_config, True)
+
+# 4
 def move_pkg_source():
     move_folder_content(PKG_SRC, f"{BUILD_DIR}/src")
 
-# 4
+# 5 
+def change_versioningit_config():
+    with open(f"{BUILD_DIR}/setup.py", "r") as f:
+        setup_content = f.read()
+    setup_content = setup_content.replace(".core", "")
+    setup_content = setup_content.replace('"rmsuffix": ""', '"rmsuffix": "-build"')
+    with open(f"{BUILD_DIR}/setup.py", "w") as f:
+        f.write(setup_content)
+
+# 6
 def move_contrib_source():
+    # see if any contribution is specified through command line args
+    specified_problems = _utils.args().contribs
     # move all contribution subfolders with prefix "_"
-    move_folder_content(CONTRIB_SRC, f"{BUILD_DIR}/src/{PKG_NAME}", prefix="_")
+    move_folder_content(
+        CONTRIB_SRC, 
+        f"{BUILD_DIR}/src/{MODULE_NAME}", 
+        prefix="_",
+        only_include=specified_problems,
+    )
     # collect a list of contributions + related strings to write later
     contribs = []
     init_file_imports = "\n"
-    init_file_all_nms = "\n_all_problem_names = [\n"
     init_file_all_cls = "\n_all_problems = [\n"
     for path in Path(CONTRIB_SRC).iterdir():
-        if path.is_dir():
-            contrib = os.path.basename(path)                    # name
-            contrib_class = contrib.title().replace("_", "")    # class
+        contrib = os.path.basename(path)                    # name
+        if path.is_dir() and \
+            (specified_problems is None or contrib in specified_problems):
+            contrib_class = _utils.problem_name_to_class(contrib)    # class
             contribs.append(contrib)
             init_file_imports += f"from ._{contrib} import {contrib_class}\n"
-            init_file_all_nms += f"\t'{contrib_class}',\n"
-            init_file_all_cls += f"\t{contrib_class},\n"
-    init_file_all_nms += "]"
+            init_file_all_cls += f"    {contrib_class},\n"
     init_file_all_cls += "]"
     # some constant strings to append to init file later
     init_file_imp_funcs = "\nfrom .list_problems import list_problem_names, list_problems"
     init_file_add_all_nms = "\n__all__ += list_problem_names()"
     init_file_add_funcs = "\n__all__ += ['list_problem_names', 'list_problems']\n"
     # write all above to files
-    with open(f"{BUILD_DIR}/src/{PKG_NAME}/__init__.py", "a") as f:
+    # compiled_code_list = set()
+    with open(f"{BUILD_DIR}/src/{MODULE_NAME}/CMakeLists.txt", "a") as f:
+        for contrib in contribs:
+            f.write(f"install(DIRECTORY _{contrib} DESTINATION .)\n")
+            if Path(f"{CONTRIB_SRC}/{contrib}/CMakeLists.txt").exists():
+                f.write(f"add_subdirectory(_{contrib})\n")
+                # compiled_code_list.add(contrib)
+    with open(f"{BUILD_DIR}/src/{MODULE_NAME}/__init__.py", "a") as f:
         f.write(init_file_imports)
         f.write(init_file_imp_funcs)
         f.write(init_file_add_all_nms)
         f.write(init_file_add_funcs)
-    with open(f"{BUILD_DIR}/src/{PKG_NAME}/list_problems.py", "a") as f:
+    with open(f"{BUILD_DIR}/src/{MODULE_NAME}/list_problems.py", "a") as f:
         f.write(init_file_imports)
-        f.write(init_file_all_nms)
         f.write(init_file_all_cls)
+    # with open(f"{ROOT_DIR}/contrib/{PROBLEMS_TO_COMPILE_FILE}", "w") as f:
+    #     f.writelines(compiled_code_list)
 
-# 5
-def write_version():
-    # get version
-    versioningit_config = {
-        "format": {
-            "distance": "{base_version}+{distance}.{vcs}{rev}",
-            "dirty": "{base_version}+{distance}.{vcs}{rev}.dirty",
-            "distance-dirty": "{base_version}+{distance}.{vcs}{rev}.dirty",
-        },
-        "write": {
-            "file": "src/espresso/_version.py"
-        }
-    }
-    version = versioningit.get_version(root, versioningit_config, True)
-    # --> read pyproject.toml
-    with open(f"{BUILD_DIR}/pyproject.toml", "r") as f:
-        file_content = f.read()
-    # --> process pyproject.toml
-    # write version to pyproject.toml (for local build)
-    file_content += "\n[tool.versioningit]"
-    file_content += f"\ndefault-version = '{version}'\n"
-    # change versioningit configs (for build from branch "esp_build")
-    file_content = file_content.replace(".core", "")
-    file_content += "\n[tool.versioningit.tag2version]"
-    file_content += "\nrmprefix = 'v'"
-    file_content += "\nrmsuffix = '-build'\n"
-    # --> write pyproject.toml
-    with open(f"{BUILD_DIR}/pyproject.toml", "w") as f:
-        f.write(file_content)
-
-# 6 move espresso_machine into espresso/_machine
+# 7 move espresso_machine into espresso/_machine
 def move_espresso_machine():
     move_folder_content(MACHINE_SRC, f"{BUILD_DIR}/src/espresso/_machine")
 
-# 7
-def install_pkg():
-    subprocess.call([sys.executable, "-m", "pip", "uninstall", "-y", PKG_NAME])
-    return subprocess.call([sys.executable, "-m", "pip", "install", "."], cwd=BUILD_DIR)
+# 8 build capability matrix
+def build_problem_capability():
+    # see if any contribution is specified through command line args
+    specified_problems = _utils.args().contribs
+    with _utils.suppress_stdout():
+        capability_report = report.capability_report(
+            problems_to_check=specified_problems
+        )
+    report_to_write = json.dumps(capability_report, indent=4)
+    with open(f"{BUILD_DIR}/src/{MODULE_NAME}/list_problems.py", "a") as f:
+        f.write("\n\n_capability_matrix = ")
+        f.write(report_to_write)
 
 # printing helper
 def println_with_emoji(content, emoji):
     try:
-        print(f"\n{emoji}  {content}")
+        print(f"\n{emoji} {content}")
     except:
         print(f"\n{content}")
 
 
 # ------------------------ main functions ------------------------
+build_pipeline = [
+    ( clean_build_folder, "Cleaning build folder..." ),
+    ( move_pkg_metadata, "Moving package metadata..." ),
+    ( write_version, "Generating version file..." ),
+    ( move_pkg_source, "Moving Espresso core packaging files..." ),
+    ( change_versioningit_config, "Removing `.core` from versioningit config..." ),
+    ( move_contrib_source, "Moving all contributions..." ),
+    ( move_espresso_machine, "Moving infrastructure code..." ),
+    ( build_problem_capability, "Building capability matrix... (this will take some time)" ),
+    # ( install_pkg, "Building Python package: geo-espresso..." ),
+]
+
 def build():
     println_with_emoji("Package building...", "🛠")
-    # 1
-    println_with_emoji("Cleaning build folder...", "🗂")
-    clean_build_folder()
-    print("OK.")
-    # 2
-    println_with_emoji("Moving package metadata...", "🗂")
-    move_pkg_metadata()
-    print("OK.")
-    # 3
-    println_with_emoji("Moving Espresso core packaging files...", "🗂")
-    move_pkg_source()
-    print("OK.")
-    # 4
-    println_with_emoji("Moving all contributions...", "🗂")
-    move_contrib_source()
-    print("OK.")
-    # 5
-    println_with_emoji("Generating version file...", "🗂")
-    write_version()
-    print("OK.")
-    # 6
-    println_with_emoji("Moving infrastructure code...", "🗂")
-    move_espresso_machine()
-    print("OK.")
-    # 6
-    println_with_emoji("Building Python package: geo-espresso...", "🗂")
-    exit_code = install_pkg()
-    if exit_code == 0: 
-        println_with_emoji("Espresso installed!", "🍰")
-    return exit_code
-
-def build_with_validate():
-    validate_script = str(Path(__file__).resolve().parent / "validate.py")
-
-    # pre-build validate
-    exit_code = subprocess.call([sys.executable, validate_script, "--pre"])
-    if exit_code != pytest.ExitCode.OK:
-        sys.exit(exit_code)
+    for (step, desc) in build_pipeline:
+        println_with_emoji(desc, "🗂")
+        try:
+            step()
+        except Exception as e:
+            println_with_emoji(f"Problem occurred in this step: {desc}\n", "❗️")
+            raise e
+        print("OK.")
+    # println_with_emoji("Espresso installed!", "🍰")
 
-    # build package
-    build()
+def install_pkg():
+    desc = "Building Python package: geo-espresso..."
+    println_with_emoji(desc, "🗂")
+    subprocess.call([sys.executable, "-m", "pip", "uninstall", "-y", PKG_NAME])
+    res = subprocess.call([sys.executable, "-m", "pip", "install", "."], cwd=BUILD_DIR)
+    if res != 0:
+        sys.exit(res)
 
-    # post-build validation
-    exit_code = subprocess.call([sys.executable, validate_script, "--post"])
-    if exit_code != pytest.ExitCode.OK:
-        sys.exit(exit_code)
-    else:
-        print("\n🍰 All done 🍰")
-        sys.exit(exit_code)
+def pre_validate():
+    validate.main(pre_build=True)
 
+def post_validate():
+    validate.main(pre_build=False)
 
 def main():
-    if args.validate:
-        build_with_validate()
-    else:
-        build()
+    _args = _utils.args()
+    if _args.pre:
+        pre_validate()
+    build()
+    if not _args.dont_install:
+        install_pkg()
+    if _args.post:
+        post_validate()
+    println_with_emoji("All done", "🍰")
 
 if __name__ == "__main__":
-    sys.exit(main())
+    main()
```

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_machine/build_package/criteria.py` & `geo-espresso-0.2.1.dev1/src/espresso/_machine/build_package/criteria.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 
 Check comments for these functions for what criteria are implemented.
 """
 
 import os
 import numpy as np
 from matplotlib.figure import Figure
+
 import run_examples
+import _utils
 
 try:
     import espresso
 except ModuleNotFoundError as e:
     e.msg += "\n\nNote: To run pre-build validation, please firstly install " \
              "`espresso` core module by running the following from the root" \
              "level of the project\n  $ pip install ."
@@ -52,15 +54,17 @@
         f"`__all__ = ['{prob_class_name}']` in the file " \
             f"contrib/{prob_name}/__init__.py"
     try:
         _init_all = parent_mod.__all__
     except:
         raise AssertionError(_class_not_in_init_all_msg)
     else:
-        assert prob_class_name in _init_all, _class_not_in_init_all_msg
+        assert prob_class_name in _init_all, \
+            _class_not_in_init_all_msg + \
+                f". We found {_init_all} but {prob_class_name} is not in there"
 
 # 5. The class is a subclass of EspressoProblem
 def _check_subclass(prob_class, prob_class_name):
     assert issubclass(prob_class, espresso.EspressoProblem), \
         f"make sure your problem class `{prob_class_name}` is a subclass of " \
             f"`espresso.EspressoProblem`, by defining it with:\n\n-------\n" \
                 f"from espresso import EspressoProblem\n\n" \
@@ -157,15 +161,15 @@
         - [optional] citations -> []
         - [optional] linked_sites -> [(name, link)]
 
     Note: a problem will have several examples, but we will put all the criteria for
     the examples to function `criteria_for_example`.
     """
     # preparation
-    names_in_folder, paths_in_folder = run_examples.get_folder_content(prob_path)
+    names_in_folder, paths_in_folder = _utils.get_folder_content(prob_path)
     prob_name = prob_path.split("/")[-1]
 
     # checking
     _check_folder_file_names(prob_name, prob_path, names_in_folder)
     _check_required_files(prob_path, names_in_folder)
     _check_licence_nonempty(prob_path)
     _check_init_all(parent_mod, prob_name, prob_class_name)
@@ -280,16 +284,16 @@
             raise NotImplementedError(f"{obj_str} is required but you haven't implemented it")
         if obj is not None:
             for check_func in to_check:
                 check_func(all_results, obj, obj_str)
 
 
 def main():
-    problems = run_examples.problems_to_run(problems_specified=["testtest"])
-    results = run_examples.run_problems(problems, pre_build=True)
+    problems = _utils.problems_to_run(problems_specified=["testtest"])
+    results = run_examples.run_problems(problems, pre_build=True, timeout=300)
     for res in results:
         criteria_for_problem(
             res["problem class"],
             res["problem class str"],
             res["problem path"],
             res["parent module"], 
         )
```

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_machine/build_package/report.py` & `geo-espresso-0.2.1.dev1/src/espresso/_machine/build_package/report.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 """Generate API compliance report 
 
 Usage:
 - To generate raw report, raw_compliance_report(problems_to_check=None, pre_build=True)
 - To generate report, compliance_report(problems_to_check=None, pre_build=True)
 - To print report, print_compliance_report(report)
 """
-
 import run_examples
 import criteria
+import _utils
 
 
 def _init_attr_report():
+    import criteria
     _report = {
         "required": dict(),
         "optional": dict(),
         "additional": set(),
     }
     for attr_check in criteria.attributes_to_check:
         _, attr_str, required, _ = attr_check
         _report_key = "required" if required else "optional"
         _attr_key_name = attr_str.split("(")[0]
         _report[_report_key][_attr_key_name] = []
     return _report
 
 def _collect_compliance_info(all_results, report):
+    import criteria
     _has_init_error = isinstance(all_results["prob_instance"], Exception)
     if _has_init_error:
         _init_error = all_results["prob_instance"]
     for attr_check in criteria.attributes_to_check:
         attr_key, attr_str, required, to_check = attr_check
         _report_key = "required" if required else "optional"
         _attr_key_name = attr_str.split("(")[0]
@@ -62,15 +64,15 @@
     if isinstance(p, Exception):
         return
     p_dir = [attr for attr in dir(p) if not attr.startswith("_")]
     _standard_attr = _example_standard(p, report)
     _additional_attr = {a for a in p_dir if a not in _standard_attr}
     report["additional"].update(_additional_attr)
 
-def raw_compliance_report(problems_to_check=None, pre_build=True):
+def raw_compliance_report(problems_to_check=None, pre_build=True, timeout=None):
     """Run all problems and generate a raw compliance report
     
     A typical raw report looks like:
     {
         'FmmTomography': {
             'metadata': True, 
             'attributes': {
@@ -84,16 +86,16 @@
                     'exe_fm2dss', 'clean_tmp_files', 'tmp_paths', 'tmp_files'
                 }
             }
         }
     }
     """
     report = dict()
-    problems = run_examples.problems_to_run(problems_specified=problems_to_check)
-    results = run_examples.run_problems(problems, pre_build=pre_build)
+    problems = _utils.problems_to_run(problems_to_check)
+    results = run_examples.run_problems(problems, pre_build=pre_build, timeout=timeout)
     for res in results:
         _report_for_problem = dict()
         # problem level report
         if isinstance(res["parent module"], Exception):
             _report_for_problem["metadata"] = res["parent module"]
         else:
             try:
@@ -143,15 +145,15 @@
 def _analyse_compliance(new_report):
     _metadata_ok = new_report["metadata"] == "OK"
     _required_count = new_report["required_count"]
     _required_ok = _required_count["implemented"] == _required_count["total"]
     _optional_ok = new_report["optional_count"]["error"] == 0
     return _metadata_ok and _required_ok and _optional_ok
 
-def compliance_report(problems_to_check=None, pre_build=True):
+def compliance_report(problems_to_check=None, pre_build=True, timeout=60):
     """Generate a readable compliance report based on running raw report
     
     A typical compliance report looks like:
     {
         'FmmTomography': {
             'metadata': 'OK', 
             'required': {'model_size': 'OK', 'data_size': 'OK', 'good_model': 'OK', 'starting_model': 'OK', 'data': 'OK', 'forward': 'OK'}, 
@@ -160,15 +162,15 @@
             'optional_count': {'implemented': 3, 'not_implemented': 7, 'error': 0, 'total': 10}, 
             'additional': {'clean_tmp_files', 'tmp_paths', 'exe_fm2dss', 'tmp_files'}, 
             'additional_count': 4, 
             'api_compliance': True,
         }
     }
     """
-    raw_report = raw_compliance_report(problems_to_check, pre_build)
+    raw_report = raw_compliance_report(problems_to_check, pre_build, timeout)
     new_report = dict()
     for prob_name, prob_report in raw_report.items():
         _new_report = dict()
         # metadata
         _metadata = prob_report["metadata"]
         _new_report["metadata"] = "OK" if _metadata == True else _metadata
         # check possibility to continue
@@ -188,15 +190,15 @@
         _new_report["additional"] = prob_report["attributes"]["additional"]
         _new_report["additional_count"] = len(_new_report["additional"])
         # sum up
         _new_report["api_compliance"] = _analyse_compliance(_new_report)
         new_report[prob_name] = _new_report
     return new_report
 
-# from SO: https://stackoverflow.com/questions/287871/how-do-i-print-colored-text-to-the-terminal
+# from SO: https://stackoverflow.com/a/287944
 class bcolors:
     HEADER = '\033[95m'
     OKBLUE = '\033[94m'
     OKCYAN = '\033[96m'
     OKGREEN = '\033[92m'
     WARNING = '\033[93m'
     FAIL = '\033[91m'
@@ -301,7 +303,24 @@
             print(f"\t.{attr_name}")
         #### sum up
         _api_compliance = r["api_compliance"]
         if _api_compliance:
             print(cformat(bcolors.OKCYAN, f"\n{prob} is API-compliance. Cheers!"))
         else:
             print(cformat(bcolors.FAIL, f"\n{prob} is not API-compliant."))
+
+def capability_report(problems_to_check=None, timeout=1):
+    # those with TimeoutError will be approximated to be OK
+    _compliance_report = compliance_report(problems_to_check, True, timeout)
+    _capability_report = dict()
+    for prob, res in _compliance_report.items():
+        _new_report = dict()
+        if "required" not in res:
+            raise RuntimeError(res)
+        for attr, attr_res in res["required"].items():
+            _new_report[attr] = int(attr_res == "OK" or isinstance(attr_res, TimeoutError))
+        for attr, attr_res in res["optional"].items():
+            _new_report[attr] = int(attr_res == "OK" or isinstance(attr_res, TimeoutError))
+        for additional in res["additional"]:
+            _new_report[additional] = 1
+        _capability_report[prob] = _new_report
+    return _capability_report
```

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_machine/doc_utils/gen_docs.py` & `geo-espresso-0.2.1.dev1/src/espresso/_machine/doc_utils/gen_docs.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_machine/new_contribution/_template/LICENCE` & `geo-espresso-0.2.1.dev1/src/espresso/_machine/new_contribution/_template/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_machine/new_contribution/_template/README.md` & `geo-espresso-0.2.1.dev1/src/espresso/_machine/new_contribution/_template/README.md`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_machine/new_contribution/_template/example_name.py` & `geo-espresso-0.2.1.dev1/src/espresso/_machine/new_contribution/_template/example_name.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_machine/new_contribution/create_new_contrib.py` & `geo-espresso-0.2.1.dev1/src/espresso/_machine/new_contribution/create_new_contrib.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_magnetotelluric_1D/LICENCE` & `geo-espresso-0.2.1.dev1/src/espresso/_magnetotelluric_1D/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_magnetotelluric_1D/README.md` & `geo-espresso-0.2.1.dev1/src/espresso/_magnetotelluric_1D/README.md`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_magnetotelluric_1D/__init__.py` & `geo-espresso-0.2.1.dev1/src/espresso/_magnetotelluric_1D/__init__.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_magnetotelluric_1D/_magnetotelluric_1D.py` & `geo-espresso-0.2.1.dev1/src/espresso/_magnetotelluric_1D/_magnetotelluric_1D.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,15 @@
             axs[1].plot(np.log10(1/self._freqs), phase2, 'k-', lw = 1, zorder = 2)
         axs[0].set_ylabel('Log$_{10}$ $\\rho_{app}$ ($\Omega$m)')
         axs[1].set_yticks([0,45,90])
         axs[1].set_ylabel('Phase (deg.)')
         axs[1].set_xlabel('Log$_{10}$ Period (s)')
         axs[0].grid(lw=0.2)
         axs[1].grid(lw=0.2)
-        axs[0].legend()
+        # axs[0].legend()
         plt.tight_layout()
         #plt.show()
         return fig
 
     def misfit(self, data, data2, Cm_inv = None):
         res = data - data2
         if Cm_inv is None:
```

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_magnetotelluric_1D/data/16-A_KN2.dat` & `geo-espresso-0.2.1.dev1/src/espresso/_magnetotelluric_1D/data/16-A_KN2.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_magnetotelluric_1D/examples/example_01.py` & `geo-espresso-0.2.1.dev1/src/espresso/_magnetotelluric_1D/examples/example_01.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_magnetotelluric_1D/examples/field_MT.py` & `geo-espresso-0.2.1.dev1/src/espresso/_magnetotelluric_1D/examples/field_MT.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_magnetotelluric_1D/examples/synthetic_AMT.py` & `geo-espresso-0.2.1.dev1/src/espresso/_magnetotelluric_1D/examples/synthetic_AMT.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_pumping_test/LICENCE` & `geo-espresso-0.2.1.dev1/src/espresso/_pumping_test/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_pumping_test/README.md` & `geo-espresso-0.2.1.dev1/src/espresso/_pumping_test/README.md`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_pumping_test/_pumping_test.py` & `geo-espresso-0.2.1.dev1/src/espresso/_pumping_test/_pumping_test.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_simple_regression/LICENCE` & `geo-espresso-0.2.1.dev1/src/espresso/_simple_regression/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_simple_regression/_simple_regression.py` & `geo-espresso-0.2.1.dev1/src/espresso/_simple_regression/_simple_regression.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_slug_test/LICENCE` & `geo-espresso-0.2.1.dev1/src/espresso/_slug_test/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_slug_test/README.md` & `geo-espresso-0.2.1.dev1/src/espresso/_slug_test/README.md`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_slug_test/_slug_test.py` & `geo-espresso-0.2.1.dev1/src/espresso/_slug_test/_slug_test.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_xray_tomography/LICENCE` & `geo-espresso-0.2.1.dev1/src/espresso/_xray_tomography/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_xray_tomography/README.md` & `geo-espresso-0.2.1.dev1/src/espresso/_xray_tomography/README.md`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_xray_tomography/_xray_tomography.py` & `geo-espresso-0.2.1.dev1/src/espresso/_xray_tomography/_xray_tomography.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_xray_tomography/data/csiro_logo.png` & `geo-espresso-0.2.1.dev1/src/espresso/_xray_tomography/data/csiro_logo.png`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_xray_tomography/data/example1.dat` & `geo-espresso-0.2.1.dev1/src/espresso/_xray_tomography/data/example1.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_xray_tomography/data/example2.dat` & `geo-espresso-0.2.1.dev1/src/espresso/_xray_tomography/data/example2.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_xray_tomography/data/example3.dat` & `geo-espresso-0.2.1.dev1/src/espresso/_xray_tomography/data/example3.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/_xray_tomography/data/inlab_logo.png` & `geo-espresso-0.2.1.dev1/src/espresso/_xray_tomography/data/inlab_logo.png`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/exceptions.py` & `geo-espresso-0.2.1.dev1/src/espresso/exceptions.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/utils/__init__.py` & `geo-espresso-0.2.1.dev1/src/espresso/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/espresso/utils/data_loader.py` & `geo-espresso-0.2.1.dev1/src/espresso/utils/data_loader.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.1.dev0/src/geo_espresso.egg-info/PKG-INFO` & `geo-espresso-0.2.1.dev1/src/geo_espresso.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo-espresso
-Version: 0.2.1.dev0
+Version: 0.2.1.dev1
 Summary: Earth Science PRoblems for the Evaluation of Strategies, Solvers and Optimizers
 Author: InLab, Espresso development team
 Keywords: inversion,inference,python package,geoscience,geophysics
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
@@ -16,21 +16,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Fortran
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: Other/Proprietary License
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: doc
 License-File: LICENCE
 
 # Espresso
 
 [![PyPI version](https://img.shields.io/pypi/v/geo-espresso?logo=pypi&style=flat-square&color=bde0fe&labelColor=f8f9fa)](https://pypi.org/project/geo-espresso/)
+[![build](https://img.shields.io/github/actions/workflow/status/inlab-geo/espresso/build_wheels.yml?branch=main&logo=githubactions&style=flat-square&color=ccd5ae&labelColor=f8f9fa)](https://github.com/inlab-geo/espresso/actions/workflows/build_wheels.yml)
 [![Documentation Status](https://img.shields.io/readthedocs/geo-espresso?logo=readthedocs&style=flat-square&color=fed9b7&labelColor=f8f9fa&logoColor=eaac8b)](https://geo-espresso.readthedocs.io/en/latest/?badge=latest)
 [![Slack](https://img.shields.io/badge/Slack-InLab_community-4A154B?logo=slack&style=flat-square&color=cdb4db&labelColor=f8f9fa&logoColor=9c89b8)](https://join.slack.com/t/inlab-community/shared_invite/zt-1ejny069z-v5ZyvP2tDjBR42OAu~TkHg)
 
 ## Introduction
 
 **E**arth **S**cience **PR**oblems for the **E**valuation of **S**trategies, 
 **S**olvers and **O**ptimizers (Espresso) is a collection of datasets, and
```

