# Comparing `tmp/usgs-strec-2.2.6.tar.gz` & `tmp/usgs-strec-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usgs-strec-2.2.6.tar", last modified: Tue Apr 11 15:46:07 2023, max compression
+gzip compressed data, was "usgs-strec-2.2.7.tar", last modified: Wed Apr 12 22:11:20 2023, max compression
```

## Comparing `usgs-strec-2.2.6.tar` & `usgs-strec-2.2.7.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 15:46:07.622855 usgs-strec-2.2.6/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      136 2023-02-27 20:02:54.000000 usgs-strec-2.2.6/.gitignore
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1667 2023-02-27 20:02:54.000000 usgs-strec-2.2.6/.gitlab-ci.yml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      589 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/.travis.yml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      671 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/CONTRIBUTING.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      631 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/DISCLAIMER.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      755 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/LICENSE.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    12026 2023-04-11 15:46:07.622855 usgs-strec-2.2.6/PKG-INFO
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    10781 2023-04-11 15:31:23.000000 usgs-strec-2.2.6/README.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1014 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/code.json
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     2610 2023-04-11 15:31:23.000000 usgs-strec-2.2.6/install.sh
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      318 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/license.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1148 2023-04-11 15:45:56.000000 usgs-strec-2.2.6/pyproject.toml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   710756 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/select_regions.png
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)       38 2023-04-11 15:46:07.622855 usgs-strec-2.2.6/setup.cfg
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 15:46:07.612855 usgs-strec-2.2.6/src/
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 15:46:07.612855 usgs-strec-2.2.6/src/strec/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)        0 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/__init__.py
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 15:46:07.612855 usgs-strec-2.2.6/src/strec/bin/
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     8371 2023-04-11 15:31:23.000000 usgs-strec-2.2.6/src/strec/bin/regcalc.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     8008 2023-02-27 20:02:54.000000 usgs-strec-2.2.6/src/strec/bin/strec_cfg.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9523 2023-04-11 15:31:23.000000 usgs-strec-2.2.6/src/strec/calc.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     3562 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/cmt.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4869 2023-04-11 15:31:23.000000 usgs-strec-2.2.6/src/strec/config.py
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 15:46:07.622855 usgs-strec-2.2.6/src/strec/data/
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)      877 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/data/REGION_GRIDS_README.txt
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)   750725 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/data/active.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    36449 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/data/domains.xlsx
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    95983 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/data/land.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      240 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/data/maximum_interface_depths.csv
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)  6086656 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/data/moment_tensors.db
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)   138345 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/data/ocean.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     6153 2023-04-11 15:31:23.000000 usgs-strec-2.2.6/src/strec/data/select.conf
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1753 2023-04-11 15:31:23.000000 usgs-strec-2.2.6/src/strec/data/selectspec.conf
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)   271186 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/data/stable.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1794 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/data/strec.ini
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   204430 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/data/subduction.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    24246 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/data/volcanic.geojson
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5373 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/database.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3544 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/distance.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     7142 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/gcmt.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3227 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/gmreg.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2639 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/kagan.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9386 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/slab.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    13185 2023-04-11 15:31:23.000000 usgs-strec-2.2.6/src/strec/sm_probs.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4493 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/src/strec/subduction.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    23230 2023-04-11 15:31:23.000000 usgs-strec-2.2.6/src/strec/subtype.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     8163 2023-04-11 15:31:23.000000 usgs-strec-2.2.6/src/strec/utils.py
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 15:46:07.622855 usgs-strec-2.2.6/src/usgs_strec.egg-info/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    12026 2023-04-11 15:46:07.000000 usgs-strec-2.2.6/src/usgs_strec.egg-info/PKG-INFO
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2222 2023-04-11 15:46:07.000000 usgs-strec-2.2.6/src/usgs_strec.egg-info/SOURCES.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)        1 2023-04-11 15:46:07.000000 usgs-strec-2.2.6/src/usgs_strec.egg-info/dependency_links.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)       86 2023-04-11 15:46:07.000000 usgs-strec-2.2.6/src/usgs_strec.egg-info/entry_points.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      292 2023-04-11 15:46:07.000000 usgs-strec-2.2.6/src/usgs_strec.egg-info/requires.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)        6 2023-04-11 15:46:07.000000 usgs-strec-2.2.6/src/usgs_strec.egg-info/top_level.txt
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 15:46:07.612855 usgs-strec-2.2.6/test/
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 15:46:07.612855 usgs-strec-2.2.6/test/src/
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 15:46:07.622855 usgs-strec-2.2.6/test/src/data/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1294 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/data/AMlvPS_trench.json
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    39480 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/data/large_events.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)  6086656 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/data/strec.db
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      404 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/data/test.ndk
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    40865 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/data/test_regimes.xlsx
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 15:46:07.622855 usgs-strec-2.2.6/test/src/strec/
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    10144 2023-04-11 15:31:23.000000 usgs-strec-2.2.6/test/src/strec/calc_test.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     2466 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/strec/cmt_test.py
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-11 15:46:07.622855 usgs-strec-2.2.6/test/src/strec/data/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    49629 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/strec/data/big_focals.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9650 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/strec/data/comcatid_catalog.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9879 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/strec/data/focal_catalog.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9797 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/strec/data/hypocols_catalog.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9646 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/strec/data/id_catalog.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9991 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/strec/data/moment_catalog.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   170434 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/strec/data/nga_matched.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    10154 2023-04-11 15:31:23.000000 usgs-strec-2.2.6/test/src/strec/data/simple_catalog.xlsx
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5325 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/strec/data/subsampled_nga_results.xlsx
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    63437 2023-02-27 20:02:54.000000 usgs-strec-2.2.6/test/src/strec/data/van_slab2_dep_02.23.18.grd
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    62496 2023-02-27 20:02:54.000000 usgs-strec-2.2.6/test/src/strec/data/van_slab2_dip_02.23.18.grd
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    55666 2023-02-27 20:02:54.000000 usgs-strec-2.2.6/test/src/strec/data/van_slab2_str_02.23.18.grd
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    53921 2023-02-27 20:02:54.000000 usgs-strec-2.2.6/test/src/strec/data/van_slab2_thk_02.23.18.grd
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    62608 2023-02-27 20:02:54.000000 usgs-strec-2.2.6/test/src/strec/data/van_slab2_unc_02.23.18.grd
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     2329 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/strec/database_test.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9839 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/strec/distance_test.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     1717 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/strec/gcmt_test.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1729 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/strec/gmreg_test.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     1602 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/strec/kagan_test.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     8109 2023-04-11 15:31:23.000000 usgs-strec-2.2.6/test/src/strec/probs_test.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     1876 2023-02-27 20:02:54.000000 usgs-strec-2.2.6/test/src/strec/slab_test.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     4520 2023-02-27 20:02:06.000000 usgs-strec-2.2.6/test/src/strec/subduction_test.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     8116 2023-04-11 15:31:23.000000 usgs-strec-2.2.6/test/src/strec/subtype_test.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     3562 2023-04-11 15:31:23.000000 usgs-strec-2.2.6/test/src/strec/utils_test.py
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-12 22:11:20.894021 usgs-strec-2.2.7/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      136 2023-02-27 20:02:54.000000 usgs-strec-2.2.7/.gitignore
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1667 2023-02-27 20:02:54.000000 usgs-strec-2.2.7/.gitlab-ci.yml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      589 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/.travis.yml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      671 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/CONTRIBUTING.md
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      631 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/DISCLAIMER.md
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      755 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/LICENSE.md
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    12026 2023-04-12 22:11:20.894021 usgs-strec-2.2.7/PKG-INFO
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    10781 2023-04-11 15:31:23.000000 usgs-strec-2.2.7/README.md
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1014 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/code.json
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     2610 2023-04-11 15:31:23.000000 usgs-strec-2.2.7/install.sh
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      318 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/license.txt
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1148 2023-04-12 21:02:21.000000 usgs-strec-2.2.7/pyproject.toml
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   710756 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/select_regions.png
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)       38 2023-04-12 22:11:20.894021 usgs-strec-2.2.7/setup.cfg
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-12 22:11:20.884021 usgs-strec-2.2.7/src/
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-12 22:11:20.884021 usgs-strec-2.2.7/src/strec/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)        0 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/__init__.py
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-12 22:11:20.884021 usgs-strec-2.2.7/src/strec/bin/
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     8371 2023-04-11 15:31:23.000000 usgs-strec-2.2.7/src/strec/bin/regcalc.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     8152 2023-04-12 20:23:25.000000 usgs-strec-2.2.7/src/strec/bin/strec_cfg.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9523 2023-04-11 15:31:23.000000 usgs-strec-2.2.7/src/strec/calc.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     3562 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/cmt.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4869 2023-04-11 15:31:23.000000 usgs-strec-2.2.7/src/strec/config.py
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-12 22:11:20.894021 usgs-strec-2.2.7/src/strec/data/
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)      877 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/data/REGION_GRIDS_README.txt
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)   750725 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/data/active.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    36449 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/data/domains.xlsx
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    95983 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/data/land.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      240 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/data/maximum_interface_depths.csv
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)  6086656 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/data/moment_tensors.db
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)   138345 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/data/ocean.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     6153 2023-04-11 15:31:23.000000 usgs-strec-2.2.7/src/strec/data/select.conf
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1753 2023-04-11 15:31:23.000000 usgs-strec-2.2.7/src/strec/data/selectspec.conf
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)   271186 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/data/stable.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1794 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/data/strec.ini
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   204430 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/data/subduction.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    24246 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/data/volcanic.geojson
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5461 2023-04-12 20:50:34.000000 usgs-strec-2.2.7/src/strec/database.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3544 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/distance.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     7142 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/gcmt.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3227 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/gmreg.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2639 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/kagan.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9386 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/slab.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    13185 2023-04-11 15:31:23.000000 usgs-strec-2.2.7/src/strec/sm_probs.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4493 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/src/strec/subduction.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    23230 2023-04-11 15:31:23.000000 usgs-strec-2.2.7/src/strec/subtype.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     8163 2023-04-11 15:31:23.000000 usgs-strec-2.2.7/src/strec/utils.py
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-12 22:11:20.894021 usgs-strec-2.2.7/src/usgs_strec.egg-info/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    12026 2023-04-12 22:11:20.000000 usgs-strec-2.2.7/src/usgs_strec.egg-info/PKG-INFO
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2222 2023-04-12 22:11:20.000000 usgs-strec-2.2.7/src/usgs_strec.egg-info/SOURCES.txt
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)        1 2023-04-12 22:11:20.000000 usgs-strec-2.2.7/src/usgs_strec.egg-info/dependency_links.txt
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)       86 2023-04-12 22:11:20.000000 usgs-strec-2.2.7/src/usgs_strec.egg-info/entry_points.txt
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      292 2023-04-12 22:11:20.000000 usgs-strec-2.2.7/src/usgs_strec.egg-info/requires.txt
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)        6 2023-04-12 22:11:20.000000 usgs-strec-2.2.7/src/usgs_strec.egg-info/top_level.txt
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-12 22:11:20.884021 usgs-strec-2.2.7/test/
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-12 22:11:20.884021 usgs-strec-2.2.7/test/src/
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-12 22:11:20.894021 usgs-strec-2.2.7/test/src/data/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1294 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/data/AMlvPS_trench.json
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    39480 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/data/large_events.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)  6086656 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/data/strec.db
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)      404 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/data/test.ndk
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    40865 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/data/test_regimes.xlsx
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-12 22:11:20.894021 usgs-strec-2.2.7/test/src/strec/
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    10144 2023-04-11 15:31:23.000000 usgs-strec-2.2.7/test/src/strec/calc_test.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     2466 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/strec/cmt_test.py
+drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-04-12 22:11:20.894021 usgs-strec-2.2.7/test/src/strec/data/
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    49629 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/strec/data/big_focals.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9650 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/strec/data/comcatid_catalog.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9879 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/strec/data/focal_catalog.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9797 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/strec/data/hypocols_catalog.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9646 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/strec/data/id_catalog.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9991 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/strec/data/moment_catalog.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)   170434 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/strec/data/nga_matched.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)    10154 2023-04-11 15:31:23.000000 usgs-strec-2.2.7/test/src/strec/data/simple_catalog.xlsx
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5325 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/strec/data/subsampled_nga_results.xlsx
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    63437 2023-02-27 20:02:54.000000 usgs-strec-2.2.7/test/src/strec/data/van_slab2_dep_02.23.18.grd
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    62496 2023-02-27 20:02:54.000000 usgs-strec-2.2.7/test/src/strec/data/van_slab2_dip_02.23.18.grd
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    55666 2023-02-27 20:02:54.000000 usgs-strec-2.2.7/test/src/strec/data/van_slab2_str_02.23.18.grd
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    53921 2023-02-27 20:02:54.000000 usgs-strec-2.2.7/test/src/strec/data/van_slab2_thk_02.23.18.grd
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)    62608 2023-02-27 20:02:54.000000 usgs-strec-2.2.7/test/src/strec/data/van_slab2_unc_02.23.18.grd
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     2329 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/strec/database_test.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9839 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/strec/distance_test.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     1717 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/strec/gcmt_test.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1729 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/strec/gmreg_test.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     1602 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/strec/kagan_test.py
+-rw-r--r--   0 mhearne   (1000) mhearne   (1000)     8109 2023-04-11 15:31:23.000000 usgs-strec-2.2.7/test/src/strec/probs_test.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     1876 2023-02-27 20:02:54.000000 usgs-strec-2.2.7/test/src/strec/slab_test.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     4520 2023-02-27 20:02:06.000000 usgs-strec-2.2.7/test/src/strec/subduction_test.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     8116 2023-04-11 15:31:23.000000 usgs-strec-2.2.7/test/src/strec/subtype_test.py
+-rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     3562 2023-04-11 15:31:23.000000 usgs-strec-2.2.7/test/src/strec/utils_test.py
```

### Comparing `usgs-strec-2.2.6/.gitlab-ci.yml` & `usgs-strec-2.2.7/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/.travis.yml` & `usgs-strec-2.2.7/.travis.yml`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/CONTRIBUTING.md` & `usgs-strec-2.2.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/DISCLAIMER.md` & `usgs-strec-2.2.7/DISCLAIMER.md`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/LICENSE.md` & `usgs-strec-2.2.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/PKG-INFO` & `usgs-strec-2.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usgs-strec
-Version: 2.2.6
+Version: 2.2.7
 Summary: USGS SeismoTectonic Regime Earthquake Calculator (STREC)
 Author-email: Mike Hearne <mhearne@usgs.gov>, Eric Thompson <ethompson@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United
         States because it contains materials that originally came from the United
