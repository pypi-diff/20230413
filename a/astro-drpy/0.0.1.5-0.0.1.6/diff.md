# Comparing `tmp/astro-drpy-0.0.1.5.tar.gz` & `tmp/astro-drpy-0.0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-drpy-0.0.1.5.tar", last modified: Tue Apr  4 17:02:28 2023, max compression
+gzip compressed data, was "astro-drpy-0.0.1.6.tar", last modified: Thu Apr 13 06:39:09 2023, max compression
```

## Comparing `astro-drpy-0.0.1.5.tar` & `astro-drpy-0.0.1.6.tar`

### file list

```diff
@@ -1,535 +1,535 @@
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-04 17:02:28.366966 astro-drpy-0.0.1.5/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    35149 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/LICENSE
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1243 2023-04-04 17:02:28.362966 astro-drpy-0.0.1.5/PKG-INFO
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      666 2023-02-06 04:59:52.000000 astro-drpy-0.0.1.5/README.md
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1082 2023-02-08 17:46:37.000000 astro-drpy-0.0.1.5/pyproject.toml
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      106 2023-04-04 16:27:59.000000 astro-drpy-0.0.1.5/requirements.txt
--rw-rw-r--   0 zrn       (1007) zrn       (1007)       38 2023-04-04 17:02:28.366966 astro-drpy-0.0.1.5/setup.cfg
--rw-rw-r--   0 zrn       (1007) zrn       (1007)       37 2022-12-01 18:47:37.000000 astro-drpy-0.0.1.5/setup.py
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-04 17:02:27.186921 astro-drpy-0.0.1.5/src/
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-04 17:02:27.206922 astro-drpy-0.0.1.5/src/astro_drpy.egg-info/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1243 2023-04-04 17:02:27.000000 astro-drpy-0.0.1.5/src/astro_drpy.egg-info/PKG-INFO
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    25421 2023-04-04 17:02:27.000000 astro-drpy-0.0.1.5/src/astro_drpy.egg-info/SOURCES.txt
--rw-rw-r--   0 zrn       (1007) zrn       (1007)        1 2023-04-04 17:02:27.000000 astro-drpy-0.0.1.5/src/astro_drpy.egg-info/dependency_links.txt
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      107 2023-04-04 17:02:27.000000 astro-drpy-0.0.1.5/src/astro_drpy.egg-info/requires.txt
--rw-rw-r--   0 zrn       (1007) zrn       (1007)        5 2023-04-04 17:02:27.000000 astro-drpy-0.0.1.5/src/astro_drpy.egg-info/top_level.txt
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-04 17:02:27.214922 astro-drpy-0.0.1.5/src/drpy/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      969 2023-04-04 15:24:40.000000 astro-drpy-0.0.1.5/src/drpy/__init__.py
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-04 17:02:27.234923 astro-drpy-0.0.1.5/src/drpy/batch/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      108 2023-02-05 14:09:14.000000 astro-drpy-0.0.1.5/src/drpy/batch/__init__.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    12653 2023-02-05 14:09:37.000000 astro-drpy-0.0.1.5/src/drpy/batch/core.py
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-04 17:02:27.254923 astro-drpy-0.0.1.5/src/drpy/image/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      109 2023-02-05 14:09:48.000000 astro-drpy-0.0.1.5/src/drpy/image/__init__.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2857 2023-02-05 14:10:09.000000 astro-drpy-0.0.1.5/src/drpy/image/core.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     8804 2023-02-05 14:11:20.000000 astro-drpy-0.0.1.5/src/drpy/image/utils.py
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-04 17:02:27.262924 astro-drpy-0.0.1.5/src/drpy/modeling/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      175 2023-02-05 14:11:42.000000 astro-drpy-0.0.1.5/src/drpy/modeling/__init__.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    16057 2023-02-05 14:11:54.000000 astro-drpy-0.0.1.5/src/drpy/modeling/core.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1165 2022-11-29 12:56:55.000000 astro-drpy-0.0.1.5/src/drpy/modeling/function.py
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-04 17:02:27.270924 astro-drpy-0.0.1.5/src/drpy/onedspec/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      380 2023-02-05 14:12:22.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/__init__.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     8887 2023-02-05 14:12:32.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/center.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    24261 2023-03-06 07:55:21.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/core.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     8555 2023-02-08 17:48:04.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/io.py
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-04 17:02:27.186921 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-04 17:02:27.274924 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/extinction/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      191 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/extinction/baoextinct.dat
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-04 17:02:27.294925 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    13707 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/README
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-04 17:02:27.390929 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/blackbody/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2778 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/blackbody/b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1918 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/blackbody/h.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2653 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/blackbody/i.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1917 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/blackbody/j.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2286 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/blackbody/k.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     5237 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/blackbody/l.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     5242 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/blackbody/lprime.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3762 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/blackbody/m.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      602 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/blackbody/mkbbcal.cl
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      598 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/blackbody/mkbbdat.cl
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     8770 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/blackbody/params.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2653 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/blackbody/r.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      224 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/blackbody/standards.men
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2639 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/blackbody/u.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2778 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/blackbody/v.dat
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-04 17:02:27.502933 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/bstdscal/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      468 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/bstdscal/hr3454.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      468 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/bstdscal/hr3982.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      472 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/bstdscal/hr4468.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      472 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/bstdscal/hr4534.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      468 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/bstdscal/hr5191.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      470 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/bstdscal/hr5511.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      479 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/bstdscal/hr7001.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      467 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/bstdscal/hr718.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      470 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/bstdscal/hr7596.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      470 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/bstdscal/hr7950.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      468 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/bstdscal/hr8634.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      470 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/bstdscal/hr9087.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      177 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/bstdscal/names.men
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      265 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/bstdscal/standards.men
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-04 17:02:27.618937 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctio/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      248 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctio/multi1m.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      680 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctio/multi4m.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      168 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctio/multi4mech.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    14757 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctio/nd1m.100mag.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    14745 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctio/nd1m.125mag.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    15440 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctio/nd1m.250mag.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    14502 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctio/nd1m.500mag.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     4484 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctio/nd4m.l000mag.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     4495 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctio/nd4m.l250mag.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     5212 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctio/nd4m.rc500mag.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     4498 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u000mag.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     4506 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u025mag.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     4501 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u075mag.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     4502 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u150mag.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     4507 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u225mag.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      607 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctio/ndfilters.men
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-04 17:02:27.830946 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      466 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/bd25.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      465 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/bd8.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      706 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/cd32.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      708 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/eg21.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      705 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/eg274.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      469 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/f110.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      464 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/f15.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      467 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/f25.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      469 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/f56.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      468 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/f98.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      652 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/g9937.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      469 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/h600.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      468 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/hz15.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      543 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/hz2.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      544 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/hz4.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      468 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/kopf27.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      711 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l1020.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      673 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l1788.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      705 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l2415.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      551 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l2511.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      662 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l3218.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      712 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l377.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      711 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l3864.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      708 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l4364.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      595 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l4816.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      709 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l6248.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      696 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l7379.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      648 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l74546.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      693 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l7987.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      580 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l8702.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      709 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l9239.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      906 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l93080.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      592 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l9491.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      717 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l97030.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      870 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/lds235.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      497 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/lds749.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      387 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/names.men
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      719 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/ross627.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      932 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/standards.men
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      194 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/w1346.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      995 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/w485a.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      445 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctioextinct.dat
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-04 17:02:27.950950 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2092 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/cd32.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1298 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/cd32blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1258 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/cd32red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2028 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/eg21.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1298 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/eg21blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1209 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/eg21red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2078 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/eg274.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1299 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/eg274blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1258 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/eg274red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2011 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/f110.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1302 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/f110blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1182 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/f110red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2065 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/f56.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/f56blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1124 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/f56red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2066 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/h600.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/h600blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1127 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/h600red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2066 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l1020.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l1020blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1244 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l1020red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2059 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l1788.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l1788blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1229 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l1788red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2046 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l2415.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l2415blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1213 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l2415red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2018 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l3218.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l3218blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1076 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l3218red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2123 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l377.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1300 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l377blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1292 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l377red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2066 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l3864.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l3864blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1124 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l3864red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2092 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l4364.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l4364blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1156 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l4364red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2012 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l4816.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l4816blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1076 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l4816red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2080 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l6248.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l6248blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1245 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l6248red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2038 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l7379.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1286 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l7379blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1207 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l7379red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1108 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l745.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1108 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l745red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2032 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l7987.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l7987blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1197 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l7987red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2093 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l9239.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l9239blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1261 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l9239red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2014 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l9491.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l9491blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1181 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l9491red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1016 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/standards.men
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-04 17:02:28.070955 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1167 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/aaareadme.hst
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   244272 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fagk81d266.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   245040 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fbd28d4211.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   249264 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fbd33d2642.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   245040 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fbd75d325.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   125712 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fbpm16274.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   244992 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/ffeige110.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   245040 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/ffeige34.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   244368 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fg191b2b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   248640 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fg93_48.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   249120 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fgd108.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   248784 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fgd50.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   248160 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fgrw70d5824.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   104112 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fhd49798.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   126960 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fhd60753.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   244944 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fhd93521.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   114000 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fhr153.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   102480 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fhr1996.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   125472 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fhr4554.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   104016 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fhr5191.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   123696 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fhr7001.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   248160 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fhz2.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   248448 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fhz21.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   246000 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fhz4.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   245040 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fhz44.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   246912 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/flb227.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   246960 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/flds749b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   245040 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fngc7293.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   106869 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/magk81d266.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   107205 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mbd28d4211.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   109053 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mbd33d2642.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   107205 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mbd75d325.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    54999 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mbpm16274.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   107184 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mfeige110.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   107205 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mfeige34.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   106911 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mg191b2b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   108780 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mg93_48.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   108990 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mgd108.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   108843 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mgd50.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   108570 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mgrw70d5824.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    45549 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mhd49798.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    55545 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mhd60753.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   107163 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mhd93521.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    49875 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mhr153.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    44835 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mhr1996.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    54894 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mhr4554.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    45507 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mhr5191.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    54117 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mhr7001.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   108570 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mhz2.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   108696 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mhz21.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   107625 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mhz4.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   107205 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mhz44.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   108024 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mlb227.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   108045 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mlds749b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   107205 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mngc7293.dat
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-04 17:02:28.090955 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      430 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/40erib.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      472 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/bd253941.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      464 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/bd284211.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      473 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/bd332642.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      471 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/bd404032.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      471 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/bd82015.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      474 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/feige110.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      469 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/feige15.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      447 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/feige24.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      472 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/feige25.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      474 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/feige34.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      474 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/feige56.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      474 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/feige92.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      473 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/feige98.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      449 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/g191b2b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      451 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/g4718.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      451 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/g9937.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      498 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/gd140.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      499 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/gd190.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      503 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/grw705824.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      452 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/grw708247.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      455 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/grw738031.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      447 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/he3.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      472 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/hiltner102.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      476 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/hiltner600.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      414 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/hz14.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      469 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/hz15.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      430 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/hz2.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      447 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/hz29.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      427 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/hz4.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      446 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/hz43.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      448 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/hz44.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      431 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/hz7.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      470 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/kopff27.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      449 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/l13633.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      506 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/l151234b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      453 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/l74546a.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      432 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/l8702.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      452 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/l93080.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      500 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/l97030.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      433 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/lb1240.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      430 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/lb227.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      453 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/lds235b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      502 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/lds749b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      839 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/names.men
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      495 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/ross627.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      448 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/ross640.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      503 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/sa29130.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1336 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/standards.men
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      434 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/ton573.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      500 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/wolf1346.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      450 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/wolf485a.dat
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-04 17:02:28.098956 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1250 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/bd082015.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1254 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/bd174708.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1244 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/bd253941.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1193 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/bd262606.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1239 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/bd284211.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1254 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/bd332642.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1253 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/bd404032.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1251 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/feige110.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1297 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/feige15.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1297 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/feige25.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1252 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/feige34.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/feige56.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1298 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/feige92.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1300 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/feige98.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1247 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/g191b2b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1249 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/hd109995.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1251 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/hd117880.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1247 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/hd161817.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1177 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/hd17520.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1172 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/hd192281.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1173 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/hd19445.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1162 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/hd217086.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1258 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/hd2857.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1257 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/hd60778.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1249 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/hd74721.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1176 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/hd84937.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1249 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/hd86986.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1248 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/he3.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1232 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/hiltner102.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1255 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/hiltner600.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1271 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/hr7001.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1250 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/hz44.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1294 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/kopff27.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      137 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/names.men
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      523 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/standards.men
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1250 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/wolf1346.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1062 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/kpnoextinct.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      950 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/names.men
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-04 17:02:28.106956 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/oke1990/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1105 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/oke1990/bd284211.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1083 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/oke1990/bd75325.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1132 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/oke1990/feige110.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1131 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/oke1990/feige34.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1131 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/oke1990/feige67.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1130 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/oke1990/g13831.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1130 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/oke1990/g191b2b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1134 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/oke1990/g19374.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1128 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/oke1990/g249.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1129 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/oke1990/gd108.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1129 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/oke1990/gd248.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1128 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/oke1990/hz21.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1131 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/oke1990/ltt9491.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      111 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/oke1990/names.men
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      188 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/oke1990/standards.men
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-04 17:02:28.298963 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      681 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/aaareadme.oke
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fbd25d4655.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fbd28d4211.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fbd33d2642.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fbd75d325.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/ffeige110.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/ffeige34.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/ffeige66.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/ffeige67.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fg138_31.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fg158_100.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fg191b2b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fg193_74.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fg24_9.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fg60_54.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fgd108.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fgd248.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fgd50.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fgrw70d5824.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fhd93521.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fhz21.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fhz4.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fhz44.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fltt9491.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fngc7293.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fsa95_42.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mbd25d4655.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mbd28d4211.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mbd33d2642.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mbd75d325.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mfeige110.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mfeige34.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mfeige66.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mfeige67.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mg138_31.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mg158_100.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mg191b2b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mg193_74.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mg24_9.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mg60_54.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mgd108.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mgd248.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mgd50.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mgrw70d5824.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mhd93521.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mhz21.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mhz4.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mhz44.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mltt9491.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mngc7293.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/msa95_42.dat
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-04 17:02:28.306964 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      685 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/40erib.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1454 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/bd174708.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1393 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/bd262606.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      756 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/feige24.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1574 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/g191b2b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      728 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/g4718.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      724 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/g9937.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      811 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/gd140.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      682 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/gd190.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      782 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/grw705824.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      713 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/grw708247.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      763 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/grw738031.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1373 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/hd19445.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1376 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/hd84937.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1557 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/he3.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      612 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/hz29.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      773 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/hz43.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1577 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/hz44.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      776 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/l13633.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      768 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/l151234b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      780 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/l74546a.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      639 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/l93080.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      738 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/l97030.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      606 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/lds235b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      781 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/lds749b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      631 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/names.men
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      917 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/ross627.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      775 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/ross640.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      781 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/sa29130.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      774 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/standards.men
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1807 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/wolf1346.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      705 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/wolf485a.dat
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-04 17:02:28.318964 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     6283 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr1544.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr1544blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3916 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr1544red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     6180 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr3454.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr3454blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3476 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr3454red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     6149 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr4468.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr4468blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3446 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr4468red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     6249 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr4963.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr4963blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3844 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr4963red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     6234 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr5501.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr5501blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3843 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr5501red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     6261 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr718.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3747 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr718blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3886 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr718red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     6265 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr7596.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr7596blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3887 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr7596red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     6250 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr7950.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr7950blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3872 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr7950red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     6259 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr8634.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr8634blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3887 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr8634red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     6238 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr9087.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr9087blue.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3872 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr9087red.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      677 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/names.men
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      988 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/standards.men
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-04 17:02:28.322964 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2534 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/bd284211.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/cygob2no9.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2284 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/eg81.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2534 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/feige110.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2533 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/feige34.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2533 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/feige66.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2533 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/feige67.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2533 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/g191b2b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2531 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/gd140.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2288 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/hd192281.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2288 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/hd217086.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2536 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/hilt600.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2284 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/hz14.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2530 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/hz44.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      152 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/names.men
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/pg0205134.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/pg0216032.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/pg0310149.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2535 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/pg0823546.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/pg0846249.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/pg0934554.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/pg0939262.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/pg1121145.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/pg1545035.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2220 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/pg1708602.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      627 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/standards.men
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     2534 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/wolf1346.dat
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-04 17:02:28.346965 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      664 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/bd284211.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/cygob2no9.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      660 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/eg81.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      664 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/feige110.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      663 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/feige34.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      663 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/feige66.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      663 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/feige67.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      663 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/g191b2b.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      661 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/gd140.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      664 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/hd192281.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      664 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/hd217086.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      666 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/hiltner600.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      660 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/hz14.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      660 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/hz44.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      138 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/names.men
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/pg0205134.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/pg0216032.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/pg0310149.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/pg0823546.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      617 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/pg0846249.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/pg0934554.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/pg0939262.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/pg1121145.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/pg1545035.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      641 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/pg1708602.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      416 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/standards.men
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      664 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/wolf1346.dat
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     9478 2023-04-04 16:27:50.000000 astro-drpy-0.0.1.5/src/drpy/plotting.py
-drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-04 17:02:28.358966 astro-drpy-0.0.1.5/src/drpy/twodspec/
--rw-rw-r--   0 zrn       (1007) zrn       (1007)      353 2023-02-05 14:13:11.000000 astro-drpy-0.0.1.5/src/drpy/twodspec/__init__.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    66729 2023-04-04 17:01:54.000000 astro-drpy-0.0.1.5/src/drpy/twodspec/longslit.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     3268 2023-02-21 15:22:01.000000 astro-drpy-0.0.1.5/src/drpy/twodspec/utils.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)     1704 2022-11-30 07:57:09.000000 astro-drpy-0.0.1.5/src/drpy/utils.py
--rw-rw-r--   0 zrn       (1007) zrn       (1007)    13583 2023-02-05 14:08:08.000000 astro-drpy-0.0.1.5/src/drpy/validate.py
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:09.504351 astro-drpy-0.0.1.6/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    35149 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/LICENSE
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1243 2023-04-13 06:39:09.504351 astro-drpy-0.0.1.6/PKG-INFO
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      666 2023-02-06 04:59:52.000000 astro-drpy-0.0.1.6/README.md
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1082 2023-02-08 17:46:37.000000 astro-drpy-0.0.1.6/pyproject.toml
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      106 2023-04-04 16:27:59.000000 astro-drpy-0.0.1.6/requirements.txt
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)       38 2023-04-13 06:39:09.504351 astro-drpy-0.0.1.6/setup.cfg
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)       37 2022-12-01 18:47:37.000000 astro-drpy-0.0.1.6/setup.py
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:07.772295 astro-drpy-0.0.1.6/src/
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:07.796296 astro-drpy-0.0.1.6/src/astro_drpy.egg-info/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1243 2023-04-13 06:39:07.000000 astro-drpy-0.0.1.6/src/astro_drpy.egg-info/PKG-INFO
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    25421 2023-04-13 06:39:07.000000 astro-drpy-0.0.1.6/src/astro_drpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)        1 2023-04-13 06:39:07.000000 astro-drpy-0.0.1.6/src/astro_drpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      107 2023-04-13 06:39:07.000000 astro-drpy-0.0.1.6/src/astro_drpy.egg-info/requires.txt
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)        5 2023-04-13 06:39:07.000000 astro-drpy-0.0.1.6/src/astro_drpy.egg-info/top_level.txt
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:07.804296 astro-drpy-0.0.1.6/src/drpy/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1080 2023-04-10 12:06:57.000000 astro-drpy-0.0.1.6/src/drpy/__init__.py
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:07.812296 astro-drpy-0.0.1.6/src/drpy/batch/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      108 2023-02-05 14:09:14.000000 astro-drpy-0.0.1.6/src/drpy/batch/__init__.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    18108 2023-04-09 09:14:51.000000 astro-drpy-0.0.1.6/src/drpy/batch/core.py
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:07.840297 astro-drpy-0.0.1.6/src/drpy/image/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      109 2023-02-05 14:09:48.000000 astro-drpy-0.0.1.6/src/drpy/image/__init__.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2624 2023-04-08 16:02:07.000000 astro-drpy-0.0.1.6/src/drpy/image/core.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     9178 2023-04-10 16:29:40.000000 astro-drpy-0.0.1.6/src/drpy/image/utils.py
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:07.868298 astro-drpy-0.0.1.6/src/drpy/modeling/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      175 2023-02-05 14:11:42.000000 astro-drpy-0.0.1.6/src/drpy/modeling/__init__.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    16057 2023-04-10 05:38:40.000000 astro-drpy-0.0.1.6/src/drpy/modeling/core.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1165 2022-11-29 12:56:55.000000 astro-drpy-0.0.1.6/src/drpy/modeling/function.py
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:07.884298 astro-drpy-0.0.1.6/src/drpy/onedspec/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      380 2023-02-05 14:12:22.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/__init__.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     8887 2023-02-05 14:12:32.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/center.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    24324 2023-04-10 14:57:51.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/core.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     8555 2023-02-08 17:48:04.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/io.py
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:07.772295 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:07.888298 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/extinction/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      191 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/extinction/baoextinct.dat
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:07.908299 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    13707 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/README
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:08.004302 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2778 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1918 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/h.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2653 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/i.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1917 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/j.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2286 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/k.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     5237 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/l.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     5242 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/lprime.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3762 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/m.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      602 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/mkbbcal.cl
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      598 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/mkbbdat.cl
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     8770 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/params.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2653 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/r.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      224 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/standards.men
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2639 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/u.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2778 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/v.dat
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:08.116306 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/bstdscal/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      468 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/bstdscal/hr3454.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      468 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/bstdscal/hr3982.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      472 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/bstdscal/hr4468.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      472 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/bstdscal/hr4534.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      468 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/bstdscal/hr5191.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      470 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/bstdscal/hr5511.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      479 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/bstdscal/hr7001.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      467 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/bstdscal/hr718.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      470 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/bstdscal/hr7596.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      470 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/bstdscal/hr7950.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      468 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/bstdscal/hr8634.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      470 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/bstdscal/hr9087.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      177 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/bstdscal/names.men
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      265 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/bstdscal/standards.men
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:08.232310 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      248 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/multi1m.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      680 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/multi4m.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      168 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/multi4mech.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    14757 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd1m.100mag.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    14745 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd1m.125mag.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    15440 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd1m.250mag.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    14502 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd1m.500mag.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     4484 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd4m.l000mag.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     4495 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd4m.l250mag.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     5212 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd4m.rc500mag.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     4498 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u000mag.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     4506 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u025mag.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     4501 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u075mag.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     4502 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u150mag.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     4507 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u225mag.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      607 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/ndfilters.men
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:08.572321 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      466 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/bd25.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      465 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/bd8.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      706 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/cd32.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      708 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/eg21.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      705 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/eg274.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      469 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/f110.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      464 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/f15.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      467 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/f25.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      469 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/f56.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      468 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/f98.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      652 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/g9937.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      469 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/h600.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      468 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/hz15.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      543 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/hz2.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      544 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/hz4.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      468 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/kopf27.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      711 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l1020.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      673 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l1788.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      705 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l2415.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      551 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l2511.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      662 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l3218.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      712 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l377.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      711 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l3864.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      708 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l4364.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      595 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l4816.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      709 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l6248.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      696 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l7379.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      648 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l74546.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      693 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l7987.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      580 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l8702.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      709 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l9239.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      906 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l93080.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      592 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l9491.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      717 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l97030.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      870 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/lds235.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      497 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/lds749.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      387 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/names.men
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      719 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/ross627.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      932 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/standards.men
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      194 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/w1346.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      995 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/w485a.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      445 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctioextinct.dat
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:09.064337 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2092 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/cd32.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1298 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/cd32blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1258 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/cd32red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2028 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/eg21.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1298 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/eg21blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1209 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/eg21red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2078 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/eg274.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1299 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/eg274blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1258 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/eg274red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2011 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/f110.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1302 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/f110blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1182 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/f110red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2065 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/f56.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/f56blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1124 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/f56red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2066 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/h600.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/h600blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1127 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/h600red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2066 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l1020.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l1020blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1244 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l1020red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2059 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l1788.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l1788blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1229 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l1788red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2046 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l2415.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l2415blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1213 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l2415red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2018 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l3218.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l3218blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1076 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l3218red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2123 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l377.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1300 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l377blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1292 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l377red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2066 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l3864.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l3864blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1124 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l3864red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2092 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l4364.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l4364blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1156 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l4364red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2012 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l4816.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l4816blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1076 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l4816red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2080 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l6248.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l6248blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1245 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l6248red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2038 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l7379.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1286 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l7379blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1207 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l7379red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1108 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l745.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1108 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l745red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2032 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l7987.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l7987blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1197 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l7987red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2093 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l9239.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l9239blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1261 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l9239red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2014 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l9491.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l9491blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1181 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l9491red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1016 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/standards.men
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:09.236343 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1167 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/aaareadme.hst
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   244272 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fagk81d266.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   245040 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fbd28d4211.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   249264 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fbd33d2642.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   245040 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fbd75d325.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   125712 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fbpm16274.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   244992 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/ffeige110.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   245040 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/ffeige34.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   244368 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fg191b2b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   248640 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fg93_48.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   249120 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fgd108.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   248784 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fgd50.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   248160 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fgrw70d5824.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   104112 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhd49798.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   126960 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhd60753.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   244944 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhd93521.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   114000 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhr153.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   102480 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhr1996.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   125472 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhr4554.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   104016 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhr5191.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   123696 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhr7001.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   248160 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhz2.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   248448 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhz21.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   246000 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhz4.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   245040 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhz44.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   246912 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/flb227.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   246960 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/flds749b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   245040 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fngc7293.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   106869 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/magk81d266.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   107205 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mbd28d4211.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   109053 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mbd33d2642.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   107205 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mbd75d325.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    54999 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mbpm16274.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   107184 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mfeige110.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   107205 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mfeige34.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   106911 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mg191b2b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   108780 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mg93_48.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   108990 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mgd108.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   108843 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mgd50.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   108570 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mgrw70d5824.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    45549 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhd49798.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    55545 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhd60753.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   107163 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhd93521.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    49875 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhr153.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    44835 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhr1996.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    54894 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhr4554.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    45507 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhr5191.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    54117 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhr7001.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   108570 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhz2.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   108696 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhz21.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   107625 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhz4.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   107205 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhz44.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   108024 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mlb227.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   108045 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mlds749b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   107205 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mngc7293.dat
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:09.272344 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      430 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/40erib.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      472 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/bd253941.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      464 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/bd284211.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      473 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/bd332642.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      471 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/bd404032.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      471 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/bd82015.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      474 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/feige110.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      469 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/feige15.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      447 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/feige24.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      472 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/feige25.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      474 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/feige34.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      474 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/feige56.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      474 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/feige92.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      473 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/feige98.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      449 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/g191b2b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      451 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/g4718.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      451 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/g9937.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      498 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/gd140.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      499 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/gd190.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      503 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/grw705824.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      452 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/grw708247.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      455 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/grw738031.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      447 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/he3.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      472 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/hiltner102.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      476 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/hiltner600.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      414 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/hz14.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      469 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/hz15.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      430 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/hz2.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      447 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/hz29.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      427 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/hz4.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      446 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/hz43.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      448 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/hz44.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      431 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/hz7.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      470 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/kopff27.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      449 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/l13633.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      506 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/l151234b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      453 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/l74546a.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      432 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/l8702.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      452 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/l93080.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      500 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/l97030.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      433 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/lb1240.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      430 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/lb227.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      453 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/lds235b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      502 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/lds749b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      839 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/names.men
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      495 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/ross627.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      448 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/ross640.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      503 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/sa29130.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1336 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/standards.men
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      434 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/ton573.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      500 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/wolf1346.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      450 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/wolf485a.dat
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:09.284344 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1250 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/bd082015.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1254 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/bd174708.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1244 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/bd253941.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1193 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/bd262606.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1239 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/bd284211.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1254 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/bd332642.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1253 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/bd404032.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1251 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/feige110.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1297 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/feige15.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1297 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/feige25.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1252 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/feige34.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1301 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/feige56.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1298 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/feige92.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1300 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/feige98.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1247 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/g191b2b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1249 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd109995.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1251 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd117880.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1247 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd161817.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1177 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd17520.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1172 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd192281.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1173 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd19445.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1162 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd217086.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1258 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd2857.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1257 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd60778.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1249 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd74721.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1176 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd84937.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1249 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd86986.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1248 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/he3.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1232 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hiltner102.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1255 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hiltner600.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1271 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hr7001.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1250 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hz44.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1294 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/kopff27.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      137 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/names.men
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      523 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/standards.men
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1250 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/wolf1346.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1062 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/kpnoextinct.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      950 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/names.men
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:09.288344 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1105 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/bd284211.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1083 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/bd75325.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1132 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/feige110.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1131 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/feige34.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1131 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/feige67.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1130 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/g13831.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1130 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/g191b2b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1134 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/g19374.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1128 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/g249.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1129 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/gd108.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1129 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/gd248.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1128 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/hz21.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1131 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/ltt9491.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      111 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/names.men
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      188 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/standards.men
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:09.436349 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      681 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/aaareadme.oke
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fbd25d4655.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fbd28d4211.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fbd33d2642.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fbd75d325.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/ffeige110.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/ffeige34.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/ffeige66.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/ffeige67.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fg138_31.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fg158_100.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fg191b2b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fg193_74.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fg24_9.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fg60_54.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fgd108.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fgd248.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fgd50.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fgrw70d5824.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fhd93521.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fhz21.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fhz4.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fhz44.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fltt9491.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fngc7293.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   240064 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fsa95_42.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mbd25d4655.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mbd28d4211.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mbd33d2642.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mbd75d325.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mfeige110.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mfeige34.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mfeige66.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mfeige67.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mg138_31.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mg158_100.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mg191b2b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mg193_74.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mg24_9.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mg60_54.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mgd108.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mgd248.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mgd50.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mgrw70d5824.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mhd93521.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mhz21.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mhz4.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mhz44.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mltt9491.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mngc7293.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)   116281 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/msa95_42.dat
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:09.444349 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      685 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/40erib.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1454 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/bd174708.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1393 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/bd262606.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      756 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/feige24.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1574 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/g191b2b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      728 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/g4718.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      724 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/g9937.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      811 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/gd140.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      682 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/gd190.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      782 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/grw705824.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      713 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/grw708247.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      763 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/grw738031.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1373 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/hd19445.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1376 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/hd84937.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1557 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/he3.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      612 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/hz29.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      773 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/hz43.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1577 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/hz44.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      776 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/l13633.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      768 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/l151234b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      780 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/l74546a.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      639 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/l93080.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      738 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/l97030.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      606 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/lds235b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      781 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/lds749b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      631 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/names.men
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      917 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/ross627.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      775 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/ross640.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      781 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/sa29130.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      774 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/standards.men
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1807 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/wolf1346.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      705 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/wolf485a.dat
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:09.456350 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     6283 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr1544.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr1544blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3916 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr1544red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     6180 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr3454.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr3454blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3476 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr3454red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     6149 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr4468.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr4468blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3446 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr4468red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     6249 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr4963.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr4963blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3844 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr4963red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     6234 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr5501.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr5501blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3843 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr5501red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     6261 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr718.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3747 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr718blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3886 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr718red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     6265 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr7596.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr7596blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3887 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr7596red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     6250 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr7950.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr7950blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3872 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr7950red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     6259 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr8634.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr8634blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3887 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr8634red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     6238 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr9087.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3748 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr9087blue.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3872 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr9087red.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      677 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/names.men
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      988 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/standards.men
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:09.464350 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2534 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/bd284211.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/cygob2no9.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2284 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/eg81.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2534 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/feige110.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2533 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/feige34.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2533 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/feige66.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2533 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/feige67.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2533 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/g191b2b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2531 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/gd140.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2288 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/hd192281.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2288 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/hd217086.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2536 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/hilt600.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2284 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/hz14.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2530 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/hz44.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      152 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/names.men
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg0205134.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg0216032.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg0310149.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2535 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg0823546.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg0846249.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg0934554.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg0939262.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg1121145.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2289 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg1545035.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2220 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg1708602.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      627 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/standards.men
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     2534 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/wolf1346.dat
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:09.488351 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      664 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/bd284211.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/cygob2no9.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      660 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/eg81.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      664 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/feige110.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      663 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/feige34.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      663 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/feige66.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      663 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/feige67.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      663 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/g191b2b.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      661 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/gd140.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      664 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/hd192281.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      664 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/hd217086.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      666 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/hiltner600.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      660 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/hz14.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      660 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/hz44.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      138 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/names.men
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg0205134.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg0216032.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg0310149.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg0823546.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      617 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg0846249.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg0934554.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg0939262.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg1121145.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      665 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg1545035.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      641 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg1708602.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      416 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/standards.men
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      664 2022-11-28 15:01:10.000000 astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/wolf1346.dat
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    10234 2023-04-13 06:32:54.000000 astro-drpy-0.0.1.6/src/drpy/plotting.py
+drwxrwxr-x   0 zrn       (1007) zrn       (1007)        0 2023-04-13 06:39:09.496351 astro-drpy-0.0.1.6/src/drpy/twodspec/
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)      353 2023-02-05 14:13:11.000000 astro-drpy-0.0.1.6/src/drpy/twodspec/__init__.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    70816 2023-04-13 06:36:02.000000 astro-drpy-0.0.1.6/src/drpy/twodspec/longslit.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     3268 2023-02-21 15:22:01.000000 astro-drpy-0.0.1.6/src/drpy/twodspec/utils.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)     1704 2022-11-30 07:57:09.000000 astro-drpy-0.0.1.6/src/drpy/utils.py
+-rw-rw-r--   0 zrn       (1007) zrn       (1007)    13466 2023-04-11 14:42:08.000000 astro-drpy-0.0.1.6/src/drpy/validate.py
```

### Comparing `astro-drpy-0.0.1.5/LICENSE` & `astro-drpy-0.0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/PKG-INFO` & `astro-drpy-0.0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-drpy
-Version: 0.0.1.5
+Version: 0.0.1.6
 Summary: A data reduction toolkit for astronomical photometry and spectroscopy.
 Author-email: Ruining ZHAO <ruiningzhao@mail.bnu.edu.cn>
 Project-URL: Homepage, https://github.com/RuiningZHAO/drpy
 Project-URL: Tracker, https://github.com/RuiningZHAO/drpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `astro-drpy-0.0.1.5/README.md` & `astro-drpy-0.0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/pyproject.toml` & `astro-drpy-0.0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/astro_drpy.egg-info/PKG-INFO` & `astro-drpy-0.0.1.6/src/astro_drpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-drpy
