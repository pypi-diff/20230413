# Comparing `tmp/MapProxy-1.9.0.tar.gz` & `tmp/MapProxy-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MapProxy-1.9.0.tar", last modified: Fri Jul 22 08:01:24 2016, max compression
+gzip compressed data, was "dist/MapProxy-1.9.1.tar", last modified: Wed Jan 18 14:24:16 2017, max compression
```

## Comparing `MapProxy-1.9.0.tar` & `MapProxy-1.9.1.tar`

### file list

```diff
@@ -1,588 +1,590 @@
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/
--rw-r--r--   0 olt        (501) staff       (20)    22355 2016-07-22 07:40:29.000000 MapProxy-1.9.0/CHANGES.txt
--rw-r--r--   0 olt        (501) staff       (20)     1903 2013-12-10 14:17:57.000000 MapProxy-1.9.0/COPYING.txt
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/doc/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/doc/_static/
--rw-r--r--   0 olt        (501) staff       (20)     1368 2012-04-23 07:43:43.000000 MapProxy-1.9.0/doc/_static/logo.png
--rw-r--r--   0 olt        (501) staff       (20)      760 2016-04-20 09:59:38.000000 MapProxy-1.9.0/doc/_static/mapproxy.css
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/doc/_templates/
--rw-r--r--   0 olt        (501) staff       (20)      950 2016-04-20 09:59:38.000000 MapProxy-1.9.0/doc/_templates/layout.html
--rw-r--r--   0 olt        (501) staff       (20)     1210 2016-04-20 09:59:38.000000 MapProxy-1.9.0/doc/_templates/navbar.html
--rwxr-xr-x   0 olt        (501) staff       (20)       15 2015-04-08 07:53:15.000000 MapProxy-1.9.0/doc/_templates/toctree.html
--rw-r--r--   0 olt        (501) staff       (20)    19527 2015-02-04 07:28:26.000000 MapProxy-1.9.0/doc/auth.rst
--rw-r--r--   0 olt        (501) staff       (20)     9864 2016-04-20 09:59:38.000000 MapProxy-1.9.0/doc/caches.rst
--rw-r--r--   0 olt        (501) staff       (20)     6663 2016-07-22 07:45:13.000000 MapProxy-1.9.0/doc/conf.py
--rw-r--r--   0 olt        (501) staff       (20)    40232 2016-05-19 09:09:18.000000 MapProxy-1.9.0/doc/configuration.rst
--rw-r--r--   0 olt        (501) staff       (20)    29224 2016-06-30 11:25:20.000000 MapProxy-1.9.0/doc/configuration_examples.rst
--rw-r--r--   0 olt        (501) staff       (20)     3749 2015-02-04 07:28:26.000000 MapProxy-1.9.0/doc/coverages.rst
--rw-r--r--   0 olt        (501) staff       (20)     4472 2015-02-04 07:28:26.000000 MapProxy-1.9.0/doc/decorate_img.rst
--rw-r--r--   0 olt        (501) staff       (20)    15158 2016-04-20 09:59:38.000000 MapProxy-1.9.0/doc/deployment.rst
--rw-r--r--   0 olt        (501) staff       (20)     4781 2015-04-08 07:53:15.000000 MapProxy-1.9.0/doc/development.rst
--rw-r--r--   0 olt        (501) staff       (20)   102253 2013-04-25 08:38:23.000000 MapProxy-1.9.0/doc/GM.txt
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/doc/imgs/
--rw-r--r--   0 olt        (501) staff       (20)    20437 2012-04-23 07:43:43.000000 MapProxy-1.9.0/doc/imgs/bicubic.png
--rw-r--r--   0 olt        (501) staff       (20)    18588 2012-04-23 07:43:43.000000 MapProxy-1.9.0/doc/imgs/bilinear.png
--rw-r--r--   0 olt        (501) staff       (20)     7633 2012-04-23 07:43:43.000000 MapProxy-1.9.0/doc/imgs/labeling-dynamic.png
--rw-r--r--   0 olt        (501) staff       (20)     6825 2012-04-23 07:43:43.000000 MapProxy-1.9.0/doc/imgs/labeling-meta-buffer.png
--rw-r--r--   0 olt        (501) staff       (20)     4011 2012-04-23 07:43:43.000000 MapProxy-1.9.0/doc/imgs/labeling-metatiling-buffer.png
--rw-r--r--   0 olt        (501) staff       (20)     2594 2012-04-23 07:43:43.000000 MapProxy-1.9.0/doc/imgs/labeling-metatiling.png
--rw-r--r--   0 olt        (501) staff       (20)     7765 2012-04-23 07:43:43.000000 MapProxy-1.9.0/doc/imgs/labeling-no-clip.png
--rw-r--r--   0 olt        (501) staff       (20)     5092 2012-04-23 07:43:43.000000 MapProxy-1.9.0/doc/imgs/labeling-no-placement.png
--rw-r--r--   0 olt        (501) staff       (20)     5321 2012-04-23 07:43:43.000000 MapProxy-1.9.0/doc/imgs/labeling-partial-false.png
--rw-r--r--   0 olt        (501) staff       (20)     6567 2012-04-23 07:43:43.000000 MapProxy-1.9.0/doc/imgs/labeling-repeated.png
--rw-r--r--   0 olt        (501) staff       (20)    32025 2015-04-08 07:53:15.000000 MapProxy-1.9.0/doc/imgs/mapnik-webmerc-hq.png
--rw-r--r--   0 olt        (501) staff       (20)    12649 2015-04-08 07:53:15.000000 MapProxy-1.9.0/doc/imgs/mapnik-webmerc.png
--rw-r--r--   0 olt        (501) staff       (20)    18652 2013-04-25 08:38:23.000000 MapProxy-1.9.0/doc/imgs/mapproxy-demo.png
--rw-r--r--   0 olt        (501) staff       (20)    15501 2012-04-23 07:43:43.000000 MapProxy-1.9.0/doc/imgs/nearest.png
--rw-r--r--   0 olt        (501) staff       (20)      483 2016-02-10 12:08:11.000000 MapProxy-1.9.0/doc/index.rst
--rw-r--r--   0 olt        (501) staff       (20)     5265 2016-02-10 12:08:11.000000 MapProxy-1.9.0/doc/inspire.rst
--rw-r--r--   0 olt        (501) staff       (20)     8021 2016-02-10 12:08:11.000000 MapProxy-1.9.0/doc/install.rst
--rw-r--r--   0 olt        (501) staff       (20)     2540 2015-02-04 07:28:26.000000 MapProxy-1.9.0/doc/install_osgeo4w.rst
--rw-r--r--   0 olt        (501) staff       (20)     4461 2016-02-10 12:08:11.000000 MapProxy-1.9.0/doc/install_windows.rst
--rw-r--r--   0 olt        (501) staff       (20)    10699 2015-04-08 07:53:15.000000 MapProxy-1.9.0/doc/labeling.rst
--rw-r--r--   0 olt        (501) staff       (20)     3435 2016-04-20 09:59:38.000000 MapProxy-1.9.0/doc/Makefile
--rw-r--r--   0 olt        (501) staff       (20)     2042 2016-02-10 12:08:11.000000 MapProxy-1.9.0/doc/mapproxy_2.rst
--rw-r--r--   0 olt        (501) staff       (20)    16579 2016-05-10 09:45:16.000000 MapProxy-1.9.0/doc/mapproxy_util.rst
--rw-r--r--   0 olt        (501) staff       (20)     5174 2015-02-04 07:28:26.000000 MapProxy-1.9.0/doc/mapproxy_util_autoconfig.rst
--rw-r--r--   0 olt        (501) staff       (20)    14561 2016-04-20 09:59:38.000000 MapProxy-1.9.0/doc/seed.rst
--rw-r--r--   0 olt        (501) staff       (20)     2379 2016-03-08 10:35:31.000000 MapProxy-1.9.0/doc/seed2.rst
--rw-r--r--   0 olt        (501) staff       (20)    13221 2016-04-20 09:59:38.000000 MapProxy-1.9.0/doc/services.rst
--rw-r--r--   0 olt        (501) staff       (20)    17263 2016-06-30 11:25:20.000000 MapProxy-1.9.0/doc/sources.rst
--rw-r--r--   0 olt        (501) staff       (20)    15008 2016-04-20 09:59:38.000000 MapProxy-1.9.0/doc/tutorial.rst
--rw-r--r--   0 olt        (501) staff       (20)     2444 2013-12-10 14:17:57.000000 MapProxy-1.9.0/doc/tutorial.yaml
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/doc/yaml/
--rw-r--r--   0 olt        (501) staff       (20)     1076 2013-04-25 08:38:23.000000 MapProxy-1.9.0/doc/yaml/cache_conf.yaml
--rw-r--r--   0 olt        (501) staff       (20)     1148 2013-04-25 08:38:23.000000 MapProxy-1.9.0/doc/yaml/grid_conf.yaml
--rw-r--r--   0 olt        (501) staff       (20)     1178 2013-04-25 08:38:23.000000 MapProxy-1.9.0/doc/yaml/merged_conf.yaml
--rw-r--r--   0 olt        (501) staff       (20)     1188 2013-04-25 08:38:23.000000 MapProxy-1.9.0/doc/yaml/meta_conf.yaml
--rw-r--r--   0 olt        (501) staff       (20)      195 2013-04-25 08:38:23.000000 MapProxy-1.9.0/doc/yaml/seed.yaml
--rw-r--r--   0 olt        (501) staff       (20)      926 2013-04-25 08:38:23.000000 MapProxy-1.9.0/doc/yaml/simple_conf.yaml
--rw-r--r--   0 olt        (501) staff       (20)    11358 2012-04-23 07:43:43.000000 MapProxy-1.9.0/LICENSE.txt
--rw-r--r--   0 olt        (501) staff       (20)      860 2016-02-10 12:08:11.000000 MapProxy-1.9.0/MANIFEST.in
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/
--rw-r--r--   0 olt        (501) staff       (20)       55 2013-11-23 11:35:51.000000 MapProxy-1.9.0/mapproxy/__init__.py
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/cache/
--rw-r--r--   0 olt        (501) staff       (20)     1255 2013-11-23 11:35:51.000000 MapProxy-1.9.0/mapproxy/cache/__init__.py
--rw-r--r--   0 olt        (501) staff       (20)     3292 2015-07-30 08:03:02.000000 MapProxy-1.9.0/mapproxy/cache/base.py
--rw-r--r--   0 olt        (501) staff       (20)    10779 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/cache/couchdb.py
--rw-r--r--   0 olt        (501) staff       (20)     1064 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/cache/dummy.py
--rw-r--r--   0 olt        (501) staff       (20)    12739 2016-04-20 09:59:38.000000 MapProxy-1.9.0/mapproxy/cache/file.py
--rw-r--r--   0 olt        (501) staff       (20)     2719 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/cache/legend.py
--rw-r--r--   0 olt        (501) staff       (20)    11620 2016-04-20 09:59:38.000000 MapProxy-1.9.0/mapproxy/cache/mbtiles.py
--rw-r--r--   0 olt        (501) staff       (20)     2459 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/cache/meta.py
--rw-r--r--   0 olt        (501) staff       (20)     3438 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/cache/renderd.py
--rw-r--r--   0 olt        (501) staff       (20)     6482 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/cache/riak.py
--rw-r--r--   0 olt        (501) staff       (20)    14294 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/cache/sqlite.py
--rw-r--r--   0 olt        (501) staff       (20)    16906 2016-05-11 08:29:26.000000 MapProxy-1.9.0/mapproxy/cache/tile.py
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/client/
--rw-r--r--   0 olt        (501) staff       (20)        0 2013-11-23 11:35:51.000000 MapProxy-1.9.0/mapproxy/client/__init__.py
--rw-r--r--   0 olt        (501) staff       (20)     1323 2016-05-12 11:05:09.000000 MapProxy-1.9.0/mapproxy/client/arcgis.py
--rw-r--r--   0 olt        (501) staff       (20)     4672 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/client/cgi.py
--rw-r--r--   0 olt        (501) staff       (20)    10298 2016-03-15 14:53:54.000000 MapProxy-1.9.0/mapproxy/client/http.py
--rw-r--r--   0 olt        (501) staff       (20)     1236 2013-11-23 11:35:51.000000 MapProxy-1.9.0/mapproxy/client/log.py
--rw-r--r--   0 olt        (501) staff       (20)     5668 2016-03-01 13:31:26.000000 MapProxy-1.9.0/mapproxy/client/tile.py
--rw-r--r--   0 olt        (501) staff       (20)     8720 2016-05-10 07:04:51.000000 MapProxy-1.9.0/mapproxy/client/wms.py
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/compat/
--rw-r--r--   0 olt        (501) staff       (20)      771 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/compat/__init__.py
--rw-r--r--   0 olt        (501) staff       (20)     2834 2016-05-11 08:29:26.000000 MapProxy-1.9.0/mapproxy/compat/image.py
--rw-r--r--   0 olt        (501) staff       (20)      395 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/compat/itertools.py
--rw-r--r--   0 olt        (501) staff       (20)      151 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/compat/modules.py
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/config/
--rw-r--r--   0 olt        (501) staff       (20)      945 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/config/__init__.py
--rw-r--r--   0 olt        (501) staff       (20)     6682 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/config/config.py
--rw-r--r--   0 olt        (501) staff       (20)     2878 2015-08-24 15:01:14.000000 MapProxy-1.9.0/mapproxy/config/coverage.py
--rw-r--r--   0 olt        (501) staff       (20)     2650 2016-03-15 14:53:54.000000 MapProxy-1.9.0/mapproxy/config/defaults.py
--rw-r--r--   0 olt        (501) staff       (20)    74612 2016-06-15 08:41:51.000000 MapProxy-1.9.0/mapproxy/config/loader.py
--rw-r--r--   0 olt        (501) staff       (20)    15256 2016-06-15 08:30:34.000000 MapProxy-1.9.0/mapproxy/config/spec.py
--rw-r--r--   0 olt        (501) staff       (20)     8876 2016-05-11 08:29:26.000000 MapProxy-1.9.0/mapproxy/config/validator.py
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/config_template/
--rw-r--r--   0 olt        (501) staff       (20)      451 2013-11-23 11:35:51.000000 MapProxy-1.9.0/mapproxy/config_template/__init__.py
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/config_template/base_config/
--rw-r--r--   0 olt        (501) staff       (20)      384 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/config_template/base_config/config.wsgi
--rw-r--r--   0 olt        (501) staff       (20)    17806 2015-04-08 07:30:13.000000 MapProxy-1.9.0/mapproxy/config_template/base_config/full_example.yaml
--rw-r--r--   0 olt        (501) staff       (20)     2320 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/config_template/base_config/full_seed_example.yaml
--rw-r--r--   0 olt        (501) staff       (20)      649 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/config_template/base_config/log.ini
--rw-r--r--   0 olt        (501) staff       (20)     1493 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/config_template/base_config/mapproxy.yaml
--rw-r--r--   0 olt        (501) staff       (20)      529 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/config_template/base_config/seed.yaml
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/config_template/paster/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/config_template/paster/etc/
--rw-r--r--   0 olt        (501) staff       (20)      418 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/config_template/paster/etc/config.ini
--rw-r--r--   0 olt        (501) staff       (20)      169 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/config_template/paster/etc/config.wsgi
--rw-r--r--   0 olt        (501) staff       (20)      612 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/config_template/paster/etc/develop.ini
--rw-r--r--   0 olt        (501) staff       (20)      734 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/config_template/paster/etc/log_deploy.ini
--rw-r--r--   0 olt        (501) staff       (20)     4056 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/config_template/paster/etc/mapproxy.yaml
--rw-r--r--   0 olt        (501) staff       (20)     1071 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/config_template/paster/etc/seed.yaml
--rw-r--r--   0 olt        (501) staff       (20)     4526 2013-11-23 11:35:51.000000 MapProxy-1.9.0/mapproxy/exception.py
--rw-r--r--   0 olt        (501) staff       (20)     4662 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/featureinfo.py
--rw-r--r--   0 olt        (501) staff       (20)    38801 2016-05-19 09:12:50.000000 MapProxy-1.9.0/mapproxy/grid.py
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/image/
--rw-r--r--   0 olt        (501) staff       (20)    15583 2016-06-15 08:30:34.000000 MapProxy-1.9.0/mapproxy/image/__init__.py
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/image/fonts/
--rw-r--r--   0 olt        (501) staff       (20)        0 2013-11-23 11:35:51.000000 MapProxy-1.9.0/mapproxy/image/fonts/__init__.py
--rw-r--r--   0 olt        (501) staff       (20)   622020 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/image/fonts/DejaVuSans.ttf
--rw-r--r--   0 olt        (501) staff       (20)   320812 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/image/fonts/DejaVuSansMono.ttf
--rw-r--r--   0 olt        (501) staff       (20)     4816 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/image/fonts/LICENSE
--rw-r--r--   0 olt        (501) staff       (20)     2106 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/image/mask.py
--rw-r--r--   0 olt        (501) staff       (20)    10381 2016-05-20 09:42:04.000000 MapProxy-1.9.0/mapproxy/image/merge.py
--rw-r--r--   0 olt        (501) staff       (20)    12216 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/image/message.py
--rw-r--r--   0 olt        (501) staff       (20)     5412 2016-05-10 09:45:16.000000 MapProxy-1.9.0/mapproxy/image/opts.py
--rw-r--r--   0 olt        (501) staff       (20)     5951 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/image/tile.py
--rw-r--r--   0 olt        (501) staff       (20)     8933 2016-05-10 07:49:25.000000 MapProxy-1.9.0/mapproxy/image/transform.py
--rw-r--r--   0 olt        (501) staff       (20)    15459 2016-05-20 09:52:29.000000 MapProxy-1.9.0/mapproxy/layer.py
--rw-r--r--   0 olt        (501) staff       (20)     7614 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/multiapp.py
--rw-r--r--   0 olt        (501) staff       (20)     8047 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/proj.py
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/request/
--rw-r--r--   0 olt        (501) staff       (20)      737 2013-11-23 11:35:51.000000 MapProxy-1.9.0/mapproxy/request/__init__.py
--rw-r--r--   0 olt        (501) staff       (20)     4212 2016-05-12 11:05:09.000000 MapProxy-1.9.0/mapproxy/request/arcgis.py
--rw-r--r--   0 olt        (501) staff       (20)    14968 2015-05-08 08:57:23.000000 MapProxy-1.9.0/mapproxy/request/base.py
--rw-r--r--   0 olt        (501) staff       (20)     4172 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/request/tile.py
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/request/wms/
--rw-r--r--   0 olt        (501) staff       (20)    26808 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/request/wms/__init__.py
--rw-r--r--   0 olt        (501) staff       (20)     3481 2013-12-10 14:17:57.000000 MapProxy-1.9.0/mapproxy/request/wms/exception.py
--rw-r--r--   0 olt        (501) staff       (20)    12838 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/request/wmts.py
--rw-r--r--   0 olt        (501) staff       (20)     7699 2016-06-30 11:24:28.000000 MapProxy-1.9.0/mapproxy/response.py
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/script/
--rw-r--r--   0 olt        (501) staff       (20)        0 2013-11-23 11:35:51.000000 MapProxy-1.9.0/mapproxy/script/__init__.py
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/script/conf/
--rw-r--r--   0 olt        (501) staff       (20)        0 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/script/conf/__init__.py
--rw-r--r--   0 olt        (501) staff       (20)     6906 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/script/conf/app.py
--rw-r--r--   0 olt        (501) staff       (20)     1272 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/script/conf/caches.py
--rw-r--r--   0 olt        (501) staff       (20)     1473 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/script/conf/layers.py
--rw-r--r--   0 olt        (501) staff       (20)     1253 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/script/conf/seeds.py
--rw-r--r--   0 olt        (501) staff       (20)     2271 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/script/conf/sources.py
--rw-r--r--   0 olt        (501) staff       (20)     5237 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/script/conf/utils.py
--rw-r--r--   0 olt        (501) staff       (20)     8816 2016-05-10 09:45:16.000000 MapProxy-1.9.0/mapproxy/script/export.py
--rw-r--r--   0 olt        (501) staff       (20)     7411 2016-06-30 11:25:20.000000 MapProxy-1.9.0/mapproxy/script/grids.py
--rw-r--r--   0 olt        (501) staff       (20)     4181 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/script/scales.py
--rwxr-xr-x   0 olt        (501) staff       (20)    12917 2016-04-20 09:59:38.000000 MapProxy-1.9.0/mapproxy/script/util.py
--rw-r--r--   0 olt        (501) staff       (20)     6049 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/script/wms_capabilities.py
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/seed/
--rw-r--r--   0 olt        (501) staff       (20)        0 2013-11-23 11:35:51.000000 MapProxy-1.9.0/mapproxy/seed/__init__.py
--rw-r--r--   0 olt        (501) staff       (20)     3758 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/seed/cachelock.py
--rw-r--r--   0 olt        (501) staff       (20)     3867 2015-04-08 09:27:41.000000 MapProxy-1.9.0/mapproxy/seed/cleanup.py
--rw-r--r--   0 olt        (501) staff       (20)    17613 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/seed/config.py
--rw-r--r--   0 olt        (501) staff       (20)    11300 2016-04-20 09:59:38.000000 MapProxy-1.9.0/mapproxy/seed/script.py
--rw-r--r--   0 olt        (501) staff       (20)    17485 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/seed/seeder.py
--rw-r--r--   0 olt        (501) staff       (20)     2204 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/seed/spec.py
--rw-r--r--   0 olt        (501) staff       (20)     9538 2016-05-10 09:45:16.000000 MapProxy-1.9.0/mapproxy/seed/util.py
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/service/
--rw-r--r--   0 olt        (501) staff       (20)      646 2013-11-23 11:35:51.000000 MapProxy-1.9.0/mapproxy/service/__init__.py
--rw-r--r--   0 olt        (501) staff       (20)     1692 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/service/base.py
--rw-r--r--   0 olt        (501) staff       (20)    11137 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/service/demo.py
--rw-r--r--   0 olt        (501) staff       (20)    12350 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/service/kml.py
--rw-r--r--   0 olt        (501) staff       (20)     1357 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/service/ows.py
--rw-r--r--   0 olt        (501) staff       (20)     2236 2015-08-11 06:53:54.000000 MapProxy-1.9.0/mapproxy/service/template_helper.py
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/service/templates/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/service/templates/demo/
--rw-r--r--   0 olt        (501) staff       (20)      457 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/service/templates/demo/capabilities_demo.html
--rw-r--r--   0 olt        (501) staff       (20)     8027 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/service/templates/demo/demo.html
--rw-r--r--   0 olt        (501) staff       (20)      272 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/service/templates/demo/openlayers-demo.cfg
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/service/templates/demo/static/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/service/templates/demo/static/img/
--rw-r--r--   0 olt        (501) staff       (20)       42 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/service/templates/demo/static/img/blank.gif
--rw-r--r--   0 olt        (501) staff       (20)      451 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/service/templates/demo/static/img/east-mini.png
--rw-r--r--   0 olt        (501) staff       (20)      484 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/service/templates/demo/static/img/north-mini.png
--rw-r--r--   0 olt        (501) staff       (20)      481 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/service/templates/demo/static/img/south-mini.png
--rw-r--r--   0 olt        (501) staff       (20)      453 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/service/templates/demo/static/img/west-mini.png
--rw-r--r--   0 olt        (501) staff       (20)      359 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/service/templates/demo/static/img/zoom-minus-mini.png
--rw-r--r--   0 olt        (501) staff       (20)      489 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/service/templates/demo/static/img/zoom-plus-mini.png
--rw-r--r--   0 olt        (501) staff       (20)     1072 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/service/templates/demo/static/img/zoom-world-mini.png
--rw-r--r--   0 olt        (501) staff       (20)     1368 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/service/templates/demo/static/logo.png
--rw-r--r--   0 olt        (501) staff       (20)   163900 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/service/templates/demo/static/OpenLayers.js
--rw-r--r--   0 olt        (501) staff       (20)     1994 2013-12-10 14:17:57.000000 MapProxy-1.9.0/mapproxy/service/templates/demo/static/site.css
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/service/templates/demo/static/theme/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/service/templates/demo/static/theme/default/
--rw-r--r--   0 olt        (501) staff       (20)        0 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/service/templates/demo/static/theme/default/framedCloud.css
--rw-r--r--   0 olt        (501) staff       (20)      303 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/service/templates/demo/static/theme/default/google.css
--rw-r--r--   0 olt        (501) staff       (20)      212 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/service/templates/demo/static/theme/default/ie6-style.css
--rw-r--r--   0 olt        (501) staff       (20)     9892 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/service/templates/demo/static/theme/default/style.css
--rw-r--r--   0 olt        (501) staff       (20)      966 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/service/templates/demo/static.html
--rw-r--r--   0 olt        (501) staff       (20)     3300 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/service/templates/demo/tms_demo.html
--rw-r--r--   0 olt        (501) staff       (20)     3083 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/service/templates/demo/wms_demo.html
--rw-r--r--   0 olt        (501) staff       (20)     2949 2016-05-10 15:21:46.000000 MapProxy-1.9.0/mapproxy/service/templates/demo/wmts_demo.html
--rw-r--r--   0 olt        (501) staff       (20)      463 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/service/templates/tms_capabilities.xml
--rw-r--r--   0 olt        (501) staff       (20)      101 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/service/templates/tms_exception.xml
--rw-r--r--   0 olt        (501) staff       (20)      227 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/service/templates/tms_root_resource.xml
--rw-r--r--   0 olt        (501) staff       (20)      694 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/service/templates/tms_tilemap_capabilities.xml
--rw-r--r--   0 olt        (501) staff       (20)     2853 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/service/templates/wms100capabilities.xml
--rw-r--r--   0 olt        (501) staff       (20)       82 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/service/templates/wms100exception.xml
--rw-r--r--   0 olt        (501) staff       (20)     5458 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/service/templates/wms110capabilities.xml
--rw-r--r--   0 olt        (501) staff       (20)      291 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/service/templates/wms110exception.xml
--rw-r--r--   0 olt        (501) staff       (20)     6457 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/service/templates/wms111capabilities.xml
--rw-r--r--   0 olt        (501) staff       (20)      291 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/service/templates/wms111exception.xml
--rw-r--r--   0 olt        (501) staff       (20)    12954 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/service/templates/wms130capabilities.xml
--rw-r--r--   0 olt        (501) staff       (20)      392 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/service/templates/wms130exception.xml
--rw-r--r--   0 olt        (501) staff       (20)     4968 2015-11-12 14:37:50.000000 MapProxy-1.9.0/mapproxy/service/templates/wmts100capabilities.xml
--rw-r--r--   0 olt        (501) staff       (20)      483 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/service/templates/wmts100exception.xml
--rw-r--r--   0 olt        (501) staff       (20)    18478 2015-11-17 08:15:29.000000 MapProxy-1.9.0/mapproxy/service/tile.py
--rw-r--r--   0 olt        (501) staff       (20)    31057 2016-05-13 13:38:53.000000 MapProxy-1.9.0/mapproxy/service/wms.py
--rw-r--r--   0 olt        (501) staff       (20)    11836 2016-06-14 11:54:52.000000 MapProxy-1.9.0/mapproxy/service/wmts.py
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/source/
--rw-r--r--   0 olt        (501) staff       (20)     2346 2016-06-15 08:30:34.000000 MapProxy-1.9.0/mapproxy/source/__init__.py
--rw-r--r--   0 olt        (501) staff       (20)     1086 2016-05-12 11:05:09.000000 MapProxy-1.9.0/mapproxy/source/arcgis.py
--rw-r--r--   0 olt        (501) staff       (20)     1447 2013-11-26 14:44:55.000000 MapProxy-1.9.0/mapproxy/source/error.py
--rw-r--r--   0 olt        (501) staff       (20)     5514 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/source/mapnik.py
--rw-r--r--   0 olt        (501) staff       (20)     3667 2016-05-13 13:51:17.000000 MapProxy-1.9.0/mapproxy/source/tile.py
--rw-r--r--   0 olt        (501) staff       (20)     9418 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/source/wms.py
--rw-r--r--   0 olt        (501) staff       (20)    13654 2015-09-14 11:09:04.000000 MapProxy-1.9.0/mapproxy/srs.py
--rw-r--r--   0 olt        (501) staff       (20)     1930 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/template.py
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/test/
--rw-r--r--   0 olt        (501) staff       (20)        0 2013-11-23 11:35:51.000000 MapProxy-1.9.0/mapproxy/test/__init__.py
--rw-r--r--   0 olt        (501) staff       (20)     7181 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/helper.py
--rw-r--r--   0 olt        (501) staff       (20)    15532 2016-04-20 09:59:38.000000 MapProxy-1.9.0/mapproxy/test/http.py
--rw-r--r--   0 olt        (501) staff       (20)     6538 2015-04-08 11:32:54.000000 MapProxy-1.9.0/mapproxy/test/image.py
--rw-r--r--   0 olt        (501) staff       (20)    83748 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/mocker.py
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/test/schemas/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/
--rw-r--r--   0 olt        (501) staff       (20)    62819 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/common.xsd
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/
--rw-r--r--   0 olt        (501) staff       (20)     6026 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_bul.xsd
--rw-r--r--   0 olt        (501) staff       (20)     5108 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_cze.xsd
--rw-r--r--   0 olt        (501) staff       (20)     4988 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_dan.xsd
--rw-r--r--   0 olt        (501) staff       (20)     5150 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_dut.xsd
--rw-r--r--   0 olt        (501) staff       (20)     6464 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_eng.xsd
--rw-r--r--   0 olt        (501) staff       (20)     4945 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_est.xsd
--rw-r--r--   0 olt        (501) staff       (20)     5002 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_fin.xsd
--rw-r--r--   0 olt        (501) staff       (20)     5183 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_fre.xsd
--rw-r--r--   0 olt        (501) staff       (20)     5086 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_ger.xsd
--rw-r--r--   0 olt        (501) staff       (20)     5035 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_gle.xsd
--rw-r--r--   0 olt        (501) staff       (20)     6049 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_gre.xsd
--rw-r--r--   0 olt        (501) staff       (20)     5098 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_hun.xsd
--rw-r--r--   0 olt        (501) staff       (20)     5092 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_ita.xsd
--rw-r--r--   0 olt        (501) staff       (20)     5094 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_lav.xsd
--rw-r--r--   0 olt        (501) staff       (20)     5096 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_lit.xsd
--rw-r--r--   0 olt        (501) staff       (20)     4984 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_mlt.xsd
--rw-r--r--   0 olt        (501) staff       (20)     5150 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_pol.xsd
--rw-r--r--   0 olt        (501) staff       (20)     5099 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_por.xsd
--rw-r--r--   0 olt        (501) staff       (20)     5100 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_rum.xsd
--rw-r--r--   0 olt        (501) staff       (20)     5053 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_slo.xsd
--rw-r--r--   0 olt        (501) staff       (20)     5022 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_slv.xsd
--rw-r--r--   0 olt        (501) staff       (20)     5177 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_spa.xsd
--rw-r--r--   0 olt        (501) staff       (20)     5024 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_swe.xsd
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/examples/
--rw-r--r--   0 olt        (501) staff       (20)     4997 2011-04-26 14:20:06.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/examples/inspireresourcemddataset.xml
--rw-r--r--   0 olt        (501) staff       (20)     4800 2011-04-26 14:19:14.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/examples/inspireresourcemdseries.xml
--rw-r--r--   0 olt        (501) staff       (20)     4805 2011-04-26 14:19:48.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/examples/inspireresourcemdservice.xml
--rw-r--r--   0 olt        (501) staff       (20)    28131 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/network.xsd
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/inspire_vs/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/inspire_vs/1.0/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/inspire_vs/1.0/examples/
--rw-r--r--   0 olt        (501) staff       (20)    18083 2011-04-26 13:41:44.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/inspire_vs/1.0/examples/wms_at.xml
--rw-r--r--   0 olt        (501) staff       (20)    17428 2011-04-26 13:41:42.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/inspire_vs/1.0/examples/wms_geoimage.xml
--rw-r--r--   0 olt        (501) staff       (20)    15455 2011-04-26 13:41:42.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/inspire_vs/1.0/examples/WMS_Image2000GetCapabilities_InspireSchema.xml
--rw-r--r--   0 olt        (501) staff       (20)     1561 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/test/schemas/inspire/inspire_vs/1.0/inspire_vs.xsd
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/test/schemas/kml/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/test/schemas/kml/2.2.0/
--rw-r--r--   0 olt        (501) staff       (20)     1973 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/kml/2.2.0/atom-author-link.xsd
--rw-r--r--   0 olt        (501) staff       (20)    66296 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/kml/2.2.0/ogckml22.xsd
--rw-r--r--   0 olt        (501) staff       (20)      462 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/kml/2.2.0/ReadMe.txt
--rw-r--r--   0 olt        (501) staff       (20)    74544 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/kml/2.2.0/xAL.xsd
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/test/schemas/ows/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/test/schemas/ows/1.1.0/
--rw-r--r--   0 olt        (501) staff       (20)    13319 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/ows/1.1.0/ows19115subset.xsd
--rw-r--r--   0 olt        (501) staff       (20)     1121 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/ows/1.1.0/owsAll.xsd
--rw-r--r--   0 olt        (501) staff       (20)    11942 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/ows/1.1.0/owsCommon.xsd
--rw-r--r--   0 olt        (501) staff       (20)     6995 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/ows/1.1.0/owsContents.xsd
--rw-r--r--   0 olt        (501) staff       (20)     7677 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/ows/1.1.0/owsDataIdentification.xsd
--rw-r--r--   0 olt        (501) staff       (20)    14363 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/ows/1.1.0/owsDomainType.xsd
--rw-r--r--   0 olt        (501) staff       (20)     4892 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/ows/1.1.0/owsExceptionReport.xsd
--rw-r--r--   0 olt        (501) staff       (20)     7265 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/ows/1.1.0/owsGetCapabilities.xsd
--rw-r--r--   0 olt        (501) staff       (20)     3295 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/ows/1.1.0/owsGetResourceByID.xsd
--rw-r--r--   0 olt        (501) staff       (20)     4190 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/ows/1.1.0/owsInputOutputData.xsd
--rw-r--r--   0 olt        (501) staff       (20)     6456 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/ows/1.1.0/owsManifest.xsd
--rw-r--r--   0 olt        (501) staff       (20)     8926 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/ows/1.1.0/owsOperationsMetadata.xsd
--rw-r--r--   0 olt        (501) staff       (20)     3573 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/ows/1.1.0/owsServiceIdentification.xsd
--rw-r--r--   0 olt        (501) staff       (20)     2279 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/ows/1.1.0/owsServiceProvider.xsd
--rw-r--r--   0 olt        (501) staff       (20)     3356 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/ows/1.1.0/ReadMe.txt
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/test/schemas/sld/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/test/schemas/sld/1.1.0/
--rw-r--r--   0 olt        (501) staff       (20)     1629 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/sld/1.1.0/sld_capabilities.xsd
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/test/schemas/wms/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/test/schemas/wms/1.0.0/
--rw-r--r--   0 olt        (501) staff       (20)    16836 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wms/1.0.0/capabilities_1_0_0.dtd
--rw-r--r--   0 olt        (501) staff       (20)     7897 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wms/1.0.0/capabilities_1_0_0.xml
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/test/schemas/wms/1.0.7/
--rw-r--r--   0 olt        (501) staff       (20)    23882 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wms/1.0.7/capabilities_1_0_7.dtd
--rw-r--r--   0 olt        (501) staff       (20)    11104 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wms/1.0.7/capabilities_1_0_7.xml
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/test/schemas/wms/1.1.0/
--rw-r--r--   0 olt        (501) staff       (20)    10158 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wms/1.1.0/capabilities_1_1_0.dtd
--rw-r--r--   0 olt        (501) staff       (20)    13161 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wms/1.1.0/capabilities_1_1_0.xml
--rw-r--r--   0 olt        (501) staff       (20)      205 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wms/1.1.0/exception_1_1_0.dtd
--rw-r--r--   0 olt        (501) staff       (20)     1081 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wms/1.1.0/exception_1_1_0.xml
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/test/schemas/wms/1.1.1/
--rw-r--r--   0 olt        (501) staff       (20)    10505 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wms/1.1.1/capabilities_1_1_1.dtd
--rw-r--r--   0 olt        (501) staff       (20)    13178 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wms/1.1.1/capabilities_1_1_1.xml
--rw-r--r--   0 olt        (501) staff       (20)      205 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wms/1.1.1/exception_1_1_1.dtd
--rw-r--r--   0 olt        (501) staff       (20)     1095 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wms/1.1.1/exception_1_1_1.xml
--rw-r--r--   0 olt        (501) staff       (20)     2852 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wms/1.1.1/OGC-exception.xsd
--rw-r--r--   0 olt        (501) staff       (20)     1465 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wms/1.1.1/WMS_DescribeLayerResponse.dtd
--rw-r--r--   0 olt        (501) staff       (20)      204 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wms/1.1.1/WMS_exception_1_1_1.dtd
--rw-r--r--   0 olt        (501) staff       (20)    10438 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wms/1.1.1/WMS_MS_Capabilities.dtd
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/test/schemas/wms/1.3.0/
--rw-r--r--   0 olt        (501) staff       (20)    11475 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wms/1.3.0/capabilities_1_3_0.xml
--rw-r--r--   0 olt        (501) staff       (20)    21391 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wms/1.3.0/capabilities_1_3_0.xsd
--rw-r--r--   0 olt        (501) staff       (20)     1099 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wms/1.3.0/exceptions_1_3_0.xml
--rw-r--r--   0 olt        (501) staff       (20)      982 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wms/1.3.0/exceptions_1_3_0.xsd
--rw-r--r--   0 olt        (501) staff       (20)      315 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wms/1.3.0/ReadMe.txt
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/test/schemas/wmsc/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/test/schemas/wmsc/1.1.1/
--rw-r--r--   0 olt        (501) staff       (20)    10505 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wmsc/1.1.1/capabilities_1_1_1.dtd
--rw-r--r--   0 olt        (501) staff       (20)    13178 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wmsc/1.1.1/capabilities_1_1_1.xml
--rw-r--r--   0 olt        (501) staff       (20)      205 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wmsc/1.1.1/exception_1_1_1.dtd
--rw-r--r--   0 olt        (501) staff       (20)     1095 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wmsc/1.1.1/exception_1_1_1.xml
--rw-r--r--   0 olt        (501) staff       (20)     2852 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wmsc/1.1.1/OGC-exception.xsd
--rw-r--r--   0 olt        (501) staff       (20)     1465 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wmsc/1.1.1/WMS_DescribeLayerResponse.dtd
--rw-r--r--   0 olt        (501) staff       (20)      204 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wmsc/1.1.1/WMS_exception_1_1_1.dtd
--rw-r--r--   0 olt        (501) staff       (20)    10781 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wmsc/1.1.1/WMS_MS_Capabilities.dtd
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/test/schemas/wmts/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/test/schemas/wmts/1.0/
--rw-r--r--   0 olt        (501) staff       (20)     1100 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wmts/1.0/ReadMe.txt
--rw-r--r--   0 olt        (501) staff       (20)     1203 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wmts/1.0/wmts.xsd
--rw-r--r--   0 olt        (501) staff       (20)     5540 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wmts/1.0/wmtsAbstract.wsdl
--rw-r--r--   0 olt        (501) staff       (20)     1548 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wmts/1.0/wmtsGetCapabilities_request.xsd
--rw-r--r--   0 olt        (501) staff       (20)    21708 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wmts/1.0/wmtsGetCapabilities_response.xsd
--rw-r--r--   0 olt        (501) staff       (20)     2208 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wmts/1.0/wmtsGetFeatureInfo_request.xsd
--rw-r--r--   0 olt        (501) staff       (20)     2817 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wmts/1.0/wmtsGetFeatureInfo_response.xsd
--rw-r--r--   0 olt        (501) staff       (20)     3243 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wmts/1.0/wmtsGetTile_request.xsd
--rw-r--r--   0 olt        (501) staff       (20)     2881 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wmts/1.0/wmtsKVP.xsd
--rw-r--r--   0 olt        (501) staff       (20)     2455 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/wmts/1.0/wmtsPayload_response.xsd
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/test/schemas/xlink/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/test/schemas/xlink/1.0.0/
--rw-r--r--   0 olt        (501) staff       (20)      182 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/xlink/1.0.0/ReadMe.txt
--rw-r--r--   0 olt        (501) staff       (20)     5249 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/xlink/1.0.0/xlinks.xsd
--rw-r--r--   0 olt        (501) staff       (20)     8836 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/schemas/xml.xsd
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/test/system/
--rw-r--r--   0 olt        (501) staff       (20)     3468 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/system/__init__.py
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/
--rw-r--r--   0 olt        (501) staff       (20)      986 2016-05-12 11:05:09.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/arcgis.yaml
--rw-r--r--   0 olt        (501) staff       (20)     1226 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/auth.yaml
--rw-r--r--   0 olt        (501) staff       (20)     8192 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/cache.mbtiles
--rw-r--r--   0 olt        (501) staff       (20)     1470 2016-05-11 08:29:26.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/cache_band_merge.yaml
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/cache_data/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/cache_data/dop_cache_EPSG3857/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/cache_data/dop_cache_EPSG3857/00/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/cache_data/dop_cache_EPSG3857/00/000/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/cache_data/dop_cache_EPSG3857/00/000/000/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/cache_data/dop_cache_EPSG3857/00/000/000/000/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/cache_data/dop_cache_EPSG3857/00/000/000/000/000/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/cache_data/dop_cache_EPSG3857/00/000/000/000/000/000/
--rwxr-xr-x   0 olt        (501) staff       (20)      760 2016-05-11 08:29:26.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/cache_data/dop_cache_EPSG3857/00/000/000/000/000/000/000.png
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/cache_data/wms_cache_EPSG900913/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/cache_data/wms_cache_EPSG900913/01/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/cache_data/wms_cache_EPSG900913/01/000/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/cache_data/wms_cache_EPSG900913/01/000/000/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/cache_data/wms_cache_EPSG900913/01/000/000/000/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/cache_data/wms_cache_EPSG900913/01/000/000/000/000/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/cache_data/wms_cache_EPSG900913/01/000/000/000/000/000/
--rw-r--r--   0 olt        (501) staff       (20)    10214 2015-04-09 13:02:34.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/cache_data/wms_cache_EPSG900913/01/000/000/000/000/000/001.jpeg
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/cache_data/wms_cache_transparent_EPSG900913/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/cache_data/wms_cache_transparent_EPSG900913/01/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/cache_data/wms_cache_transparent_EPSG900913/01/000/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/cache_data/wms_cache_transparent_EPSG900913/01/000/000/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/cache_data/wms_cache_transparent_EPSG900913/01/000/000/000/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/cache_data/wms_cache_transparent_EPSG900913/01/000/000/000/000/
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/cache_data/wms_cache_transparent_EPSG900913/01/000/000/000/000/000/
--rw-r--r--   0 olt        (501) staff       (20)      463 2015-04-09 13:02:34.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/cache_data/wms_cache_transparent_EPSG900913/01/000/000/000/000/000/001.png
--rw-r--r--   0 olt        (501) staff       (20)      844 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/cache_grid_names.yaml
--rw-r--r--   0 olt        (501) staff       (20)      410 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/cache_mbtiles.yaml
--rw-r--r--   0 olt        (501) staff       (20)     1556 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/cache_source.yaml
--rw-r--r--   0 olt        (501) staff       (20)      611 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/cgi.py
--rw-r--r--   0 olt        (501) staff       (20)     2780 2013-12-10 14:17:57.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/combined_sources.yaml
--rw-r--r--   0 olt        (501) staff       (20)     1955 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/coverage.yaml
--rw-r--r--   0 olt        (501) staff       (20)      376 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/disable_storage.yaml
--rw-r--r--   0 olt        (501) staff       (20)       45 2013-12-10 14:17:57.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/empty_ogrdata.geojson
--rw-r--r--   0 olt        (501) staff       (20)     1926 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/formats.yaml
--rw-r--r--   0 olt        (501) staff       (20)     2943 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/inspire.yaml
--rw-r--r--   0 olt        (501) staff       (20)     3756 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/inspire_full.yaml
--rw-r--r--   0 olt        (501) staff       (20)     1332 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/kml_layer.yaml
--rw-r--r--   0 olt        (501) staff       (20)     6066 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/layer.yaml
--rw-r--r--   0 olt        (501) staff       (20)     1042 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/layergroups.yaml
--rw-r--r--   0 olt        (501) staff       (20)     1722 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/layergroups_root.yaml
--rw-r--r--   0 olt        (501) staff       (20)     2471 2013-04-25 08:38:23.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/legendgraphic.yaml
--rw-r--r--   0 olt        (501) staff       (20)     1053 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/mapnik_source.yaml
--rw-r--r--   0 olt        (501) staff       (20)      193 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/mapproxy_export.yaml
--rw-r--r--   0 olt        (501) staff       (20)      350 2013-04-25 08:38:23.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/mapserver.yaml
--rw-r--r--   0 olt        (501) staff       (20)     1186 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/mixed_mode.yaml
--rw-r--r--   0 olt        (501) staff       (20)     2265 2016-04-20 09:59:38.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/multi_cache_layers.yaml
--rw-r--r--   0 olt        (501) staff       (20)      299 2013-04-25 08:38:23.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/multiapp1.yaml
--rw-r--r--   0 olt        (501) staff       (20)      291 2013-04-25 08:38:23.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/multiapp2.yaml
--rw-r--r--   0 olt        (501) staff       (20)      999 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/renderd_client.yaml
--rw-r--r--   0 olt        (501) staff       (20)     1729 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/scalehints.yaml
--rw-r--r--   0 olt        (501) staff       (20)     1755 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/seed.yaml
--rw-r--r--   0 olt        (501) staff       (20)      608 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/seed_mapproxy.yaml
--rw-r--r--   0 olt        (501) staff       (20)      176 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/seed_old.yaml
--rw-r--r--   0 olt        (501) staff       (20)      216 2013-04-25 08:38:23.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/seed_timeouts.yaml
--rw-r--r--   0 olt        (501) staff       (20)      427 2013-04-25 08:38:23.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/seed_timeouts_mapproxy.yaml
--rw-r--r--   0 olt        (501) staff       (20)     1245 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/seedonly.yaml
--rw-r--r--   0 olt        (501) staff       (20)      661 2013-04-25 08:38:23.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/sld.yaml
--rw-r--r--   0 olt        (501) staff       (20)     1724 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/source_errors.yaml
--rw-r--r--   0 olt        (501) staff       (20)     1723 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/source_errors_raise.yaml
--rw-r--r--   0 olt        (501) staff       (20)      376 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/tileservice_origin.yaml
--rw-r--r--   0 olt        (501) staff       (20)      448 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/tilesource_minmax_res.yaml
--rw-r--r--   0 olt        (501) staff       (20)       97 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/util-conf-base-grids.yaml
--rw-r--r--   0 olt        (501) staff       (20)      224 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/util-conf-overwrite.yaml
--rw-r--r--   0 olt        (501) staff       (20)     3883 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/util-conf-wms-111-cap.xml
--rw-r--r--   0 olt        (501) staff       (20)      669 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/util_grids.yaml
--rw-r--r--   0 olt        (501) staff       (20)     6060 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/util_wms_capabilities111.xml
--rw-r--r--   0 olt        (501) staff       (20)     4440 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/util_wms_capabilities130.xml
--rw-r--r--   0 olt        (501) staff       (20)      304 2013-12-10 14:17:57.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/util_wms_capabilities_service_exception.xml
--rw-r--r--   0 olt        (501) staff       (20)      839 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/watermark.yaml
--rw-r--r--   0 olt        (501) staff       (20)      537 2015-04-08 07:30:13.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/wms_srs_extent.yaml
--rw-r--r--   0 olt        (501) staff       (20)     1142 2015-04-08 07:30:13.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/wms_versions.yaml
--rw-r--r--   0 olt        (501) staff       (20)     2616 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/wmts.yaml
--rw-r--r--   0 olt        (501) staff       (20)     1263 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/wmts_dimensions.yaml
--rw-r--r--   0 olt        (501) staff       (20)     1170 2013-04-25 08:38:23.000000 MapProxy-1.9.0/mapproxy/test/system/fixture/xslt_featureinfo.yaml
--rw-r--r--   0 olt        (501) staff       (20)     3311 2016-05-12 11:05:09.000000 MapProxy-1.9.0/mapproxy/test/system/test_arcgis.py
--rw-r--r--   0 olt        (501) staff       (20)    33630 2015-04-09 13:02:34.000000 MapProxy-1.9.0/mapproxy/test/system/test_auth.py
--rw-r--r--   0 olt        (501) staff       (20)     3564 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/test/system/test_behind_proxy.py
--rw-r--r--   0 olt        (501) staff       (20)     3703 2016-05-11 08:29:26.000000 MapProxy-1.9.0/mapproxy/test/system/test_cache_band_merge.py
--rw-r--r--   0 olt        (501) staff       (20)     4295 2015-04-09 13:02:34.000000 MapProxy-1.9.0/mapproxy/test/system/test_cache_grid_names.py
--rw-r--r--   0 olt        (501) staff       (20)     2628 2015-04-09 13:02:34.000000 MapProxy-1.9.0/mapproxy/test/system/test_cache_mbtiles.py
--rw-r--r--   0 olt        (501) staff       (20)     5012 2015-04-09 13:02:34.000000 MapProxy-1.9.0/mapproxy/test/system/test_cache_source.py
--rw-r--r--   0 olt        (501) staff       (20)    13027 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/system/test_combined_sources.py
--rw-r--r--   0 olt        (501) staff       (20)     5525 2015-04-09 13:02:34.000000 MapProxy-1.9.0/mapproxy/test/system/test_coverage.py
--rw-r--r--   0 olt        (501) staff       (20)     6737 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/system/test_decorate_img.py
--rw-r--r--   0 olt        (501) staff       (20)     2157 2013-11-23 11:35:51.000000 MapProxy-1.9.0/mapproxy/test/system/test_disable_storage.py
--rw-r--r--   0 olt        (501) staff       (20)     8765 2015-04-09 13:02:34.000000 MapProxy-1.9.0/mapproxy/test/system/test_formats.py
--rw-r--r--   0 olt        (501) staff       (20)     5318 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/test/system/test_inspire_vs.py
--rw-r--r--   0 olt        (501) staff       (20)    10512 2015-04-09 13:02:34.000000 MapProxy-1.9.0/mapproxy/test/system/test_kml.py
--rw-r--r--   0 olt        (501) staff       (20)     5736 2013-11-23 11:35:51.000000 MapProxy-1.9.0/mapproxy/test/system/test_layergroups.py
--rw-r--r--   0 olt        (501) staff       (20)    10585 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/system/test_legendgraphic.py
--rw-r--r--   0 olt        (501) staff       (20)     5379 2015-04-08 11:32:54.000000 MapProxy-1.9.0/mapproxy/test/system/test_mapnik.py
--rw-r--r--   0 olt        (501) staff       (20)     2294 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/system/test_mapserver.py
--rw-r--r--   0 olt        (501) staff       (20)     7073 2015-04-09 13:02:34.000000 MapProxy-1.9.0/mapproxy/test/system/test_mixed_mode_format.py
--rw-r--r--   0 olt        (501) staff       (20)     7101 2016-04-20 09:59:38.000000 MapProxy-1.9.0/mapproxy/test/system/test_multi_cache_layers.py
--rw-r--r--   0 olt        (501) staff       (20)     3391 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/system/test_multiapp.py
--rw-r--r--   0 olt        (501) staff       (20)    11857 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/test/system/test_renderd_client.py
--rw-r--r--   0 olt        (501) staff       (20)     4963 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/test/system/test_scalehints.py
--rw-r--r--   0 olt        (501) staff       (20)    18199 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/test/system/test_seed.py
--rw-r--r--   0 olt        (501) staff       (20)     3021 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/system/test_seed_only.py
--rw-r--r--   0 olt        (501) staff       (20)     3307 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/system/test_sld.py
--rw-r--r--   0 olt        (501) staff       (20)    11762 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/system/test_source_errors.py
--rw-r--r--   0 olt        (501) staff       (20)     2255 2015-04-09 13:02:34.000000 MapProxy-1.9.0/mapproxy/test/system/test_tilesource_minmax_res.py
--rw-r--r--   0 olt        (501) staff       (20)    10944 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/test/system/test_tms.py
--rw-r--r--   0 olt        (501) staff       (20)     1797 2013-12-10 14:17:57.000000 MapProxy-1.9.0/mapproxy/test/system/test_tms_origin.py
--rw-r--r--   0 olt        (501) staff       (20)     8279 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/system/test_util_conf.py
--rw-r--r--   0 olt        (501) staff       (20)     5662 2015-04-09 13:02:34.000000 MapProxy-1.9.0/mapproxy/test/system/test_util_export.py
--rw-r--r--   0 olt        (501) staff       (20)     3210 2015-04-09 13:02:34.000000 MapProxy-1.9.0/mapproxy/test/system/test_util_grids.py
--rw-r--r--   0 olt        (501) staff       (20)     5473 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/system/test_util_wms_capabilities.py
--rw-r--r--   0 olt        (501) staff       (20)     3475 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/system/test_watermark.py
--rw-r--r--   0 olt        (501) staff       (20)    57068 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/test/system/test_wms.py
--rw-r--r--   0 olt        (501) staff       (20)     4526 2015-04-08 07:30:13.000000 MapProxy-1.9.0/mapproxy/test/system/test_wms_srs_extent.py
--rw-r--r--   0 olt        (501) staff       (20)     2195 2015-04-08 07:30:13.000000 MapProxy-1.9.0/mapproxy/test/system/test_wms_version.py
--rw-r--r--   0 olt        (501) staff       (20)     4057 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/system/test_wmsc.py
--rw-r--r--   0 olt        (501) staff       (20)     6949 2016-06-14 11:57:24.000000 MapProxy-1.9.0/mapproxy/test/system/test_wmts.py
--rw-r--r--   0 olt        (501) staff       (20)     7152 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/system/test_wmts_dimensions.py
--rw-r--r--   0 olt        (501) staff       (20)     4430 2015-04-09 13:02:34.000000 MapProxy-1.9.0/mapproxy/test/system/test_wmts_restful.py
--rw-r--r--   0 olt        (501) staff       (20)    10457 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/test/system/test_xslt_featureinfo.py
--rw-r--r--   0 olt        (501) staff       (20)     7670 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/test_http_helper.py
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/test/unit/
--rw-r--r--   0 olt        (501) staff       (20)        0 2013-11-23 11:35:51.000000 MapProxy-1.9.0/mapproxy/test/unit/__init__.py
--rw-r--r--   0 olt        (501) staff       (20)       58 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/unit/epsg
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/test/unit/polygons/
--rw-r--r--   0 olt        (501) staff       (20)      833 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/unit/polygons/polygons.dbf
--rw-r--r--   0 olt        (501) staff       (20)     1580 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/unit/polygons/polygons.shp
--rw-r--r--   0 olt        (501) staff       (20)      124 2012-04-23 07:43:43.000000 MapProxy-1.9.0/mapproxy/test/unit/polygons/polygons.shx
--rw-r--r--   0 olt        (501) staff       (20)    10731 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/unit/test_async.py
--rw-r--r--   0 olt        (501) staff       (20)    15175 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/unit/test_auth.py
--rw-r--r--   0 olt        (501) staff       (20)    38652 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/test/unit/test_cache.py
--rw-r--r--   0 olt        (501) staff       (20)     4514 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/unit/test_cache_couchdb.py
--rw-r--r--   0 olt        (501) staff       (20)     2494 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/test/unit/test_cache_riak.py
--rw-r--r--   0 olt        (501) staff       (20)    12221 2016-04-20 09:59:38.000000 MapProxy-1.9.0/mapproxy/test/unit/test_cache_tile.py
--rw-r--r--   0 olt        (501) staff       (20)    15718 2016-05-20 09:51:16.000000 MapProxy-1.9.0/mapproxy/test/unit/test_client.py
--rw-r--r--   0 olt        (501) staff       (20)     4650 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/unit/test_client_cgi.py
--rw-r--r--   0 olt        (501) staff       (20)     3064 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/unit/test_collections.py
--rw-r--r--   0 olt        (501) staff       (20)     1616 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/unit/test_concat_legends.py
--rw-r--r--   0 olt        (501) staff       (20)    28734 2016-05-11 08:29:26.000000 MapProxy-1.9.0/mapproxy/test/unit/test_conf_loader.py
--rw-r--r--   0 olt        (501) staff       (20)    11191 2016-05-11 08:29:26.000000 MapProxy-1.9.0/mapproxy/test/unit/test_conf_validator.py
--rw-r--r--   0 olt        (501) staff       (20)     3863 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/unit/test_config.py
--rw-r--r--   0 olt        (501) staff       (20)     6373 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/unit/test_decorate_img.py
--rw-r--r--   0 olt        (501) staff       (20)    10200 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/test/unit/test_exceptions.py
--rw-r--r--   0 olt        (501) staff       (20)     6337 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/unit/test_featureinfo.py
--rw-r--r--   0 olt        (501) staff       (20)      925 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/unit/test_file_lock_load.py
--rw-r--r--   0 olt        (501) staff       (20)    16210 2016-06-16 14:31:04.000000 MapProxy-1.9.0/mapproxy/test/unit/test_geom.py
--rw-r--r--   0 olt        (501) staff       (20)    46983 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/unit/test_grid.py
--rw-r--r--   0 olt        (501) staff       (20)    29105 2016-06-15 08:30:34.000000 MapProxy-1.9.0/mapproxy/test/unit/test_image.py
--rw-r--r--   0 olt        (501) staff       (20)     4052 2015-04-08 11:32:54.000000 MapProxy-1.9.0/mapproxy/test/unit/test_image_mask.py
--rw-r--r--   0 olt        (501) staff       (20)     6743 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/unit/test_image_messages.py
--rw-r--r--   0 olt        (501) staff       (20)     5240 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/test/unit/test_image_options.py
--rw-r--r--   0 olt        (501) staff       (20)     5326 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/test/unit/test_multiapp.py
--rw-r--r--   0 olt        (501) staff       (20)     1568 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/unit/test_ogr_reader.py
--rw-r--r--   0 olt        (501) staff       (20)    21390 2016-05-12 11:05:09.000000 MapProxy-1.9.0/mapproxy/test/unit/test_request.py
--rw-r--r--   0 olt        (501) staff       (20)     3163 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/test/unit/test_request_wmts.py
--rw-r--r--   0 olt        (501) staff       (20)     2895 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/unit/test_response.py
--rw-r--r--   0 olt        (501) staff       (20)    10993 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/unit/test_seed.py
--rw-r--r--   0 olt        (501) staff       (20)     2743 2013-11-23 11:35:51.000000 MapProxy-1.9.0/mapproxy/test/unit/test_seed_cachelock.py
--rw-r--r--   0 olt        (501) staff       (20)     2525 2014-04-10 06:43:29.000000 MapProxy-1.9.0/mapproxy/test/unit/test_srs.py
--rw-r--r--   0 olt        (501) staff       (20)     3630 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/unit/test_tiled_source.py
--rw-r--r--   0 olt        (501) staff       (20)     1323 2013-11-23 11:35:51.000000 MapProxy-1.9.0/mapproxy/test/unit/test_tilefilter.py
--rw-r--r--   0 olt        (501) staff       (20)      370 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/unit/test_times.py
--rw-r--r--   0 olt        (501) staff       (20)     1756 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/test/unit/test_timeutils.py
--rw-r--r--   0 olt        (501) staff       (20)     2482 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/test/unit/test_util_conf_utils.py
--rw-r--r--   0 olt        (501) staff       (20)    14261 2016-05-11 09:21:23.000000 MapProxy-1.9.0/mapproxy/test/unit/test_utils.py
--rw-r--r--   0 olt        (501) staff       (20)     1553 2015-04-08 07:30:13.000000 MapProxy-1.9.0/mapproxy/test/unit/test_wms_capabilities.py
--rw-r--r--   0 olt        (501) staff       (20)     3597 2016-05-10 07:04:57.000000 MapProxy-1.9.0/mapproxy/test/unit/test_wms_layer.py
--rw-r--r--   0 olt        (501) staff       (20)     1904 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/test/unit/test_yaml.py
--rw-r--r--   0 olt        (501) staff       (20)     2169 2013-11-23 11:35:51.000000 MapProxy-1.9.0/mapproxy/tilefilter.py
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/util/
--rw-r--r--   0 olt        (501) staff       (20)        0 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/util/__init__.py
--rw-r--r--   0 olt        (501) staff       (20)    11181 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/util/async.py
--rw-r--r--   0 olt        (501) staff       (20)     3681 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/util/collections.py
--rw-r--r--   0 olt        (501) staff       (20)     7738 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/util/coverage.py
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/util/ext/
--rw-r--r--   0 olt        (501) staff       (20)      646 2013-11-23 11:35:51.000000 MapProxy-1.9.0/mapproxy/util/ext/__init__.py
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/util/ext/dictspec/
--rw-r--r--   0 olt        (501) staff       (20)       19 2013-11-23 11:35:51.000000 MapProxy-1.9.0/mapproxy/util/ext/dictspec/__init__.py
--rw-r--r--   0 olt        (501) staff       (20)     3691 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/util/ext/dictspec/spec.py
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/util/ext/dictspec/test/
--rw-r--r--   0 olt        (501) staff       (20)        0 2013-11-23 11:35:51.000000 MapProxy-1.9.0/mapproxy/util/ext/dictspec/test/__init__.py
--rw-r--r--   0 olt        (501) staff       (20)     9692 2016-02-10 12:08:11.000000 MapProxy-1.9.0/mapproxy/util/ext/dictspec/test/test_validator.py
--rw-r--r--   0 olt        (501) staff       (20)     6501 2016-04-26 09:24:49.000000 MapProxy-1.9.0/mapproxy/util/ext/dictspec/validator.py
--rw-r--r--   0 olt        (501) staff       (20)     5925 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/util/ext/local.py
--rw-r--r--   0 olt        (501) staff       (20)     4544 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/util/ext/lockfile.py
--rw-r--r--   0 olt        (501) staff       (20)    10840 2016-06-14 11:52:25.000000 MapProxy-1.9.0/mapproxy/util/ext/odict.py
--rw-r--r--   0 olt        (501) staff       (20)    28470 2016-02-10 12:20:56.000000 MapProxy-1.9.0/mapproxy/util/ext/serving.py
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/util/ext/tempita/
--rw-r--r--   0 olt        (501) staff       (20)    39093 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/util/ext/tempita/__init__.py
--rw-r--r--   0 olt        (501) staff       (20)     4179 2013-11-23 12:09:00.000000 MapProxy-1.9.0/mapproxy/util/ext/tempita/_looper.py
--rw-r--r--   0 olt        (501) staff       (20)      849 2013-11-23 12:09:00.000000 MapProxy-1.9.0/mapproxy/util/ext/tempita/compat3.py
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/util/ext/wmsparse/
--rw-r--r--   0 olt        (501) staff       (20)       71 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/util/ext/wmsparse/__init__.py
--rw-r--r--   0 olt        (501) staff       (20)    10572 2016-05-10 09:45:16.000000 MapProxy-1.9.0/mapproxy/util/ext/wmsparse/parse.py
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:24.000000 MapProxy-1.9.0/mapproxy/util/ext/wmsparse/test/
--rw-r--r--   0 olt        (501) staff       (20)        0 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/util/ext/wmsparse/test/__init__.py
--rw-r--r--   0 olt        (501) staff       (20)     4635 2015-05-08 08:57:23.000000 MapProxy-1.9.0/mapproxy/util/ext/wmsparse/test/test_parse.py
--rw-r--r--   0 olt        (501) staff       (20)      553 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/util/ext/wmsparse/test/test_util.py
--rw-r--r--   0 olt        (501) staff       (20)    81114 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/util/ext/wmsparse/test/wms-large-111.xml
--rw-r--r--   0 olt        (501) staff       (20)     3883 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/util/ext/wmsparse/test/wms-omniscale-111.xml
--rw-r--r--   0 olt        (501) staff       (20)     5534 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/util/ext/wmsparse/test/wms-omniscale-130.xml
--rw-r--r--   0 olt        (501) staff       (20)    22573 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/util/ext/wmsparse/test/wms_nasa_cap.xml
--rw-r--r--   0 olt        (501) staff       (20)      570 2015-02-04 07:28:26.000000 MapProxy-1.9.0/mapproxy/util/ext/wmsparse/util.py
--rw-r--r--   0 olt        (501) staff       (20)     4824 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/util/fs.py
--rw-r--r--   0 olt        (501) staff       (20)     6420 2016-06-16 14:45:26.000000 MapProxy-1.9.0/mapproxy/util/geom.py
--rw-r--r--   0 olt        (501) staff       (20)     3274 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/util/lib.py
--rw-r--r--   0 olt        (501) staff       (20)     5189 2015-11-17 08:15:03.000000 MapProxy-1.9.0/mapproxy/util/lock.py
--rw-r--r--   0 olt        (501) staff       (20)     7246 2016-04-20 09:16:05.000000 MapProxy-1.9.0/mapproxy/util/ogr.py
--rw-r--r--   0 olt        (501) staff       (20)     2379 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/util/py.py
--rw-r--r--   0 olt        (501) staff       (20)     2435 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/util/times.py
--rw-r--r--   0 olt        (501) staff       (20)     1419 2013-11-23 11:35:51.000000 MapProxy-1.9.0/mapproxy/util/wsgi.py
--rw-r--r--   0 olt        (501) staff       (20)     1609 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/util/yaml.py
--rw-r--r--   0 olt        (501) staff       (20)     1016 2015-04-08 07:53:15.000000 MapProxy-1.9.0/mapproxy/version.py
--rw-r--r--   0 olt        (501) staff       (20)     7598 2016-03-15 14:53:55.000000 MapProxy-1.9.0/mapproxy/wsgiapp.py
-drwxr-xr-x   0 olt        (501) staff       (20)        0 2016-07-22 08:01:23.000000 MapProxy-1.9.0/MapProxy.egg-info/
--rw-r--r--   0 olt        (501) staff       (20)        1 2016-07-22 08:01:19.000000 MapProxy-1.9.0/MapProxy.egg-info/dependency_links.txt
--rw-r--r--   0 olt        (501) staff       (20)      397 2016-07-22 08:01:19.000000 MapProxy-1.9.0/MapProxy.egg-info/entry_points.txt
--rw-r--r--   0 olt        (501) staff       (20)        9 2016-07-22 08:01:19.000000 MapProxy-1.9.0/MapProxy.egg-info/namespace_packages.txt
--rw-r--r--   0 olt        (501) staff       (20)        1 2013-04-03 09:13:33.000000 MapProxy-1.9.0/MapProxy.egg-info/not-zip-safe
--rw-r--r--   0 olt        (501) staff       (20)       47 2016-07-22 08:01:19.000000 MapProxy-1.9.0/MapProxy.egg-info/pbr.json
--rw-r--r--   0 olt        (501) staff       (20)     7755 2016-07-22 08:01:19.000000 MapProxy-1.9.0/MapProxy.egg-info/PKG-INFO
--rw-r--r--   0 olt        (501) staff       (20)       33 2016-07-22 08:01:19.000000 MapProxy-1.9.0/MapProxy.egg-info/requires.txt
--rw-r--r--   0 olt        (501) staff       (20)    19493 2016-07-22 08:01:23.000000 MapProxy-1.9.0/MapProxy.egg-info/SOURCES.txt
--rw-r--r--   0 olt        (501) staff       (20)        9 2016-07-22 08:01:19.000000 MapProxy-1.9.0/MapProxy.egg-info/top_level.txt
--rw-r--r--   0 olt        (501) staff       (20)     7755 2016-07-22 08:01:24.000000 MapProxy-1.9.0/PKG-INFO
--rw-r--r--   0 olt        (501) staff       (20)      654 2013-12-10 14:17:57.000000 MapProxy-1.9.0/README.rst
--rw-r--r--   0 olt        (501) staff       (20)      174 2016-02-10 12:08:11.000000 MapProxy-1.9.0/requirements-tests.txt
--rw-r--r--   0 olt        (501) staff       (20)      166 2016-07-22 08:01:24.000000 MapProxy-1.9.0/setup.cfg
--rw-r--r--   0 olt        (501) staff       (20)     3220 2016-07-22 07:45:13.000000 MapProxy-1.9.0/setup.py
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:16.000000 MapProxy-1.9.1/
+-rw-r--r--   0 olt        (501) staff       (20)    22495 2017-01-18 14:20:27.000000 MapProxy-1.9.1/CHANGES.txt
+-rw-r--r--   0 olt        (501) staff       (20)     1903 2016-09-02 13:46:18.000000 MapProxy-1.9.1/COPYING.txt
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/doc/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/doc/_static/
+-rw-r--r--   0 olt        (501) staff       (20)     1368 2012-04-23 07:43:43.000000 MapProxy-1.9.1/doc/_static/logo.png
+-rw-r--r--   0 olt        (501) staff       (20)      760 2017-01-18 12:58:59.000000 MapProxy-1.9.1/doc/_static/mapproxy.css
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/doc/_templates/
+-rw-r--r--   0 olt        (501) staff       (20)      950 2017-01-18 12:58:59.000000 MapProxy-1.9.1/doc/_templates/layout.html
+-rw-r--r--   0 olt        (501) staff       (20)     1210 2017-01-18 12:58:59.000000 MapProxy-1.9.1/doc/_templates/navbar.html
+-rwxr-xr-x   0 olt        (501) staff       (20)       15 2016-09-02 13:46:18.000000 MapProxy-1.9.1/doc/_templates/toctree.html
+-rw-r--r--   0 olt        (501) staff       (20)    19527 2017-01-18 12:58:33.000000 MapProxy-1.9.1/doc/auth.rst
+-rw-r--r--   0 olt        (501) staff       (20)     9864 2017-01-18 12:58:59.000000 MapProxy-1.9.1/doc/caches.rst
+-rw-r--r--   0 olt        (501) staff       (20)     6663 2017-01-18 14:22:02.000000 MapProxy-1.9.1/doc/conf.py
+-rw-r--r--   0 olt        (501) staff       (20)    40232 2017-01-18 12:58:59.000000 MapProxy-1.9.1/doc/configuration.rst
+-rw-r--r--   0 olt        (501) staff       (20)    29224 2017-01-18 12:58:59.000000 MapProxy-1.9.1/doc/configuration_examples.rst
+-rw-r--r--   0 olt        (501) staff       (20)     3749 2017-01-18 12:58:33.000000 MapProxy-1.9.1/doc/coverages.rst
+-rw-r--r--   0 olt        (501) staff       (20)     4472 2016-09-02 13:46:18.000000 MapProxy-1.9.1/doc/decorate_img.rst
+-rw-r--r--   0 olt        (501) staff       (20)    15158 2017-01-18 12:58:59.000000 MapProxy-1.9.1/doc/deployment.rst
+-rw-r--r--   0 olt        (501) staff       (20)     4781 2016-09-02 13:46:18.000000 MapProxy-1.9.1/doc/development.rst
+-rw-r--r--   0 olt        (501) staff       (20)   102253 2013-04-25 08:38:23.000000 MapProxy-1.9.1/doc/GM.txt
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/doc/imgs/
+-rw-r--r--   0 olt        (501) staff       (20)    20437 2012-04-23 07:43:43.000000 MapProxy-1.9.1/doc/imgs/bicubic.png
+-rw-r--r--   0 olt        (501) staff       (20)    18588 2012-04-23 07:43:43.000000 MapProxy-1.9.1/doc/imgs/bilinear.png
+-rw-r--r--   0 olt        (501) staff       (20)     7633 2012-04-23 07:43:43.000000 MapProxy-1.9.1/doc/imgs/labeling-dynamic.png
+-rw-r--r--   0 olt        (501) staff       (20)     6825 2012-04-23 07:43:43.000000 MapProxy-1.9.1/doc/imgs/labeling-meta-buffer.png
+-rw-r--r--   0 olt        (501) staff       (20)     4011 2012-04-23 07:43:43.000000 MapProxy-1.9.1/doc/imgs/labeling-metatiling-buffer.png
+-rw-r--r--   0 olt        (501) staff       (20)     2594 2012-04-23 07:43:43.000000 MapProxy-1.9.1/doc/imgs/labeling-metatiling.png
+-rw-r--r--   0 olt        (501) staff       (20)     7765 2012-04-23 07:43:43.000000 MapProxy-1.9.1/doc/imgs/labeling-no-clip.png
+-rw-r--r--   0 olt        (501) staff       (20)     5092 2012-04-23 07:43:43.000000 MapProxy-1.9.1/doc/imgs/labeling-no-placement.png
+-rw-r--r--   0 olt        (501) staff       (20)     5321 2012-04-23 07:43:43.000000 MapProxy-1.9.1/doc/imgs/labeling-partial-false.png
+-rw-r--r--   0 olt        (501) staff       (20)     6567 2012-04-23 07:43:43.000000 MapProxy-1.9.1/doc/imgs/labeling-repeated.png
+-rw-r--r--   0 olt        (501) staff       (20)    32025 2016-09-02 13:46:18.000000 MapProxy-1.9.1/doc/imgs/mapnik-webmerc-hq.png
+-rw-r--r--   0 olt        (501) staff       (20)    12649 2016-09-02 13:46:18.000000 MapProxy-1.9.1/doc/imgs/mapnik-webmerc.png
+-rw-r--r--   0 olt        (501) staff       (20)    18652 2013-04-25 08:38:23.000000 MapProxy-1.9.1/doc/imgs/mapproxy-demo.png
+-rw-r--r--   0 olt        (501) staff       (20)    15501 2012-04-23 07:43:43.000000 MapProxy-1.9.1/doc/imgs/nearest.png
+-rw-r--r--   0 olt        (501) staff       (20)      483 2017-01-18 12:58:47.000000 MapProxy-1.9.1/doc/index.rst
+-rw-r--r--   0 olt        (501) staff       (20)     5265 2017-01-18 12:58:47.000000 MapProxy-1.9.1/doc/inspire.rst
+-rw-r--r--   0 olt        (501) staff       (20)     8021 2017-01-18 12:58:47.000000 MapProxy-1.9.1/doc/install.rst
+-rw-r--r--   0 olt        (501) staff       (20)     2540 2017-01-18 14:10:52.000000 MapProxy-1.9.1/doc/install_osgeo4w.rst
+-rw-r--r--   0 olt        (501) staff       (20)     4831 2017-01-18 14:12:16.000000 MapProxy-1.9.1/doc/install_windows.rst
+-rw-r--r--   0 olt        (501) staff       (20)    10699 2016-09-02 13:46:18.000000 MapProxy-1.9.1/doc/labeling.rst
+-rw-r--r--   0 olt        (501) staff       (20)     3435 2017-01-18 12:58:59.000000 MapProxy-1.9.1/doc/Makefile
+-rw-r--r--   0 olt        (501) staff       (20)     2042 2016-09-02 13:46:18.000000 MapProxy-1.9.1/doc/mapproxy_2.rst
+-rw-r--r--   0 olt        (501) staff       (20)    16579 2017-01-18 12:58:59.000000 MapProxy-1.9.1/doc/mapproxy_util.rst
+-rw-r--r--   0 olt        (501) staff       (20)     5174 2016-09-02 13:46:18.000000 MapProxy-1.9.1/doc/mapproxy_util_autoconfig.rst
+-rw-r--r--   0 olt        (501) staff       (20)    14561 2017-01-18 12:58:59.000000 MapProxy-1.9.1/doc/seed.rst
+-rw-r--r--   0 olt        (501) staff       (20)     2379 2016-03-08 10:35:31.000000 MapProxy-1.9.1/doc/seed2.rst
+-rw-r--r--   0 olt        (501) staff       (20)    13221 2017-01-18 12:58:59.000000 MapProxy-1.9.1/doc/services.rst
+-rw-r--r--   0 olt        (501) staff       (20)    17263 2017-01-18 12:58:59.000000 MapProxy-1.9.1/doc/sources.rst
+-rw-r--r--   0 olt        (501) staff       (20)    15008 2017-01-18 12:58:59.000000 MapProxy-1.9.1/doc/tutorial.rst
+-rw-r--r--   0 olt        (501) staff       (20)     2444 2016-09-02 13:46:18.000000 MapProxy-1.9.1/doc/tutorial.yaml
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/doc/yaml/
+-rw-r--r--   0 olt        (501) staff       (20)     1076 2017-01-18 12:58:33.000000 MapProxy-1.9.1/doc/yaml/cache_conf.yaml
+-rw-r--r--   0 olt        (501) staff       (20)     1148 2017-01-18 12:58:33.000000 MapProxy-1.9.1/doc/yaml/grid_conf.yaml
+-rw-r--r--   0 olt        (501) staff       (20)     1178 2017-01-18 12:58:33.000000 MapProxy-1.9.1/doc/yaml/merged_conf.yaml
+-rw-r--r--   0 olt        (501) staff       (20)     1188 2017-01-18 12:58:33.000000 MapProxy-1.9.1/doc/yaml/meta_conf.yaml
+-rw-r--r--   0 olt        (501) staff       (20)      195 2013-04-25 08:38:23.000000 MapProxy-1.9.1/doc/yaml/seed.yaml
+-rw-r--r--   0 olt        (501) staff       (20)      926 2017-01-18 12:58:33.000000 MapProxy-1.9.1/doc/yaml/simple_conf.yaml
+-rw-r--r--   0 olt        (501) staff       (20)    11358 2012-04-23 07:43:43.000000 MapProxy-1.9.1/LICENSE.txt
+-rw-r--r--   0 olt        (501) staff       (20)      860 2016-09-02 13:46:18.000000 MapProxy-1.9.1/MANIFEST.in
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/
+-rw-r--r--   0 olt        (501) staff       (20)       55 2013-11-23 11:35:51.000000 MapProxy-1.9.1/mapproxy/__init__.py
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/cache/
+-rw-r--r--   0 olt        (501) staff       (20)     1255 2017-01-18 12:58:33.000000 MapProxy-1.9.1/mapproxy/cache/__init__.py
+-rw-r--r--   0 olt        (501) staff       (20)     3292 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/cache/base.py
+-rw-r--r--   0 olt        (501) staff       (20)    10779 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/cache/couchdb.py
+-rw-r--r--   0 olt        (501) staff       (20)     1064 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/cache/dummy.py
+-rw-r--r--   0 olt        (501) staff       (20)    12739 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/cache/file.py
+-rw-r--r--   0 olt        (501) staff       (20)     2719 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/cache/legend.py
+-rw-r--r--   0 olt        (501) staff       (20)    11620 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/cache/mbtiles.py
+-rw-r--r--   0 olt        (501) staff       (20)     2459 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/cache/meta.py
+-rw-r--r--   0 olt        (501) staff       (20)     3438 2017-01-18 12:58:33.000000 MapProxy-1.9.1/mapproxy/cache/renderd.py
+-rw-r--r--   0 olt        (501) staff       (20)     6482 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/cache/riak.py
+-rw-r--r--   0 olt        (501) staff       (20)    14294 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/cache/sqlite.py
+-rw-r--r--   0 olt        (501) staff       (20)    16906 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/cache/tile.py
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/client/
+-rw-r--r--   0 olt        (501) staff       (20)        0 2013-11-23 11:35:51.000000 MapProxy-1.9.1/mapproxy/client/__init__.py
+-rw-r--r--   0 olt        (501) staff       (20)     1323 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/client/arcgis.py
+-rw-r--r--   0 olt        (501) staff       (20)     4672 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/client/cgi.py
+-rw-r--r--   0 olt        (501) staff       (20)    10298 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/client/http.py
+-rw-r--r--   0 olt        (501) staff       (20)     1236 2013-11-23 11:35:51.000000 MapProxy-1.9.1/mapproxy/client/log.py
+-rw-r--r--   0 olt        (501) staff       (20)     5668 2016-03-01 13:31:26.000000 MapProxy-1.9.1/mapproxy/client/tile.py
+-rw-r--r--   0 olt        (501) staff       (20)     8720 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/client/wms.py
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/compat/
+-rw-r--r--   0 olt        (501) staff       (20)      771 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/compat/__init__.py
+-rw-r--r--   0 olt        (501) staff       (20)     2834 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/compat/image.py
+-rw-r--r--   0 olt        (501) staff       (20)      395 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/compat/itertools.py
+-rw-r--r--   0 olt        (501) staff       (20)      151 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/compat/modules.py
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/config/
+-rw-r--r--   0 olt        (501) staff       (20)      945 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/config/__init__.py
+-rw-r--r--   0 olt        (501) staff       (20)     6682 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/config/config.py
+-rw-r--r--   0 olt        (501) staff       (20)     2878 2017-01-18 12:58:27.000000 MapProxy-1.9.1/mapproxy/config/coverage.py
+-rw-r--r--   0 olt        (501) staff       (20)     2650 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/config/defaults.py
+-rw-r--r--   0 olt        (501) staff       (20)    74612 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/config/loader.py
+-rw-r--r--   0 olt        (501) staff       (20)    15256 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/config/spec.py
+-rw-r--r--   0 olt        (501) staff       (20)     8876 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/config/validator.py
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/config_template/
+-rw-r--r--   0 olt        (501) staff       (20)      451 2013-11-23 11:35:51.000000 MapProxy-1.9.1/mapproxy/config_template/__init__.py
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/config_template/base_config/
+-rw-r--r--   0 olt        (501) staff       (20)      384 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/config_template/base_config/config.wsgi
+-rw-r--r--   0 olt        (501) staff       (20)    17806 2017-01-18 12:58:33.000000 MapProxy-1.9.1/mapproxy/config_template/base_config/full_example.yaml
+-rw-r--r--   0 olt        (501) staff       (20)     2320 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/config_template/base_config/full_seed_example.yaml
+-rw-r--r--   0 olt        (501) staff       (20)      649 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/config_template/base_config/log.ini
+-rw-r--r--   0 olt        (501) staff       (20)     1493 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/config_template/base_config/mapproxy.yaml
+-rw-r--r--   0 olt        (501) staff       (20)      529 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/config_template/base_config/seed.yaml
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/config_template/paster/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/config_template/paster/etc/
+-rw-r--r--   0 olt        (501) staff       (20)      418 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/config_template/paster/etc/config.ini
+-rw-r--r--   0 olt        (501) staff       (20)      169 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/config_template/paster/etc/config.wsgi
+-rw-r--r--   0 olt        (501) staff       (20)      612 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/config_template/paster/etc/develop.ini
+-rw-r--r--   0 olt        (501) staff       (20)      734 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/config_template/paster/etc/log_deploy.ini
+-rw-r--r--   0 olt        (501) staff       (20)     4056 2017-01-18 12:58:33.000000 MapProxy-1.9.1/mapproxy/config_template/paster/etc/mapproxy.yaml
+-rw-r--r--   0 olt        (501) staff       (20)     1071 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/config_template/paster/etc/seed.yaml
+-rw-r--r--   0 olt        (501) staff       (20)     4526 2013-11-23 11:35:51.000000 MapProxy-1.9.1/mapproxy/exception.py
+-rw-r--r--   0 olt        (501) staff       (20)     4662 2017-01-18 12:58:33.000000 MapProxy-1.9.1/mapproxy/featureinfo.py
+-rw-r--r--   0 olt        (501) staff       (20)    38801 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/grid.py
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/image/
+-rw-r--r--   0 olt        (501) staff       (20)    15583 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/image/__init__.py
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/image/fonts/
+-rw-r--r--   0 olt        (501) staff       (20)        0 2013-11-23 11:35:51.000000 MapProxy-1.9.1/mapproxy/image/fonts/__init__.py
+-rw-r--r--   0 olt        (501) staff       (20)   622020 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/image/fonts/DejaVuSans.ttf
+-rw-r--r--   0 olt        (501) staff       (20)   320812 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/image/fonts/DejaVuSansMono.ttf
+-rw-r--r--   0 olt        (501) staff       (20)     4816 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/image/fonts/LICENSE
+-rw-r--r--   0 olt        (501) staff       (20)     2106 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/image/mask.py
+-rw-r--r--   0 olt        (501) staff       (20)    10381 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/image/merge.py
+-rw-r--r--   0 olt        (501) staff       (20)    12216 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/image/message.py
+-rw-r--r--   0 olt        (501) staff       (20)     5412 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/image/opts.py
+-rw-r--r--   0 olt        (501) staff       (20)     5951 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/image/tile.py
+-rw-r--r--   0 olt        (501) staff       (20)     8933 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/image/transform.py
+-rw-r--r--   0 olt        (501) staff       (20)    15459 2017-01-18 12:58:33.000000 MapProxy-1.9.1/mapproxy/layer.py
+-rw-r--r--   0 olt        (501) staff       (20)     7614 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/multiapp.py
+-rw-r--r--   0 olt        (501) staff       (20)     8047 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/proj.py
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/request/
+-rw-r--r--   0 olt        (501) staff       (20)      737 2013-11-23 11:35:51.000000 MapProxy-1.9.1/mapproxy/request/__init__.py
+-rw-r--r--   0 olt        (501) staff       (20)     4212 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/request/arcgis.py
+-rw-r--r--   0 olt        (501) staff       (20)    14968 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/request/base.py
+-rw-r--r--   0 olt        (501) staff       (20)     4172 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/request/tile.py
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/request/wms/
+-rw-r--r--   0 olt        (501) staff       (20)    26808 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/request/wms/__init__.py
+-rw-r--r--   0 olt        (501) staff       (20)     3481 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/request/wms/exception.py
+-rw-r--r--   0 olt        (501) staff       (20)    12838 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/request/wmts.py
+-rw-r--r--   0 olt        (501) staff       (20)     7699 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/response.py
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/script/
+-rw-r--r--   0 olt        (501) staff       (20)        0 2013-11-23 11:35:51.000000 MapProxy-1.9.1/mapproxy/script/__init__.py
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/script/conf/
+-rw-r--r--   0 olt        (501) staff       (20)        0 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/script/conf/__init__.py
+-rw-r--r--   0 olt        (501) staff       (20)     6906 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/script/conf/app.py
+-rw-r--r--   0 olt        (501) staff       (20)     1272 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/script/conf/caches.py
+-rw-r--r--   0 olt        (501) staff       (20)     1473 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/script/conf/layers.py
+-rw-r--r--   0 olt        (501) staff       (20)     1253 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/script/conf/seeds.py
+-rw-r--r--   0 olt        (501) staff       (20)     2271 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/script/conf/sources.py
+-rw-r--r--   0 olt        (501) staff       (20)     5237 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/script/conf/utils.py
+-rw-r--r--   0 olt        (501) staff       (20)     8816 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/script/export.py
+-rw-r--r--   0 olt        (501) staff       (20)     7411 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/script/grids.py
+-rw-r--r--   0 olt        (501) staff       (20)     4181 2017-01-18 12:58:33.000000 MapProxy-1.9.1/mapproxy/script/scales.py
+-rwxr-xr-x   0 olt        (501) staff       (20)    12917 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/script/util.py
+-rw-r--r--   0 olt        (501) staff       (20)     6049 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/script/wms_capabilities.py
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/seed/
+-rw-r--r--   0 olt        (501) staff       (20)        0 2013-11-23 11:35:51.000000 MapProxy-1.9.1/mapproxy/seed/__init__.py
+-rw-r--r--   0 olt        (501) staff       (20)     3758 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/seed/cachelock.py
+-rw-r--r--   0 olt        (501) staff       (20)     3867 2017-01-18 12:58:33.000000 MapProxy-1.9.1/mapproxy/seed/cleanup.py
+-rw-r--r--   0 olt        (501) staff       (20)    17613 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/seed/config.py
+-rw-r--r--   0 olt        (501) staff       (20)    11300 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/seed/script.py
+-rw-r--r--   0 olt        (501) staff       (20)    17485 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/seed/seeder.py
+-rw-r--r--   0 olt        (501) staff       (20)     2204 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/seed/spec.py
+-rw-r--r--   0 olt        (501) staff       (20)     9538 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/seed/util.py
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/service/
+-rw-r--r--   0 olt        (501) staff       (20)      646 2013-11-23 11:35:51.000000 MapProxy-1.9.1/mapproxy/service/__init__.py
+-rw-r--r--   0 olt        (501) staff       (20)     1692 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/service/base.py
+-rw-r--r--   0 olt        (501) staff       (20)    11137 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/service/demo.py
+-rw-r--r--   0 olt        (501) staff       (20)    12350 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/service/kml.py
+-rw-r--r--   0 olt        (501) staff       (20)     1357 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/service/ows.py
+-rw-r--r--   0 olt        (501) staff       (20)     2236 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/service/template_helper.py
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/service/templates/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/service/templates/demo/
+-rw-r--r--   0 olt        (501) staff       (20)      457 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/service/templates/demo/capabilities_demo.html
+-rw-r--r--   0 olt        (501) staff       (20)     8027 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/service/templates/demo/demo.html
+-rw-r--r--   0 olt        (501) staff       (20)      272 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/service/templates/demo/openlayers-demo.cfg
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/service/templates/demo/static/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/service/templates/demo/static/img/
+-rw-r--r--   0 olt        (501) staff       (20)       42 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/service/templates/demo/static/img/blank.gif
+-rw-r--r--   0 olt        (501) staff       (20)      451 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/service/templates/demo/static/img/east-mini.png
+-rw-r--r--   0 olt        (501) staff       (20)      484 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/service/templates/demo/static/img/north-mini.png
+-rw-r--r--   0 olt        (501) staff       (20)      481 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/service/templates/demo/static/img/south-mini.png
+-rw-r--r--   0 olt        (501) staff       (20)      453 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/service/templates/demo/static/img/west-mini.png
+-rw-r--r--   0 olt        (501) staff       (20)      359 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/service/templates/demo/static/img/zoom-minus-mini.png
+-rw-r--r--   0 olt        (501) staff       (20)      489 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/service/templates/demo/static/img/zoom-plus-mini.png
+-rw-r--r--   0 olt        (501) staff       (20)     1072 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/service/templates/demo/static/img/zoom-world-mini.png
+-rw-r--r--   0 olt        (501) staff       (20)     1368 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/service/templates/demo/static/logo.png
+-rw-r--r--   0 olt        (501) staff       (20)   163900 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/service/templates/demo/static/OpenLayers.js
+-rw-r--r--   0 olt        (501) staff       (20)     1994 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/service/templates/demo/static/site.css
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/service/templates/demo/static/theme/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/service/templates/demo/static/theme/default/
+-rw-r--r--   0 olt        (501) staff       (20)        0 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/service/templates/demo/static/theme/default/framedCloud.css
+-rw-r--r--   0 olt        (501) staff       (20)      303 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/service/templates/demo/static/theme/default/google.css
+-rw-r--r--   0 olt        (501) staff       (20)      212 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/service/templates/demo/static/theme/default/ie6-style.css
+-rw-r--r--   0 olt        (501) staff       (20)     9892 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/service/templates/demo/static/theme/default/style.css
+-rw-r--r--   0 olt        (501) staff       (20)      966 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/service/templates/demo/static.html
+-rw-r--r--   0 olt        (501) staff       (20)     3300 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/service/templates/demo/tms_demo.html
+-rw-r--r--   0 olt        (501) staff       (20)     3083 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/service/templates/demo/wms_demo.html
+-rw-r--r--   0 olt        (501) staff       (20)     2949 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/service/templates/demo/wmts_demo.html
+-rw-r--r--   0 olt        (501) staff       (20)      463 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/service/templates/tms_capabilities.xml
+-rw-r--r--   0 olt        (501) staff       (20)      101 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/service/templates/tms_exception.xml
+-rw-r--r--   0 olt        (501) staff       (20)      227 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/service/templates/tms_root_resource.xml
+-rw-r--r--   0 olt        (501) staff       (20)      694 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/service/templates/tms_tilemap_capabilities.xml
+-rw-r--r--   0 olt        (501) staff       (20)     2853 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/service/templates/wms100capabilities.xml
+-rw-r--r--   0 olt        (501) staff       (20)       82 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/service/templates/wms100exception.xml
+-rw-r--r--   0 olt        (501) staff       (20)     5458 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/service/templates/wms110capabilities.xml
+-rw-r--r--   0 olt        (501) staff       (20)      291 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/service/templates/wms110exception.xml
+-rw-r--r--   0 olt        (501) staff       (20)     6457 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/service/templates/wms111capabilities.xml
+-rw-r--r--   0 olt        (501) staff       (20)      291 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/service/templates/wms111exception.xml
+-rw-r--r--   0 olt        (501) staff       (20)    12954 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/service/templates/wms130capabilities.xml
+-rw-r--r--   0 olt        (501) staff       (20)      392 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/service/templates/wms130exception.xml
+-rw-r--r--   0 olt        (501) staff       (20)     4968 2017-01-18 12:58:33.000000 MapProxy-1.9.1/mapproxy/service/templates/wmts100capabilities.xml
+-rw-r--r--   0 olt        (501) staff       (20)      483 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/service/templates/wmts100exception.xml
+-rw-r--r--   0 olt        (501) staff       (20)    18478 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/service/tile.py
+-rw-r--r--   0 olt        (501) staff       (20)    31057 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/service/wms.py
+-rw-r--r--   0 olt        (501) staff       (20)    11836 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/service/wmts.py
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/source/
+-rw-r--r--   0 olt        (501) staff       (20)     2346 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/source/__init__.py
+-rw-r--r--   0 olt        (501) staff       (20)     1086 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/source/arcgis.py
+-rw-r--r--   0 olt        (501) staff       (20)     1447 2013-11-26 14:44:55.000000 MapProxy-1.9.1/mapproxy/source/error.py
+-rw-r--r--   0 olt        (501) staff       (20)     5514 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/source/mapnik.py
+-rw-r--r--   0 olt        (501) staff       (20)     3667 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/source/tile.py
+-rw-r--r--   0 olt        (501) staff       (20)     9418 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/source/wms.py
+-rw-r--r--   0 olt        (501) staff       (20)    13654 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/srs.py
+-rw-r--r--   0 olt        (501) staff       (20)     1930 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/template.py
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/
+-rw-r--r--   0 olt        (501) staff       (20)        0 2013-11-23 11:35:51.000000 MapProxy-1.9.1/mapproxy/test/__init__.py
+-rw-r--r--   0 olt        (501) staff       (20)     7181 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/helper.py
+-rw-r--r--   0 olt        (501) staff       (20)    15532 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/test/http.py
+-rw-r--r--   0 olt        (501) staff       (20)     6538 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/image.py
+-rw-r--r--   0 olt        (501) staff       (20)    83748 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/mocker.py
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/schemas/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/
+-rw-r--r--   0 olt        (501) staff       (20)    62819 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/common.xsd
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/
+-rw-r--r--   0 olt        (501) staff       (20)     6026 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_bul.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     5108 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_cze.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     4988 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_dan.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     5150 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_dut.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     6464 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_eng.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     4945 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_est.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     5002 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_fin.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     5183 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_fre.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     5086 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_ger.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     5035 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_gle.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     6049 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_gre.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     5098 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_hun.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     5092 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_ita.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     5094 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_lav.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     5096 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_lit.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     4984 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_mlt.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     5150 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_pol.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     5099 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_por.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     5100 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_rum.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     5053 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_slo.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     5022 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_slv.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     5177 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_spa.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     5024 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_swe.xsd
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/examples/
+-rw-r--r--   0 olt        (501) staff       (20)     4997 2011-04-26 14:20:06.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/examples/inspireresourcemddataset.xml
+-rw-r--r--   0 olt        (501) staff       (20)     4800 2011-04-26 14:19:14.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/examples/inspireresourcemdseries.xml
+-rw-r--r--   0 olt        (501) staff       (20)     4805 2011-04-26 14:19:48.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/examples/inspireresourcemdservice.xml
+-rw-r--r--   0 olt        (501) staff       (20)    28131 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/network.xsd
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/inspire_vs/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/inspire_vs/1.0/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/inspire_vs/1.0/examples/
+-rw-r--r--   0 olt        (501) staff       (20)    18083 2011-04-26 13:41:44.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/inspire_vs/1.0/examples/wms_at.xml
+-rw-r--r--   0 olt        (501) staff       (20)    17428 2011-04-26 13:41:42.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/inspire_vs/1.0/examples/wms_geoimage.xml
+-rw-r--r--   0 olt        (501) staff       (20)    15455 2011-04-26 13:41:42.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/inspire_vs/1.0/examples/WMS_Image2000GetCapabilities_InspireSchema.xml
+-rw-r--r--   0 olt        (501) staff       (20)     1561 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/schemas/inspire/inspire_vs/1.0/inspire_vs.xsd
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/schemas/kml/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/schemas/kml/2.2.0/
+-rw-r--r--   0 olt        (501) staff       (20)     1973 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/kml/2.2.0/atom-author-link.xsd
+-rw-r--r--   0 olt        (501) staff       (20)    66296 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/kml/2.2.0/ogckml22.xsd
+-rw-r--r--   0 olt        (501) staff       (20)      462 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/kml/2.2.0/ReadMe.txt
+-rw-r--r--   0 olt        (501) staff       (20)    74544 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/kml/2.2.0/xAL.xsd
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/schemas/ows/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/schemas/ows/1.1.0/
+-rw-r--r--   0 olt        (501) staff       (20)    13319 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/ows/1.1.0/ows19115subset.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     1121 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/ows/1.1.0/owsAll.xsd
+-rw-r--r--   0 olt        (501) staff       (20)    11942 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/ows/1.1.0/owsCommon.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     6995 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/ows/1.1.0/owsContents.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     7677 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/ows/1.1.0/owsDataIdentification.xsd
+-rw-r--r--   0 olt        (501) staff       (20)    14363 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/ows/1.1.0/owsDomainType.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     4892 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/ows/1.1.0/owsExceptionReport.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     7265 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/ows/1.1.0/owsGetCapabilities.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     3295 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/ows/1.1.0/owsGetResourceByID.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     4190 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/ows/1.1.0/owsInputOutputData.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     6456 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/ows/1.1.0/owsManifest.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     8926 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/ows/1.1.0/owsOperationsMetadata.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     3573 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/ows/1.1.0/owsServiceIdentification.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     2279 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/ows/1.1.0/owsServiceProvider.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     3356 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/ows/1.1.0/ReadMe.txt
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/schemas/sld/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/schemas/sld/1.1.0/
+-rw-r--r--   0 olt        (501) staff       (20)     1629 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/sld/1.1.0/sld_capabilities.xsd
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/schemas/wms/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/schemas/wms/1.0.0/
+-rw-r--r--   0 olt        (501) staff       (20)    16836 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wms/1.0.0/capabilities_1_0_0.dtd
+-rw-r--r--   0 olt        (501) staff       (20)     7897 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wms/1.0.0/capabilities_1_0_0.xml
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/schemas/wms/1.0.7/
+-rw-r--r--   0 olt        (501) staff       (20)    23882 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wms/1.0.7/capabilities_1_0_7.dtd
+-rw-r--r--   0 olt        (501) staff       (20)    11104 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wms/1.0.7/capabilities_1_0_7.xml
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/schemas/wms/1.1.0/
+-rw-r--r--   0 olt        (501) staff       (20)    10158 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wms/1.1.0/capabilities_1_1_0.dtd
+-rw-r--r--   0 olt        (501) staff       (20)    13161 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wms/1.1.0/capabilities_1_1_0.xml
+-rw-r--r--   0 olt        (501) staff       (20)      205 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wms/1.1.0/exception_1_1_0.dtd
+-rw-r--r--   0 olt        (501) staff       (20)     1081 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wms/1.1.0/exception_1_1_0.xml
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/schemas/wms/1.1.1/
+-rw-r--r--   0 olt        (501) staff       (20)    10505 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wms/1.1.1/capabilities_1_1_1.dtd
+-rw-r--r--   0 olt        (501) staff       (20)    13178 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wms/1.1.1/capabilities_1_1_1.xml
+-rw-r--r--   0 olt        (501) staff       (20)      205 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wms/1.1.1/exception_1_1_1.dtd
+-rw-r--r--   0 olt        (501) staff       (20)     1095 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wms/1.1.1/exception_1_1_1.xml
+-rw-r--r--   0 olt        (501) staff       (20)     2852 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wms/1.1.1/OGC-exception.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     1465 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wms/1.1.1/WMS_DescribeLayerResponse.dtd
+-rw-r--r--   0 olt        (501) staff       (20)      204 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wms/1.1.1/WMS_exception_1_1_1.dtd
+-rw-r--r--   0 olt        (501) staff       (20)    10438 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wms/1.1.1/WMS_MS_Capabilities.dtd
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/schemas/wms/1.3.0/
+-rw-r--r--   0 olt        (501) staff       (20)    11475 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wms/1.3.0/capabilities_1_3_0.xml
+-rw-r--r--   0 olt        (501) staff       (20)    21391 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wms/1.3.0/capabilities_1_3_0.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     1099 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wms/1.3.0/exceptions_1_3_0.xml
+-rw-r--r--   0 olt        (501) staff       (20)      982 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wms/1.3.0/exceptions_1_3_0.xsd
+-rw-r--r--   0 olt        (501) staff       (20)      315 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wms/1.3.0/ReadMe.txt
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/schemas/wmsc/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/schemas/wmsc/1.1.1/
+-rw-r--r--   0 olt        (501) staff       (20)    10505 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wmsc/1.1.1/capabilities_1_1_1.dtd
+-rw-r--r--   0 olt        (501) staff       (20)    13178 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wmsc/1.1.1/capabilities_1_1_1.xml
+-rw-r--r--   0 olt        (501) staff       (20)      205 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wmsc/1.1.1/exception_1_1_1.dtd
+-rw-r--r--   0 olt        (501) staff       (20)     1095 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wmsc/1.1.1/exception_1_1_1.xml
+-rw-r--r--   0 olt        (501) staff       (20)     2852 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wmsc/1.1.1/OGC-exception.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     1465 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wmsc/1.1.1/WMS_DescribeLayerResponse.dtd
+-rw-r--r--   0 olt        (501) staff       (20)      204 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wmsc/1.1.1/WMS_exception_1_1_1.dtd
+-rw-r--r--   0 olt        (501) staff       (20)    10781 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wmsc/1.1.1/WMS_MS_Capabilities.dtd
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/schemas/wmts/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/schemas/wmts/1.0/
+-rw-r--r--   0 olt        (501) staff       (20)     1100 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wmts/1.0/ReadMe.txt
+-rw-r--r--   0 olt        (501) staff       (20)     1203 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wmts/1.0/wmts.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     5540 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wmts/1.0/wmtsAbstract.wsdl
+-rw-r--r--   0 olt        (501) staff       (20)     1548 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wmts/1.0/wmtsGetCapabilities_request.xsd
+-rw-r--r--   0 olt        (501) staff       (20)    21708 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wmts/1.0/wmtsGetCapabilities_response.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     2208 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wmts/1.0/wmtsGetFeatureInfo_request.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     2817 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wmts/1.0/wmtsGetFeatureInfo_response.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     3243 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wmts/1.0/wmtsGetTile_request.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     2881 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wmts/1.0/wmtsKVP.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     2455 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/wmts/1.0/wmtsPayload_response.xsd
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/schemas/xlink/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:16.000000 MapProxy-1.9.1/mapproxy/test/schemas/xlink/1.0.0/
+-rw-r--r--   0 olt        (501) staff       (20)      182 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/xlink/1.0.0/ReadMe.txt
+-rw-r--r--   0 olt        (501) staff       (20)     5249 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/xlink/1.0.0/xlinks.xsd
+-rw-r--r--   0 olt        (501) staff       (20)     8836 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/schemas/xml.xsd
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:16.000000 MapProxy-1.9.1/mapproxy/test/system/
+-rw-r--r--   0 olt        (501) staff       (20)     3468 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/__init__.py
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:16.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/
+-rw-r--r--   0 olt        (501) staff       (20)      986 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/arcgis.yaml
+-rw-r--r--   0 olt        (501) staff       (20)     1226 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/auth.yaml
+-rw-r--r--   0 olt        (501) staff       (20)     8192 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/cache.mbtiles
+-rw-r--r--   0 olt        (501) staff       (20)     1470 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/cache_band_merge.yaml
+-rw-r--r--   0 olt        (501) staff       (20)      496 2016-08-11 09:46:05.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/cache_bulk_meta_tiles.yaml
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/cache_data/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/cache_data/dop_cache_EPSG3857/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/cache_data/dop_cache_EPSG3857/00/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/cache_data/dop_cache_EPSG3857/00/000/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/cache_data/dop_cache_EPSG3857/00/000/000/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/cache_data/dop_cache_EPSG3857/00/000/000/000/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/cache_data/dop_cache_EPSG3857/00/000/000/000/000/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:16.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/cache_data/dop_cache_EPSG3857/00/000/000/000/000/000/
+-rwxr-xr-x   0 olt        (501) staff       (20)      760 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/cache_data/dop_cache_EPSG3857/00/000/000/000/000/000/000.png
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/cache_data/wms_cache_EPSG900913/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/cache_data/wms_cache_EPSG900913/01/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/cache_data/wms_cache_EPSG900913/01/000/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/cache_data/wms_cache_EPSG900913/01/000/000/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/cache_data/wms_cache_EPSG900913/01/000/000/000/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/cache_data/wms_cache_EPSG900913/01/000/000/000/000/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:16.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/cache_data/wms_cache_EPSG900913/01/000/000/000/000/000/
+-rw-r--r--   0 olt        (501) staff       (20)    10214 2015-04-09 13:02:34.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/cache_data/wms_cache_EPSG900913/01/000/000/000/000/000/001.jpeg
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/cache_data/wms_cache_transparent_EPSG900913/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/cache_data/wms_cache_transparent_EPSG900913/01/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/cache_data/wms_cache_transparent_EPSG900913/01/000/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/cache_data/wms_cache_transparent_EPSG900913/01/000/000/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/cache_data/wms_cache_transparent_EPSG900913/01/000/000/000/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/cache_data/wms_cache_transparent_EPSG900913/01/000/000/000/000/
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:16.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/cache_data/wms_cache_transparent_EPSG900913/01/000/000/000/000/000/
+-rw-r--r--   0 olt        (501) staff       (20)      463 2015-04-09 13:02:34.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/cache_data/wms_cache_transparent_EPSG900913/01/000/000/000/000/000/001.png
+-rw-r--r--   0 olt        (501) staff       (20)      844 2016-03-15 14:53:55.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/cache_grid_names.yaml
+-rw-r--r--   0 olt        (501) staff       (20)      410 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/cache_mbtiles.yaml
+-rw-r--r--   0 olt        (501) staff       (20)     1556 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/cache_source.yaml
+-rw-r--r--   0 olt        (501) staff       (20)      611 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/cgi.py
+-rw-r--r--   0 olt        (501) staff       (20)     2780 2013-12-10 14:17:57.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/combined_sources.yaml
+-rw-r--r--   0 olt        (501) staff       (20)     1955 2017-01-18 12:58:33.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/coverage.yaml
+-rw-r--r--   0 olt        (501) staff       (20)      376 2016-03-15 14:53:55.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/disable_storage.yaml
+-rw-r--r--   0 olt        (501) staff       (20)       45 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/empty_ogrdata.geojson
+-rw-r--r--   0 olt        (501) staff       (20)     1926 2017-01-18 12:58:33.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/formats.yaml
+-rw-r--r--   0 olt        (501) staff       (20)     2943 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/inspire.yaml
+-rw-r--r--   0 olt        (501) staff       (20)     3756 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/inspire_full.yaml
+-rw-r--r--   0 olt        (501) staff       (20)     1332 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/kml_layer.yaml
+-rw-r--r--   0 olt        (501) staff       (20)     6066 2017-01-18 12:58:33.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/layer.yaml
+-rw-r--r--   0 olt        (501) staff       (20)     1042 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/layergroups.yaml
+-rw-r--r--   0 olt        (501) staff       (20)     1722 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/layergroups_root.yaml
+-rw-r--r--   0 olt        (501) staff       (20)     2471 2017-01-18 12:58:33.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/legendgraphic.yaml
+-rw-r--r--   0 olt        (501) staff       (20)     1053 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/mapnik_source.yaml
+-rw-r--r--   0 olt        (501) staff       (20)      193 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/mapproxy_export.yaml
+-rw-r--r--   0 olt        (501) staff       (20)      350 2013-04-25 08:38:23.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/mapserver.yaml
+-rw-r--r--   0 olt        (501) staff       (20)     1186 2017-01-18 12:58:33.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/mixed_mode.yaml
+-rw-r--r--   0 olt        (501) staff       (20)     2265 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/multi_cache_layers.yaml
+-rw-r--r--   0 olt        (501) staff       (20)      299 2013-04-25 08:38:23.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/multiapp1.yaml
+-rw-r--r--   0 olt        (501) staff       (20)      291 2013-04-25 08:38:23.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/multiapp2.yaml
+-rw-r--r--   0 olt        (501) staff       (20)      999 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/renderd_client.yaml
+-rw-r--r--   0 olt        (501) staff       (20)     1729 2017-01-18 12:58:33.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/scalehints.yaml
+-rw-r--r--   0 olt        (501) staff       (20)     1755 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/seed.yaml
+-rw-r--r--   0 olt        (501) staff       (20)      608 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/seed_mapproxy.yaml
+-rw-r--r--   0 olt        (501) staff       (20)      176 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/seed_old.yaml
+-rw-r--r--   0 olt        (501) staff       (20)      216 2013-04-25 08:38:23.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/seed_timeouts.yaml
+-rw-r--r--   0 olt        (501) staff       (20)      427 2013-04-25 08:38:23.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/seed_timeouts_mapproxy.yaml
+-rw-r--r--   0 olt        (501) staff       (20)     1245 2017-01-18 12:58:33.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/seedonly.yaml
+-rw-r--r--   0 olt        (501) staff       (20)      661 2013-04-25 08:38:23.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/sld.yaml
+-rw-r--r--   0 olt        (501) staff       (20)     1724 2016-03-15 14:53:55.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/source_errors.yaml
+-rw-r--r--   0 olt        (501) staff       (20)     1723 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/source_errors_raise.yaml
+-rw-r--r--   0 olt        (501) staff       (20)      376 2016-03-15 14:53:55.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/tileservice_origin.yaml
+-rw-r--r--   0 olt        (501) staff       (20)      448 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/tilesource_minmax_res.yaml
+-rw-r--r--   0 olt        (501) staff       (20)       97 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/util-conf-base-grids.yaml
+-rw-r--r--   0 olt        (501) staff       (20)      224 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/util-conf-overwrite.yaml
+-rw-r--r--   0 olt        (501) staff       (20)     3883 2017-01-18 12:58:33.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/util-conf-wms-111-cap.xml
+-rw-r--r--   0 olt        (501) staff       (20)      669 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/util_grids.yaml
+-rw-r--r--   0 olt        (501) staff       (20)     6060 2017-01-18 12:58:33.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/util_wms_capabilities111.xml
+-rw-r--r--   0 olt        (501) staff       (20)     4440 2017-01-18 12:58:33.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/util_wms_capabilities130.xml
+-rw-r--r--   0 olt        (501) staff       (20)      304 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/util_wms_capabilities_service_exception.xml
+-rw-r--r--   0 olt        (501) staff       (20)      839 2016-03-15 14:53:55.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/watermark.yaml
+-rw-r--r--   0 olt        (501) staff       (20)      537 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/wms_srs_extent.yaml
+-rw-r--r--   0 olt        (501) staff       (20)     1142 2017-01-18 12:58:33.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/wms_versions.yaml
+-rw-r--r--   0 olt        (501) staff       (20)     2616 2017-01-18 12:58:33.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/wmts.yaml
+-rw-r--r--   0 olt        (501) staff       (20)     1263 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/wmts_dimensions.yaml
+-rw-r--r--   0 olt        (501) staff       (20)     1170 2013-04-25 08:38:23.000000 MapProxy-1.9.1/mapproxy/test/system/fixture/xslt_featureinfo.yaml
+-rw-r--r--   0 olt        (501) staff       (20)     3311 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/test/system/test_arcgis.py
+-rw-r--r--   0 olt        (501) staff       (20)    33630 2017-01-18 12:58:33.000000 MapProxy-1.9.1/mapproxy/test/system/test_auth.py
+-rw-r--r--   0 olt        (501) staff       (20)     3564 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_behind_proxy.py
+-rw-r--r--   0 olt        (501) staff       (20)     3630 2016-08-11 11:12:36.000000 MapProxy-1.9.1/mapproxy/test/system/test_bulk_meta_tiles.py
+-rw-r--r--   0 olt        (501) staff       (20)     3703 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/test/system/test_cache_band_merge.py
+-rw-r--r--   0 olt        (501) staff       (20)     4295 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_cache_grid_names.py
+-rw-r--r--   0 olt        (501) staff       (20)     2628 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_cache_mbtiles.py
+-rw-r--r--   0 olt        (501) staff       (20)     5012 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_cache_source.py
+-rw-r--r--   0 olt        (501) staff       (20)    13027 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_combined_sources.py
+-rw-r--r--   0 olt        (501) staff       (20)     5525 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_coverage.py
+-rw-r--r--   0 olt        (501) staff       (20)     6737 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_decorate_img.py
+-rw-r--r--   0 olt        (501) staff       (20)     2157 2013-11-23 11:35:51.000000 MapProxy-1.9.1/mapproxy/test/system/test_disable_storage.py
+-rw-r--r--   0 olt        (501) staff       (20)     8765 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_formats.py
+-rw-r--r--   0 olt        (501) staff       (20)     5318 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/system/test_inspire_vs.py
+-rw-r--r--   0 olt        (501) staff       (20)    10512 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_kml.py
+-rw-r--r--   0 olt        (501) staff       (20)     5736 2013-11-23 11:35:51.000000 MapProxy-1.9.1/mapproxy/test/system/test_layergroups.py
+-rw-r--r--   0 olt        (501) staff       (20)    10585 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_legendgraphic.py
+-rw-r--r--   0 olt        (501) staff       (20)     5379 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_mapnik.py
+-rw-r--r--   0 olt        (501) staff       (20)     2294 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_mapserver.py
+-rw-r--r--   0 olt        (501) staff       (20)     7073 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_mixed_mode_format.py
+-rw-r--r--   0 olt        (501) staff       (20)     7101 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/test/system/test_multi_cache_layers.py
+-rw-r--r--   0 olt        (501) staff       (20)     3391 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_multiapp.py
+-rw-r--r--   0 olt        (501) staff       (20)    11857 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_renderd_client.py
+-rw-r--r--   0 olt        (501) staff       (20)     4963 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_scalehints.py
+-rw-r--r--   0 olt        (501) staff       (20)    18199 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_seed.py
+-rw-r--r--   0 olt        (501) staff       (20)     3021 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_seed_only.py
+-rw-r--r--   0 olt        (501) staff       (20)     3307 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_sld.py
+-rw-r--r--   0 olt        (501) staff       (20)    11762 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_source_errors.py
+-rw-r--r--   0 olt        (501) staff       (20)     2255 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_tilesource_minmax_res.py
+-rw-r--r--   0 olt        (501) staff       (20)    10944 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_tms.py
+-rw-r--r--   0 olt        (501) staff       (20)     1797 2013-12-10 14:17:57.000000 MapProxy-1.9.1/mapproxy/test/system/test_tms_origin.py
+-rw-r--r--   0 olt        (501) staff       (20)     8279 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_util_conf.py
+-rw-r--r--   0 olt        (501) staff       (20)     5662 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_util_export.py
+-rw-r--r--   0 olt        (501) staff       (20)     3210 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_util_grids.py
+-rw-r--r--   0 olt        (501) staff       (20)     5473 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_util_wms_capabilities.py
+-rw-r--r--   0 olt        (501) staff       (20)     3475 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_watermark.py
+-rw-r--r--   0 olt        (501) staff       (20)    57068 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/system/test_wms.py
+-rw-r--r--   0 olt        (501) staff       (20)     4526 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_wms_srs_extent.py
+-rw-r--r--   0 olt        (501) staff       (20)     2195 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_wms_version.py
+-rw-r--r--   0 olt        (501) staff       (20)     4057 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_wmsc.py
+-rw-r--r--   0 olt        (501) staff       (20)     6949 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/test/system/test_wmts.py
+-rw-r--r--   0 olt        (501) staff       (20)     7152 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_wmts_dimensions.py
+-rw-r--r--   0 olt        (501) staff       (20)     4430 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_wmts_restful.py
+-rw-r--r--   0 olt        (501) staff       (20)    10457 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/system/test_xslt_featureinfo.py
+-rw-r--r--   0 olt        (501) staff       (20)     7670 2017-01-18 12:58:33.000000 MapProxy-1.9.1/mapproxy/test/test_http_helper.py
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:16.000000 MapProxy-1.9.1/mapproxy/test/unit/
+-rw-r--r--   0 olt        (501) staff       (20)        0 2013-11-23 11:35:51.000000 MapProxy-1.9.1/mapproxy/test/unit/__init__.py
+-rw-r--r--   0 olt        (501) staff       (20)       58 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/unit/epsg
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:16.000000 MapProxy-1.9.1/mapproxy/test/unit/polygons/
+-rw-r--r--   0 olt        (501) staff       (20)      833 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/unit/polygons/polygons.dbf
+-rw-r--r--   0 olt        (501) staff       (20)     1580 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/unit/polygons/polygons.shp
+-rw-r--r--   0 olt        (501) staff       (20)      124 2012-04-23 07:43:43.000000 MapProxy-1.9.1/mapproxy/test/unit/polygons/polygons.shx
+-rw-r--r--   0 olt        (501) staff       (20)    10731 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/unit/test_async.py
+-rw-r--r--   0 olt        (501) staff       (20)    15175 2016-09-19 14:56:05.000000 MapProxy-1.9.1/mapproxy/test/unit/test_auth.py
+-rw-r--r--   0 olt        (501) staff       (20)    38652 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/unit/test_cache.py
+-rw-r--r--   0 olt        (501) staff       (20)     4514 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/unit/test_cache_couchdb.py
+-rw-r--r--   0 olt        (501) staff       (20)     2494 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/test/unit/test_cache_riak.py
+-rw-r--r--   0 olt        (501) staff       (20)    12221 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/test/unit/test_cache_tile.py
+-rw-r--r--   0 olt        (501) staff       (20)    15718 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/test/unit/test_client.py
+-rw-r--r--   0 olt        (501) staff       (20)     4650 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/unit/test_client_cgi.py
+-rw-r--r--   0 olt        (501) staff       (20)     3064 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/unit/test_collections.py
+-rw-r--r--   0 olt        (501) staff       (20)     1616 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/unit/test_concat_legends.py
+-rw-r--r--   0 olt        (501) staff       (20)    28734 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/test/unit/test_conf_loader.py
+-rw-r--r--   0 olt        (501) staff       (20)    11191 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/test/unit/test_conf_validator.py
+-rw-r--r--   0 olt        (501) staff       (20)     3863 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/unit/test_config.py
+-rw-r--r--   0 olt        (501) staff       (20)     6373 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/unit/test_decorate_img.py
+-rw-r--r--   0 olt        (501) staff       (20)    10200 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/unit/test_exceptions.py
+-rw-r--r--   0 olt        (501) staff       (20)     6337 2017-01-18 12:58:33.000000 MapProxy-1.9.1/mapproxy/test/unit/test_featureinfo.py
+-rw-r--r--   0 olt        (501) staff       (20)      925 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/unit/test_file_lock_load.py
+-rw-r--r--   0 olt        (501) staff       (20)    16210 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/test/unit/test_geom.py
+-rw-r--r--   0 olt        (501) staff       (20)    46983 2017-01-18 12:58:33.000000 MapProxy-1.9.1/mapproxy/test/unit/test_grid.py
+-rw-r--r--   0 olt        (501) staff       (20)    29105 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/test/unit/test_image.py
+-rw-r--r--   0 olt        (501) staff       (20)     4052 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/unit/test_image_mask.py
+-rw-r--r--   0 olt        (501) staff       (20)     6743 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/unit/test_image_messages.py
+-rw-r--r--   0 olt        (501) staff       (20)     5240 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/unit/test_image_options.py
+-rw-r--r--   0 olt        (501) staff       (20)     5326 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/unit/test_multiapp.py
+-rw-r--r--   0 olt        (501) staff       (20)     1568 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/unit/test_ogr_reader.py
+-rw-r--r--   0 olt        (501) staff       (20)    21390 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/test/unit/test_request.py
+-rw-r--r--   0 olt        (501) staff       (20)     3163 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/unit/test_request_wmts.py
+-rw-r--r--   0 olt        (501) staff       (20)     2895 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/unit/test_response.py
+-rw-r--r--   0 olt        (501) staff       (20)    10993 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/unit/test_seed.py
+-rw-r--r--   0 olt        (501) staff       (20)     2743 2013-11-23 11:35:51.000000 MapProxy-1.9.1/mapproxy/test/unit/test_seed_cachelock.py
+-rw-r--r--   0 olt        (501) staff       (20)     2525 2014-04-10 06:43:29.000000 MapProxy-1.9.1/mapproxy/test/unit/test_srs.py
+-rw-r--r--   0 olt        (501) staff       (20)     3630 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/unit/test_tiled_source.py
+-rw-r--r--   0 olt        (501) staff       (20)     1323 2013-11-23 11:35:51.000000 MapProxy-1.9.1/mapproxy/test/unit/test_tilefilter.py
+-rw-r--r--   0 olt        (501) staff       (20)      370 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/unit/test_times.py
+-rw-r--r--   0 olt        (501) staff       (20)     1756 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/unit/test_timeutils.py
+-rw-r--r--   0 olt        (501) staff       (20)     2482 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/unit/test_util_conf_utils.py
+-rw-r--r--   0 olt        (501) staff       (20)    14261 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/test/unit/test_utils.py
+-rw-r--r--   0 olt        (501) staff       (20)     1553 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/unit/test_wms_capabilities.py
+-rw-r--r--   0 olt        (501) staff       (20)     3597 2017-01-18 12:58:33.000000 MapProxy-1.9.1/mapproxy/test/unit/test_wms_layer.py
+-rw-r--r--   0 olt        (501) staff       (20)     1904 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/test/unit/test_yaml.py
+-rw-r--r--   0 olt        (501) staff       (20)     2169 2013-11-23 11:35:51.000000 MapProxy-1.9.1/mapproxy/tilefilter.py
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:16.000000 MapProxy-1.9.1/mapproxy/util/
+-rw-r--r--   0 olt        (501) staff       (20)        0 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/util/__init__.py
+-rw-r--r--   0 olt        (501) staff       (20)    11181 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/util/async.py
+-rw-r--r--   0 olt        (501) staff       (20)     3681 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/util/collections.py
+-rw-r--r--   0 olt        (501) staff       (20)     7738 2016-11-29 15:48:55.000000 MapProxy-1.9.1/mapproxy/util/coverage.py
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:16.000000 MapProxy-1.9.1/mapproxy/util/ext/
+-rw-r--r--   0 olt        (501) staff       (20)      646 2013-11-23 11:35:51.000000 MapProxy-1.9.1/mapproxy/util/ext/__init__.py
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:16.000000 MapProxy-1.9.1/mapproxy/util/ext/dictspec/
+-rw-r--r--   0 olt        (501) staff       (20)       19 2013-11-23 11:35:51.000000 MapProxy-1.9.1/mapproxy/util/ext/dictspec/__init__.py
+-rw-r--r--   0 olt        (501) staff       (20)     3691 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/util/ext/dictspec/spec.py
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:16.000000 MapProxy-1.9.1/mapproxy/util/ext/dictspec/test/
+-rw-r--r--   0 olt        (501) staff       (20)        0 2013-11-23 11:35:51.000000 MapProxy-1.9.1/mapproxy/util/ext/dictspec/test/__init__.py
+-rw-r--r--   0 olt        (501) staff       (20)     9692 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/util/ext/dictspec/test/test_validator.py
+-rw-r--r--   0 olt        (501) staff       (20)     6501 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/util/ext/dictspec/validator.py
+-rw-r--r--   0 olt        (501) staff       (20)     5925 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/util/ext/local.py
+-rw-r--r--   0 olt        (501) staff       (20)     4544 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/util/ext/lockfile.py
+-rw-r--r--   0 olt        (501) staff       (20)    10840 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/util/ext/odict.py
+-rw-r--r--   0 olt        (501) staff       (20)    28822 2017-01-18 13:31:18.000000 MapProxy-1.9.1/mapproxy/util/ext/serving.py
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:16.000000 MapProxy-1.9.1/mapproxy/util/ext/tempita/
+-rw-r--r--   0 olt        (501) staff       (20)    39093 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/util/ext/tempita/__init__.py
+-rw-r--r--   0 olt        (501) staff       (20)     4179 2013-11-23 12:09:00.000000 MapProxy-1.9.1/mapproxy/util/ext/tempita/_looper.py
+-rw-r--r--   0 olt        (501) staff       (20)      849 2013-11-23 12:09:00.000000 MapProxy-1.9.1/mapproxy/util/ext/tempita/compat3.py
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:16.000000 MapProxy-1.9.1/mapproxy/util/ext/wmsparse/
+-rw-r--r--   0 olt        (501) staff       (20)       71 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/util/ext/wmsparse/__init__.py
+-rw-r--r--   0 olt        (501) staff       (20)    10572 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/util/ext/wmsparse/parse.py
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:16.000000 MapProxy-1.9.1/mapproxy/util/ext/wmsparse/test/
+-rw-r--r--   0 olt        (501) staff       (20)        0 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/util/ext/wmsparse/test/__init__.py
+-rw-r--r--   0 olt        (501) staff       (20)     4635 2017-01-18 12:58:33.000000 MapProxy-1.9.1/mapproxy/util/ext/wmsparse/test/test_parse.py
+-rw-r--r--   0 olt        (501) staff       (20)      553 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/util/ext/wmsparse/test/test_util.py
+-rw-r--r--   0 olt        (501) staff       (20)    81114 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/util/ext/wmsparse/test/wms-large-111.xml
+-rw-r--r--   0 olt        (501) staff       (20)     3883 2017-01-18 12:58:33.000000 MapProxy-1.9.1/mapproxy/util/ext/wmsparse/test/wms-omniscale-111.xml
+-rw-r--r--   0 olt        (501) staff       (20)     5534 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/util/ext/wmsparse/test/wms-omniscale-130.xml
+-rw-r--r--   0 olt        (501) staff       (20)    22573 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/util/ext/wmsparse/test/wms_nasa_cap.xml
+-rw-r--r--   0 olt        (501) staff       (20)      570 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/util/ext/wmsparse/util.py
+-rw-r--r--   0 olt        (501) staff       (20)     4824 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/util/fs.py
+-rw-r--r--   0 olt        (501) staff       (20)     6420 2017-01-18 12:58:59.000000 MapProxy-1.9.1/mapproxy/util/geom.py
+-rw-r--r--   0 olt        (501) staff       (20)     3274 2016-11-29 16:35:47.000000 MapProxy-1.9.1/mapproxy/util/lib.py
+-rw-r--r--   0 olt        (501) staff       (20)     5189 2016-09-07 09:52:58.000000 MapProxy-1.9.1/mapproxy/util/lock.py
+-rw-r--r--   0 olt        (501) staff       (20)     7246 2017-01-18 12:58:47.000000 MapProxy-1.9.1/mapproxy/util/ogr.py
+-rw-r--r--   0 olt        (501) staff       (20)     2379 2017-01-18 12:58:33.000000 MapProxy-1.9.1/mapproxy/util/py.py
+-rw-r--r--   0 olt        (501) staff       (20)     2435 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/util/times.py
+-rw-r--r--   0 olt        (501) staff       (20)     1419 2013-11-23 11:35:51.000000 MapProxy-1.9.1/mapproxy/util/wsgi.py
+-rw-r--r--   0 olt        (501) staff       (20)     1609 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/util/yaml.py
+-rw-r--r--   0 olt        (501) staff       (20)     1016 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/version.py
+-rw-r--r--   0 olt        (501) staff       (20)     7598 2016-09-02 13:46:18.000000 MapProxy-1.9.1/mapproxy/wsgiapp.py
+drwxr-xr-x   0 olt        (501) staff       (20)        0 2017-01-18 14:24:15.000000 MapProxy-1.9.1/MapProxy.egg-info/
+-rw-r--r--   0 olt        (501) staff       (20)        1 2017-01-18 14:24:13.000000 MapProxy-1.9.1/MapProxy.egg-info/dependency_links.txt
+-rw-r--r--   0 olt        (501) staff       (20)      397 2017-01-18 14:24:13.000000 MapProxy-1.9.1/MapProxy.egg-info/entry_points.txt
+-rw-r--r--   0 olt        (501) staff       (20)        9 2017-01-18 14:24:13.000000 MapProxy-1.9.1/MapProxy.egg-info/namespace_packages.txt
+-rw-r--r--   0 olt        (501) staff       (20)        1 2013-04-03 09:13:33.000000 MapProxy-1.9.1/MapProxy.egg-info/not-zip-safe
+-rw-r--r--   0 olt        (501) staff       (20)       47 2017-01-18 14:24:13.000000 MapProxy-1.9.1/MapProxy.egg-info/pbr.json
+-rw-r--r--   0 olt        (501) staff       (20)     7538 2017-01-18 14:24:13.000000 MapProxy-1.9.1/MapProxy.egg-info/PKG-INFO
+-rw-r--r--   0 olt        (501) staff       (20)       33 2017-01-18 14:24:13.000000 MapProxy-1.9.1/MapProxy.egg-info/requires.txt
+-rw-r--r--   0 olt        (501) staff       (20)    19594 2017-01-18 14:24:15.000000 MapProxy-1.9.1/MapProxy.egg-info/SOURCES.txt
+-rw-r--r--   0 olt        (501) staff       (20)        9 2017-01-18 14:24:13.000000 MapProxy-1.9.1/MapProxy.egg-info/top_level.txt
+-rw-r--r--   0 olt        (501) staff       (20)     7538 2017-01-18 14:24:16.000000 MapProxy-1.9.1/PKG-INFO
+-rw-r--r--   0 olt        (501) staff       (20)      654 2017-01-18 12:58:33.000000 MapProxy-1.9.1/README.rst
+-rw-r--r--   0 olt        (501) staff       (20)      174 2017-01-18 12:58:47.000000 MapProxy-1.9.1/requirements-tests.txt
+-rw-r--r--   0 olt        (501) staff       (20)      166 2017-01-18 14:24:16.000000 MapProxy-1.9.1/setup.cfg
+-rw-r--r--   0 olt        (501) staff       (20)     3220 2017-01-18 14:22:02.000000 MapProxy-1.9.1/setup.py
```

### Comparing `MapProxy-1.9.0/CHANGES.txt` & `MapProxy-1.9.1/CHANGES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+1.9.1 2017-01-18
+~~~~~~~~~~~~~~~~
+
+Fixes:
+
+- serve-develop: fixed reloader for Windows installations made
+  with recent pip version (#279)
+
 1.9.0 2016-07-22
 ~~~~~~~~~~~~~~~~
 
 Improvements:
 
 - New band merge feature. Allows to create false-color or grayscale
   images on the fly.
```

### Comparing `MapProxy-1.9.0/COPYING.txt` & `MapProxy-1.9.1/COPYING.txt`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/_static/logo.png` & `MapProxy-1.9.1/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/_static/mapproxy.css` & `MapProxy-1.9.1/doc/_static/mapproxy.css`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/_templates/layout.html` & `MapProxy-1.9.1/doc/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/_templates/navbar.html` & `MapProxy-1.9.1/doc/_templates/navbar.html`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/auth.rst` & `MapProxy-1.9.1/doc/auth.rst`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/caches.rst` & `MapProxy-1.9.1/doc/caches.rst`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/conf.py` & `MapProxy-1.9.1/doc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = '1.9'
 # The full version, including alpha/beta/rc tags.
-release = '1.9.0'
+release = '1.9.1'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
```

### Comparing `MapProxy-1.9.0/doc/configuration.rst` & `MapProxy-1.9.1/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/configuration_examples.rst` & `MapProxy-1.9.1/doc/configuration_examples.rst`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/coverages.rst` & `MapProxy-1.9.1/doc/coverages.rst`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/decorate_img.rst` & `MapProxy-1.9.1/doc/decorate_img.rst`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/deployment.rst` & `MapProxy-1.9.1/doc/deployment.rst`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/development.rst` & `MapProxy-1.9.1/doc/development.rst`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/GM.txt` & `MapProxy-1.9.1/doc/GM.txt`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/imgs/bicubic.png` & `MapProxy-1.9.1/doc/imgs/bicubic.png`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/imgs/bilinear.png` & `MapProxy-1.9.1/doc/imgs/bilinear.png`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/imgs/labeling-dynamic.png` & `MapProxy-1.9.1/doc/imgs/labeling-dynamic.png`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/imgs/labeling-meta-buffer.png` & `MapProxy-1.9.1/doc/imgs/labeling-meta-buffer.png`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/imgs/labeling-metatiling-buffer.png` & `MapProxy-1.9.1/doc/imgs/labeling-metatiling-buffer.png`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/imgs/labeling-metatiling.png` & `MapProxy-1.9.1/doc/imgs/labeling-metatiling.png`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/imgs/labeling-no-clip.png` & `MapProxy-1.9.1/doc/imgs/labeling-no-clip.png`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/imgs/labeling-no-placement.png` & `MapProxy-1.9.1/doc/imgs/labeling-no-placement.png`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/imgs/labeling-partial-false.png` & `MapProxy-1.9.1/doc/imgs/labeling-partial-false.png`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/imgs/labeling-repeated.png` & `MapProxy-1.9.1/doc/imgs/labeling-repeated.png`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/imgs/mapnik-webmerc-hq.png` & `MapProxy-1.9.1/doc/imgs/mapnik-webmerc-hq.png`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/imgs/mapnik-webmerc.png` & `MapProxy-1.9.1/doc/imgs/mapnik-webmerc.png`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/imgs/mapproxy-demo.png` & `MapProxy-1.9.1/doc/imgs/mapproxy-demo.png`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/imgs/nearest.png` & `MapProxy-1.9.1/doc/imgs/nearest.png`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/inspire.rst` & `MapProxy-1.9.1/doc/inspire.rst`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/install.rst` & `MapProxy-1.9.1/doc/install.rst`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/install_osgeo4w.rst` & `MapProxy-1.9.1/doc/install_osgeo4w.rst`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/install_windows.rst` & `MapProxy-1.9.1/doc/install_windows.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 Installation on Windows
 =======================
 
-.. note:: You can also :doc:`install MapProxy inside an existing OSGeo4W installation<install_osgeo4w>`.
-
-At frist you need a working Python installation. You can download Python from: http://www.python.org/download/. MapProxy requires Python 2.7, 3.3 or 3.4. Python 2.6 should still work, but it is no longer officially supported.
-
+At frist you need a working Python installation. You can download Python from: https://www.python.org/download/. MapProxy requires Python 2.7, 3.3, 3.4, 3.5 or 3.6. Python 2.6 should still work, but it is no longer officially supported. We would recommend the latest 2.7 version available.
 
 Virtualenv
 ----------
 
 *If* you are using your Python installation for other applications as well, then we advise you to install MapProxy into a `virtual Python environment`_ to avoid any conflicts with different dependencies. *You can skip this if you only use the Python installation for MapProxy.*
 `Read about virtualenv <http://virtualenv.openplans.org/#what-it-does>`_ if you want to now more about the benefits.
 
@@ -20,58 +17,58 @@
  C:\mapproxy_venv\Scripts\activate.bat
 
 .. note::
   The last step is required every time you start working with your MapProxy installation. Alternatively you can always explicitly call ``\mapproxy_venv\Scripts\<command>``.
 
 .. note:: Apache mod_wsgi does not work well with virtualenv on Windows. If you want to use mod_wsgi for deployment, then you should skip the creation the virtualenv.
 
-After you activated the new environment, you have access to ``python`` and ``easy_install``.
+After you activated the new environment, you have access to ``python`` and ``pip``.
 To install MapProxy with most dependencies call::
 
-  easy_install MapProxy
+  pip install MapProxy
 
 This might take a minute. You can skip the next step.
 
 
-Setuptools
-----------
+PIP
+---
 
-MapProxy and most dependencies can be installed with the ``easy_install`` command.
-You need to `install the setuptool package <http://pypi.python.org/pypi/setuptools>`_ to get the ``easy_install`` command.
+MapProxy and most dependencies can be installed with the ``pip`` command. ``pip`` is already installed if you are using Python >=2.7.9, or Python >=3.4. `Read the pip documentation for more information <https://pip.pypa.io/en/stable/installing/>`_.
 
 After that you can install MapProxy with::
 
-    c:\Python27\Scripts\easy_install MapProxy
+    c:\Python27\Scripts\pip install MapProxy
 
 This might take a minute.
 
 Dependencies
 ------------
 
 Read :ref:`dependency_details` for more information about all dependencies.
 
 
 Pillow and YAML
 ~~~~~~~~~~~~~~~
 
-Pillow and PyYAML are installed automatically by ``easy_install``.
+Pillow and PyYAML are installed automatically by ``pip``.
 
 PyProj
 ~~~~~~
 
 Since libproj4 is generally not available on a Windows system, you will also need to install the Python package ``pyproj``.
+You need to manually download the ``pyproj`` package for your system. See below for *Platform dependent packages*.
 
 ::
 
-  easy_install pyproj
+  pip install path\to\pyproj-xxx.whl
 
 
 Shapely and GEOS *(optional)*
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-Shapely can be installed with ``easy_install Shapely``. This will already include the required ``geos.dll``.
+Shapely can be installed with ``pip install Shapely``. This will already include the required ``geos.dll``.
 
 
 GDAL *(optional)*
 ~~~~~~~~~~~~~~~~~
 
 MapProxy requires GDAL/OGR for coverage support. MapProxy can either load the ``gdal.dll`` directly or use the ``osgeo.ogr`` Python package. You can `download and install inofficial Windows binaries of GDAL and the Python package <http://www.gisinternals.com/sdk/>`_ (e.g. `gdal-19-xxxx-code.msi`).
 
@@ -83,31 +80,32 @@
 Or you can add it to your `systems environment variables <http://www.computerhope.com/issues/ch000549.htm>`_.
 
 You also need to set ``GDAL_DRIVER_PATH`` or ``OGR_DRIVER_PATH`` to the ``gdalplugins`` directory when you want to use the Oracle plugin (extra download from URL above)::
 
     set GDAL_DRIVER_PATH=C:\Program Files (x86)\GDAL\gdalplugins
 
 
+.. _win_platform_packages:
+
 Platform dependent packages
 ---------------------------
 
-All Python packages are downloaded from http://pypi.python.org/, but not all platform combinations might be available as a binary package, especially if you run a 64bit version of Windows.
+``pip`` downloads all packages from https://pypi.python.org/, but not all platform combinations might be available as a binary package, especially if you run a 64bit version of Python.
 
-If you run into troubles during installation, because it is trying to compile something (e.g. complaining about ``vcvarsall.bat``), you should look at Christoph Gohlke's `Unofficial Windows Binaries for Python Extension Packages <http://www.lfd.uci.edu/~gohlke/pythonlibs/>`_.
+If you run into trouble during installation, because it is trying to compile something (e.g. complaining about ``vcvarsall.bat``), you should look at Christoph Gohlke's `Unofficial Windows Binaries for Python Extension Packages <http://www.lfd.uci.edu/~gohlke/pythonlibs/>`_. This is a reliable site for binary packages for Python. You need to download the right package: The ``cpxx`` code refers to the Python version (e.g. ``cp27`` for Python 2.7); ``win32`` for 32bit Python installations and ``amd64`` for 64bit.
 
-You can install the ``.exe`` packages with ``easy_install``::
+You can install the ``.whl``, ``.zip`` or ``.exe`` packages with ``pip``::
 
-  easy_install path\to\package-xxx.exe
+  pip install path\to\package-xxx.whl
 
 
 Check installation
 ------------------
 
 To check if the MapProxy was successfully installed you can call ``mapproxy-util``. You should see the installed version number.
 ::
 
     mapproxy-util --version
 
 
 Now continue with :ref:`Create a configuration <create_configuration>` from the installation documentation.
 
-
```

### Comparing `MapProxy-1.9.0/doc/labeling.rst` & `MapProxy-1.9.1/doc/labeling.rst`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/Makefile` & `MapProxy-1.9.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/mapproxy_2.rst` & `MapProxy-1.9.1/doc/mapproxy_2.rst`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/mapproxy_util.rst` & `MapProxy-1.9.1/doc/mapproxy_util.rst`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/mapproxy_util_autoconfig.rst` & `MapProxy-1.9.1/doc/mapproxy_util_autoconfig.rst`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/seed.rst` & `MapProxy-1.9.1/doc/seed.rst`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/seed2.rst` & `MapProxy-1.9.1/doc/seed2.rst`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/services.rst` & `MapProxy-1.9.1/doc/services.rst`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/sources.rst` & `MapProxy-1.9.1/doc/sources.rst`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/tutorial.rst` & `MapProxy-1.9.1/doc/tutorial.rst`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/tutorial.yaml` & `MapProxy-1.9.1/doc/tutorial.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/yaml/cache_conf.yaml` & `MapProxy-1.9.1/doc/yaml/cache_conf.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/yaml/grid_conf.yaml` & `MapProxy-1.9.1/doc/yaml/grid_conf.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/yaml/merged_conf.yaml` & `MapProxy-1.9.1/doc/yaml/merged_conf.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/yaml/meta_conf.yaml` & `MapProxy-1.9.1/doc/yaml/meta_conf.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/doc/yaml/simple_conf.yaml` & `MapProxy-1.9.1/doc/yaml/simple_conf.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/LICENSE.txt` & `MapProxy-1.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/MANIFEST.in` & `MapProxy-1.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/cache/__init__.py` & `MapProxy-1.9.1/mapproxy/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/cache/base.py` & `MapProxy-1.9.1/mapproxy/cache/base.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/cache/couchdb.py` & `MapProxy-1.9.1/mapproxy/cache/couchdb.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/cache/dummy.py` & `MapProxy-1.9.1/mapproxy/cache/dummy.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/cache/file.py` & `MapProxy-1.9.1/mapproxy/cache/file.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/cache/legend.py` & `MapProxy-1.9.1/mapproxy/cache/legend.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/cache/mbtiles.py` & `MapProxy-1.9.1/mapproxy/cache/mbtiles.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/cache/meta.py` & `MapProxy-1.9.1/mapproxy/cache/meta.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/cache/renderd.py` & `MapProxy-1.9.1/mapproxy/cache/renderd.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/cache/riak.py` & `MapProxy-1.9.1/mapproxy/cache/riak.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/cache/sqlite.py` & `MapProxy-1.9.1/mapproxy/cache/sqlite.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/cache/tile.py` & `MapProxy-1.9.1/mapproxy/cache/tile.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/client/arcgis.py` & `MapProxy-1.9.1/mapproxy/client/arcgis.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/client/cgi.py` & `MapProxy-1.9.1/mapproxy/client/cgi.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/client/http.py` & `MapProxy-1.9.1/mapproxy/client/http.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/client/log.py` & `MapProxy-1.9.1/mapproxy/client/log.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/client/tile.py` & `MapProxy-1.9.1/mapproxy/client/tile.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/client/wms.py` & `MapProxy-1.9.1/mapproxy/client/wms.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/compat/__init__.py` & `MapProxy-1.9.1/mapproxy/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/compat/image.py` & `MapProxy-1.9.1/mapproxy/compat/image.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/config/__init__.py` & `MapProxy-1.9.1/mapproxy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/config/config.py` & `MapProxy-1.9.1/mapproxy/config/config.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/config/coverage.py` & `MapProxy-1.9.1/mapproxy/config/coverage.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/config/defaults.py` & `MapProxy-1.9.1/mapproxy/config/defaults.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/config/loader.py` & `MapProxy-1.9.1/mapproxy/config/loader.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/config/spec.py` & `MapProxy-1.9.1/mapproxy/config/spec.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/config/validator.py` & `MapProxy-1.9.1/mapproxy/config/validator.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/config_template/base_config/full_example.yaml` & `MapProxy-1.9.1/mapproxy/config_template/base_config/full_example.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/config_template/base_config/full_seed_example.yaml` & `MapProxy-1.9.1/mapproxy/config_template/base_config/full_seed_example.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/config_template/base_config/log.ini` & `MapProxy-1.9.1/mapproxy/config_template/base_config/log.ini`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/config_template/base_config/mapproxy.yaml` & `MapProxy-1.9.1/mapproxy/config_template/base_config/mapproxy.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/config_template/base_config/seed.yaml` & `MapProxy-1.9.1/mapproxy/config_template/base_config/seed.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/config_template/paster/etc/develop.ini` & `MapProxy-1.9.1/mapproxy/config_template/paster/etc/develop.ini`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/config_template/paster/etc/log_deploy.ini` & `MapProxy-1.9.1/mapproxy/config_template/paster/etc/log_deploy.ini`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/config_template/paster/etc/mapproxy.yaml` & `MapProxy-1.9.1/mapproxy/config_template/paster/etc/mapproxy.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/config_template/paster/etc/seed.yaml` & `MapProxy-1.9.1/mapproxy/config_template/paster/etc/seed.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/exception.py` & `MapProxy-1.9.1/mapproxy/exception.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/featureinfo.py` & `MapProxy-1.9.1/mapproxy/featureinfo.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/grid.py` & `MapProxy-1.9.1/mapproxy/grid.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/image/__init__.py` & `MapProxy-1.9.1/mapproxy/image/__init__.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/image/fonts/DejaVuSans.ttf` & `MapProxy-1.9.1/mapproxy/image/fonts/DejaVuSans.ttf`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/image/fonts/DejaVuSansMono.ttf` & `MapProxy-1.9.1/mapproxy/image/fonts/DejaVuSansMono.ttf`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/image/fonts/LICENSE` & `MapProxy-1.9.1/mapproxy/image/fonts/LICENSE`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/image/mask.py` & `MapProxy-1.9.1/mapproxy/image/mask.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/image/merge.py` & `MapProxy-1.9.1/mapproxy/image/merge.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/image/message.py` & `MapProxy-1.9.1/mapproxy/image/message.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/image/opts.py` & `MapProxy-1.9.1/mapproxy/image/opts.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/image/tile.py` & `MapProxy-1.9.1/mapproxy/image/tile.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/image/transform.py` & `MapProxy-1.9.1/mapproxy/image/transform.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/layer.py` & `MapProxy-1.9.1/mapproxy/layer.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/multiapp.py` & `MapProxy-1.9.1/mapproxy/multiapp.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/proj.py` & `MapProxy-1.9.1/mapproxy/proj.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/request/__init__.py` & `MapProxy-1.9.1/mapproxy/request/__init__.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/request/arcgis.py` & `MapProxy-1.9.1/mapproxy/request/arcgis.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/request/base.py` & `MapProxy-1.9.1/mapproxy/request/base.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/request/tile.py` & `MapProxy-1.9.1/mapproxy/request/tile.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/request/wms/__init__.py` & `MapProxy-1.9.1/mapproxy/request/wms/__init__.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/request/wms/exception.py` & `MapProxy-1.9.1/mapproxy/request/wms/exception.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/request/wmts.py` & `MapProxy-1.9.1/mapproxy/request/wmts.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/response.py` & `MapProxy-1.9.1/mapproxy/response.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/script/conf/app.py` & `MapProxy-1.9.1/mapproxy/script/conf/app.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/script/conf/caches.py` & `MapProxy-1.9.1/mapproxy/script/conf/caches.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/script/conf/layers.py` & `MapProxy-1.9.1/mapproxy/script/conf/layers.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/script/conf/seeds.py` & `MapProxy-1.9.1/mapproxy/script/conf/seeds.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/script/conf/sources.py` & `MapProxy-1.9.1/mapproxy/script/conf/sources.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/script/conf/utils.py` & `MapProxy-1.9.1/mapproxy/script/conf/utils.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/script/export.py` & `MapProxy-1.9.1/mapproxy/script/export.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/script/grids.py` & `MapProxy-1.9.1/mapproxy/script/grids.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/script/scales.py` & `MapProxy-1.9.1/mapproxy/script/scales.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/script/util.py` & `MapProxy-1.9.1/mapproxy/script/util.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/script/wms_capabilities.py` & `MapProxy-1.9.1/mapproxy/script/wms_capabilities.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/seed/cachelock.py` & `MapProxy-1.9.1/mapproxy/seed/cachelock.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/seed/cleanup.py` & `MapProxy-1.9.1/mapproxy/seed/cleanup.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/seed/config.py` & `MapProxy-1.9.1/mapproxy/seed/config.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/seed/script.py` & `MapProxy-1.9.1/mapproxy/seed/script.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/seed/seeder.py` & `MapProxy-1.9.1/mapproxy/seed/seeder.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/seed/spec.py` & `MapProxy-1.9.1/mapproxy/seed/spec.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/seed/util.py` & `MapProxy-1.9.1/mapproxy/seed/util.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/service/__init__.py` & `MapProxy-1.9.1/mapproxy/service/__init__.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/service/base.py` & `MapProxy-1.9.1/mapproxy/service/base.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/service/demo.py` & `MapProxy-1.9.1/mapproxy/service/demo.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/service/kml.py` & `MapProxy-1.9.1/mapproxy/service/kml.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/service/ows.py` & `MapProxy-1.9.1/mapproxy/service/ows.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/service/template_helper.py` & `MapProxy-1.9.1/mapproxy/service/template_helper.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/service/templates/demo/demo.html` & `MapProxy-1.9.1/mapproxy/service/templates/demo/demo.html`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/service/templates/demo/static/img/zoom-world-mini.png` & `MapProxy-1.9.1/mapproxy/service/templates/demo/static/img/zoom-world-mini.png`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/service/templates/demo/static/logo.png` & `MapProxy-1.9.1/mapproxy/service/templates/demo/static/logo.png`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/service/templates/demo/static/OpenLayers.js` & `MapProxy-1.9.1/mapproxy/service/templates/demo/static/OpenLayers.js`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/service/templates/demo/static/site.css` & `MapProxy-1.9.1/mapproxy/service/templates/demo/static/site.css`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/service/templates/demo/static/theme/default/style.css` & `MapProxy-1.9.1/mapproxy/service/templates/demo/static/theme/default/style.css`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/service/templates/demo/static.html` & `MapProxy-1.9.1/mapproxy/service/templates/demo/static.html`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/service/templates/demo/tms_demo.html` & `MapProxy-1.9.1/mapproxy/service/templates/demo/tms_demo.html`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/service/templates/demo/wms_demo.html` & `MapProxy-1.9.1/mapproxy/service/templates/demo/wms_demo.html`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/service/templates/demo/wmts_demo.html` & `MapProxy-1.9.1/mapproxy/service/templates/demo/wmts_demo.html`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/service/templates/tms_tilemap_capabilities.xml` & `MapProxy-1.9.1/mapproxy/service/templates/tms_tilemap_capabilities.xml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/service/templates/wms100capabilities.xml` & `MapProxy-1.9.1/mapproxy/service/templates/wms100capabilities.xml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/service/templates/wms110capabilities.xml` & `MapProxy-1.9.1/mapproxy/service/templates/wms110capabilities.xml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/service/templates/wms111capabilities.xml` & `MapProxy-1.9.1/mapproxy/service/templates/wms111capabilities.xml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/service/templates/wms130capabilities.xml` & `MapProxy-1.9.1/mapproxy/service/templates/wms130capabilities.xml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/service/templates/wmts100capabilities.xml` & `MapProxy-1.9.1/mapproxy/service/templates/wmts100capabilities.xml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/service/tile.py` & `MapProxy-1.9.1/mapproxy/service/tile.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/service/wms.py` & `MapProxy-1.9.1/mapproxy/service/wms.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/service/wmts.py` & `MapProxy-1.9.1/mapproxy/service/wmts.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/source/__init__.py` & `MapProxy-1.9.1/mapproxy/source/__init__.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/source/arcgis.py` & `MapProxy-1.9.1/mapproxy/source/arcgis.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/source/error.py` & `MapProxy-1.9.1/mapproxy/source/error.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/source/mapnik.py` & `MapProxy-1.9.1/mapproxy/source/mapnik.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/source/tile.py` & `MapProxy-1.9.1/mapproxy/source/tile.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/source/wms.py` & `MapProxy-1.9.1/mapproxy/source/wms.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/srs.py` & `MapProxy-1.9.1/mapproxy/srs.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/template.py` & `MapProxy-1.9.1/mapproxy/template.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/helper.py` & `MapProxy-1.9.1/mapproxy/test/helper.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/http.py` & `MapProxy-1.9.1/mapproxy/test/http.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/image.py` & `MapProxy-1.9.1/mapproxy/test/image.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/mocker.py` & `MapProxy-1.9.1/mapproxy/test/mocker.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/common.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/common.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_bul.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_bul.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_cze.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_cze.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_dan.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_dan.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_dut.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_dut.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_eng.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_eng.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_est.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_est.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_fin.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_fin.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_fre.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_fre.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_ger.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_ger.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_gle.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_gle.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_gre.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_gre.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_hun.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_hun.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_ita.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_ita.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_lav.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_lav.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_lit.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_lit.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_mlt.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_mlt.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_pol.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_pol.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_por.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_por.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_rum.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_rum.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_slo.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_slo.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_slv.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_slv.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_spa.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_spa.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/enums/enum_swe.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/enums/enum_swe.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/examples/inspireresourcemddataset.xml` & `MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/examples/inspireresourcemddataset.xml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/examples/inspireresourcemdseries.xml` & `MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/examples/inspireresourcemdseries.xml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/examples/inspireresourcemdservice.xml` & `MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/examples/inspireresourcemdservice.xml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/inspire/common/1.0/network.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/inspire/common/1.0/network.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/inspire/inspire_vs/1.0/examples/wms_at.xml` & `MapProxy-1.9.1/mapproxy/test/schemas/inspire/inspire_vs/1.0/examples/wms_at.xml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/inspire/inspire_vs/1.0/examples/wms_geoimage.xml` & `MapProxy-1.9.1/mapproxy/test/schemas/inspire/inspire_vs/1.0/examples/wms_geoimage.xml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/inspire/inspire_vs/1.0/examples/WMS_Image2000GetCapabilities_InspireSchema.xml` & `MapProxy-1.9.1/mapproxy/test/schemas/inspire/inspire_vs/1.0/examples/WMS_Image2000GetCapabilities_InspireSchema.xml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/inspire/inspire_vs/1.0/inspire_vs.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/inspire/inspire_vs/1.0/inspire_vs.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/kml/2.2.0/atom-author-link.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/kml/2.2.0/atom-author-link.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/kml/2.2.0/ogckml22.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/kml/2.2.0/ogckml22.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/kml/2.2.0/xAL.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/kml/2.2.0/xAL.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/ows/1.1.0/ows19115subset.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/ows/1.1.0/ows19115subset.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/ows/1.1.0/owsAll.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/ows/1.1.0/owsAll.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/ows/1.1.0/owsCommon.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/ows/1.1.0/owsCommon.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/ows/1.1.0/owsContents.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/ows/1.1.0/owsContents.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/ows/1.1.0/owsDataIdentification.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/ows/1.1.0/owsDataIdentification.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/ows/1.1.0/owsDomainType.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/ows/1.1.0/owsDomainType.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/ows/1.1.0/owsExceptionReport.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/ows/1.1.0/owsExceptionReport.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/ows/1.1.0/owsGetCapabilities.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/ows/1.1.0/owsGetCapabilities.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/ows/1.1.0/owsGetResourceByID.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/ows/1.1.0/owsGetResourceByID.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/ows/1.1.0/owsInputOutputData.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/ows/1.1.0/owsInputOutputData.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/ows/1.1.0/owsManifest.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/ows/1.1.0/owsManifest.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/ows/1.1.0/owsOperationsMetadata.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/ows/1.1.0/owsOperationsMetadata.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/ows/1.1.0/owsServiceIdentification.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/ows/1.1.0/owsServiceIdentification.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/ows/1.1.0/owsServiceProvider.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/ows/1.1.0/owsServiceProvider.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/ows/1.1.0/ReadMe.txt` & `MapProxy-1.9.1/mapproxy/test/schemas/ows/1.1.0/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/sld/1.1.0/sld_capabilities.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/sld/1.1.0/sld_capabilities.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wms/1.0.0/capabilities_1_0_0.dtd` & `MapProxy-1.9.1/mapproxy/test/schemas/wms/1.0.0/capabilities_1_0_0.dtd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wms/1.0.0/capabilities_1_0_0.xml` & `MapProxy-1.9.1/mapproxy/test/schemas/wms/1.0.0/capabilities_1_0_0.xml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wms/1.0.7/capabilities_1_0_7.dtd` & `MapProxy-1.9.1/mapproxy/test/schemas/wms/1.0.7/capabilities_1_0_7.dtd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wms/1.0.7/capabilities_1_0_7.xml` & `MapProxy-1.9.1/mapproxy/test/schemas/wms/1.0.7/capabilities_1_0_7.xml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wms/1.1.0/capabilities_1_1_0.dtd` & `MapProxy-1.9.1/mapproxy/test/schemas/wms/1.1.0/capabilities_1_1_0.dtd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wms/1.1.0/capabilities_1_1_0.xml` & `MapProxy-1.9.1/mapproxy/test/schemas/wms/1.1.0/capabilities_1_1_0.xml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wms/1.1.0/exception_1_1_0.xml` & `MapProxy-1.9.1/mapproxy/test/schemas/wms/1.1.0/exception_1_1_0.xml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wms/1.1.1/capabilities_1_1_1.dtd` & `MapProxy-1.9.1/mapproxy/test/schemas/wms/1.1.1/capabilities_1_1_1.dtd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wms/1.1.1/capabilities_1_1_1.xml` & `MapProxy-1.9.1/mapproxy/test/schemas/wms/1.1.1/capabilities_1_1_1.xml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wms/1.1.1/exception_1_1_1.xml` & `MapProxy-1.9.1/mapproxy/test/schemas/wms/1.1.1/exception_1_1_1.xml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wms/1.1.1/OGC-exception.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/wms/1.1.1/OGC-exception.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wms/1.1.1/WMS_DescribeLayerResponse.dtd` & `MapProxy-1.9.1/mapproxy/test/schemas/wms/1.1.1/WMS_DescribeLayerResponse.dtd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wms/1.1.1/WMS_MS_Capabilities.dtd` & `MapProxy-1.9.1/mapproxy/test/schemas/wms/1.1.1/WMS_MS_Capabilities.dtd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wms/1.3.0/capabilities_1_3_0.xml` & `MapProxy-1.9.1/mapproxy/test/schemas/wms/1.3.0/capabilities_1_3_0.xml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wms/1.3.0/capabilities_1_3_0.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/wms/1.3.0/capabilities_1_3_0.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wms/1.3.0/exceptions_1_3_0.xml` & `MapProxy-1.9.1/mapproxy/test/schemas/wms/1.3.0/exceptions_1_3_0.xml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wms/1.3.0/exceptions_1_3_0.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/wms/1.3.0/exceptions_1_3_0.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wmsc/1.1.1/capabilities_1_1_1.dtd` & `MapProxy-1.9.1/mapproxy/test/schemas/wmsc/1.1.1/capabilities_1_1_1.dtd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wmsc/1.1.1/capabilities_1_1_1.xml` & `MapProxy-1.9.1/mapproxy/test/schemas/wmsc/1.1.1/capabilities_1_1_1.xml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wmsc/1.1.1/exception_1_1_1.xml` & `MapProxy-1.9.1/mapproxy/test/schemas/wmsc/1.1.1/exception_1_1_1.xml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wmsc/1.1.1/OGC-exception.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/wmsc/1.1.1/OGC-exception.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wmsc/1.1.1/WMS_DescribeLayerResponse.dtd` & `MapProxy-1.9.1/mapproxy/test/schemas/wmsc/1.1.1/WMS_DescribeLayerResponse.dtd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wmsc/1.1.1/WMS_MS_Capabilities.dtd` & `MapProxy-1.9.1/mapproxy/test/schemas/wmsc/1.1.1/WMS_MS_Capabilities.dtd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wmts/1.0/ReadMe.txt` & `MapProxy-1.9.1/mapproxy/test/schemas/wmts/1.0/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wmts/1.0/wmts.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/wmts/1.0/wmts.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wmts/1.0/wmtsAbstract.wsdl` & `MapProxy-1.9.1/mapproxy/test/schemas/wmts/1.0/wmtsAbstract.wsdl`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wmts/1.0/wmtsGetCapabilities_request.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/wmts/1.0/wmtsGetCapabilities_request.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wmts/1.0/wmtsGetCapabilities_response.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/wmts/1.0/wmtsGetCapabilities_response.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wmts/1.0/wmtsGetFeatureInfo_request.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/wmts/1.0/wmtsGetFeatureInfo_request.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wmts/1.0/wmtsGetFeatureInfo_response.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/wmts/1.0/wmtsGetFeatureInfo_response.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wmts/1.0/wmtsGetTile_request.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/wmts/1.0/wmtsGetTile_request.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wmts/1.0/wmtsKVP.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/wmts/1.0/wmtsKVP.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/wmts/1.0/wmtsPayload_response.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/wmts/1.0/wmtsPayload_response.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/xlink/1.0.0/xlinks.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/xlink/1.0.0/xlinks.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/schemas/xml.xsd` & `MapProxy-1.9.1/mapproxy/test/schemas/xml.xsd`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/__init__.py` & `MapProxy-1.9.1/mapproxy/test/system/__init__.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/arcgis.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/arcgis.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/auth.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/auth.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/cache.mbtiles` & `MapProxy-1.9.1/mapproxy/test/system/fixture/cache.mbtiles`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/cache_band_merge.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/cache_band_merge.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/cache_data/dop_cache_EPSG3857/00/000/000/000/000/000/000.png` & `MapProxy-1.9.1/mapproxy/test/system/fixture/cache_data/dop_cache_EPSG3857/00/000/000/000/000/000/000.png`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/cache_data/wms_cache_EPSG900913/01/000/000/000/000/000/001.jpeg` & `MapProxy-1.9.1/mapproxy/test/system/fixture/cache_data/wms_cache_EPSG900913/01/000/000/000/000/000/001.jpeg`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/cache_grid_names.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/cache_grid_names.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/cache_source.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/cache_source.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/cgi.py` & `MapProxy-1.9.1/mapproxy/test/system/fixture/cgi.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/combined_sources.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/combined_sources.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/coverage.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/coverage.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/formats.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/formats.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/inspire.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/inspire.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/inspire_full.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/inspire_full.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/kml_layer.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/kml_layer.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/layer.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/layer.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/layergroups.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/layergroups.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/layergroups_root.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/layergroups_root.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/legendgraphic.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/legendgraphic.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/mapnik_source.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/mapnik_source.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/mixed_mode.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/mixed_mode.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/multi_cache_layers.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/multi_cache_layers.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/renderd_client.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/renderd_client.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/scalehints.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/scalehints.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/seed.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/seed.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/seed_mapproxy.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/seed_mapproxy.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/seedonly.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/seedonly.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/sld.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/sld.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/source_errors.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/source_errors.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/source_errors_raise.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/source_errors_raise.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/util-conf-wms-111-cap.xml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/util-conf-wms-111-cap.xml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/util_grids.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/util_grids.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/util_wms_capabilities111.xml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/util_wms_capabilities111.xml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/util_wms_capabilities130.xml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/util_wms_capabilities130.xml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/watermark.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/watermark.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/wms_srs_extent.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/wms_srs_extent.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/wms_versions.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/wms_versions.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/wmts.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/wmts.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/wmts_dimensions.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/wmts_dimensions.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/fixture/xslt_featureinfo.yaml` & `MapProxy-1.9.1/mapproxy/test/system/fixture/xslt_featureinfo.yaml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_arcgis.py` & `MapProxy-1.9.1/mapproxy/test/system/test_arcgis.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_auth.py` & `MapProxy-1.9.1/mapproxy/test/system/test_auth.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_behind_proxy.py` & `MapProxy-1.9.1/mapproxy/test/system/test_behind_proxy.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_cache_band_merge.py` & `MapProxy-1.9.1/mapproxy/test/system/test_cache_band_merge.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_cache_grid_names.py` & `MapProxy-1.9.1/mapproxy/test/system/test_cache_grid_names.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_cache_mbtiles.py` & `MapProxy-1.9.1/mapproxy/test/system/test_cache_mbtiles.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_cache_source.py` & `MapProxy-1.9.1/mapproxy/test/system/test_cache_source.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_combined_sources.py` & `MapProxy-1.9.1/mapproxy/test/system/test_combined_sources.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_coverage.py` & `MapProxy-1.9.1/mapproxy/test/system/test_coverage.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_decorate_img.py` & `MapProxy-1.9.1/mapproxy/test/system/test_decorate_img.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_disable_storage.py` & `MapProxy-1.9.1/mapproxy/test/system/test_disable_storage.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_formats.py` & `MapProxy-1.9.1/mapproxy/test/system/test_formats.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_inspire_vs.py` & `MapProxy-1.9.1/mapproxy/test/system/test_inspire_vs.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_kml.py` & `MapProxy-1.9.1/mapproxy/test/system/test_kml.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_layergroups.py` & `MapProxy-1.9.1/mapproxy/test/system/test_layergroups.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_legendgraphic.py` & `MapProxy-1.9.1/mapproxy/test/system/test_legendgraphic.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_mapnik.py` & `MapProxy-1.9.1/mapproxy/test/system/test_mapnik.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_mapserver.py` & `MapProxy-1.9.1/mapproxy/test/system/test_mapserver.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_mixed_mode_format.py` & `MapProxy-1.9.1/mapproxy/test/system/test_mixed_mode_format.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_multi_cache_layers.py` & `MapProxy-1.9.1/mapproxy/test/system/test_multi_cache_layers.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_multiapp.py` & `MapProxy-1.9.1/mapproxy/test/system/test_multiapp.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_renderd_client.py` & `MapProxy-1.9.1/mapproxy/test/system/test_renderd_client.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_scalehints.py` & `MapProxy-1.9.1/mapproxy/test/system/test_scalehints.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_seed.py` & `MapProxy-1.9.1/mapproxy/test/system/test_seed.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_seed_only.py` & `MapProxy-1.9.1/mapproxy/test/system/test_seed_only.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_sld.py` & `MapProxy-1.9.1/mapproxy/test/system/test_sld.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_source_errors.py` & `MapProxy-1.9.1/mapproxy/test/system/test_source_errors.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_tilesource_minmax_res.py` & `MapProxy-1.9.1/mapproxy/test/system/test_tilesource_minmax_res.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_tms.py` & `MapProxy-1.9.1/mapproxy/test/system/test_tms.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_tms_origin.py` & `MapProxy-1.9.1/mapproxy/test/system/test_tms_origin.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_util_conf.py` & `MapProxy-1.9.1/mapproxy/test/system/test_util_conf.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_util_export.py` & `MapProxy-1.9.1/mapproxy/test/system/test_util_export.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_util_grids.py` & `MapProxy-1.9.1/mapproxy/test/system/test_util_grids.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_util_wms_capabilities.py` & `MapProxy-1.9.1/mapproxy/test/system/test_util_wms_capabilities.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_watermark.py` & `MapProxy-1.9.1/mapproxy/test/system/test_watermark.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_wms.py` & `MapProxy-1.9.1/mapproxy/test/system/test_wms.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_wms_srs_extent.py` & `MapProxy-1.9.1/mapproxy/test/system/test_wms_srs_extent.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_wms_version.py` & `MapProxy-1.9.1/mapproxy/test/system/test_wms_version.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_wmsc.py` & `MapProxy-1.9.1/mapproxy/test/system/test_wmsc.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_wmts.py` & `MapProxy-1.9.1/mapproxy/test/system/test_wmts.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_wmts_dimensions.py` & `MapProxy-1.9.1/mapproxy/test/system/test_wmts_dimensions.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_wmts_restful.py` & `MapProxy-1.9.1/mapproxy/test/system/test_wmts_restful.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/system/test_xslt_featureinfo.py` & `MapProxy-1.9.1/mapproxy/test/system/test_xslt_featureinfo.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/test_http_helper.py` & `MapProxy-1.9.1/mapproxy/test/test_http_helper.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/polygons/polygons.dbf` & `MapProxy-1.9.1/mapproxy/test/unit/polygons/polygons.dbf`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/polygons/polygons.shp` & `MapProxy-1.9.1/mapproxy/test/unit/polygons/polygons.shp`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_async.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_async.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_auth.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_auth.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_cache.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_cache.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_cache_couchdb.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_cache_couchdb.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_cache_riak.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_cache_riak.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_cache_tile.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_cache_tile.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_client.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_client_cgi.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_client_cgi.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_collections.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_collections.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_concat_legends.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_concat_legends.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_conf_loader.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_conf_loader.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_conf_validator.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_conf_validator.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_config.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_decorate_img.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_decorate_img.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_exceptions.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_featureinfo.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_featureinfo.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_file_lock_load.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_file_lock_load.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_geom.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_geom.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_grid.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_grid.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_image.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_image.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_image_mask.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_image_mask.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_image_messages.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_image_messages.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_image_options.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_image_options.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_multiapp.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_multiapp.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_ogr_reader.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_ogr_reader.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_request.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_request.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_request_wmts.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_request_wmts.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_response.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_response.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_seed.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_seed.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_seed_cachelock.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_seed_cachelock.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_srs.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_srs.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_tiled_source.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_tiled_source.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_tilefilter.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_tilefilter.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_timeutils.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_timeutils.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_util_conf_utils.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_util_conf_utils.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_utils.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_wms_capabilities.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_wms_capabilities.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_wms_layer.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_wms_layer.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/test/unit/test_yaml.py` & `MapProxy-1.9.1/mapproxy/test/unit/test_yaml.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/tilefilter.py` & `MapProxy-1.9.1/mapproxy/tilefilter.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/util/async.py` & `MapProxy-1.9.1/mapproxy/util/async.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/util/collections.py` & `MapProxy-1.9.1/mapproxy/util/collections.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/util/coverage.py` & `MapProxy-1.9.1/mapproxy/util/coverage.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/util/ext/__init__.py` & `MapProxy-1.9.1/mapproxy/util/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/util/ext/dictspec/spec.py` & `MapProxy-1.9.1/mapproxy/util/ext/dictspec/spec.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/util/ext/dictspec/test/test_validator.py` & `MapProxy-1.9.1/mapproxy/util/ext/dictspec/test/test_validator.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/util/ext/dictspec/validator.py` & `MapProxy-1.9.1/mapproxy/util/ext/dictspec/validator.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/util/ext/local.py` & `MapProxy-1.9.1/mapproxy/util/ext/local.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/util/ext/lockfile.py` & `MapProxy-1.9.1/mapproxy/util/ext/lockfile.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/util/ext/odict.py` & `MapProxy-1.9.1/mapproxy/util/ext/odict.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/util/ext/serving.py` & `MapProxy-1.9.1/mapproxy/util/ext/serving.py`

 * *Files 2% similar despite different names*

```diff
@@ -600,20 +600,25 @@
     """Spawn a new Python interpreter with the same arguments as this one,
     but running the reloader thread.
     """
     while 1:
         _log('info', ' * Restarting with reloader')
 
         args = [sys.executable] + sys.argv
-        # pip installs commands as .exe, but sys.argv[0]
-        # can miss the prefix. add .exe to avoid file-not-found
-        # in subprocess call
-        if os.name == 'nt' and '.' not in args[1]:
-            args[1] = args[1] + '.exe'
-
+        if os.name == 'nt':
+            # pip installs commands as .exe, but sys.argv[0]
+            # can miss the prefix.
+            # Add .exe to avoid file-not-found in subprocess call.
+            # Also, recent pip versions create .exe commands that are not
+            # executable by Python, but there is a -script.py which
+            # we need to call in this case. Check for this first.
+            if os.path.exists(args[1] + '-script.py'):
+                args[1] = args[1] + '-script.py'
+            elif not args[1].endswith('.exe'):
+                args[1] = args[1] + '.exe'
         new_environ = os.environ.copy()
         new_environ['WERKZEUG_RUN_MAIN'] = 'true'
 
         # a weird bug on windows. sometimes unicode strings end up in the
         # environment and subprocess.call does not like this, encode them
         # to latin1 and continue.
         if os.name == 'nt' and PY2:
```

### Comparing `MapProxy-1.9.0/mapproxy/util/ext/tempita/__init__.py` & `MapProxy-1.9.1/mapproxy/util/ext/tempita/__init__.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/util/ext/tempita/_looper.py` & `MapProxy-1.9.1/mapproxy/util/ext/tempita/_looper.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/util/ext/tempita/compat3.py` & `MapProxy-1.9.1/mapproxy/util/ext/tempita/compat3.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/util/ext/wmsparse/parse.py` & `MapProxy-1.9.1/mapproxy/util/ext/wmsparse/parse.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/util/ext/wmsparse/test/test_parse.py` & `MapProxy-1.9.1/mapproxy/util/ext/wmsparse/test/test_parse.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/util/ext/wmsparse/test/test_util.py` & `MapProxy-1.9.1/mapproxy/util/ext/wmsparse/test/test_util.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/util/ext/wmsparse/test/wms-large-111.xml` & `MapProxy-1.9.1/mapproxy/util/ext/wmsparse/test/wms-large-111.xml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/util/ext/wmsparse/test/wms-omniscale-111.xml` & `MapProxy-1.9.1/mapproxy/util/ext/wmsparse/test/wms-omniscale-111.xml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/util/ext/wmsparse/test/wms-omniscale-130.xml` & `MapProxy-1.9.1/mapproxy/util/ext/wmsparse/test/wms-omniscale-130.xml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/util/ext/wmsparse/test/wms_nasa_cap.xml` & `MapProxy-1.9.1/mapproxy/util/ext/wmsparse/test/wms_nasa_cap.xml`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/util/ext/wmsparse/util.py` & `MapProxy-1.9.1/mapproxy/util/ext/wmsparse/util.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/util/fs.py` & `MapProxy-1.9.1/mapproxy/util/fs.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/util/geom.py` & `MapProxy-1.9.1/mapproxy/util/geom.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/util/lib.py` & `MapProxy-1.9.1/mapproxy/util/lib.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/util/lock.py` & `MapProxy-1.9.1/mapproxy/util/lock.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/util/ogr.py` & `MapProxy-1.9.1/mapproxy/util/ogr.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/util/py.py` & `MapProxy-1.9.1/mapproxy/util/py.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/util/times.py` & `MapProxy-1.9.1/mapproxy/util/times.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/util/wsgi.py` & `MapProxy-1.9.1/mapproxy/util/wsgi.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/util/yaml.py` & `MapProxy-1.9.1/mapproxy/util/yaml.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/version.py` & `MapProxy-1.9.1/mapproxy/version.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/mapproxy/wsgiapp.py` & `MapProxy-1.9.1/mapproxy/wsgiapp.py`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/MapProxy.egg-info/PKG-INFO` & `MapProxy-1.9.1/MapProxy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: MapProxy
-Version: 1.9.0
+Version: 1.9.1
 Summary: An accelerating proxy for web map services
 Home-page: http://mapproxy.org
 Author: Oliver Tonnhofer
 Author-email: olt@omniscale.de
 License: Apache Software License 2.0
 Description: MapProxy is an open source proxy for geospatial data. It caches, accelerates and transforms data from existing map services and serves any desktop or web GIS client.
         
@@ -16,14 +16,22 @@
         
         Go to http://mapproxy.org/ for more information.
         
         The documentation is available at: http://mapproxy.org/docs/latest/
         
         Changes
         -------
+        1.9.1 2017-01-18
+        ~~~~~~~~~~~~~~~~
+        
+        Fixes:
+        
+        - serve-develop: fixed reloader for Windows installations made
+          with recent pip version (#279)
+        
         1.9.0 2016-07-22
         ~~~~~~~~~~~~~~~~
         
         Improvements:
         
         - New band merge feature. Allows to create false-color or grayscale
           images on the fly.
@@ -162,31 +170,14 @@
         - only init libproj when requested
         
         Other:
         
         - 1.7.x is the last release with support for Python 2.5
         - depend on Pillow if PIL is not installed
         
-        1.6.0 2013-09-12
-        ~~~~~~~~~~~~~~~~
-        
-        Improvements:
-        
-        - Riak cache supports multiple nodes
-        
-        Fixes:
-        
-        - handle SSL verification when using HTTP proxy
-        - ignore errors during single color symlinking
-        
-        Other:
-        
-        - --debug option for serve-multiapp-develop
-        - Riak cache requires Riak-Client >=2.0
-        
         
         Older changes
         -------------
         See https://raw.github.com/mapproxy/mapproxy/master/CHANGES.txt
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `MapProxy-1.9.0/MapProxy.egg-info/SOURCES.txt` & `MapProxy-1.9.1/MapProxy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -312,14 +312,15 @@
 mapproxy/test/schemas/wmts/1.0/wmtsPayload_response.xsd
 mapproxy/test/schemas/xlink/1.0.0/ReadMe.txt
 mapproxy/test/schemas/xlink/1.0.0/xlinks.xsd
 mapproxy/test/system/__init__.py
 mapproxy/test/system/test_arcgis.py
 mapproxy/test/system/test_auth.py
 mapproxy/test/system/test_behind_proxy.py
+mapproxy/test/system/test_bulk_meta_tiles.py
 mapproxy/test/system/test_cache_band_merge.py
 mapproxy/test/system/test_cache_grid_names.py
 mapproxy/test/system/test_cache_mbtiles.py
 mapproxy/test/system/test_cache_source.py
 mapproxy/test/system/test_combined_sources.py
 mapproxy/test/system/test_coverage.py
 mapproxy/test/system/test_decorate_img.py
@@ -356,14 +357,15 @@
 mapproxy/test/system/test_wmts_dimensions.py
 mapproxy/test/system/test_wmts_restful.py
 mapproxy/test/system/test_xslt_featureinfo.py
 mapproxy/test/system/fixture/arcgis.yaml
 mapproxy/test/system/fixture/auth.yaml
 mapproxy/test/system/fixture/cache.mbtiles
 mapproxy/test/system/fixture/cache_band_merge.yaml
+mapproxy/test/system/fixture/cache_bulk_meta_tiles.yaml
 mapproxy/test/system/fixture/cache_grid_names.yaml
 mapproxy/test/system/fixture/cache_mbtiles.yaml
 mapproxy/test/system/fixture/cache_source.yaml
 mapproxy/test/system/fixture/cgi.py
 mapproxy/test/system/fixture/combined_sources.yaml
 mapproxy/test/system/fixture/coverage.yaml
 mapproxy/test/system/fixture/disable_storage.yaml
```

### Comparing `MapProxy-1.9.0/PKG-INFO` & `MapProxy-1.9.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: MapProxy
-Version: 1.9.0
+Version: 1.9.1
 Summary: An accelerating proxy for web map services
 Home-page: http://mapproxy.org
 Author: Oliver Tonnhofer
 Author-email: olt@omniscale.de
 License: Apache Software License 2.0
 Description: MapProxy is an open source proxy for geospatial data. It caches, accelerates and transforms data from existing map services and serves any desktop or web GIS client.
         
@@ -16,14 +16,22 @@
         
         Go to http://mapproxy.org/ for more information.
         
         The documentation is available at: http://mapproxy.org/docs/latest/
         
         Changes
         -------
+        1.9.1 2017-01-18
+        ~~~~~~~~~~~~~~~~
+        
+        Fixes:
+        
+        - serve-develop: fixed reloader for Windows installations made
+          with recent pip version (#279)
+        
         1.9.0 2016-07-22
         ~~~~~~~~~~~~~~~~
         
         Improvements:
         
         - New band merge feature. Allows to create false-color or grayscale
           images on the fly.
@@ -162,31 +170,14 @@
         - only init libproj when requested
         
         Other:
         
         - 1.7.x is the last release with support for Python 2.5
         - depend on Pillow if PIL is not installed
         
-        1.6.0 2013-09-12
-        ~~~~~~~~~~~~~~~~
-        
-        Improvements:
-        
-        - Riak cache supports multiple nodes
-        
-        Fixes:
-        
-        - handle SSL verification when using HTTP proxy
-        - ignore errors during single color symlinking
-        
-        Other:
-        
-        - --debug option for serve-multiapp-develop
-        - Riak cache requires Riak-Client >=2.0
-        
         
         Older changes
         -------------
         See https://raw.github.com/mapproxy/mapproxy/master/CHANGES.txt
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `MapProxy-1.9.0/README.rst` & `MapProxy-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `MapProxy-1.9.0/setup.py` & `MapProxy-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         -------------
         See https://raw.github.com/mapproxy/mapproxy/master/CHANGES.txt
         '''))
     return readme + ''.join(changes)
 
 setup(
     name='MapProxy',
-    version="1.9.0",
+    version="1.9.1",
     description='An accelerating proxy for web map services',
     long_description=long_description(7),
     author='Oliver Tonnhofer',
     author_email='olt@omniscale.de',
     url='http://mapproxy.org',
     license='Apache Software License 2.0',
     namespace_packages = ['mapproxy'],
```

