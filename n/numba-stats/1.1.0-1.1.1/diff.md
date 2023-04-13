# Comparing `tmp/numba-stats-1.1.0.tar.gz` & `tmp/numba-stats-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numba-stats-1.1.0.tar", last modified: Tue Mar 15 14:29:14 2022, max compression
+gzip compressed data, was "numba-stats-1.1.1.tar", last modified: Thu Apr 13 13:50:30 2023, max compression
```

## Comparing `numba-stats-1.1.0.tar` & `numba-stats-1.1.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 hdembinski   (501) staff       (20)        0 2022-03-15 14:29:14.364712 numba-stats-1.1.0/
-drwxr-xr-x   0 hdembinski   (501) staff       (20)        0 2022-03-15 14:29:14.343386 numba-stats-1.1.0/.github/
-drwxr-xr-x   0 hdembinski   (501) staff       (20)        0 2022-03-15 14:29:14.348161 numba-stats-1.1.0/.github/workflows/
--rw-r--r--   0 hdembinski   (501) staff       (20)      485 2022-03-07 17:37:00.000000 numba-stats-1.1.0/.github/workflows/ci.yml
--rw-r--r--   0 hdembinski   (501) staff       (20)      556 2022-03-15 14:28:04.000000 numba-stats-1.1.0/.github/workflows/release.yml
--rw-r--r--   0 hdembinski   (501) staff       (20)      144 2022-03-07 08:38:35.000000 numba-stats-1.1.0/.gitignore
--rw-r--r--   0 hdembinski   (501) staff       (20)     1063 2022-03-07 17:37:00.000000 numba-stats-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0 hdembinski   (501) staff       (20)     1071 2021-02-02 14:57:10.000000 numba-stats-1.1.0/LICENSE
--rw-r--r--   0 hdembinski   (501) staff       (20)       60 2021-07-20 11:46:23.000000 numba-stats-1.1.0/MANIFEST.in
--rw-r--r--   0 hdembinski   (501) staff       (20)     3580 2022-03-15 14:29:14.365029 numba-stats-1.1.0/PKG-INFO
--rw-r--r--   0 hdembinski   (501) staff       (20)     2695 2022-03-07 17:37:00.000000 numba-stats-1.1.0/README.md
-drwxr-xr-x   0 hdembinski   (501) staff       (20)        0 2022-03-15 14:29:14.348812 numba-stats-1.1.0/benchmarks/
--rw-r--r--   0 hdembinski   (501) staff       (20)        0 2021-02-02 14:06:13.000000 numba-stats-1.1.0/benchmarks/__init__.py
--rw-r--r--   0 hdembinski   (501) staff       (20)     4696 2022-03-14 18:09:25.000000 numba-stats-1.1.0/benchmarks/test_stats.py
--rwxr-xr-x   0 hdembinski   (501) staff       (20)       57 2021-07-20 14:22:37.000000 numba-stats-1.1.0/coverage.sh
--rw-r--r--   0 hdembinski   (501) staff       (20)      287 2022-03-03 20:21:02.000000 numba-stats-1.1.0/pyproject.toml
--rw-r--r--   0 hdembinski   (501) staff       (20)      834 2022-03-15 14:29:14.366062 numba-stats-1.1.0/setup.cfg
--rw-r--r--   0 hdembinski   (501) staff       (20)      158 2021-07-20 14:22:37.000000 numba-stats-1.1.0/setup.py
-drwxr-xr-x   0 hdembinski   (501) staff       (20)        0 2022-03-15 14:29:14.344079 numba-stats-1.1.0/src/
-drwxr-xr-x   0 hdembinski   (501) staff       (20)        0 2022-03-15 14:29:14.355858 numba-stats-1.1.0/src/numba_stats/
--rw-r--r--   0 hdembinski   (501) staff       (20)       53 2022-02-24 08:48:26.000000 numba-stats-1.1.0/src/numba_stats/__init__.py
--rw-r--r--   0 hdembinski   (501) staff       (20)     1514 2021-08-02 08:03:05.000000 numba-stats-1.1.0/src/numba_stats/_special.py
--rw-r--r--   0 hdembinski   (501) staff       (20)     2929 2022-03-14 18:09:25.000000 numba-stats-1.1.0/src/numba_stats/_util.py
--rw-r--r--   0 hdembinski   (501) staff       (20)      142 2022-03-15 14:29:14.000000 numba-stats-1.1.0/src/numba_stats/_version.py
--rw-r--r--   0 hdembinski   (501) staff       (20)     5049 2022-03-14 18:09:25.000000 numba-stats-1.1.0/src/numba_stats/bernstein.py
--rw-r--r--   0 hdembinski   (501) staff       (20)     1073 2022-03-14 18:09:25.000000 numba-stats-1.1.0/src/numba_stats/cpoisson.py
--rw-r--r--   0 hdembinski   (501) staff       (20)     2243 2022-03-14 18:09:25.000000 numba-stats-1.1.0/src/numba_stats/crystalball.py
--rw-r--r--   0 hdembinski   (501) staff       (20)     3932 2022-03-14 18:09:25.000000 numba-stats-1.1.0/src/numba_stats/crystalball_ex.py
--rw-r--r--   0 hdembinski   (501) staff       (20)     1508 2022-03-14 18:09:25.000000 numba-stats-1.1.0/src/numba_stats/expon.py
--rw-r--r--   0 hdembinski   (501) staff       (20)     1339 2022-03-14 18:09:25.000000 numba-stats-1.1.0/src/numba_stats/lognorm.py
--rw-r--r--   0 hdembinski   (501) staff       (20)     1293 2022-03-14 18:09:25.000000 numba-stats-1.1.0/src/numba_stats/norm.py
--rw-r--r--   0 hdembinski   (501) staff       (20)      860 2022-03-14 18:09:25.000000 numba-stats-1.1.0/src/numba_stats/poisson.py
--rw-r--r--   0 hdembinski   (501) staff       (20)     2046 2022-03-07 17:37:00.000000 numba-stats-1.1.0/src/numba_stats/qgaussian.py
--rw-r--r--   0 hdembinski   (501) staff       (20)     1357 2022-03-14 18:09:25.000000 numba-stats-1.1.0/src/numba_stats/t.py
--rw-r--r--   0 hdembinski   (501) staff       (20)     1836 2022-03-14 18:09:25.000000 numba-stats-1.1.0/src/numba_stats/truncexpon.py
--rw-r--r--   0 hdembinski   (501) staff       (20)     1793 2022-03-14 18:09:25.000000 numba-stats-1.1.0/src/numba_stats/truncnorm.py
--rw-r--r--   0 hdembinski   (501) staff       (20)     1218 2022-03-07 17:37:00.000000 numba-stats-1.1.0/src/numba_stats/tsallis.py
--rw-r--r--   0 hdembinski   (501) staff       (20)      922 2022-03-14 18:09:25.000000 numba-stats-1.1.0/src/numba_stats/uniform.py
--rw-r--r--   0 hdembinski   (501) staff       (20)      891 2022-03-14 18:09:25.000000 numba-stats-1.1.0/src/numba_stats/voigt.py
-drwxr-xr-x   0 hdembinski   (501) staff       (20)        0 2022-03-15 14:29:14.357812 numba-stats-1.1.0/src/numba_stats.egg-info/
--rw-r--r--   0 hdembinski   (501) staff       (20)     3580 2022-03-15 14:29:14.000000 numba-stats-1.1.0/src/numba_stats.egg-info/PKG-INFO
--rw-r--r--   0 hdembinski   (501) staff       (20)     1303 2022-03-15 14:29:14.000000 numba-stats-1.1.0/src/numba_stats.egg-info/SOURCES.txt
--rw-r--r--   0 hdembinski   (501) staff       (20)        1 2022-03-15 14:29:14.000000 numba-stats-1.1.0/src/numba_stats.egg-info/dependency_links.txt
--rw-r--r--   0 hdembinski   (501) staff       (20)       89 2022-03-15 14:29:14.000000 numba-stats-1.1.0/src/numba_stats.egg-info/requires.txt
--rw-r--r--   0 hdembinski   (501) staff       (20)       12 2022-03-15 14:29:14.000000 numba-stats-1.1.0/src/numba_stats.egg-info/top_level.txt
-drwxr-xr-x   0 hdembinski   (501) staff       (20)        0 2022-03-15 14:29:14.364371 numba-stats-1.1.0/tests/
--rw-r--r--   0 hdembinski   (501) staff       (20)        0 2021-03-27 11:51:03.000000 numba-stats-1.1.0/tests/__init__.py
--rw-r--r--   0 hdembinski   (501) staff       (20)     2117 2022-03-14 18:09:25.000000 numba-stats-1.1.0/tests/test_bernstein.py
--rw-r--r--   0 hdembinski   (501) staff       (20)      280 2022-03-07 08:38:35.000000 numba-stats-1.1.0/tests/test_cpoisson.py
--rw-r--r--   0 hdembinski   (501) staff       (20)     1641 2022-03-03 21:37:03.000000 numba-stats-1.1.0/tests/test_crystalball.py
--rw-r--r--   0 hdembinski   (501) staff       (20)     1868 2022-03-14 17:55:18.000000 numba-stats-1.1.0/tests/test_crystalball_ex.py
--rw-r--r--   0 hdembinski   (501) staff       (20)      577 2022-03-07 17:37:00.000000 numba-stats-1.1.0/tests/test_doc.py
--rw-r--r--   0 hdembinski   (501) staff       (20)      558 2022-03-07 08:38:35.000000 numba-stats-1.1.0/tests/test_expon.py
--rw-r--r--   0 hdembinski   (501) staff       (20)     1324 2022-03-07 08:38:35.000000 numba-stats-1.1.0/tests/test_lognorm.py
--rw-r--r--   0 hdembinski   (501) staff       (20)     1355 2022-03-14 18:09:25.000000 numba-stats-1.1.0/tests/test_norm.py
--rw-r--r--   0 hdembinski   (501) staff       (20)      504 2022-03-07 08:38:35.000000 numba-stats-1.1.0/tests/test_poisson.py
--rw-r--r--   0 hdembinski   (501) staff       (20)     1744 2022-03-07 08:38:35.000000 numba-stats-1.1.0/tests/test_qgaussian.py
--rw-r--r--   0 hdembinski   (501) staff       (20)      818 2022-03-03 21:25:10.000000 numba-stats-1.1.0/tests/test_t.py
--rw-r--r--   0 hdembinski   (501) staff       (20)     1093 2022-03-07 08:38:35.000000 numba-stats-1.1.0/tests/test_truncexpon.py
--rw-r--r--   0 hdembinski   (501) staff       (20)     1678 2022-01-09 14:09:27.000000 numba-stats-1.1.0/tests/test_truncnorm.py
--rw-r--r--   0 hdembinski   (501) staff       (20)      674 2022-03-07 08:38:35.000000 numba-stats-1.1.0/tests/test_tsallis.py
--rw-r--r--   0 hdembinski   (501) staff       (20)      921 2022-03-07 08:38:35.000000 numba-stats-1.1.0/tests/test_uniform.py
--rw-r--r--   0 hdembinski   (501) staff       (20)      366 2022-03-03 21:25:10.000000 numba-stats-1.1.0/tests/test_voigt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:50:30.748338 numba-stats-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:50:30.724336 numba-stats-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:50:30.728336 numba-stats-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-13 13:50:01.000000 numba-stats-1.1.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-13 13:50:01.000000 numba-stats-1.1.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-13 13:50:01.000000 numba-stats-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-13 13:50:01.000000 numba-stats-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-13 13:50:01.000000 numba-stats-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-13 13:50:01.000000 numba-stats-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-13 13:50:30.748338 numba-stats-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-13 13:50:01.000000 numba-stats-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:50:30.732336 numba-stats-1.1.1/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 13:50:01.000000 numba-stats-1.1.1/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-04-13 13:50:01.000000 numba-stats-1.1.1/benchmarks/test_stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       57 2023-04-13 13:50:01.000000 numba-stats-1.1.1/coverage.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-13 13:50:01.000000 numba-stats-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-13 13:50:30.748338 numba-stats-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-13 13:50:01.000000 numba-stats-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:50:30.724336 numba-stats-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:50:30.740337 numba-stats-1.1.1/src/numba_stats/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/_special.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 13:50:18.000000 numba-stats-1.1.1/src/numba_stats/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/bernstein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/cpoisson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/crystalball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/crystalball_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/expon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/lognorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/poisson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/qgaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/t.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/truncexpon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/truncnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/tsallis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/uniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-13 13:50:01.000000 numba-stats-1.1.1/src/numba_stats/voigt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:50:30.740337 numba-stats-1.1.1/src/numba_stats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-13 13:50:30.000000 numba-stats-1.1.1/src/numba_stats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-13 13:50:30.000000 numba-stats-1.1.1/src/numba_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 13:50:30.000000 numba-stats-1.1.1/src/numba_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-13 13:50:30.000000 numba-stats-1.1.1/src/numba_stats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 13:50:30.000000 numba-stats-1.1.1/src/numba_stats.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:50:30.748338 numba-stats-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/test_bernstein.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/test_cpoisson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/test_crystalball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/test_crystalball_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/test_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/test_expon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/test_lognorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/test_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/test_poisson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/test_qgaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/test_t.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/test_truncexpon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/test_truncnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/test_tsallis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/test_uniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-13 13:50:01.000000 numba-stats-1.1.1/tests/test_voigt.py
```

### Comparing `numba-stats-1.1.0/.github/workflows/release.yml` & `numba-stats-1.1.1/.github/workflows/release.yml`

 * *Files 22% similar despite different names*

```diff
@@ -11,19 +11,18 @@
     steps:
     - uses: actions/checkout@v2
 
     - uses: actions/setup-python@v2
       with:
         python-version: '3.9'
 
