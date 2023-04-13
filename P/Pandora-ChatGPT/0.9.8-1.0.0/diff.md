# Comparing `tmp/Pandora-ChatGPT-0.9.8.tar.gz` & `tmp/Pandora-ChatGPT-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pandora/pandora/dist/.tmp-bs0v6jo9/Pandora-ChatGPT-0.9.8.tar", last modified: Thu Apr  6 11:21:05 2023, max compression
+gzip compressed data, was "/home/runner/work/pandora/pandora/dist/.tmp-0pknjc0h/Pandora-ChatGPT-1.0.0.tar", last modified: Thu Apr 13 10:26:17 2023, max compression
```

## Comparing `Pandora-ChatGPT-0.9.8.tar` & `Pandora-ChatGPT-1.0.0.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:21:05.000000 Pandora-ChatGPT-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10207 2023-04-06 11:21:05.000000 Pandora-ChatGPT-0.9.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:21:05.000000 Pandora-ChatGPT-0.9.8/Pandora_ChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10207 2023-04-06 11:21:05.000000 Pandora-ChatGPT-0.9.8/Pandora_ChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-06 11:21:05.000000 Pandora-ChatGPT-0.9.8/Pandora_ChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 11:21:05.000000 Pandora-ChatGPT-0.9.8/Pandora_ChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-06 11:21:05.000000 Pandora-ChatGPT-0.9.8/Pandora_ChatGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-06 11:21:05.000000 Pandora-ChatGPT-0.9.8/Pandora_ChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-06 11:21:05.000000 Pandora-ChatGPT-0.9.8/Pandora_ChatGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/requirements_api.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 11:21:05.000000 Pandora-ChatGPT-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:21:05.000000 Pandora-ChatGPT-0.9.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:21:05.000000 Pandora-ChatGPT-0.9.8/src/pandora/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:21:05.000000 Pandora-ChatGPT-0.9.8/src/pandora/bots/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15216 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/bots/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/bots/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/cloud_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:21:05.000000 Pandora-ChatGPT-0.9.8/src/pandora/exts/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/exts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/exts/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/exts/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/exts/sentry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/exts/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:21:05.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:21:05.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:21:05.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:21:05.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:21:05.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/
--rw-r--r--   0 runner    (1001) docker     (123)   905448 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js
--rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js
--rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js
--rw-r--r--   0 runner    (1001) docker     (123)   264961 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js
--rw-r--r--   0 runner    (1001) docker     (123)    13147 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js
--rw-r--r--   0 runner    (1001) docker     (123)    24138 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js
--rw-r--r--   0 runner    (1001) docker     (123)    20480 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/68a27ff6-1185184b61bc22d0.js
--rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js
--rw-r--r--   0 runner    (1001) docker     (123)   141370 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js
--rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:21:05.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/pages/
--rw-r--r--   0 runner    (1001) docker     (123)   305755 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/pages/_error-786d27d84962122a.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:21:05.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/pages/chat/
--rw-r--r--   0 runner    (1001) docker     (123)   149531 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js
--rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:21:05.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   108647 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/css/ac221fb2caad35a6.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:21:05.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_ssgManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/favicon-32x32.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:21:05.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    29912 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_Main-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    19412 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    19676 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_Main-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    30772 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_Main-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18668 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18748 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_Math-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    14408 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_Script-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_Size1-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_Size2-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_Size3-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_Size4-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)   324208 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/Signifier-Regular.otf
--rw-r--r--   0 runner    (1001) docker     (123)   210840 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/Sohne-Buch.otf
--rw-r--r--   0 runner    (1001) docker     (123)   230012 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/Sohne-Halbfett.otf
--rw-r--r--   0 runner    (1001) docker     (123)    30824 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/SohneMono-Buch.otf
--rw-r--r--   0 runner    (1001) docker     (123)    31116 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/SohneMono-Halbfett.otf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:21:05.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:21:05.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/images/2022/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:21:05.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/images/2022/11/
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/static/images/2022/11/ChatGPT.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:21:05.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/flask/templates/chat.html
--rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:21:05.000000 Pandora-ChatGPT-0.9.8/src/pandora/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/migrations/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/migrations/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/migrations/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:21:05.000000 Pandora-ChatGPT-0.9.8/src/pandora/migrations/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/migrations/scripts/20230308_01_7ctOr.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:21:05.000000 Pandora-ChatGPT-0.9.8/src/pandora/openai/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10781 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/openai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/openai/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/openai/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/openai/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:21:05.000000 Pandora-ChatGPT-0.9.8/src/pandora/turbo/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/turbo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/turbo/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-04-06 11:20:50.000000 Pandora-ChatGPT-0.9.8/src/pandora/turbo/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:26:17.000000 Pandora-ChatGPT-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-04-13 10:26:17.000000 Pandora-ChatGPT-1.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:26:17.000000 Pandora-ChatGPT-1.0.0/Pandora_ChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-04-13 10:26:17.000000 Pandora-ChatGPT-1.0.0/Pandora_ChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-13 10:26:17.000000 Pandora-ChatGPT-1.0.0/Pandora_ChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 10:26:17.000000 Pandora-ChatGPT-1.0.0/Pandora_ChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 10:26:17.000000 Pandora-ChatGPT-1.0.0/Pandora_ChatGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-13 10:26:17.000000 Pandora-ChatGPT-1.0.0/Pandora_ChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 10:26:17.000000 Pandora-ChatGPT-1.0.0/Pandora_ChatGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/requirements_api.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 10:26:17.000000 Pandora-ChatGPT-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:26:17.000000 Pandora-ChatGPT-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:26:17.000000 Pandora-ChatGPT-1.0.0/src/pandora/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:26:17.000000 Pandora-ChatGPT-1.0.0/src/pandora/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/bots/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/bots/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/cloud_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:26:17.000000 Pandora-ChatGPT-1.0.0/src/pandora/exts/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/exts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/exts/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/exts/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/exts/sentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/exts/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:26:17.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:26:17.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:26:17.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:26:17.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:26:17.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/
+-rw-r--r--   0 runner    (1001) docker     (123)   905448 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js
+-rw-r--r--   0 runner    (1001) docker     (123)   264961 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13147 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24138 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20480 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/68a27ff6-1185184b61bc22d0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/bd26816a-981e1ddc27b37cc6.js
+-rw-r--r--   0 runner    (1001) docker     (123)   141370 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js
+-rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:26:17.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)   305755 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/pages/_error-786d27d84962122a.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:26:17.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/pages/chat/
+-rw-r--r--   0 runner    (1001) docker     (123)   149531 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:26:17.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   108647 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/css/ac221fb2caad35a6.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:26:17.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_ssgManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/favicon-32x32.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:26:17.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    29912 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_Main-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    19412 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    19676 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_Main-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    30772 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_Main-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18668 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18748 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_Math-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    14408 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_Script-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_Size1-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_Size2-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_Size3-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_Size4-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   324208 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/Signifier-Regular.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   210840 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/Sohne-Buch.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   230012 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/Sohne-Halbfett.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    30824 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/SohneMono-Buch.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    31116 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/SohneMono-Halbfett.otf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:26:17.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:26:17.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/images/2022/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:26:17.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/images/2022/11/
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/static/images/2022/11/ChatGPT.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:26:17.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/flask/templates/chat.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:26:17.000000 Pandora-ChatGPT-1.0.0/src/pandora/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/migrations/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/migrations/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/migrations/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:26:17.000000 Pandora-ChatGPT-1.0.0/src/pandora/migrations/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/migrations/scripts/20230308_01_7ctOr.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:26:17.000000 Pandora-ChatGPT-1.0.0/src/pandora/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/openai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/openai/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/openai/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/openai/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:26:17.000000 Pandora-ChatGPT-1.0.0/src/pandora/turbo/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/turbo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/turbo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11071 2023-04-13 10:26:07.000000 Pandora-ChatGPT-1.0.0/src/pandora/turbo/chat.py
```

### Comparing `Pandora-ChatGPT-0.9.8/LICENSE` & `Pandora-ChatGPT-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/PKG-INFO` & `Pandora-ChatGPT-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: Pandora-ChatGPT
-Version: 0.9.8
+Version: 1.0.0
 Summary: A command-line interface to ChatGPT
 Home-page: https://github.com/pengzhile/pandora
 Author: Neo Peng
 Author-email: pengzhile@gmail.com
 Project-URL: Source, https://github.com/pengzhile/pandora
 Project-URL: Tracker, https://github.com/pengzhile/pandora/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus gpt-3.5-turbo gpt-3.5-turbo-0301
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Natural Language :: English
@@ -143,20 +143,22 @@
 
 * 可通过 `pandora --help` 查看。
 * `-p` 或 `--proxy` 指定代理，格式：`protocol://user:pass@ip:port`。
 * `-t` 或 `--token_file` 指定一个存放`Access Token`的文件，使用`Access Token`登录。
 * `-s` 或 `--server` 以`http`服务方式启动，格式：`ip:port`。
 * `-a` 或 `--api` 使用`gpt-3.5-turbo`API请求，**你可能需要向`OpenAI`支付费用**。
 * `-l` 或 `--local` 使用本地环境登录，**你可能需要一个合适的代理IP以避免账号被风控！**
