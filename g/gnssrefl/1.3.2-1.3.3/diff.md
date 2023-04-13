# Comparing `tmp/gnssrefl-1.3.2.tar.gz` & `tmp/gnssrefl-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnssrefl-1.3.2.tar", last modified: Sat Apr  8 13:05:03 2023, max compression
+gzip compressed data, was "gnssrefl-1.3.3.tar", last modified: Thu Apr 13 07:42:59 2023, max compression
```

## Comparing `gnssrefl-1.3.2.tar` & `gnssrefl-1.3.3.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 13:05:03.385366 gnssrefl-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-08 13:04:46.000000 gnssrefl-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-08 13:04:46.000000 gnssrefl-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-08 13:05:03.385366 gnssrefl-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-08 13:04:46.000000 gnssrefl-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 13:05:03.357366 gnssrefl-1.3.2/gnssrefl/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/EGM96.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/check_rinex.py
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/check_rinex2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/computemp1mp2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19095 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/daily_avg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/daily_avg_cl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 13:05:03.361366 gnssrefl-1.3.2/gnssrefl/data/
--rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/data/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/download_ioc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/download_noaa.py
--rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/download_orbits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/download_psmsl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/download_rinex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/download_teqc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/download_tides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/download_unr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/download_wsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/felipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/filesizes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15934 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/gnssir.py
--rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/gnssir_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    50572 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/gnsssnr.f
--rw-r--r--   0 runner    (1001) docker     (123)    50579 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/gnsssnrbigger.f
--rw-r--r--   0 runner    (1001) docker     (123)   173743 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/gps.py
--rw-r--r--   0 runner    (1001) docker     (123)    40525 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/gpssnr.f
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/gpsweek.py
--rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/gpt_1wA.pickle
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/highrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/installexe_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10528 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/invsnr_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/invsnr_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    23530 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/karnak_libraries.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/kelly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/llh2xyz.py
--rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/make_json_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    22560 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/nmea2snr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/nmea2snr_cl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34269 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/phase_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/pickle_dilemma.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/prn2gps.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/query_unr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/quickLook_cl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19809 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/quickLook_function.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5879 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/quickPhase.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19480 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/quickPhase_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/quickplt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/read_snr_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    16511 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/refl_zones.py
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/refl_zones_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/refraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/rh_plot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49162 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/rinex2snr.py
--rw-r--r--   0 runner    (1001) docker     (123)    15472 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/rinex2snr_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/rinex3_rinex2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/rinex3_snr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24490 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/rinpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/rt_rinex3_snr.py
--rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/snow_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/snowdepth_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    60155 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/spline_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    58660 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/subdaily.py
--rw-r--r--   0 runner    (1001) docker     (123)     9554 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/subdaily_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/veg_multiyr.py
--rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/vwc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/vwc_input.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/xyz2llh.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/ydoy.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/gnssrefl/ymd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 13:05:03.361366 gnssrefl-1.3.2/gnssrefl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-08 13:05:03.000000 gnssrefl-1.3.2/gnssrefl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-08 13:05:03.000000 gnssrefl-1.3.2/gnssrefl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 13:05:03.000000 gnssrefl-1.3.2/gnssrefl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-08 13:05:03.000000 gnssrefl-1.3.2/gnssrefl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-08 13:05:03.000000 gnssrefl-1.3.2/gnssrefl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-08 13:05:03.000000 gnssrefl-1.3.2/gnssrefl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 13:05:03.385366 gnssrefl-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 13:05:03.385366 gnssrefl-1.3.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/test/test_gps.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-08 13:04:47.000000 gnssrefl-1.3.2/test/test_rinex2snr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:42:59.039011 gnssrefl-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-13 07:42:59.039011 gnssrefl-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:42:59.011011 gnssrefl-1.3.3/gnssrefl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/EGM96.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/check_rinex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/check_rinex2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/computemp1mp2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19095 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/daily_avg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/daily_avg_cl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:42:59.015010 gnssrefl-1.3.3/gnssrefl/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/data/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/download_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/download_noaa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/download_orbits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/download_psmsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/download_rinex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/download_teqc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/download_tides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/download_unr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/download_wsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/felipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/filesizes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15934 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/gnssir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/gnssir_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50572 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/gnsssnr.f
+-rw-r--r--   0 runner    (1001) docker     (123)    50579 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/gnsssnrbigger.f
+-rw-r--r--   0 runner    (1001) docker     (123)   174545 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40525 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/gpssnr.f
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-13 07:42:42.000000 gnssrefl-1.3.3/gnssrefl/gpsweek.py
+-rw-r--r--   0 runner    (1001) docker     (123) 21773344 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/gpt_1wA.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/highrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/installexe_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10528 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/invsnr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/invsnr_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23530 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/karnak_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/kelly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/llh2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/make_json_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22560 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/nmea2snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/nmea2snr_cl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34269 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/phase_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/pickle_dilemma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/prn2gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/query_unr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/quickLook_cl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19809 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/quickLook_function.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5879 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/quickPhase.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19480 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/quickPhase_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/quickplt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/read_snr_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16511 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/refl_zones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/refl_zones_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/refraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/rh_plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49162 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/rinex2snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15472 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/rinex2snr_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/rinex3_rinex2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/rinex3_snr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24490 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/rinpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/rt_rinex3_snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/snow_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/snowdepth_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60155 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/spline_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58660 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/subdaily.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9554 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/subdaily_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/veg_multiyr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/vwc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/vwc_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/xyz2llh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/ydoy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/gnssrefl/ymd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:42:59.015010 gnssrefl-1.3.3/gnssrefl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-13 07:42:58.000000 gnssrefl-1.3.3/gnssrefl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-13 07:42:58.000000 gnssrefl-1.3.3/gnssrefl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 07:42:58.000000 gnssrefl-1.3.3/gnssrefl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-13 07:42:58.000000 gnssrefl-1.3.3/gnssrefl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 07:42:58.000000 gnssrefl-1.3.3/gnssrefl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 07:42:58.000000 gnssrefl-1.3.3/gnssrefl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 07:42:59.039011 gnssrefl-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:42:59.039011 gnssrefl-1.3.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/test/test_gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-13 07:42:43.000000 gnssrefl-1.3.3/test/test_rinex2snr.py
```

### Comparing `gnssrefl-1.3.2/LICENSE` & `gnssrefl-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/PKG-INFO` & `gnssrefl-1.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 1.3.2
+Version: 1.3.3
 Summary: A GNSS reflectometry software package 
 Home-page: https://github.com/kristinemlarson/gnssrefl/
 Author: Kristine Larson
 Author-email: kristinem.larson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gnssrefl
 