-Version: 0.0.1.5
+Version: 0.0.1.6
 Summary: A data reduction toolkit for astronomical photometry and spectroscopy.
 Author-email: Ruining ZHAO <ruiningzhao@mail.bnu.edu.cn>
 Project-URL: Homepage, https://github.com/RuiningZHAO/drpy
 Project-URL: Tracker, https://github.com/RuiningZHAO/drpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `astro-drpy-0.0.1.5/src/astro_drpy.egg-info/SOURCES.txt` & `astro-drpy-0.0.1.6/src/astro_drpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/image/core.py` & `astro-drpy-0.0.1.6/src/drpy/image/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 import warnings
 from copy import deepcopy
 
 # AstroPy
 from astropy.time import Time
+# ccdproc
+from ccdproc.utils.slices import slice_from_string
 # drpy
 from drpy.validate import _validate1DArray, _validateCCDList
 
 __all__ = ['concatenate']
 
 
-def concatenate(ccdlist, row_range, col_range, scale=None):
+def concatenate(ccdlist, fits_section, scale=None):
     """Concatenate two frames.
 
-    The region defined by ``row_range`` and ``col_range`` in the second frame is 
-    replaced by that in the first frame. Usually this is used to concatenate 
-    flat-fields or arc spectra of different exposure times. To concatenate multiple 
-    frames, call this function repeatedly.
+    The region defined by ``fits_section`` of the second frame is replaced by that in 
+    the first frame. Usually this is used to concatenate flat-fields or arc spectra of 
+    different exposure times. To concatenate multiple frames, call this function 
+    repeatedly.
 
     Parameters
     ----------
     ccdlist : Iterable
         Iterable object containing two 2-dimensional frames.
 
-    row_range : array_like
-        Row range (python style).
-
-    col_range : array_like
-        Column range (python style).
+    fits_section : str
+        Region of the second frame to be replaced by the counterpart of the first frame.
     
     scale : scalar, array-like or `None`, optional
         Scaling factor. Frames are multiplied by scaling factor prior to concatenation.
         Default is `None`.
 
     Returns
     -------
@@ -41,45 +40,39 @@
     ccdlist = _validateCCDList(ccdlist, 2, 2)
     n_image = len(ccdlist)
     if n_image > 2:
         warnings.warn(
             '``ccdlist`` contains more than two frames. Extra frames will be ignored.', 
             RuntimeWarning)
 
-    row_start, row_end = row_range
-    col_start, col_end = col_range
+    python_slice = slice_from_string(fits_section, fits_convention=True)
 
     if scale is None:
         scale = _validate1DArray(1, 'scale', 2, True)
 
     else:
         scale = _validate1DArray(scale, 'scale', 2, True)
 
     data_arr = ccdlist[1].data * scale[1]
-    data_arr[row_start:row_end, col_start:col_end] = (
-        ccdlist[0].data[row_start:row_end, col_start:col_end] * scale[0]
-    )
+    data_arr[python_slice] = ccdlist[0].data[python_slice] * scale[0]
 
     if (ccdlist[0].uncertainty is None) | (ccdlist[1].uncertainty is None):
         uncertainty_arr = None
 
     else:
         uncertainty_arr = scale[1] * ccdlist[1].uncertainty.array
-        uncertainty_arr[row_start:row_end, col_start:col_end] = (
-            ccdlist[0].uncertainty.array[row_start:row_end, col_start:col_end] 
-            * scale[0]
-        )
+        uncertainty_arr[python_slice] = (
+            ccdlist[0].uncertainty.array[python_slice] * scale[0])
 
     if (ccdlist[0].mask is None) | (ccdlist[1].mask is None):
         mask_arr = None
 
     else:
         mask_arr = deepcopy(ccdlist[1].mask)
-        mask_arr[row_start:row_end, col_start:col_end] = (
-            ccdlist[0].mask[row_start:row_end, col_start:col_end])
+        mask_arr[python_slice] = ccdlist[0].mask[python_slice]
 
     nccd = ccdlist[0].copy()
 
     nccd.data = data_arr
 
     if uncertainty_arr is None:
         nccd.uncertainty = None
@@ -87,13 +80,12 @@
     else:
         # Here ``nccd.uncertainty`` is definitely not `None`.
         nccd.uncertainty.array = uncertainty_arr
 
     nccd.mask = mask_arr
 
     nccd.header['CONCATEN'] = (
-        '{} Data section [{}:{}, {}:{}] is from the first frame.'.format(
-            Time.now().to_value('iso', subfmt='date_hm'), (col_start + 1), col_end, 
-            (row_start + 1), row_end)
+        '{} Data section {} is from the first frame.'.format(
+            Time.now().to_value('iso', subfmt='date_hm'), fits_section)
     )
 
     return nccd
```

### Comparing `astro-drpy-0.0.1.5/src/drpy/image/utils.py` & `astro-drpy-0.0.1.6/src/drpy/image/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,19 +17,26 @@
 # drpy
 from drpy import conf
 from drpy.modeling.function import CircularGaussian
 from drpy.plotting import _plot2d
 from drpy.validate import (_validateString, _validateBool, _validateRange, 
                            _validateInteger, _validateCCD, _validatePath)
 
+# Set plot parameters
+plt.rcParams['figure.figsize'] = [conf.fig_width, conf.fig_width]
+plt.rcParams['axes.linewidth'] = 1.5
+plt.rcParams['mathtext.fontset'] = 'stix'
+plt.rcParams['font.family'] = 'STIXGeneral'
+
 __all__ = ['getFWHM']
 
 # todo: deal with NaNs in Gaussian fitting.
 def getFWHM(ccd, box_size, n_sigma, aper_radius, saturation, n_peak, use_mask=False, 
-            title='FWHM', show=conf.show, save=conf.save, path=conf.path, **kwargs):
+            title='FWHM', show=conf.fig_show, save=conf.fig_save, path=conf.fig_path, 
+            **kwargs):
     """Estimate mean FWHM of the sources in the input image.
 
     The background of the input image is first modeled by a 2-dimensional background 
     estimator, and then subtracted from the input image. Detect sources in the 
     background subtracted image. Fit circular Gaussian profiles to the detected 
     sources.
 
