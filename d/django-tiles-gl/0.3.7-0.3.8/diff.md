# Comparing `tmp/django_tiles_gl-0.3.7.tar.gz` & `tmp/django_tiles_gl-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tiles_gl-0.3.7.tar", max compression
+gzip compressed data, was "django_tiles_gl-0.3.8.tar", max compression
```

## Comparing `django_tiles_gl-0.3.7.tar` & `django_tiles_gl-0.3.8.tar`

### file list

```diff
@@ -1,2582 +1,2581 @@
--rw-r--r--   0        0        0    15362 2022-12-03 11:51:47.220650 django_tiles_gl-0.3.7/LICENSE.md
--rw-r--r--   0        0        0     5131 2022-12-03 11:51:47.220650 django_tiles_gl-0.3.7/README.md
--rw-r--r--   0        0        0        0 2022-12-03 11:51:47.316651 django_tiles_gl-0.3.7/django_tiles_gl/__init__.py
--rw-r--r--   0        0        0      103 2022-12-03 11:51:47.316651 django_tiles_gl-0.3.7/django_tiles_gl/apps.py
--rw-r--r--   0        0        0     3469 2022-12-03 11:51:47.316651 django_tiles_gl-0.3.7/django_tiles_gl/mbtiles.py
--rw-r--r--   0        0        0    80025 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/0-255.pbf
--rw-r--r--   0        0        0   134265 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/1024-1279.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/10240-10495.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/10496-10751.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/10752-11007.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/11008-11263.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/11264-11519.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/11520-11775.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/11776-12031.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/12032-12287.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/12288-12543.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/12544-12799.pbf
--rw-r--r--   0        0        0    10755 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/1280-1535.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/12800-13055.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/13056-13311.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/13312-13567.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/13568-13823.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/13824-14079.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/14080-14335.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/14336-14591.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/14592-14847.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/14848-15103.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/15104-15359.pbf
--rw-r--r--   0        0        0       29 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/1536-1791.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/15360-15615.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/15616-15871.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/15872-16127.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/16128-16383.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/16384-16639.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/16640-16895.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/16896-17151.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/17152-17407.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/17408-17663.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/17664-17919.pbf
--rw-r--r--   0        0        0       29 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/1792-2047.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/17920-18175.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/18176-18431.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/18432-18687.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/18688-18943.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/18944-19199.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/19200-19455.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/19456-19711.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/19712-19967.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/19968-20223.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/20224-20479.pbf
--rw-r--r--   0        0        0       29 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/2048-2303.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/20480-20735.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/20736-20991.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/20992-21247.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/21248-21503.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/21504-21759.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/21760-22015.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/22016-22271.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/22272-22527.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/22528-22783.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/22784-23039.pbf
--rw-r--r--   0        0        0       29 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/2304-2559.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/23040-23295.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/23296-23551.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/23552-23807.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/23808-24063.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/24064-24319.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/24320-24575.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/24576-24831.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/24832-25087.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/25088-25343.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/25344-25599.pbf
--rw-r--r--   0        0        0    70900 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/256-511.pbf
--rw-r--r--   0        0        0       29 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/2560-2815.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/25600-25855.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/25856-26111.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/26112-26367.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/26368-26623.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/26624-26879.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/26880-27135.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/27136-27391.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/27392-27647.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/27648-27903.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/27904-28159.pbf
--rw-r--r--   0        0        0       29 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/2816-3071.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/28160-28415.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/28416-28671.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/28672-28927.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/28928-29183.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/29184-29439.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/29440-29695.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/29696-29951.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/29952-30207.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/30208-30463.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/30464-30719.pbf
--rw-r--r--   0        0        0       29 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/3072-3327.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/30720-30975.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/30976-31231.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/31232-31487.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/31488-31743.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/31744-31999.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/32000-32255.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/32256-32511.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/32512-32767.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/32768-33023.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/33024-33279.pbf
--rw-r--r--   0        0        0       29 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/3328-3583.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/33280-33535.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/33536-33791.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/33792-34047.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/34048-34303.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/34304-34559.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/34560-34815.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/34816-35071.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/35072-35327.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/35328-35583.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/35584-35839.pbf
--rw-r--r--   0        0        0       29 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/3584-3839.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/35840-36095.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/36096-36351.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/36352-36607.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/36608-36863.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/36864-37119.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/37120-37375.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/37376-37631.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/37632-37887.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.328652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/37888-38143.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/38144-38399.pbf
--rw-r--r--   0        0        0       29 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/3840-4095.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/38400-38655.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/38656-38911.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/38912-39167.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/39168-39423.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/39424-39679.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/39680-39935.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/39936-40191.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/40192-40447.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/40448-40703.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/40704-40959.pbf
--rw-r--r--   0        0        0       29 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/4096-4351.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/40960-41215.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/41216-41471.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/41472-41727.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/41728-41983.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/41984-42239.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/42240-42495.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/42496-42751.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/42752-43007.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/43008-43263.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/43264-43519.pbf
--rw-r--r--   0        0        0       29 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/4352-4607.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/43520-43775.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/43776-44031.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/44032-44287.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/44288-44543.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/44544-44799.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/44800-45055.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/45056-45311.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/45312-45567.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/45568-45823.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/45824-46079.pbf
--rw-r--r--   0        0        0       29 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/4608-4863.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/46080-46335.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/46336-46591.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/46592-46847.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/46848-47103.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/47104-47359.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/47360-47615.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/47616-47871.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/47872-48127.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/48128-48383.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/48384-48639.pbf
--rw-r--r--   0        0        0       29 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/4864-5119.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/48640-48895.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/48896-49151.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/49152-49407.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/49408-49663.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/49664-49919.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/49920-50175.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/50176-50431.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/50432-50687.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/50688-50943.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/50944-51199.pbf
--rw-r--r--   0        0        0     3918 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/512-767.pbf
--rw-r--r--   0        0        0       29 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/5120-5375.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/51200-51455.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/51456-51711.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/51712-51967.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/51968-52223.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/52224-52479.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/52480-52735.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/52736-52991.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/52992-53247.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/53248-53503.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/53504-53759.pbf
--rw-r--r--   0        0        0       29 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/5376-5631.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/53760-54015.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/54016-54271.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/54272-54527.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/54528-54783.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/54784-55039.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/55040-55295.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/55296-55551.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/55552-55807.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/55808-56063.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/56064-56319.pbf
--rw-r--r--   0        0        0       29 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/5632-5887.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/56320-56575.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/56576-56831.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/56832-57087.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/57088-57343.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/57344-57599.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/57600-57855.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/57856-58111.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/58112-58367.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/58368-58623.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/58624-58879.pbf
--rw-r--r--   0        0        0       29 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/5888-6143.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/58880-59135.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/59136-59391.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/59392-59647.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/59648-59903.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/59904-60159.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/60160-60415.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/60416-60671.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/60672-60927.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/60928-61183.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/61184-61439.pbf
--rw-r--r--   0        0        0       29 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/6144-6399.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/61440-61695.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/61696-61951.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/61952-62207.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/62208-62463.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/62464-62719.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/62720-62975.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/62976-63231.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/63232-63487.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/63488-63743.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/63744-63999.pbf
--rw-r--r--   0        0        0       29 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/6400-6655.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/64000-64255.pbf
--rw-r--r--   0        0        0     3180 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/64256-64511.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/64512-64767.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/64768-65023.pbf
--rw-r--r--   0        0        0       47 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/65024-65279.pbf
--rw-r--r--   0        0        0     1640 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/65280-65535.pbf
--rw-r--r--   0        0        0       29 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/6656-6911.pbf
--rw-r--r--   0        0        0       29 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/6912-7167.pbf
--rw-r--r--   0        0        0       29 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/7168-7423.pbf
--rw-r--r--   0        0        0       29 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/7424-7679.pbf
--rw-r--r--   0        0        0    36235 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/768-1023.pbf
--rw-r--r--   0        0        0    60151 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/7680-7935.pbf
--rw-r--r--   0        0        0      739 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/7936-8191.pbf
--rw-r--r--   0        0        0    10494 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/8192-8447.pbf
--rw-r--r--   0        0        0     5692 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/8448-8703.pbf
--rw-r--r--   0        0        0     5169 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/8704-8959.pbf
--rw-r--r--   0        0        0       29 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/8960-9215.pbf
--rw-r--r--   0        0        0       29 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/9216-9471.pbf
--rw-r--r--   0        0        0      463 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/9472-9727.pbf
--rw-r--r--   0        0        0       29 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/9728-9983.pbf
--rw-r--r--   0        0        0       30 2022-12-03 11:51:47.332651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/9984-10239.pbf
--rw-r--r--   0        0        0    83614 2022-12-03 11:51:47.316651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/0-255.pbf
--rw-r--r--   0        0        0   136097 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/1024-1279.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/10240-10495.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/10496-10751.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/10752-11007.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/11008-11263.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/11264-11519.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/11520-11775.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/11776-12031.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/12032-12287.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/12288-12543.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/12544-12799.pbf
--rw-r--r--   0        0        0    10439 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/1280-1535.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/12800-13055.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/13056-13311.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/13312-13567.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/13568-13823.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/13824-14079.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/14080-14335.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/14336-14591.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/14592-14847.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/14848-15103.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/15104-15359.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/1536-1791.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/15360-15615.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/15616-15871.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/15872-16127.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/16128-16383.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/16384-16639.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/16640-16895.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/16896-17151.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/17152-17407.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/17408-17663.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/17664-17919.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/1792-2047.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/17920-18175.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/18176-18431.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/18432-18687.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/18688-18943.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/18944-19199.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/19200-19455.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/19456-19711.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/19712-19967.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/19968-20223.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/20224-20479.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/2048-2303.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/20480-20735.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/20736-20991.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/20992-21247.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/21248-21503.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/21504-21759.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/21760-22015.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/22016-22271.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/22272-22527.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/22528-22783.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/22784-23039.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/2304-2559.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/23040-23295.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/23296-23551.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/23552-23807.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/23808-24063.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/24064-24319.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/24320-24575.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/24576-24831.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/24832-25087.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/25088-25343.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/25344-25599.pbf
--rw-r--r--   0        0        0    75822 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/256-511.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/2560-2815.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/25600-25855.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/25856-26111.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/26112-26367.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/26368-26623.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/26624-26879.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/26880-27135.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/27136-27391.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/27392-27647.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/27648-27903.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/27904-28159.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/2816-3071.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/28160-28415.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/28416-28671.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/28672-28927.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/28928-29183.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/29184-29439.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/29440-29695.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/29696-29951.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/29952-30207.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/30208-30463.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/30464-30719.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/3072-3327.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/30720-30975.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/30976-31231.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/31232-31487.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/31488-31743.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/31744-31999.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/32000-32255.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/32256-32511.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/32512-32767.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/32768-33023.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/33024-33279.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/3328-3583.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/33280-33535.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/33536-33791.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/33792-34047.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/34048-34303.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/34304-34559.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/34560-34815.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/34816-35071.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/35072-35327.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/35328-35583.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/35584-35839.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/3584-3839.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/35840-36095.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/36096-36351.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/36352-36607.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/36608-36863.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/36864-37119.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/37120-37375.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/37376-37631.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/37632-37887.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/37888-38143.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/38144-38399.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/3840-4095.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/38400-38655.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/38656-38911.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.320651 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/38912-39167.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/39168-39423.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/39424-39679.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/39680-39935.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/39936-40191.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/40192-40447.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/40448-40703.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/40704-40959.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/4096-4351.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/40960-41215.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/41216-41471.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/41472-41727.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/41728-41983.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/41984-42239.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/42240-42495.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/42496-42751.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/42752-43007.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/43008-43263.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/43264-43519.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/4352-4607.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/43520-43775.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/43776-44031.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/44032-44287.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/44288-44543.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/44544-44799.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/44800-45055.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/45056-45311.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/45312-45567.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/45568-45823.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/45824-46079.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/4608-4863.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/46080-46335.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/46336-46591.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/46592-46847.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/46848-47103.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/47104-47359.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/47360-47615.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/47616-47871.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/47872-48127.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/48128-48383.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/48384-48639.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/4864-5119.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/48640-48895.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/48896-49151.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/49152-49407.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/49408-49663.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/49664-49919.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/49920-50175.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/50176-50431.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/50432-50687.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/50688-50943.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/50944-51199.pbf
--rw-r--r--   0        0        0     4101 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/512-767.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/5120-5375.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/51200-51455.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/51456-51711.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/51712-51967.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/51968-52223.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/52224-52479.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/52480-52735.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/52736-52991.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/52992-53247.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/53248-53503.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/53504-53759.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/5376-5631.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/53760-54015.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/54016-54271.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/54272-54527.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/54528-54783.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/54784-55039.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/55040-55295.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/55296-55551.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/55552-55807.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/55808-56063.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/56064-56319.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/5632-5887.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/56320-56575.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/56576-56831.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/56832-57087.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/57088-57343.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/57344-57599.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/57600-57855.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/57856-58111.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/58112-58367.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/58368-58623.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/58624-58879.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/5888-6143.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/58880-59135.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/59136-59391.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/59392-59647.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/59648-59903.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/59904-60159.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/60160-60415.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/60416-60671.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/60672-60927.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/60928-61183.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/61184-61439.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/6144-6399.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/61440-61695.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/61696-61951.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/61952-62207.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/62208-62463.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/62464-62719.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/62720-62975.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/62976-63231.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/63232-63487.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/63488-63743.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/63744-63999.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/6400-6655.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/64000-64255.pbf
--rw-r--r--   0        0        0     4609 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/64256-64511.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/64512-64767.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/64768-65023.pbf
--rw-r--r--   0        0        0       54 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/65024-65279.pbf
--rw-r--r--   0        0        0     1647 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/65280-65535.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/6656-6911.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/6912-7167.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/7168-7423.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/7424-7679.pbf
--rw-r--r--   0        0        0    36964 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/768-1023.pbf
--rw-r--r--   0        0        0    61836 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/7680-7935.pbf
--rw-r--r--   0        0        0      677 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/7936-8191.pbf
--rw-r--r--   0        0        0    10957 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/8192-8447.pbf
--rw-r--r--   0        0        0     5570 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/8448-8703.pbf
--rw-r--r--   0        0        0     5093 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/8704-8959.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/8960-9215.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/9216-9471.pbf
--rw-r--r--   0        0        0      470 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/9472-9727.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/9728-9983.pbf
--rw-r--r--   0        0        0       37 2022-12-03 11:51:47.324652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/9984-10239.pbf
--rw-r--r--   0        0        0    82954 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/0-255.pbf
--rw-r--r--   0        0        0   139691 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/1024-1279.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/10240-10495.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/10496-10751.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/10752-11007.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/11008-11263.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/11264-11519.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/11520-11775.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/11776-12031.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/12032-12287.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/12288-12543.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/12544-12799.pbf
--rw-r--r--   0        0        0    11296 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/1280-1535.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/12800-13055.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/13056-13311.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/13312-13567.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/13568-13823.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/13824-14079.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/14080-14335.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/14336-14591.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/14592-14847.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/14848-15103.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/15104-15359.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/1536-1791.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/15360-15615.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/15616-15871.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/15872-16127.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/16128-16383.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/16384-16639.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/16640-16895.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/16896-17151.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/17152-17407.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/17408-17663.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/17664-17919.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/1792-2047.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/17920-18175.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/18176-18431.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/18432-18687.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/18688-18943.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/18944-19199.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/19200-19455.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/19456-19711.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/19712-19967.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/19968-20223.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/20224-20479.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/2048-2303.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/20480-20735.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/20736-20991.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/20992-21247.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/21248-21503.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/21504-21759.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/21760-22015.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/22016-22271.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/22272-22527.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/22528-22783.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/22784-23039.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/2304-2559.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/23040-23295.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/23296-23551.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/23552-23807.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/23808-24063.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/24064-24319.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/24320-24575.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/24576-24831.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/24832-25087.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/25088-25343.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/25344-25599.pbf
--rw-r--r--   0        0        0    73897 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/256-511.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/2560-2815.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/25600-25855.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/25856-26111.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/26112-26367.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/26368-26623.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/26624-26879.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/26880-27135.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/27136-27391.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/27392-27647.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/27648-27903.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/27904-28159.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/2816-3071.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/28160-28415.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/28416-28671.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/28672-28927.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/28928-29183.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/29184-29439.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/29440-29695.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/29696-29951.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/29952-30207.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/30208-30463.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/30464-30719.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/3072-3327.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/30720-30975.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/30976-31231.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/31232-31487.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/31488-31743.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/31744-31999.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/32000-32255.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/32256-32511.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/32512-32767.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/32768-33023.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/33024-33279.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/3328-3583.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/33280-33535.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/33536-33791.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/33792-34047.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/34048-34303.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/34304-34559.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/34560-34815.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/34816-35071.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/35072-35327.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/35328-35583.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/35584-35839.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/3584-3839.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/35840-36095.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/36096-36351.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/36352-36607.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/36608-36863.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/36864-37119.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/37120-37375.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/37376-37631.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/37632-37887.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/37888-38143.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/38144-38399.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/3840-4095.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/38400-38655.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/38656-38911.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/38912-39167.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/39168-39423.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/39424-39679.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/39680-39935.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/39936-40191.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/40192-40447.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/40448-40703.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/40704-40959.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/4096-4351.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/40960-41215.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/41216-41471.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/41472-41727.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/41728-41983.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/41984-42239.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/42240-42495.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/42496-42751.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/42752-43007.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/43008-43263.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/43264-43519.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/4352-4607.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/43520-43775.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/43776-44031.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/44032-44287.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/44288-44543.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/44544-44799.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/44800-45055.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/45056-45311.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/45312-45567.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/45568-45823.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/45824-46079.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/4608-4863.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/46080-46335.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/46336-46591.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/46592-46847.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/46848-47103.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/47104-47359.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/47360-47615.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/47616-47871.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/47872-48127.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/48128-48383.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/48384-48639.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/4864-5119.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/48640-48895.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/48896-49151.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/49152-49407.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/49408-49663.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/49664-49919.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/49920-50175.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/50176-50431.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/50432-50687.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/50688-50943.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/50944-51199.pbf
--rw-r--r--   0        0        0     4109 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/512-767.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/5120-5375.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/51200-51455.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/51456-51711.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/51712-51967.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/51968-52223.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/52224-52479.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/52480-52735.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/52736-52991.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/52992-53247.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/53248-53503.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/53504-53759.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/5376-5631.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/53760-54015.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/54016-54271.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/54272-54527.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/54528-54783.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/54784-55039.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/55040-55295.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/55296-55551.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/55552-55807.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/55808-56063.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/56064-56319.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/5632-5887.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/56320-56575.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/56576-56831.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/56832-57087.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/57088-57343.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/57344-57599.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/57600-57855.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/57856-58111.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/58112-58367.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/58368-58623.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/58624-58879.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/5888-6143.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/58880-59135.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/59136-59391.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/59392-59647.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/59648-59903.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/59904-60159.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/60160-60415.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/60416-60671.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/60672-60927.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/60928-61183.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/61184-61439.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/6144-6399.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/61440-61695.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/61696-61951.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/61952-62207.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/62208-62463.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/62464-62719.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/62720-62975.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/62976-63231.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/63232-63487.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/63488-63743.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/63744-63999.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/6400-6655.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/64000-64255.pbf
--rw-r--r--   0        0        0     3309 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/64256-64511.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/64512-64767.pbf
--rw-r--r--   0        0        0       36 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/64768-65023.pbf
--rw-r--r--   0        0        0       52 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/65024-65279.pbf
--rw-r--r--   0        0        0     1645 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/65280-65535.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/6656-6911.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/6912-7167.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/7168-7423.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/7424-7679.pbf
--rw-r--r--   0        0        0    37828 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/768-1023.pbf
--rw-r--r--   0        0        0    62708 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/7680-7935.pbf
--rw-r--r--   0        0        0      767 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/7936-8191.pbf
--rw-r--r--   0        0        0    11075 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/8192-8447.pbf
--rw-r--r--   0        0        0     5918 2022-12-03 11:51:47.348652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/8448-8703.pbf
--rw-r--r--   0        0        0     5341 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/8704-8959.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/8960-9215.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/9216-9471.pbf
--rw-r--r--   0        0        0      468 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/9472-9727.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/9728-9983.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/9984-10239.pbf
--rw-r--r--   0        0        0    87547 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/0-255.pbf
--rw-r--r--   0        0        0   143840 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/1024-1279.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/10240-10495.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/10496-10751.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/10752-11007.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/11008-11263.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/11264-11519.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/11520-11775.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/11776-12031.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/12032-12287.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/12288-12543.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/12544-12799.pbf
--rw-r--r--   0        0        0    11017 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/1280-1535.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/12800-13055.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/13056-13311.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/13312-13567.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/13568-13823.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/13824-14079.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/14080-14335.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/14336-14591.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/14592-14847.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/14848-15103.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/15104-15359.pbf
--rw-r--r--   0        0        0       41 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/1536-1791.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/15360-15615.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/15616-15871.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/15872-16127.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/16128-16383.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/16384-16639.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/16640-16895.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/16896-17151.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/17152-17407.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/17408-17663.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/17664-17919.pbf
--rw-r--r--   0        0        0       41 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/1792-2047.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/17920-18175.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/18176-18431.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/18432-18687.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/18688-18943.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/18944-19199.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/19200-19455.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/19456-19711.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/19712-19967.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/19968-20223.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/20224-20479.pbf
--rw-r--r--   0        0        0       41 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/2048-2303.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/20480-20735.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/20736-20991.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/20992-21247.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/21248-21503.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/21504-21759.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/21760-22015.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/22016-22271.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/22272-22527.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/22528-22783.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/22784-23039.pbf
--rw-r--r--   0        0        0       41 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/2304-2559.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/23040-23295.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/23296-23551.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/23552-23807.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/23808-24063.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/24064-24319.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/24320-24575.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/24576-24831.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/24832-25087.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/25088-25343.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/25344-25599.pbf
--rw-r--r--   0        0        0    79892 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/256-511.pbf
--rw-r--r--   0        0        0       41 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/2560-2815.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/25600-25855.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/25856-26111.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/26112-26367.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/26368-26623.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/26624-26879.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/26880-27135.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/27136-27391.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/27392-27647.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/27648-27903.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/27904-28159.pbf
--rw-r--r--   0        0        0       41 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/2816-3071.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/28160-28415.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/28416-28671.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/28672-28927.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/28928-29183.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/29184-29439.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/29440-29695.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/29696-29951.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/29952-30207.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/30208-30463.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/30464-30719.pbf
--rw-r--r--   0        0        0       41 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/3072-3327.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/30720-30975.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/30976-31231.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/31232-31487.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/31488-31743.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/31744-31999.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/32000-32255.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/32256-32511.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/32512-32767.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/32768-33023.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/33024-33279.pbf
--rw-r--r--   0        0        0       41 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/3328-3583.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/33280-33535.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/33536-33791.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/33792-34047.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/34048-34303.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/34304-34559.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/34560-34815.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/34816-35071.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/35072-35327.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/35328-35583.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/35584-35839.pbf
--rw-r--r--   0        0        0       41 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/3584-3839.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/35840-36095.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/36096-36351.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.336652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/36352-36607.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/36608-36863.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/36864-37119.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/37120-37375.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/37376-37631.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/37632-37887.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/37888-38143.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/38144-38399.pbf
--rw-r--r--   0        0        0       41 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/3840-4095.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/38400-38655.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/38656-38911.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/38912-39167.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/39168-39423.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/39424-39679.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/39680-39935.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/39936-40191.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/40192-40447.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/40448-40703.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/40704-40959.pbf
--rw-r--r--   0        0        0       41 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/4096-4351.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/40960-41215.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/41216-41471.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/41472-41727.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/41728-41983.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/41984-42239.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/42240-42495.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/42496-42751.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/42752-43007.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/43008-43263.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/43264-43519.pbf
--rw-r--r--   0        0        0       41 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/4352-4607.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/43520-43775.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/43776-44031.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/44032-44287.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/44288-44543.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/44544-44799.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/44800-45055.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/45056-45311.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/45312-45567.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/45568-45823.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/45824-46079.pbf
--rw-r--r--   0        0        0       41 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/4608-4863.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/46080-46335.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/46336-46591.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/46592-46847.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/46848-47103.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/47104-47359.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/47360-47615.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/47616-47871.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/47872-48127.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/48128-48383.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/48384-48639.pbf
--rw-r--r--   0        0        0       41 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/4864-5119.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/48640-48895.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/48896-49151.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/49152-49407.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/49408-49663.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/49664-49919.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/49920-50175.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/50176-50431.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/50432-50687.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/50688-50943.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/50944-51199.pbf
--rw-r--r--   0        0        0     4308 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/512-767.pbf
--rw-r--r--   0        0        0       41 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/5120-5375.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/51200-51455.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/51456-51711.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/51712-51967.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/51968-52223.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/52224-52479.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/52480-52735.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/52736-52991.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/52992-53247.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/53248-53503.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/53504-53759.pbf
--rw-r--r--   0        0        0       41 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/5376-5631.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/53760-54015.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/54016-54271.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/54272-54527.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/54528-54783.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/54784-55039.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/55040-55295.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/55296-55551.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/55552-55807.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/55808-56063.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/56064-56319.pbf
--rw-r--r--   0        0        0       41 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/5632-5887.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/56320-56575.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/56576-56831.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/56832-57087.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/57088-57343.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/57344-57599.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/57600-57855.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/57856-58111.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/58112-58367.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/58368-58623.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/58624-58879.pbf
--rw-r--r--   0        0        0       41 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/5888-6143.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/58880-59135.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/59136-59391.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/59392-59647.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/59648-59903.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/59904-60159.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/60160-60415.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/60416-60671.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/60672-60927.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/60928-61183.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/61184-61439.pbf
--rw-r--r--   0        0        0       41 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/6144-6399.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/61440-61695.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/61696-61951.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/61952-62207.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/62208-62463.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/62464-62719.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/62720-62975.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/62976-63231.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/63232-63487.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/63488-63743.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/63744-63999.pbf
--rw-r--r--   0        0        0       41 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/6400-6655.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/64000-64255.pbf
--rw-r--r--   0        0        0     4765 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/64256-64511.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/64512-64767.pbf
--rw-r--r--   0        0        0       43 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/64768-65023.pbf
--rw-r--r--   0        0        0       59 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/65024-65279.pbf
--rw-r--r--   0        0        0     1652 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/65280-65535.pbf
--rw-r--r--   0        0        0       41 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/6656-6911.pbf
--rw-r--r--   0        0        0       41 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/6912-7167.pbf
--rw-r--r--   0        0        0       41 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/7168-7423.pbf
--rw-r--r--   0        0        0       41 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/7424-7679.pbf
--rw-r--r--   0        0        0    38925 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/768-1023.pbf
--rw-r--r--   0        0        0    64829 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/7680-7935.pbf
--rw-r--r--   0        0        0      705 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/7936-8191.pbf
--rw-r--r--   0        0        0    11556 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/8192-8447.pbf
--rw-r--r--   0        0        0     5865 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/8448-8703.pbf
--rw-r--r--   0        0        0     5292 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/8704-8959.pbf
--rw-r--r--   0        0        0       41 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/8960-9215.pbf
--rw-r--r--   0        0        0       41 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/9216-9471.pbf
--rw-r--r--   0        0        0      475 2022-12-03 11:51:47.340652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/9472-9727.pbf
--rw-r--r--   0        0        0       41 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/9728-9983.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.344652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/9984-10239.pbf
--rw-r--r--   0        0        0    78054 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/0-255.pbf
--rw-r--r--   0        0        0   125040 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/1024-1279.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/10240-10495.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/10496-10751.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/10752-11007.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/11008-11263.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/11264-11519.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/11520-11775.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/11776-12031.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/12032-12287.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/12288-12543.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/12544-12799.pbf
--rw-r--r--   0        0        0     9668 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/1280-1535.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/12800-13055.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/13056-13311.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/13312-13567.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/13568-13823.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/13824-14079.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/14080-14335.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/14336-14591.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/14592-14847.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/14848-15103.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/15104-15359.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/1536-1791.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/15360-15615.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/15616-15871.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/15872-16127.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/16128-16383.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/16384-16639.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/16640-16895.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/16896-17151.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/17152-17407.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/17408-17663.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/17664-17919.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/1792-2047.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/17920-18175.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/18176-18431.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/18432-18687.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/18688-18943.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/18944-19199.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/19200-19455.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/19456-19711.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/19712-19967.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/19968-20223.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/20224-20479.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/2048-2303.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/20480-20735.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/20736-20991.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/20992-21247.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/21248-21503.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/21504-21759.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/21760-22015.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/22016-22271.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/22272-22527.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/22528-22783.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/22784-23039.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/2304-2559.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/23040-23295.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/23296-23551.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/23552-23807.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/23808-24063.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/24064-24319.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/24320-24575.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/24576-24831.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/24832-25087.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/25088-25343.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/25344-25599.pbf
--rw-r--r--   0        0        0    69941 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/256-511.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/2560-2815.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/25600-25855.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/25856-26111.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/26112-26367.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/26368-26623.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/26624-26879.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/26880-27135.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/27136-27391.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/27392-27647.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/27648-27903.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/27904-28159.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/2816-3071.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/28160-28415.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/28416-28671.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/28672-28927.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/28928-29183.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/29184-29439.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/29440-29695.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/29696-29951.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/29952-30207.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/30208-30463.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/30464-30719.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/3072-3327.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/30720-30975.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/30976-31231.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/31232-31487.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/31488-31743.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/31744-31999.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/32000-32255.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/32256-32511.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/32512-32767.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/32768-33023.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/33024-33279.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/3328-3583.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/33280-33535.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/33536-33791.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/33792-34047.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/34048-34303.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/34304-34559.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.352652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/34560-34815.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/34816-35071.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/35072-35327.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/35328-35583.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/35584-35839.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/3584-3839.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/35840-36095.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/36096-36351.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/36352-36607.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/36608-36863.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/36864-37119.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/37120-37375.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/37376-37631.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/37632-37887.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/37888-38143.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/38144-38399.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/3840-4095.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/38400-38655.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/38656-38911.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/38912-39167.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/39168-39423.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/39424-39679.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/39680-39935.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/39936-40191.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/40192-40447.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/40448-40703.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/40704-40959.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/4096-4351.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/40960-41215.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/41216-41471.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/41472-41727.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/41728-41983.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/41984-42239.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/42240-42495.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/42496-42751.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/42752-43007.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/43008-43263.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/43264-43519.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/4352-4607.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/43520-43775.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/43776-44031.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/44032-44287.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/44288-44543.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/44544-44799.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/44800-45055.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/45056-45311.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/45312-45567.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/45568-45823.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/45824-46079.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/4608-4863.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/46080-46335.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/46336-46591.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/46592-46847.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/46848-47103.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/47104-47359.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/47360-47615.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/47616-47871.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/47872-48127.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/48128-48383.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/48384-48639.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/4864-5119.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/48640-48895.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/48896-49151.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/49152-49407.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/49408-49663.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/49664-49919.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/49920-50175.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/50176-50431.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/50432-50687.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/50688-50943.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/50944-51199.pbf
--rw-r--r--   0        0        0     3712 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/512-767.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/5120-5375.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/51200-51455.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/51456-51711.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/51712-51967.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/51968-52223.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/52224-52479.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/52480-52735.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/52736-52991.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/52992-53247.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/53248-53503.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/53504-53759.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/5376-5631.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/53760-54015.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/54016-54271.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/54272-54527.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/54528-54783.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/54784-55039.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/55040-55295.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/55296-55551.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/55552-55807.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/55808-56063.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/56064-56319.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/5632-5887.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/56320-56575.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/56576-56831.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/56832-57087.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/57088-57343.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/57344-57599.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/57600-57855.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/57856-58111.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/58112-58367.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/58368-58623.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/58624-58879.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/5888-6143.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/58880-59135.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/59136-59391.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/59392-59647.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/59648-59903.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/59904-60159.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/60160-60415.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/60416-60671.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/60672-60927.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/60928-61183.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/61184-61439.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/6144-6399.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/61440-61695.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/61696-61951.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/61952-62207.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/62208-62463.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/62464-62719.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/62720-62975.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/62976-63231.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/63232-63487.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/63488-63743.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/63744-63999.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/6400-6655.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/64000-64255.pbf
--rw-r--r--   0        0        0     4214 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/64256-64511.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/64512-64767.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/64768-65023.pbf
--rw-r--r--   0        0        0       49 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/65024-65279.pbf
--rw-r--r--   0        0        0     1642 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/65280-65535.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/6656-6911.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/6912-7167.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/7168-7423.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/7424-7679.pbf
--rw-r--r--   0        0        0    34219 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/768-1023.pbf
--rw-r--r--   0        0        0    57224 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/7680-7935.pbf
--rw-r--r--   0        0        0      626 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/7936-8191.pbf
--rw-r--r--   0        0        0    10083 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/8192-8447.pbf
--rw-r--r--   0        0        0     5275 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/8448-8703.pbf
--rw-r--r--   0        0        0     4845 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/8704-8959.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/8960-9215.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/9216-9471.pbf
--rw-r--r--   0        0        0      442 2022-12-03 11:51:47.356652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/9472-9727.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/9728-9983.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/9984-10239.pbf
--rw-r--r--   0        0        0    72370 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/0-255.pbf
--rw-r--r--   0        0        0   117993 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/1024-1279.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/10240-10495.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/10496-10751.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/10752-11007.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/11008-11263.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/11264-11519.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/11520-11775.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/11776-12031.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/12032-12287.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/12288-12543.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/12544-12799.pbf
--rw-r--r--   0        0        0     9508 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/1280-1535.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/12800-13055.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/13056-13311.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/13312-13567.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/13568-13823.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/13824-14079.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/14080-14335.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/14336-14591.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/14592-14847.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/14848-15103.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/15104-15359.pbf
--rw-r--r--   0        0        0       30 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/1536-1791.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/15360-15615.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/15616-15871.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/15872-16127.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/16128-16383.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/16384-16639.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/16640-16895.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/16896-17151.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/17152-17407.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/17408-17663.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/17664-17919.pbf
--rw-r--r--   0        0        0       30 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/1792-2047.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/17920-18175.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/18176-18431.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/18432-18687.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/18688-18943.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/18944-19199.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/19200-19455.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/19456-19711.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/19712-19967.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/19968-20223.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/20224-20479.pbf
--rw-r--r--   0        0        0       30 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/2048-2303.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/20480-20735.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/20736-20991.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/20992-21247.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/21248-21503.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/21504-21759.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/21760-22015.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/22016-22271.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/22272-22527.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/22528-22783.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/22784-23039.pbf
--rw-r--r--   0        0        0       30 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/2304-2559.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/23040-23295.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/23296-23551.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/23552-23807.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/23808-24063.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/24064-24319.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/24320-24575.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/24576-24831.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/24832-25087.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/25088-25343.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/25344-25599.pbf
--rw-r--r--   0        0        0    63678 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/256-511.pbf
--rw-r--r--   0        0        0       30 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/2560-2815.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/25600-25855.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/25856-26111.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/26112-26367.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/26368-26623.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/26624-26879.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/26880-27135.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/27136-27391.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/27392-27647.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/27648-27903.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/27904-28159.pbf
--rw-r--r--   0        0        0       30 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/2816-3071.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/28160-28415.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/28416-28671.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/28672-28927.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/28928-29183.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/29184-29439.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/29440-29695.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/29696-29951.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/29952-30207.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/30208-30463.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/30464-30719.pbf
--rw-r--r--   0        0        0       30 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/3072-3327.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/30720-30975.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/30976-31231.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/31232-31487.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/31488-31743.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/31744-31999.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/32000-32255.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/32256-32511.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/32512-32767.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/32768-33023.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/33024-33279.pbf
--rw-r--r--   0        0        0       30 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/3328-3583.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/33280-33535.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/33536-33791.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/33792-34047.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/34048-34303.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/34304-34559.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/34560-34815.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/34816-35071.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/35072-35327.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/35328-35583.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/35584-35839.pbf
--rw-r--r--   0        0        0       30 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/3584-3839.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/35840-36095.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/36096-36351.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/36352-36607.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/36608-36863.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/36864-37119.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/37120-37375.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/37376-37631.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/37632-37887.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/37888-38143.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/38144-38399.pbf
--rw-r--r--   0        0        0       30 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/3840-4095.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/38400-38655.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/38656-38911.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/38912-39167.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.368652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/39168-39423.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/39424-39679.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/39680-39935.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/39936-40191.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/40192-40447.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/40448-40703.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/40704-40959.pbf
--rw-r--r--   0        0        0       30 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/4096-4351.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/40960-41215.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/41216-41471.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/41472-41727.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/41728-41983.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/41984-42239.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/42240-42495.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/42496-42751.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/42752-43007.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/43008-43263.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/43264-43519.pbf
--rw-r--r--   0        0        0       30 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/4352-4607.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/43520-43775.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/43776-44031.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/44032-44287.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/44288-44543.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/44544-44799.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/44800-45055.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/45056-45311.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/45312-45567.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/45568-45823.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/45824-46079.pbf
--rw-r--r--   0        0        0       30 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/4608-4863.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/46080-46335.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/46336-46591.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/46592-46847.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/46848-47103.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/47104-47359.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/47360-47615.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/47616-47871.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/47872-48127.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/48128-48383.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/48384-48639.pbf
--rw-r--r--   0        0        0       30 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/4864-5119.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/48640-48895.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/48896-49151.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/49152-49407.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/49408-49663.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/49664-49919.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/49920-50175.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/50176-50431.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/50432-50687.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/50688-50943.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/50944-51199.pbf
--rw-r--r--   0        0        0     3430 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/512-767.pbf
--rw-r--r--   0        0        0       30 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/5120-5375.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/51200-51455.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/51456-51711.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/51712-51967.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/51968-52223.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/52224-52479.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/52480-52735.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/52736-52991.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/52992-53247.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/53248-53503.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/53504-53759.pbf
--rw-r--r--   0        0        0       30 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/5376-5631.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/53760-54015.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/54016-54271.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/54272-54527.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/54528-54783.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/54784-55039.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/55040-55295.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/55296-55551.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/55552-55807.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/55808-56063.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/56064-56319.pbf
--rw-r--r--   0        0        0       30 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/5632-5887.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/56320-56575.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/56576-56831.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/56832-57087.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/57088-57343.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/57344-57599.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/57600-57855.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/57856-58111.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/58112-58367.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/58368-58623.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/58624-58879.pbf
--rw-r--r--   0        0        0       30 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/5888-6143.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/58880-59135.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/59136-59391.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/59392-59647.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/59648-59903.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/59904-60159.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/60160-60415.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/60416-60671.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/60672-60927.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/60928-61183.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/61184-61439.pbf
--rw-r--r--   0        0        0       30 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/6144-6399.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/61440-61695.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/61696-61951.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/61952-62207.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/62208-62463.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/62464-62719.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/62720-62975.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/62976-63231.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/63232-63487.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/63488-63743.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/63744-63999.pbf
--rw-r--r--   0        0        0       30 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/6400-6655.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/64000-64255.pbf
--rw-r--r--   0        0        0     2533 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/64256-64511.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/64512-64767.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/64768-65023.pbf
--rw-r--r--   0        0        0       48 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/65024-65279.pbf
--rw-r--r--   0        0        0     1641 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/65280-65535.pbf
--rw-r--r--   0        0        0       30 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/6656-6911.pbf
--rw-r--r--   0        0        0       30 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/6912-7167.pbf
--rw-r--r--   0        0        0       30 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/7168-7423.pbf
--rw-r--r--   0        0        0       30 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/7424-7679.pbf
--rw-r--r--   0        0        0    32916 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/768-1023.pbf
--rw-r--r--   0        0        0    52825 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/7680-7935.pbf
--rw-r--r--   0        0        0      671 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/7936-8191.pbf
--rw-r--r--   0        0        0     9151 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/8192-8447.pbf
--rw-r--r--   0        0        0     5214 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/8448-8703.pbf
--rw-r--r--   0        0        0     4731 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/8704-8959.pbf
--rw-r--r--   0        0        0       30 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/8960-9215.pbf
--rw-r--r--   0        0        0       30 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/9216-9471.pbf
--rw-r--r--   0        0        0      464 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/9472-9727.pbf
--rw-r--r--   0        0        0       30 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/9728-9983.pbf
--rw-r--r--   0        0        0       31 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/9984-10239.pbf
--rw-r--r--   0        0        0    75722 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/0-255.pbf
--rw-r--r--   0        0        0   121649 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/1024-1279.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/10240-10495.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/10496-10751.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/10752-11007.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/11008-11263.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/11264-11519.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/11520-11775.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/11776-12031.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/12032-12287.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/12288-12543.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/12544-12799.pbf
--rw-r--r--   0        0        0     9260 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/1280-1535.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/12800-13055.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/13056-13311.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/13312-13567.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/13568-13823.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/13824-14079.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/14080-14335.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/14336-14591.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/14592-14847.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/14848-15103.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/15104-15359.pbf
--rw-r--r--   0        0        0       37 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/1536-1791.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/15360-15615.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/15616-15871.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/15872-16127.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/16128-16383.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/16384-16639.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/16640-16895.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/16896-17151.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/17152-17407.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/17408-17663.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/17664-17919.pbf
--rw-r--r--   0        0        0       37 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/1792-2047.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/17920-18175.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/18176-18431.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/18432-18687.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/18688-18943.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/18944-19199.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/19200-19455.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/19456-19711.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/19712-19967.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/19968-20223.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/20224-20479.pbf
--rw-r--r--   0        0        0       37 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/2048-2303.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/20480-20735.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/20736-20991.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/20992-21247.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/21248-21503.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/21504-21759.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/21760-22015.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/22016-22271.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/22272-22527.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/22528-22783.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/22784-23039.pbf
--rw-r--r--   0        0        0       37 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/2304-2559.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/23040-23295.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/23296-23551.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/23552-23807.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/23808-24063.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/24064-24319.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/24320-24575.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/24576-24831.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/24832-25087.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/25088-25343.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/25344-25599.pbf
--rw-r--r--   0        0        0    68072 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/256-511.pbf
--rw-r--r--   0        0        0       37 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/2560-2815.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/25600-25855.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/25856-26111.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/26112-26367.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/26368-26623.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/26624-26879.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/26880-27135.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/27136-27391.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/27392-27647.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/27648-27903.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/27904-28159.pbf
--rw-r--r--   0        0        0       37 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/2816-3071.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/28160-28415.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/28416-28671.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/28672-28927.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/28928-29183.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/29184-29439.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/29440-29695.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/29696-29951.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/29952-30207.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/30208-30463.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/30464-30719.pbf
--rw-r--r--   0        0        0       37 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/3072-3327.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/30720-30975.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/30976-31231.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/31232-31487.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/31488-31743.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/31744-31999.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/32000-32255.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/32256-32511.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/32512-32767.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/32768-33023.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/33024-33279.pbf
--rw-r--r--   0        0        0       37 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/3328-3583.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/33280-33535.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/33536-33791.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/33792-34047.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/34048-34303.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/34304-34559.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/34560-34815.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/34816-35071.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/35072-35327.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/35328-35583.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/35584-35839.pbf
--rw-r--r--   0        0        0       37 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/3584-3839.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/35840-36095.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.360652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/36096-36351.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/36352-36607.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/36608-36863.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/36864-37119.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/37120-37375.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/37376-37631.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/37632-37887.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/37888-38143.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/38144-38399.pbf
--rw-r--r--   0        0        0       37 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/3840-4095.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/38400-38655.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/38656-38911.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/38912-39167.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/39168-39423.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/39424-39679.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/39680-39935.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/39936-40191.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/40192-40447.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/40448-40703.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/40704-40959.pbf
--rw-r--r--   0        0        0       37 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/4096-4351.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/40960-41215.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/41216-41471.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/41472-41727.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/41728-41983.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/41984-42239.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/42240-42495.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/42496-42751.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/42752-43007.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/43008-43263.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/43264-43519.pbf
--rw-r--r--   0        0        0       37 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/4352-4607.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/43520-43775.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/43776-44031.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/44032-44287.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/44288-44543.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/44544-44799.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/44800-45055.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/45056-45311.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/45312-45567.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/45568-45823.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/45824-46079.pbf
--rw-r--r--   0        0        0       37 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/4608-4863.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/46080-46335.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/46336-46591.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/46592-46847.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/46848-47103.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/47104-47359.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/47360-47615.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/47616-47871.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/47872-48127.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/48128-48383.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/48384-48639.pbf
--rw-r--r--   0        0        0       37 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/4864-5119.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/48640-48895.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/48896-49151.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/49152-49407.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/49408-49663.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/49664-49919.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/49920-50175.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/50176-50431.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/50432-50687.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/50688-50943.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/50944-51199.pbf
--rw-r--r--   0        0        0     3555 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/512-767.pbf
--rw-r--r--   0        0        0       37 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/5120-5375.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/51200-51455.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/51456-51711.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/51712-51967.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/51968-52223.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/52224-52479.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/52480-52735.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/52736-52991.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/52992-53247.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/53248-53503.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/53504-53759.pbf
--rw-r--r--   0        0        0       37 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/5376-5631.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/53760-54015.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/54016-54271.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/54272-54527.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/54528-54783.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/54784-55039.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/55040-55295.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/55296-55551.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/55552-55807.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/55808-56063.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/56064-56319.pbf
--rw-r--r--   0        0        0       37 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/5632-5887.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/56320-56575.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/56576-56831.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/56832-57087.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/57088-57343.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/57344-57599.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/57600-57855.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/57856-58111.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/58112-58367.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/58368-58623.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/58624-58879.pbf
--rw-r--r--   0        0        0       37 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/5888-6143.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/58880-59135.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/59136-59391.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/59392-59647.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/59648-59903.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/59904-60159.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/60160-60415.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/60416-60671.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/60672-60927.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/60928-61183.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/61184-61439.pbf
--rw-r--r--   0        0        0       37 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/6144-6399.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/61440-61695.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/61696-61951.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/61952-62207.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/62208-62463.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/62464-62719.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/62720-62975.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/62976-63231.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/63232-63487.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/63488-63743.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/63744-63999.pbf
--rw-r--r--   0        0        0       37 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/6400-6655.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/64000-64255.pbf
--rw-r--r--   0        0        0     3920 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/64256-64511.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/64512-64767.pbf
--rw-r--r--   0        0        0       39 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/64768-65023.pbf
--rw-r--r--   0        0        0       55 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/65024-65279.pbf
--rw-r--r--   0        0        0     1648 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/65280-65535.pbf
--rw-r--r--   0        0        0       37 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/6656-6911.pbf
--rw-r--r--   0        0        0       37 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/6912-7167.pbf
--rw-r--r--   0        0        0       37 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/7168-7423.pbf
--rw-r--r--   0        0        0       37 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/7424-7679.pbf
--rw-r--r--   0        0        0    33074 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/768-1023.pbf
--rw-r--r--   0        0        0    55285 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/7680-7935.pbf
--rw-r--r--   0        0        0      632 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/7936-8191.pbf
--rw-r--r--   0        0        0     9699 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/8192-8447.pbf
--rw-r--r--   0        0        0     5124 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/8448-8703.pbf
--rw-r--r--   0        0        0     4751 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/8704-8959.pbf
--rw-r--r--   0        0        0       37 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/8960-9215.pbf
--rw-r--r--   0        0        0       37 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/9216-9471.pbf
--rw-r--r--   0        0        0      471 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/9472-9727.pbf
--rw-r--r--   0        0        0       37 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/9728-9983.pbf
--rw-r--r--   0        0        0       38 2022-12-03 11:51:47.364652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/9984-10239.pbf
--rw-r--r--   0        0        0    74696 2022-12-03 11:51:47.372652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/0-255.pbf
--rw-r--r--   0        0        0   122545 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/1024-1279.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/10240-10495.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/10496-10751.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/10752-11007.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/11008-11263.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/11264-11519.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/11520-11775.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/11776-12031.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/12032-12287.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/12288-12543.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/12544-12799.pbf
--rw-r--r--   0        0        0     9913 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/1280-1535.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/12800-13055.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/13056-13311.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/13312-13567.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/13568-13823.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/13824-14079.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/14080-14335.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/14336-14591.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/14592-14847.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/14848-15103.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/15104-15359.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/1536-1791.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/15360-15615.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/15616-15871.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/15872-16127.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/16128-16383.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/16384-16639.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/16640-16895.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/16896-17151.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/17152-17407.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/17408-17663.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/17664-17919.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/1792-2047.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/17920-18175.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/18176-18431.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/18432-18687.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/18688-18943.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/18944-19199.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/19200-19455.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/19456-19711.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/19712-19967.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/19968-20223.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/20224-20479.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/2048-2303.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/20480-20735.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/20736-20991.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/20992-21247.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/21248-21503.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/21504-21759.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/21760-22015.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/22016-22271.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/22272-22527.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/22528-22783.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/22784-23039.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/2304-2559.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/23040-23295.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/23296-23551.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/23552-23807.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/23808-24063.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/24064-24319.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/24320-24575.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/24576-24831.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/24832-25087.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/25088-25343.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/25344-25599.pbf
--rw-r--r--   0        0        0    66481 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/256-511.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/2560-2815.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/25600-25855.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/25856-26111.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/26112-26367.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/26368-26623.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/26624-26879.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/26880-27135.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/27136-27391.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/27392-27647.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/27648-27903.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/27904-28159.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/2816-3071.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/28160-28415.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/28416-28671.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/28672-28927.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/28928-29183.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/29184-29439.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/29440-29695.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/29696-29951.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/29952-30207.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/30208-30463.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/30464-30719.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/3072-3327.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/30720-30975.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/30976-31231.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/31232-31487.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/31488-31743.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/31744-31999.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/32000-32255.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/32256-32511.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/32512-32767.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/32768-33023.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/33024-33279.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/3328-3583.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/33280-33535.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/33536-33791.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/33792-34047.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/34048-34303.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/34304-34559.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/34560-34815.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/34816-35071.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/35072-35327.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/35328-35583.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/35584-35839.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/3584-3839.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/35840-36095.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/36096-36351.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/36352-36607.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/36608-36863.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/36864-37119.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/37120-37375.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/37376-37631.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/37632-37887.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/37888-38143.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/38144-38399.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/3840-4095.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/38400-38655.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/38656-38911.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/38912-39167.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/39168-39423.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/39424-39679.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/39680-39935.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/39936-40191.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/40192-40447.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/40448-40703.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/40704-40959.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/4096-4351.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/40960-41215.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/41216-41471.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/41472-41727.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/41728-41983.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.376652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/41984-42239.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/42240-42495.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/42496-42751.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/42752-43007.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/43008-43263.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/43264-43519.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/4352-4607.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/43520-43775.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/43776-44031.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/44032-44287.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/44288-44543.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/44544-44799.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/44800-45055.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/45056-45311.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/45312-45567.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/45568-45823.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/45824-46079.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/4608-4863.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/46080-46335.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/46336-46591.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/46592-46847.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/46848-47103.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/47104-47359.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/47360-47615.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/47616-47871.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/47872-48127.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/48128-48383.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/48384-48639.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/4864-5119.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/48640-48895.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/48896-49151.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/49152-49407.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/49408-49663.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/49664-49919.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/49920-50175.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/50176-50431.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/50432-50687.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/50688-50943.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/50944-51199.pbf
--rw-r--r--   0        0        0     3653 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/512-767.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/5120-5375.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/51200-51455.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/51456-51711.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/51712-51967.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/51968-52223.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/52224-52479.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/52480-52735.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/52736-52991.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/52992-53247.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/53248-53503.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/53504-53759.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/5376-5631.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/53760-54015.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/54016-54271.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/54272-54527.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/54528-54783.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/54784-55039.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/55040-55295.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/55296-55551.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/55552-55807.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/55808-56063.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/56064-56319.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/5632-5887.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/56320-56575.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/56576-56831.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/56832-57087.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/57088-57343.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/57344-57599.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/57600-57855.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/57856-58111.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/58112-58367.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/58368-58623.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/58624-58879.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/5888-6143.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/58880-59135.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/59136-59391.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/59392-59647.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/59648-59903.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/59904-60159.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/60160-60415.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/60416-60671.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/60672-60927.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/60928-61183.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/61184-61439.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/6144-6399.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/61440-61695.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/61696-61951.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/61952-62207.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/62208-62463.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/62464-62719.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/62720-62975.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/62976-63231.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/63232-63487.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/63488-63743.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/63744-63999.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/6400-6655.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/64000-64255.pbf
--rw-r--r--   0        0        0     2799 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/64256-64511.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/64512-64767.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/64768-65023.pbf
--rw-r--r--   0        0        0       50 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/65024-65279.pbf
--rw-r--r--   0        0        0     1643 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/65280-65535.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/6656-6911.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/6912-7167.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/7168-7423.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/7424-7679.pbf
--rw-r--r--   0        0        0    33767 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/768-1023.pbf
--rw-r--r--   0        0        0    55070 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/7680-7935.pbf
--rw-r--r--   0        0        0      650 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/7936-8191.pbf
--rw-r--r--   0        0        0     9663 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/8192-8447.pbf
--rw-r--r--   0        0        0     5373 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/8448-8703.pbf
--rw-r--r--   0        0        0     4875 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/8704-8959.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/8960-9215.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/9216-9471.pbf
--rw-r--r--   0        0        0      466 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/9472-9727.pbf
--rw-r--r--   0        0        0       32 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/9728-9983.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/9984-10239.pbf
--rw-r--r--   0        0        0    77571 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/0-255.pbf
--rw-r--r--   0        0        0   128493 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/1024-1279.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/10240-10495.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/10496-10751.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/10752-11007.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/11008-11263.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/11264-11519.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/11520-11775.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/11776-12031.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/12032-12287.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/12288-12543.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/12544-12799.pbf
--rw-r--r--   0        0        0    10358 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/1280-1535.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/12800-13055.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/13056-13311.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/13312-13567.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/13568-13823.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/13824-14079.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/14080-14335.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/14336-14591.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/14592-14847.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/14848-15103.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/15104-15359.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/1536-1791.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/15360-15615.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/15616-15871.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/15872-16127.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/16128-16383.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/16384-16639.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/16640-16895.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/16896-17151.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/17152-17407.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/17408-17663.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/17664-17919.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/1792-2047.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/17920-18175.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/18176-18431.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/18432-18687.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/18688-18943.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/18944-19199.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/19200-19455.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/19456-19711.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/19712-19967.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/19968-20223.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/20224-20479.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/2048-2303.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/20480-20735.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/20736-20991.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/20992-21247.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/21248-21503.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/21504-21759.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/21760-22015.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/22016-22271.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/22272-22527.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/22528-22783.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/22784-23039.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/2304-2559.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/23040-23295.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/23296-23551.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/23552-23807.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/23808-24063.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/24064-24319.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/24320-24575.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/24576-24831.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/24832-25087.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/25088-25343.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/25344-25599.pbf
--rw-r--r--   0        0        0    68869 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/256-511.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/2560-2815.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/25600-25855.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/25856-26111.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/26112-26367.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/26368-26623.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/26624-26879.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/26880-27135.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/27136-27391.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/27392-27647.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/27648-27903.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/27904-28159.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/2816-3071.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/28160-28415.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/28416-28671.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/28672-28927.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/28928-29183.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/29184-29439.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/29440-29695.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/29696-29951.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/29952-30207.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/30208-30463.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/30464-30719.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/3072-3327.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/30720-30975.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/30976-31231.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/31232-31487.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/31488-31743.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/31744-31999.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/32000-32255.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/32256-32511.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/32512-32767.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/32768-33023.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/33024-33279.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/3328-3583.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/33280-33535.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/33536-33791.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/33792-34047.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/34048-34303.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/34304-34559.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/34560-34815.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/34816-35071.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/35072-35327.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/35328-35583.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/35584-35839.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/3584-3839.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/35840-36095.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/36096-36351.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/36352-36607.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/36608-36863.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/36864-37119.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/37120-37375.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/37376-37631.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/37632-37887.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/37888-38143.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/38144-38399.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/3840-4095.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/38400-38655.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/38656-38911.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/38912-39167.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/39168-39423.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/39424-39679.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/39680-39935.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/39936-40191.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/40192-40447.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/40448-40703.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/40704-40959.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/4096-4351.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/40960-41215.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/41216-41471.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/41472-41727.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/41728-41983.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/41984-42239.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/42240-42495.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/42496-42751.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/42752-43007.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/43008-43263.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/43264-43519.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.392652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/4352-4607.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/43520-43775.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/43776-44031.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/44032-44287.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/44288-44543.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/44544-44799.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/44800-45055.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/45056-45311.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/45312-45567.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/45568-45823.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/45824-46079.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/4608-4863.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/46080-46335.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/46336-46591.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/46592-46847.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/46848-47103.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/47104-47359.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/47360-47615.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/47616-47871.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/47872-48127.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/48128-48383.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/48384-48639.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/4864-5119.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/48640-48895.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/48896-49151.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/49152-49407.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/49408-49663.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/49664-49919.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/49920-50175.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/50176-50431.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/50432-50687.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/50688-50943.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/50944-51199.pbf
--rw-r--r--   0        0        0     3823 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/512-767.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/5120-5375.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/51200-51455.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/51456-51711.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/51712-51967.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/51968-52223.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/52224-52479.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/52480-52735.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/52736-52991.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/52992-53247.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/53248-53503.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/53504-53759.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/5376-5631.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/53760-54015.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/54016-54271.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/54272-54527.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/54528-54783.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/54784-55039.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/55040-55295.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/55296-55551.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/55552-55807.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/55808-56063.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/56064-56319.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/5632-5887.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/56320-56575.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/56576-56831.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/56832-57087.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/57088-57343.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/57344-57599.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/57600-57855.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/57856-58111.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/58112-58367.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/58368-58623.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/58624-58879.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/5888-6143.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/58880-59135.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/59136-59391.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/59392-59647.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/59648-59903.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/59904-60159.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/60160-60415.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/60416-60671.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/60672-60927.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/60928-61183.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/61184-61439.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/6144-6399.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/61440-61695.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/61696-61951.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/61952-62207.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/62208-62463.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/62464-62719.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/62720-62975.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/62976-63231.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/63232-63487.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/63488-63743.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/63744-63999.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/6400-6655.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/64000-64255.pbf
--rw-r--r--   0        0        0     3040 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/64256-64511.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/64512-64767.pbf
--rw-r--r--   0        0        0       35 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/64768-65023.pbf
--rw-r--r--   0        0        0       51 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/65024-65279.pbf
--rw-r--r--   0        0        0     1644 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/65280-65535.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/6656-6911.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/6912-7167.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/7168-7423.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/7424-7679.pbf
--rw-r--r--   0        0        0    35063 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/768-1023.pbf
--rw-r--r--   0        0        0    57819 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/7680-7935.pbf
--rw-r--r--   0        0        0      697 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/7936-8191.pbf
--rw-r--r--   0        0        0    10092 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/8192-8447.pbf
--rw-r--r--   0        0        0     5512 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/8448-8703.pbf
--rw-r--r--   0        0        0     5072 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/8704-8959.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/8960-9215.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/9216-9471.pbf
--rw-r--r--   0        0        0      467 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/9472-9727.pbf
--rw-r--r--   0        0        0       33 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/9728-9983.pbf
--rw-r--r--   0        0        0       34 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/9984-10239.pbf
--rw-r--r--   0        0        0    80678 2022-12-03 11:51:47.380652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/0-255.pbf
--rw-r--r--   0        0        0   130485 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/1024-1279.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/10240-10495.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/10496-10751.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/10752-11007.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/11008-11263.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/11264-11519.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/11520-11775.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/11776-12031.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/12032-12287.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/12288-12543.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/12544-12799.pbf
--rw-r--r--   0        0        0     9992 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/1280-1535.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/12800-13055.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/13056-13311.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/13312-13567.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/13568-13823.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/13824-14079.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/14080-14335.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/14336-14591.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/14592-14847.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/14848-15103.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/15104-15359.pbf
--rw-r--r--   0        0        0       40 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/1536-1791.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/15360-15615.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/15616-15871.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/15872-16127.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/16128-16383.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/16384-16639.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/16640-16895.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/16896-17151.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/17152-17407.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/17408-17663.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/17664-17919.pbf
--rw-r--r--   0        0        0       40 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/1792-2047.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/17920-18175.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/18176-18431.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/18432-18687.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/18688-18943.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/18944-19199.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/19200-19455.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/19456-19711.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/19712-19967.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/19968-20223.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/20224-20479.pbf
--rw-r--r--   0        0        0       40 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/2048-2303.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/20480-20735.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/20736-20991.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/20992-21247.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/21248-21503.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/21504-21759.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/21760-22015.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/22016-22271.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/22272-22527.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/22528-22783.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/22784-23039.pbf
--rw-r--r--   0        0        0       40 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/2304-2559.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/23040-23295.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/23296-23551.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/23552-23807.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/23808-24063.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/24064-24319.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/24320-24575.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/24576-24831.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/24832-25087.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/25088-25343.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/25344-25599.pbf
--rw-r--r--   0        0        0    72562 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/256-511.pbf
--rw-r--r--   0        0        0       40 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/2560-2815.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/25600-25855.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/25856-26111.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/26112-26367.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/26368-26623.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/26624-26879.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/26880-27135.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/27136-27391.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/27392-27647.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/27648-27903.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/27904-28159.pbf
--rw-r--r--   0        0        0       40 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/2816-3071.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/28160-28415.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/28416-28671.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/28672-28927.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/28928-29183.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/29184-29439.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/29440-29695.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/29696-29951.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/29952-30207.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/30208-30463.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/30464-30719.pbf
--rw-r--r--   0        0        0       40 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/3072-3327.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/30720-30975.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/30976-31231.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/31232-31487.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/31488-31743.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/31744-31999.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/32000-32255.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/32256-32511.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/32512-32767.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/32768-33023.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/33024-33279.pbf
--rw-r--r--   0        0        0       40 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/3328-3583.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/33280-33535.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/33536-33791.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/33792-34047.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/34048-34303.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/34304-34559.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/34560-34815.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/34816-35071.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/35072-35327.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/35328-35583.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/35584-35839.pbf
--rw-r--r--   0        0        0       40 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/3584-3839.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/35840-36095.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/36096-36351.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/36352-36607.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/36608-36863.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/36864-37119.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/37120-37375.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/37376-37631.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/37632-37887.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/37888-38143.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/38144-38399.pbf
--rw-r--r--   0        0        0       40 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/3840-4095.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/38400-38655.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/38656-38911.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/38912-39167.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/39168-39423.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/39424-39679.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/39680-39935.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/39936-40191.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/40192-40447.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/40448-40703.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/40704-40959.pbf
--rw-r--r--   0        0        0       40 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/4096-4351.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/40960-41215.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/41216-41471.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/41472-41727.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/41728-41983.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/41984-42239.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/42240-42495.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/42496-42751.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.384652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/42752-43007.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/43008-43263.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/43264-43519.pbf
--rw-r--r--   0        0        0       40 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/4352-4607.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/43520-43775.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/43776-44031.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/44032-44287.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/44288-44543.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/44544-44799.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/44800-45055.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/45056-45311.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/45312-45567.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/45568-45823.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/45824-46079.pbf
--rw-r--r--   0        0        0       40 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/4608-4863.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/46080-46335.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/46336-46591.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/46592-46847.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/46848-47103.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/47104-47359.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/47360-47615.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/47616-47871.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/47872-48127.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/48128-48383.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/48384-48639.pbf
--rw-r--r--   0        0        0       40 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/4864-5119.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/48640-48895.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/48896-49151.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/49152-49407.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/49408-49663.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/49664-49919.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/49920-50175.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/50176-50431.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/50432-50687.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/50688-50943.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/50944-51199.pbf
--rw-r--r--   0        0        0     3901 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/512-767.pbf
--rw-r--r--   0        0        0       40 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/5120-5375.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/51200-51455.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/51456-51711.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/51712-51967.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/51968-52223.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/52224-52479.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/52480-52735.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/52736-52991.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/52992-53247.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/53248-53503.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/53504-53759.pbf
--rw-r--r--   0        0        0       40 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/5376-5631.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/53760-54015.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/54016-54271.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/54272-54527.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/54528-54783.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/54784-55039.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/55040-55295.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/55296-55551.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/55552-55807.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/55808-56063.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/56064-56319.pbf
--rw-r--r--   0        0        0       40 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/5632-5887.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/56320-56575.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/56576-56831.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/56832-57087.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/57088-57343.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/57344-57599.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/57600-57855.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/57856-58111.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/58112-58367.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/58368-58623.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/58624-58879.pbf
--rw-r--r--   0        0        0       40 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/5888-6143.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/58880-59135.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/59136-59391.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/59392-59647.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/59648-59903.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/59904-60159.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/60160-60415.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/60416-60671.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/60672-60927.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/60928-61183.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/61184-61439.pbf
--rw-r--r--   0        0        0       40 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/6144-6399.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/61440-61695.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/61696-61951.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/61952-62207.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/62208-62463.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/62464-62719.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/62720-62975.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/62976-63231.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/63232-63487.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/63488-63743.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/63744-63999.pbf
--rw-r--r--   0        0        0       40 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/6400-6655.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/64000-64255.pbf
--rw-r--r--   0        0        0     4343 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/64256-64511.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/64512-64767.pbf
--rw-r--r--   0        0        0       42 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/64768-65023.pbf
--rw-r--r--   0        0        0       58 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/65024-65279.pbf
--rw-r--r--   0        0        0     1651 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/65280-65535.pbf
--rw-r--r--   0        0        0       40 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/6656-6911.pbf
--rw-r--r--   0        0        0       40 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/6912-7167.pbf
--rw-r--r--   0        0        0       40 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/7168-7423.pbf
--rw-r--r--   0        0        0       40 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/7424-7679.pbf
--rw-r--r--   0        0        0    35606 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/768-1023.pbf
--rw-r--r--   0        0        0    59631 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/7680-7935.pbf
--rw-r--r--   0        0        0      681 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/7936-8191.pbf
--rw-r--r--   0        0        0    10489 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/8192-8447.pbf
--rw-r--r--   0        0        0     5413 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/8448-8703.pbf
--rw-r--r--   0        0        0     4971 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/8704-8959.pbf
--rw-r--r--   0        0        0       40 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/8960-9215.pbf
--rw-r--r--   0        0        0       40 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/9216-9471.pbf
--rw-r--r--   0        0        0      451 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/9472-9727.pbf
--rw-r--r--   0        0        0       40 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/9728-9983.pbf
--rw-r--r--   0        0        0       41 2022-12-03 11:51:47.388652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/9984-10239.pbf
--rw-r--r--   0        0        0     5984 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/maplibre/LICENSE.txt
--rw-r--r--   0        0        0    70412 2022-12-03 11:51:47.396652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/maplibre/maplibre-gl.css
--rw-r--r--   0        0        0   745464 2022-12-03 11:51:47.400652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/maplibre/maplibre-gl.js
--rw-r--r--   0        0        0     6899 2022-12-03 11:51:47.400652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/sprites/sprite.json
--rw-r--r--   0        0        0    17411 2022-12-03 11:51:47.400652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/sprites/sprite.png
--rw-r--r--   0        0        0     6958 2022-12-03 11:51:47.400652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/sprites/sprite@2x.json
--rw-r--r--   0        0        0    44709 2022-12-03 11:51:47.404652 django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/sprites/sprite@2x.png
--rw-r--r--   0        0        0      225 2022-12-03 11:51:47.404652 django_tiles_gl-0.3.7/django_tiles_gl/templates/django_tiles_gl/maplibre_head.html
--rw-r--r--   0        0        0    70896 2022-12-03 11:51:47.404652 django_tiles_gl-0.3.7/django_tiles_gl/templates/django_tiles_gl/style.json
--rw-r--r--   0        0        0        0 2022-12-03 11:51:47.404652 django_tiles_gl-0.3.7/django_tiles_gl/templatetags/__init__.py
--rw-r--r--   0        0        0      158 2022-12-03 11:51:47.404652 django_tiles_gl-0.3.7/django_tiles_gl/templatetags/tiles_gl_tags.py
--rw-r--r--   0        0        0      326 2022-12-03 11:51:47.404652 django_tiles_gl-0.3.7/django_tiles_gl/urls.py
--rw-r--r--   0        0        0      483 2022-12-03 11:51:47.404652 django_tiles_gl-0.3.7/django_tiles_gl/utils.py
--rw-r--r--   0        0        0     3855 2022-12-03 11:51:47.404652 django_tiles_gl-0.3.7/django_tiles_gl/views.py
--rw-r--r--   0        0        0     1055 2022-12-03 11:51:47.404652 django_tiles_gl-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     6936 1970-01-01 00:00:00.000000 django_tiles_gl-0.3.7/setup.py
--rw-r--r--   0        0        0     6182 1970-01-01 00:00:00.000000 django_tiles_gl-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0    15362 2023-04-13 15:12:35.531068 django_tiles_gl-0.3.8/LICENSE.md
+-rw-r--r--   0        0        0     5131 2023-04-13 15:12:35.531068 django_tiles_gl-0.3.8/README.md
+-rw-r--r--   0        0        0        0 2023-04-13 15:12:35.631069 django_tiles_gl-0.3.8/django_tiles_gl/__init__.py
+-rw-r--r--   0        0        0      103 2023-04-13 15:12:35.631069 django_tiles_gl-0.3.8/django_tiles_gl/apps.py
+-rw-r--r--   0        0        0     3469 2023-04-13 15:12:35.631069 django_tiles_gl-0.3.8/django_tiles_gl/mbtiles.py
+-rw-r--r--   0        0        0    80025 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/0-255.pbf
+-rw-r--r--   0        0        0   134265 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/1024-1279.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/10240-10495.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/10496-10751.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/10752-11007.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/11008-11263.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/11264-11519.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/11520-11775.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/11776-12031.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/12032-12287.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/12288-12543.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/12544-12799.pbf
+-rw-r--r--   0        0        0    10755 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/1280-1535.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/12800-13055.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/13056-13311.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/13312-13567.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/13568-13823.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/13824-14079.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/14080-14335.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/14336-14591.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/14592-14847.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/14848-15103.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/15104-15359.pbf
+-rw-r--r--   0        0        0       29 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/1536-1791.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/15360-15615.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/15616-15871.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/15872-16127.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/16128-16383.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/16384-16639.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/16640-16895.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/16896-17151.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/17152-17407.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/17408-17663.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/17664-17919.pbf
+-rw-r--r--   0        0        0       29 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/1792-2047.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/17920-18175.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/18176-18431.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/18432-18687.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/18688-18943.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/18944-19199.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/19200-19455.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/19456-19711.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/19712-19967.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/19968-20223.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/20224-20479.pbf
+-rw-r--r--   0        0        0       29 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/2048-2303.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/20480-20735.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/20736-20991.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/20992-21247.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/21248-21503.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/21504-21759.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/21760-22015.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/22016-22271.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/22272-22527.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/22528-22783.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/22784-23039.pbf
+-rw-r--r--   0        0        0       29 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/2304-2559.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/23040-23295.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/23296-23551.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/23552-23807.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/23808-24063.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/24064-24319.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/24320-24575.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/24576-24831.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/24832-25087.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/25088-25343.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/25344-25599.pbf
+-rw-r--r--   0        0        0    70900 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/256-511.pbf
+-rw-r--r--   0        0        0       29 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/2560-2815.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/25600-25855.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/25856-26111.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/26112-26367.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/26368-26623.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/26624-26879.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/26880-27135.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/27136-27391.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/27392-27647.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/27648-27903.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/27904-28159.pbf
+-rw-r--r--   0        0        0       29 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/2816-3071.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/28160-28415.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/28416-28671.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/28672-28927.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/28928-29183.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/29184-29439.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/29440-29695.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/29696-29951.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/29952-30207.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/30208-30463.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/30464-30719.pbf
+-rw-r--r--   0        0        0       29 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/3072-3327.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/30720-30975.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/30976-31231.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/31232-31487.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/31488-31743.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/31744-31999.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/32000-32255.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/32256-32511.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/32512-32767.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/32768-33023.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/33024-33279.pbf
+-rw-r--r--   0        0        0       29 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/3328-3583.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/33280-33535.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/33536-33791.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/33792-34047.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/34048-34303.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/34304-34559.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/34560-34815.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/34816-35071.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/35072-35327.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/35328-35583.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/35584-35839.pbf
+-rw-r--r--   0        0        0       29 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/3584-3839.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/35840-36095.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/36096-36351.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/36352-36607.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/36608-36863.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/36864-37119.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/37120-37375.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/37376-37631.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/37632-37887.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/37888-38143.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/38144-38399.pbf
+-rw-r--r--   0        0        0       29 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/3840-4095.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/38400-38655.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/38656-38911.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/38912-39167.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/39168-39423.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/39424-39679.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/39680-39935.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/39936-40191.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/40192-40447.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/40448-40703.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/40704-40959.pbf
+-rw-r--r--   0        0        0       29 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/4096-4351.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/40960-41215.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/41216-41471.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/41472-41727.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/41728-41983.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/41984-42239.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/42240-42495.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/42496-42751.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/42752-43007.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/43008-43263.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/43264-43519.pbf
+-rw-r--r--   0        0        0       29 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/4352-4607.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/43520-43775.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/43776-44031.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/44032-44287.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/44288-44543.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/44544-44799.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/44800-45055.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/45056-45311.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/45312-45567.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/45568-45823.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/45824-46079.pbf
+-rw-r--r--   0        0        0       29 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/4608-4863.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/46080-46335.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/46336-46591.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/46592-46847.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/46848-47103.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/47104-47359.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/47360-47615.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/47616-47871.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/47872-48127.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/48128-48383.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/48384-48639.pbf
+-rw-r--r--   0        0        0       29 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/4864-5119.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.643069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/48640-48895.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/48896-49151.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/49152-49407.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/49408-49663.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/49664-49919.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/49920-50175.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/50176-50431.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/50432-50687.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/50688-50943.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/50944-51199.pbf
+-rw-r--r--   0        0        0     3918 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/512-767.pbf
+-rw-r--r--   0        0        0       29 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/5120-5375.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/51200-51455.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/51456-51711.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/51712-51967.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/51968-52223.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/52224-52479.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/52480-52735.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/52736-52991.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/52992-53247.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/53248-53503.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/53504-53759.pbf
+-rw-r--r--   0        0        0       29 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/5376-5631.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/53760-54015.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/54016-54271.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/54272-54527.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/54528-54783.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/54784-55039.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/55040-55295.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/55296-55551.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/55552-55807.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/55808-56063.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/56064-56319.pbf
+-rw-r--r--   0        0        0       29 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/5632-5887.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/56320-56575.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/56576-56831.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/56832-57087.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/57088-57343.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/57344-57599.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/57600-57855.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/57856-58111.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/58112-58367.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/58368-58623.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/58624-58879.pbf
+-rw-r--r--   0        0        0       29 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/5888-6143.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/58880-59135.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/59136-59391.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/59392-59647.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/59648-59903.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/59904-60159.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/60160-60415.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/60416-60671.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/60672-60927.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/60928-61183.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/61184-61439.pbf
+-rw-r--r--   0        0        0       29 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/6144-6399.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/61440-61695.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/61696-61951.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/61952-62207.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/62208-62463.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/62464-62719.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/62720-62975.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/62976-63231.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/63232-63487.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/63488-63743.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/63744-63999.pbf
+-rw-r--r--   0        0        0       29 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/6400-6655.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/64000-64255.pbf
+-rw-r--r--   0        0        0     3180 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/64256-64511.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/64512-64767.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/64768-65023.pbf
+-rw-r--r--   0        0        0       47 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/65024-65279.pbf
+-rw-r--r--   0        0        0     1640 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/65280-65535.pbf
+-rw-r--r--   0        0        0       29 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/6656-6911.pbf
+-rw-r--r--   0        0        0       29 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/6912-7167.pbf
+-rw-r--r--   0        0        0       29 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/7168-7423.pbf
+-rw-r--r--   0        0        0       29 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/7424-7679.pbf
+-rw-r--r--   0        0        0    36235 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/768-1023.pbf
+-rw-r--r--   0        0        0    60151 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/7680-7935.pbf
+-rw-r--r--   0        0        0      739 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/7936-8191.pbf
+-rw-r--r--   0        0        0    10494 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/8192-8447.pbf
+-rw-r--r--   0        0        0     5692 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/8448-8703.pbf
+-rw-r--r--   0        0        0     5169 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/8704-8959.pbf
+-rw-r--r--   0        0        0       29 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/8960-9215.pbf
+-rw-r--r--   0        0        0       29 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/9216-9471.pbf
+-rw-r--r--   0        0        0      463 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/9472-9727.pbf
+-rw-r--r--   0        0        0       29 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/9728-9983.pbf
+-rw-r--r--   0        0        0       30 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/9984-10239.pbf
+-rw-r--r--   0        0        0    83614 2023-04-13 15:12:35.631069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/0-255.pbf
+-rw-r--r--   0        0        0   136097 2023-04-13 15:12:35.631069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/1024-1279.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.631069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/10240-10495.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.631069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/10496-10751.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.631069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/10752-11007.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.631069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/11008-11263.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.631069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/11264-11519.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.631069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/11520-11775.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.631069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/11776-12031.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.631069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/12032-12287.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.631069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/12288-12543.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.631069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/12544-12799.pbf
+-rw-r--r--   0        0        0    10439 2023-04-13 15:12:35.631069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/1280-1535.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.631069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/12800-13055.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.631069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/13056-13311.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.631069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/13312-13567.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.631069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/13568-13823.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/13824-14079.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/14080-14335.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/14336-14591.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/14592-14847.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/14848-15103.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/15104-15359.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/1536-1791.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/15360-15615.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/15616-15871.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/15872-16127.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/16128-16383.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/16384-16639.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/16640-16895.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/16896-17151.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/17152-17407.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/17408-17663.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/17664-17919.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/1792-2047.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/17920-18175.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/18176-18431.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/18432-18687.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/18688-18943.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/18944-19199.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/19200-19455.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/19456-19711.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/19712-19967.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/19968-20223.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/20224-20479.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/2048-2303.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/20480-20735.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/20736-20991.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/20992-21247.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/21248-21503.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/21504-21759.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/21760-22015.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/22016-22271.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/22272-22527.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/22528-22783.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/22784-23039.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/2304-2559.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/23040-23295.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/23296-23551.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/23552-23807.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/23808-24063.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/24064-24319.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/24320-24575.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/24576-24831.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/24832-25087.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/25088-25343.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/25344-25599.pbf
+-rw-r--r--   0        0        0    75822 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/256-511.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/2560-2815.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/25600-25855.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/25856-26111.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/26112-26367.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/26368-26623.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/26624-26879.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/26880-27135.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/27136-27391.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/27392-27647.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/27648-27903.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/27904-28159.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/2816-3071.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/28160-28415.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/28416-28671.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/28672-28927.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/28928-29183.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/29184-29439.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/29440-29695.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/29696-29951.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/29952-30207.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/30208-30463.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/30464-30719.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/3072-3327.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/30720-30975.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/30976-31231.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/31232-31487.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/31488-31743.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/31744-31999.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/32000-32255.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/32256-32511.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/32512-32767.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/32768-33023.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/33024-33279.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/3328-3583.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/33280-33535.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/33536-33791.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/33792-34047.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/34048-34303.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/34304-34559.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/34560-34815.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/34816-35071.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/35072-35327.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/35328-35583.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/35584-35839.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/3584-3839.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/35840-36095.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/36096-36351.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/36352-36607.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/36608-36863.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/36864-37119.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/37120-37375.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/37376-37631.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/37632-37887.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/37888-38143.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/38144-38399.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/3840-4095.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/38400-38655.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/38656-38911.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/38912-39167.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/39168-39423.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/39424-39679.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/39680-39935.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/39936-40191.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/40192-40447.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/40448-40703.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/40704-40959.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/4096-4351.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/40960-41215.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/41216-41471.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/41472-41727.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/41728-41983.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/41984-42239.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/42240-42495.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/42496-42751.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/42752-43007.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/43008-43263.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/43264-43519.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/4352-4607.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/43520-43775.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/43776-44031.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/44032-44287.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/44288-44543.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/44544-44799.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/44800-45055.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/45056-45311.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/45312-45567.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/45568-45823.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/45824-46079.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/4608-4863.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/46080-46335.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/46336-46591.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/46592-46847.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/46848-47103.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/47104-47359.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/47360-47615.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/47616-47871.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/47872-48127.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/48128-48383.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/48384-48639.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/4864-5119.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/48640-48895.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/48896-49151.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/49152-49407.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/49408-49663.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/49664-49919.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/49920-50175.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/50176-50431.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.635069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/50432-50687.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/50688-50943.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/50944-51199.pbf
+-rw-r--r--   0        0        0     4101 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/512-767.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/5120-5375.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/51200-51455.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/51456-51711.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/51712-51967.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/51968-52223.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/52224-52479.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/52480-52735.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/52736-52991.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/52992-53247.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/53248-53503.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/53504-53759.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/5376-5631.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/53760-54015.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/54016-54271.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/54272-54527.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/54528-54783.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/54784-55039.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/55040-55295.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/55296-55551.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/55552-55807.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/55808-56063.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/56064-56319.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/5632-5887.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/56320-56575.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/56576-56831.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/56832-57087.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/57088-57343.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/57344-57599.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/57600-57855.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/57856-58111.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/58112-58367.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/58368-58623.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/58624-58879.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/5888-6143.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/58880-59135.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/59136-59391.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/59392-59647.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/59648-59903.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/59904-60159.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/60160-60415.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/60416-60671.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/60672-60927.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/60928-61183.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/61184-61439.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/6144-6399.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/61440-61695.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/61696-61951.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/61952-62207.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/62208-62463.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/62464-62719.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/62720-62975.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/62976-63231.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/63232-63487.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/63488-63743.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/63744-63999.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/6400-6655.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/64000-64255.pbf
+-rw-r--r--   0        0        0     4609 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/64256-64511.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/64512-64767.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/64768-65023.pbf
+-rw-r--r--   0        0        0       54 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/65024-65279.pbf
+-rw-r--r--   0        0        0     1647 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/65280-65535.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/6656-6911.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/6912-7167.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/7168-7423.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/7424-7679.pbf
+-rw-r--r--   0        0        0    36964 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/768-1023.pbf
+-rw-r--r--   0        0        0    61836 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/7680-7935.pbf
+-rw-r--r--   0        0        0      677 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/7936-8191.pbf
+-rw-r--r--   0        0        0    10957 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/8192-8447.pbf
+-rw-r--r--   0        0        0     5570 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/8448-8703.pbf
+-rw-r--r--   0        0        0     5093 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/8704-8959.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/8960-9215.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/9216-9471.pbf
+-rw-r--r--   0        0        0      470 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/9472-9727.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/9728-9983.pbf
+-rw-r--r--   0        0        0       37 2023-04-13 15:12:35.639069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/9984-10239.pbf
+-rw-r--r--   0        0        0    82954 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/0-255.pbf
+-rw-r--r--   0        0        0   139691 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/1024-1279.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/10240-10495.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/10496-10751.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/10752-11007.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/11008-11263.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/11264-11519.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/11520-11775.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/11776-12031.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/12032-12287.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/12288-12543.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/12544-12799.pbf
+-rw-r--r--   0        0        0    11296 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/1280-1535.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/12800-13055.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/13056-13311.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/13312-13567.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/13568-13823.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/13824-14079.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/14080-14335.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/14336-14591.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/14592-14847.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/14848-15103.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/15104-15359.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/1536-1791.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/15360-15615.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/15616-15871.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/15872-16127.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/16128-16383.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/16384-16639.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/16640-16895.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/16896-17151.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/17152-17407.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/17408-17663.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/17664-17919.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/1792-2047.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/17920-18175.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/18176-18431.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/18432-18687.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/18688-18943.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/18944-19199.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/19200-19455.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/19456-19711.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/19712-19967.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/19968-20223.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/20224-20479.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/2048-2303.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/20480-20735.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/20736-20991.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/20992-21247.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/21248-21503.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/21504-21759.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/21760-22015.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/22016-22271.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/22272-22527.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/22528-22783.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/22784-23039.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/2304-2559.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/23040-23295.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/23296-23551.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/23552-23807.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/23808-24063.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/24064-24319.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/24320-24575.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/24576-24831.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/24832-25087.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/25088-25343.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/25344-25599.pbf
+-rw-r--r--   0        0        0    73897 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/256-511.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/2560-2815.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/25600-25855.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/25856-26111.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/26112-26367.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/26368-26623.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/26624-26879.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/26880-27135.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/27136-27391.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/27392-27647.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/27648-27903.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/27904-28159.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/2816-3071.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/28160-28415.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/28416-28671.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/28672-28927.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/28928-29183.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/29184-29439.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/29440-29695.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/29696-29951.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/29952-30207.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/30208-30463.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/30464-30719.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/3072-3327.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/30720-30975.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/30976-31231.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/31232-31487.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/31488-31743.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/31744-31999.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/32000-32255.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/32256-32511.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/32512-32767.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/32768-33023.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/33024-33279.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/3328-3583.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/33280-33535.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/33536-33791.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/33792-34047.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/34048-34303.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/34304-34559.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/34560-34815.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/34816-35071.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/35072-35327.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/35328-35583.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/35584-35839.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/3584-3839.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/35840-36095.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/36096-36351.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/36352-36607.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/36608-36863.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/36864-37119.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/37120-37375.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/37376-37631.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/37632-37887.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/37888-38143.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/38144-38399.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/3840-4095.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/38400-38655.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/38656-38911.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/38912-39167.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/39168-39423.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/39424-39679.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/39680-39935.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/39936-40191.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/40192-40447.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/40448-40703.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/40704-40959.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/4096-4351.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/40960-41215.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/41216-41471.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/41472-41727.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.659069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/41728-41983.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/41984-42239.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/42240-42495.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/42496-42751.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/42752-43007.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/43008-43263.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/43264-43519.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/4352-4607.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/43520-43775.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/43776-44031.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/44032-44287.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/44288-44543.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/44544-44799.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/44800-45055.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/45056-45311.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/45312-45567.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/45568-45823.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/45824-46079.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/4608-4863.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/46080-46335.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/46336-46591.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/46592-46847.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/46848-47103.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/47104-47359.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/47360-47615.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/47616-47871.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/47872-48127.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/48128-48383.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/48384-48639.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/4864-5119.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/48640-48895.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/48896-49151.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/49152-49407.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/49408-49663.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/49664-49919.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/49920-50175.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/50176-50431.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/50432-50687.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/50688-50943.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/50944-51199.pbf
+-rw-r--r--   0        0        0     4109 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/512-767.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/5120-5375.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/51200-51455.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/51456-51711.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/51712-51967.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/51968-52223.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/52224-52479.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/52480-52735.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/52736-52991.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/52992-53247.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/53248-53503.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/53504-53759.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/5376-5631.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/53760-54015.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/54016-54271.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/54272-54527.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/54528-54783.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/54784-55039.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/55040-55295.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/55296-55551.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/55552-55807.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/55808-56063.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/56064-56319.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/5632-5887.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/56320-56575.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/56576-56831.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/56832-57087.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/57088-57343.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/57344-57599.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/57600-57855.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/57856-58111.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/58112-58367.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/58368-58623.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/58624-58879.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/5888-6143.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/58880-59135.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/59136-59391.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/59392-59647.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/59648-59903.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/59904-60159.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/60160-60415.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/60416-60671.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/60672-60927.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/60928-61183.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/61184-61439.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/6144-6399.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/61440-61695.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/61696-61951.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/61952-62207.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/62208-62463.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/62464-62719.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/62720-62975.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/62976-63231.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/63232-63487.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/63488-63743.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/63744-63999.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/6400-6655.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/64000-64255.pbf
+-rw-r--r--   0        0        0     3309 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/64256-64511.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/64512-64767.pbf
+-rw-r--r--   0        0        0       36 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/64768-65023.pbf
+-rw-r--r--   0        0        0       52 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/65024-65279.pbf
+-rw-r--r--   0        0        0     1645 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/65280-65535.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/6656-6911.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/6912-7167.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/7168-7423.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/7424-7679.pbf
+-rw-r--r--   0        0        0    37828 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/768-1023.pbf
+-rw-r--r--   0        0        0    62708 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/7680-7935.pbf
+-rw-r--r--   0        0        0      767 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/7936-8191.pbf
+-rw-r--r--   0        0        0    11075 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/8192-8447.pbf
+-rw-r--r--   0        0        0     5918 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/8448-8703.pbf
+-rw-r--r--   0        0        0     5341 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/8704-8959.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/8960-9215.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/9216-9471.pbf
+-rw-r--r--   0        0        0      468 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/9472-9727.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/9728-9983.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.663070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/9984-10239.pbf
+-rw-r--r--   0        0        0    87547 2023-04-13 15:12:35.647069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/0-255.pbf
+-rw-r--r--   0        0        0   143840 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/1024-1279.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/10240-10495.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/10496-10751.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/10752-11007.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/11008-11263.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/11264-11519.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/11520-11775.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/11776-12031.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/12032-12287.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/12288-12543.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/12544-12799.pbf
+-rw-r--r--   0        0        0    11017 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/1280-1535.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/12800-13055.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/13056-13311.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/13312-13567.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/13568-13823.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/13824-14079.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/14080-14335.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/14336-14591.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/14592-14847.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/14848-15103.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/15104-15359.pbf
+-rw-r--r--   0        0        0       41 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/1536-1791.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/15360-15615.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/15616-15871.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/15872-16127.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/16128-16383.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/16384-16639.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/16640-16895.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/16896-17151.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/17152-17407.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/17408-17663.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/17664-17919.pbf
+-rw-r--r--   0        0        0       41 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/1792-2047.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/17920-18175.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/18176-18431.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/18432-18687.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/18688-18943.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/18944-19199.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/19200-19455.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/19456-19711.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/19712-19967.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/19968-20223.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/20224-20479.pbf
+-rw-r--r--   0        0        0       41 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/2048-2303.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/20480-20735.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/20736-20991.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/20992-21247.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/21248-21503.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/21504-21759.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/21760-22015.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/22016-22271.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/22272-22527.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/22528-22783.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/22784-23039.pbf
+-rw-r--r--   0        0        0       41 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/2304-2559.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/23040-23295.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/23296-23551.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/23552-23807.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/23808-24063.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/24064-24319.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/24320-24575.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/24576-24831.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/24832-25087.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/25088-25343.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/25344-25599.pbf
+-rw-r--r--   0        0        0    79892 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/256-511.pbf
+-rw-r--r--   0        0        0       41 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/2560-2815.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/25600-25855.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/25856-26111.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/26112-26367.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/26368-26623.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/26624-26879.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/26880-27135.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/27136-27391.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/27392-27647.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/27648-27903.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/27904-28159.pbf
+-rw-r--r--   0        0        0       41 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/2816-3071.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/28160-28415.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/28416-28671.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/28672-28927.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/28928-29183.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/29184-29439.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/29440-29695.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/29696-29951.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/29952-30207.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/30208-30463.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/30464-30719.pbf
+-rw-r--r--   0        0        0       41 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/3072-3327.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/30720-30975.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/30976-31231.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/31232-31487.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/31488-31743.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/31744-31999.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/32000-32255.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/32256-32511.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/32512-32767.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/32768-33023.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/33024-33279.pbf
+-rw-r--r--   0        0        0       41 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/3328-3583.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/33280-33535.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/33536-33791.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/33792-34047.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/34048-34303.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/34304-34559.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/34560-34815.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/34816-35071.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/35072-35327.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/35328-35583.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/35584-35839.pbf
+-rw-r--r--   0        0        0       41 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/3584-3839.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/35840-36095.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/36096-36351.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/36352-36607.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/36608-36863.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/36864-37119.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/37120-37375.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/37376-37631.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/37632-37887.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/37888-38143.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/38144-38399.pbf
+-rw-r--r--   0        0        0       41 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/3840-4095.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/38400-38655.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/38656-38911.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/38912-39167.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/39168-39423.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/39424-39679.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/39680-39935.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/39936-40191.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/40192-40447.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/40448-40703.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/40704-40959.pbf
+-rw-r--r--   0        0        0       41 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/4096-4351.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/40960-41215.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/41216-41471.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/41472-41727.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/41728-41983.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/41984-42239.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/42240-42495.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/42496-42751.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/42752-43007.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/43008-43263.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/43264-43519.pbf
+-rw-r--r--   0        0        0       41 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/4352-4607.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/43520-43775.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/43776-44031.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/44032-44287.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/44288-44543.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/44544-44799.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/44800-45055.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/45056-45311.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.651069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/45312-45567.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/45568-45823.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/45824-46079.pbf
+-rw-r--r--   0        0        0       41 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/4608-4863.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/46080-46335.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/46336-46591.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/46592-46847.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/46848-47103.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/47104-47359.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/47360-47615.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/47616-47871.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/47872-48127.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/48128-48383.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/48384-48639.pbf
+-rw-r--r--   0        0        0       41 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/4864-5119.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/48640-48895.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/48896-49151.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/49152-49407.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/49408-49663.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/49664-49919.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/49920-50175.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/50176-50431.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/50432-50687.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/50688-50943.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/50944-51199.pbf
+-rw-r--r--   0        0        0     4308 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/512-767.pbf
+-rw-r--r--   0        0        0       41 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/5120-5375.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/51200-51455.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/51456-51711.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/51712-51967.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/51968-52223.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/52224-52479.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/52480-52735.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/52736-52991.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/52992-53247.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/53248-53503.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/53504-53759.pbf
+-rw-r--r--   0        0        0       41 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/5376-5631.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/53760-54015.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/54016-54271.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/54272-54527.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/54528-54783.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/54784-55039.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/55040-55295.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/55296-55551.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/55552-55807.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/55808-56063.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/56064-56319.pbf
+-rw-r--r--   0        0        0       41 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/5632-5887.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/56320-56575.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/56576-56831.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/56832-57087.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/57088-57343.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/57344-57599.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/57600-57855.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/57856-58111.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/58112-58367.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/58368-58623.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/58624-58879.pbf
+-rw-r--r--   0        0        0       41 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/5888-6143.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/58880-59135.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/59136-59391.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/59392-59647.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/59648-59903.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/59904-60159.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/60160-60415.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/60416-60671.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/60672-60927.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/60928-61183.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/61184-61439.pbf
+-rw-r--r--   0        0        0       41 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/6144-6399.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/61440-61695.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/61696-61951.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/61952-62207.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/62208-62463.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/62464-62719.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/62720-62975.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/62976-63231.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/63232-63487.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/63488-63743.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/63744-63999.pbf
+-rw-r--r--   0        0        0       41 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/6400-6655.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/64000-64255.pbf
+-rw-r--r--   0        0        0     4765 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/64256-64511.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/64512-64767.pbf
+-rw-r--r--   0        0        0       43 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/64768-65023.pbf
+-rw-r--r--   0        0        0       59 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/65024-65279.pbf
+-rw-r--r--   0        0        0     1652 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/65280-65535.pbf
+-rw-r--r--   0        0        0       41 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/6656-6911.pbf
+-rw-r--r--   0        0        0       41 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/6912-7167.pbf
+-rw-r--r--   0        0        0       41 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/7168-7423.pbf
+-rw-r--r--   0        0        0       41 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/7424-7679.pbf
+-rw-r--r--   0        0        0    38925 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/768-1023.pbf
+-rw-r--r--   0        0        0    64829 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/7680-7935.pbf
+-rw-r--r--   0        0        0      705 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/7936-8191.pbf
+-rw-r--r--   0        0        0    11556 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/8192-8447.pbf
+-rw-r--r--   0        0        0     5865 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/8448-8703.pbf
+-rw-r--r--   0        0        0     5292 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/8704-8959.pbf
+-rw-r--r--   0        0        0       41 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/8960-9215.pbf
+-rw-r--r--   0        0        0       41 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/9216-9471.pbf
+-rw-r--r--   0        0        0      475 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/9472-9727.pbf
+-rw-r--r--   0        0        0       41 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/9728-9983.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.655069 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/9984-10239.pbf
+-rw-r--r--   0        0        0    78054 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/0-255.pbf
+-rw-r--r--   0        0        0   125040 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/1024-1279.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/10240-10495.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/10496-10751.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/10752-11007.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/11008-11263.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/11264-11519.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/11520-11775.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/11776-12031.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/12032-12287.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/12288-12543.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/12544-12799.pbf
+-rw-r--r--   0        0        0     9668 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/1280-1535.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/12800-13055.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/13056-13311.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/13312-13567.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/13568-13823.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/13824-14079.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/14080-14335.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/14336-14591.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/14592-14847.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/14848-15103.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/15104-15359.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/1536-1791.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/15360-15615.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/15616-15871.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/15872-16127.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/16128-16383.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/16384-16639.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/16640-16895.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/16896-17151.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/17152-17407.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/17408-17663.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/17664-17919.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/1792-2047.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/17920-18175.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/18176-18431.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/18432-18687.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/18688-18943.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/18944-19199.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/19200-19455.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/19456-19711.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/19712-19967.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/19968-20223.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/20224-20479.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/2048-2303.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/20480-20735.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/20736-20991.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/20992-21247.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/21248-21503.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/21504-21759.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/21760-22015.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/22016-22271.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/22272-22527.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/22528-22783.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/22784-23039.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/2304-2559.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/23040-23295.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/23296-23551.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/23552-23807.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/23808-24063.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/24064-24319.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/24320-24575.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/24576-24831.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/24832-25087.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/25088-25343.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/25344-25599.pbf
+-rw-r--r--   0        0        0    69941 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/256-511.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/2560-2815.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/25600-25855.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/25856-26111.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/26112-26367.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/26368-26623.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/26624-26879.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/26880-27135.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/27136-27391.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/27392-27647.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/27648-27903.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/27904-28159.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/2816-3071.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/28160-28415.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/28416-28671.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/28672-28927.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/28928-29183.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/29184-29439.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/29440-29695.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/29696-29951.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/29952-30207.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/30208-30463.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/30464-30719.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/3072-3327.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/30720-30975.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/30976-31231.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/31232-31487.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/31488-31743.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/31744-31999.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/32000-32255.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/32256-32511.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/32512-32767.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/32768-33023.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/33024-33279.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/3328-3583.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/33280-33535.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/33536-33791.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/33792-34047.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/34048-34303.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/34304-34559.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/34560-34815.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/34816-35071.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/35072-35327.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/35328-35583.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/35584-35839.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/3584-3839.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/35840-36095.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/36096-36351.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/36352-36607.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/36608-36863.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/36864-37119.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/37120-37375.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/37376-37631.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/37632-37887.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/37888-38143.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/38144-38399.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/3840-4095.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/38400-38655.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/38656-38911.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/38912-39167.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/39168-39423.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.667070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/39424-39679.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/39680-39935.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/39936-40191.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/40192-40447.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/40448-40703.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/40704-40959.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/4096-4351.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/40960-41215.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/41216-41471.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/41472-41727.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/41728-41983.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/41984-42239.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/42240-42495.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/42496-42751.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/42752-43007.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/43008-43263.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/43264-43519.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/4352-4607.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/43520-43775.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/43776-44031.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/44032-44287.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/44288-44543.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/44544-44799.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/44800-45055.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/45056-45311.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/45312-45567.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/45568-45823.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/45824-46079.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/4608-4863.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/46080-46335.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/46336-46591.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/46592-46847.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/46848-47103.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/47104-47359.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/47360-47615.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/47616-47871.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/47872-48127.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/48128-48383.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/48384-48639.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/4864-5119.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/48640-48895.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/48896-49151.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/49152-49407.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/49408-49663.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/49664-49919.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/49920-50175.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/50176-50431.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/50432-50687.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/50688-50943.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/50944-51199.pbf
+-rw-r--r--   0        0        0     3712 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/512-767.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/5120-5375.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/51200-51455.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/51456-51711.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/51712-51967.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/51968-52223.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/52224-52479.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/52480-52735.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/52736-52991.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/52992-53247.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/53248-53503.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/53504-53759.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/5376-5631.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/53760-54015.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/54016-54271.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/54272-54527.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/54528-54783.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/54784-55039.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/55040-55295.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/55296-55551.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/55552-55807.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/55808-56063.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/56064-56319.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/5632-5887.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/56320-56575.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/56576-56831.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/56832-57087.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/57088-57343.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/57344-57599.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/57600-57855.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/57856-58111.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/58112-58367.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/58368-58623.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/58624-58879.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/5888-6143.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/58880-59135.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/59136-59391.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/59392-59647.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/59648-59903.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/59904-60159.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/60160-60415.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/60416-60671.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/60672-60927.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/60928-61183.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/61184-61439.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/6144-6399.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/61440-61695.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/61696-61951.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/61952-62207.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/62208-62463.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/62464-62719.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/62720-62975.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/62976-63231.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/63232-63487.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/63488-63743.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/63744-63999.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/6400-6655.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/64000-64255.pbf
+-rw-r--r--   0        0        0     4214 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/64256-64511.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/64512-64767.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/64768-65023.pbf
+-rw-r--r--   0        0        0       49 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/65024-65279.pbf
+-rw-r--r--   0        0        0     1642 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/65280-65535.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/6656-6911.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/6912-7167.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/7168-7423.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/7424-7679.pbf
+-rw-r--r--   0        0        0    34219 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/768-1023.pbf
+-rw-r--r--   0        0        0    57224 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/7680-7935.pbf
+-rw-r--r--   0        0        0      626 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/7936-8191.pbf
+-rw-r--r--   0        0        0    10083 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/8192-8447.pbf
+-rw-r--r--   0        0        0     5275 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/8448-8703.pbf
+-rw-r--r--   0        0        0     4845 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/8704-8959.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/8960-9215.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/9216-9471.pbf
+-rw-r--r--   0        0        0      442 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/9472-9727.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/9728-9983.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.671070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/9984-10239.pbf
+-rw-r--r--   0        0        0    72370 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/0-255.pbf
+-rw-r--r--   0        0        0   117993 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/1024-1279.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/10240-10495.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/10496-10751.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/10752-11007.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/11008-11263.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/11264-11519.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/11520-11775.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/11776-12031.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/12032-12287.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/12288-12543.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/12544-12799.pbf
+-rw-r--r--   0        0        0     9508 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/1280-1535.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/12800-13055.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/13056-13311.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/13312-13567.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/13568-13823.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/13824-14079.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/14080-14335.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/14336-14591.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/14592-14847.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/14848-15103.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/15104-15359.pbf
+-rw-r--r--   0        0        0       30 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/1536-1791.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/15360-15615.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/15616-15871.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/15872-16127.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/16128-16383.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/16384-16639.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/16640-16895.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/16896-17151.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/17152-17407.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/17408-17663.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/17664-17919.pbf
+-rw-r--r--   0        0        0       30 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/1792-2047.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/17920-18175.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/18176-18431.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/18432-18687.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/18688-18943.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/18944-19199.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/19200-19455.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/19456-19711.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/19712-19967.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/19968-20223.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/20224-20479.pbf
+-rw-r--r--   0        0        0       30 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/2048-2303.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/20480-20735.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/20736-20991.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/20992-21247.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/21248-21503.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/21504-21759.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/21760-22015.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/22016-22271.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/22272-22527.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/22528-22783.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/22784-23039.pbf
+-rw-r--r--   0        0        0       30 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/2304-2559.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/23040-23295.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/23296-23551.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/23552-23807.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/23808-24063.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/24064-24319.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/24320-24575.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/24576-24831.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/24832-25087.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/25088-25343.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/25344-25599.pbf
+-rw-r--r--   0        0        0    63678 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/256-511.pbf
+-rw-r--r--   0        0        0       30 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/2560-2815.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/25600-25855.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/25856-26111.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/26112-26367.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/26368-26623.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/26624-26879.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/26880-27135.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/27136-27391.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/27392-27647.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/27648-27903.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/27904-28159.pbf
+-rw-r--r--   0        0        0       30 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/2816-3071.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/28160-28415.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/28416-28671.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/28672-28927.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/28928-29183.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/29184-29439.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/29440-29695.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/29696-29951.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/29952-30207.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/30208-30463.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/30464-30719.pbf
+-rw-r--r--   0        0        0       30 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/3072-3327.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/30720-30975.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/30976-31231.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/31232-31487.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/31488-31743.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/31744-31999.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/32000-32255.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/32256-32511.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/32512-32767.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/32768-33023.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/33024-33279.pbf
+-rw-r--r--   0        0        0       30 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/3328-3583.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/33280-33535.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/33536-33791.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/33792-34047.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/34048-34303.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/34304-34559.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/34560-34815.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/34816-35071.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/35072-35327.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/35328-35583.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/35584-35839.pbf
+-rw-r--r--   0        0        0       30 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/3584-3839.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/35840-36095.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/36096-36351.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/36352-36607.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/36608-36863.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/36864-37119.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/37120-37375.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/37376-37631.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/37632-37887.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/37888-38143.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/38144-38399.pbf
+-rw-r--r--   0        0        0       30 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/3840-4095.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/38400-38655.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/38656-38911.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/38912-39167.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/39168-39423.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/39424-39679.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.683070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/39680-39935.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/39936-40191.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/40192-40447.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/40448-40703.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/40704-40959.pbf
+-rw-r--r--   0        0        0       30 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/4096-4351.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/40960-41215.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/41216-41471.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/41472-41727.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/41728-41983.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/41984-42239.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/42240-42495.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/42496-42751.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/42752-43007.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/43008-43263.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/43264-43519.pbf
+-rw-r--r--   0        0        0       30 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/4352-4607.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/43520-43775.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/43776-44031.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/44032-44287.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/44288-44543.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/44544-44799.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/44800-45055.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/45056-45311.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/45312-45567.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/45568-45823.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/45824-46079.pbf
+-rw-r--r--   0        0        0       30 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/4608-4863.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/46080-46335.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/46336-46591.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/46592-46847.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/46848-47103.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/47104-47359.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/47360-47615.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/47616-47871.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/47872-48127.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/48128-48383.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/48384-48639.pbf
+-rw-r--r--   0        0        0       30 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/4864-5119.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/48640-48895.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/48896-49151.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/49152-49407.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/49408-49663.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/49664-49919.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/49920-50175.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/50176-50431.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/50432-50687.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/50688-50943.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/50944-51199.pbf
+-rw-r--r--   0        0        0     3430 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/512-767.pbf
+-rw-r--r--   0        0        0       30 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/5120-5375.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/51200-51455.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/51456-51711.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/51712-51967.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/51968-52223.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/52224-52479.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/52480-52735.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/52736-52991.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/52992-53247.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/53248-53503.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/53504-53759.pbf
+-rw-r--r--   0        0        0       30 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/5376-5631.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/53760-54015.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/54016-54271.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/54272-54527.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/54528-54783.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/54784-55039.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/55040-55295.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/55296-55551.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/55552-55807.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/55808-56063.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/56064-56319.pbf
+-rw-r--r--   0        0        0       30 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/5632-5887.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/56320-56575.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/56576-56831.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/56832-57087.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/57088-57343.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/57344-57599.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/57600-57855.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/57856-58111.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/58112-58367.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/58368-58623.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/58624-58879.pbf
+-rw-r--r--   0        0        0       30 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/5888-6143.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/58880-59135.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/59136-59391.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/59392-59647.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/59648-59903.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/59904-60159.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/60160-60415.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/60416-60671.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/60672-60927.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/60928-61183.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/61184-61439.pbf
+-rw-r--r--   0        0        0       30 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/6144-6399.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/61440-61695.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/61696-61951.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/61952-62207.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/62208-62463.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/62464-62719.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/62720-62975.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/62976-63231.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/63232-63487.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/63488-63743.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/63744-63999.pbf
+-rw-r--r--   0        0        0       30 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/6400-6655.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/64000-64255.pbf
+-rw-r--r--   0        0        0     2533 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/64256-64511.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/64512-64767.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/64768-65023.pbf
+-rw-r--r--   0        0        0       48 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/65024-65279.pbf
+-rw-r--r--   0        0        0     1641 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/65280-65535.pbf
+-rw-r--r--   0        0        0       30 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/6656-6911.pbf
+-rw-r--r--   0        0        0       30 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/6912-7167.pbf
+-rw-r--r--   0        0        0       30 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/7168-7423.pbf
+-rw-r--r--   0        0        0       30 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/7424-7679.pbf
+-rw-r--r--   0        0        0    32916 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/768-1023.pbf
+-rw-r--r--   0        0        0    52825 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/7680-7935.pbf
+-rw-r--r--   0        0        0      671 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/7936-8191.pbf
+-rw-r--r--   0        0        0     9151 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/8192-8447.pbf
+-rw-r--r--   0        0        0     5214 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/8448-8703.pbf
+-rw-r--r--   0        0        0     4731 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/8704-8959.pbf
+-rw-r--r--   0        0        0       30 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/8960-9215.pbf
+-rw-r--r--   0        0        0       30 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/9216-9471.pbf
+-rw-r--r--   0        0        0      464 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/9472-9727.pbf
+-rw-r--r--   0        0        0       30 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/9728-9983.pbf
+-rw-r--r--   0        0        0       31 2023-04-13 15:12:35.687070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/9984-10239.pbf
+-rw-r--r--   0        0        0    75722 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/0-255.pbf
+-rw-r--r--   0        0        0   121649 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/1024-1279.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/10240-10495.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/10496-10751.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/10752-11007.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/11008-11263.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/11264-11519.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/11520-11775.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/11776-12031.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/12032-12287.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/12288-12543.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/12544-12799.pbf
+-rw-r--r--   0        0        0     9260 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/1280-1535.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/12800-13055.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/13056-13311.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/13312-13567.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/13568-13823.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/13824-14079.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/14080-14335.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/14336-14591.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/14592-14847.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/14848-15103.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/15104-15359.pbf
+-rw-r--r--   0        0        0       37 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/1536-1791.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/15360-15615.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/15616-15871.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/15872-16127.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/16128-16383.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/16384-16639.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/16640-16895.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/16896-17151.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/17152-17407.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/17408-17663.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/17664-17919.pbf
+-rw-r--r--   0        0        0       37 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/1792-2047.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/17920-18175.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/18176-18431.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/18432-18687.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/18688-18943.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/18944-19199.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/19200-19455.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/19456-19711.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/19712-19967.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/19968-20223.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/20224-20479.pbf
+-rw-r--r--   0        0        0       37 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/2048-2303.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/20480-20735.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/20736-20991.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/20992-21247.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/21248-21503.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/21504-21759.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/21760-22015.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/22016-22271.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/22272-22527.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/22528-22783.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/22784-23039.pbf
+-rw-r--r--   0        0        0       37 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/2304-2559.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/23040-23295.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/23296-23551.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/23552-23807.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/23808-24063.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/24064-24319.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/24320-24575.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/24576-24831.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/24832-25087.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/25088-25343.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/25344-25599.pbf
+-rw-r--r--   0        0        0    68072 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/256-511.pbf
+-rw-r--r--   0        0        0       37 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/2560-2815.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/25600-25855.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/25856-26111.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/26112-26367.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/26368-26623.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/26624-26879.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/26880-27135.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/27136-27391.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/27392-27647.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/27648-27903.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/27904-28159.pbf
+-rw-r--r--   0        0        0       37 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/2816-3071.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/28160-28415.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/28416-28671.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/28672-28927.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/28928-29183.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/29184-29439.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/29440-29695.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/29696-29951.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/29952-30207.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/30208-30463.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/30464-30719.pbf
+-rw-r--r--   0        0        0       37 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/3072-3327.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/30720-30975.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/30976-31231.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/31232-31487.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/31488-31743.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/31744-31999.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/32000-32255.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/32256-32511.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/32512-32767.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/32768-33023.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/33024-33279.pbf
+-rw-r--r--   0        0        0       37 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/3328-3583.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/33280-33535.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/33536-33791.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/33792-34047.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/34048-34303.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/34304-34559.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/34560-34815.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/34816-35071.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/35072-35327.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/35328-35583.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/35584-35839.pbf
+-rw-r--r--   0        0        0       37 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/3584-3839.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/35840-36095.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/36096-36351.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/36352-36607.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/36608-36863.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/36864-37119.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/37120-37375.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/37376-37631.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/37632-37887.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/37888-38143.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/38144-38399.pbf
+-rw-r--r--   0        0        0       37 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/3840-4095.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/38400-38655.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.675070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/38656-38911.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/38912-39167.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/39168-39423.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/39424-39679.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/39680-39935.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/39936-40191.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/40192-40447.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/40448-40703.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/40704-40959.pbf
+-rw-r--r--   0        0        0       37 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/4096-4351.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/40960-41215.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/41216-41471.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/41472-41727.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/41728-41983.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/41984-42239.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/42240-42495.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/42496-42751.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/42752-43007.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/43008-43263.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/43264-43519.pbf
+-rw-r--r--   0        0        0       37 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/4352-4607.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/43520-43775.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/43776-44031.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/44032-44287.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/44288-44543.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/44544-44799.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/44800-45055.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/45056-45311.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/45312-45567.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/45568-45823.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/45824-46079.pbf
+-rw-r--r--   0        0        0       37 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/4608-4863.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/46080-46335.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/46336-46591.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/46592-46847.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/46848-47103.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/47104-47359.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/47360-47615.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/47616-47871.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/47872-48127.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/48128-48383.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/48384-48639.pbf
+-rw-r--r--   0        0        0       37 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/4864-5119.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/48640-48895.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/48896-49151.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/49152-49407.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/49408-49663.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/49664-49919.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/49920-50175.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/50176-50431.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/50432-50687.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/50688-50943.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/50944-51199.pbf
+-rw-r--r--   0        0        0     3555 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/512-767.pbf
+-rw-r--r--   0        0        0       37 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/5120-5375.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/51200-51455.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/51456-51711.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/51712-51967.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/51968-52223.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/52224-52479.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/52480-52735.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/52736-52991.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/52992-53247.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/53248-53503.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/53504-53759.pbf
+-rw-r--r--   0        0        0       37 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/5376-5631.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/53760-54015.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/54016-54271.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/54272-54527.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/54528-54783.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/54784-55039.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/55040-55295.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/55296-55551.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/55552-55807.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/55808-56063.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/56064-56319.pbf
+-rw-r--r--   0        0        0       37 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/5632-5887.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/56320-56575.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/56576-56831.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/56832-57087.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/57088-57343.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/57344-57599.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/57600-57855.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/57856-58111.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/58112-58367.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/58368-58623.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/58624-58879.pbf
+-rw-r--r--   0        0        0       37 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/5888-6143.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/58880-59135.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/59136-59391.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/59392-59647.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/59648-59903.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/59904-60159.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/60160-60415.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/60416-60671.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/60672-60927.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/60928-61183.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/61184-61439.pbf
+-rw-r--r--   0        0        0       37 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/6144-6399.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/61440-61695.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/61696-61951.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/61952-62207.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/62208-62463.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/62464-62719.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/62720-62975.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/62976-63231.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/63232-63487.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/63488-63743.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/63744-63999.pbf
+-rw-r--r--   0        0        0       37 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/6400-6655.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/64000-64255.pbf
+-rw-r--r--   0        0        0     3920 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/64256-64511.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/64512-64767.pbf
+-rw-r--r--   0        0        0       39 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/64768-65023.pbf
+-rw-r--r--   0        0        0       55 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/65024-65279.pbf
+-rw-r--r--   0        0        0     1648 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/65280-65535.pbf
+-rw-r--r--   0        0        0       37 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/6656-6911.pbf
+-rw-r--r--   0        0        0       37 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/6912-7167.pbf
+-rw-r--r--   0        0        0       37 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/7168-7423.pbf
+-rw-r--r--   0        0        0       37 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/7424-7679.pbf
+-rw-r--r--   0        0        0    33074 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/768-1023.pbf
+-rw-r--r--   0        0        0    55285 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/7680-7935.pbf
+-rw-r--r--   0        0        0      632 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/7936-8191.pbf
+-rw-r--r--   0        0        0     9699 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/8192-8447.pbf
+-rw-r--r--   0        0        0     5124 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/8448-8703.pbf
+-rw-r--r--   0        0        0     4751 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/8704-8959.pbf
+-rw-r--r--   0        0        0       37 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/8960-9215.pbf
+-rw-r--r--   0        0        0       37 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/9216-9471.pbf
+-rw-r--r--   0        0        0      471 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/9472-9727.pbf
+-rw-r--r--   0        0        0       37 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/9728-9983.pbf
+-rw-r--r--   0        0        0       38 2023-04-13 15:12:35.679070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/9984-10239.pbf
+-rw-r--r--   0        0        0    74696 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/0-255.pbf
+-rw-r--r--   0        0        0   122545 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/1024-1279.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/10240-10495.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/10496-10751.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/10752-11007.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/11008-11263.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/11264-11519.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/11520-11775.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/11776-12031.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/12032-12287.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/12288-12543.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/12544-12799.pbf
+-rw-r--r--   0        0        0     9913 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/1280-1535.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/12800-13055.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/13056-13311.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/13312-13567.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/13568-13823.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/13824-14079.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/14080-14335.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/14336-14591.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/14592-14847.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/14848-15103.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/15104-15359.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/1536-1791.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/15360-15615.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/15616-15871.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/15872-16127.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/16128-16383.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/16384-16639.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/16640-16895.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/16896-17151.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/17152-17407.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/17408-17663.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/17664-17919.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/1792-2047.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/17920-18175.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/18176-18431.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/18432-18687.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/18688-18943.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/18944-19199.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/19200-19455.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/19456-19711.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/19712-19967.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/19968-20223.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/20224-20479.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/2048-2303.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/20480-20735.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/20736-20991.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/20992-21247.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/21248-21503.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/21504-21759.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/21760-22015.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/22016-22271.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/22272-22527.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/22528-22783.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/22784-23039.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/2304-2559.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/23040-23295.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/23296-23551.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/23552-23807.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/23808-24063.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/24064-24319.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/24320-24575.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/24576-24831.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/24832-25087.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/25088-25343.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/25344-25599.pbf
+-rw-r--r--   0        0        0    66481 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/256-511.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/2560-2815.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/25600-25855.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/25856-26111.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/26112-26367.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/26368-26623.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/26624-26879.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/26880-27135.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/27136-27391.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/27392-27647.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/27648-27903.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/27904-28159.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/2816-3071.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/28160-28415.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/28416-28671.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/28672-28927.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/28928-29183.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/29184-29439.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/29440-29695.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/29696-29951.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/29952-30207.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/30208-30463.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/30464-30719.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/3072-3327.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/30720-30975.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/30976-31231.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/31232-31487.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/31488-31743.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/31744-31999.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/32000-32255.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/32256-32511.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/32512-32767.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/32768-33023.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/33024-33279.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/3328-3583.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/33280-33535.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/33536-33791.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/33792-34047.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/34048-34303.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/34304-34559.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/34560-34815.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/34816-35071.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/35072-35327.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/35328-35583.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/35584-35839.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/3584-3839.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/35840-36095.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/36096-36351.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/36352-36607.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/36608-36863.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/36864-37119.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/37120-37375.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/37376-37631.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/37632-37887.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/37888-38143.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/38144-38399.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/3840-4095.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/38400-38655.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/38656-38911.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/38912-39167.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/39168-39423.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/39424-39679.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/39680-39935.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.691070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/39936-40191.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/40192-40447.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/40448-40703.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/40704-40959.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/4096-4351.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/40960-41215.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/41216-41471.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/41472-41727.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/41728-41983.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/41984-42239.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/42240-42495.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/42496-42751.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/42752-43007.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/43008-43263.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/43264-43519.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/4352-4607.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/43520-43775.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/43776-44031.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/44032-44287.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/44288-44543.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/44544-44799.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/44800-45055.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/45056-45311.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/45312-45567.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/45568-45823.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/45824-46079.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/4608-4863.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/46080-46335.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/46336-46591.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/46592-46847.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/46848-47103.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/47104-47359.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/47360-47615.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/47616-47871.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/47872-48127.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/48128-48383.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/48384-48639.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/4864-5119.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/48640-48895.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/48896-49151.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/49152-49407.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/49408-49663.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/49664-49919.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/49920-50175.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/50176-50431.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/50432-50687.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/50688-50943.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/50944-51199.pbf
+-rw-r--r--   0        0        0     3653 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/512-767.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/5120-5375.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/51200-51455.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/51456-51711.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/51712-51967.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/51968-52223.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/52224-52479.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/52480-52735.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/52736-52991.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/52992-53247.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/53248-53503.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/53504-53759.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/5376-5631.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/53760-54015.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/54016-54271.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/54272-54527.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/54528-54783.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/54784-55039.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/55040-55295.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/55296-55551.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/55552-55807.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/55808-56063.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/56064-56319.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/5632-5887.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/56320-56575.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/56576-56831.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/56832-57087.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/57088-57343.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/57344-57599.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/57600-57855.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/57856-58111.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/58112-58367.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/58368-58623.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/58624-58879.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/5888-6143.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/58880-59135.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/59136-59391.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/59392-59647.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/59648-59903.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/59904-60159.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/60160-60415.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/60416-60671.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/60672-60927.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/60928-61183.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/61184-61439.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/6144-6399.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/61440-61695.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/61696-61951.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/61952-62207.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/62208-62463.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/62464-62719.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/62720-62975.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/62976-63231.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/63232-63487.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/63488-63743.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/63744-63999.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/6400-6655.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/64000-64255.pbf
+-rw-r--r--   0        0        0     2799 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/64256-64511.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/64512-64767.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/64768-65023.pbf
+-rw-r--r--   0        0        0       50 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/65024-65279.pbf
+-rw-r--r--   0        0        0     1643 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/65280-65535.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/6656-6911.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/6912-7167.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/7168-7423.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/7424-7679.pbf
+-rw-r--r--   0        0        0    33767 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/768-1023.pbf
+-rw-r--r--   0        0        0    55070 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/7680-7935.pbf
+-rw-r--r--   0        0        0      650 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/7936-8191.pbf
+-rw-r--r--   0        0        0     9663 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/8192-8447.pbf
+-rw-r--r--   0        0        0     5373 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/8448-8703.pbf
+-rw-r--r--   0        0        0     4875 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/8704-8959.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/8960-9215.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/9216-9471.pbf
+-rw-r--r--   0        0        0      466 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/9472-9727.pbf
+-rw-r--r--   0        0        0       32 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/9728-9983.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.695070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/9984-10239.pbf
+-rw-r--r--   0        0        0    77571 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/0-255.pbf
+-rw-r--r--   0        0        0   128493 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/1024-1279.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/10240-10495.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/10496-10751.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/10752-11007.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/11008-11263.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/11264-11519.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/11520-11775.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/11776-12031.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/12032-12287.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/12288-12543.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/12544-12799.pbf
+-rw-r--r--   0        0        0    10358 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/1280-1535.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/12800-13055.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/13056-13311.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/13312-13567.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/13568-13823.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/13824-14079.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/14080-14335.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/14336-14591.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/14592-14847.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/14848-15103.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/15104-15359.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/1536-1791.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/15360-15615.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/15616-15871.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/15872-16127.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/16128-16383.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/16384-16639.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/16640-16895.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/16896-17151.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/17152-17407.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/17408-17663.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/17664-17919.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/1792-2047.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/17920-18175.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/18176-18431.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/18432-18687.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/18688-18943.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/18944-19199.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/19200-19455.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/19456-19711.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/19712-19967.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/19968-20223.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/20224-20479.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/2048-2303.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/20480-20735.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/20736-20991.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/20992-21247.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/21248-21503.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/21504-21759.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/21760-22015.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/22016-22271.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/22272-22527.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/22528-22783.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/22784-23039.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/2304-2559.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/23040-23295.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/23296-23551.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/23552-23807.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/23808-24063.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/24064-24319.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/24320-24575.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/24576-24831.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/24832-25087.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/25088-25343.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/25344-25599.pbf
+-rw-r--r--   0        0        0    68869 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/256-511.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/2560-2815.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/25600-25855.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/25856-26111.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/26112-26367.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/26368-26623.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/26624-26879.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/26880-27135.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/27136-27391.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/27392-27647.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/27648-27903.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/27904-28159.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/2816-3071.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/28160-28415.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/28416-28671.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/28672-28927.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/28928-29183.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/29184-29439.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/29440-29695.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/29696-29951.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/29952-30207.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/30208-30463.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/30464-30719.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/3072-3327.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/30720-30975.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/30976-31231.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/31232-31487.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/31488-31743.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/31744-31999.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/32000-32255.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/32256-32511.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/32512-32767.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/32768-33023.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/33024-33279.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/3328-3583.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/33280-33535.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/33536-33791.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/33792-34047.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/34048-34303.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/34304-34559.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/34560-34815.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/34816-35071.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/35072-35327.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/35328-35583.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/35584-35839.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/3584-3839.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/35840-36095.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/36096-36351.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/36352-36607.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/36608-36863.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.707070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/36864-37119.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/37120-37375.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/37376-37631.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/37632-37887.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/37888-38143.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/38144-38399.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/3840-4095.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/38400-38655.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/38656-38911.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/38912-39167.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/39168-39423.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/39424-39679.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/39680-39935.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/39936-40191.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/40192-40447.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/40448-40703.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/40704-40959.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/4096-4351.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/40960-41215.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/41216-41471.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/41472-41727.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/41728-41983.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/41984-42239.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/42240-42495.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/42496-42751.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/42752-43007.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/43008-43263.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/43264-43519.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/4352-4607.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/43520-43775.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/43776-44031.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/44032-44287.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/44288-44543.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/44544-44799.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/44800-45055.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/45056-45311.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/45312-45567.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/45568-45823.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/45824-46079.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/4608-4863.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/46080-46335.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/46336-46591.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/46592-46847.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/46848-47103.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/47104-47359.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/47360-47615.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/47616-47871.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/47872-48127.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/48128-48383.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/48384-48639.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/4864-5119.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/48640-48895.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/48896-49151.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/49152-49407.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/49408-49663.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/49664-49919.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/49920-50175.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/50176-50431.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/50432-50687.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/50688-50943.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/50944-51199.pbf
+-rw-r--r--   0        0        0     3823 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/512-767.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/5120-5375.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/51200-51455.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/51456-51711.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/51712-51967.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/51968-52223.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/52224-52479.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/52480-52735.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/52736-52991.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/52992-53247.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/53248-53503.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/53504-53759.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/5376-5631.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/53760-54015.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/54016-54271.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/54272-54527.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/54528-54783.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/54784-55039.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/55040-55295.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/55296-55551.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/55552-55807.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/55808-56063.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/56064-56319.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/5632-5887.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/56320-56575.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/56576-56831.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/56832-57087.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/57088-57343.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/57344-57599.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/57600-57855.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/57856-58111.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/58112-58367.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/58368-58623.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/58624-58879.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/5888-6143.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/58880-59135.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/59136-59391.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/59392-59647.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/59648-59903.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/59904-60159.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/60160-60415.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/60416-60671.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/60672-60927.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/60928-61183.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/61184-61439.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/6144-6399.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/61440-61695.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/61696-61951.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/61952-62207.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/62208-62463.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/62464-62719.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/62720-62975.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/62976-63231.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/63232-63487.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/63488-63743.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/63744-63999.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/6400-6655.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/64000-64255.pbf
+-rw-r--r--   0        0        0     3040 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/64256-64511.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/64512-64767.pbf
+-rw-r--r--   0        0        0       35 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/64768-65023.pbf
+-rw-r--r--   0        0        0       51 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/65024-65279.pbf
+-rw-r--r--   0        0        0     1644 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/65280-65535.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/6656-6911.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/6912-7167.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/7168-7423.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/7424-7679.pbf
+-rw-r--r--   0        0        0    35063 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/768-1023.pbf
+-rw-r--r--   0        0        0    57819 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/7680-7935.pbf
+-rw-r--r--   0        0        0      697 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/7936-8191.pbf
+-rw-r--r--   0        0        0    10092 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/8192-8447.pbf
+-rw-r--r--   0        0        0     5512 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/8448-8703.pbf
+-rw-r--r--   0        0        0     5072 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/8704-8959.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/8960-9215.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/9216-9471.pbf
+-rw-r--r--   0        0        0      467 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/9472-9727.pbf
+-rw-r--r--   0        0        0       33 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/9728-9983.pbf
+-rw-r--r--   0        0        0       34 2023-04-13 15:12:35.711070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/9984-10239.pbf
+-rw-r--r--   0        0        0    80678 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/0-255.pbf
+-rw-r--r--   0        0        0   130485 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/1024-1279.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/10240-10495.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/10496-10751.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/10752-11007.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/11008-11263.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/11264-11519.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/11520-11775.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/11776-12031.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/12032-12287.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/12288-12543.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/12544-12799.pbf
+-rw-r--r--   0        0        0     9992 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/1280-1535.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/12800-13055.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/13056-13311.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/13312-13567.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/13568-13823.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/13824-14079.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/14080-14335.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/14336-14591.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/14592-14847.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/14848-15103.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/15104-15359.pbf
+-rw-r--r--   0        0        0       40 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/1536-1791.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/15360-15615.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/15616-15871.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/15872-16127.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/16128-16383.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/16384-16639.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/16640-16895.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/16896-17151.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/17152-17407.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/17408-17663.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/17664-17919.pbf
+-rw-r--r--   0        0        0       40 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/1792-2047.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/17920-18175.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/18176-18431.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/18432-18687.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/18688-18943.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/18944-19199.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/19200-19455.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/19456-19711.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/19712-19967.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/19968-20223.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/20224-20479.pbf
+-rw-r--r--   0        0        0       40 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/2048-2303.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/20480-20735.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/20736-20991.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/20992-21247.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/21248-21503.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/21504-21759.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/21760-22015.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/22016-22271.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/22272-22527.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/22528-22783.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/22784-23039.pbf
+-rw-r--r--   0        0        0       40 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/2304-2559.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/23040-23295.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/23296-23551.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/23552-23807.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/23808-24063.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/24064-24319.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/24320-24575.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/24576-24831.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/24832-25087.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/25088-25343.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/25344-25599.pbf
+-rw-r--r--   0        0        0    72562 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/256-511.pbf
+-rw-r--r--   0        0        0       40 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/2560-2815.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/25600-25855.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/25856-26111.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/26112-26367.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/26368-26623.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/26624-26879.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/26880-27135.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/27136-27391.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/27392-27647.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/27648-27903.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/27904-28159.pbf
+-rw-r--r--   0        0        0       40 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/2816-3071.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/28160-28415.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/28416-28671.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/28672-28927.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/28928-29183.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/29184-29439.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/29440-29695.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/29696-29951.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/29952-30207.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/30208-30463.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/30464-30719.pbf
+-rw-r--r--   0        0        0       40 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/3072-3327.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/30720-30975.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/30976-31231.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/31232-31487.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/31488-31743.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/31744-31999.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/32000-32255.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/32256-32511.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/32512-32767.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/32768-33023.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/33024-33279.pbf
+-rw-r--r--   0        0        0       40 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/3328-3583.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/33280-33535.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/33536-33791.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/33792-34047.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/34048-34303.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/34304-34559.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/34560-34815.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/34816-35071.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/35072-35327.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/35328-35583.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/35584-35839.pbf
+-rw-r--r--   0        0        0       40 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/3584-3839.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/35840-36095.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/36096-36351.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/36352-36607.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/36608-36863.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/36864-37119.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/37120-37375.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/37376-37631.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/37632-37887.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/37888-38143.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/38144-38399.pbf
+-rw-r--r--   0        0        0       40 2023-04-13 15:12:35.699070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/3840-4095.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/38400-38655.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/38656-38911.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/38912-39167.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/39168-39423.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/39424-39679.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/39680-39935.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/39936-40191.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/40192-40447.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/40448-40703.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/40704-40959.pbf
+-rw-r--r--   0        0        0       40 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/4096-4351.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/40960-41215.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/41216-41471.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/41472-41727.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/41728-41983.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/41984-42239.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/42240-42495.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/42496-42751.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/42752-43007.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/43008-43263.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/43264-43519.pbf
+-rw-r--r--   0        0        0       40 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/4352-4607.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/43520-43775.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/43776-44031.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/44032-44287.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/44288-44543.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/44544-44799.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/44800-45055.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/45056-45311.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/45312-45567.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/45568-45823.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/45824-46079.pbf
+-rw-r--r--   0        0        0       40 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/4608-4863.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/46080-46335.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/46336-46591.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/46592-46847.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/46848-47103.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/47104-47359.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/47360-47615.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/47616-47871.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/47872-48127.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/48128-48383.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/48384-48639.pbf
+-rw-r--r--   0        0        0       40 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/4864-5119.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/48640-48895.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/48896-49151.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/49152-49407.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/49408-49663.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/49664-49919.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/49920-50175.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/50176-50431.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/50432-50687.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/50688-50943.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/50944-51199.pbf
+-rw-r--r--   0        0        0     3901 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/512-767.pbf
+-rw-r--r--   0        0        0       40 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/5120-5375.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/51200-51455.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/51456-51711.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/51712-51967.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/51968-52223.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/52224-52479.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/52480-52735.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/52736-52991.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/52992-53247.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/53248-53503.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/53504-53759.pbf
+-rw-r--r--   0        0        0       40 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/5376-5631.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/53760-54015.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/54016-54271.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/54272-54527.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/54528-54783.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/54784-55039.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/55040-55295.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/55296-55551.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/55552-55807.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/55808-56063.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/56064-56319.pbf
+-rw-r--r--   0        0        0       40 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/5632-5887.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/56320-56575.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/56576-56831.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/56832-57087.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/57088-57343.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/57344-57599.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/57600-57855.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/57856-58111.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/58112-58367.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/58368-58623.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/58624-58879.pbf
+-rw-r--r--   0        0        0       40 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/5888-6143.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/58880-59135.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/59136-59391.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/59392-59647.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/59648-59903.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/59904-60159.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/60160-60415.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/60416-60671.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/60672-60927.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/60928-61183.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/61184-61439.pbf
+-rw-r--r--   0        0        0       40 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/6144-6399.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/61440-61695.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/61696-61951.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/61952-62207.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/62208-62463.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/62464-62719.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/62720-62975.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/62976-63231.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/63232-63487.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/63488-63743.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/63744-63999.pbf
+-rw-r--r--   0        0        0       40 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/6400-6655.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/64000-64255.pbf
+-rw-r--r--   0        0        0     4343 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/64256-64511.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/64512-64767.pbf
+-rw-r--r--   0        0        0       42 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/64768-65023.pbf
+-rw-r--r--   0        0        0       58 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/65024-65279.pbf
+-rw-r--r--   0        0        0     1651 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/65280-65535.pbf
+-rw-r--r--   0        0        0       40 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/6656-6911.pbf
+-rw-r--r--   0        0        0       40 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/6912-7167.pbf
+-rw-r--r--   0        0        0       40 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/7168-7423.pbf
+-rw-r--r--   0        0        0       40 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/7424-7679.pbf
+-rw-r--r--   0        0        0    35606 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/768-1023.pbf
+-rw-r--r--   0        0        0    59631 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/7680-7935.pbf
+-rw-r--r--   0        0        0      681 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/7936-8191.pbf
+-rw-r--r--   0        0        0    10489 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/8192-8447.pbf
+-rw-r--r--   0        0        0     5413 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/8448-8703.pbf
+-rw-r--r--   0        0        0     4971 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/8704-8959.pbf
+-rw-r--r--   0        0        0       40 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/8960-9215.pbf
+-rw-r--r--   0        0        0       40 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/9216-9471.pbf
+-rw-r--r--   0        0        0      451 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/9472-9727.pbf
+-rw-r--r--   0        0        0       40 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/9728-9983.pbf
+-rw-r--r--   0        0        0       41 2023-04-13 15:12:35.703070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/9984-10239.pbf
+-rw-r--r--   0        0        0     5984 2023-04-13 15:12:35.715070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/maplibre/LICENSE.txt
+-rw-r--r--   0        0        0    70412 2023-04-13 15:12:35.715070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/maplibre/maplibre-gl.css
+-rw-r--r--   0        0        0   745424 2023-04-13 15:12:35.719070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/maplibre/maplibre-gl.js
+-rw-r--r--   0        0        0     6899 2023-04-13 15:12:35.719070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/sprites/sprite.json
+-rw-r--r--   0        0        0    17411 2023-04-13 15:12:35.719070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/sprites/sprite.png
+-rw-r--r--   0        0        0     6958 2023-04-13 15:12:35.719070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/sprites/sprite@2x.json
+-rw-r--r--   0        0        0    44709 2023-04-13 15:12:35.719070 django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/sprites/sprite@2x.png
+-rw-r--r--   0        0        0      225 2023-04-13 15:12:35.719070 django_tiles_gl-0.3.8/django_tiles_gl/templates/django_tiles_gl/maplibre_head.html
+-rw-r--r--   0        0        0    70896 2023-04-13 15:12:35.719070 django_tiles_gl-0.3.8/django_tiles_gl/templates/django_tiles_gl/style.json
+-rw-r--r--   0        0        0        0 2023-04-13 15:12:35.719070 django_tiles_gl-0.3.8/django_tiles_gl/templatetags/__init__.py
+-rw-r--r--   0        0        0      158 2023-04-13 15:12:35.719070 django_tiles_gl-0.3.8/django_tiles_gl/templatetags/tiles_gl_tags.py
+-rw-r--r--   0        0        0      326 2023-04-13 15:12:35.719070 django_tiles_gl-0.3.8/django_tiles_gl/urls.py
+-rw-r--r--   0        0        0      483 2023-04-13 15:12:35.719070 django_tiles_gl-0.3.8/django_tiles_gl/utils.py
+-rw-r--r--   0        0        0     3855 2023-04-13 15:12:35.719070 django_tiles_gl-0.3.8/django_tiles_gl/views.py
+-rw-r--r--   0        0        0     1055 2023-04-13 15:12:35.719070 django_tiles_gl-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     6182 1970-01-01 00:00:00.000000 django_tiles_gl-0.3.8/PKG-INFO
```

### Comparing `django_tiles_gl-0.3.7/LICENSE.md` & `django_tiles_gl-0.3.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/README.md` & `django_tiles_gl-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/mbtiles.py` & `django_tiles_gl-0.3.8/django_tiles_gl/mbtiles.py`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/0-255.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/0-255.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/1024-1279.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/1024-1279.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/1280-1535.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/1280-1535.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/256-511.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/256-511.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/512-767.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/512-767.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/64256-64511.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/64256-64511.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/65280-65535.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/65280-65535.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/768-1023.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/768-1023.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/7680-7935.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/7680-7935.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/7936-8191.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/7936-8191.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/8192-8447.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/8192-8447.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/8448-8703.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/8448-8703.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/8704-8959.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold/8704-8959.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/0-255.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/0-255.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/1024-1279.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/1024-1279.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/1280-1535.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/1280-1535.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/256-511.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/256-511.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/512-767.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/512-767.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/64256-64511.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/64256-64511.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/65280-65535.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/65280-65535.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/768-1023.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/768-1023.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/7680-7935.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/7680-7935.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/7936-8191.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/7936-8191.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/8192-8447.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/8192-8447.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/8448-8703.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/8448-8703.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/8704-8959.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Bold Italic/8704-8959.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/0-255.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/0-255.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/1024-1279.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/1024-1279.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/1280-1535.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/1280-1535.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/256-511.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/256-511.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/512-767.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/512-767.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/64256-64511.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/64256-64511.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/65280-65535.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/65280-65535.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/768-1023.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/768-1023.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/7680-7935.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/7680-7935.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/7936-8191.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/7936-8191.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/8192-8447.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/8192-8447.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/8448-8703.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/8448-8703.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/8704-8959.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold/8704-8959.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/0-255.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/0-255.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/1024-1279.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/1024-1279.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/1280-1535.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/1280-1535.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/256-511.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/256-511.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/512-767.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/512-767.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/64256-64511.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/64256-64511.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/65280-65535.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/65280-65535.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/768-1023.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/768-1023.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/7680-7935.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/7680-7935.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/7936-8191.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/7936-8191.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/8192-8447.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/8192-8447.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/8448-8703.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/8448-8703.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/8704-8959.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Extra Bold Italic/8704-8959.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/0-255.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/0-255.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/1024-1279.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/1024-1279.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/1280-1535.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/1280-1535.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/256-511.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/256-511.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/512-767.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/512-767.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/64256-64511.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/64256-64511.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/65280-65535.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/65280-65535.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/768-1023.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/768-1023.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/7680-7935.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/7680-7935.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/7936-8191.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/7936-8191.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/8192-8447.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/8192-8447.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/8448-8703.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/8448-8703.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/8704-8959.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Italic/8704-8959.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/0-255.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/0-255.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/1024-1279.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/1024-1279.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/1280-1535.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/1280-1535.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/256-511.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/256-511.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/512-767.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/512-767.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/64256-64511.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/64256-64511.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/65280-65535.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/65280-65535.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/768-1023.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/768-1023.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/7680-7935.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/7680-7935.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/7936-8191.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/7936-8191.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/8192-8447.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/8192-8447.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/8448-8703.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/8448-8703.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/8704-8959.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light/8704-8959.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/0-255.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/0-255.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/1024-1279.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/1024-1279.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/1280-1535.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/1280-1535.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/256-511.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/256-511.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/512-767.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/512-767.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/64256-64511.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/64256-64511.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/65280-65535.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/65280-65535.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/768-1023.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/768-1023.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/7680-7935.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/7680-7935.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/7936-8191.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/7936-8191.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/8192-8447.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/8192-8447.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/8448-8703.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/8448-8703.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/8704-8959.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Light Italic/8704-8959.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/0-255.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/0-255.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/1024-1279.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/1024-1279.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/1280-1535.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/1280-1535.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/256-511.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/256-511.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/512-767.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/512-767.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/64256-64511.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/64256-64511.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/65280-65535.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/65280-65535.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/768-1023.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/768-1023.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/7680-7935.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/7680-7935.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/7936-8191.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/7936-8191.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/8192-8447.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/8192-8447.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/8448-8703.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/8448-8703.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/8704-8959.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Regular/8704-8959.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/0-255.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/0-255.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/1024-1279.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/1024-1279.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/1280-1535.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/1280-1535.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/256-511.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/256-511.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/512-767.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/512-767.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/64256-64511.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/64256-64511.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/65280-65535.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/65280-65535.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/768-1023.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/768-1023.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/7680-7935.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/7680-7935.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/7936-8191.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/7936-8191.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/8192-8447.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/8192-8447.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/8448-8703.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/8448-8703.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/8704-8959.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold/8704-8959.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/0-255.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/0-255.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/1024-1279.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/1024-1279.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/1280-1535.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/1280-1535.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/256-511.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/256-511.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/512-767.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/512-767.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/64256-64511.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/64256-64511.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/65280-65535.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/65280-65535.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/768-1023.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/768-1023.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/7680-7935.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/7680-7935.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/7936-8191.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/7936-8191.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/8192-8447.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/8192-8447.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/8448-8703.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/8448-8703.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/8704-8959.pbf` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/fonts/Open Sans Semibold Italic/8704-8959.pbf`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/maplibre/LICENSE.txt` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/maplibre/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/maplibre/maplibre-gl.css` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/maplibre/maplibre-gl.css`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/maplibre/maplibre-gl.js` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/maplibre/maplibre-gl.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -25168,9 +25168,8 @@
 
     //
 
     var maplibregl$1 = maplibregl;
 
     return maplibregl$1;
 
-}));
-//# sourceMappingURL=maplibre-gl.js.map
+}));
```

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/sprites/sprite.json` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/sprites/sprite.json`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/sprites/sprite.png` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/sprites/sprite.png`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/sprites/sprite@2x.json` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/sprites/sprite@2x.json`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/static/django-tiles-gl/sprites/sprite@2x.png` & `django_tiles_gl-0.3.8/django_tiles_gl/static/django-tiles-gl/sprites/sprite@2x.png`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/templates/django_tiles_gl/style.json` & `django_tiles_gl-0.3.8/django_tiles_gl/templates/django_tiles_gl/style.json`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/django_tiles_gl/views.py` & `django_tiles_gl-0.3.8/django_tiles_gl/views.py`

 * *Files identical despite different names*

### Comparing `django_tiles_gl-0.3.7/pyproject.toml` & `django_tiles_gl-0.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-tiles-gl"
-version = "0.3.7"
+version = "0.3.8"
 description = "Integrated Django Vector Tile Server based on mbtiles"
 readme = "README.md"
 authors = ["Johannes Dillmann <dev@ae35.de>"]
 license = "BSD-3-Clause"
 homepage = "https://github.com/kleingeist/django-tiles-gl"
 repository = "https://github.com/kleingeist/django-tiles-gl"
 keywords = ["django", "map", "mbtiles",]
