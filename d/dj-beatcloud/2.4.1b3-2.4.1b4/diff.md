# Comparing `tmp/dj_beatcloud-2.4.1b3.tar.gz` & `tmp/dj_beatcloud-2.4.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_beatcloud-2.4.1b3.tar", last modified: Wed Apr 12 23:26:05 2023, max compression
+gzip compressed data, was "dj_beatcloud-2.4.1b4.tar", last modified: Thu Apr 13 17:08:19 2023, max compression
```

## Comparing `dj_beatcloud-2.4.1b3.tar` & `dj_beatcloud-2.4.1b4.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-12 23:26:05.578379 dj_beatcloud-2.4.1b3/
--rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.4.1b3/LICENSE
--rw-r--r--   0 alrichards   (502) staff       (20)       64 2022-06-16 01:40:44.000000 dj_beatcloud-2.4.1b3/MANIFEST.in
--rw-r--r--   0 alrichards   (502) staff       (20)    29508 2023-04-12 23:26:05.578517 dj_beatcloud-2.4.1b3/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)    28223 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/README.md
--rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/pyproject.toml
--rw-r--r--   0 alrichards   (502) staff       (20)      164 2023-04-12 23:26:05.578978 dj_beatcloud-2.4.1b3/setup.cfg
--rw-r--r--   0 alrichards   (502) staff       (20)     2225 2023-04-12 23:24:14.000000 dj_beatcloud-2.4.1b3/setup.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-12 23:26:05.560863 dj_beatcloud-2.4.1b3/src/
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-12 23:26:05.563271 dj_beatcloud-2.4.1b3/src/dj_beatcloud.egg-info/
--rw-r--r--   0 alrichards   (502) staff       (20)    29508 2023-04-12 23:26:05.000000 dj_beatcloud-2.4.1b3/src/dj_beatcloud.egg-info/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     2193 2023-04-12 23:26:05.000000 dj_beatcloud-2.4.1b3/src/dj_beatcloud.egg-info/SOURCES.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-04-12 23:26:05.000000 dj_beatcloud-2.4.1b3/src/dj_beatcloud.egg-info/dependency_links.txt
--rw-r--r--   0 alrichards   (502) staff       (20)       50 2023-04-12 23:26:05.000000 dj_beatcloud-2.4.1b3/src/dj_beatcloud.egg-info/entry_points.txt
--rw-r--r--   0 alrichards   (502) staff       (20)      332 2023-04-12 23:26:05.000000 dj_beatcloud-2.4.1b3/src/dj_beatcloud.egg-info/requires.txt
--rw-r--r--   0 alrichards   (502) staff       (20)       18 2023-04-12 23:26:05.000000 dj_beatcloud-2.4.1b3/src/dj_beatcloud.egg-info/top_level.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-12 23:26:05.564167 dj_beatcloud-2.4.1b3/src/djtools/
--rw-r--r--   0 alrichards   (502) staff       (20)      966 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b3/src/djtools/__init__.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-12 23:26:05.566842 dj_beatcloud-2.4.1b3/src/djtools/configs/
--rw-r--r--   0 alrichards   (502) staff       (20)     6148 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b3/src/djtools/configs/.DS_Store
--rw-r--r--   0 alrichards   (502) staff       (20)     4258 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b3/src/djtools/configs/README.md
--rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b3/src/djtools/configs/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3113 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/configs/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1223 2023-03-09 22:09:23.000000 dj_beatcloud-2.4.1b3/src/djtools/configs/config.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)    13418 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/configs/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b3/src/djtools/configs/logging.conf
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-04-12 15:31:08.000000 dj_beatcloud-2.4.1b3/src/djtools/configs/registered_users.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)      878 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/configs/rekordbox_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-03-09 22:09:23.000000 dj_beatcloud-2.4.1b3/src/djtools/configs/spotify_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)     2305 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/configs/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4478 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/configs/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1721 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b3/src/djtools/dj_tools.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-12 23:26:05.567112 dj_beatcloud-2.4.1b3/src/djtools/logs/
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2022-06-16 01:40:44.000000 dj_beatcloud-2.4.1b3/src/djtools/logs/empty.txt
--rw-r--r--   0 alrichards   (502) staff       (20)     1649 2023-03-16 00:56:47.000000 dj_beatcloud-2.4.1b3/src/djtools/main.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-12 23:26:05.570397 dj_beatcloud-2.4.1b3/src/djtools/rekordbox/
--rw-r--r--   0 alrichards   (502) staff       (20)     1360 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b3/src/djtools/rekordbox/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1794 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/rekordbox/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4123 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/rekordbox/copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4521 2023-04-12 23:23:56.000000 dj_beatcloud-2.4.1b3/src/djtools/rekordbox/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)    18868 2023-04-12 23:23:56.000000 dj_beatcloud-2.4.1b3/src/djtools/rekordbox/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2859 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/rekordbox/randomize_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)    13303 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/rekordbox/tag_parsers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1225 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/rekordbox/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1390 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/rekordbox/test_copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2807 2023-04-12 23:23:56.000000 dj_beatcloud-2.4.1b3/src/djtools/rekordbox/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5142 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/rekordbox/test_playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1477 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/rekordbox/test_randomize_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3975 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/rekordbox/test_tag_parsers.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-12 23:26:05.572653 dj_beatcloud-2.4.1b3/src/djtools/spotify/
--rw-r--r--   0 alrichards   (502) staff       (20)      718 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b3/src/djtools/spotify/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3229 2023-03-09 18:55:21.000000 dj_beatcloud-2.4.1b3/src/djtools/spotify/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    15361 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/spotify/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6155 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/spotify/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1958 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b3/src/djtools/spotify/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    17499 2023-03-17 15:21:16.000000 dj_beatcloud-2.4.1b3/src/djtools/spotify/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6153 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/spotify/test_playlist_builder.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-12 23:26:05.575380 dj_beatcloud-2.4.1b3/src/djtools/sync/
--rw-r--r--   0 alrichards   (502) staff       (20)      772 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b3/src/djtools/sync/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3899 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/sync/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8237 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/sync/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4605 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/sync/sync_operations.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3282 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/sync/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     7496 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/sync/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4520 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/sync/test_sync_operations.py
--rw-r--r--   0 alrichards   (502) staff       (20)      830 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/test_main.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-12 23:26:05.577747 dj_beatcloud-2.4.1b3/src/djtools/utils/
--rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b3/src/djtools/utils/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3488 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/utils/check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1093 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/utils/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     7888 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/utils/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3227 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/utils/test_check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)      397 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b3/src/djtools/utils/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8500 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/utils/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1580 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/utils/test_url_download.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1641 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/djtools/utils/url_download.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-12 23:26:05.578220 dj_beatcloud-2.4.1b3/src/test_data/
--rw-r--r--   0 alrichards   (502) staff       (20)      138 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/test_data/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3547 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b3/src/test_data/conftest.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-13 17:08:19.237205 dj_beatcloud-2.4.1b4/
+-rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.4.1b4/LICENSE
+-rw-r--r--   0 alrichards   (502) staff       (20)       64 2022-06-16 01:40:44.000000 dj_beatcloud-2.4.1b4/MANIFEST.in
+-rw-r--r--   0 alrichards   (502) staff       (20)    29508 2023-04-13 17:08:19.237333 dj_beatcloud-2.4.1b4/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)    28223 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/README.md
+-rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/pyproject.toml
+-rw-r--r--   0 alrichards   (502) staff       (20)      164 2023-04-13 17:08:19.237628 dj_beatcloud-2.4.1b4/setup.cfg
+-rw-r--r--   0 alrichards   (502) staff       (20)     2225 2023-04-13 15:48:53.000000 dj_beatcloud-2.4.1b4/setup.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-13 17:08:19.220504 dj_beatcloud-2.4.1b4/src/
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-13 17:08:19.222709 dj_beatcloud-2.4.1b4/src/dj_beatcloud.egg-info/
+-rw-r--r--   0 alrichards   (502) staff       (20)    29508 2023-04-13 17:08:19.000000 dj_beatcloud-2.4.1b4/src/dj_beatcloud.egg-info/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     2193 2023-04-13 17:08:19.000000 dj_beatcloud-2.4.1b4/src/dj_beatcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-04-13 17:08:19.000000 dj_beatcloud-2.4.1b4/src/dj_beatcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)       50 2023-04-13 17:08:19.000000 dj_beatcloud-2.4.1b4/src/dj_beatcloud.egg-info/entry_points.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)      332 2023-04-13 17:08:19.000000 dj_beatcloud-2.4.1b4/src/dj_beatcloud.egg-info/requires.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)       18 2023-04-13 17:08:19.000000 dj_beatcloud-2.4.1b4/src/dj_beatcloud.egg-info/top_level.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-13 17:08:19.224135 dj_beatcloud-2.4.1b4/src/djtools/
+-rw-r--r--   0 alrichards   (502) staff       (20)      966 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b4/src/djtools/__init__.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-13 17:08:19.227567 dj_beatcloud-2.4.1b4/src/djtools/configs/
+-rw-r--r--   0 alrichards   (502) staff       (20)     6148 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b4/src/djtools/configs/.DS_Store
+-rw-r--r--   0 alrichards   (502) staff       (20)     4258 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b4/src/djtools/configs/README.md
+-rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b4/src/djtools/configs/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3103 2023-04-13 16:23:56.000000 dj_beatcloud-2.4.1b4/src/djtools/configs/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1223 2023-03-09 22:09:23.000000 dj_beatcloud-2.4.1b4/src/djtools/configs/config.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)    13418 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/configs/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-03-09 22:06:36.000000 dj_beatcloud-2.4.1b4/src/djtools/configs/logging.conf
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-04-13 16:51:43.000000 dj_beatcloud-2.4.1b4/src/djtools/configs/registered_users.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)      878 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/configs/rekordbox_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-03-09 22:09:23.000000 dj_beatcloud-2.4.1b4/src/djtools/configs/spotify_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)     2305 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/configs/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4478 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/configs/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1721 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b4/src/djtools/dj_tools.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-13 17:08:19.227754 dj_beatcloud-2.4.1b4/src/djtools/logs/
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2022-06-16 01:40:44.000000 dj_beatcloud-2.4.1b4/src/djtools/logs/empty.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)     1649 2023-03-16 00:56:47.000000 dj_beatcloud-2.4.1b4/src/djtools/main.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-13 17:08:19.231027 dj_beatcloud-2.4.1b4/src/djtools/rekordbox/
+-rw-r--r--   0 alrichards   (502) staff       (20)     1360 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b4/src/djtools/rekordbox/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1794 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/rekordbox/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4123 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/rekordbox/copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4521 2023-04-12 23:23:56.000000 dj_beatcloud-2.4.1b4/src/djtools/rekordbox/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    18868 2023-04-12 23:23:56.000000 dj_beatcloud-2.4.1b4/src/djtools/rekordbox/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2859 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/rekordbox/randomize_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    13303 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/rekordbox/tag_parsers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1225 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/rekordbox/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1390 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/rekordbox/test_copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2807 2023-04-12 23:23:56.000000 dj_beatcloud-2.4.1b4/src/djtools/rekordbox/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5142 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/rekordbox/test_playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1477 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/rekordbox/test_randomize_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3975 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/rekordbox/test_tag_parsers.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-13 17:08:19.232927 dj_beatcloud-2.4.1b4/src/djtools/spotify/
+-rw-r--r--   0 alrichards   (502) staff       (20)      718 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b4/src/djtools/spotify/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3229 2023-03-09 18:55:21.000000 dj_beatcloud-2.4.1b4/src/djtools/spotify/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    15361 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/spotify/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6155 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/spotify/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1958 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b4/src/djtools/spotify/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    17499 2023-03-17 15:21:16.000000 dj_beatcloud-2.4.1b4/src/djtools/spotify/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6153 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/spotify/test_playlist_builder.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-13 17:08:19.234632 dj_beatcloud-2.4.1b4/src/djtools/sync/
+-rw-r--r--   0 alrichards   (502) staff       (20)      772 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b4/src/djtools/sync/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4706 2023-04-13 16:50:12.000000 dj_beatcloud-2.4.1b4/src/djtools/sync/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     8237 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/sync/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4605 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/sync/sync_operations.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4038 2023-04-13 16:51:38.000000 dj_beatcloud-2.4.1b4/src/djtools/sync/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     7496 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/sync/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4520 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/sync/test_sync_operations.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      830 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/test_main.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-13 17:08:19.236600 dj_beatcloud-2.4.1b4/src/djtools/utils/
+-rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b4/src/djtools/utils/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3488 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/utils/check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1093 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/utils/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     7904 2023-04-13 15:40:43.000000 dj_beatcloud-2.4.1b4/src/djtools/utils/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3227 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/utils/test_check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      397 2023-01-13 18:19:45.000000 dj_beatcloud-2.4.1b4/src/djtools/utils/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     8533 2023-04-13 15:45:33.000000 dj_beatcloud-2.4.1b4/src/djtools/utils/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1580 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/utils/test_url_download.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1641 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/djtools/utils/url_download.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-04-13 17:08:19.237029 dj_beatcloud-2.4.1b4/src/test_data/
+-rw-r--r--   0 alrichards   (502) staff       (20)      138 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/test_data/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3547 2023-04-12 22:29:30.000000 dj_beatcloud-2.4.1b4/src/test_data/conftest.py
```

### Comparing `dj_beatcloud-2.4.1b3/LICENSE` & `dj_beatcloud-2.4.1b4/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/PKG-INFO` & `dj_beatcloud-2.4.1b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj_beatcloud
-Version: 2.4.1b3
+Version: 2.4.1b4
 Summary: DJ Tools is a library for managing a collection of music and Rekordbox XML files.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 License: GNU GPLv3
 Keywords: MP3 Rekordbox XML spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dj_beatcloud-2.4.1b3/README.md` & `dj_beatcloud-2.4.1b4/README.md`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/setup.py` & `dj_beatcloud-2.4.1b4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 EXTRAS = {
         'levenshtein': ['python-Levenshtein==0.12.2']
 }
 
 setup(
     name='dj_beatcloud',
-    version='2.4.1-b3',
+    version='2.4.1-b4',
     description=(
         'DJ Tools is a library for managing a collection of music and '
         'Rekordbox XML files.'
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url='https://github.com/a-rich/DJ-tools',
```

