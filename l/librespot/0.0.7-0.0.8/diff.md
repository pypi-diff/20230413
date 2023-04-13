# Comparing `tmp/librespot-0.0.7.tar.gz` & `tmp/librespot-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librespot-0.0.7.tar", last modified: Wed Nov  9 22:12:53 2022, max compression
+gzip compressed data, was "librespot-0.0.8.tar", last modified: Thu Apr 13 12:09:04 2023, max compression
```

## Comparing `librespot-0.0.7.tar` & `librespot-0.0.8.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxrwx   0        0        0        0 2022-11-09 22:12:53.549110 librespot-0.0.7/
--rw-rw-rw-   0        0        0    11572 2022-07-11 21:59:06.000000 librespot-0.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0     3988 2022-11-09 22:12:53.548591 librespot-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3561 2022-07-11 21:59:06.000000 librespot-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2022-11-09 22:12:53.466078 librespot-0.0.7/librespot/
--rw-rw-rw-   0        0        0     1168 2022-11-09 22:11:47.000000 librespot-0.0.7/librespot/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-09 22:12:53.483627 librespot-0.0.7/librespot/audio/
--rw-rw-rw-   0        0        0    36315 2022-10-07 09:50:17.000000 librespot-0.0.7/librespot/audio/__init__.py
--rw-rw-rw-   0        0        0     2897 2022-07-11 21:59:06.000000 librespot-0.0.7/librespot/audio/decoders.py
--rw-rw-rw-   0        0        0     1714 2022-07-11 21:59:06.000000 librespot-0.0.7/librespot/audio/decrypt.py
--rw-rw-rw-   0        0        0     1160 2022-07-11 21:59:06.000000 librespot-0.0.7/librespot/audio/format.py
--rw-rw-rw-   0        0        0     5621 2022-07-11 21:59:06.000000 librespot-0.0.7/librespot/audio/storage.py
--rw-rw-rw-   0        0        0      378 2022-07-11 21:59:06.000000 librespot-0.0.7/librespot/cache.py
--rw-rw-rw-   0        0        0    72485 2022-10-20 22:10:07.000000 librespot-0.0.7/librespot/core.py
--rw-rw-rw-   0        0        0    13141 2022-07-11 21:59:06.000000 librespot-0.0.7/librespot/crypto.py
--rw-rw-rw-   0        0        0      390 2022-07-11 21:59:06.000000 librespot-0.0.7/librespot/dealer.py
--rw-rw-rw-   0        0        0    14068 2022-07-11 21:59:06.000000 librespot-0.0.7/librespot/mercury.py
--rw-rw-rw-   0        0        0     8027 2022-07-11 22:35:55.000000 librespot-0.0.7/librespot/metadata.py
-drwxrwxrwx   0        0        0        0 2022-11-09 22:12:53.528454 librespot-0.0.7/librespot/proto/
--rw-rw-rw-   0        0        0    69584 2022-07-11 21:59:06.000000 librespot-0.0.7/librespot/proto/Authentication_pb2.py
--rw-rw-rw-   0        0        0     2965 2022-07-11 21:59:06.000000 librespot-0.0.7/librespot/proto/CanvazMeta_pb2.py
--rw-rw-rw-   0        0        0    19169 2022-07-11 21:59:06.000000 librespot-0.0.7/librespot/proto/Canvaz_pb2.py
--rw-rw-rw-   0        0        0     6425 2022-07-11 21:59:06.000000 librespot-0.0.7/librespot/proto/ClientToken_pb2.py
--rw-rw-rw-   0        0        0    83348 2022-07-11 21:59:06.000000 librespot-0.0.7/librespot/proto/Connect_pb2.py
--rw-rw-rw-   0        0        0     3061 2022-07-11 21:59:06.000000 librespot-0.0.7/librespot/proto/Connectivity_pb2.py
--rw-rw-rw-   0        0        0     8152 2022-07-11 21:59:06.000000 librespot-0.0.7/librespot/proto/ContextPage_pb2.py
--rw-rw-rw-   0        0        0     7395 2022-07-11 21:59:06.000000 librespot-0.0.7/librespot/proto/ContextPlayerOptions_pb2.py
--rw-rw-rw-   0        0        0     7197 2022-07-11 21:59:06.000000 librespot-0.0.7/librespot/proto/ContextTrack_pb2.py
--rw-rw-rw-   0        0        0     8845 2022-07-11 21:59:06.000000 librespot-0.0.7/librespot/proto/Context_pb2.py
--rw-rw-rw-   0        0        0     5095 2022-07-11 21:59:06.000000 librespot-0.0.7/librespot/proto/ExplicitContentPubsub_pb2.py
--rw-rw-rw-   0        0        0    87983 2022-07-11 21:59:07.000000 librespot-0.0.7/librespot/proto/Keyexchange_pb2.py
--rw-rw-rw-   0        0        0    20962 2022-07-11 21:59:07.000000 librespot-0.0.7/librespot/proto/Mercury_pb2.py
--rw-rw-rw-   0        0        0   132205 2022-07-11 21:59:07.000000 librespot-0.0.7/librespot/proto/Metadata_pb2.py
--rw-rw-rw-   0        0        0     6729 2022-07-11 21:59:07.000000 librespot-0.0.7/librespot/proto/PlayOrigin_pb2.py
--rw-rw-rw-   0        0        0     5556 2022-07-11 21:59:07.000000 librespot-0.0.7/librespot/proto/Playback_pb2.py
--rw-rw-rw-   0        0        0    67514 2022-07-11 21:59:07.000000 librespot-0.0.7/librespot/proto/Player_pb2.py
--rw-rw-rw-   0        0        0   108912 2022-07-11 21:59:07.000000 librespot-0.0.7/librespot/proto/Playlist4External_pb2.py
--rw-rw-rw-   0        0        0    16084 2022-07-11 21:59:07.000000 librespot-0.0.7/librespot/proto/PlaylistAnnotate3_pb2.py
--rw-rw-rw-   0        0        0     3662 2022-07-11 21:59:07.000000 librespot-0.0.7/librespot/proto/Pubsub_pb2.py
--rw-rw-rw-   0        0        0     3413 2022-07-11 21:59:07.000000 librespot-0.0.7/librespot/proto/Queue_pb2.py
--rw-rw-rw-   0        0        0    17651 2022-07-11 21:59:07.000000 librespot-0.0.7/librespot/proto/Restrictions_pb2.py
--rw-rw-rw-   0        0        0     5352 2022-07-11 21:59:07.000000 librespot-0.0.7/librespot/proto/Session_pb2.py
--rw-rw-rw-   0        0        0     5527 2022-07-11 21:59:07.000000 librespot-0.0.7/librespot/proto/StorageResolve_pb2.py
--rw-rw-rw-   0        0        0     6353 2022-07-11 21:59:07.000000 librespot-0.0.7/librespot/proto/TransferState_pb2.py
--rw-rw-rw-   0        0        0        0 2022-07-11 21:59:07.000000 librespot-0.0.7/librespot/proto/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-09 22:12:53.530169 librespot-0.0.7/librespot/proto/spotify/
--rw-rw-rw-   0        0        0        0 2022-07-11 21:59:07.000000 librespot-0.0.7/librespot/proto/spotify/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-09 22:12:53.531220 librespot-0.0.7/librespot/proto/spotify/login5/
--rw-rw-rw-   0        0        0        0 2022-07-11 21:59:07.000000 librespot-0.0.7/librespot/proto/spotify/login5/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-09 22:12:53.535811 librespot-0.0.7/librespot/proto/spotify/login5/v3/
--rw-rw-rw-   0        0        0     3230 2022-07-11 21:59:07.000000 librespot-0.0.7/librespot/proto/spotify/login5/v3/ClientInfo_pb2.py
--rw-rw-rw-   0        0        0    35170 2022-07-11 21:59:07.000000 librespot-0.0.7/librespot/proto/spotify/login5/v3/Login5_pb2.py
--rw-rw-rw-   0        0        0     8963 2022-07-11 21:59:07.000000 librespot-0.0.7/librespot/proto/spotify/login5/v3/UserInfo_pb2.py
--rw-rw-rw-   0        0        0        0 2022-07-11 21:59:07.000000 librespot-0.0.7/librespot/proto/spotify/login5/v3/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-09 22:12:53.539198 librespot-0.0.7/librespot/proto/spotify/login5/v3/challenges/
--rw-rw-rw-   0        0        0     7597 2022-07-11 21:59:07.000000 librespot-0.0.7/librespot/proto/spotify/login5/v3/challenges/Code_pb2.py
--rw-rw-rw-   0        0        0     6086 2022-07-11 21:59:07.000000 librespot-0.0.7/librespot/proto/spotify/login5/v3/challenges/Hashcash_pb2.py
--rw-rw-rw-   0        0        0        0 2022-07-11 21:59:07.000000 librespot-0.0.7/librespot/proto/spotify/login5/v3/challenges/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-09 22:12:53.541286 librespot-0.0.7/librespot/proto/spotify/login5/v3/credentials/
--rw-rw-rw-   0        0        0    16339 2022-07-11 21:59:07.000000 librespot-0.0.7/librespot/proto/spotify/login5/v3/credentials/Credentials_pb2.py
--rw-rw-rw-   0        0        0        0 2022-07-11 21:59:07.000000 librespot-0.0.7/librespot/proto/spotify/login5/v3/credentials/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-09 22:12:53.545151 librespot-0.0.7/librespot/proto/spotify/login5/v3/identifiers/
--rw-rw-rw-   0        0        0     4132 2022-07-11 21:59:07.000000 librespot-0.0.7/librespot/proto/spotify/login5/v3/identifiers/Identifiers.py
--rw-rw-rw-   0        0        0        0 2022-07-11 21:59:07.000000 librespot-0.0.7/librespot/proto/spotify/login5/v3/identifiers/__init__.py
--rw-rw-rw-   0        0        0     2668 2022-07-11 21:59:07.000000 librespot-0.0.7/librespot/structure.py
--rw-rw-rw-   0        0        0     3876 2022-07-11 22:23:57.000000 librespot-0.0.7/librespot/util.py
--rw-rw-rw-   0        0        0    14135 2022-07-11 21:59:07.000000 librespot-0.0.7/librespot/zeroconf.py
-drwxrwxrwx   0        0        0        0 2022-11-09 22:12:53.474075 librespot-0.0.7/librespot.egg-info/
--rw-rw-rw-   0        0        0     3988 2022-11-09 22:12:53.000000 librespot-0.0.7/librespot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2156 2022-11-09 22:12:53.000000 librespot-0.0.7/librespot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-09 22:12:53.000000 librespot-0.0.7/librespot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      132 2022-11-09 22:12:53.000000 librespot-0.0.7/librespot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2022-11-09 22:12:53.000000 librespot-0.0.7/librespot.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-11-09 22:12:53.546765 librespot-0.0.7/librespot_player/
--rw-rw-rw-   0        0        0     7643 2022-07-11 21:59:07.000000 librespot-0.0.7/librespot_player/__init__.py
--rw-rw-rw-   0        0        0       42 2022-11-09 22:12:53.549110 librespot-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      820 2022-11-09 22:11:37.000000 librespot-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:09:04.835367 librespot-0.0.8/
+-rw-rw-rw-   0        0        0    11572 2023-04-12 21:59:13.000000 librespot-0.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     3988 2023-04-13 12:09:04.834296 librespot-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3561 2023-04-12 21:59:13.000000 librespot-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 12:09:04.721266 librespot-0.0.8/librespot/
+-rw-rw-rw-   0        0        0     1168 2023-04-13 12:08:08.000000 librespot-0.0.8/librespot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:09:04.746770 librespot-0.0.8/librespot/audio/
+-rw-rw-rw-   0        0        0    36315 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/audio/__init__.py
+-rw-rw-rw-   0        0        0     2897 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/audio/decoders.py
+-rw-rw-rw-   0        0        0     1714 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/audio/decrypt.py
+-rw-rw-rw-   0        0        0     1160 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/audio/format.py
+-rw-rw-rw-   0        0        0     5621 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/audio/storage.py
+-rw-rw-rw-   0        0        0      378 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/cache.py
+-rw-rw-rw-   0        0        0    73074 2023-04-12 22:00:44.000000 librespot-0.0.8/librespot/core.py
+-rw-rw-rw-   0        0        0    13141 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/crypto.py
+-rw-rw-rw-   0        0        0      390 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/dealer.py
+-rw-rw-rw-   0        0        0    14068 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/mercury.py
+-rw-rw-rw-   0        0        0     8711 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/metadata.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:09:04.807513 librespot-0.0.8/librespot/proto/
+-rw-rw-rw-   0        0        0    69584 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/Authentication_pb2.py
+-rw-rw-rw-   0        0        0     2965 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/CanvazMeta_pb2.py
+-rw-rw-rw-   0        0        0    19169 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/Canvaz_pb2.py
+-rw-rw-rw-   0        0        0     6425 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/ClientToken_pb2.py
+-rw-rw-rw-   0        0        0    83348 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/Connect_pb2.py
+-rw-rw-rw-   0        0        0     3061 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/Connectivity_pb2.py
+-rw-rw-rw-   0        0        0     8152 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/ContextPage_pb2.py
+-rw-rw-rw-   0        0        0     7395 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/ContextPlayerOptions_pb2.py
+-rw-rw-rw-   0        0        0     7197 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/ContextTrack_pb2.py
+-rw-rw-rw-   0        0        0     8845 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/Context_pb2.py
+-rw-rw-rw-   0        0        0     5095 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/ExplicitContentPubsub_pb2.py
+-rw-rw-rw-   0        0        0    87983 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/Keyexchange_pb2.py
+-rw-rw-rw-   0        0        0    20962 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/Mercury_pb2.py
+-rw-rw-rw-   0        0        0   132205 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/Metadata_pb2.py
+-rw-rw-rw-   0        0        0     6729 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/PlayOrigin_pb2.py
+-rw-rw-rw-   0        0        0     5556 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/Playback_pb2.py
+-rw-rw-rw-   0        0        0    67514 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/Player_pb2.py
+-rw-rw-rw-   0        0        0   108912 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/Playlist4External_pb2.py
+-rw-rw-rw-   0        0        0    16084 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/PlaylistAnnotate3_pb2.py
+-rw-rw-rw-   0        0        0     3662 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/Pubsub_pb2.py
+-rw-rw-rw-   0        0        0     3413 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/Queue_pb2.py
+-rw-rw-rw-   0        0        0    17651 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/Restrictions_pb2.py
+-rw-rw-rw-   0        0        0     5352 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/Session_pb2.py
+-rw-rw-rw-   0        0        0     5527 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/StorageResolve_pb2.py
+-rw-rw-rw-   0        0        0     6353 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/TransferState_pb2.py
+-rw-rw-rw-   0        0        0        0 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:09:04.809535 librespot-0.0.8/librespot/proto/spotify/
+-rw-rw-rw-   0        0        0        0 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/spotify/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:09:04.810677 librespot-0.0.8/librespot/proto/spotify/login5/
+-rw-rw-rw-   0        0        0        0 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/spotify/login5/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:09:04.818124 librespot-0.0.8/librespot/proto/spotify/login5/v3/
+-rw-rw-rw-   0        0        0     3230 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/spotify/login5/v3/ClientInfo_pb2.py
+-rw-rw-rw-   0        0        0    35170 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/spotify/login5/v3/Login5_pb2.py
+-rw-rw-rw-   0        0        0     8963 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/spotify/login5/v3/UserInfo_pb2.py
+-rw-rw-rw-   0        0        0        0 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/spotify/login5/v3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:09:04.823603 librespot-0.0.8/librespot/proto/spotify/login5/v3/challenges/
+-rw-rw-rw-   0        0        0     7597 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/spotify/login5/v3/challenges/Code_pb2.py
+-rw-rw-rw-   0        0        0     6086 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/spotify/login5/v3/challenges/Hashcash_pb2.py
+-rw-rw-rw-   0        0        0        0 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/spotify/login5/v3/challenges/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:09:04.827207 librespot-0.0.8/librespot/proto/spotify/login5/v3/credentials/
+-rw-rw-rw-   0        0        0    16339 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/spotify/login5/v3/credentials/Credentials_pb2.py
+-rw-rw-rw-   0        0        0        0 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/spotify/login5/v3/credentials/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:09:04.831175 librespot-0.0.8/librespot/proto/spotify/login5/v3/identifiers/
+-rw-rw-rw-   0        0        0     4132 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/spotify/login5/v3/identifiers/Identifiers.py
+-rw-rw-rw-   0        0        0        0 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/proto/spotify/login5/v3/identifiers/__init__.py
+-rw-rw-rw-   0        0        0     2668 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/structure.py
+-rw-rw-rw-   0        0        0     3876 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/util.py
+-rw-rw-rw-   0        0        0    14135 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot/zeroconf.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:09:04.735839 librespot-0.0.8/librespot.egg-info/
+-rw-rw-rw-   0        0        0     3988 2023-04-13 12:09:04.000000 librespot-0.0.8/librespot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2156 2023-04-13 12:09:04.000000 librespot-0.0.8/librespot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 12:09:04.000000 librespot-0.0.8/librespot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      130 2023-04-13 12:09:04.000000 librespot-0.0.8/librespot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-04-13 12:09:04.000000 librespot-0.0.8/librespot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 12:09:04.832256 librespot-0.0.8/librespot_player/
+-rw-rw-rw-   0        0        0     7643 2023-04-12 21:59:13.000000 librespot-0.0.8/librespot_player/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-04-13 12:09:04.835888 librespot-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      820 2023-04-13 12:08:08.000000 librespot-0.0.8/setup.py
```

### Comparing `librespot-0.0.7/LICENSE.txt` & `librespot-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/PKG-INFO` & `librespot-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: librespot
-Version: 0.0.7
+Version: 0.0.8
 Summary: Open Source Spotify Client
 Home-page: https://github.com/kokarare1212/librespot-python
 Author: kokarare1212
 License: Apache-2.0
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Multimedia :: Sound/Audio
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: librespot Version: 0.0.7 Summary: Open Source
+Metadata-Version: 2.1 Name: librespot Version: 0.0.8 Summary: Open Source
 Spotify Client Home-page: https://github.com/kokarare1212/librespot-python
 Author: kokarare1212 License: Apache-2.0 Classifier: Development Status :: 1 -
 Planning Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Multimedia :: Sound/Audio Description-Content-Type: text/
 markdown License-File: LICENSE.txt ![License](https://img.shields.io/github/
 license/kokarare1212/librespot-python.svg) ![Stars](https://img.shields.io/
 github/stars/kokarare1212/librespot-python.svg) ![Forks](https://
```

### Comparing `librespot-0.0.7/README.md` & `librespot-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/__init__.py` & `librespot-0.0.8/librespot/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from librespot.crypto import DiffieHellman
 from librespot.proto.Keyexchange_pb2 import BuildInfo, Platform, Product, ProductFlags
 from librespot.structure import Closeable, Runnable
 import platform
 
 
 class Version:
-    version_name = "0.0.7"
+    version_name = "0.0.8"
 
     @staticmethod
     def platform() -> Platform:
         if platform.system() == "Windows":
             return Platform.PLATFORM_WIN32_X86
         if platform.system() == "Darwin":
             return Platform.PLATFORM_OSX_X86
```

### Comparing `librespot-0.0.7/librespot/audio/__init__.py` & `librespot-0.0.8/librespot/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/audio/decoders.py` & `librespot-0.0.8/librespot/audio/decoders.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/audio/decrypt.py` & `librespot-0.0.8/librespot/audio/decrypt.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/audio/format.py` & `librespot-0.0.8/librespot/audio/format.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/audio/storage.py` & `librespot-0.0.8/librespot/audio/storage.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/core.py` & `librespot-0.0.8/librespot/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from Cryptodome.Signature import PKCS1_v1_5
 from librespot import util, Version
 from librespot.audio import AudioKeyManager, CdnManager, PlayableContentFeeder
 from librespot.audio.storage import ChannelManager
 from librespot.cache import CacheManager
 from librespot.crypto import CipherPair, DiffieHellman, Packet
 from librespot.mercury import MercuryClient, MercuryRequests, RawMercuryRequest
-from librespot.metadata import AlbumId, ArtistId, EpisodeId, ShowId, TrackId
-from librespot.proto import Authentication_pb2 as Authentication, ClientToken_pb2 as ClientToken, Connect_pb2 as Connect, Connectivity_pb2 as Connectivity, Keyexchange_pb2 as Keyexchange, Metadata_pb2 as Metadata
+from librespot.metadata import AlbumId, ArtistId, EpisodeId, ShowId, TrackId, PlaylistId
+from librespot.proto import Authentication_pb2 as Authentication, ClientToken_pb2 as ClientToken, Connect_pb2 as Connect, Connectivity_pb2 as Connectivity, Keyexchange_pb2 as Keyexchange, Metadata_pb2 as Metadata, Playlist4External_pb2 as Playlist4External
 from librespot.proto.ExplicitContentPubsub_pb2 import UserAttributesUpdate
 from librespot.structure import Closeable, MessageListener, RequestListener, SubListener
 import base64
 import concurrent.futures
 import defusedxml.ElementTree
 import enum
 import gzip
@@ -150,14 +150,26 @@
         body = response.content
         if body is None:
             raise IOError()
         proto = Metadata.Show()
         proto.ParseFromString(body)
         return proto
 
+    def get_playlist(self, _id: PlaylistId) -> Playlist4External.SelectedListContent:
+        response = self.send("GET",
+                             "/playlist/v2/playlist/{}".format(_id.id()), None,
+                             None)
+        ApiClient.StatusCodeException.check_status(response)
+        body = response.content
+        if body is None:
+            raise IOError()
+        proto = Playlist4External.SelectedListContent()
+        proto.ParseFromString(body)
+        return proto
+
     def set_client_token(self, client_token):
         self.__client_token_str = client_token
 
     def __client_token(self):
         proto_req = ClientToken.ClientTokenRequest(
             request_type=ClientToken.ClientTokenRequestType.REQUEST_CLIENT_DATA_REQUEST,
             client_data=ClientToken.ClientDataRequest(
@@ -1634,15 +1646,15 @@
                     cmd = Packet.Type.parse(packet.cmd)
                     if cmd is None:
                         self.__session.logger.info(
                             "Skipping unknown command cmd: 0x{}, payload: {}".
                             format(util.bytes_to_hex(packet.cmd),
                                    packet.payload))
                         continue
-                except RuntimeError as ex:
+                except (RuntimeError, ConnectionResetError) as ex:
                     if self.__running:
                         self.__session.logger.fatal(
                             "Failed reading packet! {}".format(ex))
                         self.__session.reconnect()
                     break
                 if not self.__running:
                     break
```

### Comparing `librespot-0.0.7/librespot/crypto.py` & `librespot-0.0.8/librespot/crypto.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/mercury.py` & `librespot-0.0.8/librespot/mercury.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/metadata.py` & `librespot-0.0.8/librespot/metadata.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,14 +58,37 @@
     def hex_id(self) -> str:
         raise NotImplementedError
 
     def to_spotify_uri(self) -> str:
         raise NotImplementedError
 
 
+class PlaylistId(SpotifyId):
+    base62 = Base62.create_instance_with_inverted_character_set()
+    pattern = re.compile(r"spotify:playlist:(.{22})")
+    __id: str
+
+    def __init__(self, _id: str):
+        self.__id = _id
+
+    @staticmethod
+    def from_uri(uri: str) -> PlaylistId:
+        matcher = PlaylistId.pattern.search(uri)
+        if matcher is not None:
+            playlist_id = matcher.group(1)
+            return PlaylistId(playlist_id)
+        raise TypeError("Not a Spotify playlist ID: {}.".format(uri))
+
+    def id(self) -> str:
+        return self.__id
+
+    def to_spotify_uri(self) -> str:
+        return "spotify:playlist:" + self.__id
+
+
 class UnsupportedId(PlayableId):
     uri: str
 
     def __init__(self, uri: str):
         self.uri = uri
 
     def get_gid(self) -> bytes:
@@ -87,16 +110,16 @@
         self.__hex_id = hex_id.lower()
 
     @staticmethod
     def from_uri(uri: str) -> AlbumId:
         matcher = AlbumId.pattern.search(uri)
         if matcher is not None:
             album_id = matcher.group(1)
-            return AlbumId(util.bytes_to_hex(AlbumId.base62.decode(album_id.encode())))
-        raise TypeError("Not a Spotify album ID: {}.f".format(uri))
+            return AlbumId(util.bytes_to_hex(AlbumId.base62.decode(album_id.encode(), 16)))
+        raise TypeError("Not a Spotify album ID: {}.".format(uri))
 
     @staticmethod
     def from_base62(base62: str) -> AlbumId:
         return AlbumId(util.bytes_to_hex(AlbumId.base62.decode(base62.encode(), 16)))
 
     @staticmethod
     def from_hex(hex_str: str) -> AlbumId:
```

### Comparing `librespot-0.0.7/librespot/proto/Authentication_pb2.py` & `librespot-0.0.8/librespot/proto/Authentication_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/proto/CanvazMeta_pb2.py` & `librespot-0.0.8/librespot/proto/CanvazMeta_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/proto/Canvaz_pb2.py` & `librespot-0.0.8/librespot/proto/Canvaz_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/proto/ClientToken_pb2.py` & `librespot-0.0.8/librespot/proto/ClientToken_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/proto/Connect_pb2.py` & `librespot-0.0.8/librespot/proto/Connect_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/proto/Connectivity_pb2.py` & `librespot-0.0.8/librespot/proto/Connectivity_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/proto/ContextPage_pb2.py` & `librespot-0.0.8/librespot/proto/ContextPage_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/proto/ContextPlayerOptions_pb2.py` & `librespot-0.0.8/librespot/proto/ContextPlayerOptions_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/proto/ContextTrack_pb2.py` & `librespot-0.0.8/librespot/proto/ContextTrack_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/proto/Context_pb2.py` & `librespot-0.0.8/librespot/proto/Context_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/proto/ExplicitContentPubsub_pb2.py` & `librespot-0.0.8/librespot/proto/ExplicitContentPubsub_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/proto/Keyexchange_pb2.py` & `librespot-0.0.8/librespot/proto/Keyexchange_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/proto/Mercury_pb2.py` & `librespot-0.0.8/librespot/proto/Mercury_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/proto/Metadata_pb2.py` & `librespot-0.0.8/librespot/proto/Metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/proto/PlayOrigin_pb2.py` & `librespot-0.0.8/librespot/proto/PlayOrigin_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/proto/Playback_pb2.py` & `librespot-0.0.8/librespot/proto/Playback_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/proto/Player_pb2.py` & `librespot-0.0.8/librespot/proto/Player_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/proto/Playlist4External_pb2.py` & `librespot-0.0.8/librespot/proto/Playlist4External_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/proto/PlaylistAnnotate3_pb2.py` & `librespot-0.0.8/librespot/proto/PlaylistAnnotate3_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/proto/Pubsub_pb2.py` & `librespot-0.0.8/librespot/proto/Pubsub_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/proto/Queue_pb2.py` & `librespot-0.0.8/librespot/proto/Queue_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/proto/Restrictions_pb2.py` & `librespot-0.0.8/librespot/proto/Restrictions_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/proto/Session_pb2.py` & `librespot-0.0.8/librespot/proto/Session_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/proto/StorageResolve_pb2.py` & `librespot-0.0.8/librespot/proto/StorageResolve_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/proto/TransferState_pb2.py` & `librespot-0.0.8/librespot/proto/TransferState_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/proto/spotify/login5/v3/ClientInfo_pb2.py` & `librespot-0.0.8/librespot/proto/spotify/login5/v3/ClientInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/proto/spotify/login5/v3/Login5_pb2.py` & `librespot-0.0.8/librespot/proto/spotify/login5/v3/Login5_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/proto/spotify/login5/v3/UserInfo_pb2.py` & `librespot-0.0.8/librespot/proto/spotify/login5/v3/UserInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/proto/spotify/login5/v3/challenges/Code_pb2.py` & `librespot-0.0.8/librespot/proto/spotify/login5/v3/challenges/Code_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/proto/spotify/login5/v3/challenges/Hashcash_pb2.py` & `librespot-0.0.8/librespot/proto/spotify/login5/v3/challenges/Hashcash_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/proto/spotify/login5/v3/credentials/Credentials_pb2.py` & `librespot-0.0.8/librespot/proto/spotify/login5/v3/credentials/Credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/proto/spotify/login5/v3/identifiers/Identifiers.py` & `librespot-0.0.8/librespot/proto/spotify/login5/v3/identifiers/Identifiers.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/structure.py` & `librespot-0.0.8/librespot/structure.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/util.py` & `librespot-0.0.8/librespot/util.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot/zeroconf.py` & `librespot-0.0.8/librespot/zeroconf.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot.egg-info/PKG-INFO` & `librespot-0.0.8/librespot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: librespot
-Version: 0.0.7
+Version: 0.0.8
 Summary: Open Source Spotify Client
 Home-page: https://github.com/kokarare1212/librespot-python
 Author: kokarare1212
 License: Apache-2.0
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Multimedia :: Sound/Audio
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: librespot Version: 0.0.7 Summary: Open Source
+Metadata-Version: 2.1 Name: librespot Version: 0.0.8 Summary: Open Source
 Spotify Client Home-page: https://github.com/kokarare1212/librespot-python
 Author: kokarare1212 License: Apache-2.0 Classifier: Development Status :: 1 -
 Planning Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Multimedia :: Sound/Audio Description-Content-Type: text/
 markdown License-File: LICENSE.txt ![License](https://img.shields.io/github/
 license/kokarare1212/librespot-python.svg) ![Stars](https://img.shields.io/
 github/stars/kokarare1212/librespot-python.svg) ![Forks](https://
```

### Comparing `librespot-0.0.7/librespot.egg-info/SOURCES.txt` & `librespot-0.0.8/librespot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/librespot_player/__init__.py` & `librespot-0.0.8/librespot_player/__init__.py`

 * *Files identical despite different names*

### Comparing `librespot-0.0.7/setup.py` & `librespot-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 setuptools.setup(name="librespot",
-                 version="0.0.7",
+                 version="0.0.8",
                  description="Open Source Spotify Client",
                  long_description=open("README.md").read(),
                  long_description_content_type="text/markdown",
                  author="kokarare1212",
                  url="https://github.com/kokarare1212/librespot-python",
                  license="Apache-2.0",
                  packages=setuptools.find_packages("."),
```