+* `--tokens_file` 指定一个存放多`Access Token`的文件，内容为`{"key": "token"}`的形式。
 * `--sentry` 启用`sentry`框架来发送错误报告供作者查错，敏感信息**不会被发送**。
 * `-v` 或 `--verbose` 显示调试信息，且出错时打印异常堆栈信息，供查错使用。
 
 ## Docker环境变量
 
 * `PANDORA_ACCESS_TOKEN` 指定`Access Token`字符串。
+* `PANDORA_TOKENS_FILE` 指定一个存放多`Access Token`的文件路径。
 * `PANDORA_PROXY` 指定代理，格式：`protocol://user:pass@ip:port`。
 * `PANDORA_SERVER` 以`http`服务方式启动，格式：`ip:port`。
 * `PANDORA_API` 使用`gpt-3.5-turbo`API请求，**你可能需要向`OpenAI`支付费用**。
 * `PANDORA_LOGIN_LOCAL` 使用本地环境登录，**你可能需要一个合适的代理IP以避免账号被风控！**
 * `PANDORA_SENTRY` 启用`sentry`框架来发送错误报告供作者查错，敏感信息**不会被发送**。
 * `PANDORA_VERBOSE` 显示调试信息，且出错时打印异常堆栈信息，供查错使用。
 * 使用Docker方式，设置环境变量即可，无视上述`程序参数`。
@@ -199,37 +201,40 @@
 * 如果你想持久存储`Docker`中`Pandora`产生的数据，你可以挂载宿主机目录至`/data`。
 * 如果你在国内使用`pip`安装缓慢，可以考虑切换至腾讯的源：```pip config set global.index-url https://mirrors.cloud.tencent.com/pypi/simple```
 * 镜像同步版本可能不及时，如果出现这种情况建议切换至官方源：```pip config set global.index-url https://pypi.org/simple```
 * 默认使用`sqlite3`存储会话数据，如果你希望更换至`mysql`，可以这么做：
   * 执行```pip install PyMySQL```安装驱动。
   * 设置环境变量：`DATABASE_URI`为类似`mysql+pymysql://user:pass@localhost/dbname`的连接字符串。
 * 环境变量指定`OPENAI_EMAIL`可以替代登录输入用户名，`OPENAI_PASSWORD`则可以替代输入密码。