### Comparing `dj_beatcloud-2.4.1b3/src/dj_beatcloud.egg-info/PKG-INFO` & `dj_beatcloud-2.4.1b4/src/dj_beatcloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-beatcloud
-Version: 2.4.1b3
+Version: 2.4.1b4
 Summary: DJ Tools is a library for managing a collection of music and Rekordbox XML files.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 License: GNU GPLv3
 Keywords: MP3 Rekordbox XML spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dj_beatcloud-2.4.1b3/src/dj_beatcloud.egg-info/SOURCES.txt` & `dj_beatcloud-2.4.1b4/src/dj_beatcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/__init__.py` & `dj_beatcloud-2.4.1b4/src/djtools/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/configs/.DS_Store` & `dj_beatcloud-2.4.1b4/src/djtools/configs/.DS_Store`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/configs/README.md` & `dj_beatcloud-2.4.1b4/src/djtools/configs/README.md`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/configs/config.py` & `dj_beatcloud-2.4.1b4/src/djtools/configs/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 apply to multiple packages. The attributes of this configuration object
 correspond with the "configs" key of config.yaml."""
 import logging
 import os
 from pathlib import Path
 from typing_extensions import Literal
 
-from pydantic import BaseModel, Extra, NonNegativeInt, validator
+from pydantic import BaseModel, Extra, NonNegativeInt 
 
 
 logger = logging.getLogger(__name__)
 
 
 class BaseConfig(BaseModel, extra=Extra.allow):
     """Base configuration object used across the whole library."""
```

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/configs/config.yaml` & `dj_beatcloud-2.4.1b4/src/djtools/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/configs/helpers.py` & `dj_beatcloud-2.4.1b4/src/djtools/configs/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/configs/rekordbox_playlists.yaml` & `dj_beatcloud-2.4.1b4/src/djtools/configs/rekordbox_playlists.yaml`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/configs/test_config.py` & `dj_beatcloud-2.4.1b4/src/djtools/configs/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/configs/test_helpers.py` & `dj_beatcloud-2.4.1b4/src/djtools/configs/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/dj_tools.py` & `dj_beatcloud-2.4.1b4/src/djtools/dj_tools.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/main.py` & `dj_beatcloud-2.4.1b4/src/djtools/main.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/rekordbox/__init__.py` & `dj_beatcloud-2.4.1b4/src/djtools/rekordbox/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/rekordbox/config.py` & `dj_beatcloud-2.4.1b4/src/djtools/rekordbox/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/rekordbox/copy_playlists.py` & `dj_beatcloud-2.4.1b4/src/djtools/rekordbox/copy_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/rekordbox/helpers.py` & `dj_beatcloud-2.4.1b4/src/djtools/rekordbox/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/rekordbox/playlist_builder.py` & `dj_beatcloud-2.4.1b4/src/djtools/rekordbox/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/rekordbox/randomize_playlists.py` & `dj_beatcloud-2.4.1b4/src/djtools/rekordbox/randomize_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/rekordbox/tag_parsers.py` & `dj_beatcloud-2.4.1b4/src/djtools/rekordbox/tag_parsers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/rekordbox/test_config.py` & `dj_beatcloud-2.4.1b4/src/djtools/rekordbox/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/rekordbox/test_copy_playlists.py` & `dj_beatcloud-2.4.1b4/src/djtools/rekordbox/test_copy_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/rekordbox/test_helpers.py` & `dj_beatcloud-2.4.1b4/src/djtools/rekordbox/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/rekordbox/test_playlist_builder.py` & `dj_beatcloud-2.4.1b4/src/djtools/rekordbox/test_playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/rekordbox/test_randomize_playlists.py` & `dj_beatcloud-2.4.1b4/src/djtools/rekordbox/test_randomize_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/rekordbox/test_tag_parsers.py` & `dj_beatcloud-2.4.1b4/src/djtools/rekordbox/test_tag_parsers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/spotify/__init__.py` & `dj_beatcloud-2.4.1b4/src/djtools/spotify/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/spotify/config.py` & `dj_beatcloud-2.4.1b4/src/djtools/spotify/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/spotify/helpers.py` & `dj_beatcloud-2.4.1b4/src/djtools/spotify/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/spotify/playlist_builder.py` & `dj_beatcloud-2.4.1b4/src/djtools/spotify/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/spotify/test_config.py` & `dj_beatcloud-2.4.1b4/src/djtools/spotify/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/spotify/test_helpers.py` & `dj_beatcloud-2.4.1b4/src/djtools/spotify/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/spotify/test_playlist_builder.py` & `dj_beatcloud-2.4.1b4/src/djtools/spotify/test_playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/sync/__init__.py` & `dj_beatcloud-2.4.1b4/src/djtools/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/sync/config.py` & `dj_beatcloud-2.4.1b4/src/djtools/sync/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """This module contains the configuration object for the sync package.
 The attributes of this configuration object correspond with the "sync" key
 of config.yaml
 """
 import getpass
 import logging
 from pathlib import Path
-from typing import Dict, List
+from typing import List, Union
 
+from pydantic import validator
 import yaml
 
 from djtools.configs.config import BaseConfig
 
 
 logger = logging.getLogger(__name__)
 
@@ -27,15 +28,15 @@
     DOWNLOAD_XML: bool = False 
     DRYRUN: bool = False
     IMPORT_USER: str = ""
     UPLOAD_EXCLUDE_DIRS: List[Path] = []
     UPLOAD_INCLUDE_DIRS: List[Path] = []
     UPLOAD_MUSIC: bool = False 
     UPLOAD_XML: bool = False 
-    USB_PATH: Path = None
+    USB_PATH: str = ""
     USER: str = ""
 
     def __init__(self, *args, **kwargs):
         """Constructor.
 
         Raises:
             ValueError: Both include and exclude dirs can't be provided at the
