# Comparing `tmp/skyproj-1.0.2.tar.gz` & `tmp/skyproj-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skyproj-1.0.2.tar", last modified: Wed Jan 18 20:44:19 2023, max compression
+gzip compressed data, was "skyproj-1.0.3.tar", last modified: Thu Apr 13 18:27:40 2023, max compression
```

## Comparing `skyproj-1.0.2.tar` & `skyproj-1.0.3.tar`

### file list

```diff
@@ -1,163 +1,164 @@
-drwxr-xr-x   0 erykoff  (10646) ki        (1092)        0 2023-01-18 20:44:19.593485 skyproj-1.0.2/
-drwxr-xr-x   0 erykoff  (10646) ki        (1092)        0 2023-01-18 20:44:19.468484 skyproj-1.0.2/.github/
-drwxr-xr-x   0 erykoff  (10646) ki        (1092)        0 2023-01-18 20:44:19.470484 skyproj-1.0.2/.github/workflows/
--rw-r--r--   0 erykoff  (10646) ki        (1092)     1460 2023-01-18 20:43:24.000000 skyproj-1.0.2/.github/workflows/python-package.yml
--rw-r--r--   0 erykoff  (10646) ki        (1092)     1802 2022-01-11 16:25:11.000000 skyproj-1.0.2/.gitignore
--rw-r--r--   0 erykoff  (10646) ki        (1092)     1515 2022-01-11 16:25:11.000000 skyproj-1.0.2/LICENSE
--rw-r--r--   0 erykoff  (10646) ki        (1092)       59 2022-01-11 20:27:54.000000 skyproj-1.0.2/MANIFEST.in
--rw-r--r--   0 erykoff  (10646) ki        (1092)     2076 2023-01-18 20:44:19.593485 skyproj-1.0.2/PKG-INFO
--rw-r--r--   0 erykoff  (10646) ki        (1092)     1445 2022-01-12 19:57:18.000000 skyproj-1.0.2/README.md
-drwxr-xr-x   0 erykoff  (10646) ki        (1092)        0 2023-01-18 20:44:19.473484 skyproj-1.0.2/docs/
--rw-r--r--   0 erykoff  (10646) ki        (1092)      634 2022-05-04 21:11:42.000000 skyproj-1.0.2/docs/Makefile
--rw-r--r--   0 erykoff  (10646) ki        (1092)     9956 2022-05-13 21:45:01.000000 skyproj-1.0.2/docs/basic_interface.rst
--rw-r--r--   0 erykoff  (10646) ki        (1092)     3374 2022-05-04 21:11:42.000000 skyproj-1.0.2/docs/conf.py
-drwxr-xr-x   0 erykoff  (10646) ki        (1092)        0 2023-01-18 20:44:19.492484 skyproj-1.0.2/docs/images/
--rw-r--r--   0 erykoff  (10646) ki        (1092)    94103 2022-10-12 16:21:25.000000 skyproj-1.0.2/docs/images/AlbersSkyproj_with_indicatrix.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    43028 2022-05-04 21:11:42.000000 skyproj-1.0.2/docs/images/BLISS_survey.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    50903 2022-05-04 21:11:42.000000 skyproj-1.0.2/docs/images/DECaLS_survey.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    93987 2022-10-12 16:21:25.000000 skyproj-1.0.2/docs/images/DESAlbers_survey_with_indicatrices.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    51893 2022-10-12 16:21:25.000000 skyproj-1.0.2/docs/images/DES_survey.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    73327 2022-10-12 16:21:25.000000 skyproj-1.0.2/docs/images/DES_survey_with_indicatrices.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    78912 2022-05-04 21:11:42.000000 skyproj-1.0.2/docs/images/EqualEarthSkyproj_with_indicatrices.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    63405 2022-05-04 21:11:42.000000 skyproj-1.0.2/docs/images/GnomonicSkyproj_with_indicatrix.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    98133 2022-05-04 21:11:42.000000 skyproj-1.0.2/docs/images/HammerSkyproj_with_indicatrices.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    90522 2022-05-04 21:11:42.000000 skyproj-1.0.2/docs/images/LaeaSkyproj_with_indicatrices.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    65432 2022-05-04 21:11:42.000000 skyproj-1.0.2/docs/images/MagLiTeS_survey.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    81023 2022-05-04 21:11:42.000000 skyproj-1.0.2/docs/images/McBrydeSkyproj_with_indicatrices.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    88217 2022-05-04 21:11:42.000000 skyproj-1.0.2/docs/images/MollweideSkyproj_with_indicatrices.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    79466 2022-05-04 21:11:42.000000 skyproj-1.0.2/docs/images/ObliqueMollweideSkyproj.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    52120 2022-05-04 21:11:42.000000 skyproj-1.0.2/docs/images/Skyproj_with_indicatrices.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)   370290 2022-05-04 21:11:42.000000 skyproj-1.0.2/docs/images/healsparse_one.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    81432 2022-05-04 21:11:42.000000 skyproj-1.0.2/docs/images/healsparse_two.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    47640 2022-06-08 15:03:40.000000 skyproj-1.0.2/docs/images/healsparse_valid_pixels.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    83072 2022-05-04 21:11:42.000000 skyproj-1.0.2/docs/images/hpxbin.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)   106704 2022-05-04 21:11:42.000000 skyproj-1.0.2/docs/images/hpxbin_reproject.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    81719 2022-05-04 21:11:42.000000 skyproj-1.0.2/docs/images/lines_and_polygons_0.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    80741 2022-05-04 21:11:42.000000 skyproj-1.0.2/docs/images/milky_way.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    71306 2022-05-04 21:11:42.000000 skyproj-1.0.2/docs/images/milky_way_galactic.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)     3356 2022-05-04 21:11:42.000000 skyproj-1.0.2/docs/index.rst
--rw-r--r--   0 erykoff  (10646) ki        (1092)      812 2022-05-04 21:11:42.000000 skyproj-1.0.2/docs/install.rst
--rw-r--r--   0 erykoff  (10646) ki        (1092)      795 2022-05-04 21:11:42.000000 skyproj-1.0.2/docs/make.bat
--rw-r--r--   0 erykoff  (10646) ki        (1092)     5884 2022-10-12 16:21:25.000000 skyproj-1.0.2/docs/maps.rst
--rw-r--r--   0 erykoff  (10646) ki        (1092)      597 2022-05-04 21:11:42.000000 skyproj-1.0.2/docs/modules.rst
--rw-r--r--   0 erykoff  (10646) ki        (1092)     9930 2022-10-12 16:21:25.000000 skyproj-1.0.2/docs/projections.rst
--rw-r--r--   0 erykoff  (10646) ki        (1092)      451 2022-05-04 21:11:42.000000 skyproj-1.0.2/docs/quickstart.rst
--rw-r--r--   0 erykoff  (10646) ki        (1092)     4269 2022-10-12 16:21:25.000000 skyproj-1.0.2/docs/surveys.rst
--rw-r--r--   0 erykoff  (10646) ki        (1092)      183 2022-01-11 20:27:54.000000 skyproj-1.0.2/pyproject.toml
--rw-r--r--   0 erykoff  (10646) ki        (1092)      107 2022-10-12 16:21:25.000000 skyproj-1.0.2/requirements.txt
--rw-r--r--   0 erykoff  (10646) ki        (1092)     1083 2023-01-18 20:44:19.594485 skyproj-1.0.2/setup.cfg
-drwxr-xr-x   0 erykoff  (10646) ki        (1092)        0 2023-01-18 20:44:19.510485 skyproj-1.0.2/skyproj/
--rw-r--r--   0 erykoff  (10646) ki        (1092)      384 2022-05-04 21:11:42.000000 skyproj-1.0.2/skyproj/__init__.py
--rw-r--r--   0 erykoff  (10646) ki        (1092)    63236 2023-01-18 20:43:24.000000 skyproj-1.0.2/skyproj/_skyproj.py
-drwxr-xr-x   0 erykoff  (10646) ki        (1092)        0 2023-01-18 20:44:19.517485 skyproj-1.0.2/skyproj/data/
--rw-r--r--   0 erykoff  (10646) ki        (1092)     1725 2022-01-11 16:25:11.000000 skyproj-1.0.2/skyproj/data/bliss-poly.txt
--rw-r--r--   0 erykoff  (10646) ki        (1092)    12733 2022-01-11 16:25:11.000000 skyproj-1.0.2/skyproj/data/ccd_corners_xy_fill.dat
--rw-r--r--   0 erykoff  (10646) ki        (1092)   392256 2022-01-11 16:25:11.000000 skyproj-1.0.2/skyproj/data/constellationsANDstars.json
--rw-r--r--   0 erykoff  (10646) ki        (1092)     2041 2022-01-11 16:25:11.000000 skyproj-1.0.2/skyproj/data/decals-poly.txt
--rw-r--r--   0 erykoff  (10646) ki        (1092)     1183 2022-01-11 16:25:11.000000 skyproj-1.0.2/skyproj/data/derosita-poly.txt
--rw-r--r--   0 erykoff  (10646) ki        (1092)    13851 2022-01-11 16:25:11.000000 skyproj-1.0.2/skyproj/data/des-round13-poly.txt
--rw-r--r--   0 erykoff  (10646) ki        (1092)    13981 2022-01-11 16:25:11.000000 skyproj-1.0.2/skyproj/data/des-round17-poly.txt
--rw-r--r--   0 erykoff  (10646) ki        (1092)     9947 2022-02-17 17:14:54.000000 skyproj-1.0.2/skyproj/data/des-round19-poly.txt
--rw-r--r--   0 erykoff  (10646) ki        (1092)      245 2022-01-11 16:25:11.000000 skyproj-1.0.2/skyproj/data/macho_corners_xy.dat
--rw-r--r--   0 erykoff  (10646) ki        (1092)     4520 2022-01-11 16:25:11.000000 skyproj-1.0.2/skyproj/data/maglites-poly.txt
--rw-r--r--   0 erykoff  (10646) ki        (1092)    16927 2022-01-11 16:25:11.000000 skyproj-1.0.2/skyproj/data/smash_fields_final.txt
--rw-r--r--   0 erykoff  (10646) ki        (1092)     8062 2022-10-12 16:21:25.000000 skyproj-1.0.2/skyproj/hpx_utils.py
--rw-r--r--   0 erykoff  (10646) ki        (1092)     8141 2022-06-08 16:32:07.000000 skyproj-1.0.2/skyproj/mpl_utils.py
--rw-r--r--   0 erykoff  (10646) ki        (1092)     5640 2022-03-14 15:48:04.000000 skyproj-1.0.2/skyproj/projections_alt.py
--rw-r--r--   0 erykoff  (10646) ki        (1092)    10476 2023-01-17 18:27:31.000000 skyproj-1.0.2/skyproj/skyaxes.py
--rw-r--r--   0 erykoff  (10646) ki        (1092)    13637 2022-10-12 16:21:25.000000 skyproj-1.0.2/skyproj/skycrs.py
--rw-r--r--   0 erykoff  (10646) ki        (1092)     7743 2022-10-12 16:21:25.000000 skyproj-1.0.2/skyproj/skyproj.py
--rw-r--r--   0 erykoff  (10646) ki        (1092)    62403 2022-03-14 15:48:29.000000 skyproj-1.0.2/skyproj/skyproj_alt.py
--rw-r--r--   0 erykoff  (10646) ki        (1092)     6651 2022-10-12 19:51:08.000000 skyproj-1.0.2/skyproj/survey.py
--rw-r--r--   0 erykoff  (10646) ki        (1092)    12888 2022-05-16 20:46:48.000000 skyproj-1.0.2/skyproj/transforms.py
--rw-r--r--   0 erykoff  (10646) ki        (1092)    10201 2022-04-06 18:45:02.000000 skyproj-1.0.2/skyproj/transforms_noodling.py
--rw-r--r--   0 erykoff  (10646) ki        (1092)     3507 2022-03-14 15:48:39.000000 skyproj-1.0.2/skyproj/utils.py
-drwxr-xr-x   0 erykoff  (10646) ki        (1092)        0 2023-01-18 20:44:19.512485 skyproj-1.0.2/skyproj.egg-info/
--rw-r--r--   0 erykoff  (10646) ki        (1092)     2076 2023-01-18 20:44:19.000000 skyproj-1.0.2/skyproj.egg-info/PKG-INFO
--rw-r--r--   0 erykoff  (10646) ki        (1092)     4447 2023-01-18 20:44:19.000000 skyproj-1.0.2/skyproj.egg-info/SOURCES.txt
--rw-r--r--   0 erykoff  (10646) ki        (1092)        1 2023-01-18 20:44:19.000000 skyproj-1.0.2/skyproj.egg-info/dependency_links.txt
--rw-r--r--   0 erykoff  (10646) ki        (1092)       65 2023-01-18 20:44:19.000000 skyproj-1.0.2/skyproj.egg-info/requires.txt
--rw-r--r--   0 erykoff  (10646) ki        (1092)        8 2023-01-18 20:44:19.000000 skyproj-1.0.2/skyproj.egg-info/top_level.txt
--rw-r--r--   0 erykoff  (10646) ki        (1092)        1 2022-01-11 19:11:15.000000 skyproj-1.0.2/skyproj.egg-info/zip-safe
-drwxr-xr-x   0 erykoff  (10646) ki        (1092)        0 2023-01-18 20:44:19.521484 skyproj-1.0.2/tests/
-drwxr-xr-x   0 erykoff  (10646) ki        (1092)        0 2023-01-18 20:44:19.582485 skyproj-1.0.2/tests/data/
--rw-r--r--   0 erykoff  (10646) ki        (1092)    43028 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/BLISS_survey.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    50903 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/DECaLS_survey.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    71908 2022-10-12 16:21:25.000000 skyproj-1.0.2/tests/data/DESAlbers_survey.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    51893 2022-10-12 16:21:25.000000 skyproj-1.0.2/tests/data/DES_survey.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    65432 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/MagLiTeS_survey.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    73426 2022-10-12 16:21:25.000000 skyproj-1.0.2/tests/data/aea_-15.0_-45.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    61039 2022-10-12 16:21:25.000000 skyproj-1.0.2/tests/data/aea_-20.0_15.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    73579 2022-10-12 16:21:25.000000 skyproj-1.0.2/tests/data/aea_15.0_45.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    75485 2022-10-12 16:21:25.000000 skyproj-1.0.2/tests/data/aea_full_-100.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    73579 2022-10-12 16:21:25.000000 skyproj-1.0.2/tests/data/aea_full_0.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    75100 2022-10-12 16:21:25.000000 skyproj-1.0.2/tests/data/aea_full_100.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    73164 2022-10-12 16:21:25.000000 skyproj-1.0.2/tests/data/aea_full_180.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    47242 2022-10-12 16:21:25.000000 skyproj-1.0.2/tests/data/aea_zoom.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    30661 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/cyl_full_-100.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    29403 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/cyl_full_0.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    30834 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/cyl_full_100.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    30655 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/cyl_full_180.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    52120 2022-05-04 21:11:42.000000 skyproj-1.0.2/tests/data/cyl_tissot.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    32681 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/cyl_zoom.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    67611 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/eqearth_full_-100.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    62134 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/eqearth_full_0.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    67748 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/eqearth_full_100.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    63894 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/eqearth_full_180.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    48828 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/eqearth_zoom.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    52594 2022-04-14 14:50:28.000000 skyproj-1.0.2/tests/data/gnom_-120.0_75.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    34851 2022-04-14 14:50:28.000000 skyproj-1.0.2/tests/data/gnom_0.0_0.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    52795 2022-04-14 14:50:28.000000 skyproj-1.0.2/tests/data/gnom_120.0_-75.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    84628 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/hammer_full_-100.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    80024 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/hammer_full_0.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    84424 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/hammer_full_100.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    80202 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/hammer_full_180.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    45158 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/hammer_zoom.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    50879 2022-10-12 16:21:25.000000 skyproj-1.0.2/tests/data/healsparse_bool.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    47810 2022-06-08 15:03:40.000000 skyproj-1.0.2/tests/data/healsparse_bool_valid_pixels.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)   370290 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/healsparse_one.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)   112741 2022-06-08 15:03:40.000000 skyproj-1.0.2/tests/data/healsparse_rec_array.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    72138 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/healsparse_three.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    81432 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/healsparse_two.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    47640 2022-06-08 15:03:40.000000 skyproj-1.0.2/tests/data/healsparse_valid_pixels.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    49749 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/healsparse_wide_one.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    83072 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/hpxbin.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    39749 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/laea_zoom.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    84779 2022-05-13 21:45:01.000000 skyproj-1.0.2/tests/data/lines_and_polygons_0.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    85036 2022-05-13 21:45:01.000000 skyproj-1.0.2/tests/data/lines_and_polygons_180.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    92160 2022-04-14 14:50:28.000000 skyproj-1.0.2/tests/data/lines_and_polygons_obmoll_0.0_45.0_-90.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    93775 2022-04-14 14:50:28.000000 skyproj-1.0.2/tests/data/lines_and_polygons_obmoll_100.0_80.0_-90.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    70643 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/mbtfpq_full_-100.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    65238 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/mbtfpq_full_0.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    70846 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/mbtfpq_full_100.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    66241 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/mbtfpq_full_180.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    66850 2022-06-14 21:38:03.000000 skyproj-1.0.2/tests/data/mbtfpq_gaptest.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    81023 2022-05-04 21:11:42.000000 skyproj-1.0.2/tests/data/mbtfpq_tissot.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    37300 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/mbtfpq_zoom.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    80741 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/milky_way.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    71306 2022-05-04 21:11:42.000000 skyproj-1.0.2/tests/data/milky_way_galactic.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    75589 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/moll_full_-100.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    71695 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/moll_full_0.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    75701 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/moll_full_100.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    72151 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/moll_full_180.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    73034 2022-06-14 21:38:03.000000 skyproj-1.0.2/tests/data/moll_gaptest.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    37105 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/moll_zoom.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    79466 2022-04-14 14:50:28.000000 skyproj-1.0.2/tests/data/obmoll_0.0_45.0_-90.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    80295 2022-04-14 14:50:28.000000 skyproj-1.0.2/tests/data/obmoll_100.0_80.0_0.0.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)    45537 2022-03-14 15:48:39.000000 skyproj-1.0.2/tests/data/plotting_routines.png
--rw-r--r--   0 erykoff  (10646) ki        (1092)     1576 2022-10-12 16:21:25.000000 skyproj-1.0.2/tests/test_healpix_binning.py
--rw-r--r--   0 erykoff  (10646) ki        (1092)    16706 2023-01-18 20:43:24.000000 skyproj-1.0.2/tests/test_healpix_maps.py
--rw-r--r--   0 erykoff  (10646) ki        (1092)     4090 2022-05-13 21:45:01.000000 skyproj-1.0.2/tests/test_lines_polygons.py
--rw-r--r--   0 erykoff  (10646) ki        (1092)     1359 2022-05-04 21:11:42.000000 skyproj-1.0.2/tests/test_milky_way.py
--rw-r--r--   0 erykoff  (10646) ki        (1092)     1486 2022-05-04 21:11:42.000000 skyproj-1.0.2/tests/test_plotting.py
--rw-r--r--   0 erykoff  (10646) ki        (1092)     2017 2022-05-04 21:11:42.000000 skyproj-1.0.2/tests/test_projections.py
--rw-r--r--   0 erykoff  (10646) ki        (1092)     6693 2022-10-12 16:21:25.000000 skyproj-1.0.2/tests/test_skyproj.py
--rw-r--r--   0 erykoff  (10646) ki        (1092)     1462 2022-10-12 16:21:25.000000 skyproj-1.0.2/tests/test_survey.py
--rw-r--r--   0 erykoff  (10646) ki        (1092)      895 2022-05-04 21:11:42.000000 skyproj-1.0.2/tests/test_tissot.py
--rw-r--r--   0 erykoff  (10646) ki        (1092)     1515 2022-01-11 16:25:11.000000 skyproj-1.0.2/tests/test_tutorial.py
--rw-r--r--   0 erykoff  (10646) ki        (1092)      763 2022-01-11 16:25:11.000000 skyproj-1.0.2/tests/test_utils.py
-drwxr-xr-x   0 erykoff  (10646) ki        (1092)        0 2023-01-18 20:44:19.591485 skyproj-1.0.2/tutorial/
--rw-r--r--   0 erykoff  (10646) ki        (1092)      318 2022-01-12 19:57:18.000000 skyproj-1.0.2/tutorial/README.md
--rw-r--r--   0 erykoff  (10646) ki        (1092)   432870 2022-05-04 21:11:42.000000 skyproj-1.0.2/tutorial/tutorial_baseclass.ipynb
--rw-r--r--   0 erykoff  (10646) ki        (1092)  1933628 2022-10-12 16:21:25.000000 skyproj-1.0.2/tutorial/tutorial_healsparse.ipynb
--rw-r--r--   0 erykoff  (10646) ki        (1092)   551528 2022-05-04 21:11:42.000000 skyproj-1.0.2/tutorial/tutorial_surveys.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:27:40.636919 skyproj-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:27:40.604918 skyproj-1.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:27:40.608918 skyproj-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-13 18:27:28.000000 skyproj-1.0.3/.github/workflows/python-package-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-13 18:27:28.000000 skyproj-1.0.3/.github/workflows/python-package-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-13 18:27:28.000000 skyproj-1.0.3/.github/workflows/python-package-push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-13 18:27:28.000000 skyproj-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-13 18:27:28.000000 skyproj-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-13 18:27:28.000000 skyproj-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-13 18:27:40.636919 skyproj-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-13 18:27:28.000000 skyproj-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:27:40.608918 skyproj-1.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/basic_interface.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:27:40.612918 skyproj-1.0.3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    94103 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/images/AlbersSkyproj_with_indicatrix.png
+-rw-r--r--   0 runner    (1001) docker     (123)    43028 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/images/BLISS_survey.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50903 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/images/DECaLS_survey.png
+-rw-r--r--   0 runner    (1001) docker     (123)    93987 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/images/DESAlbers_survey_with_indicatrices.png
+-rw-r--r--   0 runner    (1001) docker     (123)    51893 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/images/DES_survey.png
+-rw-r--r--   0 runner    (1001) docker     (123)    73327 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/images/DES_survey_with_indicatrices.png
+-rw-r--r--   0 runner    (1001) docker     (123)    78912 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/images/EqualEarthSkyproj_with_indicatrices.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63405 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/images/GnomonicSkyproj_with_indicatrix.png
+-rw-r--r--   0 runner    (1001) docker     (123)    98133 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/images/HammerSkyproj_with_indicatrices.png
+-rw-r--r--   0 runner    (1001) docker     (123)    90522 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/images/LaeaSkyproj_with_indicatrices.png
+-rw-r--r--   0 runner    (1001) docker     (123)    65432 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/images/MagLiTeS_survey.png
+-rw-r--r--   0 runner    (1001) docker     (123)    81023 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/images/McBrydeSkyproj_with_indicatrices.png
+-rw-r--r--   0 runner    (1001) docker     (123)    88217 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/images/MollweideSkyproj_with_indicatrices.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79466 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/images/ObliqueMollweideSkyproj.png
+-rw-r--r--   0 runner    (1001) docker     (123)    52120 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/images/Skyproj_with_indicatrices.png
+-rw-r--r--   0 runner    (1001) docker     (123)   370290 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/images/healsparse_one.png
+-rw-r--r--   0 runner    (1001) docker     (123)    81432 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/images/healsparse_two.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47640 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/images/healsparse_valid_pixels.png
+-rw-r--r--   0 runner    (1001) docker     (123)    83072 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/images/hpxbin.png
+-rw-r--r--   0 runner    (1001) docker     (123)   106704 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/images/hpxbin_reproject.png
+-rw-r--r--   0 runner    (1001) docker     (123)    81719 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/images/lines_and_polygons_0.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    80741 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/images/milky_way.png
+-rw-r--r--   0 runner    (1001) docker     (123)    71306 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/images/milky_way_galactic.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68894 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/images/skyproj_full_override_sizes.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/maps.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9930 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/projections.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-04-13 18:27:28.000000 skyproj-1.0.3/docs/surveys.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-13 18:27:28.000000 skyproj-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-13 18:27:28.000000 skyproj-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-13 18:27:40.636919 skyproj-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:27:40.616918 skyproj-1.0.3/skyproj/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-13 18:27:28.000000 skyproj-1.0.3/skyproj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63679 2023-04-13 18:27:28.000000 skyproj-1.0.3/skyproj/_skyproj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:27:40.616918 skyproj-1.0.3/skyproj/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-13 18:27:28.000000 skyproj-1.0.3/skyproj/data/bliss-poly.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-04-13 18:27:28.000000 skyproj-1.0.3/skyproj/data/ccd_corners_xy_fill.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   392256 2023-04-13 18:27:28.000000 skyproj-1.0.3/skyproj/data/constellationsANDstars.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-04-13 18:27:28.000000 skyproj-1.0.3/skyproj/data/decals-poly.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-13 18:27:28.000000 skyproj-1.0.3/skyproj/data/derosita-poly.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13851 2023-04-13 18:27:28.000000 skyproj-1.0.3/skyproj/data/des-round13-poly.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13981 2023-04-13 18:27:28.000000 skyproj-1.0.3/skyproj/data/des-round17-poly.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-04-13 18:27:28.000000 skyproj-1.0.3/skyproj/data/des-round19-poly.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-13 18:27:28.000000 skyproj-1.0.3/skyproj/data/macho_corners_xy.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-04-13 18:27:28.000000 skyproj-1.0.3/skyproj/data/maglites-poly.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16927 2023-04-13 18:27:28.000000 skyproj-1.0.3/skyproj/data/smash_fields_final.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-04-13 18:27:28.000000 skyproj-1.0.3/skyproj/hpx_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-04-13 18:27:28.000000 skyproj-1.0.3/skyproj/mpl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-04-13 18:27:28.000000 skyproj-1.0.3/skyproj/skyaxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-04-13 18:27:28.000000 skyproj-1.0.3/skyproj/skycrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-04-13 18:27:28.000000 skyproj-1.0.3/skyproj/skyproj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-13 18:27:28.000000 skyproj-1.0.3/skyproj/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12888 2023-04-13 18:27:28.000000 skyproj-1.0.3/skyproj/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-13 18:27:28.000000 skyproj-1.0.3/skyproj/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:27:40.616918 skyproj-1.0.3/skyproj.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-13 18:27:40.000000 skyproj-1.0.3/skyproj.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-13 18:27:40.000000 skyproj-1.0.3/skyproj.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:27:40.000000 skyproj-1.0.3/skyproj.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 18:27:40.000000 skyproj-1.0.3/skyproj.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 18:27:40.000000 skyproj-1.0.3/skyproj.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:27:40.000000 skyproj-1.0.3/skyproj.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:27:40.620918 skyproj-1.0.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:27:40.632919 skyproj-1.0.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    43028 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/BLISS_survey.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50903 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/DECaLS_survey.png
+-rw-r--r--   0 runner    (1001) docker     (123)    71908 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/DESAlbers_survey.png
+-rw-r--r--   0 runner    (1001) docker     (123)    51893 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/DES_survey.png
+-rw-r--r--   0 runner    (1001) docker     (123)    65432 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/MagLiTeS_survey.png
+-rw-r--r--   0 runner    (1001) docker     (123)    73426 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/aea_-15.0_-45.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    61039 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/aea_-20.0_15.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    73579 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/aea_15.0_45.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    75485 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/aea_full_-100.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    73579 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/aea_full_0.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    75100 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/aea_full_100.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    73164 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/aea_full_180.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47242 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/aea_zoom.png
+-rw-r--r--   0 runner    (1001) docker     (123)    30661 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/cyl_full_-100.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29403 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/cyl_full_0.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    30834 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/cyl_full_100.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    30655 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/cyl_full_180.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    52120 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/cyl_tissot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32681 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/cyl_zoom.png
+-rw-r--r--   0 runner    (1001) docker     (123)    67611 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/eqearth_full_-100.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    62134 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/eqearth_full_0.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    67748 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/eqearth_full_100.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63894 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/eqearth_full_180.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    48828 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/eqearth_zoom.png
+-rw-r--r--   0 runner    (1001) docker     (123)    52594 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/gnom_-120.0_75.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34851 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/gnom_0.0_0.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    52795 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/gnom_120.0_-75.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    84628 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/hammer_full_-100.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    80024 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/hammer_full_0.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    84424 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/hammer_full_100.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    80202 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/hammer_full_180.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45158 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/hammer_zoom.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50879 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/healsparse_bool.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47810 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/healsparse_bool_valid_pixels.png
+-rw-r--r--   0 runner    (1001) docker     (123)   370290 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/healsparse_one.png
+-rw-r--r--   0 runner    (1001) docker     (123)   112741 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/healsparse_rec_array.png
+-rw-r--r--   0 runner    (1001) docker     (123)    72138 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/healsparse_three.png
+-rw-r--r--   0 runner    (1001) docker     (123)    81432 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/healsparse_two.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47640 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/healsparse_valid_pixels.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49749 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/healsparse_wide_one.png
+-rw-r--r--   0 runner    (1001) docker     (123)    83072 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/hpxbin.png
+-rw-r--r--   0 runner    (1001) docker     (123)    39749 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/laea_zoom.png
+-rw-r--r--   0 runner    (1001) docker     (123)    84779 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/lines_and_polygons_0.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    85036 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/lines_and_polygons_180.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    92160 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/lines_and_polygons_obmoll_0.0_45.0_-90.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    93775 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/lines_and_polygons_obmoll_100.0_80.0_-90.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    70643 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/mbtfpq_full_-100.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    65238 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/mbtfpq_full_0.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    70846 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/mbtfpq_full_100.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    66241 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/mbtfpq_full_180.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    66850 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/mbtfpq_gaptest.png
+-rw-r--r--   0 runner    (1001) docker     (123)    81023 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/mbtfpq_tissot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37300 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/mbtfpq_zoom.png
+-rw-r--r--   0 runner    (1001) docker     (123)    80741 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/milky_way.png
+-rw-r--r--   0 runner    (1001) docker     (123)    71306 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/milky_way_galactic.png
+-rw-r--r--   0 runner    (1001) docker     (123)    75589 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/moll_full_-100.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    71695 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/moll_full_0.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    75701 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/moll_full_100.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    72151 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/moll_full_180.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    73034 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/moll_gaptest.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37105 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/moll_zoom.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79466 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/obmoll_0.0_45.0_-90.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    80295 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/obmoll_100.0_80.0_0.0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45537 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/plotting_routines.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68894 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/data/skyproj_full_override_sizes.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/test_healpix_binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16706 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/test_healpix_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/test_lines_polygons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/test_milky_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/test_projections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/test_skyproj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/test_survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/test_tissot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/test_tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-13 18:27:28.000000 skyproj-1.0.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:27:40.636919 skyproj-1.0.3/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-13 18:27:28.000000 skyproj-1.0.3/tutorial/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   432870 2023-04-13 18:27:28.000000 skyproj-1.0.3/tutorial/tutorial_baseclass.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1933628 2023-04-13 18:27:28.000000 skyproj-1.0.3/tutorial/tutorial_healsparse.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   551528 2023-04-13 18:27:28.000000 skyproj-1.0.3/tutorial/tutorial_surveys.ipynb
```

### Comparing `skyproj-1.0.2/.github/workflows/python-package.yml` & `skyproj-1.0.3/.github/workflows/python-package-pr.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # This workflow will install Python dependencies, run tests and lint with a variety of Python versions
 # For more information see: https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions
 
