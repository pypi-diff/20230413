# Comparing `tmp/gnssrefl-1.3.3.tar.gz` & `tmp/gnssrefl-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnssrefl-1.3.3.tar", last modified: Thu Apr 13 07:42:59 2023, max compression
+gzip compressed data, was "gnssrefl-1.3.4.tar", last modified: Thu Apr 13 15:12:09 2023, max compression
```

## Comparing `gnssrefl-1.3.3.tar` & `gnssrefl-1.3.4.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:42:59.039011 gnssrefl-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-13 07:42:59.039011 gnssrefl-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:42:59.011011 gnssrefl-1.3.3/gnssrefl/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/EGM96.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/check_rinex.py
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/check_rinex2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/computemp1mp2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19095 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/daily_avg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/daily_avg_cl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:42:59.015010 gnssrefl-1.3.3/gnssrefl/data/
--rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/data/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/download_ioc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/download_noaa.py
--rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/download_orbits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/download_psmsl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/download_rinex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/download_teqc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/download_tides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/download_unr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/download_wsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/felipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/filesizes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15934 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/gnssir.py
--rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/gnssir_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    50572 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/gnsssnr.f
--rw-r--r--   0 runner    (1001) docker     (123)    50579 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/gnsssnrbigger.f
--rw-r--r--   0 runner    (1001) docker     (123)   174545 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/gps.py
--rw-r--r--   0 runner    (1001) docker     (123)    40525 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/gpssnr.f
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/gpsweek.py
--rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/highrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/installexe_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10528 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/invsnr_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/invsnr_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    23530 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/karnak_libraries.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/kelly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/llh2xyz.py
--rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/make_json_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    22560 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/nmea2snr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/nmea2snr_cl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34269 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/phase_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/pickle_dilemma.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/prn2gps.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/query_unr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/quickLook_cl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19809 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/quickLook_function.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5879 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/quickPhase.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19480 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/quickPhase_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/quickplt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/read_snr_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    16511 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/refl_zones.py
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/refl_zones_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/refraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/rh_plot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49162 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/rinex2snr.py
--rw-r--r--   0 runner    (1001) docker     (123)    15472 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/rinex2snr_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/rinex3_rinex2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/rinex3_snr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24490 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/rinpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/rt_rinex3_snr.py
--rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/snow_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/snowdepth_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    60155 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/spline_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    58660 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/subdaily.py
--rw-r--r--   0 runner    (1001) docker     (123)     9554 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/subdaily_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/veg_multiyr.py
--rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/vwc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/vwc_input.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/xyz2llh.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/ydoy.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/ymd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:42:59.015010 gnssrefl-1.3.3/gnssrefl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-13 07:42:58.000000 gnssrefl-1.3.3/gnssrefl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-13 07:42:58.000000 gnssrefl-1.3.3/gnssrefl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 07:42:58.000000 gnssrefl-1.3.3/gnssrefl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-13 07:42:58.000000 gnssrefl-1.3.3/gnssrefl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 07:42:58.000000 gnssrefl-1.3.3/gnssrefl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 07:42:58.000000 gnssrefl-1.3.3/gnssrefl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 07:42:59.039011 gnssrefl-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:42:59.039011 gnssrefl-1.3.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/test/test_gps.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/test/test_rinex2snr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:12:09.532938 gnssrefl-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-13 15:12:09.532938 gnssrefl-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:12:09.508937 gnssrefl-1.3.4/gnssrefl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/EGM96.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/check_rinex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/check_rinex2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/computemp1mp2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19095 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/daily_avg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/daily_avg_cl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:12:09.508937 gnssrefl-1.3.4/gnssrefl/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/data/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/download_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/download_noaa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/download_orbits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/download_psmsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/download_rinex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/download_teqc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/download_tides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/download_unr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/download_wsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/felipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/filesizes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15934 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/gnssir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/gnssir_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50572 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/gnsssnr.f
+-rw-r--r--   0 runner    (1001) docker     (123)    50579 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/gnsssnrbigger.f
+-rw-r--r--   0 runner    (1001) docker     (123)   174546 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40525 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/gpssnr.f
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/gpsweek.py
+-rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/highrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/installexe_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10528 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/invsnr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/invsnr_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23471 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/karnak_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/kelly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/llh2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/make_json_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22560 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/nmea2snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/nmea2snr_cl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34269 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/phase_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/pickle_dilemma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/prn2gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/query_unr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/quickLook_cl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19809 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/quickLook_function.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5879 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/quickPhase.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19480 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/quickPhase_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/quickplt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/read_snr_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16511 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/refl_zones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/refl_zones_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/refraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/rh_plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49164 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/rinex2snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/rinex2snr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/rinex3_rinex2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/rinex3_snr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24490 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/rinpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/rt_rinex3_snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/snow_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/snowdepth_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60155 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/spline_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58660 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/subdaily.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9554 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/subdaily_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/veg_multiyr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/vwc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/vwc_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/xyz2llh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/ydoy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/gnssrefl/ymd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:12:09.508937 gnssrefl-1.3.4/gnssrefl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-13 15:12:09.000000 gnssrefl-1.3.4/gnssrefl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-13 15:12:09.000000 gnssrefl-1.3.4/gnssrefl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:12:09.000000 gnssrefl-1.3.4/gnssrefl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-13 15:12:09.000000 gnssrefl-1.3.4/gnssrefl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 15:12:09.000000 gnssrefl-1.3.4/gnssrefl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 15:12:09.000000 gnssrefl-1.3.4/gnssrefl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 15:12:09.532938 gnssrefl-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:12:09.532938 gnssrefl-1.3.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/test/test_gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-13 15:11:55.000000 gnssrefl-1.3.4/test/test_rinex2snr.py
```

### Comparing `gnssrefl-1.3.3/LICENSE` & `gnssrefl-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/PKG-INFO` & `gnssrefl-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 1.3.3
+Version: 1.3.4
 Summary: A GNSS reflectometry software package 
 Home-page: https://github.com/kristinemlarson/gnssrefl/
 Author: Kristine Larson
 Author-email: kristinem.larson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `gnssrefl-1.3.3/README.md` & `gnssrefl-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/EGM96.py` & `gnssrefl-1.3.4/gnssrefl/EGM96.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/check_rinex.py` & `gnssrefl-1.3.4/gnssrefl/check_rinex.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/check_rinex2.py` & `gnssrefl-1.3.4/gnssrefl/check_rinex2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/computemp1mp2.py` & `gnssrefl-1.3.4/gnssrefl/computemp1mp2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/daily_avg.py` & `gnssrefl-1.3.4/gnssrefl/daily_avg.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/daily_avg_cl.py` & `gnssrefl-1.3.4/gnssrefl/daily_avg_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/data/gpt_1wA.pickle` & `gnssrefl-1.3.4/gnssrefl/data/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/download_ioc.py` & `gnssrefl-1.3.4/gnssrefl/download_ioc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/download_noaa.py` & `gnssrefl-1.3.4/gnssrefl/download_noaa.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/download_orbits.py` & `gnssrefl-1.3.4/gnssrefl/download_orbits.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/download_psmsl.py` & `gnssrefl-1.3.4/gnssrefl/download_psmsl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/download_rinex.py` & `gnssrefl-1.3.4/gnssrefl/download_rinex.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/download_teqc.py` & `gnssrefl-1.3.4/gnssrefl/download_teqc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/download_tides.py` & `gnssrefl-1.3.4/gnssrefl/download_tides.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/download_unr.py` & `gnssrefl-1.3.4/gnssrefl/download_unr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/download_wsv.py` & `gnssrefl-1.3.4/gnssrefl/download_wsv.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/felipe.py` & `gnssrefl-1.3.4/gnssrefl/felipe.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/filesizes.py` & `gnssrefl-1.3.4/gnssrefl/filesizes.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/gnssir.py` & `gnssrefl-1.3.4/gnssrefl/gnssir.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/gnssir_cl.py` & `gnssrefl-1.3.4/gnssrefl/gnssir_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/gnsssnr.f` & `gnssrefl-1.3.4/gnssrefl/gnsssnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/gnsssnrbigger.f` & `gnssrefl-1.3.4/gnssrefl/gnsssnrbigger.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/gps.py` & `gnssrefl-1.3.4/gnssrefl/gps.py`

 * *Files 0% similar despite different names*

