# Comparing `tmp/novauniverse-2.0.1.tar.gz` & `tmp/novauniverse-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "novauniverse-2.0.1.tar", last modified: Tue Apr 11 06:16:47 2023, max compression
+gzip compressed data, was "novauniverse-2.0.2.tar", last modified: Thu Apr 13 02:24:02 2023, max compression
```

## Comparing `novauniverse-2.0.1.tar` & `novauniverse-2.0.2.tar`

### file list

```diff
@@ -1,87 +1,89 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.569648 novauniverse-2.0.1/
-drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.366649 novauniverse-2.0.1/.github/
-drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.393644 novauniverse-2.0.1/.github/workflows/
--rw-rw-rw-   0        0        0      830 2023-03-22 19:01:49.000000 novauniverse-2.0.1/.github/workflows/documentation.yaml
--rw-rw-rw-   0        0        0       68 2023-03-22 18:30:58.000000 novauniverse-2.0.1/.gitignore
--rw-rw-rw-   0        0        0     1228 2023-03-22 18:04:31.000000 novauniverse-2.0.1/CHANGELOG.rst
--rw-rw-rw-   0        0        0      161 2023-03-22 18:20:14.000000 novauniverse-2.0.1/Makefile
--rw-rw-rw-   0        0        0     3136 2023-04-11 06:16:47.568642 novauniverse-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2091 2023-03-24 17:08:14.000000 novauniverse-2.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.451644 novauniverse-2.0.1/docs/
--rw-rw-rw-   0        0        0      654 2023-03-21 20:18:52.000000 novauniverse-2.0.1/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.453645 novauniverse-2.0.1/docs/_static/
--rw-rw-rw-   0        0        0  1821311 2023-03-21 20:18:52.000000 novauniverse-2.0.1/docs/_static/logo.png
--rw-rw-rw-   0        0        0      728 2023-03-22 17:20:14.000000 novauniverse-2.0.1/docs/api.rst
--rw-rw-rw-   0        0        0     1545 2023-03-22 19:18:54.000000 novauniverse-2.0.1/docs/conf.py
--rw-rw-rw-   0        0        0     1189 2023-03-22 17:55:36.000000 novauniverse-2.0.1/docs/events.rst
--rw-rw-rw-   0        0        0     3301 2023-03-22 19:02:01.000000 novauniverse-2.0.1/docs/index.rst
--rw-rw-rw-   0        0        0     3548 2023-03-22 17:20:14.000000 novauniverse-2.0.1/docs/interfaces.rst
--rw-rw-rw-   0        0        0      398 2023-03-21 20:18:52.000000 novauniverse-2.0.1/docs/interfaces.stats.discord.rst
--rw-rw-rw-   0        0        0     1449 2023-03-21 20:18:52.000000 novauniverse-2.0.1/docs/interfaces.stats.server.rst
--rwxrwxrwx   0        0        0      800 2023-03-21 20:18:52.000000 novauniverse-2.0.1/docs/make.bat
--rw-rw-rw-   0        0        0      787 2023-03-22 17:20:14.000000 novauniverse-2.0.1/docs/objects.rst
--rw-rw-rw-   0        0        0      484 2023-03-21 20:18:52.000000 novauniverse-2.0.1/docs/objects.tournaments.rst
--rw-rw-rw-   0        0        0      247 2023-03-22 17:20:14.000000 novauniverse-2.0.1/docs/utils.rst
-drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.466642 novauniverse-2.0.1/novauniverse/
--rw-rw-rw-   0        0        0     1803 2023-04-11 06:12:05.000000 novauniverse-2.0.1/novauniverse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.503644 novauniverse-2.0.1/novauniverse/api/
--rw-rw-rw-   0        0        0     2799 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/api/__init__.py
--rw-rw-rw-   0        0        0     1874 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/api/cdn.py
--rw-rw-rw-   0        0        0     1822 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/api/endpoints.py
--rw-rw-rw-   0        0        0     1135 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/api/errors.py
--rw-rw-rw-   0        0        0      554 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/configuration.py
--rw-rw-rw-   0        0        0      417 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/errors.py
--rw-rw-rw-   0        0        0     4104 2023-03-22 17:20:14.000000 novauniverse-2.0.1/novauniverse/event_client.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.511641 novauniverse-2.0.1/novauniverse/events/
--rw-rw-rw-   0        0        0     3877 2023-03-22 17:20:14.000000 novauniverse-2.0.1/novauniverse/events/__init__.py
--rw-rw-rw-   0        0        0      494 2023-03-22 17:20:14.000000 novauniverse-2.0.1/novauniverse/events/client_ready.py
--rw-rw-rw-   0        0        0     1162 2023-03-22 17:20:14.000000 novauniverse-2.0.1/novauniverse/events/player_join.py
--rw-rw-rw-   0        0        0     1045 2023-03-22 17:20:14.000000 novauniverse-2.0.1/novauniverse/events/player_leave.py
--rw-rw-rw-   0        0        0      356 2023-04-11 06:16:05.000000 novauniverse-2.0.1/novauniverse/info.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.513643 novauniverse-2.0.1/novauniverse/interfaces/
--rw-rw-rw-   0        0        0     1945 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/interfaces/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.516643 novauniverse-2.0.1/novauniverse/interfaces/mcf/
--rw-rw-rw-   0        0        0     2811 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/interfaces/mcf/__init__.py
--rw-rw-rw-   0        0        0      194 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/interfaces/mcf/mcf_tournament.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.518642 novauniverse-2.0.1/novauniverse/interfaces/stats/
--rw-rw-rw-   0        0        0        0 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/interfaces/stats/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.523643 novauniverse-2.0.1/novauniverse/interfaces/stats/discord/
--rw-rw-rw-   0        0        0      541 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/interfaces/stats/discord/__init__.py
--rw-rw-rw-   0        0        0      781 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/interfaces/stats/discord/discord_stats.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.537644 novauniverse-2.0.1/novauniverse/interfaces/stats/server/
--rw-rw-rw-   0        0        0     1024 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/interfaces/stats/server/__init__.py
--rw-rw-rw-   0        0        0      551 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/interfaces/stats/server/global_.py
--rw-rw-rw-   0        0        0     1001 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/interfaces/stats/server/nova_online_player.py
--rw-rw-rw-   0        0        0     1022 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/interfaces/stats/server/nova_server.py
--rw-rw-rw-   0        0        0      666 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/interfaces/stats/server/player_preview.py
--rw-rw-rw-   0        0        0     1926 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/interfaces/stats/server/server_info.py
--rw-rw-rw-   0        0        0      344 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/interfaces/stats/server/system.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.547646 novauniverse-2.0.1/novauniverse/objects/
--rw-rw-rw-   0        0        0      337 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/objects/__init__.py
--rw-rw-rw-   0        0        0     1018 2023-03-22 14:57:55.000000 novauniverse-2.0.1/novauniverse/objects/nova_dataclass.py
--rw-rw-rw-   0        0        0      653 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/objects/nova_player.py
--rw-rw-rw-   0        0        0      355 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/objects/order_by.py
--rw-rw-rw-   0        0        0      798 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/objects/timestamp.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.553646 novauniverse-2.0.1/novauniverse/objects/tournaments/
--rw-rw-rw-   0        0        0     1697 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/objects/tournaments/__init__.py
--rw-rw-rw-   0        0        0      975 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/objects/tournaments/tournament_player.py
--rw-rw-rw-   0        0        0      906 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/objects/tournaments/tournament_team.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.557644 novauniverse-2.0.1/novauniverse/utils/
--rw-rw-rw-   0        0        0       36 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/utils/__init__.py
--rw-rw-rw-   0        0        0     1657 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/utils/search.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.495655 novauniverse-2.0.1/novauniverse.egg-info/
--rw-rw-rw-   0        0        0     3136 2023-04-11 06:16:47.000000 novauniverse-2.0.1/novauniverse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2082 2023-04-11 06:16:47.000000 novauniverse-2.0.1/novauniverse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 06:16:47.000000 novauniverse-2.0.1/novauniverse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      148 2023-04-11 06:16:47.000000 novauniverse-2.0.1/novauniverse.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-11 06:16:47.000000 novauniverse-2.0.1/novauniverse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1597 2023-04-11 06:07:36.000000 novauniverse-2.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-11 06:16:47.569648 novauniverse-2.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.559646 novauniverse-2.0.1/tests/
--rw-rw-rw-   0        0        0       66 2023-03-21 20:18:52.000000 novauniverse-2.0.1/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.561643 novauniverse-2.0.1/tests/interfaces/
--rw-rw-rw-   0        0        0        0 2023-03-21 20:18:52.000000 novauniverse-2.0.1/tests/interfaces/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.566641 novauniverse-2.0.1/tests/interfaces/stats/
--rw-rw-rw-   0        0        0        0 2023-03-21 20:18:52.000000 novauniverse-2.0.1/tests/interfaces/stats/__init__.py
--rw-rw-rw-   0        0        0      275 2023-03-21 20:18:52.000000 novauniverse-2.0.1/tests/interfaces/stats/test_discord.py
--rw-rw-rw-   0        0        0      846 2023-03-21 20:18:52.000000 novauniverse-2.0.1/tests/interfaces/stats/test_server.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.859748 novauniverse-2.0.2/
+drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.692751 novauniverse-2.0.2/.github/
+drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.720752 novauniverse-2.0.2/.github/workflows/
+-rw-rw-rw-   0        0        0      830 2023-03-22 19:01:49.000000 novauniverse-2.0.2/.github/workflows/documentation.yaml
+-rw-rw-rw-   0        0        0       81 2023-04-13 02:18:11.000000 novauniverse-2.0.2/.gitignore
+-rw-rw-rw-   0        0        0     1228 2023-03-22 18:04:31.000000 novauniverse-2.0.2/CHANGELOG.rst
+-rw-rw-rw-   0        0        0      199 2023-04-13 01:19:26.000000 novauniverse-2.0.2/Makefile
+-rw-rw-rw-   0        0        0     3136 2023-04-13 02:24:02.858750 novauniverse-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2091 2023-03-24 17:08:14.000000 novauniverse-2.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.745748 novauniverse-2.0.2/docs/
+-rw-rw-rw-   0        0        0      654 2023-03-21 20:18:52.000000 novauniverse-2.0.2/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.747748 novauniverse-2.0.2/docs/_static/
+-rw-rw-rw-   0        0        0  1821311 2023-03-21 20:18:52.000000 novauniverse-2.0.2/docs/_static/logo.png
+-rw-rw-rw-   0        0        0      728 2023-03-22 17:20:14.000000 novauniverse-2.0.2/docs/api.rst
+-rw-rw-rw-   0        0        0     1545 2023-03-22 19:18:54.000000 novauniverse-2.0.2/docs/conf.py
+-rw-rw-rw-   0        0        0     1189 2023-03-22 17:55:36.000000 novauniverse-2.0.2/docs/events.rst
+-rw-rw-rw-   0        0        0     3301 2023-03-22 19:02:01.000000 novauniverse-2.0.2/docs/index.rst
+-rw-rw-rw-   0        0        0      364 2023-04-13 02:02:29.000000 novauniverse-2.0.2/docs/interfaces.mcf.rst
+-rw-rw-rw-   0        0        0     3567 2023-04-13 02:00:36.000000 novauniverse-2.0.2/docs/interfaces.rst
+-rw-rw-rw-   0        0        0      398 2023-04-13 02:03:17.000000 novauniverse-2.0.2/docs/interfaces.stats.discord.rst
+-rw-rw-rw-   0        0        0     1449 2023-03-21 20:18:52.000000 novauniverse-2.0.2/docs/interfaces.stats.server.rst
+-rwxrwxrwx   0        0        0      800 2023-03-21 20:18:52.000000 novauniverse-2.0.2/docs/make.bat
+-rw-rw-rw-   0        0        0      787 2023-03-22 17:20:14.000000 novauniverse-2.0.2/docs/objects.rst
+-rw-rw-rw-   0        0        0      484 2023-03-21 20:18:52.000000 novauniverse-2.0.2/docs/objects.tournaments.rst
+-rw-rw-rw-   0        0        0      247 2023-03-22 17:20:14.000000 novauniverse-2.0.2/docs/utils.rst
+drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.761748 novauniverse-2.0.2/novauniverse/
+-rw-rw-rw-   0        0        0     1760 2023-04-13 00:23:33.000000 novauniverse-2.0.2/novauniverse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.789750 novauniverse-2.0.2/novauniverse/api/
+-rw-rw-rw-   0        0        0     2799 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/api/__init__.py
+-rw-rw-rw-   0        0        0     1874 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/api/cdn.py
+-rw-rw-rw-   0        0        0     1822 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/api/endpoints.py
+-rw-rw-rw-   0        0        0     1135 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/api/errors.py
+-rw-rw-rw-   0        0        0      554 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/configuration.py
+-rw-rw-rw-   0        0        0      417 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/errors.py
+-rw-rw-rw-   0        0        0     4104 2023-03-22 17:20:14.000000 novauniverse-2.0.2/novauniverse/event_client.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.798756 novauniverse-2.0.2/novauniverse/events/
+-rw-rw-rw-   0        0        0     3877 2023-03-22 17:20:14.000000 novauniverse-2.0.2/novauniverse/events/__init__.py
+-rw-rw-rw-   0        0        0      494 2023-03-22 17:20:14.000000 novauniverse-2.0.2/novauniverse/events/client_ready.py
+-rw-rw-rw-   0        0        0     1162 2023-03-22 17:20:14.000000 novauniverse-2.0.2/novauniverse/events/player_join.py
+-rw-rw-rw-   0        0        0     1045 2023-03-22 17:20:14.000000 novauniverse-2.0.2/novauniverse/events/player_leave.py
+-rw-rw-rw-   0        0        0      356 2023-04-13 02:01:34.000000 novauniverse-2.0.2/novauniverse/info.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.800757 novauniverse-2.0.2/novauniverse/interfaces/
+-rw-rw-rw-   0        0        0     2127 2023-04-13 00:38:41.000000 novauniverse-2.0.2/novauniverse/interfaces/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.804754 novauniverse-2.0.2/novauniverse/interfaces/mcf/
+-rw-rw-rw-   0        0        0     2811 2023-04-13 01:34:13.000000 novauniverse-2.0.2/novauniverse/interfaces/mcf/__init__.py
+-rw-rw-rw-   0        0        0      194 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/interfaces/mcf/mcf_tournament.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.806751 novauniverse-2.0.2/novauniverse/interfaces/stats/
+-rw-rw-rw-   0        0        0        0 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/interfaces/stats/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.810754 novauniverse-2.0.2/novauniverse/interfaces/stats/discord/
+-rw-rw-rw-   0        0        0      541 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/interfaces/stats/discord/__init__.py
+-rw-rw-rw-   0        0        0      781 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/interfaces/stats/discord/discord_stats.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.824750 novauniverse-2.0.2/novauniverse/interfaces/stats/server/
+-rw-rw-rw-   0        0        0     1024 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/interfaces/stats/server/__init__.py
+-rw-rw-rw-   0        0        0      551 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/interfaces/stats/server/global_.py
+-rw-rw-rw-   0        0        0     1001 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/interfaces/stats/server/nova_online_player.py
+-rw-rw-rw-   0        0        0     1022 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/interfaces/stats/server/nova_server.py
+-rw-rw-rw-   0        0        0      666 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/interfaces/stats/server/player_preview.py
+-rw-rw-rw-   0        0        0     1926 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/interfaces/stats/server/server_info.py
+-rw-rw-rw-   0        0        0      344 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/interfaces/stats/server/system.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.834748 novauniverse-2.0.2/novauniverse/objects/
+-rw-rw-rw-   0        0        0      337 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/objects/__init__.py
+-rw-rw-rw-   0        0        0     1018 2023-03-22 14:57:55.000000 novauniverse-2.0.2/novauniverse/objects/nova_dataclass.py
+-rw-rw-rw-   0        0        0      653 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/objects/nova_player.py
+-rw-rw-rw-   0        0        0      355 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/objects/order_by.py
+-rw-rw-rw-   0        0        0      798 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/objects/timestamp.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.840750 novauniverse-2.0.2/novauniverse/objects/tournaments/
+-rw-rw-rw-   0        0        0     1697 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/objects/tournaments/__init__.py
+-rw-rw-rw-   0        0        0      975 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/objects/tournaments/tournament_player.py
+-rw-rw-rw-   0        0        0      906 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/objects/tournaments/tournament_team.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.844750 novauniverse-2.0.2/novauniverse/utils/
+-rw-rw-rw-   0        0        0       36 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/utils/__init__.py
+-rw-rw-rw-   0        0        0     1920 2023-04-13 02:05:26.000000 novauniverse-2.0.2/novauniverse/utils/search.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.782752 novauniverse-2.0.2/novauniverse.egg-info/
+-rw-rw-rw-   0        0        0     3136 2023-04-13 02:24:02.000000 novauniverse-2.0.2/novauniverse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2135 2023-04-13 02:24:02.000000 novauniverse-2.0.2/novauniverse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 02:24:02.000000 novauniverse-2.0.2/novauniverse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      153 2023-04-13 02:24:02.000000 novauniverse-2.0.2/novauniverse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-13 02:24:02.000000 novauniverse-2.0.2/novauniverse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2819 2023-04-13 02:23:08.000000 novauniverse-2.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 02:24:02.859748 novauniverse-2.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.847748 novauniverse-2.0.2/tests/
+-rw-rw-rw-   0        0        0       66 2023-03-21 20:18:52.000000 novauniverse-2.0.2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.851748 novauniverse-2.0.2/tests/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-03-21 20:18:52.000000 novauniverse-2.0.2/tests/interfaces/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.856749 novauniverse-2.0.2/tests/interfaces/stats/
+-rw-rw-rw-   0        0        0        0 2023-03-21 20:18:52.000000 novauniverse-2.0.2/tests/interfaces/stats/__init__.py
+-rw-rw-rw-   0        0        0      275 2023-03-21 20:18:52.000000 novauniverse-2.0.2/tests/interfaces/stats/test_discord.py
+-rw-rw-rw-   0        0        0      846 2023-03-21 20:18:52.000000 novauniverse-2.0.2/tests/interfaces/stats/test_server.py
+-rw-rw-rw-   0        0        0     1806 2023-04-13 01:59:19.000000 novauniverse-2.0.2/tests/interfaces/test_mcf.py
```

### Comparing `novauniverse-2.0.1/.github/workflows/documentation.yaml` & `novauniverse-2.0.2/.github/workflows/documentation.yaml`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/CHANGELOG.rst` & `novauniverse-2.0.2/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/PKG-INFO` & `novauniverse-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: novauniverse
-Version: 2.0.1
+Version: 2.0.2
 Summary: A modern & maintained wrapper for the Nova Universe API written in 🐍 Python.
 Author-email: Goldy <goldy@devgoldy.me>
 Project-URL: GitHub, https://github.com/NovaUniverse/NovaUniverse.py
 Project-URL: BugTracker, https://github.com/NovaUniverse/NovaUniverse.py/issues
 Project-URL: ChangeLog, https://github.com/NovaUniverse/NovaUniverse.py/blob/main/CHANGELOG.rst
 Keywords: novauniverse,minecraft novauniverse,nova universe,mc novauniverse
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: novauniverse Version: 2.0.1 Summary: A modern &
+Metadata-Version: 2.1 Name: novauniverse Version: 2.0.2 Summary: A modern &
 maintained wrapper for the Nova Universe API written in ð Python. Author-
 email: Goldy
 devgoldy.me> Project-URL: GitHub, https://github.com/NovaUniverse/
 NovaUniverse.py Project-URL: BugTracker, https://github.com/NovaUniverse/
 NovaUniverse.py/issues Project-URL: ChangeLog, https://github.com/NovaUniverse/
 NovaUniverse.py/blob/main/CHANGELOG.rst Keywords: novauniverse,minecraft
 novauniverse,nova universe,mc novauniverse Classifier: Operating System ::
```