@@ -170,30 +177,30 @@
 
             except (RuntimeError, TypeError, OptimizeWarning): # raise exception here
                 pass
 
     # Output
     fwhm, fwhm_err = np.nanmean(fwhm_arr), np.nanstd(fwhm_arr, ddof=1)
 
+    # Plot
     _validateBool(show, 'show')
 
     _validateString(title, 'title')
     if title != 'FWHM':
         title = [f'{title} FWHM (source detection)', 
                  f'{title} FWHM (Gaussian2D fitting)']
     else:
         title = [f'FWHM (source detection)', f'FWHM (Gaussian2D fitting)']
 
     fig_path = _validatePath(save, path, title)
 
     if show | save:
 
-        # Plot source detection
-        fig = plt.figure(dpi=100)
-        ax = fig.add_subplot(1, 1, 1)
+        # Source detection
+        fig, ax = plt.subplots(1, 1, dpi=100)
         # Image
         extent = (
             0.5, data_arr_bkgsb.shape[1] + 0.5, 0.5, data_arr_bkgsb.shape[0] + 0.5
         )
         _plot2d(ax=ax, ccd=data_arr_bkgsb, cmap='Greys_r', extent=extent)
         (xmin, xmax), (ymin, ymax) = ax.get_xlim(), ax.get_ylim()
         # Mask
@@ -204,28 +211,32 @@
         apertures = RectangularAperture(
             positions=np.transpose([x + 1, y + 1]), w=size, h=size, theta=0)
         apertures.plot(ax, color='r', lw=1)
         # Setting
         ax.set_xlim(xmin, xmax)
         ax.set_ylim(ymin, ymax)
         ax.set_title(title[0], fontsize=16)
+        fig.set_figheight(
+            (data_arr_bkgsb.shape[0] / data_arr_bkgsb.shape[1] * fig.get_figwidth()))
+        fig.tight_layout()
 
         if save: plt.savefig(fig_path[0], dpi=100)
 
         if show: plt.show()
 
         plt.close()
 
+        # Cutout
         if (n_peak % 4) == 0:
             nrow = n_peak // 4
         else:
             nrow = n_peak // 4 + 1
+        extent = (0.5, size + 0.5, 0.5, size + 0.5)
 
         fig = plt.figure(figsize=(10, 2 * nrow), dpi=100)
-        extent = (0.5, size + 0.5, 0.5, size + 0.5)
         for i in range(n_peak):
             ax = fig.add_subplot(nrow, 4, i + 1)
             # Image
             _plot2d(
                 ax=ax, ccd=cutout2d_arr[i], cmap='Greys_r', extent=extent, cbar=False, 
                 xlabel=None, ylabel=None)
             # Aperture