-    - run: |
-        python -m pip install --upgrade pip
-        python -m pip install --prefer-binary -e .[test]
-
-    - run: python -m pytest
-
+    # do not remove wheel
+    - run: python -m pip install --upgrade pip wheel
+    - run: python -m pip install --prefer-binary -e .[test]
     - run: python setup.py sdist bdist_wheel
+    - run: python -m pip install --force-reinstall dist/*.tar.gz
+    - run: python -m pytest
 
     - uses: pypa/gh-action-pypi-publish@master
       with:
         user: __token__
         password: ${{secrets.PYPI_TOKEN}}
```

### Comparing `numba-stats-1.1.0/.pre-commit-config.yaml` & `numba-stats-1.1.1/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #     pre-commit autoupdate
 #
 # See https://github.com/pre-commit/pre-commit
 
 repos:
 # Standard hooks
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.1.0
+  rev: v4.4.0
   hooks:
   - id: check-case-conflict
   - id: check-docstring-first
   - id: check-executables-have-shebangs
   - id: check-merge-conflict
   - id: check-symlinks
   - id: check-yaml
@@ -29,24 +29,24 @@
   - id: sort-simple-yaml
   - id: file-contents-sorter
   - id: trailing-whitespace
     exclude: ^doc/_static/.*.svg
 
 # Python linter (Flake8)
 - repo: https://github.com/PyCQA/flake8
-  rev: 4.0.1
+  rev: 6.0.0
   hooks:
   - id: flake8
 
 # Python docstring formatting
 - repo: https://github.com/pycqa/pydocstyle
-  rev: 6.1.1
+  rev: 6.3.0
   hooks:
   - id: pydocstyle
     args: ["--convention=numpy"]
     files: src/numba_stats/[^_].*\.py
 
 # Python formatting
 - repo: https://github.com/psf/black
-  rev: 22.1.0
+  rev: 23.3.0
   hooks:
   - id: black
```

### Comparing `numba-stats-1.1.0/LICENSE` & `numba-stats-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.0/PKG-INFO` & `numba-stats-1.1.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,72 +1,58 @@
-Metadata-Version: 2.1
-Name: numba-stats
-Version: 1.1.0
-Summary: Numba-accelerated implementations of common probability distributions
-Home-page: UNKNOWN
-Author: Hans Dembinski
-Author-email: hans.dembinski@gmail.com
-License: "MIT"
-Project-URL: Bug Tracker, https://github.com/hdembinski/numba-stats/issues
-Description: # numba-stats
-        
-        ![](https://img.shields.io/pypi/v/numba-stats.svg)
-        
-        We provide numba-accelerated implementations of statistical functions for common probability distributions
-        
-        * Uniform
-        * (Truncated) Normal
-        * Log-normal
-        * Poisson
-        * (Truncated) Exponential
-        * Student's t
-        * Voigtian
-        * Crystal Ball
-        * Generalised double-sided Crystal Ball
-        * Tsallis-Hagedorn, a model for the minimum bias pT distribution
-        * Q-Gaussian
-        * Bernstein density (not normalised to unity, use this in extended likelihood fits)
-        
-        with more to come. The speed gains are huge, up to a factor of 100 compared to `scipy`. Benchmarks are included in the repository and are run by `pytest`.
-        
-        ## Usage
-        
-        Each distribution is implemented in a submodule. Import the submodule that you need.
-        ```py
-        from numba_stats import norm
-        import numpy as np
-        
-        x = np.linspace(-10, 10)
-        mu = 2
-        sigma = 3
-        
-        dp = norm.pdf(x, mu, sigma)
-        p = norm.cdf(x, mu, sigma)
-        ```
-        The functions are vectorised on the variate `x`, but not on the shape parameters of the distribution. Ideally, the following functions are implemented for each distribution:
-        * `logpdf`
-        * `pdf`
-        * `cdf`
-        * `ppf`
-        
-        `cdf` and `ppf` are missing for some distributions (e.g. `voigt`), if there is currently no fast implementation available. `logpdf` is only implemented if it is more efficient and accurate compared to computing `log(dist.pdf(...))`.
-        
-        ## Documentation
-        
-        To get documentation, please use `help()` in the Python interpreter.
-        
-        Functions with equivalents in `scipy.stats` follow the Scipy calling conventions exactly. These conventions are sometimes a bit unusual, for example, in case of the exponential, the log-normal or the uniform distribution. See the SciPy docs for details.
-        
-        ## Contributions
-        
-        **You can help with adding more distributions, patches are very welcome.** Implementing a probability distribution is easy. You need to write it in simple Python that `numba` can understand. Special functions from `scipy.special` can be used after some wrapping, see submodule `numba_stats._special.py` how it is done.
-        
-        ## numba-stats and numba-scipy
-        
-        [numba-scipy](https://github.com/numba/numba-scipy) is the official package and repository for fast numba-accelerated scipy functions, are we reinventing the wheel?
-        
-        Ideally, the functionality in this package should be in `numba-scipy` and we hope that eventually this will be case. In this package, we don't offer overloads for scipy functions and classes like `numba-scipy` does. This simplifies the implementation dramatically. `numba-stats` is intended as a temporary solution until fast statistical functions are included in `numba-scipy`. `numba-stats` currently does not depend on `numba-scipy`, only on `numba` and `scipy`.
-        
-Platform: UNKNOWN
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
+# numba-stats
+
+![](https://img.shields.io/pypi/v/numba-stats.svg)
+
+We provide numba-accelerated implementations of statistical functions for common probability distributions
+
+* Uniform
+* (Truncated) Normal
+* Log-normal
+* Poisson
+* (Truncated) Exponential
+* Student's t
+* Voigtian
+* Crystal Ball
+* Generalised double-sided Crystal Ball
+* Tsallis-Hagedorn, a model for the minimum bias pT distribution
+* Q-Gaussian
+* Bernstein density (not normalised to unity, use this in extended likelihood fits)
+
+with more to come. The speed gains are huge, up to a factor of 100 compared to `scipy`. Benchmarks are included in the repository and are run by `pytest`.
+
+## Usage
+
+Each distribution is implemented in a submodule. Import the submodule that you need.
+```py
+from numba_stats import norm
+import numpy as np
+
+x = np.linspace(-10, 10)
+mu = 2
+sigma = 3
+
+dp = norm.pdf(x, mu, sigma)
+p = norm.cdf(x, mu, sigma)
+```
+The functions are vectorised on the variate `x`, but not on the shape parameters of the distribution. Ideally, the following functions are implemented for each distribution:
+* `logpdf`
+* `pdf`
+* `cdf`
+* `ppf`
+
+`cdf` and `ppf` are missing for some distributions (e.g. `voigt`), if there is currently no fast implementation available. `logpdf` is only implemented if it is more efficient and accurate compared to computing `log(dist.pdf(...))`.
+
+## Documentation
+
+To get documentation, please use `help()` in the Python interpreter.
+
+Functions with equivalents in `scipy.stats` follow the Scipy calling conventions exactly. These conventions are sometimes a bit unusual, for example, in case of the exponential, the log-normal or the uniform distribution. See the SciPy docs for details.
+
+## Contributions
+
+**You can help with adding more distributions, patches are very welcome.** Implementing a probability distribution is easy. You need to write it in simple Python that `numba` can understand. Special functions from `scipy.special` can be used after some wrapping, see submodule `numba_stats._special.py` how it is done.
+
+## numba-stats and numba-scipy
+
+[numba-scipy](https://github.com/numba/numba-scipy) is the official package and repository for fast numba-accelerated scipy functions, are we reinventing the wheel?
+
+Ideally, the functionality in this package should be in `numba-scipy` and we hope that eventually this will be case. In this package, we don't offer overloads for scipy functions and classes like `numba-scipy` does. This simplifies the implementation dramatically. `numba-stats` is intended as a temporary solution until fast statistical functions are included in `numba-scipy`. `numba-stats` currently does not depend on `numba-scipy`, only on `numba` and `scipy`.
```

### Comparing `numba-stats-1.1.0/README.md` & `numba-stats-1.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: numba-stats
+Version: 1.1.1
+Summary: Numba-accelerated implementations of common probability distributions
+Home-page: UNKNOWN
+Author: Hans Dembinski
+Author-email: hans.dembinski@gmail.com
+License: "MIT"
+Project-URL: Bug Tracker, https://github.com/hdembinski/numba-stats/issues
+Platform: UNKNOWN
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: test
+
 # numba-stats
 
 ![](https://img.shields.io/pypi/v/numba-stats.svg)
 
 We provide numba-accelerated implementations of statistical functions for common probability distributions
 
 * Uniform
@@ -52,7 +66,9 @@
 **You can help with adding more distributions, patches are very welcome.** Implementing a probability distribution is easy. You need to write it in simple Python that `numba` can understand. Special functions from `scipy.special` can be used after some wrapping, see submodule `numba_stats._special.py` how it is done.
 
 ## numba-stats and numba-scipy
 
 [numba-scipy](https://github.com/numba/numba-scipy) is the official package and repository for fast numba-accelerated scipy functions, are we reinventing the wheel?
 
 Ideally, the functionality in this package should be in `numba-scipy` and we hope that eventually this will be case. In this package, we don't offer overloads for scipy functions and classes like `numba-scipy` does. This simplifies the implementation dramatically. `numba-stats` is intended as a temporary solution until fast statistical functions are included in `numba-scipy`. `numba-stats` currently does not depend on `numba-scipy`, only on `numba` and `scipy`.
+
+
```

### Comparing `numba-stats-1.1.0/benchmarks/test_stats.py` & `numba-stats-1.1.1/benchmarks/test_stats.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.0/setup.cfg` & `numba-stats-1.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.0/src/numba_stats/bernstein.py` & `numba-stats-1.1.1/src/numba_stats/bernstein.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.0/src/numba_stats/cpoisson.py` & `numba-stats-1.1.1/src/numba_stats/cpoisson.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.0/src/numba_stats/crystalball.py` & `numba-stats-1.1.1/src/numba_stats/crystalball.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.0/src/numba_stats/crystalball_ex.py` & `numba-stats-1.1.1/src/numba_stats/crystalball_ex.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.0/src/numba_stats/expon.py` & `numba-stats-1.1.1/src/numba_stats/expon.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.0/src/numba_stats/lognorm.py` & `numba-stats-1.1.1/src/numba_stats/lognorm.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.0/src/numba_stats/norm.py` & `numba-stats-1.1.1/src/numba_stats/norm.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Normal distribution.
 
 See Also
 --------
 scipy.stats.norm: Scipy equivalent.
 """
 import numpy as np
-from ._special import erfinv as _erfinv
+from ._special import ndtri as _ndtri
 from ._util import _jit, _trans, _generate_wrappers, _prange
 from math import erf as _erf
 
 _doc_par = """
 x : ArrayLike
     Random variate.
 loc : float
@@ -29,18 +29,18 @@
 @_jit(-1)
 def _cdf1(z):
     T = type(z)
     c = T(np.sqrt(0.5))
     return T(0.5) * (T(1.0) + _erf(z * c))
 
 
-@_jit(-1, cache=False)  # cannot cache because of _erfinv
+@_jit(-1, cache=False)  # cannot cache because of _ndtri
 def _ppf1(p):
     T = type(p)
-    return T(np.sqrt(2)) * _erfinv(T(2) * p - T(1))
+    return T(_ndtri(p))
 
 
 @_jit(2)
 def _logpdf(x, loc, scale):
     r = _trans(x, loc, scale)
     for i in _prange(len(r)):
         r[i] = _logpdf1(r[i]) - np.log(scale)
```

### Comparing `numba-stats-1.1.0/src/numba_stats/poisson.py` & `numba-stats-1.1.1/src/numba_stats/poisson.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.0/src/numba_stats/qgaussian.py` & `numba-stats-1.1.1/src/numba_stats/qgaussian.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.0/src/numba_stats/t.py` & `numba-stats-1.1.1/src/numba_stats/t.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.0/src/numba_stats/truncexpon.py` & `numba-stats-1.1.1/src/numba_stats/truncexpon.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.0/src/numba_stats/truncnorm.py` & `numba-stats-1.1.1/src/numba_stats/truncnorm.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.0/src/numba_stats/tsallis.py` & `numba-stats-1.1.1/src/numba_stats/tsallis.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.0/src/numba_stats/uniform.py` & `numba-stats-1.1.1/src/numba_stats/uniform.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.0/src/numba_stats/voigt.py` & `numba-stats-1.1.1/src/numba_stats/voigt.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.0/src/numba_stats.egg-info/PKG-INFO` & `numba-stats-1.1.1/src/numba_stats.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,72 +1,74 @@
 Metadata-Version: 2.1
 Name: numba-stats
-Version: 1.1.0
+Version: 1.1.1
 Summary: Numba-accelerated implementations of common probability distributions
 Home-page: UNKNOWN
 Author: Hans Dembinski
 Author-email: hans.dembinski@gmail.com
 License: "MIT"
 Project-URL: Bug Tracker, https://github.com/hdembinski/numba-stats/issues
-Description: # numba-stats
-        
-        ![](https://img.shields.io/pypi/v/numba-stats.svg)
-        
-        We provide numba-accelerated implementations of statistical functions for common probability distributions
-        
-        * Uniform
-        * (Truncated) Normal
-        * Log-normal
-        * Poisson
-        * (Truncated) Exponential
-        * Student's t
-        * Voigtian
-        * Crystal Ball
-        * Generalised double-sided Crystal Ball
-        * Tsallis-Hagedorn, a model for the minimum bias pT distribution
-        * Q-Gaussian
-        * Bernstein density (not normalised to unity, use this in extended likelihood fits)
-        
-        with more to come. The speed gains are huge, up to a factor of 100 compared to `scipy`. Benchmarks are included in the repository and are run by `pytest`.
-        
-        ## Usage
-        
-        Each distribution is implemented in a submodule. Import the submodule that you need.
-        ```py
-        from numba_stats import norm
-        import numpy as np
-        
-        x = np.linspace(-10, 10)
-        mu = 2
-        sigma = 3
-        
-        dp = norm.pdf(x, mu, sigma)
-        p = norm.cdf(x, mu, sigma)
-        ```
-        The functions are vectorised on the variate `x`, but not on the shape parameters of the distribution. Ideally, the following functions are implemented for each distribution:
-        * `logpdf`
-        * `pdf`
-        * `cdf`
-        * `ppf`
-        
-        `cdf` and `ppf` are missing for some distributions (e.g. `voigt`), if there is currently no fast implementation available. `logpdf` is only implemented if it is more efficient and accurate compared to computing `log(dist.pdf(...))`.
-        
-        ## Documentation
-        
-        To get documentation, please use `help()` in the Python interpreter.
-        
-        Functions with equivalents in `scipy.stats` follow the Scipy calling conventions exactly. These conventions are sometimes a bit unusual, for example, in case of the exponential, the log-normal or the uniform distribution. See the SciPy docs for details.
-        
-        ## Contributions
-        
-        **You can help with adding more distributions, patches are very welcome.** Implementing a probability distribution is easy. You need to write it in simple Python that `numba` can understand. Special functions from `scipy.special` can be used after some wrapping, see submodule `numba_stats._special.py` how it is done.
-        
-        ## numba-stats and numba-scipy
-        
-        [numba-scipy](https://github.com/numba/numba-scipy) is the official package and repository for fast numba-accelerated scipy functions, are we reinventing the wheel?
-        
-        Ideally, the functionality in this package should be in `numba-scipy` and we hope that eventually this will be case. In this package, we don't offer overloads for scipy functions and classes like `numba-scipy` does. This simplifies the implementation dramatically. `numba-stats` is intended as a temporary solution until fast statistical functions are included in `numba-scipy`. `numba-stats` currently does not depend on `numba-scipy`, only on `numba` and `scipy`.
-        
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
+
+# numba-stats
+
+![](https://img.shields.io/pypi/v/numba-stats.svg)
+
+We provide numba-accelerated implementations of statistical functions for common probability distributions
+
+* Uniform
+* (Truncated) Normal
+* Log-normal
+* Poisson
+* (Truncated) Exponential
+* Student's t
+* Voigtian
+* Crystal Ball
+* Generalised double-sided Crystal Ball
+* Tsallis-Hagedorn, a model for the minimum bias pT distribution
+* Q-Gaussian
+* Bernstein density (not normalised to unity, use this in extended likelihood fits)
+
+with more to come. The speed gains are huge, up to a factor of 100 compared to `scipy`. Benchmarks are included in the repository and are run by `pytest`.
+
+## Usage
+
+Each distribution is implemented in a submodule. Import the submodule that you need.
+```py
+from numba_stats import norm
+import numpy as np
+
+x = np.linspace(-10, 10)
+mu = 2
+sigma = 3
+
+dp = norm.pdf(x, mu, sigma)
+p = norm.cdf(x, mu, sigma)
+```
+The functions are vectorised on the variate `x`, but not on the shape parameters of the distribution. Ideally, the following functions are implemented for each distribution:
+* `logpdf`
+* `pdf`
+* `cdf`
+* `ppf`
+
+`cdf` and `ppf` are missing for some distributions (e.g. `voigt`), if there is currently no fast implementation available. `logpdf` is only implemented if it is more efficient and accurate compared to computing `log(dist.pdf(...))`.
+
+## Documentation
+
+To get documentation, please use `help()` in the Python interpreter.
+
+Functions with equivalents in `scipy.stats` follow the Scipy calling conventions exactly. These conventions are sometimes a bit unusual, for example, in case of the exponential, the log-normal or the uniform distribution. See the SciPy docs for details.
+
+## Contributions
+
+**You can help with adding more distributions, patches are very welcome.** Implementing a probability distribution is easy. You need to write it in simple Python that `numba` can understand. Special functions from `scipy.special` can be used after some wrapping, see submodule `numba_stats._special.py` how it is done.
+
+## numba-stats and numba-scipy
+
+[numba-scipy](https://github.com/numba/numba-scipy) is the official package and repository for fast numba-accelerated scipy functions, are we reinventing the wheel?
+
+Ideally, the functionality in this package should be in `numba-scipy` and we hope that eventually this will be case. In this package, we don't offer overloads for scipy functions and classes like `numba-scipy` does. This simplifies the implementation dramatically. `numba-stats` is intended as a temporary solution until fast statistical functions are included in `numba-scipy`. `numba-stats` currently does not depend on `numba-scipy`, only on `numba` and `scipy`.
+
+
```

### Comparing `numba-stats-1.1.0/src/numba_stats.egg-info/SOURCES.txt` & `numba-stats-1.1.1/src/numba_stats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.0/tests/test_bernstein.py` & `numba-stats-1.1.1/tests/test_bernstein.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.0/tests/test_crystalball.py` & `numba-stats-1.1.1/tests/test_crystalball.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.0/tests/test_crystalball_ex.py` & `numba-stats-1.1.1/tests/test_crystalball_ex.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.0/tests/test_doc.py` & `numba-stats-1.1.1/tests/test_doc.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.0/tests/test_expon.py` & `numba-stats-1.1.1/tests/test_expon.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.0/tests/test_lognorm.py` & `numba-stats-1.1.1/tests/test_lognorm.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.0/tests/test_norm.py` & `numba-stats-1.1.1/tests/test_norm.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.0/tests/test_qgaussian.py` & `numba-stats-1.1.1/tests/test_qgaussian.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.0/tests/test_t.py` & `numba-stats-1.1.1/tests/test_t.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.0/tests/test_truncexpon.py` & `numba-stats-1.1.1/tests/test_truncexpon.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.0/tests/test_truncnorm.py` & `numba-stats-1.1.1/tests/test_truncnorm.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.0/tests/test_tsallis.py` & `numba-stats-1.1.1/tests/test_tsallis.py`

 * *Files identical despite different names*

### Comparing `numba-stats-1.1.0/tests/test_uniform.py` & `numba-stats-1.1.1/tests/test_uniform.py`

 * *Files identical despite different names*