-**github version: 1.3.2** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+**github version: 1.3.3** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
 
 Our documentation is now available [here.](https://gnssrefl.readthedocs.io/en/latest/)
 
 The [shortcourse registration page is live.](https://www.earthscope.org/event/2023-gnss-ir-short-course) 
 
 If you want to sign up for the GNSS-IR email list, please contact Kristine Larson.
```

### Comparing `gnssrefl-1.3.2/README.md` & `gnssrefl-1.3.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # gnssrefl
 
-**github version: 1.3.2** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+**github version: 1.3.3** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
 
 Our documentation is now available [here.](https://gnssrefl.readthedocs.io/en/latest/)
 
 The [shortcourse registration page is live.](https://www.earthscope.org/event/2023-gnss-ir-short-course) 
 
 If you want to sign up for the GNSS-IR email list, please contact Kristine Larson.
```

### Comparing `gnssrefl-1.3.2/gnssrefl/EGM96.py` & `gnssrefl-1.3.3/gnssrefl/EGM96.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/check_rinex.py` & `gnssrefl-1.3.3/gnssrefl/check_rinex.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/check_rinex2.py` & `gnssrefl-1.3.3/gnssrefl/check_rinex2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/computemp1mp2.py` & `gnssrefl-1.3.3/gnssrefl/computemp1mp2.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/daily_avg.py` & `gnssrefl-1.3.3/gnssrefl/daily_avg.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/daily_avg_cl.py` & `gnssrefl-1.3.3/gnssrefl/daily_avg_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/data/gpt_1wA.pickle` & `gnssrefl-1.3.3/gnssrefl/data/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/download_ioc.py` & `gnssrefl-1.3.3/gnssrefl/download_ioc.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,16 @@
-# -*- coding: utf-8 -*-
 import argparse
 import datetime
 import numpy as np
 import os
 import requests
 import subprocess
 import sys
 import gnssrefl.gps as g
 
-from gnssrefl.utils import validate_input_datatypes, str2bool
-
-
-def parse_arguments():
-    parser = argparse.ArgumentParser()
-    parser.add_argument("station", help="station name", type=str)
-    parser.add_argument("date1", help="first-date, 20150101", type=str)
-    parser.add_argument("date2", help="end-date, 20150101", type=str)
-    parser.add_argument("-output", default=None, help="Optional output filename", type=str)
-    parser.add_argument("-plt", default=None, help="Optional plot to screen", type=str)
-    parser.add_argument("-outliers", default=None, help="attempt to remove outliers", type=str)
-    parser.add_argument("-sensor", default=None, help="Various: flt, prs or rad, default is rad. If there are multiple sensors, they are all written to the file.", type=str)
-    parser.add_argument("-subdir", default=None, help="subdirectory for output file", type=str)
-    args = parser.parse_args().__dict__
-
-
-    # convert all expected boolean inputs from strings to booleans
-    boolean_args = ['plt','outliers']
-    args = str2bool(args, boolean_args)
-
-
-    # only return a dictionary of arguments that were added from the user - all other defaults will be set in code below
-    return {key: value for key, value in args.items() if value is not None}
-
 
 def download_ioc(station: str, date1: str, date2: str, output: str = None, plt: bool = False, outliers: bool = False, sensor= None, subdir: str=None):
     """
     Downloads and saves IOC tide gauge files
 
     Parameters
     ----------
@@ -249,14 +224,9 @@
     else:
         cmm = '{:02d}'.format(m+1)
         d2 = cyyyy + cmm + '01'
 
     return d1, d2
 
 
-def main():
-    args = parse_arguments()
-    download_ioc(**args)
-
-
 if __name__ == "__main__":
     main()
```

### Comparing `gnssrefl-1.3.2/gnssrefl/download_noaa.py` & `gnssrefl-1.3.3/gnssrefl/download_noaa.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,34 +3,15 @@
 import datetime
 import os
 import requests
 import subprocess
 import sys
 import gnssrefl.gps as g
 
-from gnssrefl.utils import validate_input_datatypes, str2bool
-
-def parse_arguments():
-    parser = argparse.ArgumentParser()
-    parser.add_argument("station", help="station name, e.g. 8768094", type=str)
-    parser.add_argument("date1", help="start-date, 20150101", type=str)
-    parser.add_argument("date2", help="end-date, 20150110", type=str)
-    parser.add_argument("-output", default=None, help="Optional output filename", type=str)
-    parser.add_argument("-plt", default=None, help="quick plot to screen", type=str)
-    parser.add_argument("-datum", default=None, help="datum (lwd for lakes?)", type=str)
-    parser.add_argument("-subdir", default=None, help="optional subdirectory name for output", type=str)
-    args = parser.parse_args().__dict__
-
-    # convert all expected boolean inputs from strings to booleans
-    boolean_args = ['plt']
-    args = str2bool(args, boolean_args)
-
-
-    # only return a dictionary of arguments that were added from the user - all other defaults will be set in code below
-    return {key: value for key, value in args.items() if value is not None}
+#from gnssrefl.utils import validate_input_datatypes, str2bool
 
 def download_noaa(station: str, date1: str, date2: str, output: str = None, plt: bool = False, datum: str = 'mllw', subdir: str = None):
     """
     Downloads NOAA tide gauge files and stores locally
     If you ask for 31 days of data or less, it will download exactly what you ask for.
     But if you want a longer time series, this code needs to query the NOAA API every month.
     To make the code easier to write, I start with the first day of the first month you ask for and end with
@@ -417,15 +398,11 @@
         error = True
     else:
         if printmeta:
             print(data['metadata'])
 
     return data, error
 
-def main():
-    args = parse_arguments()
-    download_noaa(**args)
-
 
 if __name__ == "__main__":
     main()
```

### Comparing `gnssrefl-1.3.2/gnssrefl/download_orbits.py` & `gnssrefl-1.3.3/gnssrefl/download_orbits.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/download_psmsl.py` & `gnssrefl-1.3.3/gnssrefl/download_psmsl.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,33 +7,17 @@
 import sys
 import matplotlib.pyplot as plt
 import subprocess
 import urllib
 
 import gnssrefl.gps as g
 
-from gnssrefl.utils import validate_input_datatypes, str2bool
+#from gnssrefl.utils import validate_input_datatypes, str2bool
 
 
-def parse_arguments():
-    parser = argparse.ArgumentParser()
-    parser.add_argument("station", help="station name, e.g. 10313", type=str)
-    parser.add_argument("-output", default=None, help="Optional output filename", type=str)
-    parser.add_argument("-plt", default=None, help="Optional plot to screen variable, boolean", type=str)
-    args = parser.parse_args().__dict__
-
-
-    # convert all expected boolean inputs from strings to booleans
-    boolean_args = ['plt']
-    args = str2bool(args, boolean_args)
-
-
-    # only return a dictionary of arguments that were added from the user - all other defaults will be set in code below
-    return {key: value for key, value in args.items() if value is not None}
-
 
 def download_psmsl(station: str, output: str = None, plt: bool = False):
     """
     Downloads PSMSL tide gauge files created by Simon Williams 
     in json format, converts it to plain txt or csv format
 
     Parameters
@@ -101,14 +85,10 @@
     if NV < 1:
         print('No data found')
         sys.exit()
 
     if plt:
         g.quickp('PSMSL ' + station,obs,sl)
 
-def main():
-    args = parse_arguments()
-    download_psmsl(**args)
-
 
 if __name__ == "__main__":
     main()
```

### Comparing `gnssrefl-1.3.2/gnssrefl/download_rinex.py` & `gnssrefl-1.3.3/gnssrefl/download_rinex.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/download_teqc.py` & `gnssrefl-1.3.3/gnssrefl/download_teqc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/download_tides.py` & `gnssrefl-1.3.3/gnssrefl/download_tides.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/download_unr.py` & `gnssrefl-1.3.3/gnssrefl/download_unr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/download_wsv.py` & `gnssrefl-1.3.3/gnssrefl/download_wsv.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/felipe.py` & `gnssrefl-1.3.3/gnssrefl/felipe.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/filesizes.py` & `gnssrefl-1.3.3/gnssrefl/filesizes.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/gnssir.py` & `gnssrefl-1.3.3/gnssrefl/gnssir.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/gnssir_cl.py` & `gnssrefl-1.3.3/gnssrefl/gnssir_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/gnsssnr.f` & `gnssrefl-1.3.3/gnssrefl/gnsssnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/gnsssnrbigger.f` & `gnssrefl-1.3.3/gnssrefl/gnsssnrbigger.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/gps.py` & `gnssrefl-1.3.3/gnssrefl/gps.py`

 * *Files 2% similar despite different names*

```diff
@@ -3503,15 +3503,15 @@
         else:
             print('I do not recognize the orbit type you tried to use: ', orbtype)
 
     return foundit, f, orbdir, snrexe
 
 def warn_and_exit(snrexe,fortran):
     """
-    if snr executable does not exist, exit
+    if the GNSS/GPS to SNR executable does not exist, exit
 
     snrexe : str
         name of the executable
     fortran : bool
         whether fortran is being used for translation
     """
     if not fortran:
@@ -3522,37 +3522,34 @@
         if (os.path.isfile(snrexe) == False):
             print('This RINEX translation executable does not exist:' + snrexe )
             print('Install it or use -fortran False. Exiting')
             sys.exit()
 
 def new_rinex3_rinex2(r3_filename,r2_filename,dec=1,gpsonly=False):
     """
-    assuming gfzrnx executable exists, the rinex 3 file is hatanaka
-    uncompressed and translated into a rinex 2 file
+    This code translates a RINEX 3 file into a RINEX 2.11 file.
+    It is assumed that the gfzrnx exists and that the RINEX 3 file is 
+    Hatanaka uncompressed or compressed.
 
     Parameters
     ----------
-    r3_filename : string
-         rinex 3 format filename. either Hatanaka 
+    r3_filename : str
+         RINEX 3 format filename. Either Hatanaka 
          compressed or uncompressed allowed
-
-    r2_filename : string
-         rinex 2.11 file
-
+    r2_filename : str
+         RINEX 2.11 file
     dec : integer
-        decimation factor. default is 0 or 1 which means none
-
+        decimation factor. If 0 or 1, no decimation is done.
     gpsonly : boolean
-
         whether you want only GPS signals. Default is false
 
     Returns
     -------
     fexists : boolean
-        whether rinex 2 file was created and exists
+        whether the RINEX 2.11 file was created and exists
 
     """
     fexists = False
     gexe = gfz_version()
     crnxpath = hatanaka_version()
     #lastbit =  r3_filename[-6:]
     if r3_filename[-3:] == 'crx':
@@ -3606,14 +3603,16 @@
 
 
     return fexists
 
 
 def ign_orbits(filename, directory,year):
     """
+    Downloads sp3 files from the IGN archive
+
     Parameters
     ----------
     filename : str
         name of the sp3 file
     directory : str
         location of orbits at the IGN
     year : int
@@ -3640,15 +3639,15 @@
         foundit = False
 
     return foundit 
 
 
 def ign_rinex3(station9ch, year, doy,srate):
     """
-    download rinex 3 from IGN
+    Downloads a RINEX 3 file from IGN
 
     Parameters
     ----------
     station9ch : str
         9 character station name
     year : int
         full year
@@ -3687,30 +3686,33 @@
         fexist = True
 
     return fexist
 
 
 def hatanaka_version():
     """
+    Finds the Hatanaka decompression executable
 
     Returns
     -------
-    hatanakav : string 
+    hatanakav : str 
         name/location of hatanaka executable
 
     """
     exedir = os.environ['EXE']
     hatanakav = exedir + '/CRX2RNX'
     # heroku version should be in the main area
     if not os.path.exists(hatanakav):
         hatanakav = './CRX2RNX'
     return hatanakav
 
 def gfz_version():
     """
+    Finds location of the gfzrnx executable
+
     Returns
     -------
     gfzv : str
         name/location of gfzrnx executable
 
     """
     exedir = os.environ['EXE']
@@ -3718,48 +3720,52 @@
     # heroku version should be in the main area
     if not os.path.exists(gfzv):
         gfzv = './gfzrnx'
     return gfzv
 
 def gpsSNR_version():
     """
+    Finds location of the gps to SNR executable
 
     Returns
     -------
-    gpse : string
+    gpse : str
         location of gpsSNR executable
     """
     exedir = os.environ['EXE']
     gpse = exedir + '/gpsSNR.e'
     # heroku version should be in the main area
     if not os.path.exists(gpse):
         gpse = './gpsSNR.e'
     return gpse
 
 def gnssSNR_version():
     """
+    Finds location of the GNSS to SNR executable
+
     Returns
     -------
-    gpse : string 
+    gpse : str 
         location of gnssSNR executable
 
     """
     exedir = os.environ['EXE']
     gpse = exedir + '/gnssSNR.e'
     # heroku version should be in the main area
     if not os.path.exists(gpse):
         gpse = './gnssSNR.e'
     return gpse
 
 def teqc_version():
     """
+    Finds location of the teqc executable
 
     Returns
-    --------
-    gpse : string 
+    -------
+    gpse : str
         location of teqc executable
 
     """
     exedir = os.environ['EXE']
     gpse = exedir + '/teqc'
     # heroku version should be in the main area
     if not os.path.exists(gpse):
@@ -3769,22 +3775,21 @@
 def snr_exist(station,year,doy,snrEnd):
     """
     check to see if the SNR file already exists
     uncompresses if necessary (gz or xz)
 
     Parameters
     ----------
-    station : string
+    station : str
         four character station name
-
-    year : integer
-
-    doy : integer
-
-    snrEnd : string
+    year : int
+        full year
+    doy : int
+        day of year
+    snrEnd : str
         2 character snr type, i.e. 66, 99
 
     Returns
     -------
     snre : boolean
         whether SNR file exists. 
 
@@ -3960,30 +3965,32 @@
     else:
         print('No file was found at ESA')
 
     return fstatus
 
 def get_cddis_navfile(navfile,cyyyy,cyy,cdoy):
     """
-    tries to download navigation file from CDDIS
+    Tries to download navigation file from CDDIS
+    Renames it to my convention (auto0010.22n)
 
     Parameters
     ----------
-    navfile : string
+    navfile : str
         name of GPS broadcast orbit file
-    cyyyy : string
+    cyyyy : str
         4 char year
-    cyy : string
+    cyy : str
         2 char year
-    cdoy : string
+    cdoy : str
         3 char day of year
 
     Returns
-    --------
-    navfile : string
+    -------
+    navfile : str
+        full path of the stored navigation file
 
     """
 
     cddisfile = 'brdc' + cdoy + '0.' +cyy  +'n'
     cddisfile_compressed = cddisfile + '.Z'
     cddisfile_gzip = cddisfile + '.gz'
     # where the file should be at CDDIS ....
@@ -4024,36 +4031,36 @@
         print('Change the filename to what we use ', navfile)
         subprocess.call(['mv',cddisfile,navfile])
 
     return navfile
 
 def ydoy2useful(year, doy):
     """
+    Calculates various dates
 
     Parameters
     ----------
-    year : integer
-
-    doy : integer
+    year : int
+        full year
+    doy : int
         day of year
 
     Returns
     -------
-    year : integer
-
-    month : integer
-
+    year : int
+        full year
+    month : int
+        calendar month
     day : integer
-
-    cyyyy : string
+        calendar day
+    cyyyy : str
         four character year
-    cdoy : string
+    cdoy : str
         three character day of year
-
-    YMD : string
+    YMD : str
          date as in '19-12-01' for December 1, 2019
 
     """
 
     d = datetime.datetime(year, 1, 1) + datetime.timedelta(days=(doy-1))
 #   not sure you need to do this int step
     month = int(d.month)
@@ -4063,28 +4070,28 @@
     cdd = '{:02d}'.format(day)
     cmonth = char_month_converter(month)
     YMD = cyy + cmonth + cdd
     return year, month, day, cyyyy,cdoy, YMD
 
 def prevdoy(year,doy):
     """
-    given year and doy, return previous year and doy
+    Given year and doy, return previous year and doy
 
     Parameters
     ----------
-    year : integer
-    
-    doy : integer
+    year : int
+        full year
+    doy : int
+        day of year
 
     Returns
     -------
-    pyear : integer
+    pyear : int
         previous year
-
-    pdoy : integer 
+    pdoy : int
         previous day of year 
     """
     if (doy == 1):
         pyear = year -1
         doyx,cdoyx,cyyyy,cyy = ymd2doy(pyear,12,31)
         pdoy = doyx
     else:
@@ -4096,24 +4103,24 @@
 
 def nextdoy(year,doy):
     """
     given a year/doy returns the subsequent year/doy
 
     Parameters
     ----------
-    year : integer
-
-    doy : integer
+    year : int
+        day of year
+    doy : int
+        day of year
 
     Returns
     -------
-    nyear : integer
+    nyear : int
         next year
-
-    ndoy : integer
+    ndoy : int
         next day of year
 
     """
     dec31,cdoy,ctmp,ctmp2 = ymd2doy(year,12,31)
     if (doy == dec31):
         nyear = year + 1
         ndoy = 1
@@ -4122,14 +4129,15 @@
         ndoy = doy + 1
 
     return nyear, ndoy
 
 def read_sp3file(file_path):
     """ 
     input: file_path is the sp3file name
+    I do not believe this is used
 
     Returns
     -------
     sp3 : ndarray
     colums are satnum, gpsweek, gps_sow, x,y,z
     x,y,z are in meters
     satnum has 0, 100, 200, 300 added for gps, glonass, galileo,beidou,
@@ -4175,20 +4183,26 @@
     f.close()
     nr,nc = sp3.shape
     #print('number of rows and columns being returned from the sp3 file', nr,nc)
     return sp3
 
 def nicerTime(UTCtime):
     """
-    input float hour
-    output HH:MM string
-    2021 may 3, changed to deal with hour boundaries
-    since thsi only does hours and minutes, it rounds up or down
-    depending on seconds < or > 30
-    fails near midnite ... 
+    Converts fractional time (hours) to HH:MM
+
+    Parameters
+    ----------
+    UTCtime : float
+        fractional hours of the day 
+
+    Returns 
+    -------
+    T : str
+        output as HH:MM 
+
     """
     hour = int(np.floor(UTCtime))
     minute = int ( np.floor(60* ( UTCtime - hour )))
     second = int ( 3600*UTCtime - 3600*hour  - 60*minute)
     #print(hour,minute,second)
     if (second > 30):
         # up the minutes ...
@@ -4203,31 +4217,31 @@
     T = chour + ':' + cminute  
 
     return T
 
 
 def big_Disk_work_hard(station,year,month,day):
     """
-    attempts to pick up subdaily files from the NGS archive
+    Attempts to pick up subdaily RINEX 2.11 files from the NGS archive
     creates a single RINEX file
 
-    Parameters
-    -----------
-    station: string
-        4 character id station name
+    If day is 0, then month is presumed to be the day of year
 
-    year: integer
-        year
+    Requires teqc
 
-    month: integer
+    Parameters
+    ----------
+    station: str
+        4 char station name
+    year: int
+        year
+    month: int
         month
-
     day: integer
         day
-        if day is 0, then month is presumed to be the day of year
 
     """
     if (day == 0):
         doy = month
         year, month, day, cyyyy,cdoy, YMD = ydoy2useful(year,doy)
         cyy = cyyyy[2:4]
     else:
@@ -4263,32 +4277,32 @@
     print('file created: ', rinexfile)
     # should delete the hourly files
     subprocess.call(blist)
 
 
 def big_Disk_in_DC_hourly(station, year, month, day,idtag):
     """
-    picks up a one hour RINEX file from CORS. and gunzips it
+    Picks up a one hour RINEX file from CORS. and gunzips it
 
     Parameters
-    ---------
-    station : string
-        
-    year : integer
-
-    month : integer
-
+    ----------
+    station : str
+        4 ch station name
+    year : int
+        full year
+    month : int
+        calendar month
     day : integer
         day of the month. if zero, it means month is really day of year
-    idtag : character
-        small case letter from a to x (i think)
+    idtag : str
+        small case letter from a to x; tells the code which hour it is
+
     """
     doy,cdoy,cyyyy,cyy = ymd2doy(year,month,day)
-    #rinexfile,rinexfiled = rinex_name(station, year, month, day)
-    # compressed rinexfile
+    # define names
     crinexfile = station + cdoy + idtag + '.' + cyy + 'o.gz'
     rinexfile =  station + cdoy + idtag + '.' + cyy + 'o'
     # do not know if this works - but what the hey
     mainadd = 'https://geodesy.noaa.gov/corsdata/rinex/'
     #mainadd = 'ftp://www.ngs.noaa.gov/cors/rinex/'
     url = mainadd + cyyyy + '/' + cdoy+ '/' + station + '/' + crinexfile
     print(url)
@@ -4313,20 +4327,20 @@
 
 def ftitle(freq):
     """
     makes a frequency title for plots 
 
     Parameters
     ----------
-    freq : integer
-        frequency
+    freq : int
+        GNSS frequency
 
     Returns
     -------
-    returnf : string
+    returnf : str
         nice string for the constellation/frequency for the title of a plot
     """
     f=str(freq)
     out = {}
     out['1'] = 'GPS L1'
     out['2'] = 'GPS L2'
     out['20'] = 'GPS L2C'
@@ -4354,15 +4368,15 @@
 def cdate2nums(col1):
     """
     returns fractional year from ch date, e.g. 2012-02-15
     if time is blank, return 3000
 
     Parameters
     ----------
-    col1 : string
+    col1 : str
         date in yyyyy-mm-dd, 2012-02-15
 
     Returns
     -------
     t : float
         fractional date, year + doy/365.25
     """
@@ -4380,15 +4394,15 @@
 
 def cdate2ydoy(col1):
     """
     returns year and day of year from character date, e.g. '2012-02-15'
 
     Parameters
     ----------
-    col1 : string
+    col1 : str
         date in yyyyy-mm-dd, 2012-02-15
 
     Returns
     -------
     year : int 
         full year
     doy : int 
@@ -4405,28 +4419,28 @@
         #t = year + doy/365.25
 
     return year, doy
 
 
 def l2c_l5_list(year,doy):
     """
-    creates a satellite list of L2C and L5 transmitting satellites
+    Creates a satellite list of L2C and L5 transmitting satellites
+    for a given year/doy
 
     Parameters
     ----------
-    year: integer
-        year
-
+    year: int
+        full year
     doy: integer
         day of year
 
     Returns
     -------
     l2csatlist : numpy array (int)
-        satellites  possibly transmittingL2C 
+        satellites possibly transmittingL2C 
 
     l5satlist : numpy array (int)
         satellites possibly transmitting L5 
 
     """
 
     # this numpy array has the satellite number, year, and doy of each launch of a L2C satellite
@@ -4460,41 +4474,42 @@
     """
     j=bytes(string,'ascii') + b'\0\0'
 
     return array(j)
 
 def ymd_hhmmss(year,doy,utc,dtime):
     """
+
     Parameters
     ----------
-    year : integer
-
-    doy : integer
-
+    year : int
+        full year
+    doy : int
+        full year
     UTC : float
         fractional hours
-
     dtime : bool
         whether you want datetime object
 
     Returns 
     -------
-    bigT : datetime
+    bigT : datetime object
 
     year : int
-
+        full year
     month : int
-
+        calendar month
     day : int
-
+        calendar day
     hour : int
-
+        hour of the day
     minute: int
-
+        minutes of the day
     second : int
+        seconds
 
     """
     year = int(year) # just in case
     d = datetime.datetime(year, 1, 1) + datetime.timedelta(days=(doy-1))
     month = int(d.month)
     day = int(d.day)
     hour = int(np.floor(utc))
@@ -4577,20 +4592,21 @@
     return modifiedjulian
 
 def more_confused_obstimes(tvd):
     """
 
     Parameters
     ----------
-    tvd : numpy file floats
+    tvd : numpy array of floats
         lsp results from a loadtxt command
 
     Returns
     -------
-    modifiedjulian : numpy array of floats
+    modifiedjulian : numpy array of floats 
+         mjd values
         
     """
     nr,nc = tvd.shape
     modifiedjulian = []
     if nr > 0:
         for ijk in range(0,nr):
             #MM DD HH Min Sec
@@ -4606,14 +4622,15 @@
 
     return modifiedjulian
 
 
 
 def read_simon_williams(filename,outfilename):
     """
+    Reads a PSMSL file and creates a new one 
     
     Parameters
     ----------
     filename : str
         datafile of GNSS based water level measurements from 
         the archive at PSMSL created by Simon Williams 
 
@@ -4717,14 +4734,15 @@
     ----------
     t : list of integers
         with year, month, day, hour, minute, second 
 
     Returns
     -------
     obstimes : datetime 
+
     """
     nr,nc = t.shape
     obstimes = []
 
     # if i read in the file better, would not have to change from float
     # year mon day hour min sealevel doy mjd seconds
     if nr > 0:
```

### Comparing `gnssrefl-1.3.2/gnssrefl/gpssnr.f` & `gnssrefl-1.3.3/gnssrefl/gpssnr.f`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/gpsweek.py` & `gnssrefl-1.3.3/gnssrefl/gpsweek.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/gpt_1wA.pickle` & `gnssrefl-1.3.3/gnssrefl/gpt_1wA.pickle`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/highrate.py` & `gnssrefl-1.3.3/gnssrefl/highrate.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/installexe_cl.py` & `gnssrefl-1.3.3/gnssrefl/installexe_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/invsnr_cl.py` & `gnssrefl-1.3.3/gnssrefl/invsnr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/invsnr_input.py` & `gnssrefl-1.3.3/gnssrefl/invsnr_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/karnak_libraries.py` & `gnssrefl-1.3.3/gnssrefl/karnak_libraries.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/kelly.py` & `gnssrefl-1.3.3/gnssrefl/kelly.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/llh2xyz.py` & `gnssrefl-1.3.3/gnssrefl/llh2xyz.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/make_json_input.py` & `gnssrefl-1.3.3/gnssrefl/make_json_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/nmea2snr.py` & `gnssrefl-1.3.3/gnssrefl/nmea2snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/nmea2snr_cl.py` & `gnssrefl-1.3.3/gnssrefl/nmea2snr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/phase_functions.py` & `gnssrefl-1.3.3/gnssrefl/phase_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/prn2gps.py` & `gnssrefl-1.3.3/gnssrefl/prn2gps.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/query_unr.py` & `gnssrefl-1.3.3/gnssrefl/query_unr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/quickLook_cl.py` & `gnssrefl-1.3.3/gnssrefl/quickLook_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/quickLook_function.py` & `gnssrefl-1.3.3/gnssrefl/quickLook_function.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/quickPhase.py` & `gnssrefl-1.3.3/gnssrefl/quickPhase.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/quickPhase_function.py` & `gnssrefl-1.3.3/gnssrefl/quickPhase_function.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/quickplt.py` & `gnssrefl-1.3.3/gnssrefl/quickplt.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/read_snr_files.py` & `gnssrefl-1.3.3/gnssrefl/read_snr_files.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/refl_zones.py` & `gnssrefl-1.3.3/gnssrefl/refl_zones.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/refl_zones_cl.py` & `gnssrefl-1.3.3/gnssrefl/refl_zones_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/refraction.py` & `gnssrefl-1.3.3/gnssrefl/refraction.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/rh_plot.py` & `gnssrefl-1.3.3/gnssrefl/rh_plot.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/rinex2snr.py` & `gnssrefl-1.3.3/gnssrefl/rinex2snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/rinex2snr_cl.py` & `gnssrefl-1.3.3/gnssrefl/rinex2snr_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/rinex3_rinex2.py` & `gnssrefl-1.3.3/gnssrefl/rinex3_rinex2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,76 @@
 # -*- coding: utf-8 -*-
 """
 Translates rinex3 to rinex2. relies on gfzrnx
 """
 import argparse
 import os
-import gnssrefl.gps as g
+import subprocess
 import sys
 
+import gnssrefl.gps as g
+
 def main():
     """
     Converts a RINEX 3 file into a RINEX 2.11 file. Uses gfzrnx.
 
     Parameters
     ----------
     rinex3 : str
         filename for RINEX 3 file
-    rinex2 : str
+    rinex2 : str, optional
         filename for RINEX 2.11 file
-    dec : integer
-        optional decimation value (seconds)
-    gpsonly : boolean
+    dec : integer, optional
+        decimation value (seconds)
+    gpsonly : bool, optional
         whether to remove everything except GPS. Default is False
 
     """
 
     parser = argparse.ArgumentParser()
     parser.add_argument("rinex3", help="rinex3 filename", type=str)
-    parser.add_argument("rinex2", help="rinex2 filename", type=str)
+    parser.add_argument("-rinex2", help="rinex2 filename", type=str,default=None)
     parser.add_argument("-dec", help="decimation value (seconds)", type=int,default=None)
     parser.add_argument("-gpsonly", help="remove everything except GPS", type=str,default=None)
 
     args = parser.parse_args()
     rinex3 = args.rinex3
-    rinex2 = args.rinex2
 
-    rinex2 = args.rinex2
     gexe = g.gfz_version()
 
-    if args.gpsonly == None:
-        gpsonly = False
-    else:
+    # should use utils but don't have the time
+    gpsonly = False
+    if (args.gpsonly == 'True') or (args.gpsonly == 'T'):
         gpsonly = True
 
-    if args.dec == None:
+    if args.rinex2 is None:
+        station = rinex3[0:4].lower()
+        cyyyy = rinex3[12:16]
+        cdoy = rinex3[16:19]
+        rinex2 = station + cdoy + '0.' + cyyyy[2:4] + 'o'
+        print('Output filename ', rinex2)
+    else:
+        rinex2 = args.rinex2
+
+    if args.dec is None:
         dec = 1
     else:
         dec=args.dec
 
     if not os.path.exists(gexe):
         print('Required gfzrnx executable does not exist. Exiting.')
         sys.exit()
 
 
     if os.path.isfile(rinex3):
+        print('Your RINEX input file does exist:', rinex3)
+        if (rinex3[-2::] == 'gz'):
+            print('Must gunzip version 3 rinex')
+            subprocess.call(['gunzip', rinex3])
+            rinex3 = rinex3[0:-3]
         g.new_rinex3_rinex2(rinex3,rinex2,dec,gpsonly)
     else:
         print('ERROR: your input file does not exist:', rinex3)
         sys.exit()
 
     if os.path.isfile(rinex2):
         print('SUCCESS: new file created', rinex2)
```

### Comparing `gnssrefl-1.3.2/gnssrefl/rinex3_snr.py` & `gnssrefl-1.3.3/gnssrefl/rinex3_snr.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # -*- coding: utf-8 -*-
 """
 """
 import argparse
 import os
+import subprocess 
+import sys
+
 import gnssrefl.gps as g
 import gnssrefl.rinex2snr as r
-import sys
 
 def main():
     """
 
     Creates SNR file from RINEX 3 file that is stored locally
     Requires the gfzrnx executable to be available.
 
@@ -21,17 +23,23 @@
     orb : str
         optional orbit choice.  default is gbm
     """
 
     parser = argparse.ArgumentParser()
     parser.add_argument("rinex3", help="rinex3 filename", type=str)
     parser.add_argument("-orb", help="orbit choice", default='gbm',type=str)
+    parser.add_argument("-snr", help="SNR file ending (default is 66)", default=None,type=str)
 
 
     args = parser.parse_args()
+    if args.snr is None:
+        snr = '66'
+    else:
+        snr = int(args.snr)
+
     rinex3 = args.rinex3
     station = rinex3[0:4].lower()
     STATION = rinex3[0:4]
     year = rinex3[12:16]
     cdoy = rinex3[16:19] 
     idoy = int(cdoy)
 
@@ -52,21 +60,25 @@
         print('Required gfzrnx executable does not exist. Exiting.')
         sys.exit()
 
 
     # first step will be to translate to rinex2
 
     if os.path.isfile(rinex3):
-        #print('found version 3 rinex')
+        print('Found version 3 input file ')
+        if (rinex3[-2::] == 'gz'):
+            print('Must gunzip version 3 rinex')
+            subprocess.call(['gunzip', rinex3])
+            rinex3 = rinex3[0:-3]
         g.new_rinex3_rinex2(rinex3,rinex2)
     else:
         print('ERROR: your input file does not exist:', rinex3)
         sys.exit()
     if os.path.isfile(rinex2):
-        #print('found version 2 rinex')
+        print('found version 2 rinex')
         isnr = 66;  rate = 30; idoy = int(cdoy); iyear = int(year)
         rate = '30'; dec_rate = 0; archive = 'unavco' ; fortran = False; translator = 'hybrid'
         year_list = [iyear]; doy_list = [idoy]; rate = 'low';   nol = True; overwrite = False; srate = 30; mk = False; skipit = 1
         strip = False; stream = 'S'  ; bkg = 'IGS' # many of these are fake values because the file has already been translated to rinex2
         r.run_rinex2snr(station, year_list, doy_list, isnr, orbtype, rate,dec_rate,archive,fortran,nol,
                 overwrite,translator,srate,mk,skipit,stream,strip,bkg)
```

### Comparing `gnssrefl-1.3.2/gnssrefl/rinpy.py` & `gnssrefl-1.3.3/gnssrefl/rinpy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/rt_rinex3_snr.py` & `gnssrefl-1.3.3/gnssrefl/rt_rinex3_snr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/snow_functions.py` & `gnssrefl-1.3.3/gnssrefl/snow_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/snowdepth_cl.py` & `gnssrefl-1.3.3/gnssrefl/snowdepth_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/spline_functions.py` & `gnssrefl-1.3.3/gnssrefl/spline_functions.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/subdaily.py` & `gnssrefl-1.3.3/gnssrefl/subdaily.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/subdaily_cl.py` & `gnssrefl-1.3.3/gnssrefl/subdaily_cl.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/utils.py` & `gnssrefl-1.3.3/gnssrefl/utils.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/veg_multiyr.py` & `gnssrefl-1.3.3/gnssrefl/veg_multiyr.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/vwc.py` & `gnssrefl-1.3.3/gnssrefl/vwc.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/vwc_input.py` & `gnssrefl-1.3.3/gnssrefl/vwc_input.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/xyz2llh.py` & `gnssrefl-1.3.3/gnssrefl/xyz2llh.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/ydoy.py` & `gnssrefl-1.3.3/gnssrefl/ydoy.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl/ymd.py` & `gnssrefl-1.3.3/gnssrefl/ymd.py`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl.egg-info/PKG-INFO` & `gnssrefl-1.3.3/gnssrefl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: gnssrefl
-Version: 1.3.2
+Version: 1.3.3
 Summary: A GNSS reflectometry software package 
 Home-page: https://github.com/kristinemlarson/gnssrefl/
 Author: Kristine Larson
 Author-email: kristinem.larson@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gnssrefl
 
-**github version: 1.3.2** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
+**github version: 1.3.3** [![PyPI Version](https://img.shields.io/pypi/v/gnssrefl.svg)](https://pypi.python.org/pypi/gnssrefl) [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.5601495.svg)](http://dx.doi.org/10.5281/zenodo.5601495) [![Documentation Status](https://readthedocs.org/projects/gnssrefl/badge/?version=latest)](https://gnssrefl.readthedocs.io/en/latest/?badge=latest)
 
 Our documentation is now available [here.](https://gnssrefl.readthedocs.io/en/latest/)
 
 The [shortcourse registration page is live.](https://www.earthscope.org/event/2023-gnss-ir-short-course) 
 
 If you want to sign up for the GNSS-IR email list, please contact Kristine Larson.
```

### Comparing `gnssrefl-1.3.2/gnssrefl.egg-info/SOURCES.txt` & `gnssrefl-1.3.3/gnssrefl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/gnssrefl.egg-info/entry_points.txt` & `gnssrefl-1.3.3/gnssrefl.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/pyproject.toml` & `gnssrefl-1.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gnssrefl-1.3.2/setup.py` & `gnssrefl-1.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 requirements = ["numpy","wget","scipy","matplotlib","requests","progress","astropy","simplekml","earthscope-sdk"]
 setup(
     name="gnssrefl",
-    version="1.3.2",
+    version="1.3.3",
     author="Kristine Larson",
     author_email="kristinem.larson@gmail.com",
     description="A GNSS reflectometry software package ",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/kristinemlarson/gnssrefl/",
     packages=find_packages(),
```

### Comparing `gnssrefl-1.3.2/test/test_gps.py` & `gnssrefl-1.3.3/test/test_gps.py`

 * *Files identical despite different names*