```

### Comparing `astro-drpy-0.0.1.5/src/drpy/modeling/core.py` & `astro-drpy-0.0.1.6/src/drpy/modeling/core.py`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/modeling/function.py` & `astro-drpy-0.0.1.6/src/drpy/modeling/function.py`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/center.py` & `astro-drpy-0.0.1.6/src/drpy/onedspec/center.py`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/core.py` & `astro-drpy-0.0.1.6/src/drpy/onedspec/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,16 @@
 from .io import loadSpectrum1D, loadStandardSpectrum, loadExtinctionCurve
 
 __all__ = ['dispcor', 'sensfunc', 'calibrate1d']
 
 
 def dispcor(spectrum1d, reverse, reference, n_piece=3, refit=True, n_iter=5, 
             sigma_lower=None, sigma_upper=None, grow=False, use_mask=False, 
-            title='dispcor', show=conf.show, save=conf.save, path=conf.path):
+            title='dispcor', show=conf.fig_show, save=conf.fig_save, 
+            path=conf.fig_path):
     """Dispersion correction.
 
     Parameters
     ----------
     spectrum1d : `~specutils.Spectrum1D` or `~numpy.ndarray`
         Input spectrum.
 
@@ -175,32 +176,34 @@
 
     fig_path = _validatePath(save, path, title)
 
     if show | save:
 
         xlabel = f'spectral axis [{unit_spectral_axis.to_string()}]'
 
-        fig = plt.figure(figsize=(8, 4), dpi=100)
-        ax = fig.add_subplot(1, 1, 1)
+        fig, ax = plt.subplots(1, 1, dpi=100)
+
         # Spectrum
         ax.step(
             spectral_axis, flux + 1, where='mid', color='C0', zorder=3, label='custom')
         ax.step(
             spectral_axis_ref, flux_ref, where='mid', color='C1', zorder=3, 
             label='reference')
+
         # Settings
         ax.grid(axis='both', color='0.95', zorder=-1)
         ax.set_xlim(spectral_axis[0], spectral_axis[-1])
         ax.tick_params(
             which='major', direction='in', top=True, right=True, length=5, width=1.5, 
             labelsize=12)
         ax.set_xlabel(xlabel, fontsize=16)
         ax.set_ylabel('flux', fontsize=16)
         ax.legend(fontsize=16)
         ax.set_title(title, fontsize=16)
+        fig.set_figheight(0.5 * fig.get_figwidth())
         fig.tight_layout()
         
         if save: plt.savefig(fig_path, dpi=100)
 
         if show: plt.show()
 
         plt.close()
@@ -223,19 +226,19 @@
     # `__setattr__` of `~specutils.Spectrum1D` is disabled
     new_spectrum1d = Spectrum1D(
         spectral_axis=spectral_axis, flux=new_spectrum1d.flux, 
         uncertainty=new_spectrum1d.uncertainty, mask=new_spectrum1d.mask, meta=meta)
 
     return new_spectrum1d
 
-# todo: slit loss.
+
 def sensfunc(spectrum1d, exptime, airmass, extinct, standard, bandwid=None, 
              bandsep=None, n_piece=3, n_iter=5, sigma_lower=None, sigma_upper=None, 
-             grow=False, use_mask=False, title='sensfunc', show=conf.show, 
-             save=conf.save, path=conf.path):
+             grow=False, use_mask=False, title='sensfunc', show=conf.fig_show, 
+             save=conf.fig_save, path=conf.fig_path):
     """Create sensitivity function.
     
     Parameters
     ----------
     spectrum1d : `~specutils.Spectrum1D` or `~numpy.ndarray`
         Input spectrum.
 
@@ -476,32 +479,36 @@
 
     _validateString(title, 'title')
 
     fig_path = _validatePath(save, path, title)
 
     if show | save:
 
-        fig = plt.figure(figsize=(6, 4), dpi=100)
-        ax = fig.add_subplot(1, 1, 1)
+        fig, ax = plt.subplots(1, 1, dpi=100)
+
         # Spectrum
         _plotSpectrum1D(
             ax, wavelength_obs, (flux_obs / bin_width_obs), xlabel='wavelength [A]')
+
         # Bandpasses
         ymin, ymax = ax.get_ylim()
         height = (ymax - ymin) * 0.06
         patches = list()
         for i, bandpass in enumerate(bandpass_arr):
             width = bandpass[1] - bandpass[0]
             rectangle = Rectangle(
                 (bandpass[0], (flux_bp_obs[i] - height / 2)), width, height)
             patches.append(rectangle)
         patch_collection = PatchCollection(
             patches, facecolor='None', edgecolor='r', lw=1.5, zorder=2.5)
         ax.add_collection(patch_collection)
+
+        # Settings
         ax.set_title(title, fontsize=16)
+        fig.set_figheight(fig.get_figwidth * 2 / 3)
         fig.tight_layout()
 
         if save: plt.savefig(fig_path, dpi=100)
 
         if show: plt.show()
 
         plt.close()
```

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/io.py` & `astro-drpy-0.0.1.6/src/drpy/onedspec/io.py`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/README` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/README`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/blackbody/b.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/b.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/blackbody/h.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/h.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/blackbody/i.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/i.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/blackbody/j.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/j.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/blackbody/k.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/k.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/blackbody/l.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/l.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/blackbody/lprime.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/lprime.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/blackbody/m.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/m.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/blackbody/mkbbcal.cl` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/mkbbcal.cl`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/blackbody/mkbbdat.cl` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/mkbbdat.cl`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/blackbody/params.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/params.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/blackbody/r.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/r.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/blackbody/u.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/u.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/blackbody/v.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/blackbody/v.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctio/multi4m.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/multi4m.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctio/nd1m.100mag.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd1m.100mag.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctio/nd1m.125mag.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd1m.125mag.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctio/nd1m.250mag.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd1m.250mag.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctio/nd1m.500mag.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd1m.500mag.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctio/nd4m.l000mag.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd4m.l000mag.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctio/nd4m.l250mag.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd4m.l250mag.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctio/nd4m.rc500mag.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd4m.rc500mag.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u000mag.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u000mag.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u025mag.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u025mag.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u075mag.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u075mag.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u150mag.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u150mag.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u225mag.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/nd4m.u225mag.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctio/ndfilters.men` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctio/ndfilters.men`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/cd32.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/cd32.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/eg21.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/eg21.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/eg274.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/eg274.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/g9937.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/g9937.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/hz2.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/hz2.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/hz4.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/hz4.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l1020.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l1020.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l1788.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l1788.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l2415.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l2415.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l2511.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l2511.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l3218.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l3218.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l377.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l377.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l3864.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l3864.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l4364.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l4364.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l4816.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l4816.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l6248.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l6248.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l7379.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l7379.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l74546.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l74546.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l7987.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l7987.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l8702.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l8702.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l9239.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l9239.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l93080.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l93080.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l9491.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l9491.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/l97030.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/l97030.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/lds235.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/lds235.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/ross627.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/ross627.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/standards.men` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/standards.men`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctiocal/w485a.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctiocal/w485a.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/cd32.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/cd32.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/cd32blue.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/cd32blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/cd32red.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/cd32red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/eg21.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/eg21.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/eg21blue.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/eg21blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/eg21red.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/eg21red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/eg274.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/eg274.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/eg274blue.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/eg274blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/eg274red.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/eg274red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/f110.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/f110.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/f110blue.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/f110blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/f110red.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/f110red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/f56.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/f56.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/f56blue.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/f56blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/f56red.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/f56red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/h600.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/h600.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/h600blue.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/h600blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/h600red.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/h600red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l1020.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l1020.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l1020blue.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l1020blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l1020red.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l1020red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l1788.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l1788.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l1788blue.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l1788blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l1788red.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l1788red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l2415.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l2415.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l2415blue.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l2415blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l2415red.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l2415red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l3218.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l3218.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l3218blue.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l3218blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l3218red.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l3218red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l377.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l377.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l377blue.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l377blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l377red.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l377red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l3864.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l3864.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l3864blue.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l3864blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l3864red.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l3864red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l4364.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l4364.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l4364blue.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l4364blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l4364red.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l4364red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l4816.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l4816.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l4816blue.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l4816blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l4816red.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l4816red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l6248.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l6248.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l6248blue.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l6248blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l6248red.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l6248red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l7379.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l7379.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l7379blue.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l7379blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l7379red.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l7379red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l745.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l745.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l745red.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l745red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l7987.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l7987.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l7987blue.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l7987blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l7987red.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l7987red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l9239.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l9239.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l9239blue.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l9239blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l9239red.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l9239red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l9491.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l9491.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l9491blue.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l9491blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/l9491red.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/l9491red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/ctionewcal/standards.men` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/ctionewcal/standards.men`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/aaareadme.hst` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/aaareadme.hst`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fagk81d266.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fagk81d266.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fbd28d4211.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fbd28d4211.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fbd33d2642.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fbd33d2642.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fbd75d325.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fbd75d325.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fbpm16274.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fbpm16274.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/ffeige110.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/ffeige110.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/ffeige34.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/ffeige34.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fg191b2b.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fg191b2b.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fg93_48.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fg93_48.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fgd108.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fgd108.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fgd50.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fgd50.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fgrw70d5824.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fgrw70d5824.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fhd49798.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhd49798.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fhd60753.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhd60753.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fhd93521.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhd93521.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fhr153.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhr153.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fhr1996.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhr1996.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fhr4554.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhr4554.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fhr5191.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhr5191.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fhr7001.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhr7001.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fhz2.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhz2.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fhz21.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhz21.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fhz4.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhz4.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fhz44.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fhz44.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/flb227.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/flb227.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/flds749b.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/flds749b.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/fngc7293.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/fngc7293.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/magk81d266.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/magk81d266.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mbd28d4211.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mbd28d4211.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mbd33d2642.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mbd33d2642.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mbd75d325.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mbd75d325.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mbpm16274.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mbpm16274.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mfeige110.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mfeige110.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mfeige34.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mfeige34.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mg191b2b.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mg191b2b.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mg93_48.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mg93_48.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mgd108.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mgd108.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mgd50.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mgd50.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mgrw70d5824.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mgrw70d5824.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mhd49798.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhd49798.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mhd60753.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhd60753.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mhd93521.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhd93521.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mhr153.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhr153.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mhr1996.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhr1996.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mhr4554.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhr4554.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mhr5191.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhr5191.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mhr7001.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhr7001.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mhz2.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhz2.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mhz21.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhz21.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mhz4.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhz4.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mhz44.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mhz44.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mlb227.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mlb227.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mlds749b.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mlds749b.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/hststan/mngc7293.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/hststan/mngc7293.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/names.men` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/names.men`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/iidscal/standards.men` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/iidscal/standards.men`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/bd082015.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/bd082015.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/bd174708.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/bd174708.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/bd253941.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/bd253941.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/bd262606.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/bd262606.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/bd284211.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/bd284211.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/bd332642.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/bd332642.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/bd404032.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/bd404032.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/feige110.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/feige110.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/feige15.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/feige15.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/feige25.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/feige25.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/feige34.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/feige34.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/feige56.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/feige56.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/feige92.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/feige92.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/feige98.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/feige98.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/g191b2b.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/g191b2b.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/hd109995.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd109995.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/hd117880.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd117880.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/hd161817.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd161817.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/hd17520.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd17520.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/hd192281.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd192281.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/hd19445.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd19445.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/hd217086.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd217086.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/hd2857.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd2857.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/hd60778.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd60778.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/hd74721.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd74721.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/hd84937.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd84937.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/hd86986.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hd86986.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/he3.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/he3.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/hiltner102.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hiltner102.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/hiltner600.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hiltner600.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/hr7001.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hr7001.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/hz44.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/hz44.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/kopff27.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/kopff27.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/standards.men` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/standards.men`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/irscal/wolf1346.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/irscal/wolf1346.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/kpnoextinct.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/kpnoextinct.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/names.men` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/names.men`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/oke1990/bd284211.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/bd284211.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/oke1990/bd75325.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/bd75325.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/oke1990/feige110.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/feige110.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/oke1990/feige34.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/feige34.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/oke1990/feige67.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/feige67.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/oke1990/g13831.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/g13831.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/oke1990/g191b2b.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/g191b2b.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/oke1990/g19374.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/g19374.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/oke1990/g249.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/g249.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/oke1990/gd108.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/gd108.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/oke1990/gd248.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/gd248.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/oke1990/hz21.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/hz21.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/oke1990/ltt9491.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/oke1990/ltt9491.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/aaareadme.oke` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/aaareadme.oke`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fbd25d4655.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fbd25d4655.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fbd28d4211.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fbd28d4211.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fbd33d2642.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fbd33d2642.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fbd75d325.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fbd75d325.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/ffeige110.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/ffeige110.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/ffeige34.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/ffeige34.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/ffeige66.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/ffeige66.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/ffeige67.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/ffeige67.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fg138_31.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fg138_31.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fg158_100.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fg158_100.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fg191b2b.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fg191b2b.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fg193_74.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fg193_74.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fg24_9.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fg24_9.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fg60_54.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fg60_54.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fgd108.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fgd108.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fgd248.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fgd248.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fgd50.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fgd50.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fgrw70d5824.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fgrw70d5824.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fhd93521.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fhd93521.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fhz21.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fhz21.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fhz4.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fhz4.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fhz44.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fhz44.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fltt9491.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fltt9491.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fngc7293.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fngc7293.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/fsa95_42.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/fsa95_42.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mbd25d4655.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mbd25d4655.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mbd28d4211.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mbd28d4211.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mbd33d2642.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mbd33d2642.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mbd75d325.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mbd75d325.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mfeige110.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mfeige110.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mfeige34.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mfeige34.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mfeige66.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mfeige66.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mfeige67.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mfeige67.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mg138_31.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mg138_31.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mg158_100.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mg158_100.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mg191b2b.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mg191b2b.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mg193_74.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mg193_74.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mg24_9.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mg24_9.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mg60_54.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mg60_54.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mgd108.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mgd108.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mgd248.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mgd248.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mgd50.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mgd50.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mgrw70d5824.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mgrw70d5824.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mhd93521.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mhd93521.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mhz21.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mhz21.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mhz4.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mhz4.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mhz44.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mhz44.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mltt9491.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mltt9491.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/mngc7293.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/mngc7293.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/okestan/msa95_42.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/okestan/msa95_42.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/40erib.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/40erib.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/bd174708.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/bd174708.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/bd262606.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/bd262606.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/feige24.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/feige24.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/g191b2b.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/g191b2b.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/g4718.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/g4718.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/g9937.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/g9937.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/gd140.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/gd140.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/gd190.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/gd190.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/grw705824.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/grw705824.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/grw708247.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/grw708247.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/grw738031.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/grw738031.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/hd19445.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/hd19445.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/hd84937.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/hd84937.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/he3.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/he3.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/hz29.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/hz29.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/hz43.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/hz43.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/hz44.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/hz44.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/l13633.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/l13633.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/l151234b.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/l151234b.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/l74546a.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/l74546a.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/l93080.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/l93080.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/l97030.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/l97030.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/lds235b.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/lds235b.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/lds749b.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/lds749b.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/names.men` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/names.men`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/ross627.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/ross627.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/ross640.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/ross640.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/sa29130.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/sa29130.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/standards.men` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/standards.men`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/wolf1346.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/wolf1346.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/redcal/wolf485a.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/redcal/wolf485a.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr1544.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr1544.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr1544blue.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr1544blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr1544red.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr1544red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr3454.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr3454.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr3454blue.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr3454blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr3454red.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr3454red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr4468.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr4468.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr4468blue.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr4468blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr4468red.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr4468red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr4963.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr4963.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr4963blue.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr4963blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr4963red.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr4963red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr5501.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr5501.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr5501blue.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr5501blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr5501red.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr5501red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr718.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr718.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr718blue.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr718blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr718red.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr718red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr7596.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr7596.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr7596blue.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr7596blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr7596red.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr7596red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr7950.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr7950.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr7950blue.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr7950blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr7950red.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr7950red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr8634.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr8634.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr8634blue.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr8634blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr8634red.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr8634red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr9087.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr9087.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr9087blue.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr9087blue.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/hr9087red.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/hr9087red.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/names.men` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/names.men`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec16cal/standards.men` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec16cal/standards.men`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/bd284211.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/bd284211.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/cygob2no9.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/cygob2no9.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/eg81.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/eg81.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/feige110.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/feige110.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/feige34.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/feige34.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/feige66.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/feige66.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/feige67.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/feige67.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/g191b2b.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/g191b2b.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/gd140.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/gd140.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/hd192281.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/hd192281.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/hd217086.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/hd217086.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/hilt600.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/hilt600.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/hz14.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/hz14.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/hz44.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/hz44.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/pg0205134.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg0205134.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/pg0216032.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg0216032.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/pg0310149.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg0310149.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/pg0823546.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg0823546.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/pg0846249.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg0846249.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/pg0934554.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg0934554.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/pg0939262.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg0939262.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/pg1121145.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg1121145.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/pg1545035.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg1545035.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/pg1708602.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/pg1708602.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/standards.men` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/standards.men`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spec50cal/wolf1346.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spec50cal/wolf1346.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/bd284211.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/bd284211.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/cygob2no9.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/cygob2no9.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/eg81.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/eg81.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/feige110.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/feige110.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/feige34.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/feige34.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/feige66.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/feige66.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/feige67.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/feige67.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/g191b2b.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/g191b2b.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/gd140.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/gd140.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/hd192281.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/hd192281.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/hd217086.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/hd217086.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/hiltner600.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/hiltner600.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/hz14.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/hz14.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/hz44.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/hz44.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/pg0205134.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg0205134.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/pg0216032.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg0216032.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/pg0310149.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg0310149.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/pg0823546.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg0823546.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/pg0846249.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg0846249.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/pg0934554.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg0934554.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/pg0939262.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg0939262.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/pg1121145.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg1121145.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/pg1545035.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg1545035.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/pg1708602.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/pg1708602.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/onedspec/lib/onedstds/spechayescal/wolf1346.dat` & `astro-drpy-0.0.1.6/src/drpy/onedspec/lib/onedstds/spechayescal/wolf1346.dat`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/plotting.py` & `astro-drpy-0.0.1.6/src/drpy/plotting.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,25 +11,89 @@
 # drpy
 from drpy import conf
 
 from .validate import (_validateBool, _validatePath, _validateRange, _validateString, 
                        _validateSpectrum)
 
 # Set plot parameters
