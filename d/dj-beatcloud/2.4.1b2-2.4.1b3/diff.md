# Comparing `tmp/dj_beatcloud-2.4.1b2.tar.gz` & `tmp/dj_beatcloud-2.4.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_beatcloud-2.4.1b2.tar", last modified: Sat Mar 18 00:23:35 2023, max compression
+gzip compressed data, was "dj_beatcloud-2.4.1b3.tar", last modified: Wed Apr 12 23:26:05 2023, max compression
```

## Comparing `dj_beatcloud-2.4.1b2.tar` & `dj_beatcloud-2.4.1b3.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-03-18 00:23:35.539414 dj_beatcloud-2.4.1b2/
--rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.4.1b2/LICENSE
--rw-r--r--   0 alrichards   (502) staff       (20)       64 2022-06-16 01:40:44.000000 dj_beatcloud-2.4.1b2/MANIFEST.in
--rw-r--r--   0 alrichards   (502) staff       (20)    29508 2023-03-18 00:23:35.539553 dj_beatcloud-2.4.1b2/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)    28223 2023-03-18 00:19:54.000000 dj_beatcloud-2.4.1b2/README.md
--rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-03-18 00:19:54.000000 dj_beatcloud-2.4.1b2/pyproject.toml
--rw-r--r--   0 alrichards   (502) staff       (20)      164 2023-03-18 00:23:35.540503 dj_beatcloud-2.4.1b2/setup.cfg
--rw-r--r--   0 alrichards   (502) staff       (20)     2225 2023-03-18 00:19:57.000000 dj_beatcloud-2.4.1b2/setup.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-03-18 00:23:35.516889 dj_beatcloud-2.4.1b2/src/
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-03-18 00:23:35.520144 dj_beatcloud-2.4.1b2/src/dj_beatcloud.egg-info/
--rw-r--r--   0 alrichards   (502) staff       (20)    29508 2023-03-18 00:23:35.000000 dj_beatcloud-2.4.1b2/src/dj_beatcloud.egg-info/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     2193 2023-03-18 00:23:35.000000 dj_beatcloud-2.4.1b2/src/dj_beatcloud.egg-info/SOURCES.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-03-18 00:23:35.000000 dj_beatcloud-2.4.1b2/src/dj_beatcloud.egg-info/dependency_links.txt
--rw-r--r--   0 alrichards   (502) staff       (20)       50 2023-03-18 00:23:35.000000 dj_beatcloud-2.4.1b2/src/dj_beatcloud.egg-info/entry_points.txt
--rw-r--r--   0 alrichards   (502) staff       (20)      332 2023-03-18 00:23:35.000000 dj_beatcloud-2.4.1b2/src/dj_beatcloud.egg-info/requires.txt
--rw-r--r--   0 alrichards   (502) staff       (20)       18 2023-03-18 00:23:35.000000 dj_beatcloud-2.4.1b2/src/dj_beatcloud.egg-info/top_level.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-03-18 00:23:35.521443 dj_beatcloud-2.4.1b2/src/djtools/
--rw-r--r--   0 alrichards   (502) staff       (20)      966 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b2/src/djtools/__init__.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-03-18 00:23:35.525790 dj_beatcloud-2.4.1b2/src/djtools/configs/
--rw-r--r--   0 alrichards   (502) staff       (20)     6148 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b2/src/djtools/configs/.DS_Store
--rw-r--r--   0 alrichards   (502) staff       (20)     4258 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b2/src/djtools/configs/README.md
--rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b2/src/djtools/configs/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3081 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b2/src/djtools/configs/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1223 2023-03-09 22:09:23.000000 dj_beatcloud-2.4.1b2/src/djtools/configs/config.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)    13162 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b2/src/djtools/configs/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b2/src/djtools/configs/logging.conf
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-03-15 20:01:35.000000 dj_beatcloud-2.4.1b2/src/djtools/configs/registered_users.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)     1053 2023-03-18 00:19:57.000000 dj_beatcloud-2.4.1b2/src/djtools/configs/rekordbox_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-03-09 22:09:23.000000 dj_beatcloud-2.4.1b2/src/djtools/configs/spotify_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)     2303 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b2/src/djtools/configs/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4217 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b2/src/djtools/configs/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1721 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b2/src/djtools/dj_tools.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-03-18 00:23:35.526203 dj_beatcloud-2.4.1b2/src/djtools/logs/
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2022-06-16 01:40:44.000000 dj_beatcloud-2.4.1b2/src/djtools/logs/empty.txt
--rw-r--r--   0 alrichards   (502) staff       (20)     1649 2023-03-16 00:56:47.000000 dj_beatcloud-2.4.1b2/src/djtools/main.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-03-18 00:23:35.530393 dj_beatcloud-2.4.1b2/src/djtools/rekordbox/
--rw-r--r--   0 alrichards   (502) staff       (20)     1360 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b2/src/djtools/rekordbox/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1852 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b2/src/djtools/rekordbox/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4280 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b2/src/djtools/rekordbox/copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4549 2023-03-18 00:19:54.000000 dj_beatcloud-2.4.1b2/src/djtools/rekordbox/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)    18973 2023-03-18 00:19:54.000000 dj_beatcloud-2.4.1b2/src/djtools/rekordbox/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2875 2023-03-18 00:19:54.000000 dj_beatcloud-2.4.1b2/src/djtools/rekordbox/randomize_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)    13303 2023-03-18 00:19:54.000000 dj_beatcloud-2.4.1b2/src/djtools/rekordbox/tag_parsers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1185 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b2/src/djtools/rekordbox/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1419 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b2/src/djtools/rekordbox/test_copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2890 2023-03-18 00:19:57.000000 dj_beatcloud-2.4.1b2/src/djtools/rekordbox/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5190 2023-03-18 00:19:54.000000 dj_beatcloud-2.4.1b2/src/djtools/rekordbox/test_playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1518 2023-03-18 00:19:57.000000 dj_beatcloud-2.4.1b2/src/djtools/rekordbox/test_randomize_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3978 2023-03-18 00:21:55.000000 dj_beatcloud-2.4.1b2/src/djtools/rekordbox/test_tag_parsers.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-03-18 00:23:35.532680 dj_beatcloud-2.4.1b2/src/djtools/spotify/
--rw-r--r--   0 alrichards   (502) staff       (20)      718 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b2/src/djtools/spotify/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3229 2023-03-09 18:55:21.000000 dj_beatcloud-2.4.1b2/src/djtools/spotify/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    15560 2023-03-18 00:19:54.000000 dj_beatcloud-2.4.1b2/src/djtools/spotify/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6199 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b2/src/djtools/spotify/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1958 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b2/src/djtools/spotify/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    17499 2023-03-17 15:21:16.000000 dj_beatcloud-2.4.1b2/src/djtools/spotify/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6385 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b2/src/djtools/spotify/test_playlist_builder.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-03-18 00:23:35.534841 dj_beatcloud-2.4.1b2/src/djtools/sync/
--rw-r--r--   0 alrichards   (502) staff       (20)      772 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b2/src/djtools/sync/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3954 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b2/src/djtools/sync/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8295 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b2/src/djtools/sync/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4914 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b2/src/djtools/sync/sync_operations.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3239 2023-03-17 23:24:20.000000 dj_beatcloud-2.4.1b2/src/djtools/sync/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     7672 2023-03-18 00:19:57.000000 dj_beatcloud-2.4.1b2/src/djtools/sync/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4710 2023-03-18 00:19:57.000000 dj_beatcloud-2.4.1b2/src/djtools/sync/test_sync_operations.py
--rw-r--r--   0 alrichards   (502) staff       (20)      830 2023-03-18 00:19:57.000000 dj_beatcloud-2.4.1b2/src/djtools/test_main.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-03-18 00:23:35.538344 dj_beatcloud-2.4.1b2/src/djtools/utils/
--rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b2/src/djtools/utils/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3546 2023-03-16 00:15:12.000000 dj_beatcloud-2.4.1b2/src/djtools/utils/check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1064 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b2/src/djtools/utils/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8795 2023-03-18 00:19:54.000000 dj_beatcloud-2.4.1b2/src/djtools/utils/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3179 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b2/src/djtools/utils/test_check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)      397 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b2/src/djtools/utils/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     9151 2023-03-18 00:19:54.000000 dj_beatcloud-2.4.1b2/src/djtools/utils/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1558 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b2/src/djtools/utils/test_url_download.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1800 2023-03-16 00:15:04.000000 dj_beatcloud-2.4.1b2/src/djtools/utils/url_download.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-03-18 00:23:35.539215 dj_beatcloud-2.4.1b2/src/test_data/
--rw-r--r--   0 alrichards   (502) staff       (20)      137 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b2/src/test_data/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3749 2023-03-18 00:19:57.000000 dj_beatcloud-2.4.1b2/src/test_data/conftest.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-12 23:26:05.578379 dj_beatcloud-2.4.1b3/
+-rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.4.1b3/LICENSE
+-rw-r--r--   0 alrichards   (502) staff       (20)       64 2022-06-16 01:40:44.000000 dj_beatcloud-2.4.1b3/MANIFEST.in
+-rw-r--r--   0 alrichards   (502) staff       (20)    29508 2023-04-12 23:26:05.578517 dj_beatcloud-2.4.1b3/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)    28223 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/README.md
+-rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/pyproject.toml
+-rw-r--r--   0 alrichards   (502) staff       (20)      164 2023-04-12 23:26:05.578978 dj_beatcloud-2.4.1b3/setup.cfg
+-rw-r--r--   0 alrichards   (502) staff       (20)     2225 2023-04-12 23:24:14.000000 dj_beatcloud-2.4.1b3/setup.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-12 23:26:05.560863 dj_beatcloud-2.4.1b3/src/
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-12 23:26:05.563271 dj_beatcloud-2.4.1b3/src/dj_beatcloud.egg-info/
+-rw-r--r--   0 alrichards   (502) staff       (20)    29508 2023-04-12 23:26:05.000000 dj_beatcloud-2.4.1b3/src/dj_beatcloud.egg-info/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     2193 2023-04-12 23:26:05.000000 dj_beatcloud-2.4.1b3/src/dj_beatcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-04-12 23:26:05.000000 dj_beatcloud-2.4.1b3/src/dj_beatcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)       50 2023-04-12 23:26:05.000000 dj_beatcloud-2.4.1b3/src/dj_beatcloud.egg-info/entry_points.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)      332 2023-04-12 23:26:05.000000 dj_beatcloud-2.4.1b3/src/dj_beatcloud.egg-info/requires.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)       18 2023-04-12 23:26:05.000000 dj_beatcloud-2.4.1b3/src/dj_beatcloud.egg-info/top_level.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-12 23:26:05.564167 dj_beatcloud-2.4.1b3/src/djtools/
+-rw-r--r--   0 alrichards   (502) staff       (20)      966 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b3/src/djtools/__init__.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-12 23:26:05.566842 dj_beatcloud-2.4.1b3/src/djtools/configs/
+-rw-r--r--   0 alrichards   (502) staff       (20)     6148 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b3/src/djtools/configs/.DS_Store
+-rw-r--r--   0 alrichards   (502) staff       (20)     4258 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b3/src/djtools/configs/README.md
+-rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b3/src/djtools/configs/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3113 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/configs/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1223 2023-03-09 22:09:23.000000 dj_beatcloud-2.4.1b3/src/djtools/configs/config.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)    13418 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/configs/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b3/src/djtools/configs/logging.conf
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-04-12 15:31:08.000000 dj_beatcloud-2.4.1b3/src/djtools/configs/registered_users.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)      878 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/configs/rekordbox_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-03-09 22:09:23.000000 dj_beatcloud-2.4.1b3/src/djtools/configs/spotify_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)     2305 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/configs/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4478 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/configs/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1721 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b3/src/djtools/dj_tools.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-12 23:26:05.567112 dj_beatcloud-2.4.1b3/src/djtools/logs/
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2022-06-16 01:40:44.000000 dj_beatcloud-2.4.1b3/src/djtools/logs/empty.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)     1649 2023-03-16 00:56:47.000000 dj_beatcloud-2.4.1b3/src/djtools/main.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-12 23:26:05.570397 dj_beatcloud-2.4.1b3/src/djtools/rekordbox/
+-rw-r--r--   0 alrichards   (502) staff       (20)     1360 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b3/src/djtools/rekordbox/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1794 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/rekordbox/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4123 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/rekordbox/copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4521 2023-04-12 23:23:56.000000 dj_beatcloud-2.4.1b3/src/djtools/rekordbox/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    18868 2023-04-12 23:23:56.000000 dj_beatcloud-2.4.1b3/src/djtools/rekordbox/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2859 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/rekordbox/randomize_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    13303 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/rekordbox/tag_parsers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1225 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/rekordbox/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1390 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/rekordbox/test_copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2807 2023-04-12 23:23:56.000000 dj_beatcloud-2.4.1b3/src/djtools/rekordbox/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5142 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/rekordbox/test_playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1477 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/rekordbox/test_randomize_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3975 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/rekordbox/test_tag_parsers.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-12 23:26:05.572653 dj_beatcloud-2.4.1b3/src/djtools/spotify/
+-rw-r--r--   0 alrichards   (502) staff       (20)      718 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b3/src/djtools/spotify/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3229 2023-03-09 18:55:21.000000 dj_beatcloud-2.4.1b3/src/djtools/spotify/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    15361 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/spotify/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6155 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/spotify/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1958 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b3/src/djtools/spotify/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    17499 2023-03-17 15:21:16.000000 dj_beatcloud-2.4.1b3/src/djtools/spotify/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6153 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/spotify/test_playlist_builder.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-12 23:26:05.575380 dj_beatcloud-2.4.1b3/src/djtools/sync/
+-rw-r--r--   0 alrichards   (502) staff       (20)      772 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b3/src/djtools/sync/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3899 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/sync/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     8237 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/sync/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4605 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/sync/sync_operations.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3282 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/sync/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     7496 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/sync/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4520 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/sync/test_sync_operations.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      830 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/test_main.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-12 23:26:05.577747 dj_beatcloud-2.4.1b3/src/djtools/utils/
+-rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b3/src/djtools/utils/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3488 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/utils/check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1093 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/utils/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     7888 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/utils/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3227 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/utils/test_check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      397 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b3/src/djtools/utils/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     8500 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/utils/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1580 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/utils/test_url_download.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1641 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/utils/url_download.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-12 23:26:05.578220 dj_beatcloud-2.4.1b3/src/test_data/
+-rw-r--r--   0 alrichards   (502) staff       (20)      138 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/test_data/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3547 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/test_data/conftest.py
```

### Comparing `dj_beatcloud-2.4.1b2/LICENSE` & `dj_beatcloud-2.4.1b3/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b2/PKG-INFO` & `dj_beatcloud-2.4.1b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj_beatcloud
-Version: 2.4.1b2
+Version: 2.4.1b3
 Summary: DJ Tools is a library for managing a collection of music and Rekordbox XML files.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 License: GNU GPLv3
 Keywords: MP3 Rekordbox XML spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dj_beatcloud-2.4.1b2/README.md` & `dj_beatcloud-2.4.1b3/README.md`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b2/setup.py` & `dj_beatcloud-2.4.1b3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 EXTRAS = {
         'levenshtein': ['python-Levenshtein==0.12.2']
 }
 
 setup(
     name='dj_beatcloud',
-    version='2.4.1-b2',
+    version='2.4.1-b3',
     description=(
         'DJ Tools is a library for managing a collection of music and '
         'Rekordbox XML files.'
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url='https://github.com/a-rich/DJ-tools',
```

