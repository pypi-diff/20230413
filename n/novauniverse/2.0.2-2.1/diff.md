# Comparing `tmp/novauniverse-2.0.2.tar.gz` & `tmp/novauniverse-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "novauniverse-2.0.2.tar", last modified: Thu Apr 13 02:24:02 2023, max compression
+gzip compressed data, was "novauniverse-2.1.tar", last modified: Thu Apr 13 14:36:51 2023, max compression
```

## Comparing `novauniverse-2.0.2.tar` & `novauniverse-2.1.tar`

### file list

```diff
@@ -1,89 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.859748 novauniverse-2.0.2/
-drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.692751 novauniverse-2.0.2/.github/
-drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.720752 novauniverse-2.0.2/.github/workflows/
--rw-rw-rw-   0        0        0      830 2023-03-22 19:01:49.000000 novauniverse-2.0.2/.github/workflows/documentation.yaml
--rw-rw-rw-   0        0        0       81 2023-04-13 02:18:11.000000 novauniverse-2.0.2/.gitignore
--rw-rw-rw-   0        0        0     1228 2023-03-22 18:04:31.000000 novauniverse-2.0.2/CHANGELOG.rst
--rw-rw-rw-   0        0        0      199 2023-04-13 01:19:26.000000 novauniverse-2.0.2/Makefile
--rw-rw-rw-   0        0        0     3136 2023-04-13 02:24:02.858750 novauniverse-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2091 2023-03-24 17:08:14.000000 novauniverse-2.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.745748 novauniverse-2.0.2/docs/
--rw-rw-rw-   0        0        0      654 2023-03-21 20:18:52.000000 novauniverse-2.0.2/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.747748 novauniverse-2.0.2/docs/_static/
--rw-rw-rw-   0        0        0  1821311 2023-03-21 20:18:52.000000 novauniverse-2.0.2/docs/_static/logo.png
--rw-rw-rw-   0        0        0      728 2023-03-22 17:20:14.000000 novauniverse-2.0.2/docs/api.rst
--rw-rw-rw-   0        0        0     1545 2023-03-22 19:18:54.000000 novauniverse-2.0.2/docs/conf.py
--rw-rw-rw-   0        0        0     1189 2023-03-22 17:55:36.000000 novauniverse-2.0.2/docs/events.rst
--rw-rw-rw-   0        0        0     3301 2023-03-22 19:02:01.000000 novauniverse-2.0.2/docs/index.rst
--rw-rw-rw-   0        0        0      364 2023-04-13 02:02:29.000000 novauniverse-2.0.2/docs/interfaces.mcf.rst
--rw-rw-rw-   0        0        0     3567 2023-04-13 02:00:36.000000 novauniverse-2.0.2/docs/interfaces.rst
--rw-rw-rw-   0        0        0      398 2023-04-13 02:03:17.000000 novauniverse-2.0.2/docs/interfaces.stats.discord.rst
--rw-rw-rw-   0        0        0     1449 2023-03-21 20:18:52.000000 novauniverse-2.0.2/docs/interfaces.stats.server.rst
--rwxrwxrwx   0        0        0      800 2023-03-21 20:18:52.000000 novauniverse-2.0.2/docs/make.bat
--rw-rw-rw-   0        0        0      787 2023-03-22 17:20:14.000000 novauniverse-2.0.2/docs/objects.rst
--rw-rw-rw-   0        0        0      484 2023-03-21 20:18:52.000000 novauniverse-2.0.2/docs/objects.tournaments.rst
--rw-rw-rw-   0        0        0      247 2023-03-22 17:20:14.000000 novauniverse-2.0.2/docs/utils.rst
-drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.761748 novauniverse-2.0.2/novauniverse/
--rw-rw-rw-   0        0        0     1760 2023-04-13 00:23:33.000000 novauniverse-2.0.2/novauniverse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.789750 novauniverse-2.0.2/novauniverse/api/
--rw-rw-rw-   0        0        0     2799 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/api/__init__.py
--rw-rw-rw-   0        0        0     1874 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/api/cdn.py
--rw-rw-rw-   0        0        0     1822 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/api/endpoints.py
--rw-rw-rw-   0        0        0     1135 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/api/errors.py
--rw-rw-rw-   0        0        0      554 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/configuration.py
--rw-rw-rw-   0        0        0      417 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/errors.py
--rw-rw-rw-   0        0        0     4104 2023-03-22 17:20:14.000000 novauniverse-2.0.2/novauniverse/event_client.py
-drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.798756 novauniverse-2.0.2/novauniverse/events/
--rw-rw-rw-   0        0        0     3877 2023-03-22 17:20:14.000000 novauniverse-2.0.2/novauniverse/events/__init__.py
--rw-rw-rw-   0        0        0      494 2023-03-22 17:20:14.000000 novauniverse-2.0.2/novauniverse/events/client_ready.py
--rw-rw-rw-   0        0        0     1162 2023-03-22 17:20:14.000000 novauniverse-2.0.2/novauniverse/events/player_join.py
--rw-rw-rw-   0        0        0     1045 2023-03-22 17:20:14.000000 novauniverse-2.0.2/novauniverse/events/player_leave.py
--rw-rw-rw-   0        0        0      356 2023-04-13 02:01:34.000000 novauniverse-2.0.2/novauniverse/info.py
-drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.800757 novauniverse-2.0.2/novauniverse/interfaces/
--rw-rw-rw-   0        0        0     2127 2023-04-13 00:38:41.000000 novauniverse-2.0.2/novauniverse/interfaces/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.804754 novauniverse-2.0.2/novauniverse/interfaces/mcf/
--rw-rw-rw-   0        0        0     2811 2023-04-13 01:34:13.000000 novauniverse-2.0.2/novauniverse/interfaces/mcf/__init__.py
--rw-rw-rw-   0        0        0      194 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/interfaces/mcf/mcf_tournament.py
-drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.806751 novauniverse-2.0.2/novauniverse/interfaces/stats/
--rw-rw-rw-   0        0        0        0 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/interfaces/stats/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.810754 novauniverse-2.0.2/novauniverse/interfaces/stats/discord/
--rw-rw-rw-   0        0        0      541 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/interfaces/stats/discord/__init__.py
--rw-rw-rw-   0        0        0      781 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/interfaces/stats/discord/discord_stats.py
-drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.824750 novauniverse-2.0.2/novauniverse/interfaces/stats/server/
--rw-rw-rw-   0        0        0     1024 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/interfaces/stats/server/__init__.py
--rw-rw-rw-   0        0        0      551 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/interfaces/stats/server/global_.py
--rw-rw-rw-   0        0        0     1001 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/interfaces/stats/server/nova_online_player.py
--rw-rw-rw-   0        0        0     1022 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/interfaces/stats/server/nova_server.py
--rw-rw-rw-   0        0        0      666 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/interfaces/stats/server/player_preview.py
--rw-rw-rw-   0        0        0     1926 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/interfaces/stats/server/server_info.py
--rw-rw-rw-   0        0        0      344 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/interfaces/stats/server/system.py
-drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.834748 novauniverse-2.0.2/novauniverse/objects/
--rw-rw-rw-   0        0        0      337 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/objects/__init__.py
--rw-rw-rw-   0        0        0     1018 2023-03-22 14:57:55.000000 novauniverse-2.0.2/novauniverse/objects/nova_dataclass.py
--rw-rw-rw-   0        0        0      653 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/objects/nova_player.py
--rw-rw-rw-   0        0        0      355 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/objects/order_by.py
--rw-rw-rw-   0        0        0      798 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/objects/timestamp.py
-drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.840750 novauniverse-2.0.2/novauniverse/objects/tournaments/
--rw-rw-rw-   0        0        0     1697 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/objects/tournaments/__init__.py
--rw-rw-rw-   0        0        0      975 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/objects/tournaments/tournament_player.py
--rw-rw-rw-   0        0        0      906 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/objects/tournaments/tournament_team.py
-drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.844750 novauniverse-2.0.2/novauniverse/utils/
--rw-rw-rw-   0        0        0       36 2023-03-21 20:18:52.000000 novauniverse-2.0.2/novauniverse/utils/__init__.py
--rw-rw-rw-   0        0        0     1920 2023-04-13 02:05:26.000000 novauniverse-2.0.2/novauniverse/utils/search.py
-drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.782752 novauniverse-2.0.2/novauniverse.egg-info/
--rw-rw-rw-   0        0        0     3136 2023-04-13 02:24:02.000000 novauniverse-2.0.2/novauniverse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2135 2023-04-13 02:24:02.000000 novauniverse-2.0.2/novauniverse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 02:24:02.000000 novauniverse-2.0.2/novauniverse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      153 2023-04-13 02:24:02.000000 novauniverse-2.0.2/novauniverse.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-13 02:24:02.000000 novauniverse-2.0.2/novauniverse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2819 2023-04-13 02:23:08.000000 novauniverse-2.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 02:24:02.859748 novauniverse-2.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.847748 novauniverse-2.0.2/tests/
--rw-rw-rw-   0        0        0       66 2023-03-21 20:18:52.000000 novauniverse-2.0.2/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.851748 novauniverse-2.0.2/tests/interfaces/
--rw-rw-rw-   0        0        0        0 2023-03-21 20:18:52.000000 novauniverse-2.0.2/tests/interfaces/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 02:24:02.856749 novauniverse-2.0.2/tests/interfaces/stats/
--rw-rw-rw-   0        0        0        0 2023-03-21 20:18:52.000000 novauniverse-2.0.2/tests/interfaces/stats/__init__.py
--rw-rw-rw-   0        0        0      275 2023-03-21 20:18:52.000000 novauniverse-2.0.2/tests/interfaces/stats/test_discord.py
--rw-rw-rw-   0        0        0      846 2023-03-21 20:18:52.000000 novauniverse-2.0.2/tests/interfaces/stats/test_server.py
--rw-rw-rw-   0        0        0     1806 2023-04-13 01:59:19.000000 novauniverse-2.0.2/tests/interfaces/test_mcf.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.811695 novauniverse-2.1/
+drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.607692 novauniverse-2.1/.github/
+drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.637693 novauniverse-2.1/.github/workflows/
+-rw-rw-rw-   0        0        0      830 2023-03-22 19:01:49.000000 novauniverse-2.1/.github/workflows/documentation.yaml
+-rw-rw-rw-   0        0        0      807 2023-04-13 12:53:33.000000 novauniverse-2.1/.github/workflows/lint_and_test.yaml
+-rw-rw-rw-   0        0        0       81 2023-04-13 02:18:11.000000 novauniverse-2.1/.gitignore
+-rw-rw-rw-   0        0        0     1228 2023-03-22 18:04:31.000000 novauniverse-2.1/CHANGELOG.rst
+-rw-rw-rw-   0        0        0      210 2023-04-13 13:05:33.000000 novauniverse-2.1/Makefile
+-rw-rw-rw-   0        0        0     3134 2023-04-13 14:36:51.810693 novauniverse-2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2091 2023-03-24 17:08:14.000000 novauniverse-2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.666698 novauniverse-2.1/docs/
+-rw-rw-rw-   0        0        0      654 2023-03-21 20:18:52.000000 novauniverse-2.1/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.668695 novauniverse-2.1/docs/_static/
+-rw-rw-rw-   0        0        0  1821311 2023-03-21 20:18:52.000000 novauniverse-2.1/docs/_static/logo.png
+-rw-rw-rw-   0        0        0      728 2023-03-22 17:20:14.000000 novauniverse-2.1/docs/api.rst
+-rw-rw-rw-   0        0        0     1545 2023-03-22 19:18:54.000000 novauniverse-2.1/docs/conf.py
+-rw-rw-rw-   0        0        0     1189 2023-03-22 17:55:36.000000 novauniverse-2.1/docs/events.rst
+-rw-rw-rw-   0        0        0     3301 2023-03-22 19:02:01.000000 novauniverse-2.1/docs/index.rst
+-rw-rw-rw-   0        0        0     3717 2023-04-13 14:33:57.000000 novauniverse-2.1/docs/interfaces.rst
+-rw-rw-rw-   0        0        0      398 2023-04-13 14:23:48.000000 novauniverse-2.1/docs/interfaces.stats.discord.rst
+-rw-rw-rw-   0        0        0     1449 2023-03-21 20:18:52.000000 novauniverse-2.1/docs/interfaces.stats.server.rst
+-rw-rw-rw-   0        0        0      387 2023-04-13 14:33:12.000000 novauniverse-2.1/docs/interfaces.tournaments.mcf.rst
+-rw-rw-rw-   0        0        0      443 2023-04-13 14:33:17.000000 novauniverse-2.1/docs/interfaces.tournaments.nova_games.rst
+-rw-rw-rw-   0        0        0      211 2023-04-13 14:34:06.000000 novauniverse-2.1/docs/interfaces.tournaments.rst
+-rwxrwxrwx   0        0        0      800 2023-03-21 20:18:52.000000 novauniverse-2.1/docs/make.bat
+-rw-rw-rw-   0        0        0      787 2023-04-13 14:32:57.000000 novauniverse-2.1/docs/objects.rst
+-rw-rw-rw-   0        0        0      595 2023-04-13 14:32:53.000000 novauniverse-2.1/docs/objects.tournaments.rst
+-rw-rw-rw-   0        0        0      247 2023-03-22 17:20:14.000000 novauniverse-2.1/docs/utils.rst
+drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.684700 novauniverse-2.1/novauniverse/
+-rw-rw-rw-   0        0        0     1783 2023-04-13 14:02:33.000000 novauniverse-2.1/novauniverse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.725694 novauniverse-2.1/novauniverse/api/
+-rw-rw-rw-   0        0        0     2799 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/api/__init__.py
+-rw-rw-rw-   0        0        0     1894 2023-04-13 12:41:13.000000 novauniverse-2.1/novauniverse/api/cdn.py
+-rw-rw-rw-   0        0        0     1822 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/api/endpoints.py
+-rw-rw-rw-   0        0        0     1135 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/api/errors.py
+-rw-rw-rw-   0        0        0      554 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/configuration.py
+-rw-rw-rw-   0        0        0      417 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/errors.py
+-rw-rw-rw-   0        0        0     4082 2023-04-13 12:42:35.000000 novauniverse-2.1/novauniverse/event_client.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.733694 novauniverse-2.1/novauniverse/events/
+-rw-rw-rw-   0        0        0     3877 2023-03-22 17:20:14.000000 novauniverse-2.1/novauniverse/events/__init__.py
+-rw-rw-rw-   0        0        0      494 2023-03-22 17:20:14.000000 novauniverse-2.1/novauniverse/events/client_ready.py
+-rw-rw-rw-   0        0        0     1162 2023-03-22 17:20:14.000000 novauniverse-2.1/novauniverse/events/player_join.py
+-rw-rw-rw-   0        0        0     1045 2023-03-22 17:20:14.000000 novauniverse-2.1/novauniverse/events/player_leave.py
+-rw-rw-rw-   0        0        0      354 2023-04-13 14:35:46.000000 novauniverse-2.1/novauniverse/info.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.734693 novauniverse-2.1/novauniverse/interfaces/
+-rw-rw-rw-   0        0        0     2100 2023-04-13 13:20:40.000000 novauniverse-2.1/novauniverse/interfaces/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.736696 novauniverse-2.1/novauniverse/interfaces/stats/
+-rw-rw-rw-   0        0        0        0 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/interfaces/stats/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.740693 novauniverse-2.1/novauniverse/interfaces/stats/discord/
+-rw-rw-rw-   0        0        0      541 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/interfaces/stats/discord/__init__.py
+-rw-rw-rw-   0        0        0      781 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/interfaces/stats/discord/discord_stats.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.756694 novauniverse-2.1/novauniverse/interfaces/stats/server/
+-rw-rw-rw-   0        0        0     1024 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/interfaces/stats/server/__init__.py
+-rw-rw-rw-   0        0        0      551 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/interfaces/stats/server/global_.py
+-rw-rw-rw-   0        0        0     1001 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/interfaces/stats/server/nova_online_player.py
+-rw-rw-rw-   0        0        0     1022 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/interfaces/stats/server/nova_server.py
+-rw-rw-rw-   0        0        0      666 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/interfaces/stats/server/player_preview.py
+-rw-rw-rw-   0        0        0     1926 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/interfaces/stats/server/server_info.py
+-rw-rw-rw-   0        0        0      344 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/interfaces/stats/server/system.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.759695 novauniverse-2.1/novauniverse/interfaces/tournaments/
+-rw-rw-rw-   0        0        0     2794 2023-04-13 14:02:03.000000 novauniverse-2.1/novauniverse/interfaces/tournaments/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.763701 novauniverse-2.1/novauniverse/interfaces/tournaments/mcf/
+-rw-rw-rw-   0        0        0     1216 2023-04-13 14:02:35.000000 novauniverse-2.1/novauniverse/interfaces/tournaments/mcf/__init__.py
+-rw-rw-rw-   0        0        0      200 2023-04-13 14:01:44.000000 novauniverse-2.1/novauniverse/interfaces/tournaments/mcf/mcf_tournament.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.768695 novauniverse-2.1/novauniverse/interfaces/tournaments/nova_games/
+-rw-rw-rw-   0        0        0     1307 2023-04-13 14:01:22.000000 novauniverse-2.1/novauniverse/interfaces/tournaments/nova_games/__init__.py
+-rw-rw-rw-   0        0        0      213 2023-04-13 14:01:35.000000 novauniverse-2.1/novauniverse/interfaces/tournaments/nova_games/nova_games_tournament.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.778692 novauniverse-2.1/novauniverse/objects/
+-rw-rw-rw-   0        0        0      337 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/objects/__init__.py
+-rw-rw-rw-   0        0        0     1018 2023-03-22 14:57:55.000000 novauniverse-2.1/novauniverse/objects/nova_dataclass.py
+-rw-rw-rw-   0        0        0      653 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/objects/nova_player.py
+-rw-rw-rw-   0        0        0      355 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/objects/order_by.py
+-rw-rw-rw-   0        0        0      798 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/objects/timestamp.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.784692 novauniverse-2.1/novauniverse/objects/tournaments/
+-rw-rw-rw-   0        0        0     1697 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/objects/tournaments/__init__.py
+-rw-rw-rw-   0        0        0      975 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/objects/tournaments/tournament_player.py
+-rw-rw-rw-   0        0        0      906 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/objects/tournaments/tournament_team.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.788701 novauniverse-2.1/novauniverse/utils/
+-rw-rw-rw-   0        0        0       36 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/utils/__init__.py
+-rw-rw-rw-   0        0        0     1920 2023-04-13 02:05:26.000000 novauniverse-2.1/novauniverse/utils/search.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.718692 novauniverse-2.1/novauniverse.egg-info/
+-rw-rw-rw-   0        0        0     3134 2023-04-13 14:36:51.000000 novauniverse-2.1/novauniverse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2563 2023-04-13 14:36:51.000000 novauniverse-2.1/novauniverse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 14:36:51.000000 novauniverse-2.1/novauniverse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      153 2023-04-13 14:36:51.000000 novauniverse-2.1/novauniverse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-13 14:36:51.000000 novauniverse-2.1/novauniverse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2901 2023-04-13 12:53:43.000000 novauniverse-2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 14:36:51.811695 novauniverse-2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.793694 novauniverse-2.1/tests/
+-rw-rw-rw-   0        0        0       66 2023-03-21 20:18:52.000000 novauniverse-2.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.796694 novauniverse-2.1/tests/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-03-21 20:18:52.000000 novauniverse-2.1/tests/interfaces/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.802694 novauniverse-2.1/tests/interfaces/stats/
+-rw-rw-rw-   0        0        0        0 2023-03-21 20:18:52.000000 novauniverse-2.1/tests/interfaces/stats/__init__.py
+-rw-rw-rw-   0        0        0      275 2023-03-21 20:18:52.000000 novauniverse-2.1/tests/interfaces/stats/test_discord.py
+-rw-rw-rw-   0        0        0      846 2023-03-21 20:18:52.000000 novauniverse-2.1/tests/interfaces/stats/test_server.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.808692 novauniverse-2.1/tests/interfaces/tournaments/
+-rw-rw-rw-   0        0        0        0 2023-04-13 14:07:39.000000 novauniverse-2.1/tests/interfaces/tournaments/__init__.py
+-rw-rw-rw-   0        0        0     1565 2023-04-13 14:18:56.000000 novauniverse-2.1/tests/interfaces/tournaments/test_mcf.py
+-rw-rw-rw-   0        0        0     1645 2023-04-13 14:18:06.000000 novauniverse-2.1/tests/interfaces/tournaments/test_nova_games.py
```

### Comparing `novauniverse-2.0.2/.github/workflows/documentation.yaml` & `novauniverse-2.1/.github/workflows/documentation.yaml`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/CHANGELOG.rst` & `novauniverse-2.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/PKG-INFO` & `novauniverse-2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: novauniverse
-Version: 2.0.2
+Version: 2.1
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
-Metadata-Version: 2.1 Name: novauniverse Version: 2.0.2 Summary: A modern &
+Metadata-Version: 2.1 Name: novauniverse Version: 2.1 Summary: A modern &
 maintained wrapper for the Nova Universe API written in ð Python. Author-
 email: Goldy
 devgoldy.me> Project-URL: GitHub, https://github.com/NovaUniverse/
 NovaUniverse.py Project-URL: BugTracker, https://github.com/NovaUniverse/
 NovaUniverse.py/issues Project-URL: ChangeLog, https://github.com/NovaUniverse/
 NovaUniverse.py/blob/main/CHANGELOG.rst Keywords: novauniverse,minecraft
 novauniverse,nova universe,mc novauniverse Classifier: Operating System ::
```