```diff
@@ -2515,15 +2515,15 @@
     """
     crnxpath = hatanaka_version()
     # added this for people that submit doy instead of month and day
     month, day, doy, cyyyy, cyy, cdoy = ymd2ch(year,month,day)
 
     rinexfile,rinexfiled = rinex_name(station, year, month, day)
 
-    print('Using new unavco protocols')
+    #print('Using new unavco protocols')
     #unavco = 'https://data-idm.unavco.org/archive/gnss/highrate/1-Hz/rinex/' 
     unavco = 'https://data.unavco.org/archive/gnss/highrate/1-Hz/rinex/'
 
 
     filename1 = rinexfile + '.Z'
     filename2 = rinexfiled + '.Z'
     url1 = unavco+  cyyyy + '/' + cdoy + '/' + station + '/' + filename1
```

### Comparing `gnssrefl-1.3.3/gnssrefl/gpssnr.f` & `gnssrefl-1.3.4/gnssrefl/gpssnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/gpsweek.py` & `gnssrefl-1.3.4/gnssrefl/gpsweek.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/gpt_1wA.pickle` & `gnssrefl-1.3.4/gnssrefl/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/highrate.py` & `gnssrefl-1.3.4/gnssrefl/highrate.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/installexe_cl.py` & `gnssrefl-1.3.4/gnssrefl/installexe_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/invsnr_cl.py` & `gnssrefl-1.3.4/gnssrefl/invsnr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/invsnr_input.py` & `gnssrefl-1.3.4/gnssrefl/invsnr_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/karnak_libraries.py` & `gnssrefl-1.3.4/gnssrefl/karnak_libraries.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,14 @@
         return file_name,foundit
     cydoy =  cyyyy + '/' + cdoy + '/'
     s1 = time.time()
     if (archive == 'unavco'):
         # original dir1 = 'https://data.unavco.org/archive/gnss/rinex3/obs/' + cyyyy + '/' + cdoy + '/'
         #url1 =      'https://data-idm.unavco.org/archive/gnss/rinex3/obs/' + cydoy + file_name
         url1 =      'https://data.unavco.org/archive/gnss/rinex3/obs/' + cydoy + file_name