### Comparing `dj_beatcloud-2.4.1b2/src/dj_beatcloud.egg-info/PKG-INFO` & `dj_beatcloud-2.4.1b3/src/dj_beatcloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-beatcloud
-Version: 2.4.1b2
+Version: 2.4.1b3
 Summary: DJ Tools is a library for managing a collection of music and Rekordbox XML files.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 License: GNU GPLv3
 Keywords: MP3 Rekordbox XML spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dj_beatcloud-2.4.1b2/src/dj_beatcloud.egg-info/SOURCES.txt` & `dj_beatcloud-2.4.1b3/src/dj_beatcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/__init__.py` & `dj_beatcloud-2.4.1b3/src/djtools/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/configs/.DS_Store` & `dj_beatcloud-2.4.1b3/src/djtools/configs/.DS_Store`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/configs/README.md` & `dj_beatcloud-2.4.1b3/src/djtools/configs/README.md`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/configs/config.py` & `dj_beatcloud-2.4.1b3/src/djtools/configs/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 """This module contains the base configuration object. All the attributes of
 this configuration object either don't apply to any particular package or they
 apply to multiple packages. The attributes of this configuration object
 correspond with the "configs" key of config.yaml."""
 import logging
 import os
+from pathlib import Path
 from typing_extensions import Literal
 
-from pydantic import BaseModel, Extra, NonNegativeInt
+from pydantic import BaseModel, Extra, NonNegativeInt, validator
 
 
 logger = logging.getLogger(__name__)
 
 
 class BaseConfig(BaseModel, extra=Extra.allow):
     """Base configuration object used across the whole library."""
 
     AWS_PROFILE: str = "default"
     LOG_LEVEL: Literal[
         "DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"
     ] = "INFO"
     VERBOSITY: NonNegativeInt = 0
-    XML_PATH: str = ""
+    XML_PATH: Path = None
 
     def __init__(self, *args, **kwargs):
         """Constructor.
         
         Raises:
             RuntimeError: awscli must be installed.
             RuntimeError: AWS_PROFILE must be valid.
@@ -64,14 +65,14 @@
         if not self.XML_PATH:
             logger.warning(
                 "XML_PATH is not set. Without this set to a valid Rekordbox "
                 "XML export, you cannot use the following features: "
                 "COPY_PLAYLISTS, DOWNLOAD_XML, RANDOMIZE_PLAYLISTS, "
                 "REKORDBOX_PLAYLISTS, UPLOAD_XML"
             )
-        elif not os.path.exists(self.XML_PATH):
+        elif not self.XML_PATH.exists():
             logger.warning(
                 "XML_PATH does not exist. Without this set to a valid "
                 "Rekordbox XML export, you cannot use the following features: "
                 "COPY_PLAYLISTS, DOWNLOAD_XML, RANDOMIZE_PLAYLISTS, "
                 "REKORDBOX_PLAYLISTS, UPLOAD_XML"
             )
```

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/configs/config.yaml` & `dj_beatcloud-2.4.1b3/src/djtools/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/configs/helpers.py` & `dj_beatcloud-2.4.1b3/src/djtools/configs/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """This module is responible for building this library's configuration objects
 using config.yaml. If command-line arguments are provided, this module
 overrides the corresponding configuration options with these arguments.
 """
 import argparse
 from argparse import ArgumentParser
 import logging
-import os
-from typing import Any, Dict, Union
+from pathlib import Path
+from typing import Any, Dict, List, Union
 
 import yaml
 
 from djtools.configs.config import BaseConfig
 from djtools.rekordbox.config import RekordboxConfig
 from djtools.spotify.config import SpotifyConfig
 from djtools.sync.config import SyncConfig
 from djtools.utils.config import UtilsConfig
-from djtools.utils.helpers import make_dirs
 
 
 logger = logging.getLogger(__name__)
 
 pkg_cfg = {
     "configs": BaseConfig,
     "rekordbox": RekordboxConfig,
@@ -105,15 +104,15 @@
         help=(
             "Minimum similarity to indicate overlap between Beatcloud and "
             "Spotify / local tracks"
         ),
     )
     parser.add_argument(
         "--check-tracks-local-dirs",
-        type=str,
+        type=convert_to_paths,
         nargs="+",
         help="List of local directories to check against the Beatcloud",
     )
     parser.add_argument(
         "--check-tracks-spotify-playlists",
         type=str,
         nargs="+",
@@ -123,31 +122,31 @@
         "--copy-playlists",
         type=str,
         nargs="+",
         help="List of Rekordbox playlists to copy audio files from",
     )
     parser.add_argument(
         "--copy-playlists-destination",
-        type=str,
+        type=convert_to_paths,
         help="Location to copy Rekordbox playlists' audio files to",
     )
     parser.add_argument(
         "--discord-url",
         type=str,
         help="Discord webhook URL",
     )
     parser.add_argument(
         "--download-exclude-dirs",
-        type=str,
+        type=convert_to_paths,
         nargs="+",
         help="Paths to exclude when downloading from the Beatcloud",
     )
     parser.add_argument(
         "--download-include-dirs",
-        type=str,
+        type=convert_to_paths,
         nargs="+",
         help="Paths to include when downloading from the Beatcloud",
     )
     parser.add_argument(
         "--download-music",
         action="store_true",
         help="Trigger downloading new tracks from the Beatcloud",
@@ -171,15 +170,15 @@
         "--import-user",
         type=str,
         metavar="Entry of registered_user.yaml",
         help="Registered USER whose XML_PATH you're downloading",
     )
     parser.add_argument(
         "--link-configs",
-        type=str,
+        type=convert_to_paths,
         help="Location to symlink library configuration files to",
     )
     parser.add_argument(
         "--log-level",
         choices=["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"],
         help="Logger level",
     )
@@ -250,21 +249,21 @@
     parser.add_argument(
         "--spotify-username",
         type=str,
         help="Spotify user to maintain auto-playlists for",
     )
     parser.add_argument(
         "--upload-exclude-dirs",
-        type=str,
+        type=convert_to_paths,
         nargs="+",
         help="List of paths to exclude when uploading to the Beatcloud",
     )
     parser.add_argument(
         "--upload-include-dirs",
-        type=str,
+        type=convert_to_paths,
         nargs="+",
         help="List of paths to include when uploading to the Beatcloud",
     )
     parser.add_argument(
         "--upload-music",
         action="store_true",
         help="Trigger uploading new tracks from the Beatcloud",
@@ -277,20 +276,20 @@
     parser.add_argument(
         "--url-download",
         type=str,
         help="URL to download audio file(s) from",
     )
     parser.add_argument(
         "--url-download-destination",
-        type=str,
+        type=convert_to_paths,
         help="Location to download audio file(s) to",
     )
     parser.add_argument(
         "--usb-path",
-        type=str,
+        type=convert_to_paths,
         help="Path to a drive with audio files",
     )
     parser.add_argument(
         "--user",
         type=str,
         metavar="Entry of registered_user.yaml",
         help="Entry in registered_users.yaml which maps to your USB_PATH",
@@ -300,38 +299,38 @@
         "-v",
         action="count",
         default=0,
         help="Logging verbosity",
     )
     parser.add_argument(
         "--xml-path",
-        type=str,
+        type=convert_to_paths,
         help='Path to your exported Rekordbox XML database',
     )
     args = parser.parse_args()
 
     if args.log_level:
         logger.setLevel(args.log_level)
 
     if args.link_configs:
-        args.link_configs = args.link_configs.rstrip("/")
-        if os.path.exists(args.link_configs):
+        args.link_configs = Path(args.link_configs)
+        if args.link_configs.exists():
             msg = (
                 f"{args.link_configs} must be a directory that does not "
                 "already exist"
             )
             logger.error(msg)
             raise ValueError(msg)
-        parent_dir = os.path.dirname(args.link_configs)
-        if not os.path.exists(parent_dir):
-            make_dirs(parent_dir)
-
-        package_root = os.path.dirname(os.path.dirname(__file__))
-        configs_dir = os.path.join(package_root, "configs").replace(os.sep, "/")
-        os.symlink(configs_dir, args.link_configs, target_is_directory=True)
+        parent_dir = args.link_configs.parent
+        if not parent_dir.exists():
+            parent_dir.mkdir(parents=True, exist_ok=True)
+
+        package_root = Path(__file__).parent.parent
+        configs_dir = package_root / "configs"
+        args.link_configs.symlink_to(configs_dir, target_is_directory=True)
 
     return vars(args)
 
 
 def build_config():
     """This function loads configurations for the library.
     
@@ -341,19 +340,17 @@
     Raises:
         RuntimeError: config.yaml must be a valid YAML.
 
     Returns:
         Global configuration object.
     """
     # Load "config.yaml".
-    config_dir = os.path.join(
-        os.path.dirname(os.path.dirname(__file__)), "configs"
-    ).replace(os.sep, "/")
-    config_file = os.path.join(config_dir, "config.yaml").replace(os.sep, "/")
-    if os.path.exists(config_file):
+    config_dir = Path(__file__).parent.parent / "configs"
+    config_file = config_dir / "config.yaml"
+    if config_file.exists():
         try:
             with open(config_file, mode="r", encoding="utf-8") as _file:
                 config = yaml.load(_file, Loader=yaml.FullLoader) or {}
         except Exception as exc:
             msg = f'Error reading "config.yaml": {exc}'
             logger.critical(msg)
             raise RuntimeError(msg) from Exception
@@ -399,14 +396,29 @@
             for k, v in filter_dict(cfg).items()
         }
     )
 
     return joined_config
 
 
+def convert_to_paths(paths: Union[str, List[str]]) -> Path:
+    """Convert CLI argument from string to pathlib.Path.
+
+    Args:
+        paths: String(s) representing path(s).
+
+    Returns:
+        Path 
+    """
+    if isinstance(paths, List):
+        return list(map(Path, paths))
+
+    return Path(paths)
+
+
 def filter_dict(
     sub_config: Union[RekordboxConfig, SpotifyConfig, SyncConfig, UtilsConfig],
 ) -> Dict[Any, Any]:
     """Filters out the superclass key: value pairs of a subclass.
 
     Args:
         sub_config: Instance of any subclass of BaseConfig.
```

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/configs/test_config.py` & `dj_beatcloud-2.4.1b3/src/djtools/configs/test_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 
 def test_baseconfig_no_xml_path(caplog):
     caplog.set_level("WARNING")
     cfg = {
         "AWS_PROFILE": "default",
         "SPOTIFY_CLIENT_ID": "",
-        "XML_PATH": "",
+        "XML_PATH": None,
     }
     BaseConfig(**cfg)
     assert caplog.records[0].message == (
         "XML_PATH is not set. Without this set to a valid Rekordbox XML "
         "export, you cannot use the following features: "
         "COPY_PLAYLISTS, DOWNLOAD_XML, RANDOMIZE_PLAYLISTS, "
         "REKORDBOX_PLAYLISTS, UPLOAD_XML"
```

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/configs/test_helpers.py` & `dj_beatcloud-2.4.1b3/src/djtools/configs/test_helpers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 from argparse import Namespace
-import os
+from pathlib import Path
+from typing import List
 from unittest import mock
 
 import pytest
 
 from djtools.configs.config import BaseConfig
 from djtools.configs.helpers import (
-    arg_parse, build_config, filter_dict, parse_yaml, pkg_cfg
+    arg_parse, build_config, convert_to_paths, filter_dict, parse_yaml, pkg_cfg
 )
 from test_data import MockOpen
 
 
 @mock.patch("argparse.ArgumentParser.parse_args")
 def test_arg_parse_links_configs(mock_parse_args, tmpdir):
-    config_path = os.path.join(tmpdir, "test_dir").replace(os.sep, "/")
+    config_path = Path(tmpdir) / "test_dir"
     mock_parse_args.return_value = Namespace(
         link_configs=config_path, log_level="INFO"
     )
     args = arg_parse()
-    assert os.path.islink(config_path)
+    assert config_path.is_symlink()
 
 
 @mock.patch("argparse.ArgumentParser.parse_args")
 def test_arg_parse_links_configs_dir_does_exist(mock_parse_args, tmpdir):
-    link_path = os.path.join(
-        str(tmpdir), "new_dir", "link_dir"
-    ).replace(os.sep, "/")
+    link_path = Path(tmpdir) / "new_dir" / "link_dir"
     mock_parse_args.return_value = Namespace(
         link_configs=link_path, log_level="INFO"
     )
     args = arg_parse()
