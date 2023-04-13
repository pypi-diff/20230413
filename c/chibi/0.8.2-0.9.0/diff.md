# Comparing `tmp/chibi-0.8.2.tar.gz` & `tmp/chibi-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chibi-0.8.2.tar", last modified: Tue Mar 31 19:17:40 2020, max compression
+gzip compressed data, was "dist/chibi-0.9.0.tar", last modified: Fri Jun 26 06:41:06 2020, max compression
```

## Comparing `chibi-0.8.2.tar` & `chibi-0.9.0.tar`

### file list

```diff
@@ -1,263 +1,215 @@
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:40.062238 chibi-0.8.2/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      150 2020-02-23 22:26:05.000000 chibi-0.8.2/AUTHORS.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3487 2020-02-23 22:28:08.000000 chibi-0.8.2/CONTRIBUTING.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      108 2020-02-24 01:48:21.000000 chibi-0.8.2/HISTORY.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      481 2019-12-21 21:12:58.000000 chibi-0.8.2/LICENSE
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      262 2020-02-23 22:30:23.000000 chibi-0.8.2/MANIFEST.in
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2429 2020-03-31 19:17:40.062238 chibi-0.8.2/PKG-INFO
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1263 2020-02-23 22:24:11.000000 chibi-0.8.2/README.rst
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:39.915571 chibi-0.8.2/chibi/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      106 2020-03-31 19:17:21.000000 chibi-0.8.2/chibi/__init__.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:39.915571 chibi-0.8.2/chibi/atlas/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3578 2020-03-08 06:58:01.000000 chibi-0.8.2/chibi/atlas/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2656 2019-04-08 19:18:19.000000 chibi-0.8.2/chibi/atlas/tree.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      231 2018-12-12 21:14:52.000000 chibi-0.8.2/chibi/b64.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:39.915571 chibi-0.8.2/chibi/chain/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1054 2019-12-21 21:12:58.000000 chibi-0.8.2/chibi/chain/__init__.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:39.948904 chibi-0.8.2/chibi/command/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1686 2020-03-10 20:49:38.000000 chibi-0.8.2/chibi/command/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      215 2020-03-10 20:49:38.000000 chibi-0.8.2/chibi/command/dd.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:39.952237 chibi-0.8.2/chibi/command/disk/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-10 20:49:38.000000 chibi-0.8.2/chibi/command/disk/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      269 2020-03-10 20:49:38.000000 chibi-0.8.2/chibi/command/disk/dd.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      162 2020-03-10 20:49:38.000000 chibi-0.8.2/chibi/command/disk/format.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      182 2020-03-10 20:49:38.000000 chibi-0.8.2/chibi/command/disk/mount.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:39.955571 chibi-0.8.2/chibi/command/echo/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      123 2020-03-10 20:49:38.000000 chibi-0.8.2/chibi/command/echo/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      470 2020-03-10 20:49:38.000000 chibi-0.8.2/chibi/command/echo/cowsay.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      457 2020-03-10 20:49:38.000000 chibi-0.8.2/chibi/command/echo/echo.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      472 2020-03-10 20:49:38.000000 chibi-0.8.2/chibi/command/echo/ponysay.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:39.955571 chibi-0.8.2/chibi/command/file/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-10 20:49:38.000000 chibi-0.8.2/chibi/command/file/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      150 2020-03-10 20:49:38.000000 chibi-0.8.2/chibi/command/file/tar.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:39.958904 chibi-0.8.2/chibi/command/firewall/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      620 2020-03-10 20:49:38.000000 chibi-0.8.2/chibi/command/firewall/__init__.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:39.968904 chibi-0.8.2/chibi/command/git/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      850 2020-03-10 20:49:38.000000 chibi-0.8.2/chibi/command/git/__init__.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:39.968904 chibi-0.8.2/chibi/command/mpd/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-10 20:49:38.000000 chibi-0.8.2/chibi/command/mpd/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      334 2020-03-10 20:49:38.000000 chibi-0.8.2/chibi/command/mpd/mpc.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1897 2020-03-10 20:49:38.000000 chibi-0.8.2/chibi/command/network.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      592 2020-03-10 20:49:38.000000 chibi-0.8.2/chibi/command/nmap.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1443 2020-03-10 20:49:38.000000 chibi-0.8.2/chibi/command/nmcli.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:39.968904 chibi-0.8.2/chibi/command/pip/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      858 2020-03-10 20:49:38.000000 chibi-0.8.2/chibi/command/pip/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      743 2020-03-10 20:49:38.000000 chibi-0.8.2/chibi/command/qr.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:39.972237 chibi-0.8.2/chibi/command/rabbitmq/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      712 2020-03-10 20:49:38.000000 chibi-0.8.2/chibi/command/rabbitmq/__init__.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:39.972237 chibi-0.8.2/chibi/command/rpm/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      162 2020-03-10 20:49:38.000000 chibi-0.8.2/chibi/command/rpm/__init__.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:39.972237 chibi-0.8.2/chibi/command/systemctl/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2093 2020-03-10 20:49:38.000000 chibi-0.8.2/chibi/command/systemctl/__init__.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:39.972237 chibi-0.8.2/chibi/command/yum/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1352 2020-03-10 20:49:38.000000 chibi-0.8.2/chibi/command/yum/__init__.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:39.972237 chibi-0.8.2/chibi/config/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      270 2020-03-06 20:21:02.000000 chibi-0.8.2/chibi/config/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2444 2020-03-08 00:40:45.000000 chibi-0.8.2/chibi/config/config.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      284 2020-03-02 22:57:59.000000 chibi-0.8.2/chibi/config/logger.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:39.975571 chibi-0.8.2/chibi/fancy/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:14:51.000000 chibi-0.8.2/chibi/fancy/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      531 2018-12-12 21:14:51.000000 chibi-0.8.2/chibi/fancy/is_type.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:39.975571 chibi-0.8.2/chibi/file/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      101 2018-12-12 21:14:52.000000 chibi-0.8.2/chibi/file/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     4845 2020-03-13 14:51:40.000000 chibi-0.8.2/chibi/file/file.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1711 2019-09-24 18:14:12.000000 chibi-0.8.2/chibi/file/image.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:39.978904 chibi-0.8.2/chibi/file/other/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      536 2020-03-06 02:06:53.000000 chibi-0.8.2/chibi/file/other/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1676 2020-01-08 04:49:10.000000 chibi-0.8.2/chibi/file/other/chibi_csv.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      319 2019-12-24 06:32:24.000000 chibi-0.8.2/chibi/file/other/chibi_json.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      250 2020-03-06 02:12:49.000000 chibi-0.8.2/chibi/file/other/chibi_python.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      456 2019-12-24 06:31:10.000000 chibi-0.8.2/chibi/file/other/chibi_yaml.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     8989 2020-03-31 18:43:18.000000 chibi-0.8.2/chibi/file/path.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)    10305 2020-03-03 04:18:09.000000 chibi-0.8.2/chibi/file/snippets.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      675 2019-12-21 21:12:58.000000 chibi-0.8.2/chibi/file/temp.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:39.985571 chibi-0.8.2/chibi/madness/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       46 2018-12-12 21:14:52.000000 chibi-0.8.2/chibi/madness/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:14:52.000000 chibi-0.8.2/chibi/madness/byte.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      371 2019-07-18 21:49:37.000000 chibi-0.8.2/chibi/madness/file.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2523 2019-02-26 12:01:40.000000 chibi-0.8.2/chibi/madness/string.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:39.985571 chibi-0.8.2/chibi/metaphors/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       46 2019-12-21 21:25:16.000000 chibi-0.8.2/chibi/metaphors/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1141 2020-02-21 21:24:25.000000 chibi-0.8.2/chibi/metaphors/book.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      502 2019-04-04 18:35:55.000000 chibi-0.8.2/chibi/module.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:39.992237 chibi-0.8.2/chibi/net/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-10 20:48:04.000000 chibi-0.8.2/chibi/net/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       68 2019-07-22 17:38:19.000000 chibi-0.8.2/chibi/net/hostname.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:39.992237 chibi-0.8.2/chibi/net/network/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:14:51.000000 chibi-0.8.2/chibi/net/network/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1145 2019-04-27 00:19:43.000000 chibi-0.8.2/chibi/net/network/interface.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:39.992237 chibi-0.8.2/chibi/net/network_manager/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2019-07-18 14:00:45.000000 chibi-0.8.2/chibi/net/network_manager/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2186 2019-07-22 17:05:16.000000 chibi-0.8.2/chibi/nix.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:39.995571 chibi-0.8.2/chibi/object/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       64 2019-02-14 22:27:50.000000 chibi-0.8.2/chibi/object/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     4883 2019-08-27 15:29:30.000000 chibi-0.8.2/chibi/object/descriptor.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2339 2019-02-26 12:10:40.000000 chibi-0.8.2/chibi/object/object.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1663 2018-12-12 21:14:52.000000 chibi-0.8.2/chibi/parser.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:39.995571 chibi-0.8.2/chibi/pipeline/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       58 2019-04-25 15:54:05.000000 chibi-0.8.2/chibi/pipeline/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1738 2019-06-10 21:29:23.000000 chibi-0.8.2/chibi/pipeline/pipeline.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      211 2019-06-10 21:37:52.000000 chibi-0.8.2/chibi/pipeline/xml.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:39.998904 chibi-0.8.2/chibi/snippet/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:14:52.000000 chibi-0.8.2/chibi/snippet/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     7353 2020-02-21 21:24:25.000000 chibi-0.8.2/chibi/snippet/dict.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)    29717 2019-02-26 12:11:42.000000 chibi-0.8.2/chibi/snippet/extra_string.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2019-07-18 15:16:51.000000 chibi-0.8.2/chibi/snippet/file.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      198 2019-06-10 20:01:16.000000 chibi-0.8.2/chibi/snippet/image.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      898 2019-02-26 12:10:06.000000 chibi-0.8.2/chibi/snippet/is_type.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1131 2019-04-27 00:15:55.000000 chibi-0.8.2/chibi/snippet/iter.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1187 2019-02-26 12:03:24.000000 chibi-0.8.2/chibi/snippet/regex.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2744 2020-03-29 05:37:54.000000 chibi-0.8.2/chibi/snippet/string.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      295 2019-07-22 17:07:01.000000 chibi-0.8.2/chibi/snippet/table.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1235 2019-07-23 21:13:00.000000 chibi-0.8.2/chibi/snippet/xml.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:39.998904 chibi-0.8.2/chibi/units/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:14:52.000000 chibi-0.8.2/chibi/units/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2712 2019-02-26 12:04:25.000000 chibi-0.8.2/chibi/units/base.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1574 2018-12-12 21:14:52.000000 chibi-0.8.2/chibi/units/prefix.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      647 2018-12-12 21:14:52.000000 chibi-0.8.2/chibi/units/si.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:39.915571 chibi-0.8.2/chibi.egg-info/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2429 2020-03-31 19:17:39.000000 chibi-0.8.2/chibi.egg-info/PKG-INFO
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     5348 2020-03-31 19:17:39.000000 chibi-0.8.2/chibi.egg-info/SOURCES.txt
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        1 2020-03-31 19:17:39.000000 chibi-0.8.2/chibi.egg-info/dependency_links.txt
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        1 2020-03-31 19:17:39.000000 chibi-0.8.2/chibi.egg-info/not-zip-safe
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      131 2020-03-31 19:17:39.000000 chibi-0.8.2/chibi.egg-info/requires.txt
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        6 2020-03-31 19:17:39.000000 chibi-0.8.2/chibi.egg-info/top_level.txt
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:40.025571 chibi-0.8.2/docs/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      606 2020-02-23 22:31:16.000000 chibi-0.8.2/docs/Makefile
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       28 2020-02-23 22:30:23.000000 chibi-0.8.2/docs/authors.rst
--rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)     4768 2020-02-23 22:30:49.000000 chibi-0.8.2/docs/conf.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       33 2020-02-23 22:30:23.000000 chibi-0.8.2/docs/contributing.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       28 2020-02-23 22:30:23.000000 chibi-0.8.2/docs/history.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      302 2020-02-23 22:30:56.000000 chibi-0.8.2/docs/index.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1094 2020-02-23 22:31:02.000000 chibi-0.8.2/docs/installation.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      767 2020-02-23 22:31:07.000000 chibi-0.8.2/docs/make.bat
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       27 2020-02-23 22:30:23.000000 chibi-0.8.2/docs/readme.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       65 2020-02-23 22:31:28.000000 chibi-0.8.2/docs/usage.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      443 2020-03-31 19:17:40.062238 chibi-0.8.2/setup.cfg
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1101 2020-03-31 19:17:21.000000 chibi-0.8.2/setup.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:40.028904 chibi-0.8.2/tests/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:15:06.000000 chibi-0.8.2/tests/__init__.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:40.028904 chibi-0.8.2/tests/api/
--rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)    12288 2018-12-12 21:15:07.000000 chibi-0.8.2/tests/api/.endpoint.py.swp
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:40.042238 chibi-0.8.2/tests/atlas/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:15:07.000000 chibi-0.8.2/tests/atlas/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3093 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/atlas/chibi_atlas.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1581 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/atlas/chibi_atlas_ignore_case.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     4762 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/atlas/chibi_tree.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1024 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/atlas/loads.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      359 2018-12-12 21:15:06.000000 chibi-0.8.2/tests/b64.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:40.042238 chibi-0.8.2/tests/chain/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/chain/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2472 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/chain/chain.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:40.045571 chibi-0.8.2/tests/command/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:15:06.000000 chibi-0.8.2/tests/command/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1292 2018-12-12 21:15:06.000000 chibi-0.8.2/tests/command/command.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:40.045571 chibi-0.8.2/tests/command/echo/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:15:06.000000 chibi-0.8.2/tests/command/echo/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      339 2018-12-12 21:15:06.000000 chibi-0.8.2/tests/command/echo/cowsay.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      338 2018-12-12 21:15:06.000000 chibi-0.8.2/tests/command/echo/echo.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      342 2018-12-12 21:15:06.000000 chibi-0.8.2/tests/command/echo/ponysay.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3213 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/command/network.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:40.045571 chibi-0.8.2/tests/command/yum/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:15:06.000000 chibi-0.8.2/tests/command/yum/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      473 2018-12-12 21:15:06.000000 chibi-0.8.2/tests/command/yum/install.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      495 2018-12-12 21:15:06.000000 chibi-0.8.2/tests/command/yum/localinstall.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      456 2018-12-12 21:15:06.000000 chibi-0.8.2/tests/command/yum/update.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      472 2018-12-12 21:15:06.000000 chibi-0.8.2/tests/command/yum/yum.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:40.048904 chibi-0.8.2/tests/config/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-02 22:38:29.000000 chibi-0.8.2/tests/config/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2692 2020-03-08 00:21:55.000000 chibi-0.8.2/tests/config/config.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-03 02:30:48.000000 chibi-0.8.2/tests/config/logger.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:40.052238 chibi-0.8.2/tests/file/
--rw-------   0 dem4ply   (1000) dem4ply   (1000)    58162 2018-12-12 21:15:06.000000 chibi-0.8.2/tests/file/1529990793499.jpg
--rw-------   0 dem4ply   (1000) dem4ply   (1000)   207885 2018-12-12 21:15:06.000000 chibi-0.8.2/tests/file/1535359854403.png
--rw-------   0 dem4ply   (1000) dem4ply   (1000)   563123 2018-12-12 21:15:06.000000 chibi-0.8.2/tests/file/1536637012160.gif
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:15:06.000000 chibi-0.8.2/tests/file/__init__.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:40.052238 chibi-0.8.2/tests/file/chibi_file/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:15:06.000000 chibi-0.8.2/tests/file/chibi_file/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2100 2019-06-11 21:29:13.000000 chibi-0.8.2/tests/file/chibi_file/append.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      394 2018-12-12 21:18:30.000000 chibi-0.8.2/tests/file/chibi_file/check_sum_md5.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      772 2019-12-21 23:55:31.000000 chibi-0.8.2/tests/file/chibi_file/class_resolution.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1157 2019-09-10 17:56:36.000000 chibi-0.8.2/tests/file/chibi_file/copy.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      845 2019-07-22 17:54:24.000000 chibi-0.8.2/tests/file/chibi_file/find.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1015 2019-12-24 06:37:02.000000 chibi-0.8.2/tests/file/chibi_file/json.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      603 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/file/chibi_file/properites.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1496 2019-12-24 06:37:31.000000 chibi-0.8.2/tests/file/chibi_file/yaml.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2392 2020-03-10 20:44:17.000000 chibi-0.8.2/tests/file/image.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:40.055571 chibi-0.8.2/tests/file/orphan_function/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:15:07.000000 chibi-0.8.2/tests/file/orphan_function/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      533 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/file/orphan_function/add_extensions.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1257 2020-02-22 02:54:29.000000 chibi-0.8.2/tests/file/orphan_function/cd.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      622 2020-03-02 16:05:47.000000 chibi-0.8.2/tests/file/orphan_function/chown.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      282 2019-05-04 02:01:25.000000 chibi-0.8.2/tests/file/orphan_function/common_root.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1475 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/file/orphan_function/copy.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      637 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/file/orphan_function/delete.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      570 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/file/orphan_function/exists.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      531 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/file/orphan_function/file_dir.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1591 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/file/orphan_function/find.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      481 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/file/orphan_function/get_relative_path.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      787 2020-02-22 02:52:02.000000 chibi-0.8.2/tests/file/orphan_function/infalte_dir.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      531 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/file/orphan_function/is_dir.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      538 2018-12-12 21:15:06.000000 chibi-0.8.2/tests/file/orphan_function/is_file.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      813 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/file/orphan_function/join.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      996 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/file/orphan_function/ls.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1221 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/file/orphan_function/ls_only_dir.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1479 2020-03-02 16:06:50.000000 chibi-0.8.2/tests/file/orphan_function/mkdir.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1699 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/file/orphan_function/move.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1011 2018-12-12 21:15:07.000000 chibi-0.8.2/tests/file/orphan_function/stat.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:40.055571 chibi-0.8.2/tests/file/other/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/file/other/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2644 2020-01-09 03:57:44.000000 chibi-0.8.2/tests/file/other/chibi_csv.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:40.055571 chibi-0.8.2/tests/file/path/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:15:07.000000 chibi-0.8.2/tests/file/path/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1158 2020-02-22 02:53:47.000000 chibi-0.8.2/tests/file/path/current_dir.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1439 2020-03-31 18:43:02.000000 chibi-0.8.2/tests/file/path/glob.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     8605 2020-03-06 01:57:55.000000 chibi-0.8.2/tests/file/path/path.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1037 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/file/path/temp.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:40.055571 chibi-0.8.2/tests/internet/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:15:06.000000 chibi-0.8.2/tests/internet/__init__.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:40.055571 chibi-0.8.2/tests/internet/api/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:15:06.000000 chibi-0.8.2/tests/internet/api/__init__.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:40.058904 chibi-0.8.2/tests/internet/api/four_chan/
--rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)    12288 2018-12-12 21:15:06.000000 chibi-0.8.2/tests/internet/api/four_chan/.client.py.swo
--rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)    12288 2018-12-12 21:15:06.000000 chibi-0.8.2/tests/internet/api/four_chan/.client.py.swp
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:40.058904 chibi-0.8.2/tests/madness/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:15:07.000000 chibi-0.8.2/tests/madness/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      846 2018-12-12 21:15:07.000000 chibi-0.8.2/tests/madness/string.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:40.058904 chibi-0.8.2/tests/metaphors/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2019-12-21 21:22:48.000000 chibi-0.8.2/tests/metaphors/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3209 2020-02-21 21:24:25.000000 chibi-0.8.2/tests/metaphors/book.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      851 2019-04-05 17:54:01.000000 chibi-0.8.2/tests/module.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:40.058904 chibi-0.8.2/tests/net/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:15:06.000000 chibi-0.8.2/tests/net/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-10 20:48:29.000000 chibi-0.8.2/tests/net/download.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      191 2019-07-22 17:38:32.000000 chibi-0.8.2/tests/net/hostname.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2724 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/net/interface.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:40.058904 chibi-0.8.2/tests/nix/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:15:06.000000 chibi-0.8.2/tests/nix/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     4585 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/nix/nix.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:40.058904 chibi-0.8.2/tests/object/
--rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2019-02-14 22:32:09.000000 chibi-0.8.2/tests/object/__init__.py
--rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)      497 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/object/descriptors.py
--rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)     2668 2020-03-06 21:35:51.000000 chibi-0.8.2/tests/object/object.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:40.058904 chibi-0.8.2/tests/parser/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:15:07.000000 chibi-0.8.2/tests/parser/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      762 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/parser/bool.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:40.062238 chibi-0.8.2/tests/pipeline/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2019-04-25 15:50:15.000000 chibi-0.8.2/tests/pipeline/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      836 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/pipeline/pipeline.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      860 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/pipeline/xml.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:40.062238 chibi-0.8.2/tests/snippet/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:15:07.000000 chibi-0.8.2/tests/snippet/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     7355 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/snippet/dict.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1689 2020-02-22 02:50:47.000000 chibi-0.8.2/tests/snippet/files.py
--rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)      764 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/snippet/is_type.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      662 2019-04-26 23:52:58.000000 chibi-0.8.2/tests/snippet/iter.py
--rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)     1894 2019-02-25 17:46:51.000000 chibi-0.8.2/tests/snippet/regex.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1792 2020-03-30 21:15:30.000000 chibi-0.8.2/tests/snippet/string.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      283 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/snippet/table.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3644 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/snippet/xml.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-31 19:17:40.062238 chibi-0.8.2/tests/units/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:15:07.000000 chibi-0.8.2/tests/units/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2666 2018-12-12 21:15:07.000000 chibi-0.8.2/tests/units/base.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      241 2019-12-21 21:12:58.000000 chibi-0.8.2/tests/units/is.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.480967 chibi-0.9.0/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      150 2020-02-23 22:26:05.000000 chibi-0.9.0/AUTHORS.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3487 2020-02-23 22:28:08.000000 chibi-0.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      108 2020-02-24 01:48:21.000000 chibi-0.9.0/HISTORY.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      481 2019-12-21 21:12:58.000000 chibi-0.9.0/LICENSE
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      262 2020-02-23 22:30:23.000000 chibi-0.9.0/MANIFEST.in
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2429 2020-06-26 06:41:06.480967 chibi-0.9.0/PKG-INFO
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1263 2020-02-23 22:24:11.000000 chibi-0.9.0/README.rst
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.394300 chibi-0.9.0/chibi/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      106 2020-06-26 06:39:47.000000 chibi-0.9.0/chibi/__init__.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.394300 chibi-0.9.0/chibi/atlas/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3971 2020-04-20 16:35:05.000000 chibi-0.9.0/chibi/atlas/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      442 2020-04-27 20:35:46.000000 chibi-0.9.0/chibi/atlas/multi.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2656 2019-04-08 19:18:19.000000 chibi-0.9.0/chibi/atlas/tree.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      231 2018-12-12 21:14:52.000000 chibi-0.9.0/chibi/b64.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.394300 chibi-0.9.0/chibi/chain/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1054 2019-12-21 21:12:58.000000 chibi-0.9.0/chibi/chain/__init__.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.397633 chibi-0.9.0/chibi/config/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      270 2020-03-06 20:21:02.000000 chibi-0.9.0/chibi/config/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2417 2020-04-09 01:45:00.000000 chibi-0.9.0/chibi/config/config.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      284 2020-03-02 22:57:59.000000 chibi-0.9.0/chibi/config/logger.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.397633 chibi-0.9.0/chibi/fancy/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:14:51.000000 chibi-0.9.0/chibi/fancy/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      531 2018-12-12 21:14:51.000000 chibi-0.9.0/chibi/fancy/is_type.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.397633 chibi-0.9.0/chibi/file/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      101 2018-12-12 21:14:52.000000 chibi-0.9.0/chibi/file/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     4845 2020-03-13 14:51:40.000000 chibi-0.9.0/chibi/file/file.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1711 2019-09-24 18:14:12.000000 chibi-0.9.0/chibi/file/image.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.397633 chibi-0.9.0/chibi/file/other/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      577 2020-04-12 16:30:52.000000 chibi-0.9.0/chibi/file/other/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1676 2020-01-08 04:49:10.000000 chibi-0.9.0/chibi/file/other/chibi_csv.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      319 2019-12-24 06:32:24.000000 chibi-0.9.0/chibi/file/other/chibi_json.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      594 2020-04-09 01:37:32.000000 chibi-0.9.0/chibi/file/other/chibi_python.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1196 2020-04-27 20:41:50.000000 chibi-0.9.0/chibi/file/other/chibi_systemd.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      456 2019-12-24 06:31:10.000000 chibi-0.9.0/chibi/file/other/chibi_yaml.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)    10080 2020-04-27 20:22:57.000000 chibi-0.9.0/chibi/file/path.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)    10305 2020-04-08 20:41:14.000000 chibi-0.9.0/chibi/file/snippets.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      675 2019-12-21 21:12:58.000000 chibi-0.9.0/chibi/file/temp.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.400967 chibi-0.9.0/chibi/madness/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       46 2018-12-12 21:14:52.000000 chibi-0.9.0/chibi/madness/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:14:52.000000 chibi-0.9.0/chibi/madness/byte.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      371 2019-07-18 21:49:37.000000 chibi-0.9.0/chibi/madness/file.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2523 2019-02-26 12:01:40.000000 chibi-0.9.0/chibi/madness/string.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.400967 chibi-0.9.0/chibi/metaphors/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       46 2019-12-21 21:25:16.000000 chibi-0.9.0/chibi/metaphors/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1141 2020-02-21 21:24:25.000000 chibi-0.9.0/chibi/metaphors/book.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      502 2019-04-04 18:35:55.000000 chibi-0.9.0/chibi/module.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.400967 chibi-0.9.0/chibi/net/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-10 20:48:04.000000 chibi-0.9.0/chibi/net/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       68 2019-07-22 17:38:19.000000 chibi-0.9.0/chibi/net/hostname.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.400967 chibi-0.9.0/chibi/net/network/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:14:51.000000 chibi-0.9.0/chibi/net/network/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1145 2019-04-27 00:19:43.000000 chibi-0.9.0/chibi/net/network/interface.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.400967 chibi-0.9.0/chibi/net/network_manager/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2019-07-18 14:00:45.000000 chibi-0.9.0/chibi/net/network_manager/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2186 2019-07-22 17:05:16.000000 chibi-0.9.0/chibi/nix.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.400967 chibi-0.9.0/chibi/object/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       64 2019-02-14 22:27:50.000000 chibi-0.9.0/chibi/object/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     4883 2019-08-27 15:29:30.000000 chibi-0.9.0/chibi/object/descriptor.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2339 2019-02-26 12:10:40.000000 chibi-0.9.0/chibi/object/object.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1663 2018-12-12 21:14:52.000000 chibi-0.9.0/chibi/parser.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.400967 chibi-0.9.0/chibi/pipeline/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       58 2019-04-25 15:54:05.000000 chibi-0.9.0/chibi/pipeline/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1738 2019-06-10 21:29:23.000000 chibi-0.9.0/chibi/pipeline/pipeline.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      211 2019-06-10 21:37:52.000000 chibi-0.9.0/chibi/pipeline/xml.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.404300 chibi-0.9.0/chibi/snippet/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:14:52.000000 chibi-0.9.0/chibi/snippet/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     7353 2020-02-21 21:24:25.000000 chibi-0.9.0/chibi/snippet/dict.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)    29717 2019-02-26 12:11:42.000000 chibi-0.9.0/chibi/snippet/extra_string.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2019-07-18 15:16:51.000000 chibi-0.9.0/chibi/snippet/file.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      198 2019-06-10 20:01:16.000000 chibi-0.9.0/chibi/snippet/image.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      898 2019-02-26 12:10:06.000000 chibi-0.9.0/chibi/snippet/is_type.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1131 2020-04-12 16:23:43.000000 chibi-0.9.0/chibi/snippet/iter.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1187 2020-04-12 16:16:46.000000 chibi-0.9.0/chibi/snippet/regex.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2744 2020-04-12 16:16:28.000000 chibi-0.9.0/chibi/snippet/string.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      295 2019-07-22 17:07:01.000000 chibi-0.9.0/chibi/snippet/table.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1235 2019-07-23 21:13:00.000000 chibi-0.9.0/chibi/snippet/xml.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.404300 chibi-0.9.0/chibi/units/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:14:52.000000 chibi-0.9.0/chibi/units/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2712 2019-02-26 12:04:25.000000 chibi-0.9.0/chibi/units/base.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1574 2018-12-12 21:14:52.000000 chibi-0.9.0/chibi/units/prefix.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      647 2018-12-12 21:14:52.000000 chibi-0.9.0/chibi/units/si.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.394300 chibi-0.9.0/chibi.egg-info/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2429 2020-06-26 06:41:05.000000 chibi-0.9.0/chibi.egg-info/PKG-INFO
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     4415 2020-06-26 06:41:06.000000 chibi-0.9.0/chibi.egg-info/SOURCES.txt
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        1 2020-06-26 06:41:05.000000 chibi-0.9.0/chibi.egg-info/dependency_links.txt
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        1 2020-06-26 06:41:05.000000 chibi-0.9.0/chibi.egg-info/not-zip-safe
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      114 2020-06-26 06:41:05.000000 chibi-0.9.0/chibi.egg-info/requires.txt
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        6 2020-06-26 06:41:05.000000 chibi-0.9.0/chibi.egg-info/top_level.txt
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.450967 chibi-0.9.0/docs/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      606 2020-02-23 22:31:16.000000 chibi-0.9.0/docs/Makefile
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       28 2020-02-23 22:30:23.000000 chibi-0.9.0/docs/authors.rst
+-rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)     4768 2020-02-23 22:30:49.000000 chibi-0.9.0/docs/conf.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       33 2020-02-23 22:30:23.000000 chibi-0.9.0/docs/contributing.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       28 2020-02-23 22:30:23.000000 chibi-0.9.0/docs/history.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      302 2020-02-23 22:30:56.000000 chibi-0.9.0/docs/index.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1094 2020-02-23 22:31:02.000000 chibi-0.9.0/docs/installation.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      767 2020-02-23 22:31:07.000000 chibi-0.9.0/docs/make.bat
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       27 2020-02-23 22:30:23.000000 chibi-0.9.0/docs/readme.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       65 2020-02-23 22:31:28.000000 chibi-0.9.0/docs/usage.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      443 2020-06-26 06:41:06.480967 chibi-0.9.0/setup.cfg
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1081 2020-06-26 06:39:47.000000 chibi-0.9.0/setup.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.450967 chibi-0.9.0/tests/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:15:06.000000 chibi-0.9.0/tests/__init__.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.450967 chibi-0.9.0/tests/api/
+-rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)    12288 2018-12-12 21:15:07.000000 chibi-0.9.0/tests/api/.endpoint.py.swp
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.460967 chibi-0.9.0/tests/atlas/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:15:07.000000 chibi-0.9.0/tests/atlas/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3093 2019-12-21 21:12:58.000000 chibi-0.9.0/tests/atlas/chibi_atlas.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1581 2019-12-21 21:12:58.000000 chibi-0.9.0/tests/atlas/chibi_atlas_ignore_case.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     4762 2019-12-21 21:12:58.000000 chibi-0.9.0/tests/atlas/chibi_tree.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1024 2019-12-21 21:12:58.000000 chibi-0.9.0/tests/atlas/loads.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      540 2020-04-27 20:35:35.000000 chibi-0.9.0/tests/atlas/multi.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      359 2018-12-12 21:15:06.000000 chibi-0.9.0/tests/b64.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.464300 chibi-0.9.0/tests/chain/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2019-12-21 21:12:58.000000 chibi-0.9.0/tests/chain/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2472 2019-12-21 21:12:58.000000 chibi-0.9.0/tests/chain/chain.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.464300 chibi-0.9.0/tests/config/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-02 22:38:29.000000 chibi-0.9.0/tests/config/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2692 2020-03-08 00:21:55.000000 chibi-0.9.0/tests/config/config.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-03 02:30:48.000000 chibi-0.9.0/tests/config/logger.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.470967 chibi-0.9.0/tests/file/
+-rw-------   0 dem4ply   (1000) dem4ply   (1000)    58162 2018-12-12 21:15:06.000000 chibi-0.9.0/tests/file/1529990793499.jpg
+-rw-------   0 dem4ply   (1000) dem4ply   (1000)   207885 2018-12-12 21:15:06.000000 chibi-0.9.0/tests/file/1535359854403.png
+-rw-------   0 dem4ply   (1000) dem4ply   (1000)   563123 2018-12-12 21:15:06.000000 chibi-0.9.0/tests/file/1536637012160.gif
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:15:06.000000 chibi-0.9.0/tests/file/__init__.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.470967 chibi-0.9.0/tests/file/chibi_file/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:15:06.000000 chibi-0.9.0/tests/file/chibi_file/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2100 2019-06-11 21:29:13.000000 chibi-0.9.0/tests/file/chibi_file/append.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      394 2018-12-12 21:18:30.000000 chibi-0.9.0/tests/file/chibi_file/check_sum_md5.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      772 2019-12-21 23:55:31.000000 chibi-0.9.0/tests/file/chibi_file/class_resolution.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1157 2019-09-10 17:56:36.000000 chibi-0.9.0/tests/file/chibi_file/copy.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      845 2019-07-22 17:54:24.000000 chibi-0.9.0/tests/file/chibi_file/find.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1015 2019-12-24 06:37:02.000000 chibi-0.9.0/tests/file/chibi_file/json.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      603 2019-12-21 21:12:58.000000 chibi-0.9.0/tests/file/chibi_file/properites.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1496 2019-12-24 06:37:31.000000 chibi-0.9.0/tests/file/chibi_file/yaml.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2392 2020-03-10 20:44:17.000000 chibi-0.9.0/tests/file/image.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.474300 chibi-0.9.0/tests/file/orphan_function/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:15:07.000000 chibi-0.9.0/tests/file/orphan_function/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      533 2019-12-21 21:12:58.000000 chibi-0.9.0/tests/file/orphan_function/add_extensions.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1257 2020-02-22 02:54:29.000000 chibi-0.9.0/tests/file/orphan_function/cd.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      622 2020-03-02 16:05:47.000000 chibi-0.9.0/tests/file/orphan_function/chown.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      282 2019-05-04 02:01:25.000000 chibi-0.9.0/tests/file/orphan_function/common_root.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1475 2019-12-21 21:12:58.000000 chibi-0.9.0/tests/file/orphan_function/copy.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      637 2019-12-21 21:12:58.000000 chibi-0.9.0/tests/file/orphan_function/delete.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      570 2019-12-21 21:12:58.000000 chibi-0.9.0/tests/file/orphan_function/exists.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      531 2019-12-21 21:12:58.000000 chibi-0.9.0/tests/file/orphan_function/file_dir.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1591 2019-12-21 21:12:58.000000 chibi-0.9.0/tests/file/orphan_function/find.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      481 2019-12-21 21:12:58.000000 chibi-0.9.0/tests/file/orphan_function/get_relative_path.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      787 2020-02-22 02:52:02.000000 chibi-0.9.0/tests/file/orphan_function/infalte_dir.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      531 2019-12-21 21:12:58.000000 chibi-0.9.0/tests/file/orphan_function/is_dir.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      538 2018-12-12 21:15:06.000000 chibi-0.9.0/tests/file/orphan_function/is_file.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      813 2019-12-21 21:12:58.000000 chibi-0.9.0/tests/file/orphan_function/join.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      996 2019-12-21 21:12:58.000000 chibi-0.9.0/tests/file/orphan_function/ls.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1221 2020-04-27 20:22:09.000000 chibi-0.9.0/tests/file/orphan_function/ls_only_dir.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1479 2020-03-02 16:06:50.000000 chibi-0.9.0/tests/file/orphan_function/mkdir.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1699 2019-12-21 21:12:58.000000 chibi-0.9.0/tests/file/orphan_function/move.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1011 2018-12-12 21:15:07.000000 chibi-0.9.0/tests/file/orphan_function/stat.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.474300 chibi-0.9.0/tests/file/other/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2019-12-21 21:12:58.000000 chibi-0.9.0/tests/file/other/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2644 2020-01-09 03:57:44.000000 chibi-0.9.0/tests/file/other/chibi_csv.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1774 2020-04-27 20:41:03.000000 chibi-0.9.0/tests/file/other/chibi_systemd.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.474300 chibi-0.9.0/tests/file/path/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:15:07.000000 chibi-0.9.0/tests/file/path/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1158 2020-02-22 02:53:47.000000 chibi-0.9.0/tests/file/path/current_dir.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1872 2020-04-05 21:35:08.000000 chibi-0.9.0/tests/file/path/glob.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     9263 2020-04-27 20:23:21.000000 chibi-0.9.0/tests/file/path/path.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1037 2019-12-21 21:12:58.000000 chibi-0.9.0/tests/file/path/temp.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.474300 chibi-0.9.0/tests/internet/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:15:06.000000 chibi-0.9.0/tests/internet/__init__.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.474300 chibi-0.9.0/tests/internet/api/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:15:06.000000 chibi-0.9.0/tests/internet/api/__init__.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.477633 chibi-0.9.0/tests/internet/api/four_chan/
+-rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)    12288 2018-12-12 21:15:06.000000 chibi-0.9.0/tests/internet/api/four_chan/.client.py.swo
+-rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)    12288 2018-12-12 21:15:06.000000 chibi-0.9.0/tests/internet/api/four_chan/.client.py.swp
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.477633 chibi-0.9.0/tests/madness/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:15:07.000000 chibi-0.9.0/tests/madness/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      846 2018-12-12 21:15:07.000000 chibi-0.9.0/tests/madness/string.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.477633 chibi-0.9.0/tests/metaphors/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2019-12-21 21:22:48.000000 chibi-0.9.0/tests/metaphors/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3209 2020-02-21 21:24:25.000000 chibi-0.9.0/tests/metaphors/book.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      851 2019-04-05 17:54:01.000000 chibi-0.9.0/tests/module.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.477633 chibi-0.9.0/tests/net/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:15:06.000000 chibi-0.9.0/tests/net/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2020-03-10 20:48:29.000000 chibi-0.9.0/tests/net/download.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      191 2019-07-22 17:38:32.000000 chibi-0.9.0/tests/net/hostname.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2724 2019-12-21 21:12:58.000000 chibi-0.9.0/tests/net/interface.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.477633 chibi-0.9.0/tests/nix/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:15:06.000000 chibi-0.9.0/tests/nix/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     4996 2020-04-27 20:14:35.000000 chibi-0.9.0/tests/nix/nix.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.477633 chibi-0.9.0/tests/object/
+-rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2019-02-14 22:32:09.000000 chibi-0.9.0/tests/object/__init__.py
+-rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)      497 2019-12-21 21:12:58.000000 chibi-0.9.0/tests/object/descriptors.py
+-rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)     2668 2020-03-06 21:35:51.000000 chibi-0.9.0/tests/object/object.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.477633 chibi-0.9.0/tests/parser/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:15:07.000000 chibi-0.9.0/tests/parser/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      762 2019-12-21 21:12:58.000000 chibi-0.9.0/tests/parser/bool.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.480967 chibi-0.9.0/tests/pipeline/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2019-04-25 15:50:15.000000 chibi-0.9.0/tests/pipeline/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      836 2019-12-21 21:12:58.000000 chibi-0.9.0/tests/pipeline/pipeline.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      860 2019-12-21 21:12:58.000000 chibi-0.9.0/tests/pipeline/xml.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.480967 chibi-0.9.0/tests/snippet/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:15:07.000000 chibi-0.9.0/tests/snippet/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     7355 2019-12-21 21:12:58.000000 chibi-0.9.0/tests/snippet/dict.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1689 2020-02-22 02:50:47.000000 chibi-0.9.0/tests/snippet/files.py
+-rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)      764 2019-12-21 21:12:58.000000 chibi-0.9.0/tests/snippet/is_type.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      662 2020-04-12 16:24:00.000000 chibi-0.9.0/tests/snippet/iter.py
+-rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)     1894 2019-02-25 17:46:51.000000 chibi-0.9.0/tests/snippet/regex.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1792 2020-03-30 21:15:30.000000 chibi-0.9.0/tests/snippet/string.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      283 2019-12-21 21:12:58.000000 chibi-0.9.0/tests/snippet/table.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3644 2019-12-21 21:12:58.000000 chibi-0.9.0/tests/snippet/xml.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2020-06-26 06:41:06.480967 chibi-0.9.0/tests/units/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2018-12-12 21:15:07.000000 chibi-0.9.0/tests/units/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2666 2018-12-12 21:15:07.000000 chibi-0.9.0/tests/units/base.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      241 2019-12-21 21:12:58.000000 chibi-0.9.0/tests/units/is.py
```

### Comparing `chibi-0.8.2/CONTRIBUTING.rst` & `chibi-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/PKG-INFO` & `chibi-0.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: chibi
-Version: 0.8.2
+Version: 0.9.0
 Summary: UNKNOWN
 Home-page: https://github.com/dem4ply/chibi
 Author: dem4ply
 Author-email: UNKNOWN
 License: WTFPL
 Description: =====
         chibi