```

### Comparing `usgs-strec-2.2.6/README.md` & `usgs-strec-2.2.7/README.md`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/code.json` & `usgs-strec-2.2.7/code.json`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/install.sh` & `usgs-strec-2.2.7/install.sh`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/pyproject.toml` & `usgs-strec-2.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "usgs-strec"
-version = "2.2.6"
+version = "2.2.7"
 description = "USGS SeismoTectonic Regime Earthquake Calculator (STREC)"
 authors = [
     {name = "Mike Hearne", email="mhearne@usgs.gov"},
     {name = "Eric Thompson", email="ethompson@usgs.gov"},
 ]
 
 license = {file = "LICENSE.md"}
```

### Comparing `usgs-strec-2.2.6/select_regions.png` & `usgs-strec-2.2.7/select_regions.png`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/src/strec/bin/regcalc.py` & `usgs-strec-2.2.7/src/strec/bin/regcalc.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/src/strec/bin/strec_cfg.py` & `usgs-strec-2.2.7/src/strec/bin/strec_cfg.py`

 * *Files 3% similar despite different names*

```diff
@@ -251,18 +251,22 @@
             source = "GCMT"
             stash_dataframe(gcmt_dataframe, dbfile, source, create_db=True)
         except Exception as e:
             gcmt_msg = f"Failed to download GCMT data: {str(e)}"
             messages.append(gcmt_msg)
 
     if moment_data:
+        dbfile = pathlib.Path(config["DATA"]["dbfile"])
+        create_db = True
+        if dbfile.exists():
+            create_db = False
         try:
             moment_dataframe = read_datafile(moment_data)
             stash_dataframe(
-                moment_dataframe, dbfile, moment_data_source, create_db=True
+                moment_dataframe, dbfile, moment_data_source, create_db=create_db
             )
         except Exception as e:
             moment_msg = f"Could not parse moment datafile {moment_data}: {str(e)}"
             messages.append(moment_msg)
     if len(messages):
         print("Errors were encountered during the course of downloading/loading data:")
         for message in messages:
```