-name: Build and Test
+name: Build and Test (PR)
 
 on:
-  push:
-    branches: [ '**' ]
   pull_request:
     branches: [ '**' ]
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
@@ -30,15 +28,15 @@
         miniforge-version: latest
         miniforge-variant: Mambaforge
 
     - name: Configure conda and install code
       shell: bash -l {0}
       run: |
         mamba config --set always_yes yes
-        mamba install --quiet numpy "astropy>=4.0" "matplotlib${{ matrix.matplotlib-version }}" hpgeom setuptools_scm setuptools_scm_git_archive healsparse "pyproj>=3.1" flake8 pytest jupyter nbconvert
+        mamba install numpy "astropy>=4.0" "matplotlib${{ matrix.matplotlib-version }}" hpgeom setuptools_scm setuptools_scm_git_archive healsparse "pyproj>=3.1" flake8 pytest jupyter "nbconvert<7"
         python -m pip install --no-deps .
 
     - name: Lint with flake8
       shell: bash -l {0}
       run: |
         # stop the build if it fails flake8 with default setup.cfg
         flake8 . --count --show-source --statistics
```

### Comparing `skyproj-1.0.2/.gitignore` & `skyproj-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/LICENSE` & `skyproj-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/PKG-INFO` & `skyproj-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skyproj
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python tools for making sky projections and maps
 Home-page: https://github.com/lsstdesc/skyproj
 Author: Eli Rykoff, Alex Drlica-Wagner, and others
 Author-email: erykoff@stanford.edu
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `skyproj-1.0.2/README.md` & `skyproj-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/docs/Makefile` & `skyproj-1.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/docs/basic_interface.rst` & `skyproj-1.0.3/docs/basic_interface.rst`

 * *Files 6% similar despite different names*

