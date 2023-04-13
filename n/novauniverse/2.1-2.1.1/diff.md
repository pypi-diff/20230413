# Comparing `tmp/novauniverse-2.1.tar.gz` & `tmp/novauniverse-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "novauniverse-2.1.tar", last modified: Thu Apr 13 14:36:51 2023, max compression
+gzip compressed data, was "novauniverse-2.1.1.tar", last modified: Thu Apr 13 16:04:49 2023, max compression
```

## Comparing `novauniverse-2.1.tar` & `novauniverse-2.1.1.tar`

### file list

```diff
@@ -1,100 +1,67 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.811695 novauniverse-2.1/
-drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.607692 novauniverse-2.1/.github/
-drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.637693 novauniverse-2.1/.github/workflows/
--rw-rw-rw-   0        0        0      830 2023-03-22 19:01:49.000000 novauniverse-2.1/.github/workflows/documentation.yaml
--rw-rw-rw-   0        0        0      807 2023-04-13 12:53:33.000000 novauniverse-2.1/.github/workflows/lint_and_test.yaml
--rw-rw-rw-   0        0        0       81 2023-04-13 02:18:11.000000 novauniverse-2.1/.gitignore
--rw-rw-rw-   0        0        0     1228 2023-03-22 18:04:31.000000 novauniverse-2.1/CHANGELOG.rst
--rw-rw-rw-   0        0        0      210 2023-04-13 13:05:33.000000 novauniverse-2.1/Makefile
--rw-rw-rw-   0        0        0     3134 2023-04-13 14:36:51.810693 novauniverse-2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2091 2023-03-24 17:08:14.000000 novauniverse-2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.666698 novauniverse-2.1/docs/
--rw-rw-rw-   0        0        0      654 2023-03-21 20:18:52.000000 novauniverse-2.1/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.668695 novauniverse-2.1/docs/_static/
--rw-rw-rw-   0        0        0  1821311 2023-03-21 20:18:52.000000 novauniverse-2.1/docs/_static/logo.png
--rw-rw-rw-   0        0        0      728 2023-03-22 17:20:14.000000 novauniverse-2.1/docs/api.rst
--rw-rw-rw-   0        0        0     1545 2023-03-22 19:18:54.000000 novauniverse-2.1/docs/conf.py
--rw-rw-rw-   0        0        0     1189 2023-03-22 17:55:36.000000 novauniverse-2.1/docs/events.rst
--rw-rw-rw-   0        0        0     3301 2023-03-22 19:02:01.000000 novauniverse-2.1/docs/index.rst
--rw-rw-rw-   0        0        0     3717 2023-04-13 14:33:57.000000 novauniverse-2.1/docs/interfaces.rst
--rw-rw-rw-   0        0        0      398 2023-04-13 14:23:48.000000 novauniverse-2.1/docs/interfaces.stats.discord.rst
--rw-rw-rw-   0        0        0     1449 2023-03-21 20:18:52.000000 novauniverse-2.1/docs/interfaces.stats.server.rst
--rw-rw-rw-   0        0        0      387 2023-04-13 14:33:12.000000 novauniverse-2.1/docs/interfaces.tournaments.mcf.rst
--rw-rw-rw-   0        0        0      443 2023-04-13 14:33:17.000000 novauniverse-2.1/docs/interfaces.tournaments.nova_games.rst
--rw-rw-rw-   0        0        0      211 2023-04-13 14:34:06.000000 novauniverse-2.1/docs/interfaces.tournaments.rst
--rwxrwxrwx   0        0        0      800 2023-03-21 20:18:52.000000 novauniverse-2.1/docs/make.bat
--rw-rw-rw-   0        0        0      787 2023-04-13 14:32:57.000000 novauniverse-2.1/docs/objects.rst
--rw-rw-rw-   0        0        0      595 2023-04-13 14:32:53.000000 novauniverse-2.1/docs/objects.tournaments.rst
--rw-rw-rw-   0        0        0      247 2023-03-22 17:20:14.000000 novauniverse-2.1/docs/utils.rst
-drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.684700 novauniverse-2.1/novauniverse/
--rw-rw-rw-   0        0        0     1783 2023-04-13 14:02:33.000000 novauniverse-2.1/novauniverse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.725694 novauniverse-2.1/novauniverse/api/
--rw-rw-rw-   0        0        0     2799 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/api/__init__.py
--rw-rw-rw-   0        0        0     1894 2023-04-13 12:41:13.000000 novauniverse-2.1/novauniverse/api/cdn.py
--rw-rw-rw-   0        0        0     1822 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/api/endpoints.py
--rw-rw-rw-   0        0        0     1135 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/api/errors.py
--rw-rw-rw-   0        0        0      554 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/configuration.py
--rw-rw-rw-   0        0        0      417 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/errors.py
--rw-rw-rw-   0        0        0     4082 2023-04-13 12:42:35.000000 novauniverse-2.1/novauniverse/event_client.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.733694 novauniverse-2.1/novauniverse/events/
--rw-rw-rw-   0        0        0     3877 2023-03-22 17:20:14.000000 novauniverse-2.1/novauniverse/events/__init__.py
--rw-rw-rw-   0        0        0      494 2023-03-22 17:20:14.000000 novauniverse-2.1/novauniverse/events/client_ready.py
--rw-rw-rw-   0        0        0     1162 2023-03-22 17:20:14.000000 novauniverse-2.1/novauniverse/events/player_join.py
--rw-rw-rw-   0        0        0     1045 2023-03-22 17:20:14.000000 novauniverse-2.1/novauniverse/events/player_leave.py
--rw-rw-rw-   0        0        0      354 2023-04-13 14:35:46.000000 novauniverse-2.1/novauniverse/info.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.734693 novauniverse-2.1/novauniverse/interfaces/
--rw-rw-rw-   0        0        0     2100 2023-04-13 13:20:40.000000 novauniverse-2.1/novauniverse/interfaces/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.736696 novauniverse-2.1/novauniverse/interfaces/stats/
--rw-rw-rw-   0        0        0        0 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/interfaces/stats/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.740693 novauniverse-2.1/novauniverse/interfaces/stats/discord/
--rw-rw-rw-   0        0        0      541 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/interfaces/stats/discord/__init__.py
--rw-rw-rw-   0        0        0      781 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/interfaces/stats/discord/discord_stats.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.756694 novauniverse-2.1/novauniverse/interfaces/stats/server/
--rw-rw-rw-   0        0        0     1024 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/interfaces/stats/server/__init__.py
--rw-rw-rw-   0        0        0      551 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/interfaces/stats/server/global_.py
--rw-rw-rw-   0        0        0     1001 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/interfaces/stats/server/nova_online_player.py
--rw-rw-rw-   0        0        0     1022 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/interfaces/stats/server/nova_server.py
--rw-rw-rw-   0        0        0      666 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/interfaces/stats/server/player_preview.py
--rw-rw-rw-   0        0        0     1926 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/interfaces/stats/server/server_info.py
--rw-rw-rw-   0        0        0      344 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/interfaces/stats/server/system.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.759695 novauniverse-2.1/novauniverse/interfaces/tournaments/
--rw-rw-rw-   0        0        0     2794 2023-04-13 14:02:03.000000 novauniverse-2.1/novauniverse/interfaces/tournaments/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.763701 novauniverse-2.1/novauniverse/interfaces/tournaments/mcf/
--rw-rw-rw-   0        0        0     1216 2023-04-13 14:02:35.000000 novauniverse-2.1/novauniverse/interfaces/tournaments/mcf/__init__.py
--rw-rw-rw-   0        0        0      200 2023-04-13 14:01:44.000000 novauniverse-2.1/novauniverse/interfaces/tournaments/mcf/mcf_tournament.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.768695 novauniverse-2.1/novauniverse/interfaces/tournaments/nova_games/
--rw-rw-rw-   0        0        0     1307 2023-04-13 14:01:22.000000 novauniverse-2.1/novauniverse/interfaces/tournaments/nova_games/__init__.py
--rw-rw-rw-   0        0        0      213 2023-04-13 14:01:35.000000 novauniverse-2.1/novauniverse/interfaces/tournaments/nova_games/nova_games_tournament.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.778692 novauniverse-2.1/novauniverse/objects/
--rw-rw-rw-   0        0        0      337 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/objects/__init__.py
--rw-rw-rw-   0        0        0     1018 2023-03-22 14:57:55.000000 novauniverse-2.1/novauniverse/objects/nova_dataclass.py
--rw-rw-rw-   0        0        0      653 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/objects/nova_player.py
--rw-rw-rw-   0        0        0      355 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/objects/order_by.py
--rw-rw-rw-   0        0        0      798 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/objects/timestamp.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.784692 novauniverse-2.1/novauniverse/objects/tournaments/
--rw-rw-rw-   0        0        0     1697 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/objects/tournaments/__init__.py
--rw-rw-rw-   0        0        0      975 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/objects/tournaments/tournament_player.py
--rw-rw-rw-   0        0        0      906 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/objects/tournaments/tournament_team.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.788701 novauniverse-2.1/novauniverse/utils/
--rw-rw-rw-   0        0        0       36 2023-03-21 20:18:52.000000 novauniverse-2.1/novauniverse/utils/__init__.py
--rw-rw-rw-   0        0        0     1920 2023-04-13 02:05:26.000000 novauniverse-2.1/novauniverse/utils/search.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.718692 novauniverse-2.1/novauniverse.egg-info/
--rw-rw-rw-   0        0        0     3134 2023-04-13 14:36:51.000000 novauniverse-2.1/novauniverse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2563 2023-04-13 14:36:51.000000 novauniverse-2.1/novauniverse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 14:36:51.000000 novauniverse-2.1/novauniverse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      153 2023-04-13 14:36:51.000000 novauniverse-2.1/novauniverse.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-13 14:36:51.000000 novauniverse-2.1/novauniverse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2901 2023-04-13 12:53:43.000000 novauniverse-2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 14:36:51.811695 novauniverse-2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.793694 novauniverse-2.1/tests/
--rw-rw-rw-   0        0        0       66 2023-03-21 20:18:52.000000 novauniverse-2.1/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.796694 novauniverse-2.1/tests/interfaces/
--rw-rw-rw-   0        0        0        0 2023-03-21 20:18:52.000000 novauniverse-2.1/tests/interfaces/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.802694 novauniverse-2.1/tests/interfaces/stats/
--rw-rw-rw-   0        0        0        0 2023-03-21 20:18:52.000000 novauniverse-2.1/tests/interfaces/stats/__init__.py
--rw-rw-rw-   0        0        0      275 2023-03-21 20:18:52.000000 novauniverse-2.1/tests/interfaces/stats/test_discord.py
--rw-rw-rw-   0        0        0      846 2023-03-21 20:18:52.000000 novauniverse-2.1/tests/interfaces/stats/test_server.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:36:51.808692 novauniverse-2.1/tests/interfaces/tournaments/
--rw-rw-rw-   0        0        0        0 2023-04-13 14:07:39.000000 novauniverse-2.1/tests/interfaces/tournaments/__init__.py
--rw-rw-rw-   0        0        0     1565 2023-04-13 14:18:56.000000 novauniverse-2.1/tests/interfaces/tournaments/test_mcf.py
--rw-rw-rw-   0        0        0     1645 2023-04-13 14:18:06.000000 novauniverse-2.1/tests/interfaces/tournaments/test_nova_games.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:04:49.887873 novauniverse-2.1.1/
+-rw-rw-rw-   0        0        0       81 2023-04-13 02:18:11.000000 novauniverse-2.1.1/.gitignore
+-rw-rw-rw-   0        0        0     1228 2023-03-22 18:04:31.000000 novauniverse-2.1.1/CHANGELOG.rst
+-rw-rw-rw-   0        0        0       38 2023-04-13 16:04:12.000000 novauniverse-2.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      210 2023-04-13 13:05:33.000000 novauniverse-2.1.1/Makefile
+-rw-rw-rw-   0        0        0     3136 2023-04-13 16:04:49.886870 novauniverse-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2091 2023-03-24 17:08:14.000000 novauniverse-2.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 16:04:49.801872 novauniverse-2.1.1/novauniverse/
+-rw-rw-rw-   0        0        0     1783 2023-04-13 14:02:33.000000 novauniverse-2.1.1/novauniverse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:04:49.829869 novauniverse-2.1.1/novauniverse/api/
+-rw-rw-rw-   0        0        0     2799 2023-03-21 20:18:52.000000 novauniverse-2.1.1/novauniverse/api/__init__.py
+-rw-rw-rw-   0        0        0     1894 2023-04-13 12:41:13.000000 novauniverse-2.1.1/novauniverse/api/cdn.py
+-rw-rw-rw-   0        0        0     1822 2023-03-21 20:18:52.000000 novauniverse-2.1.1/novauniverse/api/endpoints.py
+-rw-rw-rw-   0        0        0     1135 2023-03-21 20:18:52.000000 novauniverse-2.1.1/novauniverse/api/errors.py
+-rw-rw-rw-   0        0        0      554 2023-03-21 20:18:52.000000 novauniverse-2.1.1/novauniverse/configuration.py
+-rw-rw-rw-   0        0        0      417 2023-03-21 20:18:52.000000 novauniverse-2.1.1/novauniverse/errors.py
+-rw-rw-rw-   0        0        0     4082 2023-04-13 12:42:35.000000 novauniverse-2.1.1/novauniverse/event_client.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:04:49.836870 novauniverse-2.1.1/novauniverse/events/
+-rw-rw-rw-   0        0        0     3877 2023-03-22 17:20:14.000000 novauniverse-2.1.1/novauniverse/events/__init__.py
+-rw-rw-rw-   0        0        0      494 2023-03-22 17:20:14.000000 novauniverse-2.1.1/novauniverse/events/client_ready.py
+-rw-rw-rw-   0        0        0     1162 2023-03-22 17:20:14.000000 novauniverse-2.1.1/novauniverse/events/player_join.py
+-rw-rw-rw-   0        0        0     1045 2023-03-22 17:20:14.000000 novauniverse-2.1.1/novauniverse/events/player_leave.py
+-rw-rw-rw-   0        0        0      356 2023-04-13 16:04:33.000000 novauniverse-2.1.1/novauniverse/info.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:04:49.838868 novauniverse-2.1.1/novauniverse/interfaces/
+-rw-rw-rw-   0        0        0     2100 2023-04-13 13:20:40.000000 novauniverse-2.1.1/novauniverse/interfaces/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:04:49.840867 novauniverse-2.1.1/novauniverse/interfaces/stats/
+-rw-rw-rw-   0        0        0        0 2023-03-21 20:18:52.000000 novauniverse-2.1.1/novauniverse/interfaces/stats/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:04:49.844870 novauniverse-2.1.1/novauniverse/interfaces/stats/discord/
+-rw-rw-rw-   0        0        0      541 2023-03-21 20:18:52.000000 novauniverse-2.1.1/novauniverse/interfaces/stats/discord/__init__.py
+-rw-rw-rw-   0        0        0      781 2023-03-21 20:18:52.000000 novauniverse-2.1.1/novauniverse/interfaces/stats/discord/discord_stats.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:04:49.858869 novauniverse-2.1.1/novauniverse/interfaces/stats/server/
+-rw-rw-rw-   0        0        0     1024 2023-03-21 20:18:52.000000 novauniverse-2.1.1/novauniverse/interfaces/stats/server/__init__.py
+-rw-rw-rw-   0        0        0      551 2023-03-21 20:18:52.000000 novauniverse-2.1.1/novauniverse/interfaces/stats/server/global_.py
+-rw-rw-rw-   0        0        0     1001 2023-03-21 20:18:52.000000 novauniverse-2.1.1/novauniverse/interfaces/stats/server/nova_online_player.py
+-rw-rw-rw-   0        0        0     1022 2023-03-21 20:18:52.000000 novauniverse-2.1.1/novauniverse/interfaces/stats/server/nova_server.py
+-rw-rw-rw-   0        0        0      666 2023-03-21 20:18:52.000000 novauniverse-2.1.1/novauniverse/interfaces/stats/server/player_preview.py
+-rw-rw-rw-   0        0        0     1926 2023-03-21 20:18:52.000000 novauniverse-2.1.1/novauniverse/interfaces/stats/server/server_info.py
+-rw-rw-rw-   0        0        0      344 2023-03-21 20:18:52.000000 novauniverse-2.1.1/novauniverse/interfaces/stats/server/system.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:04:49.860876 novauniverse-2.1.1/novauniverse/interfaces/tournaments/
+-rw-rw-rw-   0        0        0     2794 2023-04-13 14:02:03.000000 novauniverse-2.1.1/novauniverse/interfaces/tournaments/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:04:49.863867 novauniverse-2.1.1/novauniverse/interfaces/tournaments/mcf/
+-rw-rw-rw-   0        0        0     1216 2023-04-13 14:02:35.000000 novauniverse-2.1.1/novauniverse/interfaces/tournaments/mcf/__init__.py
+-rw-rw-rw-   0        0        0      200 2023-04-13 14:01:44.000000 novauniverse-2.1.1/novauniverse/interfaces/tournaments/mcf/mcf_tournament.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:04:49.867868 novauniverse-2.1.1/novauniverse/interfaces/tournaments/nova_games/
+-rw-rw-rw-   0        0        0     1307 2023-04-13 14:01:22.000000 novauniverse-2.1.1/novauniverse/interfaces/tournaments/nova_games/__init__.py
+-rw-rw-rw-   0        0        0      213 2023-04-13 14:01:35.000000 novauniverse-2.1.1/novauniverse/interfaces/tournaments/nova_games/nova_games_tournament.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:04:49.876870 novauniverse-2.1.1/novauniverse/objects/
+-rw-rw-rw-   0        0        0      337 2023-03-21 20:18:52.000000 novauniverse-2.1.1/novauniverse/objects/__init__.py
+-rw-rw-rw-   0        0        0     1018 2023-03-22 14:57:55.000000 novauniverse-2.1.1/novauniverse/objects/nova_dataclass.py
+-rw-rw-rw-   0        0        0      653 2023-03-21 20:18:52.000000 novauniverse-2.1.1/novauniverse/objects/nova_player.py
+-rw-rw-rw-   0        0        0      355 2023-03-21 20:18:52.000000 novauniverse-2.1.1/novauniverse/objects/order_by.py
+-rw-rw-rw-   0        0        0      798 2023-03-21 20:18:52.000000 novauniverse-2.1.1/novauniverse/objects/timestamp.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:04:49.881871 novauniverse-2.1.1/novauniverse/objects/tournaments/
+-rw-rw-rw-   0        0        0     1697 2023-03-21 20:18:52.000000 novauniverse-2.1.1/novauniverse/objects/tournaments/__init__.py
+-rw-rw-rw-   0        0        0      975 2023-03-21 20:18:52.000000 novauniverse-2.1.1/novauniverse/objects/tournaments/tournament_player.py
+-rw-rw-rw-   0        0        0      906 2023-03-21 20:18:52.000000 novauniverse-2.1.1/novauniverse/objects/tournaments/tournament_team.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:04:49.885868 novauniverse-2.1.1/novauniverse/utils/
+-rw-rw-rw-   0        0        0       36 2023-03-21 20:18:52.000000 novauniverse-2.1.1/novauniverse/utils/__init__.py
+-rw-rw-rw-   0        0        0     1920 2023-04-13 02:05:26.000000 novauniverse-2.1.1/novauniverse/utils/search.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:04:49.822867 novauniverse-2.1.1/novauniverse.egg-info/
+-rw-rw-rw-   0        0        0     3136 2023-04-13 16:04:49.000000 novauniverse-2.1.1/novauniverse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1846 2023-04-13 16:04:49.000000 novauniverse-2.1.1/novauniverse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 16:04:49.000000 novauniverse-2.1.1/novauniverse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      153 2023-04-13 16:04:49.000000 novauniverse-2.1.1/novauniverse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-13 16:04:49.000000 novauniverse-2.1.1/novauniverse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3017 2023-04-13 16:04:23.000000 novauniverse-2.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 16:04:49.887873 novauniverse-2.1.1/setup.cfg
```

### Comparing `novauniverse-2.1/CHANGELOG.rst` & `novauniverse-2.1.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `novauniverse-2.1/PKG-INFO` & `novauniverse-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: novauniverse
-Version: 2.1
+Version: 2.1.1
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
-Metadata-Version: 2.1 Name: novauniverse Version: 2.1 Summary: A modern &
+Metadata-Version: 2.1 Name: novauniverse Version: 2.1.1 Summary: A modern &
 maintained wrapper for the Nova Universe API written in ð Python. Author-
 email: Goldy
 devgoldy.me> Project-URL: GitHub, https://github.com/NovaUniverse/
 NovaUniverse.py Project-URL: BugTracker, https://github.com/NovaUniverse/
 NovaUniverse.py/issues Project-URL: ChangeLog, https://github.com/NovaUniverse/
 NovaUniverse.py/blob/main/CHANGELOG.rst Keywords: novauniverse,minecraft
 novauniverse,nova universe,mc novauniverse Classifier: Operating System ::
```