```

### Comparing `chibi-0.8.2/README.rst` & `chibi-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/chibi/atlas/__init__.py` & `chibi-0.9.0/chibi/atlas/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -92,28 +92,40 @@
         return super().__setattr__( name, value )
 
     def __setitem__( self, key, value ):
         key = key.lower()
         return super().__setitem__( key, value )
 
 
+def _default_factory():
+    return Chibi_atlas_default()
+
+
 class Chibi_atlas_default( defaultdict, Chibi_atlas ):
     """
     chibi atlas que emula `py:class:collections.defaultdict`
     """
-    pass
+    def __init__( self, default_factory=None, *args, **kw ):
+        if default_factory is None:
+            default_factory = _default_factory
+        super().__init__( default_factory, *args, **kw )
 
 
 class __Chibi_atlas_list( list ):
     def __getitem__( self, index ):
         value = super().__getitem__( index, )
-        return _wrap( value )
+        value = _wrap( value )
+        self[ index ] = value
+        return value
 
     def __iter__( self ):
-        return map( _wrap, super().__iter__() )
+        for i, v in enumerate( super().__iter__() ):
+            value = _wrap( v )
+            self[ i ] = value
+            yield value
 
 
 def _wrap( val, klass=None ):
     if type( val ) == dict:
         if klass is None:
             return Chibi_atlas( val )
         else:
```

### Comparing `chibi-0.8.2/chibi/atlas/tree.py` & `chibi-0.9.0/chibi/atlas/tree.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/chibi/chain/__init__.py` & `chibi-0.9.0/chibi/chain/__init__.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/chibi/config/config.py` & `chibi-0.9.0/chibi/config/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,23 @@
+import sys
 import logging
 from chibi.atlas import Chibi_atlas, Chibi_atlas_default
 from chibi.file import Chibi_path
 from chibi.file.other import Chibi_json, Chibi_yaml, Chibi_python
 
 
 logger = logging.getLogger( 'chibi.config.Configuration' )
 
 
 __all__ = [ 'Configuration' ]
 
 
+sys.path.append( './' )
+
+
 def _default_factory():
     return Configuration()
 
 
 class Configuration( Chibi_atlas_default ):
     def __init__( self, default_factory=None, *args, **kw ):
         if default_factory is None:
@@ -23,18 +27,16 @@
     def load( self, path ):
         path = Chibi_path( path )
         with path as f:
             if isinstance( f, ( Chibi_json, Chibi_yaml ) ):
                 for k, v in f.read().items():
                     self[ k ] = v
             elif isinstance( f, Chibi_python ):
-                value = f.read()
                 logger.info( f"ejecutanto archivo python {f}" )