+plt.rcParams['figure.figsize'] = [conf.fig_width, conf.fig_width]
 plt.rcParams['axes.linewidth'] = 1.5
 plt.rcParams['mathtext.fontset'] = 'stix'
 plt.rcParams['font.family'] = 'STIXGeneral'
 
 __all__ = ['plotFitting', 'plotSpectrum1D', 'plot2d']
 
 
-# todo: add _plotFitting?
+def _plotFitting(ax, x, y, residual, mask, y_fit, x_fit, threshold_lower, 
+                 threshold_upper, xlabel='x', ylabel='y', use_relative=False):
+    """Plot fitting."""
+
+    if (threshold_lower is None) & (threshold_upper is None):
+        ymin = None; ymax = None
+    elif threshold_lower is None:
+        ymax = 1.67 * threshold_upper; ymin = -ymax
+    elif threshold_upper is None:
+        ymin = 1.67 * threshold_lower; ymax = -ymin
+    else:
+        ymax = 1.67 * np.max(np.abs([threshold_lower, threshold_upper])); ymin = -ymax
+    
+    # Data
+    ax[0].plot(x[mask], y[mask], '+', c='lightgrey', ms=8)
+    ax[0].plot(x[~mask], y[~mask], '+', c='black', ms=8)
+    # Fitted data
+    ax[0].plot(x_fit, y_fit, '-', c='red', lw=1.5)
+    
+    # Settings
+    ax[0].grid(True, ls='--')
+    # ticks
+    ax[0].tick_params(
+        which='major', direction='in', top=True, right=True, length=5, width=1.5, 
+        labelsize=12)
+    ax[0].minorticks_off()
+    # lim
+    ax[0].set_xlim(x_fit[0], x_fit[-1])
+    if ymin is not None:
+        if use_relative:
+            ax[0].set_ylim((y_fit.min() + y_fit.max() * ymin), y_fit.max() * (1 + ymax))
+        else:
+            ax[0].set_ylim(y_fit.min() + ymin, y_fit.max() + ymax)
+    # labels
+    ax[0].set_ylabel(ylabel, fontsize=16)
+
+    # Residual
+    ax[1].plot(x[mask], residual[mask], '+', c='lightgrey', ms=8)
+    ax[1].plot(x[~mask], residual[~mask], '+', c='black', ms=8)
+    ax[1].axhline(y=0, ls='-', c='red', lw=1.5)
+    if threshold_lower is not None:
+        ax[1].axhline(y=threshold_lower, ls='--', c='red', lw=1.5)
+    if threshold_upper is not None:
+        ax[1].axhline(y=threshold_upper, ls='--', c='red', lw=1.5)
+    
+    # Settings
+    ax[1].grid(True, ls='--')
+    # ticks
+    ax[1].tick_params(
+        which='major', direction='in', top=True, right=True, length=5, width=1.5, 
+        labelsize=12)
+    ax[1].minorticks_off()
+    # lim
+    ax[1].set_ylim(ymin, ymax)
+    # label
+    ax[1].set_xlabel(xlabel, fontsize=16)
+    if use_relative:
+        label_residual = 'rel. residual'
+    else:
+        label_residual = 'residual'
+    ax[1].set_ylabel(label_residual, fontsize=16)
+
+    
 def plotFitting(x, y, residual, mask, y_fit, x_fit=None, threshold_lower=None, 
                 threshold_upper=None, xlabel='x', ylabel='y', title='fitting', 
-                show=conf.show, save=conf.save, path=conf.path, use_relative=False):
+                show=conf.fig_show, save=conf.fig_save, path=conf.fig_path, 
+                use_relative=False):
     """Plot fitting.
 
     Parameters
     ----------
     show : bool, optional
         Whether to show plot.
 
@@ -63,73 +127,25 @@
         if threshold_upper is not None:
             if np.isnan(threshold_upper) | np.isinf(threshold_upper):
                 threshold_upper = None
             else:
                 _validateRange(
                     threshold_upper, 'threshold_upper', (0, None), (True, None))
 
-        _validateString(xlabel, 'xlabel')
-        _validateString(ylabel, 'ylabel')
-
         _validateBool(use_relative, 'use_relative')
-        if use_relative:
-            label_residual = 'rel. residual'
-        else:
-            label_residual = 'residual'
 
-        fig = plt.figure(figsize=(6, 6), dpi=100)
-        gs = gridspec.GridSpec(3, 1)
-        ax = fig.add_subplot(gs[:2]), fig.add_subplot(gs[2])
-
-        # Data
-        ax[0].plot(x[mask], y[mask], '+', c='lightgrey', ms=8)
-        ax[0].plot(x[~mask], y[~mask], '+', c='black', ms=8)
-        # Fitted data
-        ax[0].plot(x_fit, y_fit, '-', c='red', lw=1.5)
-        # Settings
-        ax[0].grid(True, ls='--')
-        ax[0].set_xlim(x_fit[0], x_fit[-1])
-        # ax[0].set_ylim(y_fit.min(), y_fit.max())
-        ax[0].tick_params(
-            which='major', direction='in', top=True, right=True, length=5, width=1.5, 
-            labelsize=12)
-        ax[0].minorticks_off()
-        ax[0].set_xticklabels([])
-        ax[0].set_ylabel(ylabel, fontsize=16)
-
-        # Residual
-        ax[1].plot(x[mask], residual[mask], '+', c='lightgrey', ms=8)
-        ax[1].plot(x[~mask], residual[~mask], '+', c='black', ms=8)
-        # Settings
-        ax[1].grid(True, ls='--')
-        ax[1].axhline(y=0, ls='-', c='red', lw=1.5)
-        if threshold_lower is not None:
-            ax[1].axhline(y=threshold_lower, ls='--', c='red', lw=1.5)
-        if threshold_upper is not None:
-            ax[1].axhline(y=threshold_upper, ls='--', c='red', lw=1.5)
-        ax[1].set_xlim(x_fit[0], x_fit[-1])
-        if threshold_lower is not None:
-            ymin = 1.67 * threshold_lower
-        else:
-            ymin = None
-        if threshold_upper is not None:
-            ymax = 1.67 * threshold_upper
-        else:
-            ymax = None
-        ax[1].set_ylim(ymin, ymax)
-        ax[1].tick_params(
-            which='major', direction='in', top=True, right=True, length=5, width=1.5, 
-            labelsize=12)
-        ax[1].minorticks_off()
-        ax[1].set_xlabel(xlabel, fontsize=16)
-        ax[1].set_ylabel(label_residual, fontsize=16)
+        fig, ax = plt.subplots(2, 1, sharex=True, height_ratios=[3, 1], dpi=100)
+        fig.subplots_adjust(hspace=0)
+        _plotFitting(
+            ax, x, y, residual, mask, y_fit, x_fit, threshold_lower, threshold_upper, 
+            xlabel, ylabel, use_relative)
+        ax[0].set_title(title, fontsize=16)
         fig.align_ylabels()
-        fig.suptitle(title, fontsize=16)
         fig.tight_layout()
-
+        
         if save: plt.savefig(fig_path, dpi=100)
 
         if show: plt.show()
 
         plt.close()
 
 
@@ -160,17 +176,17 @@
     ax.tick_params(
         which='major', direction='in', top=True, right=True, length=5, width=1.5, 
         labelsize=12)
     ax.minorticks_off()
     ax.set_xlabel(xlabel, fontsize=16)
     ax.set_ylabel(ylabel, fontsize=16)
     
-# todo: add mask, add legend?
-def plotSpectrum1D(spectrum1d, title='spectrum', show=conf.show, save=conf.save, 
-                   path=conf.path):
+# todo: label masked pixels, add legend?
+def plotSpectrum1D(spectrum1d, title='spectrum', show=conf.fig_show, 
+                   save=conf.fig_save, path=conf.fig_path):
     """Plot 1-dimensional spectrum of type `~specutils.Spectrum1D`.
     
     Parameters
     ----------
     spectrum1d : `~specutils.Spectrum1D` or `~numpy.ndarray`
         Input spectrum.
 
@@ -204,19 +220,20 @@
         # Labels
         unit_spectral_axis = new_spectrum1d.spectral_axis.unit.to_string()
         unit_flux = new_spectrum1d.flux.unit.to_string()
 
         xlabel = f'spectral axis [{unit_spectral_axis}]'
         ylabel = f'flux [{unit_flux}]'
 
-        fig = plt.figure(figsize=(6, 4), dpi=100)
-        ax = fig.add_subplot(1, 1, 1)
-        _plotSpectrum1D(ax, spectral_axis, flux, uncertainty, xlabel=xlabel, ylabel=ylabel)
+        fig, ax = plt.subplots(1, 1, dpi=100)
+        _plotSpectrum1D(
+            ax, spectral_axis, flux, uncertainty, xlabel=xlabel, ylabel=ylabel)
         # ax.legend(fontsize=16)
         ax.set_title(title, fontsize=16)
+        fig.set_figheight(0.7 * fig.get_figwidth())
         fig.tight_layout()
 
         if save: plt.savefig(fig_path, dpi=100)
 
         if show: plt.show()
 
         plt.close()
@@ -248,24 +265,27 @@
         width=1.5, labelsize=12)
     ax.minorticks_off()
     ax.set_xlabel(xlabel, fontsize=16)
     ax.set_ylabel(ylabel, fontsize=16)
 
     # Colorbar
     if cbar:
-        cb = plt.colorbar(im, ax=ax, use_gridspec=True)
+        cb = plt.colorbar(
+            im, ax=ax, fraction=(0.046 * ccd.shape[0] / ccd.shape[1]), pad=0.04, 
+            use_gridspec=True)
         # Settings
         cb.ax.tick_params(
             which='major', direction='in', right=True, color='w', length=5, width=1.5, 
             labelsize=12)
         cb.ax.set_ylabel(cblabel, fontsize=16)
 
 
-def plot2d(ccd, cmap='Greys_r', contrast=0.25, extent=None, cbar=True, title='image', 
-           show=conf.show, save=conf.save, path=conf.path, **kwargs):
+def plot2d(ccd, cmap='Greys_r', contrast=0.25, extent=None, cbar=True, xlabel='column', 
+           ylabel='row', cblabel='pixel value', title='image', show=conf.fig_show, 
+           save=conf.fig_save, path=conf.fig_path, **kwargs):
     """Plot image.
 
     Parameters
     ----------
     show : bool, optional
         Whether to show plot.
 
@@ -280,22 +300,23 @@
 
     _validateString(title, 'title')
 
     fig_path = _validatePath(save, path, title)
 
     if show | save:
 
-        fig = plt.figure(figsize=(6, 6), dpi=100)
-        ax = fig.add_subplot(1, 1, 1)
         if extent is None:
-            extent = (0.5, ccd.shape[1] + 0.5, 0.5, ccd.shape[0] + 0.5)
+            extent = (-0.5, ccd.shape[1] - 0.5, -0.5, ccd.shape[0] - 0.5)
+
+        fig, ax = plt.subplots(1, 1, dpi=100)
         _plot2d(
-            ax=ax, ccd=ccd, cmap=cmap, contrast=contrast, cbar=cbar, extent=extent, 
-            **kwargs)
-        fig.suptitle(title, fontsize=16)
+            ax=ax, ccd=ccd, cmap=cmap, contrast=contrast, extent=extent, cbar=cbar, 
+            xlabel=xlabel, ylabel=ylabel, cblabel=cblabel, **kwargs)
+        ax.set_title(title, fontsize=16)
+        fig.set_figheight(ccd.shape[0] / ccd.shape[1] * fig.get_figwidth())
         fig.tight_layout()
 
         if save: plt.savefig(fig_path, dpi=100)
 
         if show: plt.show()
 
         plt.close()
```

### Comparing `astro-drpy-0.0.1.5/src/drpy/twodspec/longslit.py` & `astro-drpy-0.0.1.6/src/drpy/twodspec/longslit.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 # NumPy
 import numpy as np
 # SciPy
 from scipy import interpolate, signal, ndimage
 from scipy.optimize import OptimizeWarning
 # matplotlib
-from matplotlib import gridspec
 import matplotlib.pyplot as plt
+from matplotlib.backends.backend_pdf import PdfPages
 # AstroPy
 import astropy.units as u
 from astropy.time import Time
 from astropy.nddata import CCDData, StdDevUncertainty
 from astropy.convolution import convolve_fft, Gaussian2DKernel, interpolate_replace_nans
 # ccdproc
 from ccdproc import flat_correct
@@ -20,35 +20,36 @@
 from specutils import Spectrum1D
 # drpy
 from drpy import conf
 from drpy.batch import CCDDataList
 from drpy.onedspec import loadExtinctionCurve
 from drpy.onedspec.center import _center1D_Gaussian, _refinePeakBases, _refinePeaks
 from drpy.modeling import Poly1D, Spline1D, Spline2D, GaussianSmoothing2D
-from drpy.plotting import plotFitting, _plot2d, _plotSpectrum1D
+from drpy.plotting import plotFitting, _plotFitting, plot2d, _plot2d, _plotSpectrum1D
 from drpy.validate import (_validateBool, _validateString, _validateRange, 
                            _validateInteger, _validate1DArray, _validateNDArray, 
                            _validateCCDData, _validateCCDList, _validateCCD, 
                            _validateSpectrum, _validateBins, _validateAperture, 
                            _validatePath)
 
 from .utils import invertCoordinateMap
 
 # Set plot parameters
+plt.rcParams['figure.figsize'] = [conf.fig_width, conf.fig_width]
 plt.rcParams['axes.linewidth'] = 1.5
 plt.rcParams['mathtext.fontset'] = 'stix'
 plt.rcParams['font.family'] = 'STIXGeneral'
 
 __all__ = ['response', 'illumination', 'align', 'fitcoords', 'transform', 'trace', 
            'background', 'extract', 'calibrate2d']
 
 
 def response(ccd, slit_along, n_piece=3, n_iter=5, sigma_lower=None, sigma_upper=None, 
-             grow=False, use_mask=False, title='response', show=conf.show, 
-             save=conf.save, path=conf.path):
+             grow=False, use_mask=False, show=conf.fig_show, save=conf.fig_save, 
+             path=conf.fig_path):
     """Determine response calibration.
 
     Parameters
     ----------
     ccd : `~astropy.nddata.CCDData` or `~numpy.ndarray`
         Input frame.
 