### Comparing `usgs-strec-2.2.6/src/strec/calc.py` & `usgs-strec-2.2.7/src/strec/calc.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/src/strec/cmt.py` & `usgs-strec-2.2.7/src/strec/cmt.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/src/strec/config.py` & `usgs-strec-2.2.7/src/strec/config.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/src/strec/data/REGION_GRIDS_README.txt` & `usgs-strec-2.2.7/src/strec/data/REGION_GRIDS_README.txt`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/src/strec/data/active.geojson` & `usgs-strec-2.2.7/src/strec/data/active.geojson`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/src/strec/data/domains.xlsx` & `usgs-strec-2.2.7/src/strec/data/domains.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/src/strec/data/land.geojson` & `usgs-strec-2.2.7/src/strec/data/land.geojson`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/src/strec/data/moment_tensors.db` & `usgs-strec-2.2.7/src/strec/data/moment_tensors.db`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/src/strec/data/ocean.geojson` & `usgs-strec-2.2.7/src/strec/data/ocean.geojson`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/src/strec/data/select.conf` & `usgs-strec-2.2.7/src/strec/data/select.conf`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/src/strec/data/selectspec.conf` & `usgs-strec-2.2.7/src/strec/data/selectspec.conf`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/src/strec/data/stable.geojson` & `usgs-strec-2.2.7/src/strec/data/stable.geojson`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/src/strec/data/strec.ini` & `usgs-strec-2.2.7/src/strec/data/strec.ini`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/src/strec/data/subduction.geojson` & `usgs-strec-2.2.7/src/strec/data/subduction.geojson`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/src/strec/data/volcanic.geojson` & `usgs-strec-2.2.7/src/strec/data/volcanic.geojson`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/src/strec/database.py` & `usgs-strec-2.2.7/src/strec/database.py`

 * *Files 5% similar despite different names*