-                logger.debug( value )
-                exec( value )
+                module = f.import_()
             else:
                 raise NotImplementedError(
                     "no esta implementado la carga de configuracion de los "
                     f"archivos {type(f)} de {f}" )
 
 
 class Logger_configuration( Chibi_atlas ):
```

### Comparing `chibi-0.8.2/chibi/fancy/is_type.py` & `chibi-0.9.0/chibi/fancy/is_type.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/chibi/file/file.py` & `chibi-0.9.0/chibi/file/file.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/chibi/file/image.py` & `chibi-0.9.0/chibi/file/image.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/chibi/file/other/chibi_csv.py` & `chibi-0.9.0/chibi/file/other/chibi_csv.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/chibi/file/path.py` & `chibi-0.9.0/chibi/file/path.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,21 +8,23 @@
 import magic
 
 
 logger = logging.getLogger( "chibi.file.chibi_path" )
 
 
 class Chibi_path( str ):
-    def __new__( cls, *args, **kw ):
+    def __new__( cls, *args, chibi_file_class=None, **kw ):
         args_2 = []
         for a in args:
             if '~' in a:
                 a = os.path.expanduser( a )
             args_2.append( a )
-        return str.__new__( cls, *args_2, **kw )
+        result = str.__new__( cls, *args_2, **kw )
+        result._chibi_file_class = chibi_file_class
+        return result
 
     def __add__( self, other ):
         """
         une el path con otro path o una cadena
 
         Parameters
         ==========
@@ -57,16 +59,15 @@
             return super().__contains__( other )
 
     @property
     def is_a_folder( self ):
         """
         es una carpeta
         """
-        from chibi.file.snippets import is_a_folder
-        return is_a_folder( self )
+        return os.path.isdir( self )
 
     @property
     def is_a_file( self ):
         """
         es un archivo
         """
         from chibi.file.snippets import is_a_file
@@ -78,14 +79,15 @@
 
     @property
     def dir_name( self ):
         """
         regresa la carpeta padre
         """
         from chibi.file.snippets import file_dir
+        return type( self )( os.path.dirname( str( self ) ) )
         return self.__class__( file_dir( self ) )
 
     @property
     def base_name( self ):
         """
         regresa el nombre del archivo o de la carpeta
         """
@@ -95,22 +97,27 @@
     def file_name( self ):
         """
         regresa el nombre del archivo sin la extencion
         """
         file_name, ext = os.path.splitext( self.base_name )
         return file_name
 
-    def open( self ):
+    def open( self, chibi_file_class=None ):
         """
         abre el archivo usando un chibi file
         """
         if self.is_a_folder:
             raise NotImplementedError
-        from . import Chibi_file
-        return Chibi_file( self )
+        if chibi_file_class is None:
+            if self._chibi_file_class is None:
+                from .file import Chibi_file
+                chibi_file_class = Chibi_file
+            else:
+                chibi_file_class = self._chibi_file_class
+        return chibi_file_class( self )
 
     def relative_to( self, root ):
         from .snippets import get_relative_path
         return type( self )( get_relative_path( self, root=root ) )
 
     def mkdir( self, **kw ):
         """