```diff
@@ -185,14 +185,15 @@
 Plotting `HealSparse` maps can be performed with the :code:`draw_hspmap()` method on a :code:`Skyproj()` subclass.
 The default setting for drawing a map is to automatically zoom in on the ra/dec range of the map to be plotted.
 For speed and efficiency, map plotting in `SkyProj` is performed by first rasterizing the input map at a resolution appropriate for the given plot.
 For more details on plotting :code:`HealSparse` and :code:`HEALPix` maps, see :ref:`maps`.
 
 .. code-block :: python
 
+    import matplotlib.pyplot as plt
     import numpy as np
     import healsparse as hsp
     import skyproj
 
     # Make a square noise field.
     hspmap = hsp.HealSparseMap.make_empty(32, 4096, np.float32)
     poly = hsp.geom.Polygon(ra=[0.0, 10.0, 10.0, 0.0], dec=[0.0, 0.0, 10.0, 10.0], value=1.0)
@@ -227,7 +228,40 @@
 
 In addition, the default behavior on zoom is for the map to retain the original projection.
 When zooming in to a small region far from the central longitude this can lead to large distortion (as seen in the Tissot Indicatrices of the McBryde projection above).
 There is currently experimental support for reprojecting on the current displayed central longitude by hitting :code:`R` (for Reproject) when the mouse is within the plot window.
 Performing the reprojection may be slow, and there are some cases where it can go awry.
 When the zoom is below 1 degree across the reprojection will use a Gnomonic (tangent-plane) projection which has sufficiently small distortion at all locations.
 
+
+Plotting Customization
+----------------------
+
+Much of the plotting functionality is decided by `SkyProj` itself.
+However, there is a lot of customization available.
+The fonts, font sizes, tick label sizes, etc, are all determined by the :code:`matplotlib` RC parameter dictionary.
+A few of these in particular should be highlighted:
+
+* :code:`xticks.labelsize`: Sets the label size for the x (longitude) ticks on the plot.
+* :code:`yticks.labelsize`: Sets the label size for the y (latitude) ticks on the plot.
+* :code:`axes.linewidth`: Sets the width of the boundary of the full plot.
+* :code:`axes.labelsize`: Sets the size of the x/y (lon/lat) labels; this will default to 16 unless specifically overridden with an :code:`rcparams`.
+
+These values (and any others) can be overridden at the time of map instantiation with a temporary dictionary, like so:
+
+.. code-block :: python
+
+    import matplotlib.pyplot as plt
+    import skyproj
+
+    # These values are comically exaggerated for effect.
+    rcparams = {'xtick.labelsize': 20,
+                'ytick.labelsize': 4,
+                'axes.linewidth': 5}
+
+    fig, ax = plt.subplots(figsize=(8, 5))
+    sp = skyproj.McBrydeSkyproj(ax=ax, rcparams=rcparams)
+    plt.show()
+
+.. image:: images/skyproj_full_override_sizes.png
+   :width: 600
+   :alt: McBrydeSkyproj with comically exaggerated label size overrides.
```