+* 环境变量`API_SYSTEM_PROMPT`可以替换`api`模式下的系统`prompt`。
 
 ## Cloud模式
 
 * 搭建一个跟官方很像的`ChatGPT`服务，不能说很像，只能说一样。
 * 该模式使用`pandora-cloud`启动，前提是你如前面所说安装好了。
 * Docker环境变量：`PANDORA_CLOUD` 启动`cloud`模式。
 * 该模式参数含义与普通模式相同，可`--help`查看。
 
 ## 使用Cloudflare Workers代理
 
 * 如果你感觉默认的`https://chat.gateway.do`在你那里可能被墙了，可以使用如下方法自行代理。
 * 你需要一个`Cloudflare`账号，如果没有，可以[注册](https://dash.cloudflare.com/sign-up)一个。
 * 登录后，点击`Workers`，然后点击`Create a Worker`，填入服务名称后点击`创建服务`。
 * 点开你刚才创建的服务，点击`快速编辑`按钮，贴入下面的代码，然后点击`保存并部署`。
+
   ```javascript
   export default {
     async fetch(request, env) {
       const url = new URL(request.url);
       url.host = 'chat.gateway.do';
       return fetch(new Request(url, request))
     }
   }
   ```
+
 * 点击`触发器`选项卡，可以添加自定义访问域名。
 * 参考`高阶设置`中的环境变量使用你的服务地址进行替换。
 * 这里有一个示例代理地址：`https://chat1.gateway.do`。
 
 ## 其他说明
 
 * 项目是站在其他巨人的肩膀上，感谢！
```

### Comparing `Pandora-ChatGPT-0.9.8/Pandora_ChatGPT.egg-info/PKG-INFO` & `Pandora-ChatGPT-1.0.0/Pandora_ChatGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: Pandora-ChatGPT
-Version: 0.9.8
+Version: 1.0.0
 Summary: A command-line interface to ChatGPT
 Home-page: https://github.com/pengzhile/pandora
 Author: Neo Peng
 Author-email: pengzhile@gmail.com
 Project-URL: Source, https://github.com/pengzhile/pandora
 Project-URL: Tracker, https://github.com/pengzhile/pandora/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus gpt-3.5-turbo gpt-3.5-turbo-0301
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Natural Language :: English
@@ -143,20 +143,22 @@
 
 * 可通过 `pandora --help` 查看。
 * `-p` 或 `--proxy` 指定代理，格式：`protocol://user:pass@ip:port`。
 * `-t` 或 `--token_file` 指定一个存放`Access Token`的文件，使用`Access Token`登录。
 * `-s` 或 `--server` 以`http`服务方式启动，格式：`ip:port`。
 * `-a` 或 `--api` 使用`gpt-3.5-turbo`API请求，**你可能需要向`OpenAI`支付费用**。
 * `-l` 或 `--local` 使用本地环境登录，**你可能需要一个合适的代理IP以避免账号被风控！**
+* `--tokens_file` 指定一个存放多`Access Token`的文件，内容为`{"key": "token"}`的形式。
 * `--sentry` 启用`sentry`框架来发送错误报告供作者查错，敏感信息**不会被发送**。
 * `-v` 或 `--verbose` 显示调试信息，且出错时打印异常堆栈信息，供查错使用。
 
 ## Docker环境变量
 
 * `PANDORA_ACCESS_TOKEN` 指定`Access Token`字符串。
+* `PANDORA_TOKENS_FILE` 指定一个存放多`Access Token`的文件路径。
 * `PANDORA_PROXY` 指定代理，格式：`protocol://user:pass@ip:port`。
 * `PANDORA_SERVER` 以`http`服务方式启动，格式：`ip:port`。
 * `PANDORA_API` 使用`gpt-3.5-turbo`API请求，**你可能需要向`OpenAI`支付费用**。
 * `PANDORA_LOGIN_LOCAL` 使用本地环境登录，**你可能需要一个合适的代理IP以避免账号被风控！**
 * `PANDORA_SENTRY` 启用`sentry`框架来发送错误报告供作者查错，敏感信息**不会被发送**。
 * `PANDORA_VERBOSE` 显示调试信息，且出错时打印异常堆栈信息，供查错使用。
 * 使用Docker方式，设置环境变量即可，无视上述`程序参数`。
@@ -199,37 +201,40 @@
 * 如果你想持久存储`Docker`中`Pandora`产生的数据，你可以挂载宿主机目录至`/data`。
 * 如果你在国内使用`pip`安装缓慢，可以考虑切换至腾讯的源：```pip config set global.index-url https://mirrors.cloud.tencent.com/pypi/simple```
 * 镜像同步版本可能不及时，如果出现这种情况建议切换至官方源：```pip config set global.index-url https://pypi.org/simple```
 * 默认使用`sqlite3`存储会话数据，如果你希望更换至`mysql`，可以这么做：
   * 执行```pip install PyMySQL```安装驱动。
   * 设置环境变量：`DATABASE_URI`为类似`mysql+pymysql://user:pass@localhost/dbname`的连接字符串。
 * 环境变量指定`OPENAI_EMAIL`可以替代登录输入用户名，`OPENAI_PASSWORD`则可以替代输入密码。
+* 环境变量`API_SYSTEM_PROMPT`可以替换`api`模式下的系统`prompt`。
 
 ## Cloud模式
 
 * 搭建一个跟官方很像的`ChatGPT`服务，不能说很像，只能说一样。
 * 该模式使用`pandora-cloud`启动，前提是你如前面所说安装好了。
 * Docker环境变量：`PANDORA_CLOUD` 启动`cloud`模式。
 * 该模式参数含义与普通模式相同，可`--help`查看。
 
 ## 使用Cloudflare Workers代理
 
 * 如果你感觉默认的`https://chat.gateway.do`在你那里可能被墙了，可以使用如下方法自行代理。
 * 你需要一个`Cloudflare`账号，如果没有，可以[注册](https://dash.cloudflare.com/sign-up)一个。
 * 登录后，点击`Workers`，然后点击`Create a Worker`，填入服务名称后点击`创建服务`。
 * 点开你刚才创建的服务，点击`快速编辑`按钮，贴入下面的代码，然后点击`保存并部署`。
+
   ```javascript
   export default {
     async fetch(request, env) {
       const url = new URL(request.url);
       url.host = 'chat.gateway.do';
       return fetch(new Request(url, request))
     }
   }
   ```
+
 * 点击`触发器`选项卡，可以添加自定义访问域名。
 * 参考`高阶设置`中的环境变量使用你的服务地址进行替换。
 * 这里有一个示例代理地址：`https://chat1.gateway.do`。
 
 ## 其他说明
 
 * 项目是站在其他巨人的肩膀上，感谢！
```

### Comparing `Pandora-ChatGPT-0.9.8/Pandora_ChatGPT.egg-info/SOURCES.txt` & `Pandora-ChatGPT-1.0.0/Pandora_ChatGPT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/README.md` & `Pandora-ChatGPT-1.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -106,20 +106,22 @@
 
 * 可通过 `pandora --help` 查看。
 * `-p` 或 `--proxy` 指定代理，格式：`protocol://user:pass@ip:port`。
 * `-t` 或 `--token_file` 指定一个存放`Access Token`的文件，使用`Access Token`登录。
 * `-s` 或 `--server` 以`http`服务方式启动，格式：`ip:port`。
 * `-a` 或 `--api` 使用`gpt-3.5-turbo`API请求，**你可能需要向`OpenAI`支付费用**。
 * `-l` 或 `--local` 使用本地环境登录，**你可能需要一个合适的代理IP以避免账号被风控！**
+* `--tokens_file` 指定一个存放多`Access Token`的文件，内容为`{"key": "token"}`的形式。
 * `--sentry` 启用`sentry`框架来发送错误报告供作者查错，敏感信息**不会被发送**。
 * `-v` 或 `--verbose` 显示调试信息，且出错时打印异常堆栈信息，供查错使用。
 
 ## Docker环境变量
 
 * `PANDORA_ACCESS_TOKEN` 指定`Access Token`字符串。
+* `PANDORA_TOKENS_FILE` 指定一个存放多`Access Token`的文件路径。
 * `PANDORA_PROXY` 指定代理，格式：`protocol://user:pass@ip:port`。
 * `PANDORA_SERVER` 以`http`服务方式启动，格式：`ip:port`。
 * `PANDORA_API` 使用`gpt-3.5-turbo`API请求，**你可能需要向`OpenAI`支付费用**。
 * `PANDORA_LOGIN_LOCAL` 使用本地环境登录，**你可能需要一个合适的代理IP以避免账号被风控！**
 * `PANDORA_SENTRY` 启用`sentry`框架来发送错误报告供作者查错，敏感信息**不会被发送**。
 * `PANDORA_VERBOSE` 显示调试信息，且出错时打印异常堆栈信息，供查错使用。
 * 使用Docker方式，设置环境变量即可，无视上述`程序参数`。
@@ -162,37 +164,40 @@
 * 如果你想持久存储`Docker`中`Pandora`产生的数据，你可以挂载宿主机目录至`/data`。
 * 如果你在国内使用`pip`安装缓慢，可以考虑切换至腾讯的源：```pip config set global.index-url https://mirrors.cloud.tencent.com/pypi/simple```
 * 镜像同步版本可能不及时，如果出现这种情况建议切换至官方源：```pip config set global.index-url https://pypi.org/simple```
 * 默认使用`sqlite3`存储会话数据，如果你希望更换至`mysql`，可以这么做：
   * 执行```pip install PyMySQL```安装驱动。
   * 设置环境变量：`DATABASE_URI`为类似`mysql+pymysql://user:pass@localhost/dbname`的连接字符串。
 * 环境变量指定`OPENAI_EMAIL`可以替代登录输入用户名，`OPENAI_PASSWORD`则可以替代输入密码。
+* 环境变量`API_SYSTEM_PROMPT`可以替换`api`模式下的系统`prompt`。
 
 ## Cloud模式
 
 * 搭建一个跟官方很像的`ChatGPT`服务，不能说很像，只能说一样。
 * 该模式使用`pandora-cloud`启动，前提是你如前面所说安装好了。
 * Docker环境变量：`PANDORA_CLOUD` 启动`cloud`模式。
 * 该模式参数含义与普通模式相同，可`--help`查看。
 
 ## 使用Cloudflare Workers代理
 
 * 如果你感觉默认的`https://chat.gateway.do`在你那里可能被墙了，可以使用如下方法自行代理。
 * 你需要一个`Cloudflare`账号，如果没有，可以[注册](https://dash.cloudflare.com/sign-up)一个。
 * 登录后，点击`Workers`，然后点击`Create a Worker`，填入服务名称后点击`创建服务`。
 * 点开你刚才创建的服务，点击`快速编辑`按钮，贴入下面的代码，然后点击`保存并部署`。
+
   ```javascript
   export default {
     async fetch(request, env) {
       const url = new URL(request.url);
       url.host = 'chat.gateway.do';
       return fetch(new Request(url, request))
     }
   }
   ```
+
 * 点击`触发器`选项卡，可以添加自定义访问域名。
 * 参考`高阶设置`中的环境变量使用你的服务地址进行替换。
 * 这里有一个示例代理地址：`https://chat1.gateway.do`。
 
 ## 其他说明
 
 * 项目是站在其他巨人的肩膀上，感谢！
```

### Comparing `Pandora-ChatGPT-0.9.8/setup.py` & `Pandora-ChatGPT-1.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         ]
     },
     project_urls={
         'Source': 'https://github.com/pengzhile/pandora',
         'Tracker': 'https://github.com/pengzhile/pandora/issues',
     },
     classifiers=[
-        'Development Status :: 4 - Beta',
+        'Development Status :: 5 - Production/Stable',
 
         'Environment :: Console',
         'Environment :: Web Environment',
 
         'Framework :: Flask',
 
         'Intended Audience :: Developers',
```

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/bots/legacy.py` & `Pandora-ChatGPT-1.0.0/src/pandora/bots/legacy.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,17 +31,20 @@
         self.user_prompts = []
         self.edit_index = None
 
 
 class ChatBot:
     def __init__(self, chatgpt):
         self.chatgpt = chatgpt
+        self.token_key = None
         self.state = None
 
     def run(self):
+        self.token_key = self.__choice_token_key()
+
         conversation_base = self.__choice_conversation()
         if conversation_base:
             self.__load_conversation(conversation_base['id'])
         else:
             self.__new_conversation()
 
         self.__talk_loop()
@@ -152,15 +155,15 @@
                 return
 
             self.state.edit_index = int(choice)
             return
 
     def __print_access_token(self):
         Console.warn_b('\n#### Your access token (keep it private)')
-        Console.warn(self.chatgpt.access_token)
+        Console.warn(self.chatgpt.get_access_token(token_key=self.token_key))
         print()
 
     def __clear_screen(self):
         Console.clear()
 
         if self.state:
             self.__print_conversation_title(self.state.title)
@@ -187,50 +190,50 @@
             return
 
         new_title = Prompt.ask('New title')
         if len(new_title) > 64:
             Console.error('#### Title too long.')
             return
 
-        if self.chatgpt.set_conversation_title(state.conversation_id, new_title):
+        if self.chatgpt.set_conversation_title(state.conversation_id, new_title, token=self.token_key):
             state.title = new_title
             Console.debug('#### Set title success.')
         else:
             Console.error('#### Set title failed.')
 
     def __clear_conversations(self):
         if not Confirm.ask('Are you sure?', default=False):
             return
 
-        if self.chatgpt.clear_conversations():
+        if self.chatgpt.clear_conversations(token=self.token_key):
             self.run()
         else:
             Console.error('#### Clear conversations failed.')
 
     def __del_conversation(self, state: State):
         if not state.conversation_id:
             Console.error('#### Conversation has not been created.')
             return
 
         if not Confirm.ask('Are you sure?', default=False):
             return
 
-        if self.chatgpt.del_conversation(state.conversation_id):
+        if self.chatgpt.del_conversation(state.conversation_id, token=self.token_key):
             self.run()
         else:
             Console.error('#### Delete conversation failed.')
 
     def __load_conversation(self, conversation_id):
         if not conversation_id:
             return
 
         self.state = State(conversation_id=conversation_id)
 
         nodes = []
-        result = self.chatgpt.get_conversation(conversation_id)
+        result = self.chatgpt.get_conversation(conversation_id, token=self.token_key)
         current_node_id = result['current_node']
 
         while True:
             node = result['mapping'][current_node_id]
             if not node.get('parent'):
                 break
 
@@ -284,44 +287,45 @@
             self.state.user_prompts = self.state.user_prompts[0:idx]
 
             self.state.edit_index = None
         else:
             self.state.user_prompt = ChatPrompt(prompt, parent_id=self.state.chatgpt_prompt.message_id)
 
         status, _, generator = self.chatgpt.talk(prompt, self.state.model_slug, self.state.user_prompt.message_id,
-                                                 self.state.user_prompt.parent_id, self.state.conversation_id)
+                                                 self.state.user_prompt.parent_id, self.state.conversation_id,
+                                                 token=self.token_key)
         self.__print_reply(status, generator)
 
         self.state.user_prompts.append(self.state.user_prompt)
 
         if first_prompt:
             new_title = self.chatgpt.gen_conversation_title(self.state.conversation_id, self.state.model_slug,
-                                                            self.state.chatgpt_prompt.message_id)
+                                                            self.state.chatgpt_prompt.message_id, token=self.token_key)
             self.state.title = new_title
             Console.debug_bh('#### Title generated: ' + new_title)
 
     def __regenerate_reply(self, state):
         if not state.conversation_id:
             Console.error('#### Conversation has not been created.')
             return
 
         status, _, generator = self.chatgpt.regenerate_reply(state.user_prompt.prompt, state.model_slug,
                                                              state.conversation_id, state.user_prompt.message_id,
-                                                             state.user_prompt.parent_id)
+                                                             state.user_prompt.parent_id, token=self.token_key)
         print()
         Console.success_b('ChatGPT:')
         self.__print_reply(status, generator)
 
     def __continue(self, state):
         if not state.conversation_id:
             Console.error('#### Conversation has not been created.')
             return
 
         status, _, generator = self.chatgpt.goon(state.model_slug, state.chatgpt_prompt.message_id,
-                                                 state.conversation_id)
+                                                 state.conversation_id, token=self.token_key)
         print()
         Console.success_b('ChatGPT:')
         self.__print_reply(status, generator)
 
     def __print_reply(self, status, generator):
         if 200 != status:
             raise Exception(status, next(generator))
@@ -350,15 +354,15 @@
 
             if text:
                 Console.success(text, end='')
 
         print('\n')
 
     def __choice_conversation(self, page=1, page_size=20):
-        conversations = self.chatgpt.list_conversations((page - 1) * page_size, page_size)
+        conversations = self.chatgpt.list_conversations((page - 1) * page_size, page_size, token=self.token_key)
         if not conversations['total']:
             return None
 
         choices = ['c', 'r', 'dd']
         items = conversations['items']
         first_page = 0 == conversations['offset']
         last_page = (conversations['offset'] + conversations['limit']) >= conversations['total']
@@ -379,21 +383,30 @@
             choices.append('p')
             Console.warn('  p.\t<< Previous page')
 
         Console.warn('  t?.\tSet title for the conversation, eg: t1')
         Console.warn('  d?.\tDelete the conversation, eg: d1')
         Console.warn('  dd.\t!! Clear all conversations')
         Console.warn('  r.\tRefresh conversation list')
+
+        if len(self.chatgpt.list_token_keys()) > 1:
+            choices.append('k')
+            Console.warn('  k.\tChoice access token')
+
         Console.warn('  c.\t** Start new chat')
 
         while True:
             choice = Prompt.ask('Your choice', choices=choices, show_choices=False)
             if 'c' == choice:
                 return None
 
+            if 'k' == choice:
+                self.run()
+                return
+
             if 'r' == choice:
                 return self.__choice_conversation(page, page_size)
 
             if 'n' == choice:
                 return self.__choice_conversation(page + 1, page_size)
 
             if 'p' == choice:
@@ -409,16 +422,35 @@
 
             if 'd' == choice[0]:
                 self.__del_conversation(State(conversation_id=items[int(choice[1:]) - 1]['id']))
                 continue
 
             return items[int(choice) - 1]
 
+    def __choice_token_key(self):
+        tokens = self.chatgpt.list_token_keys()
+
+        size = len(tokens)
+        if 1 == size:
+            return None
+
+        choices = ['r']
+        Console.info_b('Choice access token:')
+        for idx, item in enumerate(tokens):
+            number = str(idx + 1)
+            choices.append(number)
+            Console.info('  {}.\t{}'.format(number, item))
+
+        while True:
+            choice = Prompt.ask('Your choice', choices=choices, show_choices=False)
+
+            return tokens[int(choice) - 1]
+
     def __choice_model(self):
-        models = self.chatgpt.list_models()
+        models = self.chatgpt.list_models(token=self.token_key)
 
         size = len(models)
         if 1 == size:
             return models[0]
 
         choices = ['r']
         Console.info_b('Choice model:')
```

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/bots/server.py` & `Pandora-ChatGPT-1.0.0/src/pandora/bots/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,14 +98,18 @@
         self.logger.error(e)
 
         return make_response(jsonify({
             'code': e.code,
             'message': str(e.original_exception if self.debug and hasattr(e, 'original_exception') else e.name)
         }), 500)
 
+    @staticmethod
+    def __get_token_key():
+        return request.headers.get('X-Use-Token', None)
+
     def chat(self, conversation_id=None):
         query = {'chatId': [conversation_id]} if conversation_id else {}
 
         return render_template('chat.html',
                                pandora_base=request.url_root.strip('/'),
                                pandora_sentry=self.sentry,
                                query=query
@@ -175,77 +179,80 @@
                 'can_continue',
             ],
         }
 
         return jsonify(ret)
 
     def list_models(self):
-        return self.__proxy_result(self.chatgpt.list_models(True))
+        return self.__proxy_result(self.chatgpt.list_models(True, self.__get_token_key()))
 
     def list_conversations(self):
         offset = request.args.get('offset', '1')
         limit = request.args.get('limit', '20')
 
-        return self.__proxy_result(self.chatgpt.list_conversations(offset, limit, True))
+        return self.__proxy_result(self.chatgpt.list_conversations(offset, limit, True, self.__get_token_key()))
 
     def get_conversation(self, conversation_id):
-        return self.__proxy_result(self.chatgpt.get_conversation(conversation_id, True))
+        return self.__proxy_result(self.chatgpt.get_conversation(conversation_id, True, self.__get_token_key()))
 
     def del_conversation(self, conversation_id):
-        return self.__proxy_result(self.chatgpt.del_conversation(conversation_id, True))
+        return self.__proxy_result(self.chatgpt.del_conversation(conversation_id, True, self.__get_token_key()))
 
     def clear_conversations(self):
-        return self.__proxy_result(self.chatgpt.clear_conversations(True))
+        return self.__proxy_result(self.chatgpt.clear_conversations(True, self.__get_token_key()))
 
     def set_conversation_title(self, conversation_id):
         title = request.json['title']
 
-        return self.__proxy_result(self.chatgpt.set_conversation_title(conversation_id, title, True))
+        return self.__proxy_result(
+            self.chatgpt.set_conversation_title(conversation_id, title, True, self.__get_token_key()))
 
     def gen_conversation_title(self, conversation_id):
         payload = request.json
         model = payload['model']
         message_id = payload['message_id']
 
-        return self.__proxy_result(self.chatgpt.gen_conversation_title(conversation_id, model, message_id, True))
+        return self.__proxy_result(
+            self.chatgpt.gen_conversation_title(conversation_id, model, message_id, True, self.__get_token_key()))
 
     def talk(self):
         payload = request.json
         prompt = payload['prompt']
         model = payload['model']
         message_id = payload['message_id']
         parent_message_id = payload['parent_message_id']
         conversation_id = payload.get('conversation_id')
         stream = payload.get('stream', True)
 
         return self.__process_stream(
-            *self.chatgpt.talk(prompt, model, message_id, parent_message_id, conversation_id, stream), stream)
+            *self.chatgpt.talk(prompt, model, message_id, parent_message_id, conversation_id, stream,
+                               self.__get_token_key()), stream)
 
     def goon(self):
         payload = request.json
         model = payload['model']
         parent_message_id = payload['parent_message_id']
         conversation_id = payload.get('conversation_id')
         stream = payload.get('stream', True)
 
         return self.__process_stream(
-            *self.chatgpt.goon(model, parent_message_id, conversation_id, stream), stream)
+            *self.chatgpt.goon(model, parent_message_id, conversation_id, stream, self.__get_token_key()), stream)
 
     def regenerate(self):
         payload = request.json
         prompt = payload['prompt']
         model = payload['model']
         message_id = payload['message_id']
         parent_message_id = payload['parent_message_id']
         conversation_id = payload['conversation_id']
         stream = payload.get('stream', True)
 
         return self.__process_stream(
-            *self.chatgpt.regenerate_reply(prompt, model, conversation_id, message_id, parent_message_id, stream),
-            stream)
+            *self.chatgpt.regenerate_reply(prompt, model, conversation_id, message_id, parent_message_id, stream,
+                                           self.__get_token_key()), stream)
 
     @staticmethod
     def __process_stream(status, headers, generator, stream):
         if stream:
             return Response(API.wrap_stream_out(generator, status), mimetype=headers['Content-Type'], status=status)
 
         last_json = None