@@ -125,19 +132,33 @@
             logger.warning(
                 "mkdir de chibi path recibio parametros {}".format( kw ) )
 
     def move( self, dest ):
         """
         move the chibi path al destino
         """
+        dest = Chibi_path( dest )
         if self.is_a_file:
             if dest.is_a_folder:
                 dest += self.base_name
-        shutil.move( str( self ), str( dest ) )
-        logger.info( "{} -> {}".format( self, dest ) )
+            shutil.move( str( self ), str( dest ) )
+            logger.info( "{} -> {}".format( self, dest ) )
+        elif self.is_a_folder:
+            shutil.move( str( self ), str( dest ) )
+            logger.info( "{} -> {}".format( self, dest ) )
+        elif self.is_glob:
+            if not dest.exists:
+                dest.mkdir()
+            if dest.is_a_folder:
+                return [
+                    f.move( dest + f.base_name ) for f in self.expand ]
+            else:
+                raise NotImplementedError(
+                    "el destino no es un folder y la src "
+                    "es un glob '{self}'" )
 
     def copy( self, dest, **kw ):
         """
         copia el archivo o carpeta al destino
         """
         from.snippets import copy
         dest = Chibi_path( dest )
@@ -309,7 +330,14 @@
         elif self.is_a_folder:
             raise NotADirectoryError(
                 f"no implementado touch a un folder '{self}'" )
         else:
             raise NotADirectoryError(
                 f"no implementado touch cuando no es un "
                 f"archivo o folder'{self}'" )
