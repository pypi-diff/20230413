# Comparing `tmp/dkist-processing-pac-2.0.0rc5.tar.gz` & `tmp/dkist-processing-pac-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-pac-2.0.0rc5.tar", last modified: Tue Mar 21 21:39:14 2023, max compression
+gzip compressed data, was "dkist-processing-pac-2.1.0.tar", last modified: Wed Apr 12 22:06:22 2023, max compression
```

## Comparing `dkist-processing-pac-2.0.0rc5.tar` & `dkist-processing-pac-2.1.0.tar`

### file list

```diff
@@ -1,86 +1,80 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-21 21:39:14.342896 dkist-processing-pac-2.0.0rc5/
--rw-rw-rw-   0 root         (0) root         (0)      714 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      906 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      306 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/.readthedocs.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3652 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     3547 2023-03-21 21:39:14.342896 dkist-processing-pac-2.0.0rc5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3042 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2346 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-21 21:39:14.338895 dkist-processing-pac-2.0.0rc5/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)      115 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/changelog/16.misc.rst
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/changelog/17.feature.rst
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/changelog/18.bugfix.rst
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/changelog/19.bugfix.rst
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/changelog/20.feature.rst
--rw-rw-rw-   0 root         (0) root         (0)      388 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/changelog/21.bugfix.rst
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-21 21:39:14.338895 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-21 21:39:14.338895 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-21 21:39:14.338895 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/CS_files/
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/CS_files/aggressive_CS.txt
--rw-rw-rw-   0 root         (0) root         (0)      763 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/CS_files/asp16_CS.txt
--rw-rw-rw-   0 root         (0) root         (0)      289 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/CS_files/efficient_CS.txt
--rw-rw-rw-   0 root         (0) root         (0)      223 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/CS_files/may_CS.txt
--rw-rw-rw-   0 root         (0) root         (0)      255 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/constants.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-21 21:39:14.338895 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/fit_modes/
--rw-rw-rw-   0 root         (0) root         (0)      376 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/fit_modes/M12_fitUV.yml
--rw-rw-rw-   0 root         (0) root         (0)      378 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/fit_modes/baseline.yml
--rw-rw-rw-   0 root         (0) root         (0)      376 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/fit_modes/fit_QUV.yml
--rw-rw-rw-   0 root         (0) root         (0)      379 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/fit_modes/no_T.yml
--rw-rw-rw-   0 root         (0) root         (0)      377 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/fit_modes/use_M12.yml
--rw-rw-rw-   0 root         (0) root         (0)      378 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/fit_modes/use_M12_I_sys_per_step.yml
--rw-rw-rw-   0 root         (0) root         (0)      375 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/fit_modes/use_M12_globalRet_globalTrans.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-21 21:39:14.342896 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/init_values/
--rw-rw-rw-   0 root         (0) root         (0)   284469 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/init_values/OCCal_VIS_cu_pars.asdf
--rw-rw-rw-   0 root         (0) root         (0)   192191 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/init_values/OCCal_VIS_tm_pars.asdf
--rw-rw-rw-   0 root         (0) root         (0)    32177 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/py_table.txt
--rw-rw-rw-   0 root         (0) root         (0)   306602 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/telescope_db.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-21 21:39:14.342896 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/fitter/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/fitter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15220 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/fitter/fitter_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     5017 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/fitter/fitting_core.py
--rw-rw-rw-   0 root         (0) root         (0)     9110 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/fitter/polcal_fitter.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-21 21:39:14.342896 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/input_data/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/input_data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10286 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/input_data/drawer.py
--rw-rw-rw-   0 root         (0) root         (0)     6161 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/input_data/dresser.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-21 21:39:14.342896 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/optics/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/optics/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11414 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/optics/calibration_unit.py
--rw-rw-rw-   0 root         (0) root         (0)     3383 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/optics/mueller_matrices.py
--rw-rw-rw-   0 root         (0) root         (0)    12300 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/optics/telescope.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-21 21:39:14.342896 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/
--rw-rw-rw-   0 root         (0) root         (0)      121 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15374 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     7793 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/test_calibration_unit.py
--rw-rw-rw-   0 root         (0) root         (0)     7639 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/test_drawer.py
--rw-rw-rw-   0 root         (0) root         (0)     4587 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/test_dresser.py
--rw-rw-rw-   0 root         (0) root         (0)     9205 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/test_fitter_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/test_mueller_matrices.py
--rw-rw-rw-   0 root         (0) root         (0)     2107 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/test_nd_parameter_array.py
--rw-rw-rw-   0 root         (0) root         (0)     3571 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/test_polcal_fitter.py
--rw-rw-rw-   0 root         (0) root         (0)    15571 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/test_telescope.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-21 21:39:14.338895 dkist-processing-pac-2.0.0rc5/dkist_processing_pac.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     3547 2023-03-21 21:39:14.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2558 2023-03-21 21:39:14.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-03-21 21:39:14.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-03-21 21:39:14.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-03-21 21:39:14.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-21 21:39:14.342896 dkist-processing-pac-2.0.0rc5/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     5571 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/docs/background.rst
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1831 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      125 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     8458 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/docs/layout.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/docs/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-21 21:39:14.342896 dkist-processing-pac-2.0.0rc5/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1461 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      162 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/licenses/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1182 2023-03-21 21:39:14.346896 dkist-processing-pac-2.0.0rc5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      102 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 22:06:22.876697 dkist-processing-pac-2.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)      714 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      906 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      306 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/.readthedocs.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     5625 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3544 2023-04-12 22:06:22.880697 dkist-processing-pac-2.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3042 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2346 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 22:06:22.872697 dkist-processing-pac-2.1.0/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/changelog/.gitempty
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 22:06:22.872697 dkist-processing-pac-2.1.0/dkist_processing_pac/
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 22:06:22.872697 dkist-processing-pac-2.1.0/dkist_processing_pac/data/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 22:06:22.872697 dkist-processing-pac-2.1.0/dkist_processing_pac/data/CS_files/
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/data/CS_files/aggressive_CS.txt
+-rw-rw-rw-   0 root         (0) root         (0)      763 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/data/CS_files/asp16_CS.txt
+-rw-rw-rw-   0 root         (0) root         (0)      289 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/data/CS_files/efficient_CS.txt
+-rw-rw-rw-   0 root         (0) root         (0)      223 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/data/CS_files/may_CS.txt
+-rw-rw-rw-   0 root         (0) root         (0)      255 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/data/constants.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 22:06:22.872697 dkist-processing-pac-2.1.0/dkist_processing_pac/data/fit_modes/
+-rw-rw-rw-   0 root         (0) root         (0)      376 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/data/fit_modes/M12_fitUV.yml
+-rw-rw-rw-   0 root         (0) root         (0)      378 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/data/fit_modes/baseline.yml
+-rw-rw-rw-   0 root         (0) root         (0)      376 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/data/fit_modes/fit_QUV.yml
+-rw-rw-rw-   0 root         (0) root         (0)      379 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/data/fit_modes/no_T.yml
+-rw-rw-rw-   0 root         (0) root         (0)      377 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/data/fit_modes/use_M12.yml
+-rw-rw-rw-   0 root         (0) root         (0)      378 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/data/fit_modes/use_M12_I_sys_per_step.yml
+-rw-rw-rw-   0 root         (0) root         (0)      375 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/data/fit_modes/use_M12_globalRet_globalTrans.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 22:06:22.876697 dkist-processing-pac-2.1.0/dkist_processing_pac/data/init_values/
+-rw-rw-rw-   0 root         (0) root         (0)   284469 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/data/init_values/OCCal_VIS_cu_pars.asdf
+-rw-rw-rw-   0 root         (0) root         (0)   192191 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/data/init_values/OCCal_VIS_tm_pars.asdf
+-rw-rw-rw-   0 root         (0) root         (0)    32177 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/data/py_table.txt
+-rw-rw-rw-   0 root         (0) root         (0)   306602 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/data/telescope_db.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 22:06:22.876697 dkist-processing-pac-2.1.0/dkist_processing_pac/fitter/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/fitter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15220 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/fitter/fitter_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     5017 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/fitter/fitting_core.py
+-rw-rw-rw-   0 root         (0) root         (0)     9110 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/fitter/polcal_fitter.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 22:06:22.876697 dkist-processing-pac-2.1.0/dkist_processing_pac/input_data/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/input_data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10286 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/input_data/drawer.py
+-rw-rw-rw-   0 root         (0) root         (0)     6161 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/input_data/dresser.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 22:06:22.876697 dkist-processing-pac-2.1.0/dkist_processing_pac/optics/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/optics/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11414 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/optics/calibration_unit.py
+-rw-rw-rw-   0 root         (0) root         (0)     3383 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/optics/mueller_matrices.py
+-rw-rw-rw-   0 root         (0) root         (0)    12300 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/optics/telescope.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 22:06:22.876697 dkist-processing-pac-2.1.0/dkist_processing_pac/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15374 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     7793 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/tests/test_calibration_unit.py
+-rw-rw-rw-   0 root         (0) root         (0)     7639 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/tests/test_drawer.py
+-rw-rw-rw-   0 root         (0) root         (0)     4587 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/tests/test_dresser.py
+-rw-rw-rw-   0 root         (0) root         (0)     9205 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/tests/test_fitter_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/tests/test_mueller_matrices.py
+-rw-rw-rw-   0 root         (0) root         (0)     2107 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/tests/test_nd_parameter_array.py
+-rw-rw-rw-   0 root         (0) root         (0)     3571 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/tests/test_polcal_fitter.py
+-rw-rw-rw-   0 root         (0) root         (0)    15571 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/dkist_processing_pac/tests/test_telescope.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 22:06:22.872697 dkist-processing-pac-2.1.0/dkist_processing_pac.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     3544 2023-04-12 22:06:22.000000 dkist-processing-pac-2.1.0/dkist_processing_pac.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2414 2023-04-12 22:06:22.000000 dkist-processing-pac-2.1.0/dkist_processing_pac.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-12 22:06:22.000000 dkist-processing-pac-2.1.0/dkist_processing_pac.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-04-12 22:06:22.000000 dkist-processing-pac-2.1.0/dkist_processing_pac.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-12 22:06:22.000000 dkist-processing-pac-2.1.0/dkist_processing_pac.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 22:06:22.876697 dkist-processing-pac-2.1.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     5821 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/docs/background.rst
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1831 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      125 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8458 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/docs/layout.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/docs/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-12 22:06:22.876697 dkist-processing-pac-2.1.0/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      162 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/licenses/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2023-04-12 22:06:22.880697 dkist-processing-pac-2.1.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      102 2023-04-12 22:06:17.000000 dkist-processing-pac-2.1.0/setup.py
```

### Comparing `dkist-processing-pac-2.0.0rc5/.gitignore` & `dkist-processing-pac-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc5/.pre-commit-config.yaml` & `dkist-processing-pac-2.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc5/PKG-INFO` & `dkist-processing-pac-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-pac
-Version: 2.0.0rc5
+Version: 2.1.0
 Summary: PA&C Pipeline
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-pac/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: unknown
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/pac
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-pac-2.0.0rc5/README.rst` & `dkist-processing-pac-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc5/bitbucket-pipelines.yml` & `dkist-processing-pac-2.1.0/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc5/check_changelog_updated.sh` & `dkist-processing-pac-2.1.0/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/CS_files/asp16_CS.txt` & `dkist-processing-pac-2.1.0/dkist_processing_pac/data/CS_files/asp16_CS.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/init_values/OCCal_VIS_cu_pars.asdf` & `dkist-processing-pac-2.1.0/dkist_processing_pac/data/init_values/OCCal_VIS_cu_pars.asdf`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/init_values/OCCal_VIS_tm_pars.asdf` & `dkist-processing-pac-2.1.0/dkist_processing_pac/data/init_values/OCCal_VIS_tm_pars.asdf`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/py_table.txt` & `dkist-processing-pac-2.1.0/dkist_processing_pac/data/py_table.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/telescope_db.txt` & `dkist-processing-pac-2.1.0/dkist_processing_pac/data/telescope_db.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/fitter/fitter_parameters.py` & `dkist-processing-pac-2.1.0/dkist_processing_pac/fitter/fitter_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/fitter/fitting_core.py` & `dkist-processing-pac-2.1.0/dkist_processing_pac/fitter/fitting_core.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/fitter/polcal_fitter.py` & `dkist-processing-pac-2.1.0/dkist_processing_pac/fitter/polcal_fitter.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/input_data/drawer.py` & `dkist-processing-pac-2.1.0/dkist_processing_pac/input_data/drawer.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/input_data/dresser.py` & `dkist-processing-pac-2.1.0/dkist_processing_pac/input_data/dresser.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/optics/calibration_unit.py` & `dkist-processing-pac-2.1.0/dkist_processing_pac/optics/calibration_unit.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/optics/mueller_matrices.py` & `dkist-processing-pac-2.1.0/dkist_processing_pac/optics/mueller_matrices.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/optics/telescope.py` & `dkist-processing-pac-2.1.0/dkist_processing_pac/optics/telescope.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
 def compute_coordinate_transform_angle(time) -> float:
     """Calculate the angle needed to transform data into a coordinate frame that matches SDO and HINODE.
 
     This angle rotates the DKIST +Q direction (which is nominally aligned with the altitude axis of the telescope) so it
     is oriented perpendicular to the solar meridian.
 
-    The required angle is the solar orientation angle (i.e., the parallactic angle + Sun P angle) minus 90 degrees.
+    The required angle is the solar orientation angle (i.e., the parallactic angle - Sun P angle) minus 90 degrees.
 
     All angles are in radians.
 
     Parameters
     ----------
     time : astropy.time.Time
         The absolute date/time at which to compute the orientation angle
```

### Comparing `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/conftest.py` & `dkist-processing-pac-2.1.0/dkist_processing_pac/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/test_calibration_unit.py` & `dkist-processing-pac-2.1.0/dkist_processing_pac/tests/test_calibration_unit.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/test_drawer.py` & `dkist-processing-pac-2.1.0/dkist_processing_pac/tests/test_drawer.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/test_dresser.py` & `dkist-processing-pac-2.1.0/dkist_processing_pac/tests/test_dresser.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/test_fitter_parameters.py` & `dkist-processing-pac-2.1.0/dkist_processing_pac/tests/test_fitter_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/test_nd_parameter_array.py` & `dkist-processing-pac-2.1.0/dkist_processing_pac/tests/test_nd_parameter_array.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/test_polcal_fitter.py` & `dkist-processing-pac-2.1.0/dkist_processing_pac/tests/test_polcal_fitter.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/test_telescope.py` & `dkist-processing-pac-2.1.0/dkist_processing_pac/tests/test_telescope.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc5/dkist_processing_pac.egg-info/PKG-INFO` & `dkist-processing-pac-2.1.0/dkist_processing_pac.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-pac
-Version: 2.0.0rc5
+Version: 2.1.0
 Summary: PA&C Pipeline
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-pac/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: unknown
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/pac
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-pac-2.0.0rc5/dkist_processing_pac.egg-info/SOURCES.txt` & `dkist-processing-pac-2.1.0/dkist_processing_pac.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,14 @@
 README.rst
 bitbucket-pipelines.yml
 check_changelog_updated.sh
 pyproject.toml
 setup.cfg
 setup.py
 changelog/.gitempty
-changelog/16.misc.rst
-changelog/17.feature.rst
-changelog/18.bugfix.rst
-changelog/19.bugfix.rst
-changelog/20.feature.rst
-changelog/21.bugfix.rst
 dkist_processing_pac/__init__.py
 dkist_processing_pac.egg-info/PKG-INFO
 dkist_processing_pac.egg-info/SOURCES.txt
 dkist_processing_pac.egg-info/dependency_links.txt
 dkist_processing_pac.egg-info/requires.txt
 dkist_processing_pac.egg-info/top_level.txt
 dkist_processing_pac/data/__init__.py
```

### Comparing `dkist-processing-pac-2.0.0rc5/docs/Makefile` & `dkist-processing-pac-2.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc5/docs/background.rst` & `dkist-processing-pac-2.1.0/docs/background.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 Background
 ==========
 
+**NOTE:** This goal of this page is to provide a basic understanding of how DKIST approaches polarization calibration.
+For a more detailed explanation please see `Harrington et al. (2023) <https://link.springer.com/article/10.1007/s11207-022-02101-6>`_.
+
 An input Stokes vector that has traveled through DKIST down to the entrance of the Coude lab can be described as
 :math:`\vec{S}_{coud\acute{e}} = \mathbf{M}_{36} \mathbf{M}_{12} \vec{S}_{in}`, where :math:`\mathbf{M}_{12}`
 is a combination of the Mueller matrices for mirrors 1 and 2 (primary and secondary), and :math:`\mathbf{M}_{36}`,
 is the same for mirrors 3 - 6. The reason for grouping them together like this will become clear later. Also note that
 some rotation matrices have been omitted, but the general concept is correct.
 
 Once light enters the Coude lab it bounces off a bunch of mirrors and goes through an instrument optic that is
@@ -32,15 +35,15 @@
   :label: full
 
 Fortunately we already know what :math:`\mathbf{M}_{12}` and :math:`\mathbf{M}_{36}` are because we measured them in a
 lab, so if we know :math:`\mathbf{O}` then we’re set…
 
 The Rol of PolCal Data
 ----------------------
-…Unfortunately we don’t. We have a pretty damn good idea, but instruments change often enough that :math:`\mathbf{O}`
+…Unfortunately we don’t. We have a pretty good idea, but instruments change often enough that :math:`\mathbf{O}`
 needs to be computed every time science data are acquired. To do this we take PolCal data. During this task type the
 **Calibration Unit** (CU) is inserted in the GOS between mirrors 2 and 3. The CU has a bunch of optics that can change
 the polarization state of light and these optics are inserted into the beam in a series of steps. The full set of different CU
 configurations is called a **Calibration Sequence** (CS). The light path now looks like this:
 
 .. math::
   \vec{I}_{obs, i} = \mathbf{O}\ \mathbf{M}_{36}\ \mathbf{C}_i\ \mathbf{M}_{12} \vec{S}_{in},
```

### Comparing `dkist-processing-pac-2.0.0rc5/docs/conf.py` & `dkist-processing-pac-2.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc5/docs/layout.rst` & `dkist-processing-pac-2.1.0/docs/layout.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc5/docs/make.bat` & `dkist-processing-pac-2.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc5/licenses/LICENSE.rst` & `dkist-processing-pac-2.1.0/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc5/pyproject.toml` & `dkist-processing-pac-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc5/setup.cfg` & `dkist-processing-pac-2.1.0/setup.cfg`

 * *Files identical despite different names*