```

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/cloud_launcher.py` & `Pandora-ChatGPT-1.0.0/src/pandora/cloud_launcher.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/exts/hooks.py` & `Pandora-ChatGPT-1.0.0/src/pandora/exts/hooks.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/exts/token.py` & `Pandora-ChatGPT-1.0.0/src/pandora/exts/token.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/113-23682f80a24dd00d.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/14-0cb0d20affbd720d.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/174-bd28069f281ef76f.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/1f110208-44a6f43ddc5e9011.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/264-13e92c51b0315184.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/360-442b869f1ba4bb1b.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/424-d1d3bfe6a3ca6c4a.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/554.9b8bfd0762461d74.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/762-222df1028c0c1555.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/949.1a6eb804b5e91f61.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/framework-7a789ee31d2a7534.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/main-149b337e061b4d04.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/pages/_app-aaa11de1926dcafe.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/pages/chat/[[...chatId]]-76751174916fa3f7.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/chunks/webpack-c9a868e8e0796ec6.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/css/ac221fb2caad35a6.css` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/css/ac221fb2caad35a6.css`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/_next/static/olf4sv64FWIcQ_zCGl90t/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/apple-touch-icon.png` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/favicon-16x16.png` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/favicon-32x32.png` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Bold.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_Caligraphic-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_Fraktur-Bold.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_Fraktur-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_Main-Bold.woff` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_Main-Bold.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_Main-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_Main-Italic.woff` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_Main-Italic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_Main-Regular.woff` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_Main-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_Math-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_Math-Italic.woff` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_Math-Italic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_SansSerif-Bold.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_SansSerif-Italic.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_SansSerif-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_Script-Regular.woff` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_Script-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_Size1-Regular.woff` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_Size1-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_Size2-Regular.woff` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_Size2-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_Size3-Regular.woff` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_Size3-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_Size4-Regular.woff` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_Size4-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/KaTeX_Typewriter-Regular.woff`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/Signifier-Regular.otf` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/Signifier-Regular.otf`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/Sohne-Buch.otf` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/Sohne-Buch.otf`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/Sohne-Halbfett.otf` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/Sohne-Halbfett.otf`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/SohneMono-Buch.otf` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/SohneMono-Buch.otf`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/fonts/SohneMono-Halbfett.otf` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/fonts/SohneMono-Halbfett.otf`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/static/images/2022/11/ChatGPT.jpg` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/static/images/2022/11/ChatGPT.jpg`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/flask/templates/chat.html` & `Pandora-ChatGPT-1.0.0/src/pandora/flask/templates/chat.html`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/launcher.py` & `Pandora-ChatGPT-1.0.0/src/pandora/launcher.py`

 * *Files 11% similar despite different names*