+
+    @property
+    def inflate( self ):
+        if '~' in self:
+            return os.path.expanduser( self )
+        else:
+            return os.path.abspath( self )
```

### Comparing `chibi-0.8.2/chibi/file/snippets.py` & `chibi-0.9.0/chibi/file/snippets.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/chibi/file/temp.py` & `chibi-0.9.0/chibi/file/temp.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/chibi/madness/string.py` & `chibi-0.9.0/chibi/madness/string.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/chibi/metaphors/book.py` & `chibi-0.9.0/chibi/metaphors/book.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/chibi/net/network/interface.py` & `chibi-0.9.0/chibi/net/network/interface.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/chibi/nix.py` & `chibi-0.9.0/chibi/nix.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/chibi/object/descriptor.py` & `chibi-0.9.0/chibi/object/descriptor.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/chibi/object/object.py` & `chibi-0.9.0/chibi/object/object.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/chibi/parser.py` & `chibi-0.9.0/chibi/parser.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/chibi/pipeline/pipeline.py` & `chibi-0.9.0/chibi/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/chibi/snippet/dict.py` & `chibi-0.9.0/chibi/snippet/dict.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/chibi/snippet/extra_string.py` & `chibi-0.9.0/chibi/snippet/extra_string.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/chibi/snippet/is_type.py` & `chibi-0.9.0/chibi/snippet/is_type.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/chibi/snippet/iter.py` & `chibi-0.9.0/chibi/snippet/iter.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/chibi/snippet/regex.py` & `chibi-0.9.0/chibi/snippet/regex.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/chibi/snippet/string.py` & `chibi-0.9.0/chibi/snippet/string.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/chibi/snippet/xml.py` & `chibi-0.9.0/chibi/snippet/xml.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/chibi/units/base.py` & `chibi-0.9.0/chibi/units/base.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/chibi/units/prefix.py` & `chibi-0.9.0/chibi/units/prefix.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/chibi/units/si.py` & `chibi-0.9.0/chibi/units/si.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/chibi.egg-info/PKG-INFO` & `chibi-0.9.0/chibi.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: chibi
-Version: 0.8.2
+Version: 0.9.0
 Summary: UNKNOWN
 Home-page: https://github.com/dem4ply/chibi
 Author: dem4ply
 Author-email: UNKNOWN
 License: WTFPL
 Description: =====
         chibi
```

### Comparing `chibi-0.8.2/chibi.egg-info/SOURCES.txt` & `chibi-0.9.0/chibi.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -14,41 +14,17 @@
 chibi.egg-info/PKG-INFO
 chibi.egg-info/SOURCES.txt
 chibi.egg-info/dependency_links.txt
 chibi.egg-info/not-zip-safe
 chibi.egg-info/requires.txt
 chibi.egg-info/top_level.txt
 chibi/atlas/__init__.py
+chibi/atlas/multi.py
 chibi/atlas/tree.py
 chibi/chain/__init__.py