@@ -102,44 +103,45 @@
 
     # Apply mask
     data_arr[mask_arr] = np.nan
 
     # Average along spatial (slit) axis
     x = np.arange(n_col)
     # Bad pixels (NaNs or infs) in the original frame (if any) may lead to unmasked 
-    # elements in ``y`` and may cause an error in the spline fitting below. Bad columns 
-    # will raise warnings but may not cause error.
+    # elements in ``y`` and may cause an error in the spline fitting below.
     y = np.nanmean(data_arr, axis=0)
     mask_y = np.all(mask_arr, axis=0)
 
-    # Fit cubic spline function
+    # Fit cubic spline function (always float64)
     spl, residual, threshold_lower, threshold_upper, master_mask = Spline1D(
         x=x, y=y, weight=None, mask=mask_y, order=3, n_piece=n_piece, n_iter=n_iter, 
         sigma_lower=sigma_lower, sigma_upper=sigma_upper, grow=grow, use_relative=True)
-    y_fit = spl(x)
-    uncertainty_y_fit = (y_fit * residual)[~master_mask].std(ddof=1)
+    
+    # Control precision
+    y_fit = spl(x).astype(ccd.dtype)
+    rms_y_fit = (y_fit * residual)[~master_mask].std(dtype=ccd.dtype)
 
-    # Plot
+    # Fitting plot
     plotFitting(
         x=x, y=y, residual=residual, mask=master_mask, x_fit=x, y_fit=y_fit, 
         threshold_lower=threshold_lower, threshold_upper=threshold_upper, 
-        xlabel='dispersion axis [px]', ylabel='pixel value', title=title, 
+        xlabel='dispersion axis [px]', ylabel='pixel value', title='response', 
         show=show, save=save, path=path, use_relative=True)
 
     if slit_along == 'col':
         rccd = CCDData(
             data=(np.tile(y_fit, (n_row, 1)) * nccd.unit), 
-            uncertainty=StdDevUncertainty(np.full((n_row, n_col), uncertainty_y_fit)), 
+            uncertainty=StdDevUncertainty(np.full((n_row, n_col), rms_y_fit)), 
             mask=np.tile(master_mask, (n_row, 1))
         )
 
     else:
         rccd = CCDData(
             data=(np.tile(y_fit, (n_row, 1)).T * nccd.unit), 
-            uncertainty=StdDevUncertainty(np.full((n_col, n_row), uncertainty_y_fit)), 
+            uncertainty=StdDevUncertainty(np.full((n_col, n_row), rms_y_fit)), 
             mask=np.tile(master_mask, (n_row, 1)).T
         )
 
     # Response calibrated frame
     nccd = flat_correct(ccd=nccd, flat=rccd, norm_value=1)
 
     if ccd.uncertainty is None:
@@ -157,18 +159,18 @@
         nccd = np.ma.array(nccd.data, mask=nccd.mask)
 
     else:
         nccd = deepcopy(nccd.data)
 
     return nccd
 
-# todo: improve multiplot (or plot arrays). doc.
+# todo: doc.
 def illumination(ccd, slit_along, method, sigma=None, n_piece=None, bins=5, n_iter=5, 
                  sigma_lower=None, sigma_upper=None, grow=False, use_mask=False, 
-                 title='illumination', show=conf.show, save=conf.save, path=conf.path):
+                 show=conf.fig_show, save=conf.fig_save, path=conf.fig_path):
     """Model illumination.
 
     Parameters
     ----------
     ccd : `~astropy.nddata.CCDData` or `~numpy.ndarray`
         Input frame.
 
@@ -327,16 +329,17 @@
                 n_piece=n_piece, n_iter=n_iter, sigma_lower=sigma_lower, 
                 sigma_upper=sigma_upper, axis=0, grow=grow, use_relative=True)
 
             data_fit = bispl(idx_col, idx_row, grid=True).T
         
         master_mask |= mask_arr
         
-        uncertainty_arr = np.full(
-            (n_row, n_col), (data_fit * residual)[~master_mask].std(ddof=1))
+        data_fit = data_fit.astype(ccd.dtype)
+        rms_arr = np.full(
+            (n_row, n_col), (data_fit * residual)[~master_mask].std(dtype=ccd.dtype))
 
         # In 2D case, ``loc_bin`` is only used as index, thus converted to ``int``.
         idx_bin = loc_bin.astype(int)
         bin_data_arr = data_arr[:, idx_bin].T
         bin_data_fit = data_fit[:, idx_bin].T
         bin_mask_arr = master_mask[:, idx_bin].T
         bin_residual = residual[:, idx_bin].T
@@ -354,15 +357,15 @@
     elif method == 'iraf':  # 1-dimensional method (`iraf`)
 
         n_piece = _validate1DArray(n_piece, 'n_piece', n_bin, True)
 
         # Apply mask
         data_arr[mask_arr] = np.nan
 
-        uncertainty_arr = np.zeros_like(data_arr)
+        rms_arr = np.zeros_like(data_arr)
         master_mask = np.zeros_like(data_arr, dtype=bool)
 
         bin_data_arr = np.zeros((n_bin, n_row))
         bin_data_fit = np.zeros((n_bin, n_row))
         bin_mask_arr = np.zeros((n_bin, n_row), dtype=bool)
         bin_residual = np.zeros((n_bin, n_row))
         bin_threshold_lower = [None] * n_bin
@@ -377,49 +380,71 @@
             # Fit cubic spline function
             bin_spl, bin_residual[i], bin_threshold_lower[i], bin_threshold_upper[i], \
             bin_mask_arr[i] = Spline1D(
                 x=idx_row, y=bin_data_arr[i], weight=None, mask=bin_mask, order=3, 
                 n_piece=n_piece[i], n_iter=n_iter, sigma_lower=sigma_lower, 
                 sigma_upper=sigma_upper, grow=grow, use_relative=True)
             bin_data_fit[i] = bin_spl(idx_row)
-            uncertainty_arr[:, bin_start:bin_end] = (
-                bin_data_fit[i] * bin_residual[i])[~bin_mask_arr[i]].std(ddof=1)
+            rms_arr[:, bin_start:bin_end] = (
+                bin_data_fit[i] * bin_residual[i])[~bin_mask_arr[i]].std()
             master_mask[bin_mask_arr[i], bin_start:bin_end] = True
         
         # Interpolate
         data_fit = interpolate.interp1d(
             x=loc_bin, y=bin_data_fit.T, axis=1, kind='linear', bounds_error=False, 
-            fill_value='extrapolate', assume_sorted=True)(idx_col)
+            fill_value='extrapolate', assume_sorted=True)(idx_col).astype(ccd.dtype)
 
     if slit_along != 'col':
         data_fit = data_fit.T
-        uncertainty_arr = uncertainty_arr.T
+        rms_arr = rms_arr.T
         master_mask = master_mask.T
         n_col, n_row = n_row, n_col
         idx_col, idx_row = idx_row, idx_col
 
-    # Plot
+    # Fitting plot
     if slit_along == 'col':
         x = idx_row
     else:
         x = idx_col
+    
+    _validateBool(show, 'show')
 
-    for i in range(n_bin):
-        plotFitting(
-            x=x, y=bin_data_arr[i], residual=bin_residual[i], mask=bin_mask_arr[i], 
-            x_fit=x, y_fit=bin_data_fit[i], threshold_lower=bin_threshold_lower[i], 
-            threshold_upper=bin_threshold_upper[i], xlabel='spatial axis [px]', 
-            ylabel='pixel value', title=f'{title} at {slit_along} {loc_bin[i]}', 
-            show=show, save=save, path=path, use_relative=True)
+    fig_path = _validatePath(save, path, 'illumination fitting', '.pdf')
+
+    if show | save:
+
+        with PdfPages(fig_path, keep_empty=False) as pdf:
+
+            for i in range(n_bin):
+
+                fig, ax = plt.subplots(2, 1, sharex=True, height_ratios=[3, 1], dpi=100)
+                fig.subplots_adjust(hspace=0)
+
+                _plotFitting(
+                    ax=ax, x=x, y=bin_data_arr[i], residual=bin_residual[i], 
+                    mask=bin_mask_arr[i], x_fit=x, y_fit=bin_data_fit[i], 
+                    threshold_lower=bin_threshold_lower[i], 
+                    threshold_upper=bin_threshold_upper[i], xlabel='spatial axis [px]', 
+                    ylabel='pixel value', use_relative=True)
+
+                ax[0].set_title(f'profile at bin {loc_bin[i]}', fontsize=16)
+                fig.align_ylabels()
+                fig.tight_layout()
+
+                if save: pdf.savefig(fig, dpi=100)
+
+                if show: plt.show()
+
+                plt.close()
     
     # Illumination
     nccd.data = deepcopy(data_fit)
 
     if nccd.uncertainty is not None:
-        nccd.uncertainty.array = deepcopy(uncertainty_arr)
+        nccd.uncertainty.array = deepcopy(rms_arr)
 
     if nccd.mask is not None:
         nccd.mask[master_mask] = True
 
     # Output
     if isinstance(ccd, CCDData):
         nccd.header['MKILLUM'] = '{} Illumination.'.format(
@@ -519,18 +544,18 @@
         nccd.header['ALIGNMEN'] = '{} Aligned (shift = {}).'.format(
             Time.now().to_value('iso', subfmt='date_hm'), shift)
         
         nccdlist.append(nccd)
 
     return CCDDataList(nccdlist)
 
-# todo: improve multiplot
+
 def fitcoords(ccd, slit_along, order=0, n_med=5, prominence=1e-3, n_piece=3, n_iter=5, 
               sigma_lower=None, sigma_upper=None, grow=False, use_mask=False, 
-              show=conf.show, save=conf.save, path=conf.path, **kwargs):
+              show=conf.fig_show, save=conf.fig_save, path=conf.fig_path, **kwargs):
     """Fit distortion across the slit.
     
     Parameters
     ----------
     ccd : `~astropy.nddata.CCDData` or `numpy.ndarray`
         Input frame.
     
@@ -664,14 +689,15 @@
             x=loc_bin, y=shift_arr, weight=None, mask=None, order=3, n_piece=n_piece, 
             n_iter=n_iter, sigma_lower=sigma_lower, sigma_upper=sigma_upper, grow=grow, 
             use_relative=False)
         shift_fit = spl(idx_row)
 
         U = idx_col + shift_fit[:, np.newaxis]
 
+        # Fitting plot
         plotFitting(
             x=loc_bin, y=shift_arr, residual=residual, mask=mask, x_fit=idx_row, 
             y_fit=shift_fit, threshold_lower=threshold_lower, 
             threshold_upper=threshold_upper, xlabel='spatial axis [px]', 
             ylabel='shift value [px]', title='zeropoint shift curve', show=show, 
             save=save, path=path, use_relative=False)
 
@@ -763,23 +789,26 @@
             x=x, y=y, z=z, weight=None, mask=mask, order=(order, 3), 
             n_piece=(1, n_piece), bbox=bbox, n_iter=n_iter, sigma_lower=sigma_lower, 
             sigma_upper=sigma_upper, axis=None, grow=grow, use_relative=False)
 
         # !!! Extrapolation is used here (see above) !!!
         U = bispl(idx_col, idx_row, grid=True).T
 
+        # Plot
         _validateBool(show, 'show')
 
-        title = ['peak detection', 'distortion residual']
+        title = 'peak detection'
 
         fig_path = _validatePath(save, path, title)
+        fig_path_fitting = _validatePath(save, path, 'distortion fitting', '.pdf')
 
         if show | save:
-
-            fig = plt.figure(figsize=(6, 6), dpi=100)
+            
+            # Peak detection
+            fig = plt.figure(dpi=100)
             # Split into subplots
             n_subplot = 2
             length = n_col // n_subplot + 1
             for i in range(n_subplot):
                 idx_start, idx_end = i * length, (i + 1) * length
                 idx_peak = np.where((idx_start <= peaks) & (peaks < idx_end))[0]
                 ax = fig.add_subplot(n_subplot, 1, i + 1)
@@ -798,61 +827,69 @@
                     which='major', direction='in', top=True, right=True, length=5, 
                     width=1.5, labelsize=12)
                 ax.tick_params(
                     which='minor', direction='in', top=True, right=True, length=3, 
                     width=1.5, labelsize=12)
                 ax.set_ylabel('normalized intensity', fontsize=16)
             ax.set_xlabel('dispersion axis [px]', fontsize=16)
+            ax.set_title(title, fontsize=16)
             fig.align_ylabels()
-            fig.suptitle(title[0], fontsize=16)
             fig.tight_layout()
 
-            if save: plt.savefig(fig_path[0], dpi=100)
+            if save: plt.savefig(fig_path, dpi=100)
 
             if show: plt.show()
             
             plt.close()
 
+            # Distortion fitting
             if n_bin // 10 >= 10:
                 idx_plot = np.linspace(0, n_bin - 1, 11).astype(int)
 
             else:
                 idx_plot = np.arange(0, n_bin, 10)
                 if idx_plot[-1] != n_bin - 1:
                     idx_plot = np.hstack([idx_plot, n_bin - 1])
 
             z_fit = bispl(idx_col, loc_bin, grid=True).T
+            
+            with PdfPages(fig_path_fitting, keep_empty=False) as pdf:
 