```diff
@@ -127,14 +127,15 @@
         cursor.execute('INSERT INTO source (source) values ("%s")' % source.lower())
         conn.commit()
         cursor.execute('SELECT id from source where source = "%s"' % source.lower())
         sourceid = cursor.fetchone()[0]
         dataframe["sourceid"] = sourceid
 
     dataframe.to_sql("earthquake", conn, if_exists="append", index=False)
+    print(f"Inserted {len(dataframe)} records from {source} into database {datafile}")
 
     conn.close()
 
 
 def fetch_dataframe(datafile):
     """Return a pandas dataframe containing earthquake information.
 
@@ -163,13 +164,14 @@
     # get the data source information
     dataframe["source"] = ""
     usources = dataframe["sourceid"].unique()
     for source in usources:
         cursor.execute("SELECT source FROM source WHERE id=%i" % source)
         tsource = cursor.fetchone()[0]
         rowidx = dataframe["sourceid"] == source
+
         dataframe.loc[rowidx, "source"] = tsource
 
     dataframe.drop("sourceid", axis=1, inplace=True)
 
     conn.close()
     return dataframe
```

### Comparing `usgs-strec-2.2.6/src/strec/distance.py` & `usgs-strec-2.2.7/src/strec/distance.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/src/strec/gcmt.py` & `usgs-strec-2.2.7/src/strec/gcmt.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/src/strec/gmreg.py` & `usgs-strec-2.2.7/src/strec/gmreg.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/src/strec/kagan.py` & `usgs-strec-2.2.7/src/strec/kagan.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/src/strec/slab.py` & `usgs-strec-2.2.7/src/strec/slab.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/src/strec/sm_probs.py` & `usgs-strec-2.2.7/src/strec/sm_probs.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/src/strec/subduction.py` & `usgs-strec-2.2.7/src/strec/subduction.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/src/strec/subtype.py` & `usgs-strec-2.2.7/src/strec/subtype.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/src/strec/utils.py` & `usgs-strec-2.2.7/src/strec/utils.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/src/usgs_strec.egg-info/PKG-INFO` & `usgs-strec-2.2.7/src/usgs_strec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usgs-strec
-Version: 2.2.6
+Version: 2.2.7
 Summary: USGS SeismoTectonic Regime Earthquake Calculator (STREC)
 Author-email: Mike Hearne <mhearne@usgs.gov>, Eric Thompson <ethompson@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United
         States because it contains materials that originally came from the United