### Comparing `novauniverse-2.0.2/README.md` & `novauniverse-2.1/README.md`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/docs/Makefile` & `novauniverse-2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/docs/_static/logo.png` & `novauniverse-2.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/docs/api.rst` & `novauniverse-2.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/docs/conf.py` & `novauniverse-2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/docs/events.rst` & `novauniverse-2.1/docs/events.rst`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/docs/index.rst` & `novauniverse-2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/docs/interfaces.rst` & `novauniverse-2.1/docs/interfaces.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Interfaces 🧩
 ===============================
 
 .. toctree::
    :maxdepth: 1
 
-   interfaces.mcf
+   interfaces.tournaments.mcf
+   interfaces.tournaments.nova_games
    interfaces.stats.discord
    interfaces.stats.server
 
-
 .. _The Interface:
 
 The Interface ✨
 ------------------
 The easiest way to retrieve data from the Nova api using NovaUniverse.py is by using the interfaces available to you. As of March 2023, this api wrapper covers some of the novauniverse api's endpoints with an interface.
 
    **Here's a quick showcase on how to use them.**
@@ -111,7 +111,15 @@
 
 Interface Reference
 ---------------------
 .. automodule:: novauniverse.interfaces
    :members:
    :undoc-members:
    :show-inheritance:
+
+
+Other interfaces
+------------------
+.. toctree::
+   :maxdepth: 1
+
+   interfaces.tournaments
```

### Comparing `novauniverse-2.0.2/docs/interfaces.stats.server.rst` & `novauniverse-2.1/docs/interfaces.stats.server.rst`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/docs/make.bat` & `novauniverse-2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/docs/objects.rst` & `novauniverse-2.1/docs/objects.rst`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/novauniverse/__init__.py` & `novauniverse-2.1/novauniverse/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 """🐉 NovaUniverse.py config."""
 
 # Endpoint Interfaces.
 # ------------------------
 #from .interfaces.news import News
 from .interfaces.stats.discord import Discord
 from .interfaces.stats.server import Server, NovaOnlinePlayer
