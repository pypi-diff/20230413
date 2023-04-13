# Comparing `tmp/astro-gdt-2.0.0.tar.gz` & `tmp/astro-gdt-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-gdt-2.0.0.tar", last modified: Wed Apr 12 19:18:49 2023, max compression
+gzip compressed data, was "astro-gdt-2.0.1.tar", last modified: Thu Apr 13 16:22:07 2023, max compression
```

## Comparing `astro-gdt-2.0.0.tar` & `astro-gdt-2.0.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-12 19:18:49.946048 astro-gdt-2.0.0/
--rw-r--r--   0 wcleveland   (502) staff       (20)       44 2023-04-12 13:18:15.000000 astro-gdt-2.0.0/MANIFEST.in
--rw-r--r--   0 wcleveland   (502) staff       (20)     2156 2023-04-12 19:18:49.945761 astro-gdt-2.0.0/PKG-INFO
--rw-r--r--   0 wcleveland   (502) staff       (20)     1295 2023-04-12 14:57:38.000000 astro-gdt-2.0.0/PYPI-README.rst
--rw-r--r--   0 wcleveland   (502) staff       (20)     3648 2023-04-12 14:58:55.000000 astro-gdt-2.0.0/README.rst
--rw-r--r--   0 wcleveland   (502) staff       (20)    11357 2023-03-28 14:21:11.000000 astro-gdt-2.0.0/license.txt
-drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-12 19:18:49.907509 astro-gdt-2.0.0/scripts/
--rw-r--r--   0 wcleveland   (502) staff       (20)     6142 2023-04-12 14:56:06.000000 astro-gdt-2.0.0/scripts/gdt-data
--rw-r--r--   0 wcleveland   (502) staff       (20)       38 2023-04-12 19:18:49.946126 astro-gdt-2.0.0/setup.cfg
--rw-r--r--   0 wcleveland   (502) staff       (20)     3310 2023-04-12 18:40:17.000000 astro-gdt-2.0.0/setup.py
-drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-12 19:18:49.900408 astro-gdt-2.0.0/src/
-drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-12 19:18:49.909674 astro-gdt-2.0.0/src/astro_gdt.egg-info/
--rw-r--r--   0 wcleveland   (502) staff       (20)     2156 2023-04-12 19:18:49.000000 astro-gdt-2.0.0/src/astro_gdt.egg-info/PKG-INFO
--rw-r--r--   0 wcleveland   (502) staff       (20)     1725 2023-04-12 19:18:49.000000 astro-gdt-2.0.0/src/astro_gdt.egg-info/SOURCES.txt
--rw-r--r--   0 wcleveland   (502) staff       (20)        1 2023-04-12 19:18:49.000000 astro-gdt-2.0.0/src/astro_gdt.egg-info/dependency_links.txt
--rw-r--r--   0 wcleveland   (502) staff       (20)      186 2023-04-12 19:18:49.000000 astro-gdt-2.0.0/src/astro_gdt.egg-info/requires.txt
--rw-r--r--   0 wcleveland   (502) staff       (20)        4 2023-04-12 19:18:49.000000 astro-gdt-2.0.0/src/astro_gdt.egg-info/top_level.txt
-drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-12 19:18:49.902863 astro-gdt-2.0.0/src/gdt/
-drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-12 19:18:49.921994 astro-gdt-2.0.0/src/gdt/core/
--rw-r--r--   0 wcleveland   (502) staff       (20)     1718 2023-04-12 19:07:37.000000 astro-gdt-2.0.0/src/gdt/core/__init__.py
-drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-12 19:18:49.924503 astro-gdt-2.0.0/src/gdt/core/background/
--rw-r--r--   0 wcleveland   (502) staff       (20)        0 2023-03-28 15:49:38.000000 astro-gdt-2.0.0/src/gdt/core/background/__init__.py
--rw-r--r--   0 wcleveland   (502) staff       (20)    10352 2023-03-28 15:49:38.000000 astro-gdt-2.0.0/src/gdt/core/background/binned.py
--rw-r--r--   0 wcleveland   (502) staff       (20)    11176 2023-03-28 15:54:41.000000 astro-gdt-2.0.0/src/gdt/core/background/fitter.py
--rw-r--r--   0 wcleveland   (502) staff       (20)    15005 2023-04-12 13:18:15.000000 astro-gdt-2.0.0/src/gdt/core/background/primitives.py
--rw-r--r--   0 wcleveland   (502) staff       (20)    10734 2023-03-28 15:49:38.000000 astro-gdt-2.0.0/src/gdt/core/background/unbinned.py
-drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-12 19:18:49.926144 astro-gdt-2.0.0/src/gdt/core/binning/
--rw-r--r--   0 wcleveland   (502) staff       (20)        0 2023-03-28 15:49:38.000000 astro-gdt-2.0.0/src/gdt/core/binning/__init__.py
--rw-r--r--   0 wcleveland   (502) staff       (20)    10018 2023-03-28 15:49:38.000000 astro-gdt-2.0.0/src/gdt/core/binning/binned.py
--rw-r--r--   0 wcleveland   (502) staff       (20)     7377 2023-03-28 15:49:38.000000 astro-gdt-2.0.0/src/gdt/core/binning/unbinned.py
--rw-r--r--   0 wcleveland   (502) staff       (20)     8526 2023-04-12 13:18:15.000000 astro-gdt-2.0.0/src/gdt/core/collection.py
-drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-12 19:18:49.927413 astro-gdt-2.0.0/src/gdt/core/coords/
--rw-r--r--   0 wcleveland   (502) staff       (20)      154 2023-03-28 14:21:11.000000 astro-gdt-2.0.0/src/gdt/core/coords/__init__.py
--rw-r--r--   0 wcleveland   (502) staff       (20)    13230 2023-03-28 16:25:21.000000 astro-gdt-2.0.0/src/gdt/core/coords/quaternion.py
-drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-12 19:18:49.929873 astro-gdt-2.0.0/src/gdt/core/coords/spacecraft/
--rw-r--r--   0 wcleveland   (502) staff       (20)     1455 2023-03-28 14:21:11.000000 astro-gdt-2.0.0/src/gdt/core/coords/spacecraft/__init__.py
--rw-r--r--   0 wcleveland   (502) staff       (20)     5087 2023-03-28 14:21:11.000000 astro-gdt-2.0.0/src/gdt/core/coords/spacecraft/axes.py
--rw-r--r--   0 wcleveland   (502) staff       (20)    14856 2023-03-28 16:25:21.000000 astro-gdt-2.0.0/src/gdt/core/coords/spacecraft/frame.py
--rw-r--r--   0 wcleveland   (502) staff       (20)     2915 2023-03-28 14:21:11.000000 astro-gdt-2.0.0/src/gdt/core/coords/spacecraft/model.py
--rw-r--r--   0 wcleveland   (502) staff       (20)   101533 2023-03-28 14:21:11.000000 astro-gdt-2.0.0/src/gdt/core/data_primitives.py
--rw-r--r--   0 wcleveland   (502) staff       (20)     5736 2023-03-28 14:21:11.000000 astro-gdt-2.0.0/src/gdt/core/detector.py
--rw-r--r--   0 wcleveland   (502) staff       (20)     7234 2023-03-28 14:21:11.000000 astro-gdt-2.0.0/src/gdt/core/file.py
--rw-r--r--   0 wcleveland   (502) staff       (20)     4425 2023-03-28 14:21:11.000000 astro-gdt-2.0.0/src/gdt/core/geomagnetic.py
--rw-r--r--   0 wcleveland   (502) staff       (20)     7584 2023-03-28 16:04:17.000000 astro-gdt-2.0.0/src/gdt/core/headers.py
--rw-r--r--   0 wcleveland   (502) staff       (20)    34543 2023-04-12 13:18:15.000000 astro-gdt-2.0.0/src/gdt/core/healpix.py
--rw-r--r--   0 wcleveland   (502) staff       (20)    20760 2023-03-31 16:28:22.000000 astro-gdt-2.0.0/src/gdt/core/heasarc.py
--rw-r--r--   0 wcleveland   (502) staff       (20)    24394 2023-03-28 15:54:41.000000 astro-gdt-2.0.0/src/gdt/core/pha.py
--rw-r--r--   0 wcleveland   (502) staff       (20)    19046 2023-03-28 14:21:11.000000 astro-gdt-2.0.0/src/gdt/core/phaii.py
-drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-12 19:18:49.936957 astro-gdt-2.0.0/src/gdt/core/plot/
--rw-r--r--   0 wcleveland   (502) staff       (20)        0 2023-03-28 15:49:38.000000 astro-gdt-2.0.0/src/gdt/core/plot/__init__.py
--rw-r--r--   0 wcleveland   (502) staff       (20)     1768 2023-03-28 15:49:38.000000 astro-gdt-2.0.0/src/gdt/core/plot/defaults.py
--rw-r--r--   0 wcleveland   (502) staff       (20)    10441 2023-03-28 15:49:38.000000 astro-gdt-2.0.0/src/gdt/core/plot/drm.py
--rw-r--r--   0 wcleveland   (502) staff       (20)     7634 2023-03-28 15:54:41.000000 astro-gdt-2.0.0/src/gdt/core/plot/earthplot.py
--rw-r--r--   0 wcleveland   (502) staff       (20)    36973 2023-03-28 15:54:41.000000 astro-gdt-2.0.0/src/gdt/core/plot/lib.py
--rw-r--r--   0 wcleveland   (502) staff       (20)     8207 2023-03-28 15:49:38.000000 astro-gdt-2.0.0/src/gdt/core/plot/lightcurve.py
--rw-r--r--   0 wcleveland   (502) staff       (20)    13209 2023-03-28 15:49:38.000000 astro-gdt-2.0.0/src/gdt/core/plot/model.py
--rw-r--r--   0 wcleveland   (502) staff       (20)    80329 2023-03-28 15:54:41.000000 astro-gdt-2.0.0/src/gdt/core/plot/plot.py
--rw-r--r--   0 wcleveland   (502) staff       (20)    26448 2023-03-28 15:54:41.000000 astro-gdt-2.0.0/src/gdt/core/plot/sky.py
--rw-r--r--   0 wcleveland   (502) staff       (20)     8355 2023-03-28 15:49:38.000000 astro-gdt-2.0.0/src/gdt/core/plot/spectrum.py
--rw-r--r--   0 wcleveland   (502) staff       (20)    25468 2023-03-28 14:21:11.000000 astro-gdt-2.0.0/src/gdt/core/response.py
-drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-12 19:18:49.940092 astro-gdt-2.0.0/src/gdt/core/simulate/
--rw-r--r--   0 wcleveland   (502) staff       (20)       90 2023-03-28 14:21:11.000000 astro-gdt-2.0.0/src/gdt/core/simulate/__init__.py
--rw-r--r--   0 wcleveland   (502) staff       (20)    15759 2023-03-28 15:54:41.000000 astro-gdt-2.0.0/src/gdt/core/simulate/generators.py
--rw-r--r--   0 wcleveland   (502) staff       (20)     9886 2023-03-28 15:54:41.000000 astro-gdt-2.0.0/src/gdt/core/simulate/pha.py
--rw-r--r--   0 wcleveland   (502) staff       (20)     3902 2023-03-28 14:21:11.000000 astro-gdt-2.0.0/src/gdt/core/simulate/profiles.py
--rw-r--r--   0 wcleveland   (502) staff       (20)    13459 2023-03-28 16:29:39.000000 astro-gdt-2.0.0/src/gdt/core/simulate/tte.py
-drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-12 19:18:49.943002 astro-gdt-2.0.0/src/gdt/core/spectra/
--rw-r--r--   0 wcleveland   (502) staff       (20)        0 2023-03-28 14:21:11.000000 astro-gdt-2.0.0/src/gdt/core/spectra/__init__.py
--rw-r--r--   0 wcleveland   (502) staff       (20)    50761 2023-03-28 15:54:41.000000 astro-gdt-2.0.0/src/gdt/core/spectra/fitting.py
--rw-r--r--   0 wcleveland   (502) staff       (20)    47277 2023-03-28 14:21:11.000000 astro-gdt-2.0.0/src/gdt/core/spectra/functions.py
--rw-r--r--   0 wcleveland   (502) staff       (20)    17921 2023-03-28 14:21:11.000000 astro-gdt-2.0.0/src/gdt/core/spectra/parameters.py
--rw-r--r--   0 wcleveland   (502) staff       (20)     4281 2023-03-28 14:21:11.000000 astro-gdt-2.0.0/src/gdt/core/time.py
--rw-r--r--   0 wcleveland   (502) staff       (20)    20488 2023-03-28 14:21:11.000000 astro-gdt-2.0.0/src/gdt/core/tte.py
--rw-r--r--   0 wcleveland   (502) staff       (20)    10592 2023-03-28 14:21:11.000000 astro-gdt-2.0.0/src/gdt/core/types.py
-drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-12 19:18:49.943518 astro-gdt-2.0.0/src/gdt/data/
--rw-r--r--   0 wcleveland   (502) staff       (20)   302085 2023-04-12 13:18:15.000000 astro-gdt-2.0.0/src/gdt/data/specfit.npz
+drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-13 16:22:07.076363 astro-gdt-2.0.1/
+-rw-r--r--   0 wcleveland   (502) staff       (20)       44 2023-04-12 13:18:15.000000 astro-gdt-2.0.1/MANIFEST.in
+-rw-r--r--   0 wcleveland   (502) staff       (20)     2156 2023-04-13 16:22:07.076073 astro-gdt-2.0.1/PKG-INFO
+-rw-r--r--   0 wcleveland   (502) staff       (20)     1295 2023-04-13 16:18:43.000000 astro-gdt-2.0.1/PYPI-README.rst
+-rw-r--r--   0 wcleveland   (502) staff       (20)     3648 2023-04-13 16:18:43.000000 astro-gdt-2.0.1/README.rst
+-rw-r--r--   0 wcleveland   (502) staff       (20)    11357 2023-03-28 14:21:11.000000 astro-gdt-2.0.1/license.txt
+drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-13 16:22:07.036507 astro-gdt-2.0.1/scripts/
+-rw-r--r--   0 wcleveland   (502) staff       (20)     6306 2023-04-13 16:18:43.000000 astro-gdt-2.0.1/scripts/gdt-data
+-rw-r--r--   0 wcleveland   (502) staff       (20)       38 2023-04-13 16:22:07.076443 astro-gdt-2.0.1/setup.cfg
+-rw-r--r--   0 wcleveland   (502) staff       (20)     3311 2023-04-13 16:18:43.000000 astro-gdt-2.0.1/setup.py
+drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-13 16:22:07.031819 astro-gdt-2.0.1/src/
+drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-13 16:22:07.038672 astro-gdt-2.0.1/src/astro_gdt.egg-info/
+-rw-r--r--   0 wcleveland   (502) staff       (20)     2156 2023-04-13 16:22:07.000000 astro-gdt-2.0.1/src/astro_gdt.egg-info/PKG-INFO
+-rw-r--r--   0 wcleveland   (502) staff       (20)     1725 2023-04-13 16:22:07.000000 astro-gdt-2.0.1/src/astro_gdt.egg-info/SOURCES.txt
+-rw-r--r--   0 wcleveland   (502) staff       (20)        1 2023-04-13 16:22:07.000000 astro-gdt-2.0.1/src/astro_gdt.egg-info/dependency_links.txt
+-rw-r--r--   0 wcleveland   (502) staff       (20)      187 2023-04-13 16:22:07.000000 astro-gdt-2.0.1/src/astro_gdt.egg-info/requires.txt
+-rw-r--r--   0 wcleveland   (502) staff       (20)        4 2023-04-13 16:22:07.000000 astro-gdt-2.0.1/src/astro_gdt.egg-info/top_level.txt
+drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-13 16:22:07.032889 astro-gdt-2.0.1/src/gdt/
+drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-13 16:22:07.052646 astro-gdt-2.0.1/src/gdt/core/
+-rw-r--r--   0 wcleveland   (502) staff       (20)     1718 2023-04-13 16:18:43.000000 astro-gdt-2.0.1/src/gdt/core/__init__.py
+drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-13 16:22:07.054937 astro-gdt-2.0.1/src/gdt/core/background/
+-rw-r--r--   0 wcleveland   (502) staff       (20)        0 2023-03-28 15:49:38.000000 astro-gdt-2.0.1/src/gdt/core/background/__init__.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)    10352 2023-03-28 15:49:38.000000 astro-gdt-2.0.1/src/gdt/core/background/binned.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)    11176 2023-03-28 15:54:41.000000 astro-gdt-2.0.1/src/gdt/core/background/fitter.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)    15005 2023-04-12 13:18:15.000000 astro-gdt-2.0.1/src/gdt/core/background/primitives.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)    10734 2023-03-28 15:49:38.000000 astro-gdt-2.0.1/src/gdt/core/background/unbinned.py
+drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-13 16:22:07.056616 astro-gdt-2.0.1/src/gdt/core/binning/
+-rw-r--r--   0 wcleveland   (502) staff       (20)        0 2023-03-28 15:49:38.000000 astro-gdt-2.0.1/src/gdt/core/binning/__init__.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)    10018 2023-03-28 15:49:38.000000 astro-gdt-2.0.1/src/gdt/core/binning/binned.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)     7377 2023-03-28 15:49:38.000000 astro-gdt-2.0.1/src/gdt/core/binning/unbinned.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)     8526 2023-04-12 13:18:15.000000 astro-gdt-2.0.1/src/gdt/core/collection.py
+drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-13 16:22:07.057930 astro-gdt-2.0.1/src/gdt/core/coords/
+-rw-r--r--   0 wcleveland   (502) staff       (20)      154 2023-03-28 14:21:11.000000 astro-gdt-2.0.1/src/gdt/core/coords/__init__.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)    13230 2023-03-28 16:25:21.000000 astro-gdt-2.0.1/src/gdt/core/coords/quaternion.py
+drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-13 16:22:07.060323 astro-gdt-2.0.1/src/gdt/core/coords/spacecraft/
+-rw-r--r--   0 wcleveland   (502) staff       (20)     1455 2023-03-28 14:21:11.000000 astro-gdt-2.0.1/src/gdt/core/coords/spacecraft/__init__.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)     5087 2023-03-28 14:21:11.000000 astro-gdt-2.0.1/src/gdt/core/coords/spacecraft/axes.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)    14856 2023-03-28 16:25:21.000000 astro-gdt-2.0.1/src/gdt/core/coords/spacecraft/frame.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)     2915 2023-03-28 14:21:11.000000 astro-gdt-2.0.1/src/gdt/core/coords/spacecraft/model.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)   101533 2023-03-28 14:21:11.000000 astro-gdt-2.0.1/src/gdt/core/data_primitives.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)     5736 2023-03-28 14:21:11.000000 astro-gdt-2.0.1/src/gdt/core/detector.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)     7234 2023-03-28 14:21:11.000000 astro-gdt-2.0.1/src/gdt/core/file.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)     4425 2023-03-28 14:21:11.000000 astro-gdt-2.0.1/src/gdt/core/geomagnetic.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)     7584 2023-03-28 16:04:17.000000 astro-gdt-2.0.1/src/gdt/core/headers.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)    34543 2023-04-12 13:18:15.000000 astro-gdt-2.0.1/src/gdt/core/healpix.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)    20760 2023-03-31 16:28:22.000000 astro-gdt-2.0.1/src/gdt/core/heasarc.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)    24394 2023-03-28 15:54:41.000000 astro-gdt-2.0.1/src/gdt/core/pha.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)    19046 2023-03-28 14:21:11.000000 astro-gdt-2.0.1/src/gdt/core/phaii.py
+drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-13 16:22:07.067000 astro-gdt-2.0.1/src/gdt/core/plot/
+-rw-r--r--   0 wcleveland   (502) staff       (20)        0 2023-03-28 15:49:38.000000 astro-gdt-2.0.1/src/gdt/core/plot/__init__.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)     1768 2023-03-28 15:49:38.000000 astro-gdt-2.0.1/src/gdt/core/plot/defaults.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)    10441 2023-03-28 15:49:38.000000 astro-gdt-2.0.1/src/gdt/core/plot/drm.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)     7634 2023-03-28 15:54:41.000000 astro-gdt-2.0.1/src/gdt/core/plot/earthplot.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)    36973 2023-03-28 15:54:41.000000 astro-gdt-2.0.1/src/gdt/core/plot/lib.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)     8207 2023-03-28 15:49:38.000000 astro-gdt-2.0.1/src/gdt/core/plot/lightcurve.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)    13209 2023-03-28 15:49:38.000000 astro-gdt-2.0.1/src/gdt/core/plot/model.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)    80329 2023-03-28 15:54:41.000000 astro-gdt-2.0.1/src/gdt/core/plot/plot.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)    26448 2023-03-28 15:54:41.000000 astro-gdt-2.0.1/src/gdt/core/plot/sky.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)     8355 2023-03-28 15:49:38.000000 astro-gdt-2.0.1/src/gdt/core/plot/spectrum.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)    25468 2023-03-28 14:21:11.000000 astro-gdt-2.0.1/src/gdt/core/response.py
+drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-13 16:22:07.070299 astro-gdt-2.0.1/src/gdt/core/simulate/
+-rw-r--r--   0 wcleveland   (502) staff       (20)       90 2023-03-28 14:21:11.000000 astro-gdt-2.0.1/src/gdt/core/simulate/__init__.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)    15759 2023-03-28 15:54:41.000000 astro-gdt-2.0.1/src/gdt/core/simulate/generators.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)     9886 2023-03-28 15:54:41.000000 astro-gdt-2.0.1/src/gdt/core/simulate/pha.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)     3902 2023-03-28 14:21:11.000000 astro-gdt-2.0.1/src/gdt/core/simulate/profiles.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)    13459 2023-03-28 16:29:39.000000 astro-gdt-2.0.1/src/gdt/core/simulate/tte.py
+drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-13 16:22:07.073464 astro-gdt-2.0.1/src/gdt/core/spectra/
+-rw-r--r--   0 wcleveland   (502) staff       (20)        0 2023-03-28 14:21:11.000000 astro-gdt-2.0.1/src/gdt/core/spectra/__init__.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)    50761 2023-03-28 15:54:41.000000 astro-gdt-2.0.1/src/gdt/core/spectra/fitting.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)    47277 2023-03-28 14:21:11.000000 astro-gdt-2.0.1/src/gdt/core/spectra/functions.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)    17921 2023-03-28 14:21:11.000000 astro-gdt-2.0.1/src/gdt/core/spectra/parameters.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)     4281 2023-03-28 14:21:11.000000 astro-gdt-2.0.1/src/gdt/core/time.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)    20488 2023-03-28 14:21:11.000000 astro-gdt-2.0.1/src/gdt/core/tte.py
+-rw-r--r--   0 wcleveland   (502) staff       (20)    10592 2023-03-28 14:21:11.000000 astro-gdt-2.0.1/src/gdt/core/types.py
+drwxr-xr-x   0 wcleveland   (502) staff       (20)        0 2023-04-13 16:22:07.073977 astro-gdt-2.0.1/src/gdt/data/
+-rw-r--r--   0 wcleveland   (502) staff       (20)   302085 2023-04-12 13:18:15.000000 astro-gdt-2.0.1/src/gdt/data/specfit.npz
```

### Comparing `astro-gdt-2.0.0/PKG-INFO` & `astro-gdt-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-gdt
-Version: 2.0.0
+Version: 2.0.1
 Summary: Gamma-ray Data Tools: Core Components
 Home-page: https://github.com/USRA-STI/gdt-core
 Author: Cleveland, Goldstein, Kocevski
 Project-URL: Documentation, https://astro-gdt.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/USRA-STI/gdt-core
 Project-URL: Tracker, https://github.com/USRA-STI/gdt-core/issues
 Keywords: astronomy,gammaray,gamma-ray,usra