### Comparing `skyproj-1.0.2/docs/conf.py` & `skyproj-1.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/docs/images/AlbersSkyproj_with_indicatrix.png` & `skyproj-1.0.3/docs/images/AlbersSkyproj_with_indicatrix.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/docs/images/BLISS_survey.png` & `skyproj-1.0.3/docs/images/BLISS_survey.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/docs/images/DECaLS_survey.png` & `skyproj-1.0.3/docs/images/DECaLS_survey.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/docs/images/DESAlbers_survey_with_indicatrices.png` & `skyproj-1.0.3/docs/images/DESAlbers_survey_with_indicatrices.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/docs/images/DES_survey.png` & `skyproj-1.0.3/docs/images/DES_survey.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/docs/images/DES_survey_with_indicatrices.png` & `skyproj-1.0.3/docs/images/DES_survey_with_indicatrices.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/docs/images/EqualEarthSkyproj_with_indicatrices.png` & `skyproj-1.0.3/docs/images/EqualEarthSkyproj_with_indicatrices.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/docs/images/GnomonicSkyproj_with_indicatrix.png` & `skyproj-1.0.3/docs/images/GnomonicSkyproj_with_indicatrix.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/docs/images/HammerSkyproj_with_indicatrices.png` & `skyproj-1.0.3/docs/images/HammerSkyproj_with_indicatrices.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/docs/images/LaeaSkyproj_with_indicatrices.png` & `skyproj-1.0.3/docs/images/LaeaSkyproj_with_indicatrices.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/docs/images/MagLiTeS_survey.png` & `skyproj-1.0.3/docs/images/MagLiTeS_survey.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/docs/images/McBrydeSkyproj_with_indicatrices.png` & `skyproj-1.0.3/docs/images/McBrydeSkyproj_with_indicatrices.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/docs/images/MollweideSkyproj_with_indicatrices.png` & `skyproj-1.0.3/docs/images/MollweideSkyproj_with_indicatrices.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/docs/images/ObliqueMollweideSkyproj.png` & `skyproj-1.0.3/docs/images/ObliqueMollweideSkyproj.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/docs/images/Skyproj_with_indicatrices.png` & `skyproj-1.0.3/docs/images/Skyproj_with_indicatrices.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/docs/images/healsparse_one.png` & `skyproj-1.0.3/docs/images/healsparse_one.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/docs/images/healsparse_two.png` & `skyproj-1.0.3/docs/images/healsparse_two.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/docs/images/healsparse_valid_pixels.png` & `skyproj-1.0.3/docs/images/healsparse_valid_pixels.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/docs/images/hpxbin.png` & `skyproj-1.0.3/docs/images/hpxbin.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/docs/images/hpxbin_reproject.png` & `skyproj-1.0.3/docs/images/hpxbin_reproject.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/docs/images/lines_and_polygons_0.0.png` & `skyproj-1.0.3/docs/images/lines_and_polygons_0.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/docs/images/milky_way.png` & `skyproj-1.0.3/docs/images/milky_way.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/docs/images/milky_way_galactic.png` & `skyproj-1.0.3/docs/images/milky_way_galactic.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/docs/index.rst` & `skyproj-1.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/docs/install.rst` & `skyproj-1.0.3/docs/install.rst`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/docs/make.bat` & `skyproj-1.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/docs/maps.rst` & `skyproj-1.0.3/docs/maps.rst`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/docs/modules.rst` & `skyproj-1.0.3/docs/modules.rst`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/docs/projections.rst` & `skyproj-1.0.3/docs/projections.rst`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/docs/surveys.rst` & `skyproj-1.0.3/docs/surveys.rst`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/setup.cfg` & `skyproj-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/skyproj/_skyproj.py` & `skyproj-1.0.3/skyproj/_skyproj.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,19 +40,24 @@
         Label longitude ticks from 0 to 360 degrees (``positive``) or
         from -180 to 180 degrees (``symmetric``).
     autorescale : `bool`, optional
         Automatically rescale color bars when zoomed?
     galactic : `bool`, optional
         Plotting in Galactic coordinates?  Recommendation for Galactic plots
         is to have longitude_ticks set to ``symmetric`` and celestial = True.