### Comparing `novauniverse-2.0.1/README.md` & `novauniverse-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/docs/Makefile` & `novauniverse-2.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/docs/_static/logo.png` & `novauniverse-2.0.2/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/docs/api.rst` & `novauniverse-2.0.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/docs/conf.py` & `novauniverse-2.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/docs/events.rst` & `novauniverse-2.0.2/docs/events.rst`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/docs/index.rst` & `novauniverse-2.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/docs/interfaces.rst` & `novauniverse-2.0.2/docs/interfaces.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Interfaces 🧩
 ===============================
 
 .. toctree::
    :maxdepth: 1
 
+   interfaces.mcf
    interfaces.stats.discord
    interfaces.stats.server
 
 
 .. _The Interface:
 
 The Interface ✨
```

### Comparing `novauniverse-2.0.1/docs/interfaces.stats.server.rst` & `novauniverse-2.0.2/docs/interfaces.stats.server.rst`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/docs/make.bat` & `novauniverse-2.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/docs/objects.rst` & `novauniverse-2.0.2/docs/objects.rst`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/novauniverse/__init__.py` & `novauniverse-2.0.2/novauniverse/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,37 +10,32 @@
 from devgoldyutils.logging import add_custom_handler, log
 
 nova_logger = add_custom_handler(log.getLogger(LOGGER_NAME), level=log.WARNING)
 """
 The python ``logging.Logger()`` class for NovaUniverse.py.
 
 ---------------
-### ``Example:``
 
-You can disable and also adjust the level of logging from the api wrapper like this:
+⭐Example:
+------------
 
-```python
-import logging
-nova_logger.setLevel(logging.DEBUG)
-```
+You can disable and also adjust the level of logging from the api wrapper like this::
 
-If your using the ``novauniverse.EventClient`` class, a shortcut for enabling debugging would be this:
+    import logging
+    nova_logger.setLevel(logging.DEBUG)
 
-```python
-EventClient(debug=True)
-```
+If your using the ``novauniverse.EventClient`` class, a shortcut for enabling debugging would be this::
 
-If you want to completely disable logging like example warnings, you can do that with:
+    EventClient(debug=True)
 
-```python
-nova_logger.setLevel(logging.NOTSET)
-```
-"""
+If you want to completely disable logging like example remove warnings, you can do that with::
+
+    nova_logger.setLevel(logging.NOTSET)
 