@@ -38,17 +38,17 @@
 -------------------
 
 If you don't plan to contribute code to the project, the recommended install method is installing from PyPI using:
 
 .. code-block:: sh
 
    pip install astro-gdt
-   gdt data init
+   gdt-data init
 
-The ``gdt data init`` is required to initialize the library after installation.
+The ``gdt-data init`` is required to initialize the library after installation.
 
 
 Contributing Code or Documentation
 ----------------------------------
 
 If you plan to help with the development or documentation of astro-gdt, then please visit our github site at
 https://github.com/USRA-STI/gdt-core.
```

### Comparing `astro-gdt-2.0.0/PYPI-README.rst` & `astro-gdt-2.0.1/PYPI-README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 -------------------
 
 If you don't plan to contribute code to the project, the recommended install method is installing from PyPI using:
 
 .. code-block:: sh
 
    pip install astro-gdt
-   gdt data init
+   gdt-data init
 
-The ``gdt data init`` is required to initialize the library after installation.
+The ``gdt-data init`` is required to initialize the library after installation.
 
 
 Contributing Code or Documentation
 ----------------------------------
 
 If you plan to help with the development or documentation of astro-gdt, then please visit our github site at
 https://github.com/USRA-STI/gdt-core.
```

### Comparing `astro-gdt-2.0.0/README.rst` & `astro-gdt-2.0.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 -------------------
 
 If you don't plan to contribute code to the project, the recommended install method is installing from PyPI using:
 
 .. code-block:: sh
 
    pip install astro-gdt