+    rcparams : `dict`, optional
+        Dictionary of matplotlib rc parameters to override.  In particular, the code will
+        use ``xtick.labelsize`` and ``ytick.labelsize`` for the x and y tick labels, and
+        ``axes.linewidth`` for the map boundary.
     **kwargs : `dict`, optional
         Additional arguments to send to cartosky/proj4 projection CRS initialization.
     """
     def __init__(self, ax=None, projection_name='cyl', lon_0=0, gridlines=True, celestial=True,
-                 extent=None, longitude_ticks='positive', autorescale=True, galactic=False, **kwargs):
+                 extent=None, longitude_ticks='positive', autorescale=True, galactic=False,
+                 rcparams={}, **kwargs):
         self._redraw_dict = {'hpxmap': None,
                              'hspmap': None,
                              'im': None,
                              'inset_colorbar': None,
                              'inset_colorbar_kwargs': {},
                              'colorbar': None,
                              'colorbar_kwargs': {},
@@ -122,28 +127,32 @@
                              np.min(pts[:, 1]), np.max(pts[:, 1])]
         else:
             extent_xy = None
 
         self._boundary_lines = None
         self._boundary_labels = []
 
-        self._initialize_axes(extent, extent_xy=extent_xy)
+        if "axes.labelsize" not in rcparams:
+            rcparams["axes.labelsize"] = 16
 
-        # Set up callbacks on axis zoom.
-        self._add_change_axis_callbacks()
+        with plt.rc_context(rcparams):
+            self._initialize_axes(extent, extent_xy=extent_xy)
 
-        # Set up callback on figure resize.
-        self._frc = self.ax.figure.canvas.mpl_connect('resize_event', self._change_size)
-        self._dc = self.ax.figure.canvas.mpl_connect('draw_event', self._draw_callback)
-        self._initial_extent_xy = [0]*4
+            # Set up callbacks on axis zoom.
+            self._add_change_axis_callbacks()
 
-        # Set up reproject callback.
-        self._rpc = self.ax.figure.canvas.mpl_connect('key_press_event', self._keypress_callback)
+            # Set up callback on figure resize.
+            self._frc = self.ax.figure.canvas.mpl_connect('resize_event', self._change_size)
+            self._dc = self.ax.figure.canvas.mpl_connect('draw_event', self._draw_callback)
+            self._initial_extent_xy = [0]*4
 
-        self._draw_aa_bounds_and_labels()
+            # Set up reproject callback.
+            self._rpc = self.ax.figure.canvas.mpl_connect('key_press_event', self._keypress_callback)
+
+            self._draw_aa_bounds_and_labels()
 
     def proj(self, lon, lat):
         """Apply forward projection to a set of lon/lat positions.
 
         Convert from lon/lat to x/y.
 
         Parameters
@@ -360,14 +369,15 @@
                 if lat_line_y[0] < extent_xy[2] or lat_line_y[0] > extent_xy[3]:
                     continue
 
                 if lat_line_x[0] < extent_xy[x0_index] or lat_line_y[0] > extent_xy[x1_index]:
                     continue
 
                 label = self._tick_formatter2(axis_side, factor, [lat_level])[0]