@@ -70,14 +71,28 @@
             ]
         ):
             if not self.AWS_PROFILE:
                 msg = "Config must include AWS_PROFILE for sync operations"
                 logger.critical(msg)
                 raise RuntimeError(msg)
         
+        if (
+            any([self.DOWNLOAD_MUSIC, self.UPLOAD_MUSIC]) and not
+            (
+                self.USB_PATH if isinstance(self.USB_PATH, str)
+                else self.USB_PATH.exists()
+            )
+        ):
+            msg = (
+                "Config must include USB_PATH for both DOWNLOAD_MUSIC and "
+                "UPLOAD_MUSIC sync operations"
+            )
+            logger.critical(msg)
+            raise RuntimeError(msg)
+        
         if self.UPLOAD_MUSIC and not self.DISCORD_URL:
             logger.warning(
                 'DISCORD_URL is not configured...set this for "New Music" '
                 "discord messages!"
             )
 
         registered_users_path = (
@@ -108,10 +123,22 @@
         ):
             raise RuntimeError(
                 "Unable to import from XML of unregistered IMPORT_USER "
                 f'"{self.IMPORT_USER}"'
             )
 
         # Enter USER into "registered_users.yaml".
-        registered_users[self.USER] = self.USB_PATH
+        registered_users[self.USER] = str(self.USB_PATH)
         with open(registered_users_path, mode="w", encoding="utf-8") as _file:
             yaml.dump(registered_users, _file)