```

### Comparing `django_tiles_gl-0.3.7/setup.py` & `django_tiles_gl-0.3.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,148 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: django-tiles-gl
+Version: 0.3.8
+Summary: Integrated Django Vector Tile Server based on mbtiles
+Home-page: https://github.com/kleingeist/django-tiles-gl
+License: BSD-3-Clause
+Keywords: django,map,mbtiles
+Author: Johannes Dillmann
+Author-email: dev@ae35.de
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3
+Classifier: Framework :: Django :: 4
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: GIS
+Requires-Dist: Django (>=3.1,<4.2)
+Project-URL: Repository, https://github.com/kleingeist/django-tiles-gl
+Description-Content-Type: text/markdown
 
-packages = \
-['django_tiles_gl', 'django_tiles_gl.templatetags']
+# Django Tiles GL
 
-package_data = \
-{'': ['*'],
- 'django_tiles_gl': ['static/django-tiles-gl/fonts/Open Sans Bold Italic/*',
-                     'static/django-tiles-gl/fonts/Open Sans Bold/*',
-                     'static/django-tiles-gl/fonts/Open Sans Extra Bold '
-                     'Italic/*',
-                     'static/django-tiles-gl/fonts/Open Sans Extra Bold/*',
-                     'static/django-tiles-gl/fonts/Open Sans Italic/*',
-                     'static/django-tiles-gl/fonts/Open Sans Light Italic/*',
-                     'static/django-tiles-gl/fonts/Open Sans Light/*',
-                     'static/django-tiles-gl/fonts/Open Sans Regular/*',
-                     'static/django-tiles-gl/fonts/Open Sans Semibold Italic/*',
-                     'static/django-tiles-gl/fonts/Open Sans Semibold/*',
-                     'static/django-tiles-gl/maplibre/*',
-                     'static/django-tiles-gl/sprites/*',
-                     'templates/django_tiles_gl/*']}
-
-install_requires = \
-['Django>=3.1,<4.2']
-
-setup_kwargs = {
-    'name': 'django-tiles-gl',
-    'version': '0.3.7',
-    'description': 'Integrated Django Vector Tile Server based on mbtiles',
-    'long_description': '# Django Tiles GL\n\nIntegrated Django Vector Tile Server based on mbtiles.\n\n\n## Description\n\nSimple app to serve [Mabpox Vector Tiles](https://docs.mapbox.com/data/tilesets/guides/vector-tiles-standards/) directly from [MBTiles files](https://github.com/mapbox/mbtiles-spec) via Django views.\n\nDjango Tiles has a minimal dependencies. It does not require GeoDjano or any other libraries. Its only dependency is Django itself.\n\nDjango Tiles GL **does not create raster tiles**. It may only be used with map libraries that support to render vector tiles like  [MapLibre](https://maplibre.org/) or [OpenLayers](https://openlayers.org/).\n\nDjango Tiles GL contains the [OSM Bright map style](https://openmaptiles.org/styles/#osm-bright) which can be used to render Vector Tiles following the [OpenMapTiles vector tile  schema](https://openmaptiles.org/schema).\n\nNote that this default style is using [OpenSans fonts](https://github.com/openmaptiles/fonts) which does only contain Latin, Greek and Cyrillic alphabets.\n\nOther tile schemes are possible by creating a custom [map style specification](https://docs.mapbox.com/mapbox-gl-js/style-spec/) and referencing Django Tiles GL [TileJSON endpoint](https://github.com/mapbox/tilejson-spec) as a source.\n\n## Usage\n\nSee the [`demo`](https://github.com/kleingeist/django-tiles-gl/tree/main/demo) Django application for a simple usage example.\n\n\n### Setup\n\n- Add `django_tiles_gl` to you `INSTALLED_APPS` setting.\n- Add `django_tiles_gl.urls` to your url patterns.\n  For example with the `tiles` prefix:\n  ```python\n  urlpatterns = [\n      ...\n      path("tiles/", include("django_tiles_gl.urls")),\n  ]\n  ```\n- Set path to your MBTiles files in you application settings.\n  ```python\n  MBTILES_DATABASE = BASE_DIR / "demo" / "data" / "berlin.mbtiles"\n  ```\n- Optionally set the default center to be set on the default map style.\n  ```python\n  MBTILES_CENTER = [13.4, 52.5, 13]   # [longitude, latitude, zoom]\n  ```\n- Optionally force absolute urls to use SSL by prefixing them with "https://".\n  This might be required if you app is running behind a reverse proxy and you\n  are not able to set [`SECURE_PROXY_SSL_HEADER`](https://docs.djangoproject.com/en/4.0/ref/settings/#secure-proxy-ssl-header)\n  from the SSL enabled proxy server.\n  ```python\n  MBTILES_FORCE_SSL = True\n  ```\n\n### Views\nTo render a map you have to include a JavaScript mapping library and refer to the `tile` endpoint or the default integrated style.\n\nDjango Tiles GL provides the following endpoints:\n\n- `{% url \'django_tiles_gl:openmaptiles_style\' %}` - Default [OpenMapTiles style defintion](https://openmaptiles.org) using the [OSM Bright map style](https://openmaptiles.org/styles/#osm-bright).\n- `{% url \'django_tiles_gl:tilejson\' %}` - [TileJSON](https://github.com/mapbox/tilejson-spec) describing the configured MBTiles files and providing the correct tile urls.\n- `{% url \'django_tiles_gl:tile\' x y z %}` - Actual tile endpoint, returning vector data in the [PBF format](https://wiki.openstreetmap.org/wiki/PBF_Format).\n\n\nDjango Tiles GL is bundles with [MapLibre](https://maplibre.org/) and provides a template tag for easy inclusion. A minimal working example has to contain the following defintions:\n\n```html\n{% load tiles_gl_tags %}\n<!DOCTYPE html>\n<html>\n<head>\n    {% maplibre_head %}\n\n    <style>\n        body { margin:0; padding:0; }\n        #map { position:absolute; top:0; bottom:0; width:100%; }\n    </style>\n</head>\n<body>\n\n<div id=\'map\'></div>\n\n<script>\nvar map = new maplibregl.Map({\n\tcontainer: \'map\',\n\tstyle: \'{% url \'django_tiles_gl:openmaptiles_style\' %}\',\n});\n</script>\n\n</body>\n</html>\n```\n\n## Data / MBTiles generation\n\nThere are mutiple tools to generate valid MBTiles databases. The easiest to use with Django Tiles GL is [OpenMapTiles](https://github.com/openmaptiles/openmaptiles) as it is compatible with the bundled default style.\n\nFor a quickstart you may generate the MbTiles for an area with the following commands:\n```sh\ngit clone https://github.com/openmaptiles/openmaptiles.git\ncd openmaptiles\n./quickstart.sh <area>\n```\n\nFo further information and optiones see [https://github.com/openmaptiles/openmaptiles](https://github.com/openmaptiles/openmaptiles)\n\n\n\n## Further Topics\n\n### Caching\n\nIt is advised setup a caching proxy for the `tile` endpoint. Please refer to you HTTP servers documentation. For example the [nginx proxy cache config](https://nginx.org/en/docs/http/ngx_http_proxy_module.html#proxy_cache)\n\n\n\n## Other Django tile server solutions\n\n- [django-geojson-tiles](https://github.com/glenrobertson/django-geojson-tiles) - Generates GeoJSON tiles from a GeoDjango model. No MBTiles support.  Not to be used as a base layer.\n\n- [django-vectortiles](https://github.com/submarcos/django-vectortiles) - Generates Vector Tile layers from GeoDjango. No MBTiles support. Not to be used as a base layer.\n\n- [django-mbtiles](https://github.com/makinacorpus/django-mbtiles) - Uses MBTiles to generate rastered tiles and [UTFGrid](https://github.com/mapbox/mbtiles-spec/blob/master/1.1/utfgrid.md). Does not support modern vector tiles. Strong inspiration for this project.\n',
-    'author': 'Johannes Dillmann',
-    'author_email': 'dev@ae35.de',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/kleingeist/django-tiles-gl',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+Integrated Django Vector Tile Server based on mbtiles.
 
 
-setup(**setup_kwargs)
+## Description
+
+Simple app to serve [Mabpox Vector Tiles](https://docs.mapbox.com/data/tilesets/guides/vector-tiles-standards/) directly from [MBTiles files](https://github.com/mapbox/mbtiles-spec) via Django views.
+
+Django Tiles has a minimal dependencies. It does not require GeoDjano or any other libraries. Its only dependency is Django itself.
+
+Django Tiles GL **does not create raster tiles**. It may only be used with map libraries that support to render vector tiles like  [MapLibre](https://maplibre.org/) or [OpenLayers](https://openlayers.org/).
+
+Django Tiles GL contains the [OSM Bright map style](https://openmaptiles.org/styles/#osm-bright) which can be used to render Vector Tiles following the [OpenMapTiles vector tile  schema](https://openmaptiles.org/schema).
+
+Note that this default style is using [OpenSans fonts](https://github.com/openmaptiles/fonts) which does only contain Latin, Greek and Cyrillic alphabets.
+
+Other tile schemes are possible by creating a custom [map style specification](https://docs.mapbox.com/mapbox-gl-js/style-spec/) and referencing Django Tiles GL [TileJSON endpoint](https://github.com/mapbox/tilejson-spec) as a source.
+
+## Usage
+
+See the [`demo`](https://github.com/kleingeist/django-tiles-gl/tree/main/demo) Django application for a simple usage example.
+
+
+### Setup
+
+- Add `django_tiles_gl` to you `INSTALLED_APPS` setting.
+- Add `django_tiles_gl.urls` to your url patterns.
+  For example with the `tiles` prefix:
+  ```python
+  urlpatterns = [
+      ...
+      path("tiles/", include("django_tiles_gl.urls")),
+  ]
+  ```
+- Set path to your MBTiles files in you application settings.
+  ```python
+  MBTILES_DATABASE = BASE_DIR / "demo" / "data" / "berlin.mbtiles"
+  ```
+- Optionally set the default center to be set on the default map style.
+  ```python
+  MBTILES_CENTER = [13.4, 52.5, 13]   # [longitude, latitude, zoom]
+  ```
+- Optionally force absolute urls to use SSL by prefixing them with "https://".
+  This might be required if you app is running behind a reverse proxy and you
+  are not able to set [`SECURE_PROXY_SSL_HEADER`](https://docs.djangoproject.com/en/4.0/ref/settings/#secure-proxy-ssl-header)
+  from the SSL enabled proxy server.
+  ```python
+  MBTILES_FORCE_SSL = True
+  ```
+
+### Views
+To render a map you have to include a JavaScript mapping library and refer to the `tile` endpoint or the default integrated style.
+
+Django Tiles GL provides the following endpoints:
+
+- `{% url 'django_tiles_gl:openmaptiles_style' %}` - Default [OpenMapTiles style defintion](https://openmaptiles.org) using the [OSM Bright map style](https://openmaptiles.org/styles/#osm-bright).
+- `{% url 'django_tiles_gl:tilejson' %}` - [TileJSON](https://github.com/mapbox/tilejson-spec) describing the configured MBTiles files and providing the correct tile urls.
+- `{% url 'django_tiles_gl:tile' x y z %}` - Actual tile endpoint, returning vector data in the [PBF format](https://wiki.openstreetmap.org/wiki/PBF_Format).
+
+
+Django Tiles GL is bundles with [MapLibre](https://maplibre.org/) and provides a template tag for easy inclusion. A minimal working example has to contain the following defintions:
+
+```html
+{% load tiles_gl_tags %}
+<!DOCTYPE html>
+<html>
+<head>
+    {% maplibre_head %}
+
+    <style>
+        body { margin:0; padding:0; }
+        #map { position:absolute; top:0; bottom:0; width:100%; }
+    </style>
+</head>
+<body>
+
+<div id='map'></div>
+
+<script>
+var map = new maplibregl.Map({
+	container: 'map',
+	style: '{% url 'django_tiles_gl:openmaptiles_style' %}',
+});
+</script>
+
+</body>
+</html>
+```
+
+## Data / MBTiles generation
+
+There are mutiple tools to generate valid MBTiles databases. The easiest to use with Django Tiles GL is [OpenMapTiles](https://github.com/openmaptiles/openmaptiles) as it is compatible with the bundled default style.
+
+For a quickstart you may generate the MbTiles for an area with the following commands:
+```sh
+git clone https://github.com/openmaptiles/openmaptiles.git
+cd openmaptiles
+./quickstart.sh <area>
+```
+
+Fo further information and optiones see [https://github.com/openmaptiles/openmaptiles](https://github.com/openmaptiles/openmaptiles)
+
+
+
+## Further Topics
+
+### Caching
+
+It is advised setup a caching proxy for the `tile` endpoint. Please refer to you HTTP servers documentation. For example the [nginx proxy cache config](https://nginx.org/en/docs/http/ngx_http_proxy_module.html#proxy_cache)
+
+
+
+## Other Django tile server solutions
+
+- [django-geojson-tiles](https://github.com/glenrobertson/django-geojson-tiles) - Generates GeoJSON tiles from a GeoDjango model. No MBTiles support.  Not to be used as a base layer.
+
+- [django-vectortiles](https://github.com/submarcos/django-vectortiles) - Generates Vector Tile layers from GeoDjango. No MBTiles support. Not to be used as a base layer.
+
+- [django-mbtiles](https://github.com/makinacorpus/django-mbtiles) - Uses MBTiles to generate rastered tiles and [UTFGrid](https://github.com/mapbox/mbtiles-spec/blob/master/1.1/utfgrid.md). Does not support modern vector tiles. Strong inspiration for this project.
+
```