-   gdt data init
+   gdt-data init
 
-The ``gdt data init`` is required to initialize the library after installation.
+The ``gdt-data init`` is required to initialize the library after installation.
 
 
 Setting up a development environment
 ------------------------------------
 
 If you do want to contribute code to this project (and astro-gdt), you can use the following commands to quickly setup a
 development environment:
```

### Comparing `astro-gdt-2.0.0/license.txt` & `astro-gdt-2.0.1/license.txt`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/scripts/gdt-data` & `astro-gdt-2.0.1/scripts/gdt-data`

 * *Files 6% similar despite different names*

```diff
@@ -26,19 +26,24 @@
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
 # implied. See the License for the specific language governing permissions and limitations under the
 # License.
 #
 import argparse
 import shutil
 from urllib.parse import urlparse
-from importlib.resources import files
-
-import os
 from pathlib import Path
 from typing import List
+
+# Use the backport version if importlib.resources for Python earlier than 3.10
+import sys
+if sys.version_info < (3, 10):
+    from importlib_resources import files
+else:
+    from importlib.resources import files
+
 from gdt.core import data_path
 from gdt.core.heasarc import FileDownloader
 
 gdt_data = files('gdt.data')
 
 
 def get_missions() -> List[str]:
```

### Comparing `astro-gdt-2.0.0/setup.py` & `astro-gdt-2.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
             "Topic :: Software Development :: Libraries",
         ],
         license_files=['license.txt'],
         keywords=['astronomy', 'gammaray', 'gamma-ray', 'usra'],
         package_dir={"": "src"},
         python_requires='>=3.8',
         install_requires=[
-            'importlib-resources;python_version<"3.9"',
+            'importlib-resources;python_version<"3.10"',
             'pyproj>=1.9.6',
             'numpy>=1.17.3',
             'scipy>=1.1.0',
             'matplotlib>=3.7.1',
             'astropy>=3.1',
             'healpy>=1.12.4',
             'cartopy>=0.21.1',
```

### Comparing `astro-gdt-2.0.0/src/astro_gdt.egg-info/PKG-INFO` & `astro-gdt-2.0.1/src/astro_gdt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-gdt
-Version: 2.0.0
+Version: 2.0.1
 Summary: Gamma-ray Data Tools: Core Components
 Home-page: https://github.com/USRA-STI/gdt-core
 Author: Cleveland, Goldstein, Kocevski
 Project-URL: Documentation, https://astro-gdt.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/USRA-STI/gdt-core
 Project-URL: Tracker, https://github.com/USRA-STI/gdt-core/issues
 Keywords: astronomy,gammaray,gamma-ray,usra
@@ -38,17 +38,17 @@
 -------------------
 
 If you don't plan to contribute code to the project, the recommended install method is installing from PyPI using:
 
 .. code-block:: sh
 
    pip install astro-gdt
-   gdt data init
+   gdt-data init
 
-The ``gdt data init`` is required to initialize the library after installation.
+The ``gdt-data init`` is required to initialize the library after installation.
 
 
 Contributing Code or Documentation
 ----------------------------------
 
 If you plan to help with the development or documentation of astro-gdt, then please visit our github site at
 https://github.com/USRA-STI/gdt-core.
```

### Comparing `astro-gdt-2.0.0/src/astro_gdt.egg-info/SOURCES.txt` & `astro-gdt-2.0.1/src/astro_gdt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/__init__.py` & `astro-gdt-2.0.1/src/gdt/core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
 # implied. See the License for the specific language governing permissions and limitations under the
 # License.
 #
 import os
 from pathlib import Path
 
-__version__ = '2.0.0'
+__version__ = '2.0.1'
 
 suite_path = Path(__file__).parent.parent
 
 if 'GDT_BASE' in os.environ:
     base_path = Path(os.environ['GDT_BASE'])
 else:
     base_path = Path.home().joinpath('.gammaray_data_tools', __version__)
```

### Comparing `astro-gdt-2.0.0/src/gdt/core/background/binned.py` & `astro-gdt-2.0.1/src/gdt/core/background/binned.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/background/fitter.py` & `astro-gdt-2.0.1/src/gdt/core/background/fitter.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/background/primitives.py` & `astro-gdt-2.0.1/src/gdt/core/background/primitives.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/background/unbinned.py` & `astro-gdt-2.0.1/src/gdt/core/background/unbinned.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/binning/binned.py` & `astro-gdt-2.0.1/src/gdt/core/binning/binned.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/binning/unbinned.py` & `astro-gdt-2.0.1/src/gdt/core/binning/unbinned.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/collection.py` & `astro-gdt-2.0.1/src/gdt/core/collection.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/coords/quaternion.py` & `astro-gdt-2.0.1/src/gdt/core/coords/quaternion.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/coords/spacecraft/__init__.py` & `astro-gdt-2.0.1/src/gdt/core/coords/spacecraft/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/coords/spacecraft/axes.py` & `astro-gdt-2.0.1/src/gdt/core/coords/spacecraft/axes.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/coords/spacecraft/frame.py` & `astro-gdt-2.0.1/src/gdt/core/coords/spacecraft/frame.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/coords/spacecraft/model.py` & `astro-gdt-2.0.1/src/gdt/core/coords/spacecraft/model.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/data_primitives.py` & `astro-gdt-2.0.1/src/gdt/core/data_primitives.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/detector.py` & `astro-gdt-2.0.1/src/gdt/core/detector.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/file.py` & `astro-gdt-2.0.1/src/gdt/core/file.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/geomagnetic.py` & `astro-gdt-2.0.1/src/gdt/core/geomagnetic.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/headers.py` & `astro-gdt-2.0.1/src/gdt/core/headers.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/healpix.py` & `astro-gdt-2.0.1/src/gdt/core/healpix.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/heasarc.py` & `astro-gdt-2.0.1/src/gdt/core/heasarc.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/pha.py` & `astro-gdt-2.0.1/src/gdt/core/pha.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/phaii.py` & `astro-gdt-2.0.1/src/gdt/core/phaii.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/plot/defaults.py` & `astro-gdt-2.0.1/src/gdt/core/plot/defaults.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/plot/drm.py` & `astro-gdt-2.0.1/src/gdt/core/plot/drm.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/plot/earthplot.py` & `astro-gdt-2.0.1/src/gdt/core/plot/earthplot.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/plot/lib.py` & `astro-gdt-2.0.1/src/gdt/core/plot/lib.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/plot/lightcurve.py` & `astro-gdt-2.0.1/src/gdt/core/plot/lightcurve.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/plot/model.py` & `astro-gdt-2.0.1/src/gdt/core/plot/model.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/plot/plot.py` & `astro-gdt-2.0.1/src/gdt/core/plot/plot.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/plot/sky.py` & `astro-gdt-2.0.1/src/gdt/core/plot/sky.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/plot/spectrum.py` & `astro-gdt-2.0.1/src/gdt/core/plot/spectrum.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/response.py` & `astro-gdt-2.0.1/src/gdt/core/response.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/simulate/generators.py` & `astro-gdt-2.0.1/src/gdt/core/simulate/generators.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/simulate/pha.py` & `astro-gdt-2.0.1/src/gdt/core/simulate/pha.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/simulate/profiles.py` & `astro-gdt-2.0.1/src/gdt/core/simulate/profiles.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/simulate/tte.py` & `astro-gdt-2.0.1/src/gdt/core/simulate/tte.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/spectra/fitting.py` & `astro-gdt-2.0.1/src/gdt/core/spectra/fitting.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/spectra/functions.py` & `astro-gdt-2.0.1/src/gdt/core/spectra/functions.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/spectra/parameters.py` & `astro-gdt-2.0.1/src/gdt/core/spectra/parameters.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/time.py` & `astro-gdt-2.0.1/src/gdt/core/time.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/tte.py` & `astro-gdt-2.0.1/src/gdt/core/tte.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/core/types.py` & `astro-gdt-2.0.1/src/gdt/core/types.py`

 * *Files identical despite different names*

### Comparing `astro-gdt-2.0.0/src/gdt/data/specfit.npz` & `astro-gdt-2.0.1/src/gdt/data/specfit.npz`

 * *Files identical despite different names*