-from .interfaces.mcf import MCF
-#from .interfaces.nova_games import NovaGames
+from .interfaces.tournaments.mcf import MCF
+from .interfaces.tournaments.nova_games import NovaGames
 
 
 # Events
 # ------------------------
 from .events import Events
 from .event_client import EventClient
```

### Comparing `novauniverse-2.0.2/novauniverse/api/__init__.py` & `novauniverse-2.1/novauniverse/api/__init__.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/novauniverse/api/cdn.py` & `novauniverse-2.1/novauniverse/api/cdn.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import requests
 
-from .errors import *
+from . import errors
 from .. import config
 
 from . import NovaAPI
 
 class NovaCDN(NovaAPI):
     """Class used to interact with CDN server at ``https://novauniverse.net/cdn/``."""
     def __init__(self, endpoint: str = None, silence_endpoint_warning:bool=False):
@@ -24,20 +24,20 @@
             else:
                 return True
         return None
 
     def get(self) -> requests.Response:
         """Send a get request to that CDN endpoint."""
 
-        if self.endpoint is None: raise NoEndpointPassed()
+        if self.endpoint is None: raise errors.NoEndpointPassed()
         if config.performance_mode is False: # Does online check if performance mode is not enabled.
-            if self.is_online is False: raise FailedConnectivityCheck()
+            if self.is_online is False: raise errors.FailedConnectivityCheck()
 
         self.logger.info(f"Sending cdn get request to '{self.endpoint}'...")
         response_file = self.__http_session.get(self.endpoint)
 
         if response_file.status_code == 200:
             self.logger.info(f"CDN get request of '{self.endpoint}' was successful!")
             return response_file
         else:
             # I think all the error messages in the CDN are spit out in plain text on HTML. I'm not sure though. (Create a github issue if there's an issue with this anywhere.)