```diff
@@ -79,14 +79,36 @@
             return access_token, False
         elif 'del' == confirm:
             os.remove(app_token_file)
 
     return None, True
 
 
+def parse_access_tokens(tokens_file, api=False):
+    if not os.path.isfile(tokens_file):
+        raise Exception('Error: {} is not a file.'.format(tokens_file))
+
+    import json
+    with open(tokens_file, 'r') as f:
+        tokens = json.load(f)
+
+    valid_tokens = {}
+    for key, value in tokens.items():
+        if not check_access_token_out(value, api=api):
+            Console.error('### Access token id: {}'.format(key))
+            continue
+        valid_tokens[key] = value
+
+    if not valid_tokens:
+        Console.error('### No valid access tokens.')
+        return None
+
+    return valid_tokens
+
+
 def main():
     global __show_verbose
 
     api_prefix = getenv('CHATGPT_API_PREFIX', 'https://chat.gateway.do')
     prefix_changed = 'https://chat.gateway.do' != api_prefix
 
     Console.debug_b(
@@ -111,14 +133,21 @@
         '--token_file',
         help='Specify an access token file and login with your access token.',
         required=False,
         type=str,
         default=None,
     )
     parser.add_argument(
+        '--tokens_file',
+        help='Specify an access tokens json file.',
+        required=False,
+        type=str,
+        default=None,
+    )
+    parser.add_argument(
         '-s',
         '--server',
         help='Start as a proxy server. Format: ip:port, default: 127.0.0.1:8008',
         required=False,
         type=str,
         default=None,
         action='store',
@@ -163,38 +192,43 @@
             from .migrations.migrate import do_migrate
 
             do_migrate()
         except (ImportError, ModuleNotFoundError):
             Console.error_bh('### You need `pip install Pandora-ChatGPT[api]` to support API mode.')
             return
 
-    access_token, need_save = confirm_access_token(args.token_file, args.server, args.api)
-    if not access_token:
-        Console.info_b('Please enter your email and password to log in ChatGPT!')
-        if not args.local:
-            Console.warn(
-                'We login via {}{}'.format(api_prefix, '' if prefix_changed else ', but it doesn\'t retain your data.'))
-        email = getenv('OPENAI_EMAIL') or Prompt.ask('  Email')
-        password = getenv('OPENAI_PASSWORD') or Prompt.ask('  Password', password=True)
-        Console.warn('### Do login, please wait...')
-        access_token = Auth0(email, password, args.proxy).auth(args.local)
-
-    if not check_access_token_out(access_token, args.api):
-        return
-
-    if need_save:
-        if args.server or Confirm.ask('Do you want to save your access token for the next login?', default=True):
-            save_access_token(access_token)
+    access_tokens = parse_access_tokens(args.tokens_file, args.api) if args.tokens_file else None
+
+    if not access_tokens:
+        access_token, need_save = confirm_access_token(args.token_file, args.server, args.api)
+        if not access_token:
+            Console.info_b('Please enter your email and password to log in ChatGPT!')
+            if not args.local:
+                Console.warn('We login via {}{}'.format(
+                    api_prefix, '' if prefix_changed else ', but it doesn\'t retain your data.'))
+            email = getenv('OPENAI_EMAIL') or Prompt.ask('  Email')
+            password = getenv('OPENAI_PASSWORD') or Prompt.ask('  Password', password=True)
+            Console.warn('### Do login, please wait...')
+            access_token = Auth0(email, password, args.proxy).auth(args.local)
+
+        if not check_access_token_out(access_token, args.api):
+            return
+
+        if need_save:
+            if args.server or Confirm.ask('Do you want to save your access token for the next login?', default=True):
+                save_access_token(access_token)
+
+        access_tokens = {'default': access_token}
 
     if args.api:
         from .turbo.chat import TurboGPT
 
-        chatgpt = TurboGPT(access_token, args.proxy)
+        chatgpt = TurboGPT(access_tokens, args.proxy)
     else:
-        chatgpt = ChatGPT(access_token, args.proxy)
+        chatgpt = ChatGPT(access_tokens, args.proxy)
 
     if args.server:
         return ChatBotServer(chatgpt, args.verbose, args.sentry).run(args.server)
 
     ChatBotLegacy(chatgpt).run()
```

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/migrations/migrate.py` & `Pandora-ChatGPT-1.0.0/src/pandora/migrations/migrate.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/migrations/models.py` & `Pandora-ChatGPT-1.0.0/src/pandora/migrations/models.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/migrations/scripts/20230308_01_7ctOr.sql` & `Pandora-ChatGPT-1.0.0/src/pandora/migrations/scripts/20230308_01_7ctOr.sql`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/openai/api.py` & `Pandora-ChatGPT-1.0.0/src/pandora/openai/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -87,134 +87,144 @@
         t = threading.Thread(target=asyncio.run, args=(self._do_request_sse(url, headers, data, queue, e),))
         t.start()
 
         return queue.get(), queue.get(), self.__generate_wrap(queue, t, e)
 
 
 class ChatGPT(API):
-    def __init__(self, access_token, proxy=None):
-        self.access_token = access_token
+    def __init__(self, access_tokens: dict, proxy=None):
+        self.access_tokens = access_tokens
+        self.access_token_key_list = list(access_tokens)
+        self.default_token_key = self.access_token_key_list[0]
         self.session = requests.Session()
         self.req_kwargs = {
             'proxies': {
                 'http': proxy,
                 'https': proxy,
             } if proxy else None,
             'verify': where(),
             'timeout': 100,
             'allow_redirects': False,
         }
 
         self.user_agent = 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) ' \
                           'Pandora/{} Safari/537.36'.format(__version__)
-        self.basic_headers = {
-            'Authorization': 'Bearer ' + self.access_token,
+
+        self.api_prefix = getenv('CHATGPT_API_PREFIX', 'https://chat.gateway.do')
+
+        super().__init__(proxy, self.req_kwargs['verify'])
+
+    def __get_headers(self, token_key=None):
+        return {
+            'Authorization': 'Bearer ' + self.get_access_token(token_key),
             'User-Agent': self.user_agent,
             'Content-Type': 'application/json',
         }
 
-        self.api_prefix = getenv('CHATGPT_API_PREFIX', 'https://chat.gateway.do')
+    def get_access_token(self, token_key=None):
+        return self.access_tokens[token_key or self.default_token_key]
 
-        super().__init__(proxy, self.req_kwargs['verify'])
+    def list_token_keys(self):
+        return self.access_token_key_list
 
-    def list_models(self, raw=False):
+    def list_models(self, raw=False, token=None):
         url = '{}/api/models'.format(self.api_prefix)
-        resp = self.session.get(url=url, headers=self.basic_headers, **self.req_kwargs)
+        resp = self.session.get(url=url, headers=self.__get_headers(token), **self.req_kwargs)
 
         if raw:
             return resp
 
         if resp.status_code != 200:
             raise Exception('list models failed: ' + self.__get_error(resp))
 
         result = resp.json()
         if 'models' not in result:
             raise Exception('list models failed: ' + resp.text)
 
         return result['models']
 
-    def list_conversations(self, offset, limit, raw=False):
+    def list_conversations(self, offset, limit, raw=False, token=None):
         url = '{}/api/conversations?offset={}&limit={}'.format(self.api_prefix, offset, limit)
-        resp = self.session.get(url=url, headers=self.basic_headers, **self.req_kwargs)
+        resp = self.session.get(url=url, headers=self.__get_headers(token), **self.req_kwargs)
 
         if raw:
             return resp
 
         if resp.status_code != 200:
             raise Exception('list conversations failed: ' + self.__get_error(resp))
 
         return resp.json()
 
-    def get_conversation(self, conversation_id, raw=False):
+    def get_conversation(self, conversation_id, raw=False, token=None):
         url = '{}/api/conversation/{}'.format(self.api_prefix, conversation_id)
-        resp = self.session.get(url=url, headers=self.basic_headers, **self.req_kwargs)
+        resp = self.session.get(url=url, headers=self.__get_headers(token), **self.req_kwargs)
 
         if raw:
             return resp
 
         if resp.status_code != 200:
             raise Exception('get conversation failed: ' + self.__get_error(resp))
 
         return resp.json()
 
-    def clear_conversations(self, raw=False):
+    def clear_conversations(self, raw=False, token=None):
         data = {
             'is_visible': False,
         }
 
         url = '{}/api/conversations'.format(self.api_prefix)
-        resp = self.session.patch(url=url, headers=self.basic_headers, json=data, **self.req_kwargs)
+        resp = self.session.patch(url=url, headers=self.__get_headers(token), json=data, **self.req_kwargs)
 
         if raw:
             return resp
 
         if resp.status_code != 200:
             raise Exception('clear conversations failed: ' + self.__get_error(resp))
 
         result = resp.json()
         if 'success' not in result:
             raise Exception('clear conversations failed: ' + resp.text)
 
         return result['success']
 
-    def del_conversation(self, conversation_id, raw=False):
+    def del_conversation(self, conversation_id, raw=False, token=None):
         data = {
             'is_visible': False,
         }
 
-        return self.__update_conversation(conversation_id, data, raw)
+        return self.__update_conversation(conversation_id, data, raw, token)
 
-    def gen_conversation_title(self, conversation_id, model, message_id, raw=False):
+    def gen_conversation_title(self, conversation_id, model, message_id, raw=False, token=None):
         url = '{}/api/conversation/gen_title/{}'.format(self.api_prefix, conversation_id)
         data = {
             'model': model,
             'message_id': message_id,
         }
-        resp = self.session.post(url=url, headers=self.basic_headers, json=data, **self.req_kwargs)
+        resp = self.session.post(url=url, headers=self.__get_headers(token), json=data, **self.req_kwargs)
 
         if raw:
             return resp
 
         if resp.status_code != 200:
             raise Exception('gen title failed: ' + self.__get_error(resp))
 
         result = resp.json()
         if 'title' not in result:
             raise Exception('gen title failed: ' + resp.text)
 
         return result['title']
 
-    def set_conversation_title(self, conversation_id, title, raw=False):
+    def set_conversation_title(self, conversation_id, title, raw=False, token=None):
         data = {
             'title': title,
         }
 
-        return self.__update_conversation(conversation_id, data, raw)
+        return self.__update_conversation(conversation_id, data, raw, token)
 
-    def talk(self, prompt, model, message_id, parent_message_id, conversation_id=None, stream=True):
+    def talk(self, prompt, model, message_id, parent_message_id, conversation_id=None, stream=True, token=None):
         data = {
             'action': 'next',
             'messages': [
                 {
                     'id': message_id,
                     'role': 'user',
                     'author': {
@@ -229,27 +239,27 @@
             'model': model,
             'parent_message_id': parent_message_id,
         }
 
         if conversation_id:
             data['conversation_id'] = conversation_id
 
-        return self.__request_conversation(data)
+        return self.__request_conversation(data, token)
 
-    def goon(self, model, parent_message_id, conversation_id, stream=True):
+    def goon(self, model, parent_message_id, conversation_id, stream=True, token=None):
         data = {
             'action': 'continue',
             'conversation_id': conversation_id,
             'model': model,
             'parent_message_id': parent_message_id,
         }
 
-        return self.__request_conversation(data)
+        return self.__request_conversation(data, token)
 
-    def regenerate_reply(self, prompt, model, conversation_id, message_id, parent_message_id, stream=True):
+    def regenerate_reply(self, prompt, model, conversation_id, message_id, parent_message_id, stream=True, token=None):
         data = {
             'action': 'variant',
             'messages': [
                 {
                     'id': message_id,
                     'role': 'user',
                     'author': {
@@ -262,25 +272,25 @@
                 }
             ],
             'model': model,
             'conversation_id': conversation_id,
             'parent_message_id': parent_message_id,
         }
 
-        return self.__request_conversation(data)
+        return self.__request_conversation(data, token)
 
-    def __request_conversation(self, data):
+    def __request_conversation(self, data, token=None):
         url = '{}/api/conversation'.format(self.api_prefix)
-        headers = {**self.session.headers, **self.basic_headers, 'Accept': 'text/event-stream'}
+        headers = {**self.session.headers, **self.__get_headers(token), 'Accept': 'text/event-stream'}
 
         return self._request_sse(url, headers, data)
 
-    def __update_conversation(self, conversation_id, data, raw=False):
+    def __update_conversation(self, conversation_id, data, raw=False, token=None):
         url = '{}/api/conversation/{}'.format(self.api_prefix, conversation_id)
-        resp = self.session.patch(url=url, headers=self.basic_headers, json=data, **self.req_kwargs)
+        resp = self.session.patch(url=url, headers=self.__get_headers(token), json=data, **self.req_kwargs)
 
         if raw:
             return resp
 
         if resp.status_code != 200:
             raise Exception('update conversation failed: ' + self.__get_error(resp))
 
@@ -295,52 +305,53 @@
         try:
             return str(resp.json()['detail'])
         except:
             return resp.text
 
 
 class ChatCompletion(API):
-    def __init__(self, api_key, proxy=None):
-        self.api_key = api_key
+    def __init__(self, proxy=None):
         self.session = requests.Session()
         self.req_kwargs = {
             'proxies': {
                 'http': proxy,
                 'https': proxy,
             } if proxy else None,
             'verify': where(),
             'timeout': 600,
             'allow_redirects': False,
         }
 
         self.user_agent = 'pandora/{}'.format(__version__)
-        self.basic_headers = {
-            'Authorization': 'Bearer ' + self.api_key,
+
+        super().__init__(proxy, self.req_kwargs['verify'])
+
+    def __get_headers(self, api_key):
+        return {
+            'Authorization': 'Bearer ' + api_key,
             'User-Agent': self.user_agent,
             'Content-Type': 'application/json',
         }
 
-        super().__init__(proxy, self.req_kwargs['verify'])
-
-    def request(self, model, messages, stream=True, **kwargs):
+    def request(self, api_key, model, messages, stream=True, **kwargs):
         data = {
             'model': model,
             'messages': messages,
             **kwargs,
             'stream': stream,
         }
 
-        return self.__request_conversation(data, stream)
+        return self.__request_conversation(api_key, data, stream)
 
-    def __request_conversation(self, data, stream):
+    def __request_conversation(self, api_key, data, stream):
         url = '{}/v1/chat/completions'.format(getenv('OPENAI_API_PREFIX', 'https://api.openai.com'))
-        headers = {**self.basic_headers, 'Accept': 'text/event-stream'}
 
         if stream:
+            headers = {**self.__get_headers(api_key), 'Accept': 'text/event-stream'}
             return self._request_sse(url, headers, data)
 
-        resp = self.session.post(url=url, headers=self.basic_headers, json=data, **self.req_kwargs)
+        resp = self.session.post(url=url, headers=self.__get_headers(api_key), json=data, **self.req_kwargs)
 
         def __generate_wrap():
             yield resp.json()
 
         return resp.status_code, resp.headers, __generate_wrap()
```

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/openai/auth.py` & `Pandora-ChatGPT-1.0.0/src/pandora/openai/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         }
         data = {
             'state': state,
             'username': self.email,
             'js-available': 'true',
             'webauthn-available': 'true',
             'is-brave': 'false',
-            'webauthn-platform-available': 'true',
+            'webauthn-platform-available': 'false',
             'action': 'default',
         }
         resp = self.session.post(url, headers=headers, data=data, allow_redirects=False, **self.req_kwargs)
 
         if resp.status_code == 302:
             return self.__part_five(state1, state)
         else:
```

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/openai/utils.py` & `Pandora-ChatGPT-1.0.0/src/pandora/openai/utils.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/turbo/base.py` & `Pandora-ChatGPT-1.0.0/src/pandora/turbo/base.py`

 * *Files identical despite different names*

### Comparing `Pandora-ChatGPT-0.9.8/src/pandora/turbo/chat.py` & `Pandora-ChatGPT-1.0.0/src/pandora/turbo/chat.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,52 @@
 # -*- coding: utf-8 -*-
 
 import json
 from datetime import datetime as dt
+from os import getenv
 
 from requests import Response
 
 from .base import Conversations, UserPrompt, Prompt, SystemPrompt
 from ..openai.api import ChatCompletion
 from ..openai.token import gpt_num_tokens
 
 
 class TurboGPT:
-    SYSTEM_PROMPT = 'You are ChatGPT, a large language model trained by OpenAI. Answer as concisely as ' \
-                    'possible.\nKnowledge cutoff: 2021-09-01\nCurrent date: {}'.format(dt.now().strftime('%Y-%m-%d'))
+    DEFAULT_SYSTEM_PROMPT = 'You are ChatGPT, a large language model trained by OpenAI. ' \
+                            'Answer as concisely as possible.\nKnowledge cutoff: 2021-09-01\n' \
+                            'Current date: {}'.format(dt.now().strftime('%Y-%m-%d'))
     TITLE_PROMPT = 'Generate a brief title for our conversation.'
     MAX_TOKENS = 4096
 