-nova_logger.setLevel(log.WARN)
+"""
 
 # Configuration
 # ---------------
 from .configuration import Config
 config = Config()
 """🐉 NovaUniverse.py config."""
```

### Comparing `novauniverse-2.0.1/novauniverse/api/__init__.py` & `novauniverse-2.0.2/novauniverse/api/__init__.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/novauniverse/api/cdn.py` & `novauniverse-2.0.2/novauniverse/api/cdn.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/novauniverse/api/endpoints.py` & `novauniverse-2.0.2/novauniverse/api/endpoints.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/novauniverse/api/errors.py` & `novauniverse-2.0.2/novauniverse/api/errors.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/novauniverse/configuration.py` & `novauniverse-2.0.2/novauniverse/configuration.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/novauniverse/event_client.py` & `novauniverse-2.0.2/novauniverse/event_client.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/novauniverse/events/__init__.py` & `novauniverse-2.0.2/novauniverse/events/__init__.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/novauniverse/events/player_join.py` & `novauniverse-2.0.2/novauniverse/events/player_join.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/novauniverse/events/player_leave.py` & `novauniverse-2.0.2/novauniverse/events/player_leave.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/novauniverse/interfaces/__init__.py` & `novauniverse-2.0.2/novauniverse/interfaces/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,23 +28,27 @@
         self.__keys = keys
 
         self.logger = LoggerAdapter(nova_logger, prefix="SearchInterface")
         super().__init__()
 
     @abstractmethod
     def search(self, query: Search | int | str, objects: List[object] = None) -> object | None:
-        """It is recommended to use ``novauniverse.utils.search.Search()`` as a query."""
-        if not isinstance(query, Search):
-            query = Search(name = str(query))
-            # TODO: Add fuzzy search in the future.
+        """It is recommended to use ``novauniverse.utils.search.Search()`` as a query but strings and integers will also work and be handled respectively."""
+
+        if isinstance(query, str) or isinstance(query, int):
+            if query.isnumeric():
+                query = Search(id = query)
+            else:
+                query = Search(name = query)
 
         if not query.search_by in self.__supports:
             query.not_supported(self)
 
         self.logger.debug(f"Searching in '{self.__class__.__name__}' by '{query.search_by.name}' for '{query.get_query()}'...")
+        # TODO: Add fuzzy search in the future.
         for object in objects:
             if object.__dict__[self.__keys[query.search_by]] == query.get_query():
                 self.logger.info(f"Found {query.get_query()} by '{query.search_by.name}'.")
                 return object
 
         return None
```

### Comparing `novauniverse-2.0.1/novauniverse/interfaces/mcf/__init__.py` & `novauniverse-2.0.2/novauniverse/interfaces/mcf/__init__.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/novauniverse/interfaces/stats/discord/__init__.py` & `novauniverse-2.0.2/novauniverse/interfaces/stats/discord/__init__.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/novauniverse/interfaces/stats/discord/discord_stats.py` & `novauniverse-2.0.2/novauniverse/interfaces/stats/discord/discord_stats.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/novauniverse/interfaces/stats/server/__init__.py` & `novauniverse-2.0.2/novauniverse/interfaces/stats/server/__init__.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/novauniverse/interfaces/stats/server/global_.py` & `novauniverse-2.0.2/novauniverse/interfaces/stats/server/global_.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/novauniverse/interfaces/stats/server/nova_online_player.py` & `novauniverse-2.0.2/novauniverse/interfaces/stats/server/nova_online_player.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/novauniverse/interfaces/stats/server/nova_server.py` & `novauniverse-2.0.2/novauniverse/interfaces/stats/server/nova_server.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/novauniverse/interfaces/stats/server/player_preview.py` & `novauniverse-2.0.2/novauniverse/interfaces/stats/server/player_preview.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/novauniverse/interfaces/stats/server/server_info.py` & `novauniverse-2.0.2/novauniverse/interfaces/stats/server/server_info.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/novauniverse/objects/nova_dataclass.py` & `novauniverse-2.0.2/novauniverse/objects/nova_dataclass.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/novauniverse/objects/nova_player.py` & `novauniverse-2.0.2/novauniverse/objects/nova_player.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/novauniverse/objects/timestamp.py` & `novauniverse-2.0.2/novauniverse/objects/timestamp.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/novauniverse/objects/tournaments/__init__.py` & `novauniverse-2.0.2/novauniverse/objects/tournaments/__init__.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/novauniverse/objects/tournaments/tournament_player.py` & `novauniverse-2.0.2/novauniverse/objects/tournaments/tournament_player.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/novauniverse/objects/tournaments/tournament_team.py` & `novauniverse-2.0.2/novauniverse/objects/tournaments/tournament_team.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.1/novauniverse/utils/search.py` & `novauniverse-2.0.2/novauniverse/utils/search.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+from typing import overload, NoReturn
 from enum import Enum
 
 from ..errors import NovaError
 
 # SearchBy Enum class
 # ---------------------
 class SearchBy(Enum):
@@ -19,14 +20,24 @@
     def __init__(self, searched_by, interface:object) -> None:
         super().__init__(f"Searching by '{searched_by}' not supported by '{interface.__class__.__name__}' interface/endpoint.")
 
 # Search class
 # ---------------
 class Search():
     """A util that allows you to search within an interface by id or name if supported."""
+    @overload
+    def __init__(self, id:str|int) -> None:
+        """Search by id."""
+        ...
+    
+    @overload
+    def __init__(self, name:str) -> None:
+        """Search by name."""
+        ...
+
     def __init__(self, id:str|int=None, name:str=None) -> None:
         self.id = id
         self.name = name
 
         self.search_by:SearchBy|None = None
 
         if self.name is not None:
@@ -41,10 +52,10 @@
         """Returns the query."""
         if self.search_by is SearchBy.ID:
             return self.id
         if self.search_by is SearchBy.NAME:
             return self.name
         return None
 
-    def not_supported(self, interface: object):
+    def not_supported(self, interface: object) -> NoReturn:
         """Raises error to warn user this interface does not support searching by id/name."""
         raise SearchNotCompletelySupported(self.search_by.name, interface)
```

### Comparing `novauniverse-2.0.1/novauniverse.egg-info/PKG-INFO` & `novauniverse-2.0.2/novauniverse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: novauniverse
-Version: 2.0.1
+Version: 2.0.2
 Summary: A modern & maintained wrapper for the Nova Universe API written in 🐍 Python.
 Author-email: Goldy <goldy@devgoldy.me>
 Project-URL: GitHub, https://github.com/NovaUniverse/NovaUniverse.py
 Project-URL: BugTracker, https://github.com/NovaUniverse/NovaUniverse.py/issues
 Project-URL: ChangeLog, https://github.com/NovaUniverse/NovaUniverse.py/blob/main/CHANGELOG.rst
 Keywords: novauniverse,minecraft novauniverse,nova universe,mc novauniverse
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: novauniverse Version: 2.0.1 Summary: A modern &
+Metadata-Version: 2.1 Name: novauniverse Version: 2.0.2 Summary: A modern &
 maintained wrapper for the Nova Universe API written in ð Python. Author-
 email: Goldy
 devgoldy.me> Project-URL: GitHub, https://github.com/NovaUniverse/
 NovaUniverse.py Project-URL: BugTracker, https://github.com/NovaUniverse/
 NovaUniverse.py/issues Project-URL: ChangeLog, https://github.com/NovaUniverse/
 NovaUniverse.py/blob/main/CHANGELOG.rst Keywords: novauniverse,minecraft
 novauniverse,nova universe,mc novauniverse Classifier: Operating System ::
```

### Comparing `novauniverse-2.0.1/novauniverse.egg-info/SOURCES.txt` & `novauniverse-2.0.2/novauniverse.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 pyproject.toml
 .github/workflows/documentation.yaml
 docs/Makefile
 docs/api.rst
 docs/conf.py
 docs/events.rst
 docs/index.rst
+docs/interfaces.mcf.rst
 docs/interfaces.rst
 docs/interfaces.stats.discord.rst
 docs/interfaces.stats.server.rst
 docs/make.bat
 docs/objects.rst
 docs/objects.tournaments.rst
 docs/utils.rst
@@ -56,10 +57,11 @@
 novauniverse/objects/tournaments/__init__.py
 novauniverse/objects/tournaments/tournament_player.py
 novauniverse/objects/tournaments/tournament_team.py
 novauniverse/utils/__init__.py
 novauniverse/utils/search.py
 tests/__init__.py
 tests/interfaces/__init__.py
+tests/interfaces/test_mcf.py
 tests/interfaces/stats/__init__.py
 tests/interfaces/stats/test_discord.py
 tests/interfaces/stats/test_server.py
```

### Comparing `novauniverse-2.0.1/tests/interfaces/stats/test_server.py` & `novauniverse-2.0.2/tests/interfaces/stats/test_server.py`

 * *Files identical despite different names*