-            raise UnSuccessfulOperation(response_file.text)
+            raise errors.UnSuccessfulOperation(response_file.text)
```

### Comparing `novauniverse-2.0.2/novauniverse/api/endpoints.py` & `novauniverse-2.1/novauniverse/api/endpoints.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/novauniverse/api/errors.py` & `novauniverse-2.1/novauniverse/api/errors.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/novauniverse/configuration.py` & `novauniverse-2.1/novauniverse/configuration.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/novauniverse/event_client.py` & `novauniverse-2.1/novauniverse/event_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
-import sys
 import time
-from typing import List, Type, NoReturn, Dict, Callable
+from typing import List, Type, NoReturn, Dict
 from devgoldyutils import LoggerAdapter
 
 import logging
 from . import nova_logger
 
 from .api import NovaAPI
 from .events import Event, EndpointEvent, Events
@@ -65,15 +64,15 @@
     # Decorator shit
     # ---------------
     def on_event(self, event: Events) -> None:
         """Decorator that allows you to run a function when an event occurs on NovaUniverse network."""
         # I'm using issubclass() here instead of isinstance() because these are just references to a class and not an actual instance of a class. 
         # Hence isinstance() will not work for my case.
         if issubclass(event.value, EndpointEvent):
-            if not event.value in [event.__class__ for endpoint in self.__endpoint_events for event in self.__endpoint_events[endpoint]]:
+            if event.value not in [event.__class__ for endpoint in self.__endpoint_events for event in self.__endpoint_events[endpoint]]:
                 self.add_event(event.value)
 
         # Handle other type of events here...
 
         def inner(func):
             # Add function to event trigger list.
             self.get_event_instance(event.value).add_function(func)
