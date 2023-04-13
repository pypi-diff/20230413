# Comparing `tmp/aa_rss_to_discord-1.4.1.tar.gz` & `tmp/aa_rss_to_discord-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_rss_to_discord-1.4.1.tar", last modified: Sun Jan 15 12:18:19 2023, max compression
+gzip compressed data, was "aa_rss_to_discord-1.4.2.tar", last modified: Thu Apr 13 20:35:22 2023, max compression
```

## Comparing `aa_rss_to_discord-1.4.1.tar` & `aa_rss_to_discord-1.4.2.tar`

### file list

```diff
@@ -1,32 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 12:18:19.020611 aa_rss_to_discord-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-01-15 12:18:03.000000 aa_rss_to_discord-1.4.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-15 12:18:03.000000 aa_rss_to_discord-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-01-15 12:18:03.000000 aa_rss_to_discord-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-01-15 12:18:19.020611 aa_rss_to_discord-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-01-15 12:18:03.000000 aa_rss_to_discord-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 12:18:19.020611 aa_rss_to_discord-1.4.1/aa_rss_to_discord/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-01-15 12:18:03.000000 aa_rss_to_discord-1.4.1/aa_rss_to_discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-01-15 12:18:03.000000 aa_rss_to_discord-1.4.1/aa_rss_to_discord/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-01-15 12:18:03.000000 aa_rss_to_discord-1.4.1/aa_rss_to_discord/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-01-15 12:18:03.000000 aa_rss_to_discord-1.4.1/aa_rss_to_discord/auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-01-15 12:18:03.000000 aa_rss_to_discord-1.4.1/aa_rss_to_discord/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 12:18:19.016611 aa_rss_to_discord-1.4.1/aa_rss_to_discord/discordbot/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 12:18:19.020611 aa_rss_to_discord-1.4.1/aa_rss_to_discord/discordbot/cogs/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-01-15 12:18:03.000000 aa_rss_to_discord-1.4.1/aa_rss_to_discord/discordbot/cogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-01-15 12:18:03.000000 aa_rss_to_discord-1.4.1/aa_rss_to_discord/discordbot/cogs/rss.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-01-15 12:18:03.000000 aa_rss_to_discord-1.4.1/aa_rss_to_discord/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 12:18:19.020611 aa_rss_to_discord-1.4.1/aa_rss_to_discord/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-01-15 12:18:03.000000 aa_rss_to_discord-1.4.1/aa_rss_to_discord/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-01-15 12:18:03.000000 aa_rss_to_discord-1.4.1/aa_rss_to_discord/migrations/0002_enable_disable_rss_feeds.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 12:18:03.000000 aa_rss_to_discord-1.4.1/aa_rss_to_discord/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-01-15 12:18:03.000000 aa_rss_to_discord-1.4.1/aa_rss_to_discord/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-01-15 12:18:03.000000 aa_rss_to_discord-1.4.1/aa_rss_to_discord/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 12:18:19.020611 aa_rss_to_discord-1.4.1/aa_rss_to_discord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-01-15 12:18:19.000000 aa_rss_to_discord-1.4.1/aa_rss_to_discord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-01-15 12:18:19.000000 aa_rss_to_discord-1.4.1/aa_rss_to_discord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-15 12:18:19.000000 aa_rss_to_discord-1.4.1/aa_rss_to_discord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-15 12:18:18.000000 aa_rss_to_discord-1.4.1/aa_rss_to_discord.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-01-15 12:18:19.000000 aa_rss_to_discord-1.4.1/aa_rss_to_discord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-15 12:18:19.000000 aa_rss_to_discord-1.4.1/aa_rss_to_discord.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-01-15 12:18:03.000000 aa_rss_to_discord-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-01-15 12:18:19.020611 aa_rss_to_discord-1.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.057346 aa_rss_to_discord-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-04-13 20:35:22.057346 aa_rss_to_discord-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.053346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/auth_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.053346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/discordbot/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.057346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/discordbot/cogs/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/discordbot/cogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/discordbot/cogs/rss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.053346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.053346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.057346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.053346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.057346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.053346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.057346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/fr_FR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.053346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/it_IT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.057346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/it_IT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/it_IT/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.053346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.057346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.053346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/ko_KR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.057346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/ko_KR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.053346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.057346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.053346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.057346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.057346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/migrations/0002_enable_disable_rss_feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.057346 aa_rss_to_discord-1.4.2/aa_rss_to_discord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-04-13 20:35:22.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-13 20:35:22.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:35:22.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:35:21.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 20:35:22.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 20:35:22.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-13 20:35:22.057346 aa_rss_to_discord-1.4.2/setup.cfg
```

### Comparing `aa_rss_to_discord-1.4.1/CHANGELOG.md` & `aa_rss_to_discord-1.4.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 The format is based on [Keep a Changelog](http://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](http://semver.org/)
 
 
 ## [In Development] - Unreleased
 
 
+## [1.4.2] - 2023-04-13
+
+### Added
+
+- German translation
+
+
 ## [1.4.1] - 2023-01-15
 
 ### Added
 
 - More Debug logging for the task to figure out what's going on for issue #23
 
 ### Changed
```

### Comparing `aa_rss_to_discord-1.4.1/LICENSE` & `aa_rss_to_discord-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-1.4.1/PKG-INFO` & `aa_rss_to_discord-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa_rss_to_discord
-Version: 1.4.1
+Version: 1.4.2
 Summary: Alliance Auth module to post news from RSS feeds to your Discord
 Home-page: https://github.com/ppfeufer/aa-rss-to-discord
 Author: Peter Pfeufer
 Author-email: develop@ppfeufer.de
 Maintainer: Peter Pfeufer
 Maintainer-email: develop@ppfeufer.de
 License: GPL-3.0
```

### Comparing `aa_rss_to_discord-1.4.1/README.md` & `aa_rss_to_discord-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-1.4.1/aa_rss_to_discord/discordbot/cogs/rss.py` & `aa_rss_to_discord-1.4.2/aa_rss_to_discord/discordbot/cogs/rss.py`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-1.4.1/aa_rss_to_discord/migrations/0001_initial.py` & `aa_rss_to_discord-1.4.2/aa_rss_to_discord/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-1.4.1/aa_rss_to_discord/models.py` & `aa_rss_to_discord-1.4.2/aa_rss_to_discord/models.py`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-1.4.1/aa_rss_to_discord/tasks.py` & `aa_rss_to_discord-1.4.2/aa_rss_to_discord/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-1.4.1/aa_rss_to_discord.egg-info/PKG-INFO` & `aa_rss_to_discord-1.4.2/aa_rss_to_discord.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-rss-to-discord
-Version: 1.4.1
+Version: 1.4.2
 Summary: Alliance Auth module to post news from RSS feeds to your Discord
 Home-page: https://github.com/ppfeufer/aa-rss-to-discord
 Author: Peter Pfeufer
 Author-email: develop@ppfeufer.de
 Maintainer: Peter Pfeufer
 Maintainer-email: develop@ppfeufer.de
 License: GPL-3.0
```

### Comparing `aa_rss_to_discord-1.4.1/setup.cfg` & `aa_rss_to_discord-1.4.2/setup.cfg`

 * *Files identical despite different names*