```

### Comparing `usgs-strec-2.2.6/src/usgs_strec.egg-info/SOURCES.txt` & `usgs-strec-2.2.7/src/usgs_strec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/test/src/data/AMlvPS_trench.json` & `usgs-strec-2.2.7/test/src/data/AMlvPS_trench.json`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/test/src/data/large_events.xlsx` & `usgs-strec-2.2.7/test/src/data/large_events.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/test/src/data/strec.db` & `usgs-strec-2.2.7/test/src/data/strec.db`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/test/src/data/test_regimes.xlsx` & `usgs-strec-2.2.7/test/src/data/test_regimes.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/test/src/strec/calc_test.py` & `usgs-strec-2.2.7/test/src/strec/calc_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/test/src/strec/cmt_test.py` & `usgs-strec-2.2.7/test/src/strec/cmt_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/test/src/strec/data/big_focals.xlsx` & `usgs-strec-2.2.7/test/src/strec/data/big_focals.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/test/src/strec/data/comcatid_catalog.xlsx` & `usgs-strec-2.2.7/test/src/strec/data/comcatid_catalog.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/test/src/strec/data/focal_catalog.xlsx` & `usgs-strec-2.2.7/test/src/strec/data/focal_catalog.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/test/src/strec/data/hypocols_catalog.xlsx` & `usgs-strec-2.2.7/test/src/strec/data/hypocols_catalog.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/test/src/strec/data/id_catalog.xlsx` & `usgs-strec-2.2.7/test/src/strec/data/id_catalog.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/test/src/strec/data/moment_catalog.xlsx` & `usgs-strec-2.2.7/test/src/strec/data/moment_catalog.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/test/src/strec/data/nga_matched.xlsx` & `usgs-strec-2.2.7/test/src/strec/data/nga_matched.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/test/src/strec/data/simple_catalog.xlsx` & `usgs-strec-2.2.7/test/src/strec/data/simple_catalog.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/test/src/strec/data/subsampled_nga_results.xlsx` & `usgs-strec-2.2.7/test/src/strec/data/subsampled_nga_results.xlsx`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/test/src/strec/data/van_slab2_dep_02.23.18.grd` & `usgs-strec-2.2.7/test/src/strec/data/van_slab2_dep_02.23.18.grd`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/test/src/strec/data/van_slab2_dip_02.23.18.grd` & `usgs-strec-2.2.7/test/src/strec/data/van_slab2_dip_02.23.18.grd`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/test/src/strec/data/van_slab2_str_02.23.18.grd` & `usgs-strec-2.2.7/test/src/strec/data/van_slab2_str_02.23.18.grd`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/test/src/strec/data/van_slab2_thk_02.23.18.grd` & `usgs-strec-2.2.7/test/src/strec/data/van_slab2_thk_02.23.18.grd`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/test/src/strec/data/van_slab2_unc_02.23.18.grd` & `usgs-strec-2.2.7/test/src/strec/data/van_slab2_unc_02.23.18.grd`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/test/src/strec/database_test.py` & `usgs-strec-2.2.7/test/src/strec/database_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/test/src/strec/distance_test.py` & `usgs-strec-2.2.7/test/src/strec/distance_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/test/src/strec/gcmt_test.py` & `usgs-strec-2.2.7/test/src/strec/gcmt_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/test/src/strec/gmreg_test.py` & `usgs-strec-2.2.7/test/src/strec/gmreg_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/test/src/strec/kagan_test.py` & `usgs-strec-2.2.7/test/src/strec/kagan_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/test/src/strec/probs_test.py` & `usgs-strec-2.2.7/test/src/strec/probs_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/test/src/strec/slab_test.py` & `usgs-strec-2.2.7/test/src/strec/slab_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/test/src/strec/subduction_test.py` & `usgs-strec-2.2.7/test/src/strec/subduction_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/test/src/strec/subtype_test.py` & `usgs-strec-2.2.7/test/src/strec/subtype_test.py`

 * *Files identical despite different names*

### Comparing `usgs-strec-2.2.6/test/src/strec/utils_test.py` & `usgs-strec-2.2.7/test/src/strec/utils_test.py`

 * *Files identical despite different names*