@@ -91,15 +90,15 @@
 
             while self.__stop is not True:
                 self.logger.debug("❤")
                 
                 for endpoint in self.__endpoint_events:
                     data = None
 
-                    if not endpoint is None:
+                    if endpoint is not None:
                         data = NovaAPI(endpoint).get()
 
                     for event in self.__endpoint_events[endpoint]:
                         if event.loop(data) is True: event.trigger_event()
 
                 self.logger.debug("\x1b[31;20m" + "❤" + "\x1b[0m" + "\n")
```

### Comparing `novauniverse-2.0.2/novauniverse/events/__init__.py` & `novauniverse-2.1/novauniverse/events/__init__.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/novauniverse/events/player_join.py` & `novauniverse-2.1/novauniverse/events/player_join.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/novauniverse/events/player_leave.py` & `novauniverse-2.1/novauniverse/events/player_leave.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/novauniverse/interfaces/__init__.py` & `novauniverse-2.1/novauniverse/interfaces/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     """A basic interface, nothing more... nothing less..."""
     # TODO: Change this docstring lmao
 
     def __init__(self) -> None:
         super().__init__()
 
 
-# TODO: Finish this off..
 class SearchInterface(ABC, Interface):
     """Adds searching to a basic NU.PY interface. Use this to add searching functionality to your interfaces."""
     def __init__(self, supports: List[SearchBy], keys: Dict[SearchBy, str]) -> None:
         self.__supports = supports
         self.__keys = keys
 
         self.logger = LoggerAdapter(nova_logger, prefix="SearchInterface")