-            for i in idx_plot:
-                plotFitting(
-                    x=refined_peaks_arr[i], y=peaks - refined_peaks_arr[i], 
-                    residual=residual[i], mask=master_mask[i], x_fit=idx_col, 
-                    y_fit=z_fit[i] - idx_col, threshold_lower=threshold_lower, 
-                    threshold_upper=threshold_upper, xlabel='dispersion axis [px]', 
-                    ylabel='shift [px]', title=f'distortion at bin {loc_bin[i]}', 
-                    show=show, save=save, path=path, use_relative=False)
-
-            residual[master_mask] = np.nan
-            cmap = plt.cm.get_cmap('Greys_r').copy(); cmap.set_bad('red', 1.)
-            extent = (0.5, residual.shape[1] + 0.5, 0.5, residual.shape[0] + 0.5)
-
-            fig = plt.figure(figsize=(6, 6), dpi=100)
-            ax = fig.add_subplot(1, 1, 1)
-            _plot2d(
-                ax, residual, cmap=cmap, contrast=0.25, extent=extent, cbar=True, 
-                xlabel='peak number', ylabel='bin number', cblabel='pixel')
-            # Settings
-            fig.suptitle(title[1], fontsize=16)
-            fig.tight_layout()
-
-            if save: plt.savefig(fig_path[1], dpi=100)
-
-            if show: plt.show()
+                for i in idx_plot:
 
-            plt.close()
+                    fig, ax = plt.subplots(
+                        2, 1, sharex=True, height_ratios=[3, 1], dpi=100)
+                    fig.subplots_adjust(hspace=0)
+
+                    _plotFitting(
+                        ax=ax, x=refined_peaks_arr[i], 
+                        y=(peaks - refined_peaks_arr[i]), residual=residual[i], 
+                        mask=master_mask[i], x_fit=idx_col, y_fit=(z_fit[i] - idx_col), 
+                        threshold_lower=threshold_lower, 
+                        threshold_upper=threshold_upper, xlabel='dispersion axis [px]', 
+                        ylabel='shift [px]', use_relative=False)
+
+                    ax[0].set_title(f'distortion at bin {loc_bin[i]}', fontsize=16)
+                    fig.align_ylabels()
+                    fig.tight_layout()
+
+                    if save: pdf.savefig(fig, dpi=100)
+
+                    if show: plt.show()
+
+                    plt.close()
+
+        # Distortion residual
+        residual[master_mask] = np.nan
+        cmap = plt.cm.get_cmap('Greys_r').copy(); cmap.set_bad('red', 1.)
+        extent = (-0.5, residual.shape[1] - 0.5, -0.5, residual.shape[0] - 0.5)
+        plot2d(
+            residual, cmap=cmap, xlabel='peak number', ylabel='bin number', 
+            cblabel='pixel', title='distortion residual', show=show, save=save, 
+            path=path)
 
     V = np.tile(idx_row, (n_col, 1)).T
 
     # Output
     if slit_along != 'col':
         U, V = V.T, U.T
 
@@ -959,22 +996,21 @@
         nccd = deepcopy(nccd.data)
 
     return nccd
 
 # todo: doc
 def trace(ccd, slit_along, fwhm, method, n_med=3, reference_bin=None, interval=None, 
           n_piece=3, n_iter=5, sigma_lower=None, sigma_upper=None, grow=False, 
-          use_mask=False, title='trace', show=conf.show, save=conf.save, 
-          path=conf.path):
+          use_mask=False, title='trace', show=conf.fig_show, save=conf.fig_save, 
+          path=conf.fig_path):
     """Trace on the 2-dimensional spectrum.
     
-    First the profiles along slit axis are binned by taking median along the dispersion 
-    axis. Then the center of the specified feature (that is the strongest one in the 
-    specified interval) in the middle bin is determined by fitting a Gaussian profile. 
-    [...]
+    First the spatial profiles are binned by taking median along the dispersion axis. 
+    Then the center of the specified feature (that is the strongest one in the 
+    interval) in the reference bin is determined by fitting a Gaussian profile. [...]
     
     Parameters
     ----------
     ccd : `~astropy.nddata.CCDData` or `~numpy.ndarray`
         Input frame.
     
     slit_along : str
@@ -989,15 +1025,16 @@
         `center` or `trace`, and
         - if `center`, a straight trace at the center of the specified feature in the 
         middle bin is returned.
         - if `trace`, the center of the specified feature is treated as an initial
         guess for bin by bin Gaussian fittings.
     
     n_med : int, optional
-        Number of profiles to median. Must be >= `3`. Large number for faint source.
+        Number of spatial profiles to median. Must be >= `3`. Large number for faint 
+        source.
         Default is `3`.
     
     reference_bin : int or `None`, optional
         Index of the reference bin.
         If `None`, the reference bin is the middle bin.
     
     interval : 2-tuple or `None`, optional
@@ -1191,15 +1228,16 @@
         # Spline fitting
         spl, residual, threshold_lower, threshold_upper, master_mask = Spline1D(
             x=loc_bin, y=refined_trace, weight=None, mask=mask, order=3, n_piece=n_piece, 
             n_iter=n_iter, sigma_lower=sigma_lower, sigma_upper=sigma_upper, grow=grow, 
             use_relative=False)
 
         fitted_trace = spl(idx_col)
-        
+    
+    # Trace plot
     _validateBool(show, 'show')
 
     _validateString(title, 'title')
     if title != 'trace':
         title = f'{title} trace'
 
     fig_path = _validatePath(save, path, title)
@@ -1210,44 +1248,51 @@
             plotFitting(
                 x=loc_bin, y=refined_trace, residual=residual, mask=master_mask, 
                 x_fit=idx_col, y_fit=fitted_trace, threshold_lower=threshold_lower, 
                 threshold_upper=threshold_upper, xlabel='dispersion axis [px]', 
                 ylabel='spatial axis [px]', title=title, show=show, save=save, 
                 path=path, use_relative=False)
 
-        extent = (0.5, data_arr.shape[1] + 0.5, 0.5, data_arr.shape[0] + 0.5)
+        if slit_along == 'col':
+            height_ratios = (1 / 4.5, n_col / n_row)
+            extent = (-0.5, n_row - 0.5, 0.5, n_col - 0.5)
+        else:
+            extent = (-0.5, n_col - 0.5, 0.5, n_row - 0.5)
+            height_ratios = (1 / 4.5, n_row / n_col)
+        fig, ax = plt.subplots(2, 1, sharex=True, height_ratios=height_ratios, dpi=100)
 
-        fig = plt.figure(figsize=(6, 6), dpi=100)
-        gs = gridspec.GridSpec(3, 1)
-        ax = fig.add_subplot(gs[0]), fig.add_subplot(gs[1:])
         # Subplot 1
         ax[0].step(idx_row, count_ref, 'k-', lw=1.5, where='mid')
-        ax[0].axvline(x=center_ref, color='r', ls='--', lw=1.5)
-        if method == 'trace':
-            ax[0].axvline(x=idx_min_ref, color='b', ls='--', lw=1.5)
-            ax[0].axvline(x=idx_max_ref, color='b', ls='--', lw=1.5)
+        ax[0].axvline(x=center_ref, color='r', ls='-', lw=1.5)
+
         # Settings
         ax[0].grid(axis='both', color='0.95', zorder=-1)
         # ax[0].set_yscale('log')
-        ax[0].set_xlim(center_ref - 10 * fwhm, center_ref + 10 * fwhm)
         ax[0].tick_params(
             which='major', direction='in', top=True, right=True, length=5, width=1.5, 
             labelsize=12)
-        ax[0].set_xlabel('spatial axis [px]', fontsize=16)
         ax[0].set_ylabel('pixel value', fontsize=16)
+        ax[0].set_title(title, fontsize=16)
+
         # Subplot 2
-        _plot2d(
-            ax=ax[1], ccd=data_arr, cmap='Greys_r', contrast=0.25, extent=extent, 
-            cbar=False)
+        if slit_along == 'col':
+            _plot2d(
+                ax=ax[1], ccd=data_arr.T, cmap='Greys_r', contrast=0.25, extent=extent, 
+                cbar=False, xlabel='row', ylabel='column', aspect='auto')
+        else:
+            _plot2d(
+                ax=ax[1], ccd=data_arr, cmap='Greys_r', contrast=0.25, extent=extent, 
+                cbar=False, aspect='auto')
         (xmin, xmax), (ymin, ymax) = ax[1].get_xlim(), ax[1].get_ylim()
-        ax[1].plot(idx_col + 1, fitted_trace + 1, 'r-', lw=1.5)
+        ax[1].plot(fitted_trace, idx_col, 'r-', lw=1.5)
+
         # Settings
         ax[1].set_xlim(xmin, xmax)
         ax[1].set_ylim(ymin, ymax)
-        fig.suptitle(title, fontsize=16)
+        fig.set_figheight(fig.get_figwidth() * np.sum(height_ratios))
         fig.tight_layout()
 
         if save: plt.savefig(fig_path, dpi=100)
 
         if show: plt.show()
 
         plt.close()
@@ -1263,16 +1308,16 @@
     trace1d = Spectrum1D(flux=(fitted_trace * u.pixel), meta=meta)
 
     return trace1d
 
 
 def background(ccd, slit_along, trace1d, distance=50, aper_width=50, degree=1, 
                n_iter=5, sigma_lower=None, sigma_upper=None, grow=False, 
-               use_mask=False, title='background', show=conf.show, save=conf.save, 
-               path=conf.path):
+               use_mask=False, title='background', show=conf.fig_show, 
+               save=conf.fig_save, path=conf.fig_path):
     """Model background.
     
     Sky background of the input frame is modeled col by col (or row by row, depending 
     on the ``slit_along``) through polynomial fittings.
 
     Parameters
     ----------
@@ -1377,74 +1422,103 @@
             x=idx_row[mask_bkg], y=data_arr[mask_bkg, i], weight=None, 
             mask=mask_arr[mask_bkg, i], degree=degree, n_iter=n_iter, 
             sigma_lower=sigma_lower, sigma_upper=sigma_upper, grow=grow, 
             use_relative=False)
 
         bkg_arr[:, i] = p(idx_row)
         mask_arr[mask_bkg, i][master_mask] = True
-        std_arr[:, i] = residual.std(ddof=1)
+        std_arr[:, i] = residual.std()
 
     _validateBool(show, 'show')
 
     _validateString(title, 'title')
     if title != 'background':
         title = f'{title} background'
 
     fig_path = _validatePath(save, path, title)
+    fig_path_fitting = _validatePath(save, path, f'{title} fitting', '.pdf')
 
     if show | save:
 
-        extent = (0.5, nccd.shape[1] + 0.5, 0.5, nccd.shape[0] + 0.5)
+        if slit_along == 'col':
+            height_ratios = (1 / 4.5, n_col / n_row)
+            extent = (-0.5, n_row - 0.5, 0.5, n_col - 0.5)
+        else:
+            extent = (-0.5, n_col - 0.5, 0.5, n_row - 0.5)
+            height_ratios = (1 / 4.5, n_row / n_col)
+        fig, ax = plt.subplots(2, 1, sharex=True, height_ratios=height_ratios, dpi=100)
 
-        fig = plt.figure(figsize=(6, 6), dpi=100)
-        gs = gridspec.GridSpec(3, 1)
-        ax = fig.add_subplot(gs[0]), fig.add_subplot(gs[1:])
         # Subplot 1
         ax[0].step(idx_row, np.nanmedian(data_arr, axis=1), 'k-', lw=1.5, where='mid')
         ax[0].axvline(x=idx_lbkg_min.mean(), color='y', ls='--', lw=1.5)
         ax[0].axvline(x=idx_lbkg_max.mean(), color='y', ls='--', lw=1.5)
         ax[0].axvline(x=idx_rbkg_min.mean(), color='b', ls='--', lw=1.5)
         ax[0].axvline(x=idx_rbkg_max.mean(), color='b', ls='--', lw=1.5)
+
         # Settings
         ax[0].grid(axis='both', color='0.95', zorder=-1)
-        ax[0].set_xlim(idx_row[0], idx_row[-1])
         ax[0].tick_params(
             which='major', direction='in', top=True, right=True, length=5, width=1.5, 
             labelsize=12)
-        ax[0].set_xlabel('spatial axis [px]', fontsize=16)
         ax[0].set_ylabel('pixel value', fontsize=16)
         ax[0].set_title(title, fontsize=16)
+
         # Subplot 2
-        _plot2d(
-            ax=ax[1], ccd=nccd.data, cmap='Greys_r', contrast=0.25, extent=extent, 
-            cbar=False)
-        (xmin, xmax), (ymin, ymax) = ax[1].get_xlim(), ax[1].get_ylim()
         if slit_along == 'col':
-            ax[1].plot(idx_col + 1, trace1d + 1, 'r--', lw=1.5)
-            ax[1].plot(idx_col + 1, idx_lbkg_min + 1, 'y--', lw=1.5)
-            ax[1].plot(idx_col + 1, idx_lbkg_max + 1, 'y--', lw=1.5)
-            ax[1].plot(idx_col + 1, idx_rbkg_min + 1, 'b--', lw=1.5)
-            ax[1].plot(idx_col + 1, idx_rbkg_max + 1, 'b--', lw=1.5)
+            _plot2d(
+                ax=ax[1], ccd=data_arr.T, cmap='Greys_r', contrast=0.25, extent=extent, 
+                cbar=False, xlabel='row', ylabel='column', aspect='auto')
         else:
-            ax[1].plot(trace1d + 1, idx_row + 1, 'r--', lw=1.5)
-            ax[1].plot(idx_lbkg_min + 1, idx_row + 1, 'y--', lw=1.5)
-            ax[1].plot(idx_lbkg_max + 1, idx_row + 1, 'y--', lw=1.5)
-            ax[1].plot(idx_rbkg_min + 1, idx_row + 1, 'b--', lw=1.5)
-            ax[1].plot(idx_rbkg_max + 1, idx_row + 1, 'b--', lw=1.5)
+            _plot2d(
+                ax=ax[1], ccd=data_arr, cmap='Greys_r', contrast=0.25, extent=extent, 
+                cbar=False, aspect='auto')
+        (xmin, xmax), (ymin, ymax) = ax[1].get_xlim(), ax[1].get_ylim()
+        ax[1].plot(idx_lbkg_min, idx_col, 'y--', lw=1.5)
+        ax[1].plot(idx_lbkg_max, idx_col, 'y--', lw=1.5)
+        ax[1].plot(idx_rbkg_min, idx_col, 'b--', lw=1.5)
+        ax[1].plot(idx_rbkg_max, idx_col, 'b--', lw=1.5)
+
         # Settings
         ax[1].set_xlim(xmin, xmax)
         ax[1].set_ylim(ymin, ymax)
+        fig.set_figheight(fig.get_figwidth() * np.sum(height_ratios))
         fig.tight_layout()
 
         if save: plt.savefig(fig_path, dpi=100)
 
         if show: plt.show()
 
         plt.close()
 