-chibi/command/__init__.py
-chibi/command/dd.py
-chibi/command/network.py
-chibi/command/nmap.py
-chibi/command/nmcli.py
-chibi/command/qr.py
-chibi/command/disk/__init__.py
-chibi/command/disk/dd.py
-chibi/command/disk/format.py
-chibi/command/disk/mount.py
-chibi/command/echo/__init__.py
-chibi/command/echo/cowsay.py
-chibi/command/echo/echo.py
-chibi/command/echo/ponysay.py
-chibi/command/file/__init__.py
-chibi/command/file/tar.py
-chibi/command/firewall/__init__.py
-chibi/command/git/__init__.py
-chibi/command/mpd/__init__.py
-chibi/command/mpd/mpc.py
-chibi/command/pip/__init__.py
-chibi/command/rabbitmq/__init__.py
-chibi/command/rpm/__init__.py
-chibi/command/systemctl/__init__.py
-chibi/command/yum/__init__.py
 chibi/config/__init__.py
 chibi/config/config.py
 chibi/config/logger.py
 chibi/fancy/__init__.py
 chibi/fancy/is_type.py
 chibi/file/__init__.py
 chibi/file/file.py
@@ -56,14 +32,15 @@
 chibi/file/path.py
 chibi/file/snippets.py
 chibi/file/temp.py
 chibi/file/other/__init__.py
 chibi/file/other/chibi_csv.py
 chibi/file/other/chibi_json.py
 chibi/file/other/chibi_python.py
+chibi/file/other/chibi_systemd.py
 chibi/file/other/chibi_yaml.py
 chibi/madness/__init__.py
 chibi/madness/byte.py
 chibi/madness/file.py
 chibi/madness/string.py
 chibi/metaphors/__init__.py
 chibi/metaphors/book.py
@@ -108,28 +85,17 @@
 tests/module.py
 tests/api/.endpoint.py.swp
 tests/atlas/__init__.py
 tests/atlas/chibi_atlas.py
 tests/atlas/chibi_atlas_ignore_case.py
 tests/atlas/chibi_tree.py
 tests/atlas/loads.py
+tests/atlas/multi.py
 tests/chain/__init__.py
 tests/chain/chain.py
-tests/command/__init__.py
-tests/command/command.py
-tests/command/network.py
-tests/command/echo/__init__.py
-tests/command/echo/cowsay.py
-tests/command/echo/echo.py
-tests/command/echo/ponysay.py
-tests/command/yum/__init__.py
-tests/command/yum/install.py
-tests/command/yum/localinstall.py
-tests/command/yum/update.py
-tests/command/yum/yum.py
 tests/config/__init__.py
 tests/config/config.py
 tests/config/logger.py
 tests/file/1529990793499.jpg
 tests/file/1535359854403.png
 tests/file/1536637012160.gif
 tests/file/__init__.py
@@ -161,14 +127,15 @@
 tests/file/orphan_function/ls.py
 tests/file/orphan_function/ls_only_dir.py
 tests/file/orphan_function/mkdir.py
 tests/file/orphan_function/move.py
 tests/file/orphan_function/stat.py
 tests/file/other/__init__.py
 tests/file/other/chibi_csv.py
+tests/file/other/chibi_systemd.py
 tests/file/path/__init__.py
 tests/file/path/current_dir.py
 tests/file/path/glob.py
 tests/file/path/path.py
 tests/file/path/temp.py
 tests/internet/__init__.py
 tests/internet/api/__init__.py
```

### Comparing `chibi-0.8.2/docs/Makefile` & `chibi-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/docs/conf.py` & `chibi-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/docs/installation.rst` & `chibi-0.9.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/docs/make.bat` & `chibi-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/setup.py` & `chibi-0.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
 requirements = [
-    'GitPython>=2.1.5', 'requests>=2.19.1', 'pika>=0.12.0',
+    'requests>=2.19.1', 'pika>=0.12.0',
     'python-magic>=0.4.15', 'Pillow>=5.3.0', 'dateutils>=0.6.6',
     'xmltodict>=0.12.0', 'pyyaml>=5.1.2' ]
 
 setup(
     name='chibi',
     keywords='chibi',
-    version='0.8.2',
+    version='0.9.0',
     description='',
     long_description=readme + '\n\n' + history,
     license="WTFPL",
     author='dem4ply',
     author_email='',
     packages=find_packages(include=['chibi', 'chibi.*']),
     install_requires=requirements,
```

### Comparing `chibi-0.8.2/tests/api/.endpoint.py.swp` & `chibi-0.9.0/tests/api/.endpoint.py.swp`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/atlas/chibi_atlas.py` & `chibi-0.9.0/tests/atlas/chibi_atlas.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/atlas/chibi_atlas_ignore_case.py` & `chibi-0.9.0/tests/atlas/chibi_atlas_ignore_case.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/atlas/chibi_tree.py` & `chibi-0.9.0/tests/atlas/chibi_tree.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/atlas/loads.py` & `chibi-0.9.0/tests/atlas/loads.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/chain/chain.py` & `chibi-0.9.0/tests/chain/chain.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/config/config.py` & `chibi-0.9.0/tests/config/config.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/file/1529990793499.jpg` & `chibi-0.9.0/tests/file/1529990793499.jpg`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/file/1535359854403.png` & `chibi-0.9.0/tests/file/1535359854403.png`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/file/1536637012160.gif` & `chibi-0.9.0/tests/file/1536637012160.gif`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/file/chibi_file/append.py` & `chibi-0.9.0/tests/file/chibi_file/append.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/file/chibi_file/class_resolution.py` & `chibi-0.9.0/tests/file/chibi_file/class_resolution.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/file/chibi_file/copy.py` & `chibi-0.9.0/tests/file/chibi_file/copy.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/file/chibi_file/find.py` & `chibi-0.9.0/tests/file/chibi_file/find.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/file/chibi_file/json.py` & `chibi-0.9.0/tests/file/chibi_file/json.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/file/chibi_file/properites.py` & `chibi-0.9.0/tests/file/chibi_file/properites.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/file/chibi_file/yaml.py` & `chibi-0.9.0/tests/file/chibi_file/yaml.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/file/image.py` & `chibi-0.9.0/tests/file/image.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/file/orphan_function/add_extensions.py` & `chibi-0.9.0/tests/file/orphan_function/add_extensions.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/file/orphan_function/cd.py` & `chibi-0.9.0/tests/file/orphan_function/cd.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/file/orphan_function/chown.py` & `chibi-0.9.0/tests/file/orphan_function/chown.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/file/orphan_function/copy.py` & `chibi-0.9.0/tests/file/orphan_function/copy.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/file/orphan_function/delete.py` & `chibi-0.9.0/tests/file/orphan_function/delete.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/file/orphan_function/exists.py` & `chibi-0.9.0/tests/file/orphan_function/exists.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/file/orphan_function/file_dir.py` & `chibi-0.9.0/tests/file/orphan_function/file_dir.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/file/orphan_function/find.py` & `chibi-0.9.0/tests/file/orphan_function/find.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/file/orphan_function/infalte_dir.py` & `chibi-0.9.0/tests/file/orphan_function/infalte_dir.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/file/orphan_function/is_dir.py` & `chibi-0.9.0/tests/file/orphan_function/is_dir.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/file/orphan_function/is_file.py` & `chibi-0.9.0/tests/file/orphan_function/is_file.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/file/orphan_function/join.py` & `chibi-0.9.0/tests/file/orphan_function/join.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/file/orphan_function/ls.py` & `chibi-0.9.0/tests/file/orphan_function/ls.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/file/orphan_function/ls_only_dir.py` & `chibi-0.9.0/tests/file/orphan_function/ls_only_dir.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/file/orphan_function/mkdir.py` & `chibi-0.9.0/tests/file/orphan_function/mkdir.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/file/orphan_function/move.py` & `chibi-0.9.0/tests/file/orphan_function/move.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/file/orphan_function/stat.py` & `chibi-0.9.0/tests/file/orphan_function/stat.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/file/other/chibi_csv.py` & `chibi-0.9.0/tests/file/other/chibi_csv.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/file/path/current_dir.py` & `chibi-0.9.0/tests/file/path/current_dir.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/file/path/glob.py` & `chibi-0.9.0/tests/file/path/glob.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,7 +37,17 @@
         dest = Chibi_path( self.root_dir ) + 'hola'
         self.assertFalse( exists( dest ) )
         source = Chibi_path( self.folder_with_files_with_content ) + '*'
         source.copy( dest )
         self.assertEqual(
             set( f.base_name for f in source.ls() ),
             set( f.base_name for f in dest.ls() ) )
+
+    def test_move( self ):
+        dest = Chibi_path( self.root_dir ) + 'hola'
+        self.assertFalse( exists( dest ) )
+        source = Chibi_path( self.folder_with_files_with_content ) + '*'
+        files = set( f.base_name for f in source.ls() )
+        source.move( dest )
+        self.assertEqual(
+            files, set( f.base_name for f in dest.ls() ) )
+        self.assertFalse( set( f.base_name for f in source.ls() ) )
```

### Comparing `chibi-0.8.2/tests/file/path/path.py` & `chibi-0.9.0/tests/file/path/path.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 
 from chibi.file import Chibi_file
 from chibi.file.path import Chibi_path
 from chibi.file.snippets import exists, ls, file_dir
 from tests.snippet.files import Test_with_files
 
 
+class Dump_chibi_file( Chibi_file ):
+    pass
+
+
 faker = Faker_factory.create()
 
 
 class Test_path( Test_with_files ):
     def setUp( self ):
         super().setUp()
         self.path = Chibi_path( self.root_dir )
@@ -243,7 +247,22 @@
         self.assertEqual( 'asdfasdf', path )
         path = Chibi_path( 'asdf|asdf' ).made_safe()
         self.assertEqual( 'asdfasdf', path )
         path = Chibi_path( 'asdf?asdf' ).made_safe()
         self.assertEqual( 'asdfasdf', path )
         path = Chibi_path( 'asdf?*<>asdf' ).made_safe()
         self.assertEqual( 'asdfasdf', path )
+
+
+class Test_path_open( Test_with_files ):
+    def test_when_open_a_file_should_retunr_a_chibi_file( self ):
+        f = self.files[0]
+        self.assertIsInstance( f.open(), Chibi_file )
+
+    def test_when_pass_the_class_should_return_the_expected_class( self ):
+        f = self.files[0]
+        self.assertIsInstance(
+            f.open( chibi_file_class=Dump_chibi_file ), Dump_chibi_file )
+
+    def test_the_chibi_path_can_carrie_the_chibi_file_whant_to_be_used( self ):
+        f = Chibi_path( self.files[0], chibi_file_class=Dump_chibi_file )
+        self.assertIsInstance( f.open(), Dump_chibi_file )
```

### Comparing `chibi-0.8.2/tests/file/path/temp.py` & `chibi-0.9.0/tests/file/path/temp.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/internet/api/four_chan/.client.py.swo` & `chibi-0.9.0/tests/internet/api/four_chan/.client.py.swo`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/internet/api/four_chan/.client.py.swp` & `chibi-0.9.0/tests/internet/api/four_chan/.client.py.swp`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/madness/string.py` & `chibi-0.9.0/tests/madness/string.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/metaphors/book.py` & `chibi-0.9.0/tests/metaphors/book.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/module.py` & `chibi-0.9.0/tests/module.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/net/interface.py` & `chibi-0.9.0/tests/net/interface.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/nix/nix.py` & `chibi-0.9.0/tests/nix/nix.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,49 +6,54 @@
     _parse_passwd, _parse_group, get_passwd, get_group,
     user_exists, group_exists, mem_info
 )
 
 
 class Test_passwd( TestCase ):
     def setUp( self ):