### Comparing `novauniverse-2.1/README.md` & `novauniverse-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `novauniverse-2.1/docs/events.rst` & `novauniverse-2.1.1/novauniverse/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,65 @@
-Events 🎟
-=========
-NovaUniverse.py being a feature rich api wrapper provides a collection of events that can be triggered by an action occurring on the Nova Universe Network. Like example a player joining the minecraft server.
+"""
+🐲 Nova Universe - A modern & maintained wrapper for the Nova Universe API written in Python.
 
-   This is how we register a player join event::
+Copyright (C) 2023 - Dev Goldy
+"""
 
-      from novauniverse import EventClient, Events, NovaOnlinePlayer 
+# Logging stuff
+# ---------------
+from .info import LOGGER_NAME
+from devgoldyutils.logging import add_custom_handler, log
 
-      client = EventClient()
+nova_logger = add_custom_handler(log.getLogger(LOGGER_NAME), level=log.WARNING)
+"""
+The python ``logging.Logger()`` class for NovaUniverse.py.
 
-      @client.on_event(Events.PLAYER_JOIN)
-      def on_player_join(player:NovaOnlinePlayer):
-         print(f"{player.username} joined {player.server_name}!")
+---------------
 
-      client.start()
+⭐Example:
+------------
 
-   If you would like to know the attributes of NovaOnlinePlayer, check this out: `NovaOnlinePlayer`_.
+You can disable and also adjust the level of logging from the api wrapper like this::
 
-   .. _NovaOnlinePlayer: https://nupy.devgoldy.me/NovaUniverse.py/interfaces.stats.server.html#novauniverse.interfaces.stats.server.nova_online_player.NovaOnlinePlayer
+    import logging
+    nova_logger.setLevel(logging.DEBUG)
 
+If your using the ``novauniverse.EventClient`` class, a shortcut for enabling debugging would be this::
 
-.. toctree::
-   :maxdepth: 1
+    EventClient(debug=True)
 
+If you want to completely disable logging like example remove warnings, you can do that with::
 
-EventClient Reference
----------------------------
-.. automodule:: novauniverse.event_client
-   :members:
-   :undoc-members:
-   :show-inheritance:
+    nova_logger.setLevel(logging.NOTSET)
 
+"""
 