@@ -36,15 +35,15 @@
 
         if isinstance(query, str) or isinstance(query, int):
             if query.isnumeric():
                 query = Search(id = query)
             else:
                 query = Search(name = query)
 
-        if not query.search_by in self.__supports:
+        if query.search_by not in self.__supports:
             query.not_supported(self)
 
         self.logger.debug(f"Searching in '{self.__class__.__name__}' by '{query.search_by.name}' for '{query.get_query()}'...")
         # TODO: Add fuzzy search in the future.
         for object in objects:
             if object.__dict__[self.__keys[query.search_by]] == query.get_query():
                 self.logger.info(f"Found {query.get_query()} by '{query.search_by.name}'.")
```

### Comparing `novauniverse-2.0.2/novauniverse/interfaces/mcf/__init__.py` & `novauniverse-2.1/novauniverse/interfaces/tournaments/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,54 @@
 from __future__ import annotations
 
-from .. import SearchInterface, SearchBy, Search, NovaAPI, Endpoints
-from .mcf_tournament import MCFTournament
-from ... import objects
-from ...objects.order_by import OrderByNotSupported
-
+from abc import abstractmethod
 from typing import List, Dict
 
-class MCF(SearchInterface):
+from .. import SearchInterface
+
+from novauniverse import objects
+from novauniverse.utils.search import SearchBy, Search
+from novauniverse.objects.order_by import OrderByNotSupported
+
+class TournamentInterface(SearchInterface):
     """
-    The interface for NovaAPI's ``/mcf`` endpoint.
-    Allows you to get latest, get all and search for 🔥mcf tournaments.
+    Tournaments at novauniverse are very similar so I made a whole separate interface class for it inheriting from the search interface. 
+    Use this for all tournaments, components in this class can be overridden and added to if needed.
     """
-    def __init__(self):
-        super().__init__(
-            supports = [SearchBy.ID, SearchBy.NAME],
-            keys = {
-                SearchBy.ID: "id",
-                SearchBy.NAME: "display_name"
-            }
-            
-        )
+    def __init__(
+        self, 
+        supports = [SearchBy.ID, SearchBy.NAME],
+        keys = {
+            SearchBy.ID: "id",
+            SearchBy.NAME: "display_name"
+        }
+    ) -> None:
+        super().__init__(supports, keys)
 
-        self.mcf_result_api = NovaAPI(Endpoints.MCF_RESULT)
-
-    def search(self, query: Search | int | str) -> MCFTournament | None:
-        """Search for an mcf tournament!"""
+    def search(self, query: Search | int | str) -> objects.NovaBasicTournament | None:
+        """Search for a tournament! Returns None if not found."""
         return super().search(query, self.get_all())
 
-    def get_all(self) -> List[MCFTournament]:
-        """Returns all 🔥mcf tournament results from api in a list. Returns empty list if none."""
-        return [MCFTournament(tournament_data) for tournament_data in self.mcf_result_api.get()]
-
-    def get_latest(self) -> MCFTournament | None:
-        """Returns the latest 🔥mcf tournament result from api. Returns None if there are no tournaments."""
-        data = self.mcf_result_api.get()
-        data.reverse()
-
-        return (lambda uwu: None if uwu is [] else MCFTournament(uwu[0]))(data)
+    @abstractmethod
+    def get_all(self) -> List[objects.NovaBasicTournament]:
+        """Returns all tournaments from the api in a list. Returns empty list if none."""
+        ...
+
+    @abstractmethod
+    def get_latest(self) -> objects.NovaBasicTournament | None:
+        """Returns the latest tournaments from the api. Returns None if there are no tournaments."""
+        ...
 
     def get_top_players(self, order_by: objects.OrderBy = 0, max_players: int = 15) -> List[objects.TournamentPlayer]:
         """
-        Returns the top ranked players based on your parameters.
+        Returns the top ranked players in this tournament based on your parameters.
         
-        This method returns a list of ``novauniverse.objects.tournaments.tournament_player.TournamentPlayer`` but with all scores and kills from previous tournaments combined.
+        This method returns a list of :py:meth:`~novauniverse.objects.tournaments.tournament_player.TournamentPlayer` but with all scores and kills from previous tournaments combined.
         """