+
                 boundary_labels.append(self._ax.text(lat_line_x[0],
                                                      lat_line_y[0],
                                                      label,
                                                      size=plt.rcParams['ytick.labelsize'],
                                                      lonlat=False,
                                                      clip_on=False,
                                                      ha=ha,
@@ -432,14 +442,15 @@
                 if prev_x is not None:
                     # Check if too close to last label.
                     if abs(x[i] - prev_x)/delta_x < 0.05:
                         continue
                 prev_x = x[i]
 
                 label = self._tick_formatter1('top', factor, [levels[i]])[0]
+
                 boundary_labels.append(self._ax.text(x[i],
                                                      y[i],
                                                      label,
                                                      size=plt.rcParams['xtick.labelsize'],
                                                      lonlat=False,
                                                      clip_on=False,
                                                      ha='right',
@@ -607,16 +618,16 @@
 
         self._aa.format_coord = self._format_coord
         self._aa.axis['left'].major_ticklabels.set_visible(True)
         self._aa.axis['right'].major_ticklabels.set_visible(False)
         self._aa.axis['bottom'].major_ticklabels.set_visible(True)
         self._aa.axis['top'].major_ticklabels.set_visible(True)
 
-        self.set_xlabel(self._default_xy_labels[0], size=16)
-        self.set_ylabel(self._default_xy_labels[1], size=16)
+        self.set_xlabel(self._default_xy_labels[0])
+        self.set_ylabel(self._default_xy_labels[1])
 
         fig.sca(self._ax)
 
         return fig, self._ax
 
     def _format_coord(self, x, y):
         """Return a coordinate format string.
```

### Comparing `skyproj-1.0.2/skyproj/data/bliss-poly.txt` & `skyproj-1.0.3/skyproj/data/bliss-poly.txt`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/skyproj/data/ccd_corners_xy_fill.dat` & `skyproj-1.0.3/skyproj/data/ccd_corners_xy_fill.dat`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/skyproj/data/constellationsANDstars.json` & `skyproj-1.0.3/skyproj/data/constellationsANDstars.json`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/skyproj/data/decals-poly.txt` & `skyproj-1.0.3/skyproj/data/decals-poly.txt`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/skyproj/data/derosita-poly.txt` & `skyproj-1.0.3/skyproj/data/derosita-poly.txt`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/skyproj/data/des-round13-poly.txt` & `skyproj-1.0.3/skyproj/data/des-round13-poly.txt`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/skyproj/data/des-round17-poly.txt` & `skyproj-1.0.3/skyproj/data/des-round17-poly.txt`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/skyproj/data/des-round19-poly.txt` & `skyproj-1.0.3/skyproj/data/des-round19-poly.txt`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/skyproj/data/maglites-poly.txt` & `skyproj-1.0.3/skyproj/data/maglites-poly.txt`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/skyproj/data/smash_fields_final.txt` & `skyproj-1.0.3/skyproj/data/smash_fields_final.txt`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/skyproj/hpx_utils.py` & `skyproj-1.0.3/skyproj/hpx_utils.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/skyproj/mpl_utils.py` & `skyproj-1.0.3/skyproj/mpl_utils.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/skyproj/skyaxes.py` & `skyproj-1.0.3/skyproj/skyaxes.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/skyproj/skycrs.py` & `skyproj-1.0.3/skyproj/skycrs.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/skyproj/skyproj.py` & `skyproj-1.0.3/skyproj/skyproj.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/skyproj/survey.py` & `skyproj-1.0.3/skyproj/survey.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/skyproj/transforms.py` & `skyproj-1.0.3/skyproj/transforms.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/skyproj/utils.py` & `skyproj-1.0.3/skyproj/utils.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/skyproj.egg-info/PKG-INFO` & `skyproj-1.0.3/skyproj.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skyproj
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python tools for making sky projections and maps
 Home-page: https://github.com/lsstdesc/skyproj
 Author: Eli Rykoff, Alex Drlica-Wagner, and others
 Author-email: erykoff@stanford.edu
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `skyproj-1.0.2/skyproj.egg-info/SOURCES.txt` & `skyproj-1.0.3/skyproj.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 .gitignore
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
-.github/workflows/python-package.yml
+.github/workflows/python-package-pr.yml
+.github/workflows/python-package-publish.yml
+.github/workflows/python-package-push.yml
 docs/Makefile
 docs/basic_interface.rst
 docs/conf.py
 docs/index.rst
 docs/install.rst
 docs/make.bat
 docs/maps.rst
@@ -36,26 +38,24 @@
 docs/images/healsparse_two.png
 docs/images/healsparse_valid_pixels.png
 docs/images/hpxbin.png
 docs/images/hpxbin_reproject.png
 docs/images/lines_and_polygons_0.0.png
 docs/images/milky_way.png
 docs/images/milky_way_galactic.png
+docs/images/skyproj_full_override_sizes.png
 skyproj/__init__.py
 skyproj/_skyproj.py
 skyproj/hpx_utils.py
 skyproj/mpl_utils.py
-skyproj/projections_alt.py
 skyproj/skyaxes.py
 skyproj/skycrs.py
 skyproj/skyproj.py
-skyproj/skyproj_alt.py
 skyproj/survey.py
 skyproj/transforms.py
-skyproj/transforms_noodling.py
 skyproj/utils.py
 skyproj.egg-info/PKG-INFO
 skyproj.egg-info/SOURCES.txt
 skyproj.egg-info/dependency_links.txt
 skyproj.egg-info/requires.txt
 skyproj.egg-info/top_level.txt
 skyproj.egg-info/zip-safe
@@ -141,11 +141,12 @@
 tests/data/moll_full_100.0.png
 tests/data/moll_full_180.0.png
 tests/data/moll_gaptest.png
 tests/data/moll_zoom.png
 tests/data/obmoll_0.0_45.0_-90.0.png
 tests/data/obmoll_100.0_80.0_0.0.png
 tests/data/plotting_routines.png
+tests/data/skyproj_full_override_sizes.png
 tutorial/README.md
 tutorial/tutorial_baseclass.ipynb
 tutorial/tutorial_healsparse.ipynb
 tutorial/tutorial_surveys.ipynb
```

### Comparing `skyproj-1.0.2/tests/data/BLISS_survey.png` & `skyproj-1.0.3/tests/data/BLISS_survey.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/DECaLS_survey.png` & `skyproj-1.0.3/tests/data/DECaLS_survey.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/DESAlbers_survey.png` & `skyproj-1.0.3/tests/data/DESAlbers_survey.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/DES_survey.png` & `skyproj-1.0.3/tests/data/DES_survey.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/MagLiTeS_survey.png` & `skyproj-1.0.3/tests/data/MagLiTeS_survey.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/aea_-15.0_-45.0.png` & `skyproj-1.0.3/tests/data/aea_-15.0_-45.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/aea_-20.0_15.0.png` & `skyproj-1.0.3/tests/data/aea_-20.0_15.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/aea_15.0_45.0.png` & `skyproj-1.0.3/tests/data/aea_15.0_45.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/aea_full_-100.0.png` & `skyproj-1.0.3/tests/data/aea_full_-100.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/aea_full_0.0.png` & `skyproj-1.0.3/tests/data/aea_full_0.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/aea_full_100.0.png` & `skyproj-1.0.3/tests/data/aea_full_100.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/aea_full_180.0.png` & `skyproj-1.0.3/tests/data/aea_full_180.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/aea_zoom.png` & `skyproj-1.0.3/tests/data/aea_zoom.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/cyl_full_-100.0.png` & `skyproj-1.0.3/tests/data/cyl_full_-100.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/cyl_full_0.0.png` & `skyproj-1.0.3/tests/data/cyl_full_0.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/cyl_full_100.0.png` & `skyproj-1.0.3/tests/data/cyl_full_100.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/cyl_full_180.0.png` & `skyproj-1.0.3/tests/data/cyl_full_180.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/cyl_tissot.png` & `skyproj-1.0.3/tests/data/cyl_tissot.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/cyl_zoom.png` & `skyproj-1.0.3/tests/data/cyl_zoom.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/eqearth_full_-100.0.png` & `skyproj-1.0.3/tests/data/eqearth_full_-100.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/eqearth_full_0.0.png` & `skyproj-1.0.3/tests/data/eqearth_full_0.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/eqearth_full_100.0.png` & `skyproj-1.0.3/tests/data/eqearth_full_100.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/eqearth_full_180.0.png` & `skyproj-1.0.3/tests/data/eqearth_full_180.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/eqearth_zoom.png` & `skyproj-1.0.3/tests/data/eqearth_zoom.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/gnom_-120.0_75.0.png` & `skyproj-1.0.3/tests/data/gnom_-120.0_75.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/gnom_0.0_0.0.png` & `skyproj-1.0.3/tests/data/gnom_0.0_0.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/gnom_120.0_-75.0.png` & `skyproj-1.0.3/tests/data/gnom_120.0_-75.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/hammer_full_-100.0.png` & `skyproj-1.0.3/tests/data/hammer_full_-100.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/hammer_full_0.0.png` & `skyproj-1.0.3/tests/data/hammer_full_0.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/hammer_full_100.0.png` & `skyproj-1.0.3/tests/data/hammer_full_100.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/hammer_full_180.0.png` & `skyproj-1.0.3/tests/data/hammer_full_180.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/hammer_zoom.png` & `skyproj-1.0.3/tests/data/hammer_zoom.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/healsparse_bool.png` & `skyproj-1.0.3/tests/data/healsparse_bool.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/healsparse_bool_valid_pixels.png` & `skyproj-1.0.3/tests/data/healsparse_bool_valid_pixels.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/healsparse_one.png` & `skyproj-1.0.3/tests/data/healsparse_one.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/healsparse_rec_array.png` & `skyproj-1.0.3/tests/data/healsparse_rec_array.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/healsparse_three.png` & `skyproj-1.0.3/tests/data/healsparse_three.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/healsparse_two.png` & `skyproj-1.0.3/tests/data/healsparse_two.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/healsparse_valid_pixels.png` & `skyproj-1.0.3/tests/data/healsparse_valid_pixels.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/healsparse_wide_one.png` & `skyproj-1.0.3/tests/data/healsparse_wide_one.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/hpxbin.png` & `skyproj-1.0.3/tests/data/hpxbin.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/laea_zoom.png` & `skyproj-1.0.3/tests/data/laea_zoom.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/lines_and_polygons_0.0.png` & `skyproj-1.0.3/tests/data/lines_and_polygons_0.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/lines_and_polygons_180.0.png` & `skyproj-1.0.3/tests/data/lines_and_polygons_180.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/lines_and_polygons_obmoll_0.0_45.0_-90.0.png` & `skyproj-1.0.3/tests/data/lines_and_polygons_obmoll_0.0_45.0_-90.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/lines_and_polygons_obmoll_100.0_80.0_-90.0.png` & `skyproj-1.0.3/tests/data/lines_and_polygons_obmoll_100.0_80.0_-90.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/mbtfpq_full_-100.0.png` & `skyproj-1.0.3/tests/data/mbtfpq_full_-100.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/mbtfpq_full_0.0.png` & `skyproj-1.0.3/tests/data/mbtfpq_full_0.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/mbtfpq_full_100.0.png` & `skyproj-1.0.3/tests/data/mbtfpq_full_100.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/mbtfpq_full_180.0.png` & `skyproj-1.0.3/tests/data/mbtfpq_full_180.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/mbtfpq_gaptest.png` & `skyproj-1.0.3/tests/data/mbtfpq_gaptest.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/mbtfpq_tissot.png` & `skyproj-1.0.3/tests/data/mbtfpq_tissot.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/mbtfpq_zoom.png` & `skyproj-1.0.3/tests/data/mbtfpq_zoom.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/milky_way.png` & `skyproj-1.0.3/tests/data/milky_way.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/milky_way_galactic.png` & `skyproj-1.0.3/tests/data/milky_way_galactic.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/moll_full_-100.0.png` & `skyproj-1.0.3/tests/data/moll_full_-100.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/moll_full_0.0.png` & `skyproj-1.0.3/tests/data/moll_full_0.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/moll_full_100.0.png` & `skyproj-1.0.3/tests/data/moll_full_100.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/moll_full_180.0.png` & `skyproj-1.0.3/tests/data/moll_full_180.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/moll_gaptest.png` & `skyproj-1.0.3/tests/data/moll_gaptest.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/moll_zoom.png` & `skyproj-1.0.3/tests/data/moll_zoom.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/obmoll_0.0_45.0_-90.0.png` & `skyproj-1.0.3/tests/data/obmoll_0.0_45.0_-90.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/obmoll_100.0_80.0_0.0.png` & `skyproj-1.0.3/tests/data/obmoll_100.0_80.0_0.0.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/data/plotting_routines.png` & `skyproj-1.0.3/tests/data/plotting_routines.png`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/test_healpix_binning.py` & `skyproj-1.0.3/tests/test_healpix_binning.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/test_healpix_maps.py` & `skyproj-1.0.3/tests/test_healpix_maps.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/test_lines_polygons.py` & `skyproj-1.0.3/tests/test_lines_polygons.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     # Test ``ellipse``.  We can only plot one point per call
     sp.ellipse(60, 15, 10, 4, 0, color='green', label='Nine')
     sp.ellipse(300, 15, 15, 2, 45, fill=True, color='red', label='Ten')
 
     sp.legend()
     fname = f'lines_and_polygons_{lon_0}.png'
     fig.savefig(tmp_path / fname)
-    err = compare_images(os.path.join(ROOT, 'data', fname), tmp_path / fname, 10.0)
+    err = compare_images(os.path.join(ROOT, 'data', fname), tmp_path / fname, 15.0)
     if err:
         raise ImageComparisonFailure(err)
 
 
 @pytest.mark.parametrize("lonlatplonp", [(0.0, 45.0, -90.0),
                                          (100.0, 80.0, -90.0)])
 def test_lines_polygons_obmoll(tmp_path, lonlatplonp):
@@ -90,10 +90,10 @@
                     edgecolor='black', facecolor='red', linestyle='--', label='Five')
     sp.draw_polygon([160, 200, 200, 160], [-20, -20, -40, -40],
                     edgecolor='red', facecolor='black', linestyle='-', label='Six')
 
     sp.legend()
     fname = f'lines_and_polygons_obmoll_{lon_0}_{lat_p}_{lon_p}.png'
     fig.savefig(tmp_path / fname)
-    err = compare_images(os.path.join(ROOT, 'data', fname), tmp_path / fname, 10.0)
+    err = compare_images(os.path.join(ROOT, 'data', fname), tmp_path / fname, 15.0)
     if err:
         raise ImageComparisonFailure(err)
```

### Comparing `skyproj-1.0.2/tests/test_milky_way.py` & `skyproj-1.0.3/tests/test_milky_way.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     fig.clf()
     ax = fig.add_subplot(111)
     sp = skyproj.McBrydeSkyproj(ax=ax)
     sp.draw_milky_way(label='Milky Way')
     sp.legend()
     fname = 'milky_way.png'
     fig.savefig(tmp_path / fname)
-    err = compare_images(os.path.join(ROOT, 'data', fname), tmp_path / fname, 10.0)
+    err = compare_images(os.path.join(ROOT, 'data', fname), tmp_path / fname, 15.0)
     if err:
         raise ImageComparisonFailure(err)
 
 
 def test_draw_milky_way_galactic(tmp_path):
     """Test drawing the Milky Way (Galactic Coordinates)."""
     plt.rcParams.update(plt.rcParamsDefault)
@@ -37,10 +37,10 @@
     fig.clf()
     ax = fig.add_subplot(111)
     sp = skyproj.McBrydeSkyproj(ax=ax, galactic=True, longitude_ticks='symmetric')
     sp.draw_milky_way(label='Milky Way')
     sp.legend()
     fname = 'milky_way_galactic.png'
     fig.savefig(tmp_path / fname)
-    err = compare_images(os.path.join(ROOT, 'data', fname), tmp_path / fname, 10.0)
+    err = compare_images(os.path.join(ROOT, 'data', fname), tmp_path / fname, 15.0)
     if err:
         raise ImageComparisonFailure(err)
```

### Comparing `skyproj-1.0.2/tests/test_plotting.py` & `skyproj-1.0.3/tests/test_plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,10 +39,10 @@
     sp.fill([20, 25, 25, 20], [20, 20, 25, 25], color='blue')
 
     # Test ``scatter`` with points.
     sp.scatter([15, 35], [15, 35], c=['magenta', 'orange'])
 
     fname = 'plotting_routines.png'
     fig.savefig(tmp_path / fname)
-    err = compare_images(os.path.join(ROOT, 'data', fname), tmp_path / fname, 10.0)
+    err = compare_images(os.path.join(ROOT, 'data', fname), tmp_path / fname, 15.0)
     if err:
         raise ImageComparisonFailure(err)
```

### Comparing `skyproj-1.0.2/tests/test_projections.py` & `skyproj-1.0.3/tests/test_projections.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tests/test_skyproj.py` & `skyproj-1.0.3/tests/test_skyproj.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     # Full image
     fig = plt.figure(1, figsize=(8, 5))
     fig.clf()
     ax = fig.add_subplot(111)
     sp = skyproj(ax=ax, lon_0=lon_0)
     fname = f'{sp.projection_name}_full_{lon_0}.png'
     fig.savefig(tmp_path / fname)
-    err = compare_images(os.path.join(ROOT, 'data', fname), tmp_path / fname, 10.0)
+    err = compare_images(os.path.join(ROOT, 'data', fname), tmp_path / fname, 15.0)
     if err:
         raise ImageComparisonFailure(err)
 
 
 @pytest.mark.parametrize("skyproj", [skyproj.Skyproj,
                                      skyproj.McBrydeSkyproj,
                                      skyproj.MollweideSkyproj,
@@ -51,15 +51,15 @@
     # Simple zoom
     fig = plt.figure(1, figsize=(8, 5))
     fig.clf()
     ax = fig.add_subplot(111)
     sp = skyproj(ax=ax, extent=[0, 50, 0, 50])
     fname = f'{sp.projection_name}_zoom.png'
     fig.savefig(tmp_path / fname)
-    err = compare_images(os.path.join(ROOT, 'data', fname), tmp_path / fname, 10.0)
+    err = compare_images(os.path.join(ROOT, 'data', fname), tmp_path / fname, 15.0)
     if err:
         raise ImageComparisonFailure(err)
 
 
 @pytest.mark.parametrize("lonlat", [(0.0, 0.0),
                                     (120.0, -75.0),
                                     (-120.0, 75.0)])
@@ -78,15 +78,15 @@
     delta_lon = delta_lat/np.cos(np.deg2rad(lat_0))
     sp.draw_polygon(
         [lon_0 - delta_lon, lon_0 + delta_lon, lon_0 + delta_lon, lon_0 - delta_lon],
         [lat_0 - delta_lat, lat_0 - delta_lat, lat_0 + delta_lat, lat_0 + delta_lat]
     )
     fname = f'gnom_{lon_0}_{lat_0}.png'
     fig.savefig(tmp_path / fname)
-    err = compare_images(os.path.join(ROOT, 'data', fname), tmp_path / fname, 10.0)
+    err = compare_images(os.path.join(ROOT, 'data', fname), tmp_path / fname, 15.0)
     if err:
         raise ImageComparisonFailure(err)
 
 
 @pytest.mark.parametrize("lonlatplonp", [(0.0, 45.0, -90.0),
                                          (100.0, 80.0, 0.0)])
 def test_skyproj_obmoll(tmp_path, lonlatplonp):
@@ -97,15 +97,15 @@
 
     fig = plt.figure(1, figsize=(8, 5))
     fig.clf()
     ax = fig.add_subplot(111)
     sp = skyproj.ObliqueMollweideSkyproj(ax=ax, lon_0=lon_0, lat_p=lat_p, lon_p=lon_p)
     fname = f'{sp.projection_name}_{lon_0}_{lat_p}_{lon_p}.png'
     fig.savefig(tmp_path / fname)
-    err = compare_images(os.path.join(ROOT, 'data', fname), tmp_path / fname, 10.0)
+    err = compare_images(os.path.join(ROOT, 'data', fname), tmp_path / fname, 15.0)
     if err:
         raise ImageComparisonFailure(err)
 
 
 @pytest.mark.parametrize("lat1lat2", [(15.0, 45.0),
                                       (-20.0, 15.0),
                                       (-15.0, -45.0)])
@@ -117,15 +117,15 @@
 
     fig = plt.figure(1, figsize=(8, 5))
     fig.clf()
     ax = fig.add_subplot(111)
     sp = skyproj.AlbersSkyproj(ax=ax, lat_1=lat_1, lat_2=lat_2)
     fname = f'{sp.projection_name}_{lat_1}_{lat_2}.png'
     fig.savefig(tmp_path / fname)
-    err = compare_images(os.path.join(ROOT, 'data', fname), tmp_path / fname, 10.0)
+    err = compare_images(os.path.join(ROOT, 'data', fname), tmp_path / fname, 15.0)
     if err:
         raise ImageComparisonFailure(err)
 
 
 @pytest.mark.parametrize("skyproj", [skyproj.Skyproj,
                                      skyproj.McBrydeSkyproj,
                                      skyproj.MollweideSkyproj,
@@ -173,10 +173,41 @@
     fig = plt.figure(1, figsize=(8, 5))
     fig.clf()
     ax = fig.add_subplot(111)
     sp = skyproj(ax=ax, lon_0=180.0)
     sp.draw_hspmap(testmap, zoom=False)
     fname = f'{sp.projection_name}_gaptest.png'
     fig.savefig(tmp_path / fname)
-    err = compare_images(os.path.join(ROOT, 'data', fname), tmp_path / fname, 10.0)
+    err = compare_images(os.path.join(ROOT, 'data', fname), tmp_path / fname, 15.0)
+    if err:
+        raise ImageComparisonFailure(err)
+
+
+def test_skyproj_override_sizes(tmp_path):
+    """Test overriding the label/width sizes."""
+    plt.rcParams.update(plt.rcParamsDefault)
+
+    rcparams = {'xtick.labelsize': 20,
+                'ytick.labelsize': 4,
+                'axes.linewidth': 5}
+
+    # Full image
+    fig = plt.figure(1, figsize=(8, 5))
+    fig.clf()
+    ax = fig.add_subplot(111)
+    _ = skyproj.McBrydeSkyproj(ax=ax, rcparams=rcparams)
+    fname = 'skyproj_full_override_sizes.png'
+    fig.savefig(tmp_path / fname)
+    err = compare_images(os.path.join(ROOT, 'data', fname), tmp_path / fname, 15.0)
+    if err:
+        raise ImageComparisonFailure(err)
+
+    # And confirm that the changes do not carry over to another plot.
+    fig = plt.figure(1, figsize=(8, 5))
+    fig.clf()
+    ax = fig.add_subplot(111)
+    _ = skyproj.McBrydeSkyproj(ax=ax)
+    fname = 'mbtfpq_full_0.0.png'
+    fig.savefig(tmp_path / fname)
+    err = compare_images(os.path.join(ROOT, 'data', fname), tmp_path / fname, 15.0)
     if err:
         raise ImageComparisonFailure(err)
```

### Comparing `skyproj-1.0.2/tests/test_survey.py` & `skyproj-1.0.3/tests/test_survey.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,10 +36,10 @@
     elif name == 'MagLiTeS':
         sp.draw_maglites(label=name)
     elif name == 'DECaLS':
         sp.draw_decals(label=name)
     sp.legend()
     fname = f'{name}_survey.png'
     fig.savefig(tmp_path / fname)
-    err = compare_images(os.path.join(ROOT, 'data', fname), tmp_path / fname, 10.0)
+    err = compare_images(os.path.join(ROOT, 'data', fname), tmp_path / fname, 15.0)
     if err:
         raise ImageComparisonFailure(err)
```

### Comparing `skyproj-1.0.2/tests/test_tissot.py` & `skyproj-1.0.3/tests/test_tissot.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,10 +23,10 @@
     fig = plt.figure(1, figsize=(8, 5))
     fig.clf()
     ax = fig.add_subplot(111)
     sp = skyproj(ax=ax)
     sp.tissot_indicatrices()
     fname = f'{sp.projection_name}_tissot.png'
     fig.savefig(tmp_path / fname)
-    err = compare_images(os.path.join(ROOT, 'data', fname), tmp_path / fname, 10.0)
+    err = compare_images(os.path.join(ROOT, 'data', fname), tmp_path / fname, 15.0)
     if err:
         raise ImageComparisonFailure(err)
```

### Comparing `skyproj-1.0.2/tests/test_tutorial.py` & `skyproj-1.0.3/tests/test_tutorial.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 https://blog.thedataincubator.com/2016/06/testing-jupyter-notebooks/
 """
 import os
 import pytest
 import subprocess
 import tempfile
 
-import nbformat
+try:
+    import nbformat
+except ImportError:
+    nbformat = None
 
 
 ROOT = os.path.abspath(os.path.dirname(__file__))
 
 
 def _notebook_run(nbfile):
     """Execute a notebook via nbconvert and collect output.
@@ -42,14 +45,15 @@
     errors = [output for cell in nb.cells if "outputs" in cell
               for output in cell["outputs"]
               if output.output_type == "error"]
 
     return nb, errors
 
 
+@pytest.mark.skipif(nbformat is None, reason="nbformat not installed.")
 @pytest.mark.parametrize("nbfile", ["tutorial_baseclass.ipynb",
                                     "tutorial_surveys.ipynb",
                                     "tutorial_healsparse.ipynb"])
 def test_tutorial_notebooks(nbfile):
     """Test running a tutorial notebook."""
     fname = os.path.abspath(os.path.join(ROOT, '../tutorial', nbfile))
     nb, errors = _notebook_run(fname)
```

### Comparing `skyproj-1.0.2/tests/test_utils.py` & `skyproj-1.0.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tutorial/tutorial_baseclass.ipynb` & `skyproj-1.0.3/tutorial/tutorial_baseclass.ipynb`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tutorial/tutorial_healsparse.ipynb` & `skyproj-1.0.3/tutorial/tutorial_healsparse.ipynb`

 * *Files identical despite different names*

### Comparing `skyproj-1.0.2/tutorial/tutorial_surveys.ipynb` & `skyproj-1.0.3/tutorial/tutorial_surveys.ipynb`

 * *Files identical despite different names*