-        print('Testing new unavco protocols:',url1)
         foundit,file_name = kelly.the_kelly_simple_way(url1,file_name)
         s2 = time.time()
         print('Download took ',np.round(s2-s1,2), ' seconds') 
         return file_name,foundit
 
     try:
         if (archive == 'ign'):
@@ -447,23 +446,24 @@
             foundit = True
     elif (archive == 'unavco-old'):
         dir1 = 'https://data.unavco.org/archive/gnss/rinex/obs/' + cydoy
         foundit, file_name = gogetit(dir1, dname, '.Z'); 
         if not foundit:
             foundit, file_name = gogetit(dir1, oname, '.Z')
     elif (archive == 'unavco'):
-        print('testing out new protocol at unavco')
         #url1 = 'https://data-idm.unavco.org/archive/gnss/rinex/obs/' + cydoy + dname + '.Z'
         url1 = 'https://data.unavco.org/archive/gnss/rinex/obs/' + cydoy + dname + '.Z'
+        print(url1)
         foundit,file_name = kelly.the_kelly_simple_way(url1, dname + '.Z')
         if not foundit:
             url2 = 'https://data.unavco.org/archive/gnss/rinex/obs/' + cydoy + oname + '.Z'
+            print(url2)
             foundit,file_name = kelly.the_kelly_simple_way(url2, oname + '.Z')
     elif (archive == 'special'):