-        players:Dict[str, objects.TournamentPlayer] = {}
+        players: Dict[str, objects.TournamentPlayer] = {}
 
         if isinstance(order_by, objects.OrderBy): order_by = order_by.value
 
         if order_by in [0, 1]:
             for player in [player for mcf in self.get_all() for player in mcf.players]:
                 if player.uuid in players:
                     players[player.uuid].score += player.score
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `novauniverse-2.0.2/novauniverse/interfaces/stats/discord/__init__.py` & `novauniverse-2.1/novauniverse/interfaces/stats/discord/__init__.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/novauniverse/interfaces/stats/discord/discord_stats.py` & `novauniverse-2.1/novauniverse/interfaces/stats/discord/discord_stats.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/novauniverse/interfaces/stats/server/__init__.py` & `novauniverse-2.1/novauniverse/interfaces/stats/server/__init__.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/novauniverse/interfaces/stats/server/global_.py` & `novauniverse-2.1/novauniverse/interfaces/stats/server/global_.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/novauniverse/interfaces/stats/server/nova_online_player.py` & `novauniverse-2.1/novauniverse/interfaces/stats/server/nova_online_player.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/novauniverse/interfaces/stats/server/nova_server.py` & `novauniverse-2.1/novauniverse/interfaces/stats/server/nova_server.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/novauniverse/interfaces/stats/server/player_preview.py` & `novauniverse-2.1/novauniverse/interfaces/stats/server/player_preview.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/novauniverse/interfaces/stats/server/server_info.py` & `novauniverse-2.1/novauniverse/interfaces/stats/server/server_info.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/novauniverse/objects/nova_dataclass.py` & `novauniverse-2.1/novauniverse/objects/nova_dataclass.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/novauniverse/objects/nova_player.py` & `novauniverse-2.1/novauniverse/objects/nova_player.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/novauniverse/objects/timestamp.py` & `novauniverse-2.1/novauniverse/objects/timestamp.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/novauniverse/objects/tournaments/__init__.py` & `novauniverse-2.1/novauniverse/objects/tournaments/__init__.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/novauniverse/objects/tournaments/tournament_player.py` & `novauniverse-2.1/novauniverse/objects/tournaments/tournament_player.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/novauniverse/objects/tournaments/tournament_team.py` & `novauniverse-2.1/novauniverse/objects/tournaments/tournament_team.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/novauniverse/utils/search.py` & `novauniverse-2.1/novauniverse/utils/search.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/novauniverse.egg-info/PKG-INFO` & `novauniverse-2.1/novauniverse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: novauniverse
-Version: 2.0.2
+Version: 2.1
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
-Metadata-Version: 2.1 Name: novauniverse Version: 2.0.2 Summary: A modern &
+Metadata-Version: 2.1 Name: novauniverse Version: 2.1 Summary: A modern &
 maintained wrapper for the Nova Universe API written in ð Python. Author-
 email: Goldy
 devgoldy.me> Project-URL: GitHub, https://github.com/NovaUniverse/
 NovaUniverse.py Project-URL: BugTracker, https://github.com/NovaUniverse/
 NovaUniverse.py/issues Project-URL: ChangeLog, https://github.com/NovaUniverse/
 NovaUniverse.py/blob/main/CHANGELOG.rst Keywords: novauniverse,minecraft
 novauniverse,nova universe,mc novauniverse Classifier: Operating System ::
```

### Comparing `novauniverse-2.0.2/novauniverse.egg-info/SOURCES.txt` & `novauniverse-2.1/novauniverse.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 .gitignore
 CHANGELOG.rst
 Makefile
 README.md
 pyproject.toml
 .github/workflows/documentation.yaml
+.github/workflows/lint_and_test.yaml
 docs/Makefile
 docs/api.rst
 docs/conf.py
 docs/events.rst
 docs/index.rst
-docs/interfaces.mcf.rst
 docs/interfaces.rst
 docs/interfaces.stats.discord.rst
 docs/interfaces.stats.server.rst
+docs/interfaces.tournaments.mcf.rst
+docs/interfaces.tournaments.nova_games.rst
+docs/interfaces.tournaments.rst
 docs/make.bat
 docs/objects.rst
 docs/objects.tournaments.rst
 docs/utils.rst
 docs/_static/logo.png
 novauniverse/__init__.py
 novauniverse/configuration.py
@@ -33,35 +36,40 @@
 novauniverse/api/endpoints.py
 novauniverse/api/errors.py
 novauniverse/events/__init__.py
 novauniverse/events/client_ready.py
 novauniverse/events/player_join.py
 novauniverse/events/player_leave.py
 novauniverse/interfaces/__init__.py
-novauniverse/interfaces/mcf/__init__.py
-novauniverse/interfaces/mcf/mcf_tournament.py
 novauniverse/interfaces/stats/__init__.py
 novauniverse/interfaces/stats/discord/__init__.py
 novauniverse/interfaces/stats/discord/discord_stats.py
 novauniverse/interfaces/stats/server/__init__.py
 novauniverse/interfaces/stats/server/global_.py
 novauniverse/interfaces/stats/server/nova_online_player.py
 novauniverse/interfaces/stats/server/nova_server.py
 novauniverse/interfaces/stats/server/player_preview.py
 novauniverse/interfaces/stats/server/server_info.py
 novauniverse/interfaces/stats/server/system.py