-        self.all_passwd = pwd.getpwall()
+        self.all_passwd = filter(
+            lambda x: x.pw_name != "nobody", pwd.getpwall() )
 
     def test_parse_passwd_should_have_the_same_data_as_the_raw( self ):
         for raw_passwd in self.all_passwd:
-            passwd = _parse_passwd( raw_passwd )
+            with self.subTest( f"parsing {raw_passwd}" ):
+                passwd = _parse_passwd( raw_passwd )
 
-            self.assertEqual( passwd.name, raw_passwd.pw_name )
-            self.assertEqual( passwd.passwd, raw_passwd.pw_passwd )
-            self.assertEqual( passwd.uid, raw_passwd.pw_uid )
-            self.assertEqual( passwd.gid, raw_passwd.pw_gid )
-            self.assertEqual( passwd.gecos, raw_passwd.pw_gecos )
-            self.assertEqual( passwd.dir, raw_passwd.pw_dir )
-            self.assertEqual( passwd.shell, raw_passwd.pw_shell )
+                self.assertEqual( passwd.name, raw_passwd.pw_name )
+                self.assertEqual( passwd.passwd, raw_passwd.pw_passwd )
+                self.assertEqual( passwd.uid, raw_passwd.pw_uid )
+                self.assertEqual( passwd.gid, raw_passwd.pw_gid )
+                self.assertEqual( passwd.gecos, raw_passwd.pw_gecos )
+                self.assertEqual( passwd.dir, raw_passwd.pw_dir )
+                self.assertEqual( passwd.shell, raw_passwd.pw_shell )
 
     def test_get_passwd_should_raise_a_exeption_if_no_args_are_send( self ):
         with self.assertRaises( ValueError ):
             get_passwd()
 
     def test_get_passwd_by_uid_should_parse_the_passwd( self ):
         for raw_passwd in self.all_passwd:
-            parse_passwd = _parse_passwd( raw_passwd )
-            passwd = get_passwd( uid=raw_passwd.pw_uid )
-            self.assertEqual( passwd, parse_passwd )
+            with self.subTest( f"parsing {raw_passwd}" ):
+                parse_passwd = _parse_passwd( raw_passwd )
+                passwd = get_passwd( uid=raw_passwd.pw_uid )
+                self.assertEqual( passwd.keys(), parse_passwd.keys() )
 
     def test_get_passwd_by_name_should_parse_the_passwd( self ):
         for raw_passwd in self.all_passwd:
-            parse_passwd = _parse_passwd( raw_passwd )
-            passwd = get_passwd( name=raw_passwd.pw_name )
-            self.assertEqual( passwd, parse_passwd )
+            with self.subTest( f"parsing {raw_passwd}" ):
+                parse_passwd = _parse_passwd( raw_passwd )
+                passwd = get_passwd( name=raw_passwd.pw_name )
+                self.assertEqual( passwd.keys(), parse_passwd.keys() )
 
     def test_get_passwd_by_name_and_uid_should_be_the_same( self ):
         for raw_passwd in self.all_passwd:
-            name_passwd = get_passwd( name=raw_passwd.pw_name )
-            uid_passwd = get_passwd( uid=raw_passwd.pw_uid )
-            self.assertEqual( name_passwd, uid_passwd )
+            with self.subTest( f"parsing {raw_passwd}" ):
+                name_passwd = get_passwd( name=raw_passwd.pw_name )
+                uid_passwd = get_passwd( uid=raw_passwd.pw_uid )
+                self.assertEqual( name_passwd, uid_passwd )
 
 
 class Test_group( TestCase ):
     def setUp( self ):
         self.all_group = grp.getgrall()
 
     def test_parse_group_should_have_the_same_data_as_the_raw( self ):
@@ -64,21 +69,21 @@
         with self.assertRaises( ValueError ):
             get_group()
 
     def test_get_group_by_gid_should_parse_the_group( self ):
         for raw_group in self.all_group:
             parse_passwd = _parse_group( raw_group )
             group = get_group( gid=raw_group.gr_gid )
-            self.assertEqual( group, parse_passwd )
+            self.assertEqual( group.keys(), parse_passwd.keys() )
 
     def test_get_group_by_name_should_parse_the_group( self ):
         for raw_group in self.all_group:
             parse_passwd = _parse_group( raw_group )
             group = get_group( name=raw_group.gr_name )
-            self.assertEqual( group, parse_passwd )
+            self.assertEqual( group.keys(), parse_passwd.keys() )
 
     def test_get_group_by_name_and_gid_should_be_the_same( self ):
         for raw_group in self.all_group:
             name_passwd = get_group( name=raw_group.gr_name )
             gid_passwd = get_group( gid=raw_group.gr_gid )
             self.assertEqual( name_passwd, gid_passwd )
```

### Comparing `chibi-0.8.2/tests/object/object.py` & `chibi-0.9.0/tests/object/object.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/parser/bool.py` & `chibi-0.9.0/tests/parser/bool.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/pipeline/pipeline.py` & `chibi-0.9.0/tests/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/pipeline/xml.py` & `chibi-0.9.0/tests/pipeline/xml.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/snippet/dict.py` & `chibi-0.9.0/tests/snippet/dict.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/snippet/files.py` & `chibi-0.9.0/tests/snippet/files.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/snippet/is_type.py` & `chibi-0.9.0/tests/snippet/is_type.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/snippet/iter.py` & `chibi-0.9.0/tests/snippet/iter.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/snippet/regex.py` & `chibi-0.9.0/tests/snippet/regex.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/snippet/string.py` & `chibi-0.9.0/tests/snippet/string.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/snippet/xml.py` & `chibi-0.9.0/tests/snippet/xml.py`

 * *Files identical despite different names*

### Comparing `chibi-0.8.2/tests/units/base.py` & `chibi-0.9.0/tests/units/base.py`

 * *Files identical despite different names*