-        print('testing out new protocol at unavco')
+        #print('testing out new protocol at unavco')
         url1 = 'https://data.unavco.org/archive/gnss/products/reflectometry/' + cydoy + oname + '.gz'
         print(url1)
         foundit,file_name = kelly.the_kelly_simple_way(url1, oname + '.gz')
         # old way
         #foundit, file_name = gogetit(dir1, oname, '.gz'); 
     elif archive == 'sopac':
         dir1 = 'ftp://garner.ucsd.edu/pub/rinex/' + cydoy
```

### Comparing `gnssrefl-1.3.3/gnssrefl/llh2xyz.py` & `gnssrefl-1.3.4/gnssrefl/llh2xyz.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/make_json_input.py` & `gnssrefl-1.3.4/gnssrefl/make_json_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/nmea2snr.py` & `gnssrefl-1.3.4/gnssrefl/nmea2snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/nmea2snr_cl.py` & `gnssrefl-1.3.4/gnssrefl/nmea2snr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/phase_functions.py` & `gnssrefl-1.3.4/gnssrefl/phase_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/prn2gps.py` & `gnssrefl-1.3.4/gnssrefl/prn2gps.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/query_unr.py` & `gnssrefl-1.3.4/gnssrefl/query_unr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/quickLook_cl.py` & `gnssrefl-1.3.4/gnssrefl/quickLook_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/quickLook_function.py` & `gnssrefl-1.3.4/gnssrefl/quickLook_function.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/quickPhase.py` & `gnssrefl-1.3.4/gnssrefl/quickPhase.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/quickPhase_function.py` & `gnssrefl-1.3.4/gnssrefl/quickPhase_function.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/quickplt.py` & `gnssrefl-1.3.4/gnssrefl/quickplt.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/read_snr_files.py` & `gnssrefl-1.3.4/gnssrefl/read_snr_files.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/refl_zones.py` & `gnssrefl-1.3.4/gnssrefl/refl_zones.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/refl_zones_cl.py` & `gnssrefl-1.3.4/gnssrefl/refl_zones_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/refraction.py` & `gnssrefl-1.3.4/gnssrefl/refraction.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/rh_plot.py` & `gnssrefl-1.3.4/gnssrefl/rh_plot.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/rinex2snr.py` & `gnssrefl-1.3.4/gnssrefl/rinex2snr.py`

 * *Files 1% similar despite different names*

```diff
@@ -456,15 +456,15 @@
                     if (os.stat(snrname).st_size == 0):
                         log.write('you created a zero file size which could mean a lot of things \n')
                         log.write('bad exe, bad snr option, do not really have the orbit file \n')
                         status = subprocess.call(['rm','-f', snrname ])
                     else:
                         log.write('A SNR file was created: {0:50s}  \n'.format(snrname_full))
                         print('\n')
-                        print('SUCCESS: SNR file was created:', snrname_full)
+                        print('SUCCESS: SNR file was created \n', snrname_full)
                         g.store_snrfile(snrname,year,station)
                 else:
                     print('No SNR file was created - check logs section for additional information')
             else:
                 print('Either the RINEX file or orbit file does not exist, so there is nothing to convert')
                 log.write('Either the RINEX file or orbit file does not exist, so there is nothing to convert \n')
         else:
```

### Comparing `gnssrefl-1.3.3/gnssrefl/rinex2snr_cl.py` & `gnssrefl-1.3.4/gnssrefl/rinex2snr_cl.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,15 @@
 
             sopac : (Scripps Orbit and Permanent Array Center)
 
             special : (set aside files at UNAVCO for reflectometry users)
 
             unavco : (University Navstar Consortium, now Earthscope)
 