-    assert os.path.exists(link_path)
-    assert os.path.islink(link_path)
+    assert link_path.exists()
+    assert link_path.is_symlink()
 
 
 @mock.patch("argparse.ArgumentParser.parse_args")
 def test_arg_parse_links_configs_dir_does_not_exist(mock_parse_args, tmpdir):
     link_path = str(tmpdir)
     mock_parse_args.return_value = Namespace(
         link_configs=link_path, log_level="INFO"
@@ -77,29 +76,41 @@
         config = build_config()
     assert 'Error reading "config.yaml"' in caplog.records[0].message
 
 
 @mock.patch("djtools.spotify.helpers.get_spotify_client")
 @mock.patch(
     "builtins.open",
-    MockOpen(files=["registered_users.yaml", "config.yaml"]).open
+    MockOpen(
+        files=["registered_users.yaml", "config.yaml"],
+        user_a=("aweeeezy", "/Volumes/AWEEEEZY/"),
+        user_b=("test_user", "/test/USB/"),
+    ).open
 )
 @mock.patch("argparse.ArgumentParser.parse_args")
 def test_build_config_no_config_yaml(mock_parse_args, mock_spotify_client):
     mock_parse_args.return_value = Namespace(
         link_configs="", log_level="INFO"
     )
-    config_dir = os.path.join(
-        os.path.dirname(os.path.dirname(__file__)), "configs"
-    ).replace(os.sep, "/")
-    config_file = os.path.join(config_dir, "config.yaml").replace(os.sep, "/")
-    with mock.patch("os.path.exists", return_value=False):
-        assert not os.path.exists(config_file)
+    config_dir = Path(__file__).parent.parent / "configs"
+    config_file = config_dir / "config.yaml"
+    with mock.patch.object(Path, "exists", return_value=False):
+        assert not config_file.exists()
         config = build_config()
-    assert os.path.exists(config_file)
+    assert config_file.exists()
+
+
+@pytest.mark.parametrize("paths", ["path", ["path1", "path2"]])
+def test_convert_to_paths(paths):
+    paths = convert_to_paths(paths)
+    if isinstance(paths, List):
+        for path in paths:
+            assert isinstance(path, Path)
+    else:
+        assert isinstance(paths, Path)
 
 
 @pytest.mark.parametrize("config", [cfg for cfg in pkg_cfg.values()])
 @mock.patch("djtools.spotify.helpers.get_spotify_client")
 @mock.patch(
     "builtins.open",
     MockOpen(files=["registered_users.yaml"], write_only=True).open
```

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/dj_tools.py` & `dj_beatcloud-2.4.1b3/src/djtools/dj_tools.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/main.py` & `dj_beatcloud-2.4.1b3/src/djtools/main.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/rekordbox/__init__.py` & `dj_beatcloud-2.4.1b3/src/djtools/rekordbox/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/rekordbox/config.py` & `dj_beatcloud-2.4.1b3/src/djtools/rekordbox/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """This module contains the configuration object for the rekordbox package.
 The attributes of this configuration object correspond with the "rekordbox" key
 of config.yaml
 """
 import logging
-import os
+from pathlib import Path
 from typing import List 
 
 from djtools.configs.config import BaseConfig
 
 
 logger = logging.getLogger(__name__)
 
 
 class RekordboxConfig(BaseConfig):
     """Configuration object for the rekordbox package."""
 
     COPY_PLAYLISTS:  List[str] = []
-    COPY_PLAYLISTS_DESTINATION: str = ""
+    COPY_PLAYLISTS_DESTINATION: Path = None
     PURE_GENRE_PLAYLISTS:  List[str] = []
     RANDOMIZE_PLAYLISTS:  List[str] = []
     REKORDBOX_PLAYLISTS: bool = False 
     REKORDBOX_PLAYLISTS_REMAINDER: str = "folder"
 
     def __init__(self, *args, **kwargs):
         """Constructor.
@@ -33,24 +33,23 @@
 
         if any(
             [
                 self.COPY_PLAYLISTS,
                 self.RANDOMIZE_PLAYLISTS,
                 self.REKORDBOX_PLAYLISTS,
             ]
-        ) and (not self.XML_PATH or not os.path.exists(self.XML_PATH)):
+        ) and (not self.XML_PATH or not self.XML_PATH.exists()):
             raise RuntimeError(
                 "Using the rekordbox package requires the config option "
                 "XML_PATH to be a valid rekordbox XML file"
             )
 
         if self.REKORDBOX_PLAYLISTS:
-            playlist_config = os.path.join(
-                os.path.dirname(os.path.dirname(__file__)),
-                "configs",
-                "rekordbox_playlists.yaml",
-            ).replace(os.sep, "/")
-            if not os.path.exists(playlist_config):
+            playlist_config = (
+                Path(__file__).parent.parent / "configs" /
+                "rekordbox_playlists.yaml"
+            )
+            if not playlist_config.exists():
                 raise RuntimeError(
                     "rekordbox_playlists.yaml must be a valid YAML to use the "
                     "REKORDBOX_PLAYLISTS feature"
                 )
```

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/rekordbox/copy_playlists.py` & `dj_beatcloud-2.4.1b3/src/djtools/rekordbox/copy_playlists.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import os
 
 from bs4 import BeautifulSoup
 from tqdm import tqdm
 
 from djtools.configs.config import BaseConfig
 from djtools.rekordbox.helpers import copy_file
-from djtools.utils.helpers import make_dirs
 
 
 def copy_playlists(config: BaseConfig):
     """Copies tracks from provided playlists to a destination.
 
     Writes a new XML with these playlists and updated Location fields.
 
@@ -31,15 +30,15 @@
             "XML_PATH".
     """
     # Load Rekordbox database from XML.
     with open(config.XML_PATH, mode="r", encoding="utf-8") as _file:	
         rekordbox_database = BeautifulSoup(_file.read(), "xml")
 
     # Create destination directory.
-    make_dirs(config.COPY_PLAYLISTS_DESTINATION)
+    config.COPY_PLAYLISTS_DESTINATION.mkdir(parents=True, exist_ok=True)
 
     # Nodes to not remove when writing the new XML.
     keep_nodes = set()
 
     # Get the set of track IDs across the provided playlists.
     # Get the parents of playlists so they aren't removed from the output XML.
     playlists_track_keys = defaultdict(set)
@@ -104,17 +103,12 @@
         playlist = rekordbox_database.find_all(
             "NODE", {"Name": playlist_name}
         )[0]
         for track_id in playlists_track_keys[playlist_name]:
             playlist.append(rekordbox_database.new_tag("TRACK", Key=track_id))
     
     # Write new XML.
-    new_rekordbox_database_path = os.path.join(
-        os.path.dirname(config.XML_PATH),
-        f"relocated_{os.path.basename(config.XML_PATH)}"
-    ).replace(os.sep, "/")
+    new_db = config.XML_PATH.parent / f"relocated_{config.XML_PATH.name}"
     with open(
-        new_rekordbox_database_path,
-        mode="wb",
-        encoding=rekordbox_database.original_encoding,
+        new_db, mode="wb", encoding=rekordbox_database.original_encoding,
     ) as _file:
         _file.write(rekordbox_database.prettify("utf-8"))
```

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/rekordbox/helpers.py` & `dj_beatcloud-2.4.1b3/src/djtools/rekordbox/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """This module contains helpers for the rekordbox package."""
-import os
+from pathlib import Path
 import re
 import shutil
 from typing import Any, Dict, List, Optional, Set, Tuple 
 from urllib.parse import quote, unquote
 
 import bs4
 from bs4 import BeautifulSoup
@@ -88,30 +88,28 @@
             return track_ids
         else:
             return set(tracks.get(tag, {}).keys())
 
 
 def copy_file(
     track: bs4.element.Tag,
-    destination: str,
+    destination: Path,
     loc_prefix: str="file://localhost",
 ):
     """Copies tracks to a destination and writes new Location field.
 
     Args:
         track: TRACK node from XML.
         destination: Directory to copy tracks to.
         loc_prefix: Location field prefix.
     """
-    loc = unquote(track["Location"]).split(loc_prefix)[-1]
-    new_loc = os.path.join(
-        destination, os.path.basename(loc)
-    ).replace(os.sep, "/")
+    loc = Path(unquote(track["Location"]).split(loc_prefix)[-1])
+    new_loc = destination / loc.name
     shutil.copyfile(loc, new_loc)		
-    track["Location"] = f"{loc_prefix}{quote(new_loc)}"
+    track["Location"] = f"{loc_prefix}{quote(new_loc.as_posix())}"
 
 
 def get_playlist_track_locations(
     soup: BeautifulSoup, _playlist: str, seen_tracks: Set[str]
 ) -> List[str]:
     """Finds playlist in "XML_PATH" that matches "_playlist" and returns a list
         of the track nodes in that playlist that aren't in "seen_tracks".
```

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/rekordbox/playlist_builder.py` & `dj_beatcloud-2.4.1b3/src/djtools/rekordbox/playlist_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 NOTE: In order for "My Tags" to be stored in the exported XML files, users must
 enable the 'Add "My Tag" to the "Comments"' setting under
 "Preferences > Advanced > Browse".
 """
 from collections import defaultdict
 import logging
-import os
 from pathlib import Path
 from typing import Dict, List, Set, Tuple, Union
 
 import bs4
 from bs4 import BeautifulSoup
 import yaml
 
@@ -55,16 +54,16 @@
         * "{}": encloses a playlist name to select those tracks. 
         * "[]": encloses a comma-delimited list of integers representing
             ratings (1 through 5) or BPMs (numbers greater than 5); ranges can
             be specified by separating two integers with a dash.
     """
     def __init__(
         self,
-        rekordbox_database: Union[str, Path],
-        playlist_config: Union[str, Path],
+        rekordbox_database: Path,
+        playlist_config: Path,
         pure_genre_playlists: List[str] = [],
         playlist_remainder_type: str = "",
     ):
         """Constructor.
 
         Args:
             rekordbox_database: Path to Rekordbox XML.
@@ -221,16 +220,17 @@
             if node.attrs and node.attrs["Name"] != "ROOT":
                 node.decompose()
         
         # Insert the auto-playlists into the playlists root.
         self._playlists_root.insert(0, self._auto_playlists_root)
 
         # Write XML file.
-        _dir, _file = os.path.split(self._database_path)
-        auto_xml_path = os.path.join(_dir, f"auto_{_file}").replace(os.sep, "/")
+        _dir = self._database_path.parent
+        _file = self._database_path.name
+        auto_xml_path = _dir / f"auto_{_file}"
         with open(
             auto_xml_path, mode="wb", encoding=self._database.orignal_encoding
         ) as _file:
             _file.write(self._database.prettify("utf-8"))
 
     def _add_other(
         self,
@@ -426,20 +426,17 @@
 
 def rekordbox_playlists(config: BaseConfig):
     """Runs the PlaylistBuilder.
 
     Args:
         config: Configuration object.
     """
-    playlist_config = os.path.join(
-        os.path.dirname(os.path.dirname(__file__)),
-        "configs",
-        "rekordbox_playlists.yaml",
-    ).replace(os.sep, "/")
-
+    playlist_config = (
+        Path(__file__).parent.parent / "configs" / "rekordbox_playlists.yaml"
+    )
     playlist_builder = PlaylistBuilder(
         rekordbox_database=config.XML_PATH,
         playlist_config=playlist_config,
         pure_genre_playlists=config.PURE_GENRE_PLAYLISTS,
         playlist_remainder_type=config.REKORDBOX_PLAYLISTS_REMAINDER,
     )
     playlist_builder()
```

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/rekordbox/randomize_playlists.py` & `dj_beatcloud-2.4.1b3/src/djtools/rekordbox/randomize_playlists.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,13 +69,14 @@
         "NODE", KeyType="0", Name="AUTO_RANDOMIZE", Type="1"
     )
     for track in randomized_tracks:
         new_playlist.append(soup.new_tag("TRACK", Key=track["TrackID"]))
     playlists_root.insert(0, new_playlist)
 
     # Write XML file.
-    _dir, _file = os.path.split(config.XML_PATH)
-    auto_xml_path = os.path.join(_dir, f"auto_{_file}").replace(os.sep, "/")
+    _dir = config.XML_PATH.parent
+    _file = config.XML_PATH.name
+    auto_xml_path = _dir / f"auto_{_file}"
     with open(
         auto_xml_path, mode="wb", encoding=soup.orignal_encoding
     ) as _file:
         _file.write(soup.prettify("utf-8"))
```

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/rekordbox/tag_parsers.py` & `dj_beatcloud-2.4.1b3/src/djtools/rekordbox/tag_parsers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/rekordbox/test_config.py` & `dj_beatcloud-2.4.1b3/src/djtools/rekordbox/test_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+from pathlib import Path
 from unittest import mock
 
 import pytest
 
 from djtools.rekordbox.config import RekordboxConfig
-from test_data import MockExists
+from test_data import mock_exists
 
 
 pytest_plugins = [
    "test_data",
 ]
 
 
@@ -17,33 +18,34 @@
         "RANDOMIZE_PLAYLISTS": [],
         "REKORDBOX_PLAYLISTS": False,
     }
     RekordboxConfig(**cfg)
 
 
 @mock.patch(
-    "djtools.rekordbox.config.os.path.exists",
-    MockExists(
-        files=[
+    "djtools.rekordbox.config.Path.exists",
+    lambda path: mock_exists(
+        [
             ("rekordbox_playlists.yaml", False),
             ("rekordbox.xml", True),
-        ]
-    ).exists,
+        ],
+        path,
+    )
 )
 def test_rekordboxconfig_no_rekordbox_playlists_config(test_xml):
     cfg = {"REKORDBOX_PLAYLISTS": True, "XML_PATH": test_xml}
     with pytest.raises(
         RuntimeError,
         match="rekordbox_playlists.yaml must be a valid YAML to use the "
             "REKORDBOX_PLAYLISTS feature"
     ):
         RekordboxConfig(**cfg)
 
 
 def test_rekordboxconfig_no_xml():
-    cfg = {"REKORDBOX_PLAYLISTS": True, "XML_PATH": ""}
+    cfg = {"REKORDBOX_PLAYLISTS": True, "XML_PATH": None}
     with pytest.raises(
         RuntimeError,
         match="Using the rekordbox package requires the config option "
             "XML_PATH to be a valid rekordbox XML file",
     ):
         RekordboxConfig(**cfg)
```

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/rekordbox/test_copy_playlists.py` & `dj_beatcloud-2.4.1b3/src/djtools/rekordbox/test_copy_playlists.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,41 @@
-import os
+from pathlib import Path
 from urllib.parse import unquote
 
 from bs4 import BeautifulSoup
 import pytest
 
 from djtools.rekordbox.copy_playlists import copy_playlists
 
 
 pytest_plugins = [
  "test_data",
 ]
 
 
 def test_copy_playlists(tmpdir, test_config, test_xml):
-    target_playlists = ["Rock", "Dubstep"]
-    new_xml = os.path.join(
-        os.path.dirname(test_xml), "relocated_rekordbox.xml"
-    ).replace(os.sep, "/")
-    test_output_dir = os.path.join(tmpdir, "output").replace(os.sep, "/")
+    target_playlists = ["Hip Hop"]
+    test_xml = Path(test_xml)
+    new_xml = test_xml.parent / "relocated_rekordbox.xml"
+    test_output_dir = Path(tmpdir) / "output"
     test_config.XML_PATH = test_xml
     test_config.COPY_PLAYLISTS = target_playlists
-    test_config.COPY_PLAYLISTS_DESTINATION = test_output_dir
+    test_config.COPY_PLAYLISTS_DESTINATION = Path(test_output_dir)
     copy_playlists(test_config)
-    assert os.listdir(test_output_dir)
-    assert os.path.exists(new_xml)
+    assert list(test_output_dir.iterdir())
+    assert new_xml.exists()
     with open(new_xml, mode="r", encoding="utf-8") as _file:
         xml = BeautifulSoup(_file.read(), "xml")
     for track in xml.find_all("TRACK"):
         if not track.get("Location"):
             continue
         assert any(x in track["Genre"] for x in target_playlists)
-        assert test_output_dir in unquote(track["Location"])
+        assert test_output_dir.as_posix() in unquote(track["Location"])
         
 
 def test_copy_playlists_invalid_playlist(tmpdir, test_config, test_xml):
     playlist = "invalid_playlist"
     test_config.XML_PATH = test_xml
     test_config.COPY_PLAYLISTS = [playlist]
-    test_config.COPY_PLAYLISTS_DESTINATION = tmpdir
+    test_config.COPY_PLAYLISTS_DESTINATION = Path(tmpdir)
     with pytest.raises(LookupError, match=f"{playlist} not found"):
         copy_playlists(test_config)
```

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/rekordbox/test_helpers.py` & `dj_beatcloud-2.4.1b3/src/djtools/rekordbox/test_helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import inspect
-import os
+from pathlib import Path
 import re
 from urllib.parse import unquote
 
-from bs4 import BeautifulSoup
 import pytest
 
 from djtools.rekordbox.helpers import (
     BooleanNode,
     copy_file,
     get_playlist_track_locations,
     set_tag,
@@ -65,31 +64,29 @@
             re.escape(f"{[x.__name__ for x in node.operators]}")
         ),
     ):
         node({})
 
 
 def test_copy_file(tmpdir, test_track):
-    dest_dir = os.path.join(tmpdir, "output").replace(os.sep, "/")
-    os.makedirs(dest_dir)
-    old_track_loc = test_track["Location"]
+    dest_dir = Path(tmpdir) / "output"
+    dest_dir.mkdir(parents=True, exist_ok=True)
+    old_track_loc = Path(test_track["Location"])
     copy_file(track=test_track, destination=dest_dir)
-    new_track_loc = test_track["Location"]
+    new_track_loc = unquote(test_track["Location"])
     loc_prefix = inspect.signature(
         copy_file
     ).parameters.get("loc_prefix").default
-    new_file_path = os.path.join(
-        dest_dir, os.path.basename(old_track_loc)
-    ).replace(os.sep, "/")
+    new_file_path = dest_dir / old_track_loc.name
     assert new_track_loc == f"{loc_prefix}{new_file_path}"
-    assert os.path.exists(unquote(new_file_path))
+    assert new_file_path.exists()
 
 
 def test_get_playlist_track_locations(xml):
-    playlist = "Dubstep"
+    playlist = "Hip Hop"
     seen_tracks = set()
     ret = get_playlist_track_locations(xml, playlist, seen_tracks)
     assert seen_tracks
     assert ret
     assert len(ret) == len(seen_tracks)
```

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/rekordbox/test_playlist_builder.py` & `dj_beatcloud-2.4.1b3/src/djtools/rekordbox/test_playlist_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from pathlib import Path
 
 from bs4 import BeautifulSoup
 import pytest
 import yaml
 
 from djtools.rekordbox.playlist_builder import (
     PlaylistBuilder, rekordbox_playlists    
@@ -15,81 +16,79 @@
 
 
 @pytest.mark.parametrize(
     "remainder_type", ["", "folder", "playlist", "invalid"]
 )
 def test_playlistbuilder(remainder_type, test_xml, test_playlist_config):
     playlist_builder = PlaylistBuilder(
-        rekordbox_database=test_xml,
-        playlist_config=test_playlist_config,
-        pure_genre_playlists=["Techno"],
+        rekordbox_database=Path(test_xml),
+        playlist_config=Path(test_playlist_config),
+        pure_genre_playlists=["Dubstep"],
         playlist_remainder_type=remainder_type
     )()
 
 
 def test_playlistbuilder_combiner_playlist_contains_new_playlist_selector_tracks(
-    test_playlist_config, test_xml
+    test_playlist_config, test_xml, xml
 ):
     # Insert test track and Combiner playlist to target it.
     with open(test_playlist_config, mode="r", encoding="utf-8",) as _file:
         playlist_config = yaml.load(_file, Loader=yaml.FullLoader) or {}
-    with open(test_xml, mode="r", encoding="utf-8") as _file:
-        db = BeautifulSoup(_file.read(), "xml")
-    new_track = db.new_tag("TRACK")
+    new_track = xml.new_tag("TRACK")
     new_track_ID = "-1"
     new_track.attrs = {
         "TrackID": new_track_ID,
         "AverageBpm": "140.00",
         "Genre": "Dubstep",
         "Rating": "255",
         "Location": "file://localhost/test-track.mp3",
         "Comments": "",
     }
-    collection = db.find_all("COLLECTION")[0]
+    collection = xml.find_all("COLLECTION")[0]
     collection.insert(0, new_track)
-    selector_playlist = "{All Bass} & [140]"
+    selector_playlist = "{Dubstep} & [140]"
     playlist_config["Combiner"]["playlists"] = [selector_playlist]
     playlist_config = {
         k: v for k, v in playlist_config.items()
         if k in ["GenreTagParser", "Combiner"]
     }
     with open(test_playlist_config, mode="w", encoding="utf-8",) as _file:
         playlist_config = yaml.dump(playlist_config, _file)
-    with open(test_xml, mode="wb", encoding=db.orignal_encoding) as _file:
-        _file.write(db.prettify("utf-8"))
+    with open(test_xml, mode="wb", encoding=xml.orignal_encoding) as _file:
+        _file.write(xml.prettify("utf-8"))
 
     # Test pre-conditions.
-    playlist = db.find_all("NODE", {"Name": "All Bass", "Type": "1"})[0]
+    playlist = xml.find_all("NODE", {"Name": "Dubstep", "Type": "1"})[0]
     for track_key in playlist.find_all("TRACK"):
         assert (
             track_key["Key"] != new_track_ID,
-            "Test track should not exist in All Bass!"
+            "Test track should not exist in Dubstep!"
         )
     test_track = None
-    for track in db.find_all("TRACK"):
+    for track in xml.find_all("TRACK"):
         if not track.get("Location"):
             continue
         if track.get("TrackID") == new_track_ID:
             test_track = track
     assert test_track, "Test track should exist in XML!"
 
     # Run the PlaylistBuilder (GenreTagParser and Combiner).
     playlist_builder = PlaylistBuilder(
-        rekordbox_database=test_xml,
-        playlist_config=test_playlist_config,
+        rekordbox_database=Path(test_xml),
+        playlist_config=Path(test_playlist_config),
     )()
 
     # Load XML generated by the PlaylistBuilder.
     path, file_name = os.path.split(test_xml)
     with open(os.path.join(path, f"auto_{file_name}"), mode="r", encoding="utf-8") as _file:
         db = BeautifulSoup(_file.read(), "xml")
 
-    # Test that the test track was inserted into the "All Bass" playlist.
+    # Test that the test track was inserted into the "Dubstep" playlist.
     test_track = None
-    playlist = db.find_all("NODE", {"Name": "All Bass", "Type": "1"})[0]
+    playlist = db.find_all("NODE", {"Name": "Dubstep", "Type": "1"})[0]
     for track_key in playlist.find_all("TRACK"):
         if track_key["Key"] == new_track_ID:
             test_track = track_key
     assert test_track, "New track was not found in the genre playlist!"
 
     # Test that the test track was inserted into the Combiner playlist.
     test_track = None
@@ -138,9 +137,9 @@
         PlaylistBuilder(
             rekordbox_database=test_xml,
             playlist_config=test_playlist_config,
         )()
 
 
 def test_rekordbox_playlists(test_config, test_xml):
-    test_config.XML_PATH = test_xml
+    test_config.XML_PATH = Path(test_xml)
     rekordbox_playlists(test_config)
```

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/rekordbox/test_randomize_playlists.py` & `dj_beatcloud-2.4.1b3/src/djtools/rekordbox/test_randomize_playlists.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-import os
+from pathlib import Path
 
 from bs4 import BeautifulSoup
 import pytest
 
 from djtools.rekordbox.randomize_playlists import randomize_playlists
 
 
 pytest_plugins = [
     "test_data",
 ]
 
 
 def test_randomize_playlists(test_config, test_xml, caplog):
     caplog.set_level("INFO")
-    playlists = ["Acid Techno", "Dubstep"]
+    playlists = ["Hip Hop"]
+    test_xml = Path(test_xml)
     test_config.XML_PATH = test_xml
     test_config.RANDOMIZE_PLAYLISTS = playlists
     randomize_playlists(test_config)
-    new_xml = os.path.join(
-        os.path.dirname(test_xml), f"auto_{os.path.basename(test_xml)}"
-    ).replace(os.sep, "/")
+    new_xml = test_xml.parent / f"auto_{test_xml.name}"
     with open(new_xml, mode="r", encoding="utf-8") as _file:
         db = BeautifulSoup(_file.read(), "xml")
     randomized_playlist = db.find_all(
         "NODE", {"Name": "AUTO_RANDOMIZE", "Type": "1"}
     )[0]
     original_playlists = [
         db.find_all("NODE", {"Name": playlist, "Type": "1"})[0]
```

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/rekordbox/test_tag_parsers.py` & `dj_beatcloud-2.4.1b3/src/djtools/rekordbox/test_tag_parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         )
         combiner_parser.get_playlist_mapping(xml)
 
 
 def test_genretagparser(test_playlist_config, xml):
     with open(test_playlist_config, mode="r", encoding="utf-8",) as _file:
         playlist_config = yaml.load(_file, Loader=yaml.FullLoader) or {}
-    genre = "Techno"
+    genre = "Hip Hop"
     parser = GenreTagParser(
         parser_config=playlist_config["GenreTagParser"],
         pure_genre_playlists=[genre],
     )
     tracks = {
         track["TrackID"]: track for track in xml.find_all("TRACK")
         if track.get("Location")
@@ -77,15 +77,15 @@
                 genre in tag for tag in tags
             )
 
 
 def test_mytagparser(test_playlist_config, xml):
     with open(test_playlist_config, mode="r", encoding="utf-8",) as _file:
         playlist_config = yaml.load(_file, Loader=yaml.FullLoader) or {}
-    mytag = "Hypnotic"
+    mytag = "Dark"
     parser = MyTagParser(parser_config=playlist_config["MyTagParser"])
     tracks = {
         track["TrackID"]: track for track in xml.find_all("TRACK")
         if track.get("Location")
     }
     playlist = xml.find_all("NODE", {"Name": mytag, "Type": "1"})[0]
     for track_key in playlist.find_all("TRACK"):
```

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/spotify/__init__.py` & `dj_beatcloud-2.4.1b3/src/djtools/spotify/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/spotify/config.py` & `dj_beatcloud-2.4.1b3/src/djtools/spotify/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/spotify/helpers.py` & `dj_beatcloud-2.4.1b3/src/djtools/spotify/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """This module contains helper functions used by the "spotify" module."""
 from concurrent.futures import ThreadPoolExecutor
 import logging
 from operator import itemgetter
 import os
+from pathlib import Path
 import sys
 from typing import Any, Dict, List, Optional, Set, Tuple, Union
 
 import asyncpraw as praw
 from fuzzywuzzy import fuzz
 import spotipy
 from spotipy.oauth2 import SpotifyOAuth
@@ -163,20 +164,16 @@
 def get_playlist_ids() -> Dict[str, str]:
     """Load Spotify playlist names -> IDs lookup.
 
     Returns:
         Dictionary of Spotify playlist names mapped to playlist IDs. 
     """
     playlist_ids = {}
-    ids_path = os.path.join(
-        os.path.dirname(os.path.dirname(__file__)),
-        "configs",
-        "spotify_playlists.yaml",
-    ).replace(os.sep, "/")
-    if os.path.exists(ids_path):
+    ids_path = Path(__file__).parent.parent / "configs" / "spotify_playlists.yaml"
+    if ids_path.exists():
         with open(ids_path, mode="r", encoding="utf-8") as _file:
             playlist_ids = yaml.load(_file, Loader=yaml.FullLoader) or {}
     
     return playlist_ids
 
 
 def get_reddit_client(config: BaseConfig) -> praw.Reddit:
@@ -211,17 +208,15 @@
         auth_manager=SpotifyOAuth(
             client_id=config.SPOTIFY_CLIENT_ID,
             client_secret=config.SPOTIFY_CLIENT_SECRET,
             redirect_uri=config.SPOTIFY_REDIRECT_URI,
             scope="playlist-modify-public",
             requests_timeout=30,
             cache_handler=spotipy.CacheFileHandler(
-                cache_path=os.path.join(
-                    os.path.dirname(__file__), ".spotify.cache"
-                ).replace(os.sep, "/"),
+                cache_path=Path(__file__).parent / ".spotify.cache"
             ),
         )
     )
     
     return spotify
 
 
@@ -498,14 +493,12 @@
 def write_playlist_ids(playlist_ids: Dict[str, str]):
     """Write playlist IDs to file.
 
     Args:
         playlist_ids: Dictionary of Spotify playlist names mapped to playlist
             IDs. 
     """
-    ids_path = os.path.join(
-        os.path.dirname(os.path.dirname(__file__)),
-        "configs",
-        "spotify_playlists.yaml",
-    ).replace(os.sep, "/")
+    ids_path = (
+        Path(__file__).parent.parent / "configs" / "spotify_playlists.yaml"
+    )
     with open(ids_path, mode="w", encoding="utf-8") as _file:
         yaml.dump(playlist_ids, _file)
```

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/spotify/playlist_builder.py` & `dj_beatcloud-2.4.1b3/src/djtools/spotify/playlist_builder.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 are then used to search the Spotify API for tracks. The resulting tracks have
 their title and artist fields compared with the reddit post title and are added
 to the respective playlist if the Levenshtein similarity passes a threshold.
 """
 import asyncio
 import logging
 import os
+from pathlib import Path
 
 import pyperclip
 import yaml
 
 from djtools.configs.config import BaseConfig
 from djtools.spotify.helpers import (
     filter_results,
@@ -51,18 +52,16 @@
         config: Configuration object.
     """
     spotify = get_spotify_client(config)
     reddit = get_reddit_client(config)
     playlist_ids = get_playlist_ids()
     
     praw_cache = {}
-    cache_file = os.path.join(
-        os.path.dirname(__file__), ".praw.cache"
-    ).replace(os.sep, "/")
-    if os.path.exists(cache_file):
+    cache_file = Path(__file__).parent / ".praw.cache"
+    if cache_file.exists():
         with open(cache_file, mode="r", encoding="utf-8") as _file:
             praw_cache = yaml.load(_file, Loader=yaml.FullLoader) or {}
     
     tasks = [
         asyncio.create_task(
             get_subreddit_posts(
                 spotify,
@@ -126,15 +125,15 @@
     user = ""
     files = []
     for line in data.split("\n"):
         if not line.startswith(" "):
             if not user:
                 user = line.split("/")[0]
             continue
-        file_, _ = os.path.splitext(line)
+        file_ = Path(line).stem
         try:
             track, artist = file_.strip().split(" - ")
         except ValueError:
             logger.warning(f'{line} is not a valid file')
             continue
         files.append((track, artist))
     files = list(filter(lambda x: len(x) == 2, files))
```

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/spotify/test_config.py` & `dj_beatcloud-2.4.1b3/src/djtools/spotify/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/spotify/test_helpers.py` & `dj_beatcloud-2.4.1b3/src/djtools/spotify/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/spotify/test_playlist_builder.py` & `dj_beatcloud-2.4.1b3/src/djtools/spotify/test_playlist_builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os
+from pathlib import Path
 from unittest import mock
 
 import pyperclip
 import pytest
 
 from djtools.spotify.config import SubredditConfig
 from djtools.spotify.playlist_builder import (
@@ -20,15 +20,15 @@
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
     "playlist_subreddits", [[], [SubredditConfig(name="jungle").dict()]],
 )
 @pytest.mark.parametrize("got_playlist_ids", [True, False])
 @pytest.mark.parametrize("got_tracks", [True, False])
-@mock.patch("os.path.exists", return_value=True)
+@mock.patch.object(Path, "exists",return_value=True)
 @mock.patch(
     "djtools.spotify.helpers.update_existing_playlist",
     return_value={
         "name": "test_playlist",
         "external_urls": {"spotify": "https://test-url.com"},
         "id": "test-id",
     },
@@ -70,15 +70,14 @@
             files=["spotify_playlists.yaml", ".praw.cache"],
             content='{"jungle": "some-id"}' if got_playlist_ids else "{}",
         ).open
     ):
         await async_update_auto_playlists(test_config)
 
 
-@pytest.mark.parametrize("input_", [True, "test.txt"])
 @mock.patch(
     "djtools.spotify.playlist_builder.filter_results",
     return_value={
         "id": "some_id",
         "name": "some_name",
         "artists": [ 
             {"name": "some_artist"},
@@ -86,42 +85,37 @@
     }
 )
 @mock.patch(
     "djtools.spotify.playlist_builder.populate_playlist",
     return_value={"some-playlist": "some-id"},
 )
 @mock.patch("djtools.spotify.playlist_builder.get_spotify_client")
+@mock.patch(
+    "pyperclip.paste",
+    return_value="""aweeeezy/Bass/2022-09-03: 5
+                   Brazil - A.M.C.mp3
+                   Endless Haze - Koherent.mp3
+                   Two Rangers - Two Rangers.mp3
+                   Under Pressure - Alix Perez, T-Man.mp3
+                   zoom.1 - Relativity Lounge, wicker's portal.mp3
+                  aweeeezy/House/2022-09-03: 2
+                   Shirt - Cour T..mp3
+                   UNKNOWN - 1 - Unknown Artist.mp3""",
+)
 def test_playlist_from_upload(
     mock_spotify,
     mock_populate_playlist,
     mock_filter_results,
-    input_,
     test_config,
     tmpdir,
 ):
     test_config.SPOTIFY_CLIENT_ID = "test_client_id"
     test_config.SPOTIFY_CLIENT_SECRET = "test_client_secret"
     test_config.SPOTIFY_REDIRECT_URI = "test_redirect_uri"
-    content = """aweeeezy/Bass/2022-09-03: 5
-                   Brazil - A.M.C.mp3
-                   Endless Haze - Koherent.mp3
-                   Two Rangers - Two Rangers.mp3
-                   Under Pressure - Alix Perez, T-Man.mp3
-                   zoom.1 - Relativity Lounge, wicker's portal.mp3
-                  aweeeezy/House/2022-09-03: 2
-                   Shirt - Cour T..mp3
-                   UNKNOWN - 1 - Unknown Artist.mp3"""
-    if isinstance(input_, bool):
-        pyperclip.copy(content)
-        test_config.PLAYLIST_FROM_UPLOAD = True
-    else:
-        path = os.path.join(tmpdir, input_).replace(os.sep, "/")
-        with open(path, mode="w", encoding="utf-8",) as _file:
-            _file.write(content)
-        test_config.PLAYLIST_FROM_UPLOAD = path
+    test_config.PLAYLIST_FROM_UPLOAD = True
     with mock.patch(
         "builtins.open",
         MockOpen(files=["spotify_playlists.yaml"], content="{}").open
     ):
         playlist_from_upload(test_config)
 
 
@@ -132,21 +126,22 @@
 @mock.patch("djtools.spotify.playlist_builder.get_spotify_client")
 def test_playlist_from_upload_handles_non_match(
     mock_spotify, mock_filter_results, test_config, caplog
 ):
     caplog.set_level("WARNING")
     title = "Under Pressure"
     artist = "Alix Perez, T-Man"
-    content = f"""aweeeezy/Bass/2022-09-03: 5
-                   {title} - {artist}.mp3"""
-    pyperclip.copy(content)
     test_config.PLAYLIST_FROM_UPLOAD = True
     with mock.patch(
         "builtins.open",
         MockOpen(files=["spotify_playlists.yaml"], content="{}").open
+    ), mock.patch(
+        "pyperclip.paste",
+        return_value=f"""aweeeezy/Bass/2022-09-03: 5
+            {title} - {artist}.mp3""",
     ):
         playlist_from_upload(test_config)
     assert caplog.records[0].message == (
         f"Could not find a match for {title} - {artist}"
     )
 
 
@@ -160,33 +155,34 @@
 ):
     caplog.set_level("ERROR")
     mock_spotify.return_value.search.side_effect = (
         mock_spotify_search.side_effect
     )
     title = "Under Pressure"
     artist = "Alix Perez, T-Man"
-    content = f"""aweeeezy/Bass/2022-09-03: 5
-                   {title} - {artist}.mp3"""
-    pyperclip.copy(content)
     test_config.PLAYLIST_FROM_UPLOAD = True
     test_config.SPOTIFY_CLIENT_ID = "test_client_id"
     test_config.SPOTIFY_CLIENT_SECRET = "test_client_secret"
     test_config.SPOTIFY_REDIRECT_URI = "test_redirect_uri"
     with mock.patch(
         "builtins.open",
         MockOpen(files=["spotify_playlists.yaml"], content="{}").open
+    ), mock.patch(
+        "pyperclip.paste",
+        return_value=f"""aweeeezy/Bass/2022-09-03: 5
+            {title} - {artist}.mp3"""
     ):
         playlist_from_upload(test_config)
     assert caplog.records[0].message.startswith(
         f'Error searching for "{title} - {artist}"'
     )
 
 
+@mock.patch("pyperclip.paste", return_value="")
 def test_playlist_from_upload_raises_runtimeerror(test_config):
-    pyperclip.copy("")
     test_config.PLAYLIST_FROM_UPLOAD = True
     with pytest.raises(
         RuntimeError,
         match="Generating a Spotify playlist from an upload requires output "
             "from an upload_music Discord webhook to be copied to the "
             "system's clipboard"
     ):
```

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/sync/__init__.py` & `dj_beatcloud-2.4.1b3/src/djtools/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/sync/config.py` & `dj_beatcloud-2.4.1b3/src/djtools/sync/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """This module contains the configuration object for the sync package.
 The attributes of this configuration object correspond with the "sync" key
 of config.yaml
 """
 import getpass
 import logging
-import os
+from pathlib import Path
 from typing import Dict, List
 
 import yaml
 
 from djtools.configs.config import BaseConfig
 
 
@@ -16,26 +16,26 @@
 
 
 class SyncConfig(BaseConfig):
     """Configuration object for the sync package."""
 
     AWS_USE_DATE_MODIFIED: bool = False 
     DISCORD_URL: str = ""
-    DOWNLOAD_EXCLUDE_DIRS: List[str] = []
-    DOWNLOAD_INCLUDE_DIRS: List[str] = []
+    DOWNLOAD_EXCLUDE_DIRS: List[Path] = []
+    DOWNLOAD_INCLUDE_DIRS: List[Path] = []
     DOWNLOAD_MUSIC: bool = False 
     DOWNLOAD_SPOTIFY: str = ""
     DOWNLOAD_XML: bool = False 
     DRYRUN: bool = False
     IMPORT_USER: str = ""
-    UPLOAD_EXCLUDE_DIRS: List[str] = []
-    UPLOAD_INCLUDE_DIRS: List[str] = []
+    UPLOAD_EXCLUDE_DIRS: List[Path] = []
+    UPLOAD_INCLUDE_DIRS: List[Path] = []
     UPLOAD_MUSIC: bool = False 
     UPLOAD_XML: bool = False 
-    USB_PATH: str = ""
+    USB_PATH: Path = None
     USER: str = ""
 
     def __init__(self, *args, **kwargs):
         """Constructor.
 
         Raises:
             ValueError: Both include and exclude dirs can't be provided at the
@@ -76,20 +76,18 @@
         
         if self.UPLOAD_MUSIC and not self.DISCORD_URL:
             logger.warning(
                 'DISCORD_URL is not configured...set this for "New Music" '
                 "discord messages!"
             )
 
-        registered_users_path = os.path.join(
-            os.path.dirname(os.path.dirname(__file__)),
-            "configs",
-            "registered_users.yaml",
-        ).replace(os.sep, "/")
-        if os.path.exists(registered_users_path):
+        registered_users_path = (
+            Path(__file__).parent.parent / "configs" / "registered_users.yaml"
+        )
+        if registered_users_path.exists():
             try:
                 with open(
                     registered_users_path, mode="r", encoding="utf-8"
                 ) as _file:
                     registered_users = (
                         yaml.load(_file, Loader=yaml.FullLoader) or {}
                     )
```

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/sync/helpers.py` & `dj_beatcloud-2.4.1b3/src/djtools/sync/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """This module contains helper functions used by the "sync_operations" module.
 Helper functions include formatting "aws s3 sync" commands, formatting the
 output of "aws s3 sync" commands, posting uploaded tracks to Discord, and
 modifying IMPORT_USER's XML to point to tracks located at "USB_PATH".
 """
 from datetime import datetime, timedelta
-from glob import glob
 from itertools import groupby
 import logging
-import os
+from pathlib import Path
 from subprocess import Popen, PIPE, CalledProcessError
 from typing import Dict, List, Optional, Union
 
 from bs4 import BeautifulSoup
 import requests
 import yaml
 
@@ -40,39 +39,43 @@
         Fully constructed "aws s3 sync" command.
     """
     if (
         (upload and config.UPLOAD_INCLUDE_DIRS)
         or (not upload and config.DOWNLOAD_INCLUDE_DIRS)
     ):
         _cmd.extend(["--exclude", "*"])
-        directories = getattr(
-            config, f'{"UP" if upload else "DOWN"}LOAD_INCLUDE_DIRS'
+        directories = map(
+            Path,
+            getattr(config, f'{"UP" if upload else "DOWN"}LOAD_INCLUDE_DIRS'),
         )
         for _dir in directories:
-            path, ext = os.path.splitext(_dir)
+            path = Path(_dir.stem)
+            ext = _dir.suffix
             if not ext:
-                path = os.path.join(_dir, "*").replace(os.sep, "/")
+                path = _dir / "*"
             else:
-                path = path + ext
-            _cmd.extend(["--include", path])
+                path = _dir.parent / path.with_suffix(ext)
+            _cmd.extend(["--include", path.as_posix()])
     if (
         (upload and config.UPLOAD_EXCLUDE_DIRS)
         or (not upload and config.DOWNLOAD_EXCLUDE_DIRS)
     ):
         _cmd.extend(["--include", "*"])
-        directories = getattr(
-            config, f'{"UP" if upload else "DOWN"}LOAD_EXCLUDE_DIRS'
+        directories = map(
+            Path,
+            getattr(config, f'{"UP" if upload else "DOWN"}LOAD_EXCLUDE_DIRS'),
         )
         for _dir in directories:
-            path, ext = os.path.splitext(_dir)
+            path = Path(_dir.stem)
+            ext = _dir.suffix
             if not ext:
-                path = os.path.join(_dir, "*").replace(os.sep, "/")
+                path = _dir / "*"
             else:
-                path = path + ext
-            _cmd.extend(["--exclude", path])
+                path = _dir.parent / path.with_suffix(ext)
+            _cmd.extend(["--exclude", path.as_posix()])
     if not config.AWS_USE_DATE_MODIFIED:
         _cmd.append("--size-only")
     if config.DRYRUN:
         _cmd.append("--dryrun")
     logger.info(" ".join(_cmd))
 
     return _cmd
@@ -82,28 +85,26 @@
     """This function modifies the "Location" field of track tags in a
         downloaded Rekordbox XML replacing the "USB_PATH" written by
         "IMPORT_USER" with the "USB_PATH" in "config.yaml".
 
     Args:
         config: Configuration object.
     """
-    registered_users_path = os.path.join(
-        os.path.dirname(os.path.dirname(__file__)),
-        "configs",
-        "registered_users.yaml",
-    ).replace(os.sep, "/")
+    registered_users_path = (
+        Path(__file__).parent.parent / "configs" / "registered_users.yaml"
+    )
 
     with open(registered_users_path, mode="r", encoding="utf-8") as _file:
         registered_users = yaml.load(_file, Loader=yaml.FullLoader)
         src = registered_users[config.IMPORT_USER].strip("/")
         dst = registered_users[config.USER].strip("/")
 
-    xml_path = os.path.join(
-        os.path.dirname(config.XML_PATH), f"{config.IMPORT_USER}_rekordbox.xml"
-    ).replace(os.sep, "/")
+    xml_path = (
+        Path(config.XML_PATH).parent / f"{config.IMPORT_USER}_rekordbox.xml"
+    )
 
     with open(xml_path, mode="r", encoding="utf-8") as _file:
         soup = BeautifulSoup(_file.read(), "xml")
         for track in soup.find_all("TRACK"):
             if not track.get("Location"):
                 continue
             track["Location"] = track["Location"].replace(src, dst)
@@ -172,44 +173,41 @@
             new_music += f"\t{track}\n"
     if new_music:
         logger.info(new_music)
 
     return new_music
 
 
-def upload_log(config: BaseConfig, log_file: str):
+def upload_log(config: BaseConfig, log_file: Path):
     """This function uploads "log_file" to the "USER" logs folder in S3. It
         then deletes all files created more than one day ago.
 
     Args:
         config: Configuration object.
         log_file: Path to log file.
     """
     if not config.AWS_PROFILE:
         logger.warning(
             "Logs cannot be backed up without specifying the config option "
             "AWS_PROFILE"
         )
         return
 
-    dst = (
-        "s3://dj.beatcloud.com/dj/logs/"
-        f"{config.USER}/{os.path.basename(log_file)}"
-    )
-    cmd = f"aws s3 cp {log_file} {dst}"
+    dst = f"s3://dj.beatcloud.com/dj/logs/{config.USER}/{log_file.name}"
+    cmd = f"aws s3 cp {log_file.as_posix()} {dst}"
     logger.info(cmd)
-    os.system(cmd)
+    Popen(cmd, shell=True).wait()
 
     now = datetime.now()
     one_day = timedelta(days=1)
-    for _file in glob(f"{os.path.dirname(log_file)}/*"):
-        if os.path.basename(_file) == "empty.txt":
+    for _file in log_file.parent.rglob("*"):
+        if _file.name == "empty.txt":
             continue
-        if os.path.getmtime(_file) < (now - one_day).timestamp():
-            os.remove(_file)
+        if _file.lstat().st_mtime < (now - one_day).timestamp():
+            _file.unlink()
 
 
 def webhook(
     url: str, content_size_limit: int = 2000, content: Optional[str] = None
 ):
     """Post track list of newly uploaded tracks to Discord channel associated
         with "url". Track list is split across multiple messages if the
```

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/sync/sync_operations.py` & `dj_beatcloud-2.4.1b3/src/djtools/sync/sync_operations.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """This module is responsible for syncing tracks between "USB_PATH" and the
 beatcloud (upload and download). It also handles uploading the Rekordbox XML
 located at "XML_PATH" and downloading the Rekordbox XML uploaded to the
 beatcloud by "IMPORT_USER" before modifying it to point to track locations at
 "USB_PATH".
 """
 import logging
-import os
+from os.path import getmtime
 from pathlib import Path
+from subprocess import Popen
 from typing import List
 
 from djtools.configs.config import BaseConfig
 from djtools.sync.helpers import (
     parse_sync_command, rewrite_xml, run_sync, webhook
 )
 from djtools.utils.check_tracks import compare_tracks
-from djtools.utils.helpers import make_dirs
 
 
 logger = logging.getLogger(__name__)
 
 
 def download_music(config: BaseConfig, beatcloud_tracks: List[str] = []):
     """This function syncs tracks from the beatcloud to "USB_PATH".
@@ -35,42 +35,33 @@
         user = config.DOWNLOAD_SPOTIFY.split("Uploads")[0].strip()
         beatcloud_tracks, beatcloud_matches = compare_tracks(
             config,
             beatcloud_tracks=beatcloud_tracks,
             download_spotify_playlist=config.DOWNLOAD_SPOTIFY,
         )
         config.DOWNLOAD_INCLUDE_DIRS = [
-            os.path.join(
-                user,
-                path.split(os.path.join(user, "").replace(os.sep, "/"))[-1]
-            )
+            (Path(user) / path.split(f"{Path(user)}/")[-1])
             for path in beatcloud_matches
         ]
         config.DOWNLOAD_EXCLUDE_DIRS = []
 
-    dest = os.path.join(config.USB_PATH, "DJ Music").replace(os.sep, "/")
-    glob_path = Path(dest)
-    old = {
-        str(p) for p in glob_path.rglob(
-            os.path.join("**", "*.*").replace(os.sep, "/")
-        )
-    }
+    dest = Path(config.USB_PATH) / "DJ Music"
+    glob_path = (Path("**") / "*.*").as_posix()
+    old = {str(p) for p in dest.rglob(glob_path)}
     logger.info(f"Found {len(old)} files")
 
     logger.info("Syncing remote track collection...")
-    make_dirs(dest)
-    cmd = ["aws", "s3", "sync", "s3://dj.beatcloud.com/dj/music/", dest]
+    dest.mkdir(parents=True, exist_ok=True)
+    cmd = [
+        "aws", "s3", "sync", "s3://dj.beatcloud.com/dj/music/", dest.as_posix()
+    ]
     run_sync(parse_sync_command(cmd, config))
 
-    new = {
-        str(p) for p in glob_path.rglob(
-            os.path.join("**", "*.*").replace(os.sep, "/")
-        )
-    }
-    difference = sorted(list(new.difference(old)), key=os.path.getmtime)
+    new = {str(p) for p in dest.rglob(glob_path)}
+    difference = sorted(list(new.difference(old)), key=getmtime)
     if difference:
         logger.info(f"Found {len(difference)} new files")
         for diff in difference:
             logger.info(f"\t{diff}")
     
     return beatcloud_tracks
 
@@ -80,53 +71,49 @@
         the "Location" field of all the tracks so that it points to USER's
         "USB_PATH".
 
     Args:
         config: Configuration object.
     """
     logger.info("Syncing remote rekordbox.xml...")
-    xml_dir = os.path.dirname(config.XML_PATH)
-    make_dirs(xml_dir)
-    _file = f'{config.IMPORT_USER}_rekordbox.xml'
-    _file = os.path.join(xml_dir, _file).replace(os.sep, "/")
+    xml_dir = Path(config.XML_PATH).parent
+    xml_dir.mkdir(parents=True, exist_ok=True)
+    _file = Path(xml_dir) / f'{config.IMPORT_USER}_rekordbox.xml'
     cmd = (
         "aws s3 cp s3://dj.beatcloud.com/dj/xml/"
         f'{config.IMPORT_USER}/rekordbox.xml {_file}'
     )
     logger.info(cmd)
-    os.system(cmd)
+    Popen(cmd, shell=True).wait()
     if config.USER != config.IMPORT_USER:
         rewrite_xml(config)
 
 
 def upload_music(config: BaseConfig):
     """This function syncs tracks from "USB_PATH" to the beatcloud.
         "AWS_USE_DATE_MODIFIED" can be used in order to reupload tracks that
         already exist in the beatcloud but have been modified since the last
         time they were uploaded (i.e. ID3 tags have been altered).
 
     Args:
         config: Configuration object.
     """
-    glob_path = Path(
-        os.path.join(config.USB_PATH, "DJ Music").replace(os.sep, "/")
-    )
-    hidden_files = {
-        str(p) for p in glob_path.rglob(
-            os.path.join("**", ".*.*").replace(os.sep, "/")
+    hidden_files = set(
+        (Path(config.USB_PATH) / "DJ Music").rglob(
+            (Path("**") / ".*.*").as_posix()
         )
-    }
+    )
     if hidden_files:
         logger.info(f"Removed {len(hidden_files)} files...")
         for _file in hidden_files:
             logger.info(f"\t{_file}")
-            os.remove(_file)
+            _file.unlink()
 
     logger.info("Syncing track collection...")
-    src = os.path.join(config.USB_PATH, "DJ Music").replace(os.sep, "/")
+    src = (Path(config.USB_PATH) / "DJ Music").as_posix()
     cmd = ["aws", "s3", "sync", src, "s3://dj.beatcloud.com/dj/music/"]
 
     if config.DISCORD_URL and not config.DRYRUN:
         webhook(
             config.DISCORD_URL,
             content=run_sync(parse_sync_command(cmd, config, upload=True)),
         )
@@ -140,8 +127,8 @@
     Args:
         config: Configuration object.
     """
     logger.info(f"Uploading {config.USER}'s rekordbox.xml...")
     dst = f"s3://dj.beatcloud.com/dj/xml/{config.USER}/"
     cmd = f"aws s3 cp {config.XML_PATH} {dst}"
     logger.info(cmd)
-    os.system(cmd)
+    Popen(cmd, shell=True).wait()
```

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/sync/test_config.py` & `dj_beatcloud-2.4.1b3/src/djtools/sync/test_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from pathlib import Path
 from unittest import mock
 
 import getpass
 import pytest
 
 
 from djtools.sync.config import SyncConfig
-from test_data import MockExists, MockOpen
+from test_data import mock_exists, MockOpen
 
 
 pytest_plugins = [
     "test_data",
 ]
 
 
@@ -62,46 +63,56 @@
     with pytest.raises(
         RuntimeError,
         match="Config must include AWS_PROFILE for sync operations"
     ):
         SyncConfig(**cfg)
 
 
-@mock.patch("builtins.open", MockOpen(files=["registered_users.yaml"], write_only=True).open)
 @mock.patch(
-    "djtools.sync.config.os.path.exists",
-    MockExists(
-        files=[
-            ("registered_users.yaml", False),
-        ]
-    ).exists,
+    "builtins.open",
+    MockOpen(files=["registered_users.yaml"],
+    write_only=True).open,
+)
+@mock.patch(
+    "djtools.sync.config.Path.exists",
+    lambda path: mock_exists([("registered_users.yaml", False)], path)
 )
 @mock.patch("djtools.spotify.helpers.get_spotify_client")
-def test_syncconfig_no_registered_users(mock_get_spotify_client, test_xml, caplog):
+def test_syncconfig_no_registered_users(
+    mock_get_spotify_client, test_xml, caplog
+):
     cfg = {
         "XML_PATH": test_xml,
         "SPOTIFY_CLIENT_ID": "id",
         "SPOTIFY_CLIENT_SECRET": "secret",
         "SPOTIFY_REDIRECT_URI": "uri",
         "SPOTIFY_USERNAME": "name",
     }
     caplog.set_level("WARNING")
     SyncConfig(**cfg)
     assert caplog.records[0].message == "No registered users!"
 
 
-@mock.patch("builtins.open", MockOpen(files=["registered_users.yaml"], write_only=True).open)
+@mock.patch(
+    "builtins.open",
+    MockOpen(files=["registered_users.yaml"],
+    write_only=True).open,
+)
 def test_syncconfig_set_user():
     cfg = {"USER": ""}
     assert not SyncConfig.__fields__["USER"].default
     sync_config = SyncConfig(**cfg)
     assert sync_config.USER == getpass.getuser()
 
 
-@mock.patch("builtins.open", MockOpen(files=["registered_users.yaml"], write_only=True).open)
+@mock.patch(
+    "builtins.open",
+    MockOpen(files=["registered_users.yaml"],
+    write_only=True).open,
+)
 @mock.patch("djtools.spotify.helpers.get_spotify_client")
 def test_syncconfig_upload_without_discord_url(
     mock_get_spotify_client, test_xml, caplog
 ):
     caplog.set_level("WARNING")
     cfg = {
         "UPLOAD_MUSIC": True,
```

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/sync/test_helpers.py` & `dj_beatcloud-2.4.1b3/src/djtools/sync/test_helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from datetime import datetime, timedelta
 import os
+from pathlib import Path
 import shutil
 import tempfile
 from unittest import mock
 
 from bs4 import BeautifulSoup
 import pytest
 
@@ -78,27 +79,24 @@
     user_a_path= "/Volumes/AWEEEEZY/"
     user_b_path= "/Volumes/my_beat_stick/"
     test_user = "aweeeezy"
     other_user = "other_user"
     test_config.USER = test_user
     test_config.IMPORT_USER = other_user
     test_config.XML_PATH = test_xml
-    other_users_xml = os.path.join(
-        os.path.dirname(test_xml), f'{other_user}_rekordbox.xml'
-    ).replace(os.sep, "/")
-    shutil.copyfile(test_xml, other_users_xml)
+    other_users_xml = Path(test_xml).parent / f"{other_user}_rekordbox.xml"
+    other_users_xml.write_text(Path(test_xml).read_text())
 
     for track in xml.find_all("TRACK"):
         if not track.get("Location"):
             continue
-        track["Location"] = os.path.join(
-            os.path.dirname(track["Location"]),
-            user_b_path.strip("/"),
-            os.path.basename(track["Location"]),
-        ).replace(os.sep, "/")
+        track["Location"] = (
+            Path(track["Location"]).parent / user_b_path.strip("/") /
+            Path(track["Location"]).name
+        )
     
     with open(
         other_users_xml, mode="wb", encoding=xml.orignal_encoding
     ) as _file:
         _file.write(xml.prettify("utf-8"))
         
     rewrite_xml(test_config)
@@ -110,19 +108,15 @@
                 continue
             assert user_a_path in track["Location"]
             assert user_b_path not in track["Location"]
 
 
 @mock.patch("djtools.sync.helpers.Popen")
 def test_run_sync(mock_popen, tmpdir):
-    with open(
-        os.path.join(tmpdir, "track.mp3").replace(os.sep, "/"),
-        mode="w",
-        encoding="utf-8",
-    ) as _file:
+    with open(Path(tmpdir) / "track.mp3", mode="w", encoding="utf-8") as _file:
         _file.write("")
     cmd = ["aws", "s3", "sync", str(tmpdir), "s3://dj.beatcloud.com/dj/music/"]
     sync_output = (
         "upload: ../../Volumes/AWEEEEZY/DJ Music/Bass/2022-12-21/track - "
             "artist.mp3 to s3://dj.beatcloud.com/dj/music/Bass/2022-12-21/"
             "track - artist.mp3\n"
         "upload: ../../Volumes/AWEEEEZY/DJ Music/Bass/2O22-12-21/other track "
@@ -165,36 +159,34 @@
         f"non-zero exit status {process.wait.return_value}."
     )
     with pytest.raises(Exception, match=msg):
         run_sync(cmd)
     assert caplog.records[0].message == msg
 
 
-@mock.patch("os.system")
-def test_upload_log(mock_os_system, tmpdir, test_config):
+@mock.patch("subprocess.Popen.wait")
+def test_upload_log(mock_subprocess, tmpdir, test_config):
     test_config.AWS_PROFILE = "DJ"
     now = datetime.now()
     one_day_ago = now - timedelta(days=1)
     test_log = f'{now.strftime("%Y-%m-%d")}.log'
     filenames = [
         "empty.txt",
         test_log, 
         f'{one_day_ago.strftime("%Y-%m-%d")}.log',
     ]
     ctime = one_day_ago.timestamp()
     for filename in filenames:
-        file_path = os.path.join(tmpdir, filename).replace(os.sep, "/")
+        file_path = Path(tmpdir) / filename
         with open(file_path, mode="w", encoding="utf-8") as _file:
             _file.write("stuff")
         if filename != test_log: 
             os.utime(file_path, (ctime, ctime))
-    upload_log(
-        test_config, os.path.join(tmpdir, test_log).replace(os.sep, "/")
-    )
-    assert len(os.listdir(tmpdir)) == len(filenames) - 1
+    upload_log(test_config, Path(tmpdir) / test_log)
+    assert len(list(Path(tmpdir).iterdir())) == len(filenames) - 1
 
 
 def test_upload_log_no_aws_profile(test_config, caplog):
     caplog.set_level("WARNING")
     test_config.AWS_PROFILE = ""
     ret = upload_log(test_config, "some_file.txt")
     assert ret is None
```

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/sync/test_sync_operations.py` & `dj_beatcloud-2.4.1b3/src/djtools/sync/test_sync_operations.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-import os
-import shutil
+from pathlib import Path
 from unittest import mock
 
 import pytest
 
 from djtools.sync.sync_operations import (
     download_music, download_xml, upload_music, upload_xml
 )
-from djtools.utils.helpers import make_dirs
 from test_data import MockOpen
 
 pytest_plugins = [
     "test_data",
 ]
 
 
@@ -25,23 +23,21 @@
 )
 def test_download_music(
     mock_compare_tracks, playlist_name, test_config, tmpdir, caplog
 ):
     caplog.set_level("INFO")
     test_config.USB_PATH = tmpdir
     test_config.DOWNLOAD_SPOTIFY = playlist_name
-    write_path = os.path.join(
-        tmpdir, "DJ Music", "file.mp3"
-    ).replace(os.sep, "/")
+    write_path = Path(tmpdir) / "DJ Music" / "file.mp3"
     cmd = [
         "aws",
         "s3",
         "sync",
         "s3://dj.beatcloud.com/dj/music/",
-        os.path.dirname(write_path),
+        write_path.parent.as_posix(),
     ]
     if playlist_name:
         cmd += ["--exclude", "*", "--include", "playlist/file.mp3"]
     cmd += ["--size-only"]
     with mock.patch(
         "djtools.sync.sync_operations.run_sync",
         side_effect=lambda *args, **kwargs: open(
@@ -50,45 +46,46 @@
     ) as mock_run_sync:
         download_music(test_config)
         mock_run_sync.assert_called_with(cmd)
     assert caplog.records[0].message == "Found 0 files"
     assert caplog.records[1].message == "Syncing remote track collection..."
     assert caplog.records[2].message == " ".join(cmd)
     assert caplog.records[3].message == "Found 1 new files"
-    assert os.path.basename(caplog.records[4].message) == "file.mp3"
+    assert Path(caplog.records[4].message).name == "file.mp3"
 
 
 @mock.patch(
     "builtins.open", 
     MockOpen(
         files=["registered_users.yaml"],
         user_a=("aweeeezy", "/Volumes/AWEEEEZY/"),
         user_b=("test_user", "/test/USB/"),
     ).open,
 )
 @mock.patch("djtools.sync.sync_operations.rewrite_xml")
-@mock.patch("os.system")
-def test_download_xml(mock_os_system, mock_rewrite_xml, test_config, test_xml, caplog):
+@mock.patch("subprocess.Popen.wait")
+def test_download_xml(
+    mock_subprocess, mock_rewrite_xml, test_config, test_xml, caplog
+):
     caplog.set_level("INFO")
     test_user = "test_user"
     other_user = "aweeeezy"
-    new_xml = os.path.join(
-        os.path.dirname(test_xml), f"{other_user}_rekordbox.xml"
-    ).replace(os.sep, "/")
-    shutil.copyfile(test_xml, new_xml)
+    test_xml = Path(test_xml)
+    new_xml = test_xml.parent / f"{other_user}_rekordbox.xml"
+    new_xml.write_text(test_xml.read_text())
     test_config.USER = test_user
     test_config.IMPORT_USER = other_user
     test_config.XML_PATH = test_xml
     download_xml(test_config)
     cmd = [
         "aws",
         "s3",
         "cp",
         f's3://dj.beatcloud.com/dj/xml/{other_user}/rekordbox.xml',
-        new_xml,
+        new_xml.as_posix(),
     ] 
     assert caplog.records[0].message == "Syncing remote rekordbox.xml..."
     assert caplog.records[1].message == " ".join(cmd)
     mock_rewrite_xml.assert_called_once()
 
 
 @pytest.mark.parametrize(
@@ -98,50 +95,45 @@
 @mock.patch("djtools.sync.sync_operations.webhook", return_value=None)
 def test_upload_music(
     mock_webhook, mock_run_sync, discord_url, tmpdir, test_config, caplog
 ):
     caplog.set_level("INFO")
     test_config.USB_PATH = tmpdir
     test_config.DISCORD_URL = discord_url
-    test_dir = os.path.join(tmpdir, "DJ Music").replace(os.sep, "/") 
-    make_dirs(test_dir)
+    test_dir = Path(tmpdir) / "DJ Music"
+    test_dir.mkdir(parents=True, exist_ok=True)
     for file_name in [".test_file.mp3", "test_file.mp3"]:
-        with open(
-            os.path.join(test_dir, file_name).replace(os.sep, "/"),
-            mode="w",
-            encoding="utf-8",
-        ) as file_:
+        with open(test_dir / file_name, mode="w", encoding="utf-8") as file_:
             file_.write("")
     upload_music(test_config)
     cmd = [
         "aws",
         "s3",
         "sync",
-        test_dir,
+        test_dir.as_posix(),
         "s3://dj.beatcloud.com/dj/music/",
         "--size-only",
     ]
     assert caplog.records[0].message == "Removed 1 files..."
-    assert os.path.basename(caplog.records[1].message) == ".test_file.mp3"
+    assert Path(caplog.records[1].message).name == ".test_file.mp3"
     assert caplog.records[2].message == "Syncing track collection..."
     assert caplog.records[3].message == " ".join(cmd)
-    assert len(os.listdir(test_dir)) == 1
+    assert len(list(test_dir.iterdir())) == 1
     mock_run_sync.assert_called_with(cmd)
     if discord_url:
         mock_webhook.assert_called_with(
             "https://discord.com/api/webhooks/some-id/", content=None
         )
 
 
-@mock.patch("os.system")
-def test_upload_xml(mock_os_system, test_config, test_xml, caplog):
+@mock.patch("subprocess.Popen.wait")
+def test_upload_xml(mock_subprocess, test_config, test_xml, caplog):
     caplog.set_level("INFO")
     test_user = "test_user"
     test_config.USER = test_user
     test_config.XML_PATH = test_xml
     cmd = f"aws s3 cp {test_xml} s3://dj.beatcloud.com/dj/xml/{test_user}/"
     upload_xml(test_config)
-    mock_os_system.assert_called_with(cmd)
     assert caplog.records[0].message == (
         f"Uploading {test_user}'s rekordbox.xml..."
     )
     assert caplog.records[1].message == cmd
```

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/test_main.py` & `dj_beatcloud-2.4.1b3/src/djtools/test_main.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/utils/__init__.py` & `dj_beatcloud-2.4.1b3/src/djtools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/utils/check_tracks.py` & `dj_beatcloud-2.4.1b3/src/djtools/utils/check_tracks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """This module is used to compare tracks from Spotify playlists and / or local
 directories to see if there is any overlap with the contents of the Beatcloud.
 """
 from itertools import groupby
 import logging
 from operator import itemgetter
-import os
 from typing import List, Optional, Tuple
 
 from djtools.configs.config import BaseConfig
 from djtools.utils.helpers import (
     find_matches, get_spotify_tracks, get_beatcloud_tracks, get_local_tracks
 )
 
@@ -67,17 +66,15 @@
 
     if not track_sets:
         return beatcloud_tracks, beatcloud_matches
 
     if not beatcloud_tracks:
         beatcloud_tracks = get_beatcloud_tracks()
     
-    path_lookup = {
-        os.path.splitext(os.path.basename(x))[0]: x for x in beatcloud_tracks
-    }
+    path_lookup = {x.stem: x for x in beatcloud_tracks}
     
     for tracks, track_type in track_sets:
         matches = find_matches(
             tracks,
             path_lookup.keys(),
             config,
         )
```

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/utils/config.py` & `dj_beatcloud-2.4.1b3/src/djtools/utils/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from pathlib import Path
 from typing import List
 
 from pydantic import NonNegativeInt
 
 from djtools.configs.config import BaseConfig
 
 
@@ -10,18 +11,18 @@
 
 
 class UtilsConfig(BaseConfig):
     """Configuration object for the utils package."""
 
     CHECK_TRACKS: bool = False 
     CHECK_TRACKS_FUZZ_RATIO: NonNegativeInt = 80
-    CHECK_TRACKS_LOCAL_DIRS:  List[str] = []
+    CHECK_TRACKS_LOCAL_DIRS:  List[Path] = []
     CHECK_TRACKS_SPOTIFY_PLAYLISTS:  List[str] = []
     URL_DOWNLOAD: str = ""
-    URL_DOWNLOAD_DESTINATION: str = ""
+    URL_DOWNLOAD_DESTINATION: Path = None
 
     def __init__(self, *args, **kwargs):
         """Constructor.
 
         Raises:
             ValueError: AWS_PROFILE must be set for CHECK_TRACKS.
         """
```

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/utils/helpers.py` & `dj_beatcloud-2.4.1b3/src/djtools/utils/helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """This module contains helper functions that are not specific to any
 particular subpackage of this library.
 """
 from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime
-from glob import glob
 from itertools import product
 import logging
 import logging.config
 import os
-from os import name as os_name
+from pathlib import Path
+from subprocess import check_output
 from typing import Any, AsyncGenerator, Dict, List, Optional, Set, Tuple
 
 from fuzzywuzzy import fuzz
 import spotipy
 from tqdm import tqdm
 
 from djtools.configs.config import BaseConfig
@@ -137,17 +137,16 @@
         artist names.
     
     Returns:
         Beatcloud track titles and artist names.
     """
     logger.info("Getting tracks from the beatcloud...")
     cmd = "aws s3 ls --recursive s3://dj.beatcloud.com/dj/music/"
-    with os.popen(cmd) as proc:
-        output = proc.read().split("\n")
-    tracks = [track for track in output if track]
+    output = check_output(cmd, shell=True).split("\n")
+    tracks = [Path(track) for track in output if track]
     logger.info(f"Got {len(tracks)} tracks")
 
     return tracks
 
 
 def get_local_tracks(config: BaseConfig) -> Dict[str, List[str]]:
     """Aggregates the files from one or more local directories in a dictionary
@@ -157,29 +156,22 @@
         config: Configuration object.
 
     Returns:
         Local file names keyed by parent directory.
     """
     local_dir_tracks = {}
     for _dir in config.CHECK_TRACKS_LOCAL_DIRS:
-        path = _dir.replace(os.sep, "/")
-        if not os.path.exists(path):
+        if not _dir.exists():
             logger.warning(
-                f"{path} does not exist; will not be able to check its "
+                f"{_dir} does not exist; will not be able to check its "
                 "contents against the beatcloud"
             )
             continue
-        files = glob(
-            os.path.join(path, "**", "*.*").replace(os.sep, "/"),
-            recursive=True,
-        )
-        if files:
-            local_dir_tracks[_dir] = [
-                os.path.splitext(os.path.basename(x))[0] for x in files
-            ]
+        files = (_dir / "**" / "*.*").rglob("*")
+        local_dir_tracks[_dir] = [_file.stem for _file in files]
 
     return local_dir_tracks
 
 
 def get_playlist_tracks(
     spotify: spotipy.Spotify, playlist_id: str
 ) -> Set[str]:
@@ -246,44 +238,19 @@
 
 def initialize_logger() -> Tuple[logging.Logger, str]:
     """Initializes logger from configuration.
 
     Returns:
         Tuple containing Logger and associated log file.
     """
-    log_file = os.path.join(
-        os.path.dirname(os.path.dirname(__file__)),
-        "logs",
-        f'{datetime.now().strftime("%Y-%m-%d")}.log',
-    ).replace(os.sep, "/")
-    log_conf = os.path.join(
-        os.path.dirname(os.path.dirname(__file__)), "configs", "logging.conf"
-    ).replace(os.sep, "/")
+    log_file = (
+        Path(__file__).parent.parent / "logs" /
+        f'{datetime.now().strftime("%Y-%m-%d")}.log'
+    )
+    log_conf = Path(__file__).parent.parent / "configs" / "logging.conf"
     logging.config.fileConfig(
         fname=log_conf,
         defaults={"logfilename": log_file},
         disable_existing_loggers=False,
     )
 
     return logging.getLogger(__name__), log_file
-
-
-def make_dirs(path: str):
-    """This function performs operating system agnostic directory creation.
-
-    Args:
-        path: Directory path.
-    """
-    if os_name == "nt":
-        cwd = os.getcwd()
-        path_parts = path.split(os.sep)
-        if path_parts and not path_parts[0]:
-            path_parts[0] = "/"
-        root = path_parts[0]
-        path_parts = path_parts[1:]
-        os.chdir(root)
-        for part in path_parts:
-            os.makedirs(part, exist_ok=True)
-            os.chdir(part)
-        os.chdir(cwd)
-    else:
-        os.makedirs(path, exist_ok=True)
```

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/utils/test_check_tracks.py` & `dj_beatcloud-2.4.1b3/src/djtools/utils/test_check_tracks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
+from pathlib import Path
 from unittest import mock
 
 import pytest
 
 from djtools.utils.check_tracks import compare_tracks
 
 
 pytest_plugins = [
     "test_data",
 ]
 
 
 @pytest.mark.parametrize("get_spotify_tracks_flag", [True, False])
 @pytest.mark.parametrize("get_local_tracks_flag", [True, False])
-@pytest.mark.parametrize("beatcloud_tracks", [[], ["track - artist"]])
+@pytest.mark.parametrize("beatcloud_tracks", [[], [Path("track - artist")]])
 @pytest.mark.parametrize("download_spotify", ["", "playlist Uploads"])
 @mock.patch("djtools.utils.check_tracks.get_local_tracks", return_value={})
 @mock.patch(
     "djtools.utils.check_tracks.get_beatcloud_tracks",
-    return_value=["aweeeezy/Bass/2022-12-21/track - artist.mp3"],
+    return_value=[Path("aweeeezy/Bass/2022-12-21/track - artist.mp3")],
 )
 @mock.patch("djtools.utils.check_tracks.get_spotify_tracks", return_value={})
 def test_compare_tracks(
     mock_get_spotify_tracks,
     mock_get_beatcloud_tracks,
     mock_get_local_tracks,
     get_spotify_tracks_flag,
@@ -30,22 +31,23 @@
     download_spotify,
     test_config,
     tmpdir,
     caplog,
 ):
     caplog.set_level("INFO")
     spotify_playlist = "playlist"
+    tmpdir = Path(tmpdir)
     test_config.CHECK_TRACKS = True
     test_config.CHECK_TRACKS_SPOTIFY_PLAYLISTS = [spotify_playlist]
-    test_config.CHECK_TRACKS_LOCAL_DIRS = [str(tmpdir)]
+    test_config.CHECK_TRACKS_LOCAL_DIRS = [tmpdir]
     test_config.DOWNLOAD_SPOTIFY = download_spotify
     if get_spotify_tracks_flag or download_spotify:
         mock_get_spotify_tracks.return_value = {"playlist": ["track - artist"]}
     if get_local_tracks_flag:
-        mock_get_local_tracks.return_value = {str(tmpdir): ["track - artist"]}
+        mock_get_local_tracks.return_value = {tmpdir: ["track - artist"]}
     ret_beatcloud_tracks, beatcloud_matches = compare_tracks(
         test_config,
         beatcloud_tracks,
         download_spotify_playlist=download_spotify,
     )
     if not get_spotify_tracks_flag and not download_spotify:
         assert caplog.records.pop(0).message == (
@@ -72,11 +74,11 @@
             "\t100: track - artist | track - artist"
         )
     if get_local_tracks_flag and not download_spotify:
         assert caplog.records.pop(0).message == (
             "\nLocal Directory Tracks / Beatcloud Matches: "
             f"{len(mock_get_local_tracks.return_value)}"
         )
-        assert caplog.records.pop(0).message == f"{str(tmpdir)}:"
+        assert caplog.records.pop(0).message == f"{tmpdir}:"
         assert caplog.records.pop(0).message == (
             "\t100: track - artist | track - artist"
         )
```

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/utils/test_helpers.py` & `dj_beatcloud-2.4.1b3/src/djtools/utils/test_helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import asyncio
 from datetime import datetime
-import os
+from pathlib import Path
 import logging
 from unittest import mock
 
 import pytest
 
 from djtools.utils.helpers import (
     add_tracks,
@@ -12,15 +12,14 @@
     catch,
     find_matches,
     initialize_logger,
     get_beatcloud_tracks,
     get_local_tracks,
     get_playlist_tracks,
     get_spotify_tracks,
-    make_dirs,
 )
 from test_data import MockOpen
 
 
 pytest_plugins = [
     "test_data",
 ]
@@ -137,38 +136,37 @@
         [],
         [
             "aweeeezy/Bass/2022-12-21/track - artist.mp3",
             "aweeeezy/Techno/2022-12-21/track - artist.mp3",
         ]
     ]
 )
-@mock.patch("os.popen")
+@mock.patch("djtools.utils.helpers.check_output")
 def test_get_beatcloud_tracks(mock_os_popen, proc_dump):
-    process = mock_os_popen.return_value.__enter__.return_value
-    process.read.side_effect = lambda: "\n".join(proc_dump)
+    proc_dump = list(map(Path, proc_dump))
+    process = mock_os_popen.return_value = "\n".join(map(Path.as_posix, proc_dump))
     tracks = get_beatcloud_tracks()
     mock_os_popen.assert_called_once()
     assert len(tracks) == len(proc_dump)
     for track, line in zip(tracks, proc_dump):
         assert track == line
 
 
 def test_get_local_tracks(tmpdir, test_config):
     check_dirs = []
+    tmpdir = Path(tmpdir)
     for dir in ["dir1", "dir2"]:
-        path = os.path.join(tmpdir, dir).replace(os.sep, "/")
-        os.makedirs(path)
+        path = tmpdir / dir
+        path.mkdir(parents=True, exist_ok=True)
         check_dirs.append(path)
-    test_config.CHECK_TRACKS_LOCAL_DIRS = check_dirs + ["nonexistent_dir"]
+    test_config.CHECK_TRACKS_LOCAL_DIRS = check_dirs + [Path("nonexistent_dir")]
     beatcloud_tracks = ["test_file1.mp3", "test_file2.mp3"]
     for index, track in enumerate(beatcloud_tracks):
         with open(
-            os.path.join(
-                check_dirs[index % len(check_dirs)], f"{track}"
-            ).replace(os.sep, "/"),
+            check_dirs[index % len(check_dirs)] / f"{track}",
             mode="w",
             encoding="utf-8",
         ) as _file:
             _file.write("")
     local_dir_tracks = get_local_tracks(test_config)
     assert all(x in local_dir_tracks for x in check_dirs)
     assert len(local_dir_tracks) == len(check_dirs)
@@ -282,24 +280,8 @@
     mock_get_playlist_tracks.assert_called_once()
 
 
 def test_initialize_logger():
     today = f'{datetime.now().strftime("%Y-%m-%d")}.log'
     logger, log_file = initialize_logger()
     assert isinstance(logger, logging.Logger)
-    assert os.path.basename(log_file) == today
-
-
-@pytest.mark.parametrize("platform", ["posix", "nt"])
-def test_make_dirs(tmpdir, platform):
-    with mock.patch("djtools.utils.helpers.os_name", platform):
-        new_dir = os.path.join(tmpdir, "test_dir").replace(os.sep, "/")
-        make_dirs(new_dir)
-        assert os.path.exists(new_dir)
-        new_sub_dir = os.path.join(
-            tmpdir, "test_dir_2", "sub_dir"
-        ).replace(os.sep, "/")
-        make_dirs(new_sub_dir)
-        assert os.path.exists(new_sub_dir)
-        rel_dir = os.path.join(tmpdir, "relative_dir").replace(os.sep, "/")
-        make_dirs(rel_dir)
-        assert os.path.exists(rel_dir)
+    assert log_file.name == today
```

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/utils/test_url_download.py` & `dj_beatcloud-2.4.1b3/src/djtools/utils/test_url_download.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os
+from pathlib import Path
 from unittest import mock
 
 import pytest
 from youtube_dl.utils import DownloadError
 
 from djtools.utils.url_download import fix_up, url_download
 
@@ -26,34 +26,35 @@
         (
             "Some Artist - Some Track.mp3",
             "Some Track - Some Artist.mp3",
         ),
     ],
 )
 def test_fix_up(test_assets):
-    test_file, expected_clean_file = test_assets
+    test_file, expected_clean_file = map(Path, test_assets)
     clean_file = fix_up(test_file)
     assert clean_file == expected_clean_file
 
 
 def test_url_download(tmpdir, test_config):
+    tmpdir = Path(tmpdir)
     test_config.URL_DOWNLOAD = (
         "https://soundcloud.com/aweeeezy_music/sets/test-download"
     )
     test_config.URL_DOWNLOAD_DESTINATION = tmpdir
     with mock.patch(
         "youtube_dl.YoutubeDL",
     ) as mock_ytdl:
         context = mock_ytdl.return_value.__enter__.return_value 
         context.download.side_effect = lambda *args, **kwargs: open(
-            os.path.join(tmpdir, "file.mp3").replace(os.sep, "/"),
+            tmpdir / "file.mp3",
             mode="w",
             encoding="utf-8",
         ).write("")
         url_download(test_config)
-    assert len(os.listdir(tmpdir)) == 1
+    assert len(list(tmpdir.iterdir())) == 1
 
 
 def test_url_download_invalid_url(test_config):
     test_config.URL_DOWNLOAD = ""
     with pytest.raises(DownloadError):
         url_download(test_config)
```

### Comparing `dj_beatcloud-2.4.1b2/src/djtools/utils/url_download.py` & `dj_beatcloud-2.4.1b3/src/djtools/utils/url_download.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,59 @@
 """This module is used to download tracks from "URL_DOWNLOAD". For example, a
 Soundcloud playlist can be made and the URL of that playlist can be provided to
 download all those tracks and rename them to cleanup the digits appended to the
 files by the youtube-dl package.
 """
 import logging
-import os
+from pathlib import Path
 import re
 
 import youtube_dl as ytdl
 
 from djtools.configs.config import BaseConfig
-from djtools.utils.helpers import make_dirs
 
 
 logger = logging.getLogger(__name__)
 
 
-def fix_up(_file: str) -> str:
+def fix_up(_file: Path) -> Path:
     """Removes digits appended to file name by youtube-dl.
 
     Args:
         _file: Music file name.
 
     Returns:
         Cleaned up music file name.
     """
-    _, ext = os.path.splitext(_file)
+    ext = _file.suffix
     exp = fr"(\-\d{{1,}}(?={ext}))"
-    stripped = os.path.splitext(re.split(exp, _file)[0])[0]
-    name = " - ".join(stripped.split(" - ")[-1::-1])
+    stripped = Path(re.split(exp, _file.as_posix())[0]).stem
+    name = Path(" - ".join(stripped.split(" - ")[-1::-1]))
 
-    return name + ext
+    return name.with_suffix(ext)
 
 
 def url_download(config: BaseConfig):
     """Downloads music files from a provided URL using the youtube-dl package.
 
     Args:
         config: Configuration object.
     """
-    dl_loc = config.URL_DOWNLOAD_DESTINATION or "."
-    dl_loc = os.path.join(dl_loc, "").replace(os.sep, "/")
-    make_dirs(dl_loc)
+    dl_loc = config.URL_DOWNLOAD_DESTINATION or Path(".")
+    dl_loc.mkdir(parents=True, exist_ok=True)
 
     ydl_opts = {
         "format": "bestaudio/best",
         "postprocessors": [{
             "key": "FFmpegExtractAudio",
             "preferredcodec": "mp3",
             "preferredquality": "320",
         }],
-        "outtmpl": dl_loc + "%(title)s.%(ext)s"
+        "outtmpl": dl_loc / "%(title)s.%(ext)s"
     }
 
     with ytdl.YoutubeDL(ydl_opts) as ydl:
         logger.info(f"Downloading {config.URL_DOWNLOAD} to {dl_loc}")
         ydl.download([config.URL_DOWNLOAD])
 
-    for _file in os.listdir(dl_loc):
-        os.rename(
-            os.path.join(dl_loc, _file).replace(os.sep, "/"),
-            os.path.join(dl_loc, fix_up(_file)).replace(os.sep, "/"),
-        )
+    for _file in dl_loc.iterdir():
+        (dl_loc / _file).rename(dl_loc / fix_up(_file))
```

### Comparing `dj_beatcloud-2.4.1b2/src/test_data/conftest.py` & `dj_beatcloud-2.4.1b3/src/test_data/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,26 +7,20 @@
 
 import pytest
 
 from djtools.configs.config import BaseConfig
 from djtools.configs.helpers import filter_dict, pkg_cfg
 
 
-class MockExists:
-    os_exists = os.path.exists
+def mock_exists(files, path):
+    for file_name, exists in files:
+        if file_name == path.name:
+            return exists
 
-    def __init__(self, files: List[Tuple[str, bool]]):
-        self._files = files
-
-    def exists(self, *args, **kwargs):
-        file_name = os.path.basename(args[0])
-        for file_, exists in self._files:
-            if file_name == file_:
-                return exists
-        return True
+    return True
 
     
 class MockOpen:
     builtin_open = open
 
     def __init__(
         self,
```