-Events Reference
----------------------------
-.. automodule:: novauniverse.events
-   :members:
-   :undoc-members:
-   :show-inheritance:
+# Configuration
+# ---------------
+from .configuration import Config
+config = Config()
+"""🐉 NovaUniverse.py config."""
+
+# Endpoint Interfaces.
+# ------------------------
+#from .interfaces.news import News
+from .interfaces.stats.discord import Discord
+from .interfaces.stats.server import Server, NovaOnlinePlayer
+from .interfaces.tournaments.mcf import MCF
+from .interfaces.tournaments.nova_games import NovaGames
+
+
+# Events
+# ------------------------
+from .events import Events
+from .event_client import EventClient
+
+from .utils.search import Search
+
+# Backend objects
+from .objects.nova_player import NovaBasicPlayer
+from .objects.timestamp import Timestamp
+from .objects.tournaments import NovaBasicTournament, TournamentPlayer, TournamentTeam
+from .objects.order_by import OrderBy
+
+# Backend utils
+from .api import Endpoints, NovaAPI, NovaCDN
```

### Comparing `novauniverse-2.1/docs/index.rst` & `novauniverse-2.1.1/novauniverse.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,207 +1,196 @@
-00000000: 2e2e 204e 6f76 6155 6e69 7665 7273 652e  .. NovaUniverse.
-00000010: 7079 2064 6f63 756d 656e 7461 7469 6f6e  py documentation
-00000020: 206d 6173 7465 7220 6669 6c65 2c20 6372   master file, cr
-00000030: 6561 7465 6420 6279 0d0a 2020 2073 7068  eated by..   sph
-00000040: 696e 782d 7175 6963 6b73 7461 7274 206f  inx-quickstart o
-00000050: 6e20 5375 6e20 4d61 7220 3139 2032 333a  n Sun Mar 19 23:
-00000060: 3236 3a31 3020 3230 3233 2e0d 0a20 2020  26:10 2023...   
-00000070: 596f 7520 6361 6e20 6164 6170 7420 7468  You can adapt th
-00000080: 6973 2066 696c 6520 636f 6d70 6c65 7465  is file complete
-00000090: 6c79 2074 6f20 796f 7572 206c 696b 696e  ly to your likin
-000000a0: 672c 2062 7574 2069 7420 7368 6f75 6c64  g, but it should
-000000b0: 2061 7420 6c65 6173 740d 0a20 2020 636f   at least..   co
-000000c0: 6e74 6169 6e20 7468 6520 726f 6f74 2060  ntain the root `
-000000d0: 746f 6374 7265 6560 2064 6972 6563 7469  toctree` directi
-000000e0: 7665 2e0d 0a0d 0af0 9f90 8d20 6e6f 7661  ve......... nova
-000000f0: 756e 6976 6572 7365 2e70 790d 0a3d 3d3d  universe.py..===
-00000100: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000110: 3d3d 0d0a 4120 6d6f 6465 726e 2026 206d  ==..A modern & m
-00000120: 6169 6e74 6169 6e65 6420 7772 6170 7065  aintained wrappe
-00000130: 7220 666f 7220 7468 6520 604e 6f76 6120  r for the `Nova 
-00000140: 556e 6976 6572 7365 2041 5049 605f 2077  Universe API`_ w
-00000150: 7269 7474 656e 2069 6e20 5079 7468 6f6e  ritten in Python
-00000160: 2e0d 0a0d 0a2e 2e20 5f4e 6f76 6120 556e  ....... _Nova Un
-00000170: 6976 6572 7365 2041 5049 3a20 6874 7470  iverse API: http
-00000180: 733a 2f2f 6e6f 7661 756e 6976 6572 7365  s://novauniverse
-00000190: 2e6e 6574 2f61 7069 2f0d 0a0d 0a2e 2e20  .net/api/...... 
-000001a0: 746f 6374 7265 653a 3a0d 0a20 2020 3a6d  toctree::..   :m
-000001b0: 6178 6465 7074 683a 2031 0d0a 0d0a 2020  axdepth: 1....  
-000001c0: 2061 7069 0d0a 2020 2065 7665 6e74 730d   api..   events.
-000001d0: 0a20 2020 696e 7465 7266 6163 6573 0d0a  .   interfaces..
-000001e0: 2020 206f 626a 6563 7473 0d0a 2020 2075     objects..   u
-000001f0: 7469 6c73 0d0a 0d0a 0d0a 5768 6174 2069  tils......What i
-00000200: 7320 4e6f 7661 556e 6976 6572 7365 2e70  s NovaUniverse.p
-00000210: 793f 0d0a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  y?..============
-00000220: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0d0a  ==============..
-00000230: 4e6f 7661 556e 6976 6572 7365 2e70 7920  NovaUniverse.py 
-00000240: 6973 2061 2041 5049 2077 7261 7070 6572  is a API wrapper
-00000250: 2066 6f72 2022 4e6f 7661 2055 6e69 7665   for "Nova Unive
-00000260: 7273 6522 2028 6d69 6e65 6372 6166 7420  rse" (minecraft 
-00000270: 6576 656e 7420 686f 7374 696e 6720 6772  event hosting gr
-00000280: 6f75 7029 2074 6861 7420 616c 6c6f 7773  oup) that allows
-00000290: 2079 6f75 2074 6f20 696e 7465 7266 6163   you to interfac
-000002a0: 6520 7769 7468 2074 6865 204e 6f76 6120  e with the Nova 
-000002b0: 556e 6976 6572 7365 2060 4150 4960 5f20  Universe `API`_ 
-000002c0: 696e 2061 2066 6173 7420 6f62 6a65 6374  in a fast object
-000002d0: 206f 7269 656e 7465 6420 7761 7920 6e61   oriented way na
-000002e0: 7469 7665 6c79 2077 6974 6869 6e20 5079  tively within Py
-000002f0: 7468 6f6e 2e20 0d0a 4f6e 6520 6f66 2074  thon. ..One of t
-00000300: 6865 2062 6f6e 7573 6573 2069 7320 7468  he bonuses is th
-00000310: 6174 2069 7420 7761 7320 6465 7665 6c6f  at it was develo
-00000320: 7065 6420 6279 2060 4d45 605f 2c20 616e  ped by `ME`_, an
-00000330: 2061 646d 696e 2061 7420 4e6f 7661 556e   admin at NovaUn
-00000340: 6976 6572 7365 2e0d 0a0d 0a2e 2e20 5f41  iverse....... _A
-00000350: 5049 3a20 6874 7470 733a 2f2f 6e6f 7661  PI: https://nova
-00000360: 756e 6976 6572 7365 2e6e 6574 2f61 7069  universe.net/api
-00000370: 0d0a 2e2e 205f 4d45 3a20 6874 7470 733a  .... _ME: https:
-00000380: 2f2f 6769 7468 7562 2e63 6f6d 2f54 4845  //github.com/THE
-00000390: 474f 4c44 454e 5052 4f0d 0a0d 0a0d 0ae2  GOLDENPRO.......
-000003a0: 9a99 202a 496e 7374 616c 6c2f 5365 7420  .. *Install/Set 
-000003b0: 5570 3a2a 0d0a 2d2d 2d2d 2d2d 2d2d 2d2d  Up:*..----------
-000003c0: 2d2d 2d2d 2d2d 2d2d 2d0d 0a31 2e20 2a2a  ---------..1. **
-000003d0: 496e 7374 616c 6c20 7061 636b 6167 6520  Install package 
-000003e0: 6672 6f6d 2070 7970 692e 2a2a 2028 496e  from pypi.** (In
-000003f0: 2064 6576 656c 6f70 6d65 6e74 2073 6f20   development so 
-00000400: 6e6f 2050 7950 6920 7061 636b 6167 6520  no PyPi package 
-00000410: 7965 742c 2069 6e73 7461 6c6c 2076 6961  yet, install via
-00000420: 2047 6974 4875 6220 696e 7374 6561 642e   GitHub instead.
-00000430: 293a 3a0d 0a0d 0a20 2020 2020 2023 5769  )::....      #Wi
-00000440: 6e64 6f77 732f 4c69 6e75 780d 0a0d 0a20  ndows/Linux.... 
-00000450: 2020 2020 2070 6970 2069 6e73 7461 6c6c       pip install
-00000460: 206e 6f76 6175 6e69 7665 7273 650d 0a0d   novauniverse...
-00000470: 0a32 2e20 2a2a 5468 6174 2773 2049 7421  .2. **That's It!
-00000480: 2a2a 202d 202a 4272 6965 6620 4578 616d  ** - *Brief Exam
-00000490: 706c 6520 4265 6c6f 772a 3a3a 0d0a 0d0a  ple Below*::....
-000004a0: 2020 2020 2020 6672 6f6d 206e 6f76 6175        from novau
-000004b0: 6e69 7665 7273 6520 696d 706f 7274 2045  niverse import E
-000004c0: 7665 6e74 436c 6965 6e74 2c20 4576 656e  ventClient, Even
-000004d0: 7473 2c20 4e6f 7661 4f6e 6c69 6e65 506c  ts, NovaOnlinePl
-000004e0: 6179 6572 200d 0a0d 0a20 2020 2020 2063  ayer ....      c
-000004f0: 6c69 656e 7420 3d20 4576 656e 7443 6c69  lient = EventCli
-00000500: 656e 7428 290d 0a0d 0a20 2020 2020 2040  ent()....      @
-00000510: 636c 6965 6e74 2e6f 6e5f 6576 656e 7428  client.on_event(
-00000520: 4576 656e 7473 2e43 4c49 454e 545f 5245  Events.CLIENT_RE
-00000530: 4144 5929 0d0a 2020 2020 2020 6465 6620  ADY)..      def 
-00000540: 636c 6965 6e74 5f69 735f 7265 6164 7928  client_is_ready(
-00000550: 293a 0d0a 2020 2020 2020 2020 2070 7269  ):..         pri
-00000560: 6e74 2822 436c 6965 6e74 2069 7320 7265  nt("Client is re
-00000570: 6164 7921 2229 0d0a 0d0a 2020 2020 2020  ady!")....      
-00000580: 4063 6c69 656e 742e 6f6e 5f65 7665 6e74  @client.on_event
-00000590: 2845 7665 6e74 732e 504c 4159 4552 5f4a  (Events.PLAYER_J
-000005a0: 4f49 4e29 0d0a 2020 2020 2020 6465 6620  OIN)..      def 
-000005b0: 6f6e 5f70 6c61 7965 725f 6a6f 696e 2870  on_player_join(p
-000005c0: 6c61 7965 723a 204e 6f76 614f 6e6c 696e  layer: NovaOnlin
-000005d0: 6550 6c61 7965 7229 3a0d 0a20 2020 2020  ePlayer):..     
-000005e0: 2020 2020 7072 696e 7428 6622 7b70 6c61      print(f"{pla
-000005f0: 7965 722e 7573 6572 6e61 6d65 7d20 6a6f  yer.username} jo
-00000600: 696e 6564 207b 706c 6179 6572 2e73 6572  ined {player.ser
-00000610: 7665 725f 6e61 6d65 7d21 2229 0d0a 0d0a  ver_name}!")....
-00000620: 2020 2020 2020 636c 6965 6e74 2e73 7461        client.sta
-00000630: 7274 2829 0d0a 0d0a 0d0a 2a45 7861 6d70  rt()......*Examp
-00000640: 6c65 733a 2a0d 0a3d 3d3d 3d3d 3d3d 3d3d  les:*..=========
-00000650: 3d3d 3d3d 3d3d 0d0a 536f 6d65 2071 7569  ======..Some qui
-00000660: 636b 2073 686f 7274 2065 7861 6d70 6c65  ck short example
-00000670: 7320 746f 2067 6574 2073 7461 7274 6564  s to get started
-00000680: 2077 6974 6820 4e6f 7661 556e 6976 6572   with NovaUniver
-00000690: 7365 2e70 792e 20f0 9f8c 9f0d 0a41 6674  se.py. ......Aft
-000006a0: 6572 2079 6f75 2068 6176 6520 6120 7265  er you have a re
-000006b0: 6164 2068 6572 6520 706c 6561 7365 2064  ad here please d
-000006c0: 6f20 6368 6563 6b20 6f75 740d 0a0d 0a20  o check out.... 
-000006d0: 2020 5468 6973 2069 7320 7768 6174 2077    This is what w
-000006e0: 6520 6361 6c6c 2069 6e74 6572 6661 6365  e call interface
-000006f0: 732e 2049 6e74 6572 6661 6365 7320 6172  s. Interfaces ar
-00000700: 6520 7573 6564 2074 6f2e 2e2e 2077 656c  e used to... wel
-00000710: 6c2e 2e2e 202a 2a69 6e74 6572 6661 6365  l... **interface
-00000720: 212a 2a20 6861 2068 612c 2079 6573 2e2e  !** ha ha, yes..
-00000730: 2e20 7468 6579 2061 7265 2068 6f77 2079  . they are how y
-00000740: 6f75 2069 6e74 6572 6661 6365 2077 6974  ou interface wit
-00000750: 6820 7468 6520 4e6f 7661 2055 6e69 7665  h the Nova Unive
-00000760: 7273 6520 4150 492e 0d0a 0d0a 2020 2047  rse API.....   G
-00000770: 6574 7469 6e67 2074 6f75 726e 616d 656e  etting tournamen
-00000780: 7420 7265 7375 6c74 733a 3a0d 0a0d 0a20  t results::.... 
-00000790: 2020 2020 2066 726f 6d20 6e6f 7661 756e       from novaun
-000007a0: 6976 6572 7365 2069 6d70 6f72 7420 4e6f  iverse import No
-000007b0: 7661 4761 6d65 732c 204d 4346 0d0a 0d0a  vaGames, MCF....
-000007c0: 2020 2020 2020 2320 4765 7420 7468 6520        # Get the 
-000007d0: 6c61 7465 7374 204e 6f76 6120 4761 6d65  latest Nova Game
-000007e0: 7320 746f 7572 6e61 6d65 6e74 2e0d 0a20  s tournament... 
-000007f0: 2020 2020 206e 6f76 615f 6761 6d65 7320       nova_games 
-00000800: 3d20 4e6f 7661 4761 6d65 7328 292e 6765  = NovaGames().ge
-00000810: 745f 6c61 7465 7374 2829 0d0a 0d0a 2020  t_latest()....  
-00000820: 2020 2020 2320 5072 696e 7473 206f 7574      # Prints out
-00000830: 2068 6f77 206d 7563 6820 6561 6368 2070   how much each p
-00000840: 6c61 7965 7220 7363 6f72 6564 2069 6e20  layer scored in 
-00000850: 7468 6174 2074 6f75 726e 616d 656e 7420  that tournament 
-00000860: 616e 6420 616c 736f 2068 6f77 206d 616e  and also how man
-00000870: 7920 6b69 6c6c 7320 7468 6579 2061 6368  y kills they ach
-00000880: 6965 7665 642e 0d0a 2020 2020 2020 666f  ieved...      fo
-00000890: 7220 706c 6179 6572 2069 6e20 6e6f 7661  r player in nova
-000008a0: 5f67 616d 6573 2e70 6c61 7965 7273 3a0d  _games.players:.
-000008b0: 0a20 2020 2020 2020 2020 7072 696e 7428  .         print(
-000008c0: 6622 277b 706c 6179 6572 2e75 7365 726e  f"'{player.usern
-000008d0: 616d 657d 2720 676f 7420 7b70 6c61 7965  ame}' got {playe
-000008e0: 722e 6b69 6c6c 737d 206b 696c 6c28 7329  r.kills} kill(s)
-000008f0: 2061 6e64 2073 636f 7265 6420 7b70 6c61   and scored {pla
-00000900: 7965 722e 7363 6f72 657d 2070 6f69 6e74  yer.score} point
-00000910: 2873 2920 696e 2074 6865 204e 6f76 6120  (s) in the Nova 
-00000920: 4761 6d65 7320 686f 7374 6564 206f 6e20  Games hosted on 
-00000930: 7b6e 6f76 615f 6761 6d65 732e 6461 7465  {nova_games.date
-00000940: 2e64 6174 6528 297d 2e22 290d 0a0d 0a20  .date()}.").... 
-00000950: 2020 4e65 6174 2072 6967 6874 20f0 9f98    Neat right ...
-00000960: 812e 0d0a 0d0a 2020 202e 2e20 6e6f 7465  ......   .. note
-00000970: 3a3a 0d0a 0d0a 2020 2020 2020 4c65 6172  ::....      Lear
-00000980: 6e20 6d6f 7265 2061 626f 7574 2069 6e74  n more about int
-00000990: 6572 6661 6365 7320 3a72 6566 3a60 6f76  erfaces :ref:`ov
-000009a0: 6572 2068 6572 652e 203c 5468 6520 496e  er here. <The In
-000009b0: 7465 7266 6163 653e 600d 0a0d 0a2d 2d2d  terface>`....---
-000009c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 0d0a  ------------....
-000009d0: 2020 2053 6561 7263 6869 6e67 2066 6f72     Searching for
-000009e0: 2061 2073 7065 6369 6669 6320 6d63 6620   a specific mcf 
-000009f0: 746f 7572 6e61 6d65 6e74 3a3a 0d0a 2020  tournament::..  
-00000a00: 200d 0a20 2020 2020 2066 726f 6d20 6e6f   ..      from no
-00000a10: 7661 756e 6976 6572 7365 2069 6d70 6f72  vauniverse impor
-00000a20: 7420 4d43 462c 2053 6561 7263 680d 0a0d  t MCF, Search...
-00000a30: 0a20 2020 2020 206d 6366 203d 204d 4346  .      mcf = MCF
-00000a40: 2829 2e73 6561 7263 6828 5365 6172 6368  ().search(Search
-00000a50: 2869 643d 3137 2929 0d0a 0d0a 2020 2020  (id=17))....    
-00000a60: 2020 666f 7220 706c 6179 6572 2069 6e20    for player in 
-00000a70: 6d63 662e 706c 6179 6572 733a 0d0a 2020  mcf.players:..  
-00000a80: 2020 2020 2020 2070 7269 6e74 2866 2227         print(f"'
-00000a90: 7b70 6c61 7965 722e 7573 6572 6e61 6d65  {player.username
-00000aa0: 7d27 2067 6f74 207b 706c 6179 6572 2e6b  }' got {player.k
-00000ab0: 696c 6c73 7d20 6b69 6c6c 2873 2920 616e  ills} kill(s) an
-00000ac0: 6420 7363 6f72 6564 207b 706c 6179 6572  d scored {player
-00000ad0: 2e73 636f 7265 7d20 706f 696e 7428 7329  .score} point(s)
-00000ae0: 2069 6e20 7468 6520 4d43 4620 686f 7374   in the MCF host
-00000af0: 6564 206f 6e20 7b6d 6366 2e64 6174 652e  ed on {mcf.date.
-00000b00: 6461 7465 2829 7d2e 2229 0d0a 0d0a 2020  date()}.")....  
-00000b10: 202e 2e20 6e6f 7465 3a3a 0d0a 0d0a 2020   .. note::....  
-00000b20: 2020 2020 4d6f 7265 2061 7420 3a72 6566      More at :ref
-00000b30: 3a60 7365 6172 6368 2069 6e74 6572 6661  :`search interfa
-00000b40: 6365 732e 203c 5468 6520 5365 6172 6368  ces. <The Search
-00000b50: 2049 6e74 6572 6661 6365 3e60 0d0a 0d0a   Interface>`....
-00000b60: 0d0a 436f 6e66 6967 7572 6174 696f 6e20  ..Configuration 
-00000b70: 5265 6665 7265 6e63 650d 0a2d 2d2d 2d2d  Reference..-----
-00000b80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000b90: 2d2d 2d2d 0d0a 2e2e 2061 7574 6f6d 6f64  ----.... automod
-00000ba0: 756c 653a 3a20 6e6f 7661 756e 6976 6572  ule:: novauniver
-00000bb0: 7365 2e63 6f6e 6669 6775 7261 7469 6f6e  se.configuration
-00000bc0: 0d0a 2020 203a 6d65 6d62 6572 733a 0d0a  ..   :members:..
-00000bd0: 2020 203a 756e 646f 632d 6d65 6d62 6572     :undoc-member
-00000be0: 733a 0d0a 2020 203a 7368 6f77 2d69 6e68  s:..   :show-inh
-00000bf0: 6572 6974 616e 6365 3a0d 0a0d 0a45 7272  eritance:....Err
-00000c00: 6f72 7320 5265 6665 7265 6e63 650d 0a2d  ors Reference..-
-00000c10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000c20: 0d0a 2e2e 2061 7574 6f6d 6f64 756c 653a  .... automodule:
-00000c30: 3a20 6e6f 7661 756e 6976 6572 7365 2e65  : novauniverse.e
-00000c40: 7272 6f72 730d 0a20 2020 3a6d 656d 6265  rrors..   :membe
-00000c50: 7273 3a0d 0a20 2020 3a75 6e64 6f63 2d6d  rs:..   :undoc-m
-00000c60: 656d 6265 7273 3a0d 0a20 2020 3a73 686f  embers:..   :sho
-00000c70: 772d 696e 6865 7269 7461 6e63 653a 0d0a  w-inheritance:..
-00000c80: 0d0a 0d0a 496e 6469 6365 7320 616e 6420  ....Indices and 
-00000c90: 7461 626c 6573 0d0a 3d3d 3d3d 3d3d 3d3d  tables..========
-00000ca0: 3d3d 3d3d 3d3d 3d3d 3d3d 0d0a 0d0a 2a20  ==========....* 
-00000cb0: 3a72 6566 3a60 6765 6e69 6e64 6578 600d  :ref:`genindex`.
-00000cc0: 0a2a 203a 7265 663a 606d 6f64 696e 6465  .* :ref:`modinde
-00000cd0: 7860 0d0a 2a20 3a72 6566 3a60 7365 6172  x`..* :ref:`sear
-00000ce0: 6368 600d 0a                             ch`..
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310d 0a4e 616d 653a 206e 6f76  : 2.1..Name: nov
+00000020: 6175 6e69 7665 7273 650d 0a56 6572 7369  auniverse..Versi
+00000030: 6f6e 3a20 322e 312e 310d 0a53 756d 6d61  on: 2.1.1..Summa
+00000040: 7279 3a20 4120 6d6f 6465 726e 2026 206d  ry: A modern & m
+00000050: 6169 6e74 6169 6e65 6420 7772 6170 7065  aintained wrappe
+00000060: 7220 666f 7220 7468 6520 4e6f 7661 2055  r for the Nova U
+00000070: 6e69 7665 7273 6520 4150 4920 7772 6974  niverse API writ
+00000080: 7465 6e20 696e 20f0 9f90 8d20 5079 7468  ten in .... Pyth
+00000090: 6f6e 2e0d 0a41 7574 686f 722d 656d 6169  on...Author-emai
+000000a0: 6c3a 2047 6f6c 6479 203c 676f 6c64 7940  l: Goldy <goldy@
+000000b0: 6465 7667 6f6c 6479 2e6d 653e 0d0a 5072  devgoldy.me>..Pr
+000000c0: 6f6a 6563 742d 5552 4c3a 2047 6974 4875  oject-URL: GitHu
+000000d0: 622c 2068 7474 7073 3a2f 2f67 6974 6875  b, https://githu
+000000e0: 622e 636f 6d2f 4e6f 7661 556e 6976 6572  b.com/NovaUniver
+000000f0: 7365 2f4e 6f76 6155 6e69 7665 7273 652e  se/NovaUniverse.
+00000100: 7079 0d0a 5072 6f6a 6563 742d 5552 4c3a  py..Project-URL:
+00000110: 2042 7567 5472 6163 6b65 722c 2068 7474   BugTracker, htt
+00000120: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000130: 4e6f 7661 556e 6976 6572 7365 2f4e 6f76  NovaUniverse/Nov
+00000140: 6155 6e69 7665 7273 652e 7079 2f69 7373  aUniverse.py/iss
+00000150: 7565 730d 0a50 726f 6a65 6374 2d55 524c  ues..Project-URL
+00000160: 3a20 4368 616e 6765 4c6f 672c 2068 7474  : ChangeLog, htt
+00000170: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000180: 4e6f 7661 556e 6976 6572 7365 2f4e 6f76  NovaUniverse/Nov
+00000190: 6155 6e69 7665 7273 652e 7079 2f62 6c6f  aUniverse.py/blo
+000001a0: 622f 6d61 696e 2f43 4841 4e47 454c 4f47  b/main/CHANGELOG
+000001b0: 2e72 7374 0d0a 4b65 7977 6f72 6473 3a20  .rst..Keywords: 
+000001c0: 6e6f 7661 756e 6976 6572 7365 2c6d 696e  novauniverse,min
+000001d0: 6563 7261 6674 206e 6f76 6175 6e69 7665  ecraft novaunive
+000001e0: 7273 652c 6e6f 7661 2075 6e69 7665 7273  rse,nova univers
+000001f0: 652c 6d63 206e 6f76 6175 6e69 7665 7273  e,mc novaunivers
+00000200: 650d 0a43 6c61 7373 6966 6965 723a 204f  e..Classifier: O
+00000210: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+00000220: 3a3a 204d 6963 726f 736f 6674 203a 3a20  :: Microsoft :: 
+00000230: 5769 6e64 6f77 7320 3a3a 2057 696e 646f  Windows :: Windo
+00000240: 7773 2031 310d 0a43 6c61 7373 6966 6965  ws 11..Classifie
+00000250: 723a 204f 7065 7261 7469 6e67 2053 7973  r: Operating Sys
+00000260: 7465 6d20 3a3a 204d 6963 726f 736f 6674  tem :: Microsoft
+00000270: 203a 3a20 5769 6e64 6f77 7320 3a3a 2057   :: Windows :: W
+00000280: 696e 646f 7773 2031 300d 0a43 6c61 7373  indows 10..Class
+00000290: 6966 6965 723a 204f 7065 7261 7469 6e67  ifier: Operating
+000002a0: 2053 7973 7465 6d20 3a3a 2050 4f53 4958   System :: POSIX
+000002b0: 203a 3a20 4c69 6e75 780d 0a43 6c61 7373   :: Linux..Class
+000002c0: 6966 6965 723a 204c 6963 656e 7365 203a  ifier: License :
+000002d0: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
+000002e0: 3a20 4d49 5420 4c69 6365 6e73 650d 0a43  : MIT License..C
+000002f0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+00000300: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000310: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
+00000320: 0d0a 436c 6173 7369 6669 6572 3a20 5072  ..Classifier: Pr
+00000330: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000340: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000350: 332e 390d 0a43 6c61 7373 6966 6965 723a  3.9..Classifier:
+00000360: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000370: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000380: 3a3a 2033 2e31 300d 0a43 6c61 7373 6966  :: 3.10..Classif
+00000390: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+000003a0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000003b0: 686f 6e20 3a3a 2033 2e31 310d 0a52 6571  hon :: 3.11..Req
+000003c0: 7569 7265 732d 5079 7468 6f6e 3a20 3e3d  uires-Python: >=
+000003d0: 332e 370d 0a44 6573 6372 6970 7469 6f6e  3.7..Description
+000003e0: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
+000003f0: 6578 742f 6d61 726b 646f 776e 0d0a 5072  ext/markdown..Pr
+00000400: 6f76 6964 6573 2d45 7874 7261 3a20 6465  ovides-Extra: de
+00000410: 760d 0a0d 0a3c 6469 7620 616c 6967 6e3d  v....<div align=
+00000420: 2263 656e 7465 7222 3e0d 0a0d 0a20 2023  "center">....  #
+00000430: 20f0 9f90 8d5b 6060 6e6f 7661 756e 6976   ....[``novauniv
+00000440: 6572 7365 2e70 7960 605d 2868 7474 7073  erse.py``](https
+00000450: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+00000460: 6563 742f 6e6f 7661 756e 6976 6572 7365  ect/novauniverse
+00000470: 2f29 0d0a 2020 0d0a 2020 3c73 7562 3e41  /)..  ..  <sub>A
+00000480: 206d 6f64 6572 6e20 2620 6d61 696e 7461   modern & mainta
+00000490: 696e 6564 2077 7261 7070 6572 2066 6f72  ined wrapper for
+000004a0: 2074 6865 205b 4e6f 7661 2055 6e69 7665   the [Nova Unive
+000004b0: 7273 6520 4150 495d 2868 7474 7073 3a2f  rse API](https:/
+000004c0: 2f6e 6f76 6175 6e69 7665 7273 652e 6e65  /novauniverse.ne
+000004d0: 742f 6170 692f 2920 7772 6974 7465 6e20  t/api/) written 
+000004e0: 696e 2050 7974 686f 6e2e 3c2f 7375 623e  in Python.</sub>
+000004f0: 0d0a 2020 0d0a 2020 5b21 5b44 6973 636f  ..  ..  [![Disco
+00000500: 7264 2053 6869 656c 645d 2868 7474 7073  rd Shield](https
+00000510: 3a2f 2f64 6973 636f 7264 6170 702e 636f  ://discordapp.co
+00000520: 6d2f 6170 692f 6775 696c 6473 2f36 3932  m/api/guilds/692
+00000530: 3736 3439 3735 3930 3237 3532 3837 312f  764975902752871/
+00000540: 7769 6467 6574 2e70 6e67 3f73 7479 6c65  widget.png?style
+00000550: 3d73 6869 656c 6429 5d28 6874 7470 733a  =shield)](https:
+00000560: 2f2f 6469 7363 6f72 642e 6767 2f34 675a  //discord.gg/4gZ
+00000570: 5356 4a37 290d 0a20 205b 215b 5079 5049  SVJ7)..  [![PyPI
+00000580: 2076 6572 7369 6f6e 5d28 6874 7470 733a   version](https:
+00000590: 2f2f 6261 6467 652e 6675 7279 2e69 6f2f  //badge.fury.io/
+000005a0: 7079 2f6e 6f76 6175 6e69 7665 7273 652e  py/novauniverse.
+000005b0: 7376 6729 5d28 6874 7470 733a 2f2f 7079  svg)](https://py
+000005c0: 7069 2e6f 7267 2f70 726f 6a65 6374 2f6e  pi.org/project/n
+000005d0: 6f76 6175 6e69 7665 7273 652f 290d 0a20  ovauniverse/).. 
+000005e0: 205b 215b 5079 7468 6f6e 2042 6164 6765   [![Python Badge
+000005f0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000600: 6965 6c64 732e 696f 2f70 7970 692f 7079  ields.io/pypi/py
+00000610: 7665 7273 696f 6e73 2f6e 6f76 6175 6e69  versions/novauni
+00000620: 7665 7273 653f 7374 796c 653d 666c 6174  verse?style=flat
+00000630: 295d 2868 7474 7073 3a2f 2f70 7970 692e  )](https://pypi.
+00000640: 6f72 672f 7072 6f6a 6563 742f 6e6f 7661  org/project/nova
+00000650: 756e 6976 6572 7365 2f20 2253 7570 706f  universe/ "Suppo
+00000660: 7274 6564 2070 7974 686f 6e20 7665 7273  rted python vers
+00000670: 696f 6e73 2e22 290d 0a20 205b 215b 446f  ions.")..  [![Do
+00000680: 6373 2042 6164 6765 5d28 6874 7470 733a  cs Badge](https:
+00000690: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000006a0: 2f67 6974 6875 622f 6163 7469 6f6e 732f  /github/actions/
+000006b0: 776f 726b 666c 6f77 2f73 7461 7475 732f  workflow/status/
+000006c0: 4e6f 7661 556e 6976 6572 7365 2f4e 6f76  NovaUniverse/Nov
+000006d0: 6155 6e69 7665 7273 652e 7079 2f64 6f63  aUniverse.py/doc
+000006e0: 756d 656e 7461 7469 6f6e 2e79 616d 6c3f  umentation.yaml?
+000006f0: 6c61 6265 6c3d 646f 6373 295d 2868 7474  label=docs)](htt
+00000700: 7073 3a2f 2f6e 7570 792e 6465 7667 6f6c  ps://nupy.devgol
+00000710: 6479 2e6d 652f 290d 0a20 200d 0a3c 2f64  dy.me/)..  ..</d
+00000720: 6976 3e0d 0a0d 0a3e 2023 2323 2320 e284  iv>....> #### ..
+00000730: b920 4e6f 7469 6365 3a20 322e 3020 6973  . Notice: 2.0 is
+00000740: 2063 7572 7265 6e74 6c79 2069 6e20 6465   currently in de
+00000750: 7665 6c6f 706d 656e 7420 736f 206e 6f74  velopment so not
+00000760: 2061 6c6c 2061 7069 2065 6e64 706f 696e   all api endpoin
+00000770: 7473 2061 7265 2069 6d70 6c65 6d65 6e74  ts are implement
+00000780: 6564 2e0d 0a0d 0a3c 7020 616c 6967 6e3d  ed.....<p align=
+00000790: 2272 6967 6874 223e 0d0a 203c 696d 6720  "right">.. <img 
+000007a0: 616c 6967 6e3d 226c 6566 7422 2073 7263  align="left" src
+000007b0: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
+000007c0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+000007d0: 636f 6d2f 4e6f 7661 556e 6976 6572 7365  com/NovaUniverse
+000007e0: 2f4e 6f76 6155 6e69 7665 7273 652e 7079  /NovaUniverse.py
+000007f0: 2f6d 6169 6e2f 646f 6373 2f5f 7374 6174  /main/docs/_stat
+00000800: 6963 2f6c 6f67 6f2e 706e 6722 2077 6964  ic/logo.png" wid
+00000810: 7468 3d22 3138 3022 202f 3e0d 0a20 0d0a  th="180" />.. ..
+00000820: 203c 6832 3e57 6861 7420 6973 204e 6f76   <h2>What is Nov
+00000830: 6120 556e 6976 6572 7365 2e70 793f 3c2f  a Universe.py?</
+00000840: 6832 3e0d 0a20 4e6f 7661 556e 6976 6572  h2>.. NovaUniver
+00000850: 7365 2e70 7920 6973 2061 6e20 4150 4920  se.py is an API 
+00000860: 7772 6170 7065 7220 666f 7220 e280 9c3c  wrapper for ...<
+00000870: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000880: 6e6f 7661 756e 6976 6572 7365 2e6e 6574  novauniverse.net
+00000890: 2f22 3e4e 6f76 6120 556e 6976 6572 7365  /">Nova Universe
+000008a0: 3c2f 613e e280 9d20 2861 206d 696e 6563  </a>... (a minec
+000008b0: 7261 6674 2065 7665 6e74 2068 6f73 7469  raft event hosti
+000008c0: 6e67 2067 726f 7570 2920 7468 6174 2061  ng group) that a
+000008d0: 6c6c 6f77 7320 796f 7520 746f 2069 6e74  llows you to int
+000008e0: 6572 6661 6365 2077 6974 6820 7468 6520  erface with the 
+000008f0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000900: 2f6e 6f76 6175 6e69 7665 7273 652e 6e65  /novauniverse.ne
+00000910: 742f 6170 6922 3e4e 6f76 6120 556e 6976  t/api">Nova Univ
+00000920: 6572 7365 2041 5049 3c2f 613e 2069 6e20  erse API</a> in 
+00000930: 6120 6661 7374 206f 626a 6563 7420 6f72  a fast object or
+00000940: 6965 6e74 6564 2077 6179 206e 6174 6976  iented way nativ
+00000950: 656c 7920 7769 7468 696e 2050 7974 686f  ely within Pytho
+00000960: 6e2e 204f 6e65 206f 6620 7468 6520 626f  n. One of the bo
+00000970: 6e75 7365 7320 6973 2074 6861 7420 6974  nuses is that it
+00000980: 2077 6173 2064 6576 656c 6f70 6564 2062   was developed b
+00000990: 7920 3c61 2068 7265 663d 2268 7474 7073  y <a href="https
+000009a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 5448  ://github.com/TH
+000009b0: 4547 4f4c 4445 4e50 524f 223e 4d45 3c2f  EGOLDENPRO">ME</
+000009c0: 613e 2c20 616e 2061 646d 696e 2061 7420  a>, an admin at 
+000009d0: 4e6f 7661 556e 6976 6572 7365 2e0d 0a3c  NovaUniverse...<
+000009e0: 2f70 3e0d 0a0d 0a3c 6272 3e0d 0a0d 0a23  /p>....<br>....#
+000009f0: 2320 2a49 6e73 7461 6c6c 2f53 6574 2055  # *Install/Set U
+00000a00: 702a 0d0a 312e 202a 2a49 6e73 7461 6c6c  p*..1. **Install
+00000a10: 2070 6163 6b61 6765 2066 726f 6d20 7079   package from py
+00000a20: 7069 2e2a 2a0d 0a60 6060 7368 0d0a 2357  pi.**..```sh..#W
+00000a30: 696e 646f 7773 2f4c 696e 7578 0d0a 0d0a  indows/Linux....
+00000a40: 7069 7020 696e 7374 616c 6c20 6e6f 7661  pip install nova
+00000a50: 756e 6976 6572 7365 0d0a 6060 600d 0a32  universe..```..2
+00000a60: 2e20 2a2a 5468 6174 2773 2049 7421 2a2a  . **That's It!**
+00000a70: 202d 202a 4272 6965 6620 4578 616d 706c   - *Brief Exampl
+00000a80: 6520 4265 6c6f 772a 0d0a 6060 6070 7974  e Below*..```pyt
+00000a90: 686f 6e0d 0a66 726f 6d20 6e6f 7661 756e  hon..from novaun
+00000aa0: 6976 6572 7365 2069 6d70 6f72 7420 4576  iverse import Ev
+00000ab0: 656e 7443 6c69 656e 742c 2045 7665 6e74  entClient, Event
+00000ac0: 732c 204e 6f76 614f 6e6c 696e 6550 6c61  s, NovaOnlinePla
+00000ad0: 7965 7220 0d0a 0d0a 636c 6965 6e74 203d  yer ....client =
+00000ae0: 2045 7665 6e74 436c 6965 6e74 2829 0d0a   EventClient()..
+00000af0: 0d0a 4063 6c69 656e 742e 6f6e 5f65 7665  ..@client.on_eve
+00000b00: 6e74 2845 7665 6e74 732e 434c 4945 4e54  nt(Events.CLIENT
+00000b10: 5f52 4541 4459 290d 0a64 6566 2063 6c69  _READY)..def cli
+00000b20: 656e 745f 6973 5f72 6561 6479 2829 3a0d  ent_is_ready():.
+00000b30: 0a20 2020 2070 7269 6e74 2822 436c 6965  .    print("Clie
+00000b40: 6e74 2069 7320 7265 6164 7921 2229 0d0a  nt is ready!")..
+00000b50: 0d0a 4063 6c69 656e 742e 6f6e 5f65 7665  ..@client.on_eve
+00000b60: 6e74 2845 7665 6e74 732e 504c 4159 4552  nt(Events.PLAYER
+00000b70: 5f4a 4f49 4e29 0d0a 6465 6620 6f6e 5f70  _JOIN)..def on_p
+00000b80: 6c61 7965 725f 6a6f 696e 2870 6c61 7965  layer_join(playe
+00000b90: 723a 4e6f 7661 4f6e 6c69 6e65 506c 6179  r:NovaOnlinePlay
+00000ba0: 6572 293a 0d0a 2020 2020 7072 696e 7428  er):..    print(
+00000bb0: 6622 7b70 6c61 7965 722e 7573 6572 6e61  f"{player.userna
+00000bc0: 6d65 7d20 6a6f 696e 6564 207b 706c 6179  me} joined {play
+00000bd0: 6572 2e73 6572 7665 725f 6e61 6d65 7d21  er.server_name}!
+00000be0: 2229 0d0a 0d0a 636c 6965 6e74 2e73 7461  ")....client.sta
+00000bf0: 7274 2829 0d0a 6060 600d 0a0d 0a3c 6272  rt()..```....<br
+00000c00: 3e0d 0a0d 0a3e 2023 2323 204d 6f72 6520  >....> ### More 
+00000c10: 4578 616d 706c 6573 2061 6e64 2049 6e66  Examples and Inf
+00000c20: 6f20 6174 2068 7474 7073 3a2f 2f6e 7570  o at https://nup
+00000c30: 792e 6465 7667 6f6c 6479 2e6d 652f 0d0a  y.devgoldy.me/..
```

### Comparing `novauniverse-2.1/novauniverse/api/__init__.py` & `novauniverse-2.1.1/novauniverse/api/__init__.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.1/novauniverse/api/cdn.py` & `novauniverse-2.1.1/novauniverse/api/cdn.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.1/novauniverse/api/endpoints.py` & `novauniverse-2.1.1/novauniverse/api/endpoints.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.1/novauniverse/api/errors.py` & `novauniverse-2.1.1/novauniverse/api/errors.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.1/novauniverse/configuration.py` & `novauniverse-2.1.1/novauniverse/configuration.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.1/novauniverse/event_client.py` & `novauniverse-2.1.1/novauniverse/event_client.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.1/novauniverse/events/__init__.py` & `novauniverse-2.1.1/novauniverse/events/__init__.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.1/novauniverse/events/player_join.py` & `novauniverse-2.1.1/novauniverse/events/player_join.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.1/novauniverse/events/player_leave.py` & `novauniverse-2.1.1/novauniverse/events/player_leave.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.1/novauniverse/interfaces/__init__.py` & `novauniverse-2.1.1/novauniverse/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.1/novauniverse/interfaces/stats/discord/__init__.py` & `novauniverse-2.1.1/novauniverse/interfaces/stats/discord/__init__.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.1/novauniverse/interfaces/stats/discord/discord_stats.py` & `novauniverse-2.1.1/novauniverse/interfaces/stats/discord/discord_stats.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.1/novauniverse/interfaces/stats/server/__init__.py` & `novauniverse-2.1.1/novauniverse/interfaces/stats/server/__init__.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.1/novauniverse/interfaces/stats/server/global_.py` & `novauniverse-2.1.1/novauniverse/interfaces/stats/server/global_.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.1/novauniverse/interfaces/stats/server/nova_online_player.py` & `novauniverse-2.1.1/novauniverse/interfaces/stats/server/nova_online_player.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.1/novauniverse/interfaces/stats/server/nova_server.py` & `novauniverse-2.1.1/novauniverse/interfaces/stats/server/nova_server.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.1/novauniverse/interfaces/stats/server/player_preview.py` & `novauniverse-2.1.1/novauniverse/interfaces/stats/server/player_preview.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.1/novauniverse/interfaces/stats/server/server_info.py` & `novauniverse-2.1.1/novauniverse/interfaces/stats/server/server_info.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.1/novauniverse/interfaces/tournaments/__init__.py` & `novauniverse-2.1.1/novauniverse/interfaces/tournaments/__init__.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.1/novauniverse/interfaces/tournaments/mcf/__init__.py` & `novauniverse-2.1.1/novauniverse/interfaces/tournaments/mcf/__init__.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.1/novauniverse/interfaces/tournaments/nova_games/__init__.py` & `novauniverse-2.1.1/novauniverse/interfaces/tournaments/nova_games/__init__.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.1/novauniverse/objects/nova_dataclass.py` & `novauniverse-2.1.1/novauniverse/objects/nova_dataclass.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.1/novauniverse/objects/nova_player.py` & `novauniverse-2.1.1/novauniverse/objects/nova_player.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.1/novauniverse/objects/timestamp.py` & `novauniverse-2.1.1/novauniverse/objects/timestamp.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.1/novauniverse/objects/tournaments/__init__.py` & `novauniverse-2.1.1/novauniverse/objects/tournaments/__init__.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.1/novauniverse/objects/tournaments/tournament_player.py` & `novauniverse-2.1.1/novauniverse/objects/tournaments/tournament_player.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.1/novauniverse/objects/tournaments/tournament_team.py` & `novauniverse-2.1.1/novauniverse/objects/tournaments/tournament_team.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.1/novauniverse/utils/search.py` & `novauniverse-2.1.1/novauniverse/utils/search.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.1/pyproject.toml` & `novauniverse-2.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -44,19 +44,24 @@
 BugTracker = "https://github.com/NovaUniverse/NovaUniverse.py/issues"
 ChangeLog = "https://github.com/NovaUniverse/NovaUniverse.py/blob/main/CHANGELOG.rst"
 
 [tool.setuptools.dynamic]
 version = { attr = "novauniverse.info.VERSION" }
 
 [build-system]
-requires = ["setuptools", "setuptools-scm"]
+requires = ["setuptools>=61.2", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
-packages = ["novauniverse"]
+include-package-data = false
+
+[tool.setuptools.packages.find]
+include = ["novauniverse*"]
+exclude = ["docs*", "tests*", ".github*"]
+
 
 
 # Ruff
 # ---------------
 
 [tool.ruff]
 # Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
```