-    def __init__(self, api_key, proxy=None):
-        self.api = ChatCompletion(api_key, proxy)
-        self.conversations = Conversations()
+    def __init__(self, api_keys: dict, proxy=None):
+        self.api_keys = api_keys
+        self.api_keys_key_list = list(api_keys)
+        self.default_api_keys_key = self.api_keys_key_list[0]
 
-    def list_models(self, raw=False):
+        self.api = ChatCompletion(proxy)
+        self.conversations_map = {}
+        self.system_prompt = getenv('API_SYSTEM_PROMPT', self.DEFAULT_SYSTEM_PROMPT)
+
+    def __get_conversations(self, api_keys_key=None):
+        if api_keys_key is None:
+            api_keys_key = self.default_api_keys_key
+
+        if api_keys_key not in self.conversations_map:
+            self.conversations_map[api_keys_key] = Conversations()
+
+        return self.conversations_map[api_keys_key]
+
+    def get_access_token(self, token_key=None):
+        return self.api_keys[token_key or self.default_api_keys_key]
+
+    def list_token_keys(self):
+        return self.api_keys_key_list
+
+    def list_models(self, raw=False, token=None):
         models = {
             'models': [{
                 'slug': 'gpt-3.5-turbo',
                 'max_tokens': 4096,
                 'title': 'Default',
                 'description': 'Turbo is the api model that powers ChatGPT',
                 'tags': []
@@ -32,18 +54,18 @@
         }
 
         if raw:
             return self.__wrap_response(models)
 
         return models['models']
 
-    def list_conversations(self, offset, limit, raw=False):
+    def list_conversations(self, offset, limit, raw=False, token=None):
         offset = int(offset)
         limit = int(limit)
-        total, items = self.conversations.list(offset, limit)
+        total, items = self.__get_conversations(token).list(offset, limit)
 
         stripped = []
         for item in items:
             stripped.append({
                 'id': item.conversation_id,
                 'title': item.title,
                 'create_time': dt.utcfromtimestamp(item.create_time).isoformat(),
@@ -52,18 +74,18 @@
         result = {'items': stripped, 'total': total, 'limit': limit, 'offset': offset}
 
         if raw:
             return self.__wrap_response(result)
 
         return result
 
-    def get_conversation(self, conversation_id, raw=False):
+    def get_conversation(self, conversation_id, raw=False, token=None):
         def __shadow():
             try:
-                conversation = self.conversations.guard_get(conversation_id)
+                conversation = self.__get_conversations(token).guard_get(conversation_id)
             except Exception as e:
                 return self.__out_error(str(e), 404)
 
             return self.__wrap_response(conversation.get_info())
 
         resp = __shadow()
 
@@ -71,39 +93,41 @@
             return resp
 
         if resp.status_code != 200:
             raise Exception('get conversation failed: ' + resp.json()['detail'])
 
         return resp.json()
 
-    def clear_conversations(self, raw=False):
+    def clear_conversations(self, raw=False, token=None):
         def __shadow():
-            self.conversations.clear()
+            self.__get_conversations(token).clear()
 
             result = {
                 'success': True
             }
 
             return self.__wrap_response(result)
 
         resp = __shadow()
 
         if raw:
             return resp
 
         return resp.json()['success']
 
-    def del_conversation(self, conversation_id, raw=False):
+    def del_conversation(self, conversation_id, raw=False, token=None):
         def __shadow():
+            conversations = self.__get_conversations(token)
+
             try:
-                conversation = self.conversations.guard_get(conversation_id)
+                conversation = conversations.guard_get(conversation_id)
             except Exception as e:
                 return self.__out_error(str(e), 404)
 
-            self.conversations.delete(conversation)
+            conversations.delete(conversation)
 
             result = {
                 'success': True
             }
 
             return self.__wrap_response(result)
 
@@ -113,30 +137,30 @@
             return resp
 
         if resp.status_code != 200:
             raise Exception('delete conversation failed: ' + resp.json()['detail'])
 
         return resp.json()['success']
 
-    def gen_conversation_title(self, conversation_id, model, message_id, raw=False):
+    def gen_conversation_title(self, conversation_id, model, message_id, raw=False, token=None):
         def __shadow():
-            conversation = self.conversations.get(conversation_id)
+            conversation = self.__get_conversations(token).get(conversation_id)
             if not conversation:
                 return self.__out_error('Conversation not found', 404)
 
             if 'New chat' != conversation.title:
                 message = {
                     'message': 'Conversation {} already has title \'{}\''.format(conversation_id, conversation.title)
                 }
                 return self.__wrap_response(message)
 
             messages = conversation.get_messages_directly(message_id)
             messages.append({'role': 'user', 'content': self.TITLE_PROMPT})
 
-            status, header, generator = self.api.request(model, messages, False)
+            status, header, generator = self.api.request(self.get_access_token(token), model, messages, False)
             last_ok, last = self.__get_completion(status, next(generator))
 
             if not last_ok:
                 return self.__out_error(last['detail'], status)
 
             conversation.set_title(last.strip('"'))
 
@@ -152,18 +176,18 @@
             return resp
 
         if resp.status_code != 200:
             raise Exception('generate title failed: ' + resp.text)
 
         return resp.json()['title']
 
-    def set_conversation_title(self, conversation_id, title, raw=False):
+    def set_conversation_title(self, conversation_id, title, raw=False, token=None):
         def __shadow():
             try:
-                conversation = self.conversations.guard_get(conversation_id)
+                conversation = self.__get_conversations(token).guard_get(conversation_id)
             except Exception as e:
                 return self.__out_error(str(e), 404)
 
             conversation.set_title(title)
 
             result = {
                 'success': True
@@ -177,59 +201,61 @@
             return resp
 
         if resp.status_code != 200:
             raise Exception('update conversation failed: ' + resp.json()['detail'])
 
         return resp.json()['success']
 
-    def talk(self, content, model, message_id, parent_message_id, conversation_id=None, stream=True):
+    def talk(self, content, model, message_id, parent_message_id, conversation_id=None, stream=True, token=None):
         system_prompt = None
         if conversation_id:
-            conversation = self.conversations.get(conversation_id)
+            conversation = self.__get_conversations(token).get(conversation_id)
             if not conversation:
                 return self.__out_error_stream('Conversation not found', 404)
 
             parent = conversation.get_prompt(parent_message_id)
         else:
-            conversation = self.conversations.new()
+            conversation = self.__get_conversations(token).new()
             parent = conversation.add_prompt(Prompt(parent_message_id))
-            parent = system_prompt = conversation.add_prompt(SystemPrompt(self.SYSTEM_PROMPT, parent))
+            parent = system_prompt = conversation.add_prompt(SystemPrompt(self.system_prompt, parent))
 
         conversation.add_prompt(UserPrompt(message_id, content, parent))
 
         user_prompt, gpt_prompt, messages = conversation.get_messages(message_id, model)
         try:
-            status, headers, generator = self.api.request(model, self.__reduce_messages(messages, model), stream)
+            status, headers, generator = self.api.request(self.get_access_token(token), model,
+                                                          self.__reduce_messages(messages, model), stream)
         except Exception as e:
             return self.__out_error_stream(str(e))
 
         def __out_generator():
             if 200 == status and system_prompt and stream:
                 yield self.__out_stream(conversation, system_prompt)
                 yield self.__out_stream(conversation, user_prompt)
 
             for line in generator:
                 yield self.__map_conversation(status, conversation, gpt_prompt, line)
 
         return status, headers, __out_generator()
 
-    def goon(self, model, parent_message_id, conversation_id, stream=True):
-        return self.regenerate_reply(None, model, conversation_id, parent_message_id, None, stream)
+    def goon(self, model, parent_message_id, conversation_id, stream=True, token=None):
+        return self.regenerate_reply(None, model, conversation_id, parent_message_id, None, stream, token)
 
-    def regenerate_reply(self, prompt, model, conversation_id, message_id, parent_message_id, stream=True):
+    def regenerate_reply(self, prompt, model, conversation_id, message_id, parent_message_id, stream=True, token=None):
         if not conversation_id:
             return self.__out_error_stream('Miss conversation_id', 400)
 
-        conversation = self.conversations.get(conversation_id)
+        conversation = self.__get_conversations(token).get(conversation_id)
         if not conversation:
             return self.__out_error_stream('Conversation not found', 404)
 
         user_prompt, gpt_prompt, messages = conversation.get_messages(message_id, model)
         try:
-            status, headers, generator = self.api.request(model, self.__reduce_messages(messages, model), stream)
+            status, headers, generator = self.api.request(self.get_access_token(token), model,
+                                                          self.__reduce_messages(messages, model), stream)
         except Exception as e:
             return self.__out_error_stream(str(e))
 
         def __out_generator():
             for line in generator:
                 yield self.__map_conversation(status, conversation, gpt_prompt, line)
```