+novauniverse/interfaces/tournaments/__init__.py
+novauniverse/interfaces/tournaments/mcf/__init__.py
+novauniverse/interfaces/tournaments/mcf/mcf_tournament.py
+novauniverse/interfaces/tournaments/nova_games/__init__.py
+novauniverse/interfaces/tournaments/nova_games/nova_games_tournament.py
 novauniverse/objects/__init__.py
 novauniverse/objects/nova_dataclass.py
 novauniverse/objects/nova_player.py
 novauniverse/objects/order_by.py
 novauniverse/objects/timestamp.py
 novauniverse/objects/tournaments/__init__.py
 novauniverse/objects/tournaments/tournament_player.py
 novauniverse/objects/tournaments/tournament_team.py
 novauniverse/utils/__init__.py
 novauniverse/utils/search.py
 tests/__init__.py
 tests/interfaces/__init__.py
-tests/interfaces/test_mcf.py
 tests/interfaces/stats/__init__.py
 tests/interfaces/stats/test_discord.py
-tests/interfaces/stats/test_server.py
+tests/interfaces/stats/test_server.py
+tests/interfaces/tournaments/__init__.py
+tests/interfaces/tournaments/test_mcf.py
+tests/interfaces/tournaments/test_nova_games.py
```

### Comparing `novauniverse-2.0.2/pyproject.toml` & `novauniverse-2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     'Programming Language :: Python :: 3.11'
 ]
 dependencies = [
     "requests",
     "importlib-metadata; python_version<'3.8'",
     "devgoldyutils>=2.4.3",
     "prettyprinter",
-    "python-decouple>=3.7"
+    "python-decouple>=3.8"
 ]
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
     "ruff",
@@ -57,15 +57,15 @@
 
 # Ruff
 # ---------------
 
 [tool.ruff]
 # Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
 select = ["E", "F"]
-ignore = ["E501", "E402", "E702"]
+ignore = ["E501", "E402", "E702", "E701"]
 
 # Allow autofix for all enabled rules (when `--fix`) is provided.
 fixable = ["A", "B", "C", "D", "E", "F", "G", "I", "N", "Q", "S", "T", "W", "ANN", "ARG", "BLE", "COM", "DJ", "DTZ", "EM", "ERA", "EXE", "FBT", "ICN", "INP", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PT", "PTH", "PYI", "RET", "RSE", "RUF", "SIM", "SLF", "TCH", "TID", "TRY", "UP", "YTT"]
 unfixable = []
 
 # Exclude a variety of commonly ignored directories.
 exclude = [
@@ -97,8 +97,11 @@
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
 target-version = "py38"
 
 [tool.ruff.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
-max-complexity = 10
+max-complexity = 10
+
+[tool.ruff.per-file-ignores]
+"__init__.py" = ["F401", "F403", "F405"]
```

### Comparing `novauniverse-2.0.2/tests/interfaces/stats/test_server.py` & `novauniverse-2.1/tests/interfaces/stats/test_server.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0.2/tests/interfaces/test_mcf.py` & `novauniverse-2.1/tests/interfaces/tournaments/test_nova_games.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 import requests
-from .. import MCF
+from ... import NovaGames
 
 from dataclasses import asdict
-from typing import List, Dict
+from typing import Dict
 
-def test_mcf_get_all():
-    data_from_wrapper = [mcf.data for mcf in MCF().get_all()]
-    data_from_raw_request = requests.get(url="https://api.novauniverse.net/v1/tournaments/mcf/result").json()
+data_from_raw_request = requests.get(url="https://api.novauniverse.net/v1/tournaments/nova_games/result").json()
+
+def test_nova_games_get_all():
+    data_from_wrapper = [nova_games.data for nova_games in NovaGames().get_all()]
 
     assert data_from_raw_request == data_from_wrapper
 
-def test_mcf_get_latest():
-    data_from_wrapper = MCF().get_latest().data
-    data_from_raw_request = requests.get(url="https://api.novauniverse.net/v1/tournaments/mcf/result").json()[-1]
+def test_nova_games_get_latest():
+    data_from_wrapper = NovaGames().get_latest().data
 
-    assert data_from_raw_request == data_from_wrapper
+    assert data_from_raw_request[-1] == data_from_wrapper
 
-def test_mcf_get_top_players():
-    data_from_wrapper = [asdict(player) for player in MCF().get_top_players()]
+def test_nova_games_get_top_players():
+    data_from_wrapper = [asdict(player) for player in NovaGames().get_top_players()]
     
     count = 0
     for player in data_from_wrapper:
         del player["data"]; del player["logger"]; del player["name"]
         data_from_wrapper[count] = player
 
         count += 1
 
-    data_from_raw_request: List[dict] = requests.get(url="https://api.novauniverse.net/v1/tournaments/mcf/result").json()
-
     players: Dict[str, dict] = {}
 
-    for player in [player for mcf in data_from_raw_request for player in mcf["players"]]:
+    for player in [player for nova_games in data_from_raw_request for player in nova_games["players"]]:
         if player["uuid"] in players:
             players[player["uuid"]]["score"] = player["score"] + players[player["uuid"]]["score"]
             players[player["uuid"]]["kills"] = player["kills"] + players[player["uuid"]]["kills"]
         else:
             player["team_number"] = None; player["uid"] = None # We null these properties as they are irrelevant and are different in every tournament.
             players[player["uuid"]] = player
 
-    data_from_raw_request = [item[1] for item in sorted(players.items(), key=lambda x: x[1]["score"], reverse=True)[:15]]
+    _data_from_raw_request = [item[1] for item in sorted(players.items(), key=lambda x: x[1]["score"], reverse=True)[:15]]
 
-    assert data_from_raw_request == data_from_wrapper
+    assert _data_from_raw_request == data_from_wrapper
```