+        # Background fitting plot
+        print(fig_path_fitting)
+        with PdfPages(fig_path_fitting, keep_empty=False) as pdf:
+
+            for i in idx_col[::10]:
+
+                fig, ax = plt.subplots(2, 1, sharex=True, height_ratios=[3, 1], dpi=100)
+                fig.subplots_adjust(hspace=0)
+
+                _plotFitting(
+                    ax=ax, x=idx_row, y=data_arr[:, i], 
+                    residual=(data_arr[:, i] - bkg_arr[:, i]), mask=mask_arr[:, i], 
+                    x_fit=idx_row, y_fit=bkg_arr[:, i], threshold_lower=None, 
+                    threshold_upper=None, xlabel='spatial axis [px]', 
+                    ylabel='pixel value', use_relative=False)
+
+                ax[0].set_title(f'background at column {i}', fontsize=16)
+                fig.align_ylabels()
+                fig.tight_layout()
+
+                if save: pdf.savefig(fig, dpi=100)
+
+                if show: plt.show()
+
+                plt.close()
+
     # Background frame
     if slit_along == 'col':
         nccd.data = deepcopy(bkg_arr)
 
         if nccd.uncertainty is not None:
             nccd.uncertainty.array = deepcopy(std_arr)
 
@@ -1469,35 +1543,49 @@
 
     else:
         nccd = deepcopy(nccd.data)
 
     return nccd
 
 
-def extract(ccd, slit_along, trace1d, aper_width, n_aper=1, spectral_axis=None, 
-            title='aperture', show=conf.show, save=conf.save, path=conf.path):
+def extract(ccd, slit_along, trace1d, aper_width, method, psf_width=None, n_aper=1, 
+            spectral_axis=None, title='aperture', show=conf.fig_show, 
+            save=conf.fig_save, path=conf.fig_path):
     """Extract 1-dimensional spectra.
     
     Parameters
     ----------
     ccd : `~astropy.nddata.CCDData` or `~numpy.ndarray`
         Input frame.
     
     slit_along : str
         `col` or `row`. If `row`, the data array of ``ccd`` will be transposed during 
         calculations. Note that this will NOT affect the returned trace.
     
     trace1d : `~specutils.Spectrum1D` or scalar or `~numpy.ndarray`
         Input trace.
     
-    aper_width : scalar or 2-tuple, optional
+    aper_width : scalar or 2-tuple
         Aperture width.
     
+    method : str
+        Extraction method. `optimal` or `sum`, and
+        - if `optimal`, the optimal extraction algorithm will be used. The spatial 
+        profile will be normalized to unity within ``psf_width``, and then pixels 
+        within ``aper_width`` will be used to compute the source flux. Only one 
+        spectrum will be extracted regardless of ``n_aper``.
+        - if `sum`, the source flux from the pixels within ``aper_width`` will be 
+        summed.
+    
+    psf_width : scalar or 2-tuple or `None`, optional
+        Width of the point spread function (used by the optimal extraction algorithm). 
+        If `None`, it will be set equal to ``aper_width``.
+    
     n_aper : int, optional
-        Number of sub-apertures.
+        Number of sub-apertures (used by the summation extraction algorithm).
         Default is `1`.
 
     spectral_axis : `~astropy.units.Quantity` or `None`
         Spectral axis of the extracted 1-dimensional spectra.
 
     Returns
     -------
@@ -1518,100 +1606,125 @@
 
     idx_row, idx_col = np.arange(n_row), np.arange(n_col)
 
     # Assume that unit of the trace is [pixel]
     if isinstance(trace1d, Spectrum1D):
         trace1d = trace1d.flux.value
     trace1d = _validate1DArray(trace1d, 'trace1d', n_col, True)
-
-    aper_width = _validateAperture(aper_width)
     
-    _validateInteger(n_aper, 'n_aper', (1, None), (True, None))
-
     # The total aperture width is the sum of ``aper_width[0]`` and ``aper_width[1]``. 
     # If they have opposite signs, the whole aperture will be on one side of the trace.
-    aper_edges = trace1d + np.linspace(
-        -aper_width[0], aper_width[1], n_aper + 1)[:, np.newaxis]
-
-    # Out-of-range problem can be ignored in background modeling while cannot here.
-    if (aper_edges.min() < -0.5) | (aper_edges.max() > n_row - 0.5):
-        raise ValueError('Aperture edge is out of range.')
-
-    data_aper = np.zeros((n_aper, n_col))
-
-    uncertainty_aper = np.zeros((n_aper, n_col)) # !!! Variance !!!
+    aper_width = _validateAperture(aper_width, 'aper_width')
+    aper_width[0] *= -1; aper_width.sort()
     
-    mask_aper = np.zeros((n_aper, n_col), dtype=bool)
-
-    for i in idx_col:
-
-        aper_start, aper_end = aper_edges[:-1, i], aper_edges[1:, i]
-
-        for j in range(n_aper):
-
-            # Internal pixels
-            mask = (aper_start[j] < idx_row - 0.5) & (idx_row + 0.5 < aper_end[j])
-            data_aper[j, i] = data_arr[mask, i].sum()
-            uncertainty_aper[j, i] = np.sum(uncertainty_arr[mask, i]**2)
-            mask_aper[j, i] = np.any(mask_arr[mask, i])
-
-            # Edge pixels
-
-            # ``idx_start`` labels the pixel where ``aper_start`` is in
-            idx_start = idx_row[idx_row - 0.5 <= aper_start[j]][-1]
-
-            # ``idx_end`` labels the pixel where ``aper_end`` is in
-            idx_end = idx_row[idx_row + 0.5 >= aper_end[j]][0]
-            
-            # ``aper_start`` and ``aper_end`` are in the same pixel
-            if idx_start == idx_end:
-                data_aper[j, i] += (
-                    data_arr[idx_end, i] * (aper_end[j] - aper_start[j]))
-                uncertainty_aper[j, i] += (
-                    uncertainty_arr[idx_end, i] * (aper_end[j] - aper_start[j]))**2
-                mask_aper[j, i] |= mask_arr[idx_end, i]
+    _validateString(method, 'method', ['optimal', 'sum'])
+    
+    if method == 'optimal':
+        
+        if psf_width is None:
+            psf_width = aper_width
+        else:
+            psf_width = _validateAperture(psf_width, 'psf_width')
+            psf_width[0] *= -1; psf_width.sort()
+            if (psf_width[0] > aper_width[0]) | (psf_width[1] < aper_width[1]):
+                raise ValueError('``aper_width`` should be <= ``psf_width.')
+        
+        psf_edges = np.vstack([np.round(trace1d).astype(int) + round(psf_width[0]), 
+                               np.round(trace1d).astype(int) + round(psf_width[1])]).T
+        
+        psf_arr = np.zeros(((psf_edges[0][1] - psf_edges[0][0] + 1), n_col))
+        for i, psf_edge in enumerate(psf_edges):
+            psf_arr[:, i] = data_arr[psf_edge[0]:(psf_edge[1] + 1), i]
+        
+        # aper_edges = trace1d + np.array([aper_width[0], aper_width[1]])[:, np.newaxis]
+        print(psf_arr)
+        
+    else:
+        
+        _validateInteger(n_aper, 'n_aper', (1, None), (True, None))
+        
+        aper_edges = trace1d + np.linspace(
+            aper_width[0], aper_width[1], n_aper + 1)[:, np.newaxis]
 
-            # in different pixels
-            else:
-                data_aper[j, i] += (
-                    data_arr[idx_start, i] * (idx_start + 0.5 - aper_start[j])
-                    + data_arr[idx_end, i] * (aper_end[j] - (idx_end - 0.5))
-                )
-                uncertainty_aper[j, i] += (
-                    (uncertainty_arr[idx_start, i]
-                     * (idx_start + 0.5 - aper_start[j]))**2 
-                    + (uncertainty_arr[idx_end, i] 
-                       * (aper_end[j] - (idx_end - 0.5)))**2
-                )
-                mask_aper[j, i] |= mask_arr[idx_start, i] | mask_arr[idx_end, i]
+        # Out-of-range problem can be ignored in background modeling while cannot here.
+        if (aper_edges.min() < -0.5) | (aper_edges.max() > n_row - 0.5):
+            raise ValueError('Aperture edge is out of range.')
+
+        data_aper = np.zeros((n_aper, n_col))
+
+        uncertainty_aper = np.zeros((n_aper, n_col)) # !!! Variance !!!
+
+        mask_aper = np.zeros((n_aper, n_col), dtype=bool)
+
+        for i in idx_col:
+
+            aper_start, aper_end = aper_edges[:-1, i], aper_edges[1:, i]
+
+            for j in range(n_aper):
+
+                # Internal pixels
+                mask = (aper_start[j] < idx_row - 0.5) & (idx_row + 0.5 < aper_end[j])
+                data_aper[j, i] = data_arr[mask, i].sum()
+                uncertainty_aper[j, i] = np.sum(uncertainty_arr[mask, i]**2)
+                mask_aper[j, i] = np.any(mask_arr[mask, i])
+
+                # Edge pixels
+
+                # ``idx_start`` labels the pixel where ``aper_start`` is in
+                idx_start = idx_row[idx_row - 0.5 <= aper_start[j]][-1]
+
+                # ``idx_end`` labels the pixel where ``aper_end`` is in
+                idx_end = idx_row[idx_row + 0.5 >= aper_end[j]][0]
+
+                # ``aper_start`` and ``aper_end`` are in the same pixel
+                if idx_start == idx_end:
+                    data_aper[j, i] += (
+                        data_arr[idx_end, i] * (aper_end[j] - aper_start[j]))
+                    uncertainty_aper[j, i] += (
+                        uncertainty_arr[idx_end, i] * (aper_end[j] - aper_start[j]))**2
+                    mask_aper[j, i] |= mask_arr[idx_end, i]
+
+                # in different pixels
+                else:
+                    data_aper[j, i] += (
+                        data_arr[idx_start, i] * (idx_start + 0.5 - aper_start[j])
+                        + data_arr[idx_end, i] * (aper_end[j] - (idx_end - 0.5))
+                    )
+                    uncertainty_aper[j, i] += (
+                        (uncertainty_arr[idx_start, i]
+                         * (idx_start + 0.5 - aper_start[j]))**2 
+                        + (uncertainty_arr[idx_end, i] 
+                           * (aper_end[j] - (idx_end - 0.5)))**2
+                    )
+                    mask_aper[j, i] |= mask_arr[idx_start, i] | mask_arr[idx_end, i]
 
-    uncertainty_aper = np.sqrt(uncertainty_aper) # Standard deviation
+        uncertainty_aper = np.sqrt(uncertainty_aper) # Standard deviation
 
     _validateBool(show, 'show')
 
     _validateString(title, 'title')
     if title != 'aperture':
         title = f'{title} aperture'
 
     fig_path = _validatePath(save, path, title)
 
     if show | save:
 
-        extent = (0.5, nccd.shape[1] + 0.5, 0.5, nccd.shape[0] + 0.5)
+        extent = (-0.5, nccd.shape[1] - 0.5, -0.5, nccd.shape[0] - 0.5)
 
         fig = plt.figure(dpi=100)
         ax = fig.add_subplot(1, 1, 1)
         _plot2d(ax=ax, ccd=nccd.data, cmap='Greys_r', contrast=0.25, extent=extent)
         (xmin, xmax), (ymin, ymax) = ax.get_xlim(), ax.get_ylim()
         if slit_along == 'col':
             for aper_edge in aper_edges:
-                ax.plot(idx_col + 1, aper_edge + 1, 'r--', lw=1.5)
+                ax.plot(idx_col, aper_edge, 'r--', lw=1.5)
         else:
             for aper_edge in aper_edges:
-                ax.plot(aper_edge + 1, idx_row + 1, 'r--', lw=1.5)
+                ax.plot(aper_edge, idx_row, 'r--', lw=1.5)
         # Settings
         ax.set_xlim(xmin, xmax)
         ax.set_ylim(ymin, ymax)
         ax.set_title(title, fontsize=16)
         fig.tight_layout()
 
         if save: plt.savefig(fig_path, dpi=100)
```

### Comparing `astro-drpy-0.0.1.5/src/drpy/twodspec/utils.py` & `astro-drpy-0.0.1.6/src/drpy/twodspec/utils.py`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/utils.py` & `astro-drpy-0.0.1.6/src/drpy/utils.py`

 * *Files identical despite different names*

### Comparing `astro-drpy-0.0.1.5/src/drpy/validate.py` & `astro-drpy-0.0.1.6/src/drpy/validate.py`

 * *Files 4% similar despite different names*

```diff
@@ -394,56 +394,51 @@
         raise ValueError('``bins`` must be 1-dimensional, when an array')
 
     bin_edges = np.vstack([bin_edges[:-1], bin_edges[1:]]).T
 
     return bin_edges
 
 
-def _validateAperture(aper_width):
+def _validateAperture(aperture, name):
     """Validate aperture width."""
 
-    if np.ndim(aper_width) == 0:
+    if np.ndim(aperture) == 0:
 
-        _validateRange(aper_width, 'aper_width', (0, None), (False, None))
+        _validateRange(aperture, name, (0, None), (False, None))
 
-        aper_width = _validate1DArray(aper_width, 'aper_width', 2, True) / 2
+        aperture = _validate1DArray(aperture, name, 2, True) / 2
 
-    elif np.ndim(aper_width) == 1:
+    elif np.ndim(aperture) == 1:
 
-        aper_width = _validate1DArray(aper_width, 'aper_width', 2, True)
+        aperture = _validate1DArray(aperture, name, 2, True)
 
         _validateRange(
-            aper_width.sum(), 'aper_width.sum()', (0, None), (False, None))
+            aperture.sum(), f'{name}.sum()', (0, None), (False, None))
 
     else:
-        raise ValueError('``aper_width`` must be 1-dimensional, when an array')
+        raise ValueError(f'``{name}`` must be 1-dimensional, when an array')
 
-    return aper_width
+    return aperture
 
 
-def _validatePath(save, path, title):
+def _validatePath(save, path, title, extension='.png'):
     """Validate path arguments."""
 
     _validateBool(save, 'save')
 
-    if save:
+    if path is None:
+        path = os.getcwd()
 
-        if path is None:
-            path = os.getcwd()
-
-        else:
-            _validateString(path, 'path')
+    else:
+        _validateString(path, 'path')
 
-        if isinstance(title, str):
-            fig_name = f'{title}.png'.replace(' ', '_')
-            fig_path = os.path.join(path, fig_name)
-        
-        else:
-            fig_path = list()
-            for t in title:
-                fig_name = f'{t}.png'.replace(' ', '_')
-                fig_path.append(os.path.join(path, fig_name))
+    if isinstance(title, str):
+        fig_name = f'{title}{extension}'.replace(' ', '_')
+        fig_path = os.path.join(path, fig_name)
 
     else:
-        fig_path = None
+        fig_path = list()
+        for t in title:
+            fig_name = f'{t}{extension}'.replace(' ', '_')
+            fig_path.append(os.path.join(path, fig_name))
 
     return fig_path
```