+
+    @validator("USB_PATH")
+    def usb_path_as_pathlib_path(cls, v: str) -> Union[Path, str]:
+        """_summary_
+
+        Args:
+            v: USB_PATH field
+
+        Returns:
+            pathlib.Path representing the USB_PATH field or else an empty string.
+        """
+        return v if not v else Path(v)
```

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/sync/helpers.py` & `dj_beatcloud-2.4.1b4/src/djtools/sync/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/sync/sync_operations.py` & `dj_beatcloud-2.4.1b4/src/djtools/sync/sync_operations.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/sync/test_config.py` & `dj_beatcloud-2.4.1b4/src/djtools/sync/test_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,14 +25,39 @@
     with pytest.raises(
         RuntimeError,
         match="Error reading registered_users.yaml",
     ):
         SyncConfig()
 
 
+@mock.patch(
+    "builtins.open",
+    MockOpen(files=["registered_users.yaml"],
+    write_only=True).open,
+)
+@pytest.mark.parametrize("operations", [(True, False), (False, True)])
+@pytest.mark.parametrize("usb_path", ["", "nonexistent/path"])
+def test_syncconfig_download_or_upload_without_usb_path(operations, usb_path):
+    download, upload = operations
+    cfg = {
+        "AWS_PROFILE": "myprofile",
+        "DOWNLOAD_MUSIC": download,
+        "UPLOAD_MUSIC": upload,
+        "USB_PATH": usb_path,
+    }
+    with pytest.raises(
+        RuntimeError,
+        match=(
+            "Config must include USB_PATH for both DOWNLOAD_MUSIC and "
+            "UPLOAD_MUSIC sync operations"
+        ),
+    ):
+        SyncConfig(**cfg)
+
+
 def test_syncconfig_download_without_import_user():
     cfg = {
         "DOWNLOAD_XML": True,
         "AWS_PROFILE": "myprofile",
         "IMPORT_USER": "not a valid user",
     }
     with pytest.raises(
@@ -111,14 +136,15 @@
 )
 @mock.patch("djtools.spotify.helpers.get_spotify_client")
 def test_syncconfig_upload_without_discord_url(
     mock_get_spotify_client, test_xml, caplog
 ):
     caplog.set_level("WARNING")
     cfg = {
+        "USB_PATH": ".",
         "UPLOAD_MUSIC": True,
         "DISCORD_URL": "",
         "XML_PATH": test_xml,
         "SPOTIFY_CLIENT_ID": "id",
         "SPOTIFY_CLIENT_SECRET": "secret",
         "SPOTIFY_REDIRECT_URI": "uri",
         "SPOTIFY_USERNAME": "name",
```

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/sync/test_helpers.py` & `dj_beatcloud-2.4.1b4/src/djtools/sync/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/sync/test_sync_operations.py` & `dj_beatcloud-2.4.1b4/src/djtools/sync/test_sync_operations.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/test_main.py` & `dj_beatcloud-2.4.1b4/src/djtools/test_main.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/utils/__init__.py` & `dj_beatcloud-2.4.1b4/src/djtools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/utils/check_tracks.py` & `dj_beatcloud-2.4.1b4/src/djtools/utils/check_tracks.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/utils/config.py` & `dj_beatcloud-2.4.1b4/src/djtools/utils/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/utils/helpers.py` & `dj_beatcloud-2.4.1b4/src/djtools/utils/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         artist names.
     
     Returns:
         Beatcloud track titles and artist names.
     """
     logger.info("Getting tracks from the beatcloud...")
     cmd = "aws s3 ls --recursive s3://dj.beatcloud.com/dj/music/"
-    output = check_output(cmd, shell=True).split("\n")
+    output = check_output(cmd, shell=True).decode("utf-8").split("\n")
     tracks = [Path(track) for track in output if track]
     logger.info(f"Got {len(tracks)} tracks")
 
     return tracks
 
 
 def get_local_tracks(config: BaseConfig) -> Dict[str, List[str]]:
```

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/utils/test_check_tracks.py` & `dj_beatcloud-2.4.1b4/src/djtools/utils/test_check_tracks.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/utils/test_helpers.py` & `dj_beatcloud-2.4.1b4/src/djtools/utils/test_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,17 @@
             "aweeeezy/Techno/2022-12-21/track - artist.mp3",
         ]
     ]
 )
 @mock.patch("djtools.utils.helpers.check_output")
 def test_get_beatcloud_tracks(mock_os_popen, proc_dump):
     proc_dump = list(map(Path, proc_dump))
-    process = mock_os_popen.return_value = "\n".join(map(Path.as_posix, proc_dump))
+    process = mock_os_popen.return_value = b"\n".join(
+        map(lambda x: x.as_posix().encode(), proc_dump)
+    )
     tracks = get_beatcloud_tracks()
     mock_os_popen.assert_called_once()
     assert len(tracks) == len(proc_dump)
     for track, line in zip(tracks, proc_dump):
         assert track == line
```

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/utils/test_url_download.py` & `dj_beatcloud-2.4.1b4/src/djtools/utils/test_url_download.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/djtools/utils/url_download.py` & `dj_beatcloud-2.4.1b4/src/djtools/utils/url_download.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.4.1b3/src/test_data/conftest.py` & `dj_beatcloud-2.4.1b4/src/test_data/conftest.py`

 * *Files identical despite different names*