-            all : (searches unavco, sopac, and sonel in that order)
+            all : (searches sopac, unavco, and sonel )
 
     doy_end : int, optional
         end day of year to be downloaded. 
 
     year_end : int, optional
         end year.
```

### Comparing `gnssrefl-1.3.3/gnssrefl/rinex3_rinex2.py` & `gnssrefl-1.3.4/gnssrefl/rinex3_rinex2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/rinex3_snr.py` & `gnssrefl-1.3.4/gnssrefl/rinex3_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/rinpy.py` & `gnssrefl-1.3.4/gnssrefl/rinpy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/rt_rinex3_snr.py` & `gnssrefl-1.3.4/gnssrefl/rt_rinex3_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/snow_functions.py` & `gnssrefl-1.3.4/gnssrefl/snow_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/snowdepth_cl.py` & `gnssrefl-1.3.4/gnssrefl/snowdepth_cl.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,20 +58,18 @@
     If simple is set to true, the algorithms computes bare soil (and thus snow depth), using
     all values together.  The default defines bare soil values every 10 degrees in azimuth.  
 
     Examples
     -------
 
     snowdepth p101 2022
-
-    would use results from a previous run of daily_avg
+        would use results from a previous run of daily_avg
 
     snowdepth p101 2022 -medfilter 0.25 -ReqTracks 50
-    
-    would run daily_avg for you.
+        would run daily_avg for you using 50 tracks/0.25 meter median filter
 
     Parameters
     ----------
     station : str
         4 character station name
     year : int
         water year (i.e. jan-june of that year and oct-dec of the previous year)
```

### Comparing `gnssrefl-1.3.3/gnssrefl/spline_functions.py` & `gnssrefl-1.3.4/gnssrefl/spline_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/subdaily.py` & `gnssrefl-1.3.4/gnssrefl/subdaily.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/subdaily_cl.py` & `gnssrefl-1.3.4/gnssrefl/subdaily_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/utils.py` & `gnssrefl-1.3.4/gnssrefl/utils.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/veg_multiyr.py` & `gnssrefl-1.3.4/gnssrefl/veg_multiyr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/vwc.py` & `gnssrefl-1.3.4/gnssrefl/vwc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/vwc_input.py` & `gnssrefl-1.3.4/gnssrefl/vwc_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/xyz2llh.py` & `gnssrefl-1.3.4/gnssrefl/xyz2llh.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/ydoy.py` & `gnssrefl-1.3.4/gnssrefl/ydoy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl/ymd.py` & `gnssrefl-1.3.4/gnssrefl/ymd.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl.egg-info/PKG-INFO` & `gnssrefl-1.3.4/gnssrefl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 1.3.3
+Version: 1.3.4
 Summary: A GNSS reflectometry software package 
 Home-page: https://github.com/kristinemlarson/gnssrefl/
 Author: Kristine Larson
 Author-email: kristinem.larson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `gnssrefl-1.3.3/gnssrefl.egg-info/SOURCES.txt` & `gnssrefl-1.3.4/gnssrefl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/gnssrefl.egg-info/entry_points.txt` & `gnssrefl-1.3.4/gnssrefl.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/pyproject.toml` & `gnssrefl-1.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.3/setup.py` & `gnssrefl-1.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 requirements = ["numpy","wget","scipy","matplotlib","requests","progress","astropy","simplekml","earthscope-sdk"]
 setup(
     name="gnssrefl",
-    version="1.3.3",
+    version="1.3.4",
     author="Kristine Larson",
     author_email="kristinem.larson@gmail.com",
     description="A GNSS reflectometry software package ",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/kristinemlarson/gnssrefl/",
     packages=find_packages(),
```

### Comparing `gnssrefl-1.3.3/test/test_gps.py` & `gnssrefl-1.3.4/test/test_gps.py`

 * *Files identical despite different names*

