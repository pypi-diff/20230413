# Comparing `tmp/systembridgefrontend-3.6.3.dev6.tar.gz` & `tmp/systembridgefrontend-3.6.3.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgefrontend-3.6.3.dev6.tar", last modified: Mon Apr 10 15:37:56 2023, max compression
+gzip compressed data, was "systembridgefrontend-3.6.3.dev7.tar", last modified: Thu Apr 13 20:21:30 2023, max compression
```

## Comparing `systembridgefrontend-3.6.3.dev6.tar` & `systembridgefrontend-3.6.3.dev7.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:37:56.129467 systembridgefrontend-3.6.3.dev6/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-10 15:37:56.129467 systembridgefrontend-3.6.3.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-10 15:37:38.000000 systembridgefrontend-3.6.3.dev6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 15:37:56.129467 systembridgefrontend-3.6.3.dev6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-10 15:37:38.000000 systembridgefrontend-3.6.3.dev6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:37:56.117467 systembridgefrontend-3.6.3.dev6/systembridgefrontend/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-10 15:37:38.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-10 15:37:54.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:37:56.117467 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-04-10 15:37:38.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/404.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:37:56.117467 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:37:56.117467 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:37:56.117467 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/XS-5P8XtA7Eb2ws6Mgd-Q/
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/XS-5P8XtA7Eb2ws6Mgd-Q/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/XS-5P8XtA7Eb2ws6Mgd-Q/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:37:56.125467 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/
--rw-r--r--   0 runner    (1001) docker     (123)    60090 2023-04-10 15:37:38.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/134-8433e2a32ffe1264.js
--rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-04-10 15:37:38.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/142-595d06bd435adc4d.js
--rw-r--r--   0 runner    (1001) docker     (123)    51312 2023-04-10 15:37:38.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/154-539d3d9bf657b776.js
--rw-r--r--   0 runner    (1001) docker     (123)   116326 2023-04-10 15:37:38.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/171.d9b946d3f22277f9.js
--rw-r--r--   0 runner    (1001) docker     (123)    69736 2023-04-10 15:37:38.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/29107295-661baa9a9eae34db.js
--rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-04-10 15:37:38.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/316-6f37cda59ad7df64.js
--rw-r--r--   0 runner    (1001) docker     (123)    50369 2023-04-10 15:37:38.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/386-37509ae1b5f18ec9.js
--rw-r--r--   0 runner    (1001) docker     (123)    69187 2023-04-10 15:37:38.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/699-a9d1dd5afe8ccb50.js
--rw-r--r--   0 runner    (1001) docker     (123)    22819 2023-04-10 15:37:38.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/716-d1503f71e8e3fa88.js
--rw-r--r--   0 runner    (1001) docker     (123)    58348 2023-04-10 15:37:38.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/75fc9c18-25984afe689afff4.js
--rw-r--r--   0 runner    (1001) docker     (123)    16926 2023-04-10 15:37:38.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/767-9a32bf4c99b35e92.js
--rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-04-10 15:37:38.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/792-98bcf34693c3b84b.js
--rw-r--r--   0 runner    (1001) docker     (123)    56242 2023-04-10 15:37:38.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/804-851168188e16a507.js
--rw-r--r--   0 runner    (1001) docker     (123)    14674 2023-04-10 15:37:38.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/826-b7f8eabaf3afc6d5.js
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-04-10 15:37:38.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js
--rw-r--r--   0 runner    (1001) docker     (123)   141052 2023-04-10 15:37:38.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/framework-2c79e2a64abdb08b.js
--rw-r--r--   0 runner    (1001) docker     (123)    90665 2023-04-10 15:37:38.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/main-4dcb7f9b52833aba.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:37:56.125467 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/pages/
--rw-r--r--   0 runner    (1001) docker     (123)    50940 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/pages/_app-d073359675509c25.js
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/pages/_error-54de1933a164a1ff.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:37:56.125467 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/pages/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:37:56.125467 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/
--rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/openon-4be476ff83910730.js
--rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/setup-58dc331f38afcee4.js
--rw-r--r--   0 runner    (1001) docker     (123)     7219 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/pages/app/data-5b613fd056889656.js
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/pages/app/notification-7c4c891692a1e4f4.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:37:56.125467 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/pages/app/player/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/pages/app/player/audio-843238cdca1b0dca.js
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/pages/app/player/video-3aa85bafaac31d57.js
--rw-r--r--   0 runner    (1001) docker     (123)    12920 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/pages/app/settings-c25cd256e27b2200.js
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/pages/index-f934b9a030f633a0.js
--rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-04-10 15:37:38.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/reactPlayerDailyMotion.da042b36db7662eb.js
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/reactPlayerFacebook.3663ffcf10139668.js
--rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/reactPlayerFilePlayer.812fbc47cf3ccebc.js
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/reactPlayerKaltura.46641a0f37607223.js
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/reactPlayerMixcloud.258ac8431338b78a.js
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/reactPlayerPreview.9b535aa9cbcb0a91.js
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/reactPlayerSoundCloud.60e72fefd71eeb25.js
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/reactPlayerStreamable.c374322fbd4a05d5.js
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/reactPlayerTwitch.52035ec5fd363953.js
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/reactPlayerVidyard.8c3ec4a7a5b4aac4.js
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/reactPlayerVimeo.5a5700a7f86e58a2.js
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/reactPlayerWistia.29aa97668baf75ea.js
--rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/reactPlayerYouTube.77a6d75e3f5e95ef.js
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/webpack-0eb9c66c948301b2.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:37:56.125467 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/css/12f80ebf97adb4a5.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:37:56.125467 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/media/
--rw-r--r--   0 runner    (1001) docker     (123)    65456 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/media/roboto-all-400-normal.2e9e9400.woff
--rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.2d9c9d60.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.d7827ae3.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.63e6dc18.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/media/roboto-greek-ext-400-normal.2b547ded.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/media/roboto-latin-400-normal.f2894edc.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/media/roboto-latin-ext-400-normal.21abc8c8.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/media/roboto-vietnamese-400-normal.c95fc061.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:37:56.125467 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:37:56.125467 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/app/bridges/
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/app/bridges/openon.html
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/app/bridges/setup.html
--rw-r--r--   0 runner    (1001) docker     (123)    19857 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/app/data.html
--rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/app/notification.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:37:56.129467 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/app/player/
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/app/player/audio.html
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/app/player/video.html
--rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-04-10 15:37:39.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/app/settings.html
--rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-04-10 15:37:38.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-04-10 15:37:38.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:37:56.117467 systembridgefrontend-3.6.3.dev6/systembridgefrontend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-10 15:37:56.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-04-10 15:37:56.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 15:37:56.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-10 15:37:56.000000 systembridgefrontend-3.6.3.dev6/systembridgefrontend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:21:30.241216 systembridgefrontend-3.6.3.dev7/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-13 20:21:30.241216 systembridgefrontend-3.6.3.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-13 20:21:10.000000 systembridgefrontend-3.6.3.dev7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 20:21:30.245216 systembridgefrontend-3.6.3.dev7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-13 20:21:10.000000 systembridgefrontend-3.6.3.dev7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:21:30.233216 systembridgefrontend-3.6.3.dev7/systembridgefrontend/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-13 20:21:10.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-13 20:21:27.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:21:30.233216 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/404.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:21:30.229216 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:21:30.233216 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:21:30.237216 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/
+-rw-r--r--   0 runner    (1001) docker     (123)    60243 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/134-12358b6301524be4.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/142-595d06bd435adc4d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    51312 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/154-539d3d9bf657b776.js
+-rw-r--r--   0 runner    (1001) docker     (123)   116326 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/171.d9b946d3f22277f9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    69736 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/29107295-661baa9a9eae34db.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/316-6f37cda59ad7df64.js
+-rw-r--r--   0 runner    (1001) docker     (123)    50369 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/386-37509ae1b5f18ec9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    69187 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/699-5a81a459894f5a37.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22819 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/716-d1503f71e8e3fa88.js
+-rw-r--r--   0 runner    (1001) docker     (123)    58348 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/75fc9c18-25984afe689afff4.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16926 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/767-9a32bf4c99b35e92.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/792-98bcf34693c3b84b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    56215 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/804-0a6dab4d173f5c2e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14674 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/826-b7f8eabaf3afc6d5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)   141052 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/framework-2c79e2a64abdb08b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    90665 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/main-4dcb7f9b52833aba.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:21:30.237216 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)    59133 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/pages/_app-3c2428351a583313.js
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/pages/_error-54de1933a164a1ff.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:21:30.241216 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/pages/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:21:30.241216 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/openon-4be476ff83910730.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/setup-58dc331f38afcee4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7219 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/pages/app/data-5b613fd056889656.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/pages/app/notification-7c4c891692a1e4f4.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:21:30.241216 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/pages/app/player/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/pages/app/player/audio-843238cdca1b0dca.js
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/pages/app/player/video-3aa85bafaac31d57.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12920 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/pages/app/settings-c25cd256e27b2200.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/pages/index-f934b9a030f633a0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/reactPlayerDailyMotion.da042b36db7662eb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/reactPlayerFacebook.3663ffcf10139668.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/reactPlayerFilePlayer.812fbc47cf3ccebc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/reactPlayerKaltura.46641a0f37607223.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/reactPlayerMixcloud.258ac8431338b78a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/reactPlayerPreview.9b535aa9cbcb0a91.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/reactPlayerSoundCloud.60e72fefd71eeb25.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/reactPlayerStreamable.c374322fbd4a05d5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/reactPlayerTwitch.52035ec5fd363953.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/reactPlayerVidyard.8c3ec4a7a5b4aac4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/reactPlayerVimeo.5a5700a7f86e58a2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/reactPlayerWistia.29aa97668baf75ea.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/reactPlayerYouTube.77a6d75e3f5e95ef.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/webpack-0eb9c66c948301b2.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:21:30.241216 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/css/12f80ebf97adb4a5.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:21:30.241216 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/media/
+-rw-r--r--   0 runner    (1001) docker     (123)    65456 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/media/roboto-all-400-normal.2e9e9400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.2d9c9d60.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.d7827ae3.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.63e6dc18.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/media/roboto-greek-ext-400-normal.2b547ded.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-04-13 20:21:12.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/media/roboto-latin-400-normal.f2894edc.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-04-13 20:21:12.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/media/roboto-latin-ext-400-normal.21abc8c8.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-04-13 20:21:12.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/media/roboto-vietnamese-400-normal.c95fc061.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:21:30.241216 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/sp5R1Ft1Y5yEAP_a5YQcA/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-13 20:21:12.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/sp5R1Ft1Y5yEAP_a5YQcA/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-13 20:21:12.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/sp5R1Ft1Y5yEAP_a5YQcA/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:21:30.241216 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:21:30.241216 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/app/bridges/
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-04-13 20:21:12.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/app/bridges/openon.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-04-13 20:21:12.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/app/bridges/setup.html
+-rw-r--r--   0 runner    (1001) docker     (123)    19857 2023-04-13 20:21:12.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/app/data.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-04-13 20:21:12.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/app/notification.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:21:30.241216 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/app/player/
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-04-13 20:21:12.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/app/player/audio.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-04-13 20:21:12.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/app/player/video.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-04-13 20:21:12.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/app/settings.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-04-13 20:21:11.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:21:30.233216 systembridgefrontend-3.6.3.dev7/systembridgefrontend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-13 20:21:30.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-04-13 20:21:30.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:21:30.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-13 20:21:30.000000 systembridgefrontend-3.6.3.dev7/systembridgefrontend.egg-info/top_level.txt
```

### Comparing `systembridgefrontend-3.6.3.dev6/pyproject.toml` & `systembridgefrontend-3.6.3.dev7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/setup.py` & `systembridgefrontend-3.6.3.dev7/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/404.html` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/404.html`

 * *Files 14% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>404: This page could not be found</title><meta name="next-head-count" content="3"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/12f80ebf97adb4a5.css" as="style"/><link rel="stylesheet" href="/_next/static/css/12f80ebf97adb4a5.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-0eb9c66c948301b2.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-4dcb7f9b52833aba.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d073359675509c25.js" defer=""></script><script src="/_next/static/chunks/pages/_error-54de1933a164a1ff.js" defer=""></script><script src="/_next/static/XS-5P8XtA7Eb2ws6Mgd-Q/_buildManifest.js" defer=""></script><script src="/_next/static/XS-5P8XtA7Eb2ws6Mgd-Q/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><div style="font-family:system-ui,&quot;Segoe UI&quot;,Roboto,Helvetica,Arial,sans-serif,&quot;Apple Color Emoji&quot;,&quot;Segoe UI Emoji&quot;;height:100vh;text-align:center;display:flex;flex-direction:column;align-items:center;justify-content:center"><div><style>body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}</style><h1 class="next-error-h1" style="display:inline-block;margin:0 20px 0 0;padding-right:23px;font-size:24px;font-weight:500;vertical-align:top;line-height:49px">404</h1><div style="display:inline-block;text-align:left"><h2 style="font-size:14px;font-weight:400;line-height:49px;margin:0">This page could not be found<!-- -->.</h2></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"statusCode":404}},"page":"/_error","query":{},"buildId":"XS-5P8XtA7Eb2ws6Mgd-Q","nextExport":true,"isFallback":false,"gip":true,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>404: This page could not be found</title><meta name="next-head-count" content="3"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/12f80ebf97adb4a5.css" as="style"/><link rel="stylesheet" href="/_next/static/css/12f80ebf97adb4a5.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-0eb9c66c948301b2.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-4dcb7f9b52833aba.js" defer=""></script><script src="/_next/static/chunks/pages/_app-3c2428351a583313.js" defer=""></script><script src="/_next/static/chunks/pages/_error-54de1933a164a1ff.js" defer=""></script><script src="/_next/static/sp5R1Ft1Y5yEAP_a5YQcA/_buildManifest.js" defer=""></script><script src="/_next/static/sp5R1Ft1Y5yEAP_a5YQcA/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><div style="font-family:system-ui,&quot;Segoe UI&quot;,Roboto,Helvetica,Arial,sans-serif,&quot;Apple Color Emoji&quot;,&quot;Segoe UI Emoji&quot;;height:100vh;text-align:center;display:flex;flex-direction:column;align-items:center;justify-content:center"><div><style>body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}</style><h1 class="next-error-h1" style="display:inline-block;margin:0 20px 0 0;padding-right:23px;font-size:24px;font-weight:500;vertical-align:top;line-height:49px">404</h1><div style="display:inline-block;text-align:left"><h2 style="font-size:14px;font-weight:400;line-height:49px;margin:0">This page could not be found<!-- -->.</h2></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"statusCode":404}},"page":"/_error","query":{},"buildId":"sp5R1Ft1Y5yEAP_a5YQcA","nextExport":true,"isFallback":false,"gip":true,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/XS-5P8XtA7Eb2ws6Mgd-Q/_buildManifest.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/sp5R1Ft1Y5yEAP_a5YQcA/_buildManifest.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -12,8 +12,8 @@
         "/app/data": [a, c, s, t, "static/chunks/716-d1503f71e8e3fa88.js", "static/chunks/pages/app/data-5b613fd056889656.js"],
         "/app/notification": [a, s, i, "static/chunks/pages/app/notification-7c4c891692a1e4f4.js"],
         "/app/player/audio": [a, c, b, s, e, f, u, "static/chunks/pages/app/player/audio-843238cdca1b0dca.js"],
         "/app/player/video": [a, c, b, s, e, f, u, "static/chunks/pages/app/player/video-3aa85bafaac31d57.js"],
         "/app/settings": [a, c, s, e, t, p, d, n, "static/chunks/826-b7f8eabaf3afc6d5.js", "static/chunks/pages/app/settings-c25cd256e27b2200.js"],
         sortedPages: ["/", "/_app", "/_error", "/app/bridges/openon", "/app/bridges/setup", "/app/data", "/app/notification", "/app/player/audio", "/app/player/video", "/app/settings"]
     }
-}("static/chunks/b2e984c5-f44d94ec783f59d4.js", "static/chunks/134-8433e2a32ffe1264.js", "static/chunks/792-98bcf34693c3b84b.js", "static/chunks/316-6f37cda59ad7df64.js", "static/chunks/29107295-661baa9a9eae34db.js", "static/chunks/699-a9d1dd5afe8ccb50.js", "static/chunks/154-539d3d9bf657b776.js", "static/chunks/804-851168188e16a507.js", "static/chunks/767-9a32bf4c99b35e92.js", "static/chunks/75fc9c18-25984afe689afff4.js", "static/chunks/386-37509ae1b5f18ec9.js", "static/chunks/142-595d06bd435adc4d.js"), self.__BUILD_MANIFEST_CB && self.__BUILD_MANIFEST_CB();
+}("static/chunks/b2e984c5-f44d94ec783f59d4.js", "static/chunks/134-12358b6301524be4.js", "static/chunks/792-98bcf34693c3b84b.js", "static/chunks/316-6f37cda59ad7df64.js", "static/chunks/29107295-661baa9a9eae34db.js", "static/chunks/699-5a81a459894f5a37.js", "static/chunks/154-539d3d9bf657b776.js", "static/chunks/804-0a6dab4d173f5c2e.js", "static/chunks/767-9a32bf4c99b35e92.js", "static/chunks/75fc9c18-25984afe689afff4.js", "static/chunks/386-37509ae1b5f18ec9.js", "static/chunks/142-595d06bd435adc4d.js"), self.__BUILD_MANIFEST_CB && self.__BUILD_MANIFEST_CB();
```

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/134-8433e2a32ffe1264.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/134-12358b6301524be4.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -202,19 +202,19 @@
                             style: C
                         }, M, n.createElement("rect", {
                             width: "24",
                             height: "24",
                             fill: "transparent"
                         }))));
                         var _, j = T,
-                            B = !0 === w || "number" != typeof w ? 2 : w,
-                            I = !O && (b || x);
-                        if (B < 0 && (I = !I), w && (j = n.createElement("g", {
+                            I = !0 === w || "number" != typeof w ? 2 : w,
+                            B = !O && (b || x);
+                        if (I < 0 && (B = !B), w && (j = n.createElement("g", {
                                 style: {
-                                    animation: "spin" + (I ? "-inverse" : "") + " linear " + Math.abs(B) + "s infinite",
+                                    animation: "spin" + (B ? "-inverse" : "") + " linear " + Math.abs(I) + "s infinite",
                                     transformOrigin: "center"
                                 }
                             }, T, !(b || x || 0 !== k) && n.createElement("rect", {
                                 width: "24",
                                 height: "24",
                                 fill: "transparent"
                             }))), O) return j;
@@ -228,15 +228,15 @@
                             style: C,
                             role: N,
                             "aria-labelledby": _
                         }, z), l && n.createElement("title", {
                             id: A
                         }, l), d && n.createElement("desc", {
                             id: L
-                        }, d), !O && w && (I ? n.createElement("style", null, "@keyframes spin-inverse { from { transform: rotate(0deg) } to { transform: rotate(-360deg) } }") : n.createElement("style", null, "@keyframes spin { from { transform: rotate(0deg) } to { transform: rotate(360deg) } }")), j)
+                        }, d), !O && w && (B ? n.createElement("style", null, "@keyframes spin-inverse { from { transform: rotate(0deg) } to { transform: rotate(-360deg) } }") : n.createElement("style", null, "@keyframes spin { from { transform: rotate(0deg) } to { transform: rotate(360deg) } }")), j)
                     });
                 d.displayName = "Icon", d.propTypes = {
                     path: o.string.isRequired,
                     size: o.oneOfType([o.number, o.string]),
                     color: o.string,
                     horizontal: o.bool,
                     vertical: o.bool,
@@ -395,59 +395,62 @@
                 });
             var Z = x
         },
         7357: function(e, t, r) {
             "use strict";
             r.d(t, {
                 Z: function() {
-                    return g
+                    return b
                 }
             });
             var n = r(7462),
                 o = r(3366),
                 i = r(7294),
                 a = r(6010),
                 l = r(9731),
                 s = r(6523),
                 c = r(9707),
                 u = r(6682),
                 p = r(5893);
             let d = ["className", "component"];
             var f = r(7078),
-                m = r(1919);
-            let h = (0, m.Z)(),
-                v = function(e = {}) {
+                m = r(1919),
+                h = r(606);
+            let v = (0, m.Z)(),
+                g = function(e = {}) {
                     let {
-                        defaultTheme: t,
-                        defaultClassName: r = "MuiBox-root",
-                        generateClassName: f
-                    } = e, m = (0, l.ZP)("div", {
+                        themeId: t,
+                        defaultTheme: r,
+                        defaultClassName: f = "MuiBox-root",
+                        generateClassName: m
+                    } = e, h = (0, l.ZP)("div", {
                         shouldForwardProp: e => "theme" !== e && "sx" !== e && "as" !== e
-                    })(s.Z), h = i.forwardRef(function(e, i) {
-                        let l = (0, u.Z)(t),
+                    })(s.Z), v = i.forwardRef(function(e, i) {
+                        let l = (0, u.Z)(r),
                             s = (0, c.Z)(e),
                             {
-                                className: h,
-                                component: v = "div"
+                                className: v,
+                                component: g = "div"
                             } = s,
-                            g = (0, o.Z)(s, d);
-                        return (0, p.jsx)(m, (0, n.Z)({
-                            as: v,
+                            b = (0, o.Z)(s, d);
+                        return (0, p.jsx)(h, (0, n.Z)({
+                            as: g,
                             ref: i,
-                            className: (0, a.Z)(h, f ? f(r) : r),
-                            theme: l
-                        }, g))
+                            className: (0, a.Z)(v, m ? m(f) : f),
+                            theme: t && l[t] || l
+                        }, b))
                     });
-                    return h
+                    return v
                 }({
-                    defaultTheme: h,
+                    themeId: h.Z,
+                    defaultTheme: v,
                     defaultClassName: "MuiBox-root",
                     generateClassName: f.Z.generate
                 });
-            var g = v
+            var b = g
         },
         3321: function(e, t, r) {
             "use strict";
             r.d(t, {
                 Z: function() {
                     return $
                 }
@@ -700,15 +703,15 @@
                         }),
                         _ = Z(T),
                         j = z && (0, y.jsx)(w, {
                             className: _.startIcon,
                             ownerState: T,
                             children: z
                         }),
-                        B = k && (0, y.jsx)(R, {
+                        I = k && (0, y.jsx)(R, {
                             className: _.endIcon,
                             ownerState: T,
                             children: k
                         });
                     return (0, y.jsxs)(S, (0, o.Z)({
                         ownerState: T,
                         className: (0, a.Z)(r.className, _.root, m),
@@ -716,15 +719,15 @@
                         disabled: h,
                         focusRipple: !g,
                         focusVisibleClassName: (0, a.Z)(_.focusVisible, C),
                         ref: t,
                         type: P
                     }, M, {
                         classes: _,
-                        children: [j, u, B]
+                        children: [j, u, I]
                     }))
                 });
             var $ = C
         },
         2022: function(e, t, r) {
             "use strict";
             let n, o, i, a;
@@ -1134,16 +1137,16 @@
                     }))
                 });
             var _ = r(4867);
 
             function j(e) {
                 return (0, _.Z)("MuiButtonBase", e)
             }
-            let B = (0, R.Z)("MuiButtonBase", ["root", "disabled", "focusVisible"]),
-                I = ["action", "centerRipple", "children", "className", "component", "disabled", "disableRipple", "disableTouchRipple", "focusRipple", "focusVisibleClassName", "LinkComponent", "onBlur", "onClick", "onContextMenu", "onDragLeave", "onFocus", "onFocusVisible", "onKeyDown", "onKeyUp", "onMouseDown", "onMouseLeave", "onMouseUp", "onTouchEnd", "onTouchMove", "onTouchStart", "tabIndex", "TouchRippleProps", "touchRippleRef", "type"],
+            let I = (0, R.Z)("MuiButtonBase", ["root", "disabled", "focusVisible"]),
+                B = ["action", "centerRipple", "children", "className", "component", "disabled", "disableRipple", "disableTouchRipple", "focusRipple", "focusVisibleClassName", "LinkComponent", "onBlur", "onClick", "onContextMenu", "onDragLeave", "onFocus", "onFocusVisible", "onKeyDown", "onKeyUp", "onMouseDown", "onMouseLeave", "onMouseUp", "onTouchEnd", "onTouchMove", "onTouchStart", "tabIndex", "TouchRippleProps", "touchRippleRef", "type"],
                 N = e => {
                     let {
                         disabled: t,
                         focusVisible: r,
                         focusVisibleClassName: n,
                         classes: o
                     } = e, i = (0, p.Z)({
@@ -1174,15 +1177,15 @@
                     MozAppearance: "none",
                     WebkitAppearance: "none",
                     textDecoration: "none",
                     color: "inherit",
                     "&::-moz-focus-inner": {
                         borderStyle: "none"
                     },
-                    [`&.${B.disabled}`]: {
+                    [`&.${I.disabled}`]: {
                         pointerEvents: "none",
                         cursor: "default"
                     },
                     "@media print": {
                         colorAdjust: "exact"
                     }
                 }),
@@ -1211,21 +1214,21 @@
                             onKeyDown: O,
                             onKeyUp: z,
                             onMouseDown: P,
                             onMouseLeave: E,
                             onMouseUp: M,
                             onTouchEnd: _,
                             onTouchMove: j,
-                            onTouchStart: B,
+                            onTouchStart: I,
                             tabIndex: L = 0,
                             TouchRippleProps: W,
                             touchRippleRef: F,
                             type: D
                         } = r,
-                        V = (0, s.Z)(r, I),
+                        V = (0, s.Z)(r, B),
                         q = c.useRef(null),
                         G = c.useRef(null),
                         U = (0, m.Z)(G, F),
                         {
                             isFocusVisibleRef: H,
                             onFocus: X,
                             onBlur: Y,
@@ -1250,15 +1253,15 @@
                     let en = er("start", P),
                         eo = er("stop", S),
                         ei = er("stop", R),
                         ea = er("stop", M),
                         el = er("stop", e => {
                             J && e.preventDefault(), E && E(e)
                         }),
-                        es = er("start", B),
+                        es = er("start", I),
                         ec = er("stop", _),
                         eu = er("stop", j),
                         ep = er("stop", e => {
                             Y(e), !1 === H.current && Q(!1), Z && Z(e)
                         }, !1),
                         ed = (0, h.Z)(e => {
                             q.current || (q.current = e.currentTarget), X(e), !0 === H.current && (Q(!0), $ && $(e)), C && C(e)
@@ -2222,43 +2225,46 @@
                 });
             var S = k
         },
         948: function(e, t, r) {
             "use strict";
             r.d(t, {
                 Dz: function() {
-                    return a
+                    return l
                 },
                 FO: function() {
-                    return i
+                    return a
                 }
             });
             var n = r(182),
-                o = r(247);
-            let i = e => (0, n.x9)(e) && "classes" !== e,
-                a = n.x9,
-                l = (0, n.ZP)({
+                o = r(247),
+                i = r(606);
+            let a = e => (0, n.x9)(e) && "classes" !== e,
+                l = n.x9,
+                s = (0, n.ZP)({
+                    themeId: i.Z,
                     defaultTheme: o.Z,
-                    rootShouldForwardProp: i
+                    rootShouldForwardProp: a
                 });
-            t.ZP = l
+            t.ZP = s
         },
         2734: function(e, t, r) {
             "use strict";
             r.d(t, {
                 Z: function() {
-                    return i
+                    return a
                 }
             }), r(7294);
             var n = r(6682),
-                o = r(247);
+                o = r(247),
+                i = r(606);
 
-            function i() {
+            function a() {
                 let e = (0, n.Z)(o.Z);
-                return e
+                return e[i.Z] || e
             }
         },
         8298: function(e, t, r) {
             "use strict";
             r.d(t, {
                 Z: function() {
                     return c
@@ -2404,15 +2410,15 @@
                             return e(t, (0, o.Z)({}, r, n, {
                                 shouldForwardProp: m(k, n, !0)
                             })).apply(void 0, y)
                         }, k
                     }
                 }).bind();
             /**
-             * @mui/styled-engine v5.11.16
+             * @mui/styled-engine v5.12.0
              *
              * @license MIT
              * This source code is licensed under the MIT license found in the
              * LICENSE file in the root directory of this source tree.
              */
             function g(e, t) {
                 let r = v(e, t);
@@ -2424,18 +2430,18 @@
                 Array.isArray(e.__emotion_styles) && (e.__emotion_styles = t(e.__emotion_styles))
             }
         },
         182: function(e, t, r) {
             "use strict";
             r.d(t, {
                 ZP: function() {
-                    return Z
+                    return y
                 },
                 x9: function() {
-                    return y
+                    return v
                 }
             });
             var n = r(3366),
                 o = r(7462),
                 i = r(9731),
                 a = r(6500),
                 l = r(8320);
@@ -2451,116 +2457,121 @@
                 } = e, r = (0, n.Z)(e, s), o = t || "";
                 return Object.keys(r).sort().forEach(t => {
                     "color" === t ? o += c(o) ? e[t] : (0, l.Z)(e[t]) : o += `${c(o)?t:(0,l.Z)(t)}${(0,l.Z)(e[t].toString())}`
                 }), o
             }
             var p = r(6523);
             let d = ["name", "slot", "skipVariantsResolver", "skipSx", "overridesResolver"],
-                f = ["theme"],
-                m = ["theme"];
-
-            function h(e) {
-                return 0 === Object.keys(e).length
-            }
-            let v = (e, t) => t.components && t.components[e] && t.components[e].styleOverrides ? t.components[e].styleOverrides : null,
-                g = (e, t) => {
+                f = (e, t) => t.components && t.components[e] && t.components[e].styleOverrides ? t.components[e].styleOverrides : null,
+                m = (e, t) => {
                     let r = [];
                     t && t.components && t.components[e] && t.components[e].variants && (r = t.components[e].variants);
                     let n = {};
                     return r.forEach(e => {
                         let t = u(e.props);
                         n[t] = e.style
                     }), n
                 },
-                b = (e, t, r, n) => {
+                h = (e, t, r, n) => {
                     var o, i;
                     let {
                         ownerState: a = {}
                     } = e, l = [], s = null == r ? void 0 : null == (o = r.components) ? void 0 : null == (i = o[n]) ? void 0 : i.variants;
                     return s && s.forEach(r => {
                         let n = !0;
                         Object.keys(r.props).forEach(t => {
                             a[t] !== r.props[t] && e[t] !== r.props[t] && (n = !1)
                         }), n && l.push(t[u(r.props)])
                     }), l
                 };
 
-            function y(e) {
+            function v(e) {
                 return "ownerState" !== e && "theme" !== e && "sx" !== e && "as" !== e
             }
-            let x = (0, a.Z)();
+            let g = (0, a.Z)();
 
-            function Z(e = {}) {
+            function b({
+                defaultTheme: e,
+                theme: t,
+                themeId: r
+            }) {
+                return 0 === Object.keys(t).length ? e : t[r] || t
+            }
+
+            function y(e = {}) {
                 let {
-                    defaultTheme: t = x,
-                    rootShouldForwardProp: r = y,
-                    slotShouldForwardProp: a = y
-                } = e, l = e => {
-                    let r = h(e.theme) ? t : e.theme;
-                    return (0, p.Z)((0, o.Z)({}, e, {
-                        theme: r
+                    themeId: t,
+                    defaultTheme: r = g,
+                    rootShouldForwardProp: a = v,
+                    slotShouldForwardProp: l = v
+                } = e, s = e => (0, p.Z)((0, o.Z)({}, e, {
+                    theme: b((0, o.Z)({}, e, {
+                        defaultTheme: r,
+                        themeId: t
                     }))
-                };
-                return l.__mui_systemSx = !0, (e, s = {}) => {
-                    let c;
+                }));
+                return s.__mui_systemSx = !0, (e, c = {}) => {
+                    let u;
                     (0, i.Co)(e, e => e.filter(e => !(null != e && e.__mui_systemSx)));
                     let {
-                        name: u,
-                        slot: p,
-                        skipVariantsResolver: x,
-                        skipSx: Z,
-                        overridesResolver: k
-                    } = s, S = (0, n.Z)(s, d), w = void 0 !== x ? x : p && "Root" !== p || !1, R = Z || !1, C = y;
-                    "Root" === p ? C = r : p ? C = a : "string" == typeof e && e.charCodeAt(0) > 96 && (C = void 0);
-                    let $ = (0, i.ZP)(e, (0, o.Z)({
-                            shouldForwardProp: C,
-                            label: c
-                        }, S)),
-                        O = (e, ...r) => {
-                            let i = r ? r.map(e => "function" == typeof e && e.__emotion_real !== e ? r => {
-                                    let {
-                                        theme: i
-                                    } = r, a = (0, n.Z)(r, f);
-                                    return e((0, o.Z)({
-                                        theme: h(i) ? t : i
-                                    }, a))
-                                } : e) : [],
+                        name: p,
+                        slot: g,
+                        skipVariantsResolver: y,
+                        skipSx: x,
+                        overridesResolver: Z
+                    } = c, k = (0, n.Z)(c, d), S = void 0 !== y ? y : g && "Root" !== g || !1, w = x || !1, R = v;
+                    "Root" === g ? R = a : g ? R = l : "string" == typeof e && e.charCodeAt(0) > 96 && (R = void 0);
+                    let C = (0, i.ZP)(e, (0, o.Z)({
+                            shouldForwardProp: R,
+                            label: u
+                        }, k)),
+                        $ = (e, ...n) => {
+                            let i = n ? n.map(e => "function" == typeof e && e.__emotion_real !== e ? n => e((0, o.Z)({}, n, {
+                                    theme: b((0, o.Z)({}, n, {
+                                        defaultTheme: r,
+                                        themeId: t
+                                    }))
+                                })) : e) : [],
                                 a = e;
-                            u && k && i.push(e => {
-                                let r = h(e.theme) ? t : e.theme,
-                                    n = v(u, r);
-                                if (n) {
+                            p && Z && i.push(e => {
+                                let n = b((0, o.Z)({}, e, {
+                                        defaultTheme: r,
+                                        themeId: t
+                                    })),
+                                    i = f(p, n);
+                                if (i) {
                                     let t = {};
-                                    return Object.entries(n).forEach(([n, i]) => {
-                                        t[n] = "function" == typeof i ? i((0, o.Z)({}, e, {
-                                            theme: r
+                                    return Object.entries(i).forEach(([r, i]) => {
+                                        t[r] = "function" == typeof i ? i((0, o.Z)({}, e, {
+                                            theme: n
                                         })) : i
-                                    }), k(e, t)
+                                    }), Z(e, t)
                                 }
                                 return null
-                            }), u && !w && i.push(e => {
-                                let r = h(e.theme) ? t : e.theme;
-                                return b(e, g(u, r), r, u)
-                            }), R || i.push(l);
-                            let s = i.length - r.length;
-                            if (Array.isArray(e) && s > 0) {
-                                let t = Array(s).fill("");
+                            }), p && !S && i.push(e => {
+                                let n = b((0, o.Z)({}, e, {
+                                    defaultTheme: r,
+                                    themeId: t
+                                }));
+                                return h(e, m(p, n), n, p)
+                            }), w || i.push(s);
+                            let l = i.length - n.length;
+                            if (Array.isArray(e) && l > 0) {
+                                let t = Array(l).fill("");
                                 (a = [...e, ...t]).raw = [...e.raw, ...t]
-                            } else "function" == typeof e && e.__emotion_real !== e && (a = r => {
-                                let {
-                                    theme: i
-                                } = r, a = (0, n.Z)(r, m);
-                                return e((0, o.Z)({
-                                    theme: h(i) ? t : i
-                                }, a))
-                            });
-                            let c = $(a, ...i);
+                            } else "function" == typeof e && e.__emotion_real !== e && (a = n => e((0, o.Z)({}, n, {
+                                theme: b((0, o.Z)({}, n, {
+                                    defaultTheme: r,
+                                    themeId: t
+                                }))
+                            })));
+                            let c = C(a, ...i);
                             return c
                         };
-                    return $.withConfig && (O.withConfig = $.withConfig), O
+                    return C.withConfig && ($.withConfig = C.withConfig), $
                 }
             }
         },
         9707: function(e, t, r) {
             "use strict";
             r.d(t, {
                 Z: function() {
```

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/142-595d06bd435adc4d.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/142-595d06bd435adc4d.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/154-539d3d9bf657b776.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/154-539d3d9bf657b776.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/171.d9b946d3f22277f9.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/171.d9b946d3f22277f9.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/29107295-661baa9a9eae34db.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/29107295-661baa9a9eae34db.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/316-6f37cda59ad7df64.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/316-6f37cda59ad7df64.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/386-37509ae1b5f18ec9.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/386-37509ae1b5f18ec9.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/699-a9d1dd5afe8ccb50.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/699-5a81a459894f5a37.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -517,15 +517,15 @@
                 R = r(7167),
                 w = r(4423),
                 S = r(948),
                 k = r(1657),
                 P = r(8216),
                 C = r(1705),
                 E = r(8974),
-                M = r(2287),
+                M = r(7297),
                 I = r(8712),
                 F = r(5827);
             let O = ["aria-describedby", "autoComplete", "autoFocus", "className", "color", "components", "componentsProps", "defaultValue", "disabled", "disableInjectingGlobalStyles", "endAdornment", "error", "fullWidth", "id", "inputComponent", "inputProps", "inputRef", "margin", "maxRows", "minRows", "multiline", "name", "onBlur", "onChange", "onClick", "onFocus", "onKeyDown", "onKeyUp", "placeholder", "readOnly", "renderSuffix", "rows", "size", "slotProps", "slots", "startAdornment", "type", "value"],
                 T = (e, t) => {
                     let {
                         ownerState: r
                     } = e;
@@ -3199,30 +3199,30 @@
                     width: "100%",
                     boxSizing: "border-box"
                 });
 
             function e8(e, t) {
                 return "object" == typeof t && null !== t ? e === t : String(e) === String(t)
             }
-            let e3 = e => {
+            let e9 = e => {
                     let {
                         classes: t,
                         variant: r,
                         disabled: n,
                         multiple: o,
                         open: i,
                         error: l
                     } = e, a = {
                         select: ["select", r, n && "disabled", o && "multiple", l && "error"],
                         icon: ["icon", `icon${(0,F.Z)(r)}`, i && "iconOpen", n && "disabled"],
                         nativeInput: ["nativeInput"]
                     };
                     return (0, d.Z)(a, e1, t)
                 },
-                e9 = a.forwardRef(function(e, t) {
+                e3 = a.forwardRef(function(e, t) {
                     var r;
                     let n, d;
                     let {
                         "aria-describedby": u,
                         "aria-label": c,
                         autoFocus: p,
                         autoWidth: f,
@@ -3367,15 +3367,15 @@
                     let eb = z.id || (C ? `mui-component-select-${C}` : void 0),
                         eZ = (0, i.Z)({}, e, {
                             variant: $,
                             value: W,
                             open: ec,
                             error: y
                         }),
-                        eg = e3(eZ);
+                        eg = e9(eZ);
                     return (0, v.jsxs)(a.Fragment, {
                         children: [(0, v.jsx)(e2, (0, i.Z)({
                             ref: et,
                             tabIndex: void 0 !== j ? j : g ? null : 0,
                             role: "button",
                             "aria-disabled": g ? "true" : void 0,
                             "aria-expanded": ec ? "true" : "false",
@@ -3508,15 +3508,15 @@
                             filled: (0, v.jsx)(tl, {
                                 ownerState: j
                             })
                         })[z],
                         B = (0, en.Z)(t, $.ref);
                     return (0, v.jsx)(a.Fragment, {
                         children: a.cloneElement($, (0, i.Z)({
-                            inputComponent: S ? eJ : e9,
+                            inputComponent: S ? eJ : e3,
                             inputProps: (0, i.Z)({
                                 children: o,
                                 error: A.error,
                                 IconComponent: h,
                                 variant: z,
                                 type: void 0,
                                 multiple: w
```

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/716-d1503f71e8e3fa88.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/716-d1503f71e8e3fa88.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/75fc9c18-25984afe689afff4.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/75fc9c18-25984afe689afff4.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/767-9a32bf4c99b35e92.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/767-9a32bf4c99b35e92.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/792-98bcf34693c3b84b.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/792-98bcf34693c3b84b.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/804-851168188e16a507.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/804-0a6dab4d173f5c2e.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1046,15 +1046,15 @@
 
             function eD(e) {
                 return (0, eL.Z)("MuiPopper", e)
             }(0, eA.Z)("MuiPopper", ["root"]);
             var eE = o(6504),
                 eM = o(1873),
                 eT = o(5893);
-            let ej = ["anchorEl", "children", "component", "direction", "disablePortal", "modifiers", "open", "ownerState", "placement", "popperOptions", "popperRef", "slotProps", "slots", "TransitionProps"],
+            let ej = ["anchorEl", "children", "component", "direction", "disablePortal", "modifiers", "open", "placement", "popperOptions", "popperRef", "slotProps", "slots", "TransitionProps", "ownerState"],
                 eN = ["anchorEl", "children", "container", "direction", "disablePortal", "keepMounted", "modifiers", "open", "placement", "popperOptions", "popperRef", "style", "transition", "slotProps", "slots"];
 
             function ez(e) {
                 return "function" == typeof e ? e() : e
             }
             let eW = () => (0, m.Z)({
                     root: ["root"]
@@ -1066,50 +1066,49 @@
                         anchorEl: r,
                         children: n,
                         component: a,
                         direction: i,
                         disablePortal: l,
                         modifiers: s,
                         open: c,
-                        ownerState: f,
-                        placement: m,
-                        popperOptions: h,
-                        popperRef: g,
-                        slotProps: v = {},
-                        slots: b = {},
-                        TransitionProps: y
-                    } = e, x = (0, p.Z)(e, ej), w = d.useRef(null), Z = (0, C.Z)(w, t), $ = d.useRef(null), O = (0, C.Z)($, g), S = d.useRef(O);
+                        placement: f,
+                        popperOptions: m,
+                        popperRef: h,
+                        slotProps: g = {},
+                        slots: v = {},
+                        TransitionProps: b
+                    } = e, y = (0, p.Z)(e, ej), x = d.useRef(null), w = (0, C.Z)(x, t), Z = d.useRef(null), $ = (0, C.Z)(Z, h), O = d.useRef($);
                     (0, k.Z)(() => {
-                        S.current = O
-                    }, [O]), d.useImperativeHandle(g, () => $.current, []);
-                    let P = function(e, t) {
+                        O.current = $
+                    }, [$]), d.useImperativeHandle(h, () => Z.current, []);
+                    let S = function(e, t) {
                             if ("ltr" === t) return e;
                             switch (e) {
                                 case "bottom-end":
                                     return "bottom-start";
                                 case "bottom-start":
                                     return "bottom-end";
                                 case "top-end":
                                     return "top-start";
                                 case "top-start":
                                     return "top-end";
                                 default:
                                     return e
                             }
-                        }(m, i),
-                        [I, R] = d.useState(P),
-                        [L, A] = d.useState(ez(r));
+                        }(f, i),
+                        [P, I] = d.useState(S),
+                        [R, L] = d.useState(ez(r));
                     d.useEffect(() => {
-                        $.current && $.current.forceUpdate()
+                        Z.current && Z.current.forceUpdate()
                     }), d.useEffect(() => {
-                        r && A(ez(r))
+                        r && L(ez(r))
                     }, [r]), (0, k.Z)(() => {
-                        if (!L || !c) return;
+                        if (!R || !c) return;
                         let e = e => {
-                                R(e.placement)
+                                I(e.placement)
                             },
                             t = [{
                                 name: "preventOverflow",
                                 options: {
                                     altBoundary: l
                                 }
                             }, {
@@ -1123,43 +1122,43 @@
                                 phase: "afterWrite",
                                 fn: ({
                                     state: t
                                 }) => {
                                     e(t)
                                 }
                             }];
-                        null != s && (t = t.concat(s)), h && null != h.modifiers && (t = t.concat(h.modifiers));
-                        let o = eI(L, w.current, (0, u.Z)({
-                            placement: P
-                        }, h, {
+                        null != s && (t = t.concat(s)), m && null != m.modifiers && (t = t.concat(m.modifiers));
+                        let o = eI(R, x.current, (0, u.Z)({
+                            placement: S
+                        }, m, {
                             modifiers: t
                         }));
-                        return S.current(o), () => {
-                            o.destroy(), S.current(null)
+                        return O.current(o), () => {
+                            o.destroy(), O.current(null)
                         }
-                    }, [L, l, s, c, h, P]);
-                    let D = {
-                        placement: I
+                    }, [R, l, s, c, m, S]);
+                    let A = {
+                        placement: P
                     };
-                    null !== y && (D.TransitionProps = y);
-                    let E = eW(),
-                        M = null != (o = null != a ? a : b.root) ? o : "div",
-                        T = (0, eE.Z)({
-                            elementType: M,
-                            externalSlotProps: v.root,
-                            externalForwardedProps: x,
+                    null !== b && (A.TransitionProps = b);
+                    let D = eW(),
+                        E = null != (o = null != a ? a : v.root) ? o : "div",
+                        M = (0, eE.Z)({
+                            elementType: E,
+                            externalSlotProps: g.root,
+                            externalForwardedProps: y,
                             additionalProps: {
                                 role: "tooltip",
-                                ref: Z
+                                ref: w
                             },
-                            ownerState: (0, u.Z)({}, e, f),
-                            className: E.root
+                            ownerState: e,
+                            className: D.root
                         });
-                    return (0, eT.jsx)(M, (0, u.Z)({}, T, {
-                        children: "function" == typeof n ? n(D) : n
+                    return (0, eT.jsx)(E, (0, u.Z)({}, M, {
+                        children: "function" == typeof n ? n(A) : n
                     }))
                 }),
                 eV = d.forwardRef(function(e, t) {
                     let o;
                     let {
                         anchorEl: r,
                         children: n,
```

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/826-b7f8eabaf3afc6d5.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/826-b7f8eabaf3afc6d5.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/framework-2c79e2a64abdb08b.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/framework-2c79e2a64abdb08b.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/main-4dcb7f9b52833aba.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/main-4dcb7f9b52833aba.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/pages/_app-d073359675509c25.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/pages/_app-3c2428351a583313.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,261 +1,69 @@
 (self.webpackChunk_N_E = self.webpackChunk_N_E || []).push([
     [888], {
-        8417: function(e, t, r) {
+        4697: function(e, t, r) {
             "use strict";
-            r.d(t, {
-                Z: function() {
-                    return L
-                }
-            });
-            var n = function() {
-                    function e(e) {
-                        var t = this;
-                        this._insertTag = function(e) {
-                            var r;
-                            r = 0 === t.tags.length ? t.insertionPoint ? t.insertionPoint.nextSibling : t.prepend ? t.container.firstChild : t.before : t.tags[t.tags.length - 1].nextSibling, t.container.insertBefore(e, r), t.tags.push(e)
-                        }, this.isSpeedy = void 0 === e.speedy || e.speedy, this.tags = [], this.ctr = 0, this.nonce = e.nonce, this.key = e.key, this.container = e.container, this.prepend = e.prepend, this.insertionPoint = e.insertionPoint, this.before = null
-                    }
-                    var t = e.prototype;
-                    return t.hydrate = function(e) {
-                        e.forEach(this._insertTag)
-                    }, t.insert = function(e) {
-                        if (this.ctr % (this.isSpeedy ? 65e3 : 1) == 0) {
-                            var t;
-                            this._insertTag(((t = document.createElement("style")).setAttribute("data-emotion", this.key), void 0 !== this.nonce && t.setAttribute("nonce", this.nonce), t.appendChild(document.createTextNode("")), t.setAttribute("data-s", ""), t))
-                        }
-                        var r = this.tags[this.tags.length - 1];
-                        if (this.isSpeedy) {
-                            var n = function(e) {
-                                if (e.sheet) return e.sheet;
-                                for (var t = 0; t < document.styleSheets.length; t++)
-                                    if (document.styleSheets[t].ownerNode === e) return document.styleSheets[t]
-                            }(r);
-                            try {
-                                n.insertRule(e, n.cssRules.length)
-                            } catch (e) {}
-                        } else r.appendChild(document.createTextNode(e));
-                        this.ctr++
-                    }, t.flush = function() {
-                        this.tags.forEach(function(e) {
-                            return e.parentNode && e.parentNode.removeChild(e)
-                        }), this.tags = [], this.ctr = 0
-                    }, e
-                }(),
-                o = Math.abs,
-                i = String.fromCharCode,
-                a = Object.assign;
-
-            function s(e, t, r) {
-                return e.replace(t, r)
-            }
-
-            function u(e, t) {
-                return e.indexOf(t)
-            }
-
-            function c(e, t) {
-                return 0 | e.charCodeAt(t)
-            }
-
-            function l(e, t, r) {
-                return e.slice(t, r)
-            }
-
-            function f(e) {
-                return e.length
-            }
-
-            function p(e, t) {
-                return t.push(e), e
-            }
-            var d = 1,
-                m = 1,
-                h = 0,
-                y = 0,
-                g = 0,
-                b = "";
-
-            function v(e, t, r, n, o, i, a) {
-                return {
-                    value: e,
-                    root: t,
-                    parent: r,
-                    type: n,
-                    props: o,
-                    children: i,
-                    line: d,
-                    column: m,
-                    length: a,
-                    return: ""
-                }
-            }
-
-            function x(e, t) {
-                return a(v("", null, null, "", null, null, 0), e, {
-                    length: -e.length
-                }, t)
-            }
-
-            function k() {
-                return g = y < h ? c(b, y++) : 0, m++, 10 === g && (m = 1, d++), g
-            }
-
-            function Z() {
-                return c(b, y)
-            }
-
-            function $(e) {
-                switch (e) {
-                    case 0:
-                    case 9:
-                    case 10:
-                    case 13:
-                    case 32:
-                        return 5;
-                    case 33:
-                    case 43:
-                    case 44:
-                    case 47:
-                    case 62:
-                    case 64:
-                    case 126:
-                    case 59:
-                    case 123:
-                    case 125:
-                        return 4;
-                    case 58:
-                        return 3;
-                    case 34:
-                    case 39:
-                    case 40:
-                    case 91:
-                        return 2;
-                    case 41:
-                    case 93:
-                        return 1
-                }
-                return 0
-            }
-
-            function w(e) {
-                return d = m = 1, h = f(b = e), y = 0, []
-            }
-
-            function S(e) {
-                var t, r;
-                return (t = y - 1, r = function e(t) {
-                    for (; k();) switch (g) {
-                        case t:
-                            return y;
-                        case 34:
-                        case 39:
-                            34 !== t && 39 !== t && e(g);
-                            break;
-                        case 40:
-                            41 === t && e(t);
-                            break;
-                        case 92:
-                            k()
-                    }
-                    return y
-                }(91 === e ? e + 2 : 40 === e ? e + 1 : e), l(b, t, r)).trim()
-            }
-            var O = "-ms-",
-                A = "-moz-",
-                C = "-webkit-",
-                P = "comm",
-                j = "rule",
-                E = "decl",
-                T = "@keyframes";
-
-            function _(e, t) {
-                for (var r = "", n = e.length, o = 0; o < n; o++) r += t(e[o], o, e, t) || "";
-                return r
-            }
-
-            function M(e, t, r, n) {
-                switch (e.type) {
-                    case "@import":
-                    case E:
-                        return e.return = e.return || e.value;
-                    case P:
-                        return "";
-                    case T:
-                        return e.return = e.value + "{" + _(e.children, n) + "}";
-                    case j:
-                        e.value = e.props.join(",")
-                }
-                return f(r = _(e.children, n)) ? e.return = e.value + "{" + r + "}" : ""
-            }
-
-            function R(e, t, r, n, i, a, u, c, f, p, d) {
-                for (var m = i - 1, h = 0 === i ? a : [""], y = h.length, g = 0, b = 0, x = 0; g < n; ++g)
-                    for (var k = 0, Z = l(e, m + 1, m = o(b = u[g])), $ = e; k < y; ++k)($ = (b > 0 ? h[k] + " " + Z : s(Z, /&\f/g, h[k])).trim()) && (f[x++] = $);
-                return v(e, t, r, 0 === i ? j : c, f, p, d)
-            }
-
-            function B(e, t, r, n) {
-                return v(e, t, r, E, l(e, 0, n), l(e, n + 1, -1), n)
-            }
-            var I = function(e, t, r) {
-                    for (var n = 0, o = 0; n = o, o = Z(), 38 === n && 12 === o && (t[r] = 1), !$(o);) k();
-                    return l(b, e, y)
+            var n = r(1526),
+                o = r(6411),
+                i = r(6686),
+                a = r(7563),
+                u = r(211),
+                s = r(8160),
+                c = r(2190),
+                l = function(e, t, r) {
+                    for (var n = 0, i = 0; n = i, i = (0, o.fj)(), 38 === n && 12 === i && (t[r] = 1), !(0, o.r)(i);)(0, o.lp)();
+                    return (0, o.tP)(e, o.FK)
                 },
-                z = function(e, t) {
+                f = function(e, t) {
                     var r = -1,
                         n = 44;
-                    do switch ($(n)) {
+                    do switch ((0, o.r)(n)) {
                         case 0:
-                            38 === n && 12 === Z() && (t[r] = 1), e[r] += I(y - 1, t, r);
+                            38 === n && 12 === (0, o.fj)() && (t[r] = 1), e[r] += l(o.FK - 1, t, r);
                             break;
                         case 2:
-                            e[r] += S(n);
+                            e[r] += (0, o.iF)(n);
                             break;
                         case 4:
                             if (44 === n) {
-                                e[++r] = 58 === Z() ? "&\f" : "", t[r] = e[r].length;
+                                e[++r] = 58 === (0, o.fj)() ? "&\f" : "", t[r] = e[r].length;
                                 break
                             }
                         default:
-                            e[r] += i(n)
+                            e[r] += (0, i.Dp)(n)
                     }
-                    while (n = k());
+                    while (n = (0, o.lp)());
                     return e
                 },
-                F = function(e, t) {
-                    var r;
-                    return r = z(w(e), t), b = "", r
-                },
-                K = new WeakMap,
-                W = function(e) {
+                p = new WeakMap,
+                d = function(e) {
                     if ("rule" === e.type && e.parent && !(e.length < 1)) {
                         for (var t = e.value, r = e.parent, n = e.column === r.column && e.line === r.line;
                             "rule" !== r.type;)
                             if (!(r = r.parent)) return;
-                        if ((1 !== e.props.length || 58 === t.charCodeAt(0) || K.get(r)) && !n) {
-                            K.set(e, !0);
-                            for (var o = [], i = F(t, o), a = r.props, s = 0, u = 0; s < i.length; s++)
-                                for (var c = 0; c < a.length; c++, u++) e.props[u] = o[s] ? i[s].replace(/&\f/g, a[c]) : a[c] + " " + i[s]
+                        if ((1 !== e.props.length || 58 === t.charCodeAt(0) || p.get(r)) && !n) {
+                            p.set(e, !0);
+                            for (var i = [], a = (0, o.cE)(f((0, o.un)(t), i)), u = r.props, s = 0, c = 0; s < a.length; s++)
+                                for (var l = 0; l < u.length; l++, c++) e.props[c] = i[s] ? a[s].replace(/&\f/g, u[l]) : u[l] + " " + a[s]
                         }
                     }
                 },
-                N = function(e) {
+                m = function(e) {
                     if ("decl" === e.type) {
                         var t = e.value;
                         108 === t.charCodeAt(0) && 98 === t.charCodeAt(2) && (e.return = "", e.value = "")
                     }
                 },
-                G = [function(e, t, r, n) {
+                h = [function(e, t, r, n) {
                     if (e.length > -1 && !e.return) switch (e.type) {
-                        case E:
+                        case a.h5:
                             e.return = function e(t, r) {
-                                switch (45 ^ c(t, 0) ? (((r << 2 ^ c(t, 0)) << 2 ^ c(t, 1)) << 2 ^ c(t, 2)) << 2 ^ c(t, 3) : 0) {
+                                switch ((0, i.vp)(t, r)) {
                                     case 5103:
-                                        return C + "print-" + t + t;
+                                        return a.G$ + "print-" + t + t;
                                     case 5737:
                                     case 4201:
                                     case 3177:
                                     case 3433:
                                     case 1641:
                                     case 4457:
                                     case 2921:
@@ -273,268 +81,161 @@
                                     case 4855:
                                     case 4215:
                                     case 6389:
                                     case 5109:
                                     case 5365:
                                     case 5621:
                                     case 3829:
-                                        return C + t + t;
+                                        return a.G$ + t + t;
                                     case 5349:
                                     case 4246:
                                     case 4810:
                                     case 6968:
                                     case 2756:
-                                        return C + t + A + t + O + t + t;
+                                        return a.G$ + t + a.uj + t + a.MS + t + t;
                                     case 6828:
                                     case 4268:
-                                        return C + t + O + t + t;
+                                        return a.G$ + t + a.MS + t + t;
                                     case 6165:
-                                        return C + t + O + "flex-" + t + t;
+                                        return a.G$ + t + a.MS + "flex-" + t + t;
                                     case 5187:
-                                        return C + t + s(t, /(\w+).+(:[^]+)/, C + "box-$1$2" + O + "flex-$1$2") + t;
+                                        return a.G$ + t + (0, i.gx)(t, /(\w+).+(:[^]+)/, a.G$ + "box-$1$2" + a.MS + "flex-$1$2") + t;
                                     case 5443:
-                                        return C + t + O + "flex-item-" + s(t, /flex-|-self/, "") + t;
+                                        return a.G$ + t + a.MS + "flex-item-" + (0, i.gx)(t, /flex-|-self/, "") + t;
                                     case 4675:
-                                        return C + t + O + "flex-line-pack" + s(t, /align-content|flex-|-self/, "") + t;
+                                        return a.G$ + t + a.MS + "flex-line-pack" + (0, i.gx)(t, /align-content|flex-|-self/, "") + t;
                                     case 5548:
-                                        return C + t + O + s(t, "shrink", "negative") + t;
+                                        return a.G$ + t + a.MS + (0, i.gx)(t, "shrink", "negative") + t;
                                     case 5292:
-                                        return C + t + O + s(t, "basis", "preferred-size") + t;
+                                        return a.G$ + t + a.MS + (0, i.gx)(t, "basis", "preferred-size") + t;
                                     case 6060:
-                                        return C + "box-" + s(t, "-grow", "") + C + t + O + s(t, "grow", "positive") + t;
+                                        return a.G$ + "box-" + (0, i.gx)(t, "-grow", "") + a.G$ + t + a.MS + (0, i.gx)(t, "grow", "positive") + t;
                                     case 4554:
-                                        return C + s(t, /([^-])(transform)/g, "$1" + C + "$2") + t;
+                                        return a.G$ + (0, i.gx)(t, /([^-])(transform)/g, "$1" + a.G$ + "$2") + t;
                                     case 6187:
-                                        return s(s(s(t, /(zoom-|grab)/, C + "$1"), /(image-set)/, C + "$1"), t, "") + t;
+                                        return (0, i.gx)((0, i.gx)((0, i.gx)(t, /(zoom-|grab)/, a.G$ + "$1"), /(image-set)/, a.G$ + "$1"), t, "") + t;
                                     case 5495:
                                     case 3959:
-                                        return s(t, /(image-set\([^]*)/, C + "$1$`$1");
+                                        return (0, i.gx)(t, /(image-set\([^]*)/, a.G$ + "$1$`$1");
                                     case 4968:
-                                        return s(s(t, /(.+:)(flex-)?(.*)/, C + "box-pack:$3" + O + "flex-pack:$3"), /s.+-b[^;]+/, "justify") + C + t + t;
+                                        return (0, i.gx)((0, i.gx)(t, /(.+:)(flex-)?(.*)/, a.G$ + "box-pack:$3" + a.MS + "flex-pack:$3"), /s.+-b[^;]+/, "justify") + a.G$ + t + t;
                                     case 4095:
                                     case 3583:
                                     case 4068:
                                     case 2532:
-                                        return s(t, /(.+)-inline(.+)/, C + "$1$2") + t;
+                                        return (0, i.gx)(t, /(.+)-inline(.+)/, a.G$ + "$1$2") + t;
                                     case 8116:
                                     case 7059:
                                     case 5753:
                                     case 5535:
                                     case 5445:
                                     case 5701:
                                     case 4933:
                                     case 4677:
                                     case 5533:
                                     case 5789:
                                     case 5021:
                                     case 4765:
-                                        if (f(t) - 1 - r > 6) switch (c(t, r + 1)) {
+                                        if ((0, i.to)(t) - 1 - r > 6) switch ((0, i.uO)(t, r + 1)) {
                                             case 109:
-                                                if (45 !== c(t, r + 4)) break;
+                                                if (45 !== (0, i.uO)(t, r + 4)) break;
                                             case 102:
-                                                return s(t, /(.+:)(.+)-([^]+)/, "$1" + C + "$2-$3$1" + A + (108 == c(t, r + 3) ? "$3" : "$2-$3")) + t;
+                                                return (0, i.gx)(t, /(.+:)(.+)-([^]+)/, "$1" + a.G$ + "$2-$3$1" + a.uj + (108 == (0, i.uO)(t, r + 3) ? "$3" : "$2-$3")) + t;
                                             case 115:
-                                                return ~u(t, "stretch") ? e(s(t, "stretch", "fill-available"), r) + t : t
+                                                return ~(0, i.Cw)(t, "stretch") ? e((0, i.gx)(t, "stretch", "fill-available"), r) + t : t
                                         }
                                         break;
                                     case 4949:
-                                        if (115 !== c(t, r + 1)) break;
+                                        if (115 !== (0, i.uO)(t, r + 1)) break;
                                     case 6444:
-                                        switch (c(t, f(t) - 3 - (~u(t, "!important") && 10))) {
+                                        switch ((0, i.uO)(t, (0, i.to)(t) - 3 - (~(0, i.Cw)(t, "!important") && 10))) {
                                             case 107:
-                                                return s(t, ":", ":" + C) + t;
+                                                return (0, i.gx)(t, ":", ":" + a.G$) + t;
                                             case 101:
-                                                return s(t, /(.+:)([^;!]+)(;|!.+)?/, "$1" + C + (45 === c(t, 14) ? "inline-" : "") + "box$3$1" + C + "$2$3$1" + O + "$2box$3") + t
+                                                return (0, i.gx)(t, /(.+:)([^;!]+)(;|!.+)?/, "$1" + a.G$ + (45 === (0, i.uO)(t, 14) ? "inline-" : "") + "box$3$1" + a.G$ + "$2$3$1" + a.MS + "$2box$3") + t
                                         }
                                         break;
                                     case 5936:
-                                        switch (c(t, r + 11)) {
+                                        switch ((0, i.uO)(t, r + 11)) {
                                             case 114:
-                                                return C + t + O + s(t, /[svh]\w+-[tblr]{2}/, "tb") + t;
+                                                return a.G$ + t + a.MS + (0, i.gx)(t, /[svh]\w+-[tblr]{2}/, "tb") + t;
                                             case 108:
-                                                return C + t + O + s(t, /[svh]\w+-[tblr]{2}/, "tb-rl") + t;
+                                                return a.G$ + t + a.MS + (0, i.gx)(t, /[svh]\w+-[tblr]{2}/, "tb-rl") + t;
                                             case 45:
-                                                return C + t + O + s(t, /[svh]\w+-[tblr]{2}/, "lr") + t
+                                                return a.G$ + t + a.MS + (0, i.gx)(t, /[svh]\w+-[tblr]{2}/, "lr") + t
                                         }
-                                        return C + t + O + t + t
+                                        return a.G$ + t + a.MS + t + t
                                 }
                                 return t
                             }(e.value, e.length);
                             break;
-                        case T:
-                            return _([x(e, {
-                                value: s(e.value, "@", "@" + C)
+                        case a.lK:
+                            return (0, u.q)([(0, o.JG)(e, {
+                                value: (0, i.gx)(e.value, "@", "@" + a.G$)
                             })], n);
-                        case j:
-                            if (e.length) return e.props.map(function(t) {
-                                var r;
-                                switch (r = t, (r = /(::plac\w+|:read-\w+)/.exec(r)) ? r[0] : r) {
+                        case a.Fr:
+                            if (e.length) return (0, i.$e)(e.props, function(t) {
+                                switch ((0, i.EQ)(t, /(::plac\w+|:read-\w+)/)) {
                                     case ":read-only":
                                     case ":read-write":
-                                        return _([x(e, {
-                                            props: [s(t, /:(read-\w+)/, ":" + A + "$1")]
+                                        return (0, u.q)([(0, o.JG)(e, {
+                                            props: [(0, i.gx)(t, /:(read-\w+)/, ":" + a.uj + "$1")]
                                         })], n);
                                     case "::placeholder":
-                                        return _([x(e, {
-                                            props: [s(t, /:(plac\w+)/, ":" + C + "input-$1")]
-                                        }), x(e, {
-                                            props: [s(t, /:(plac\w+)/, ":" + A + "$1")]
-                                        }), x(e, {
-                                            props: [s(t, /:(plac\w+)/, O + "input-$1")]
+                                        return (0, u.q)([(0, o.JG)(e, {
+                                            props: [(0, i.gx)(t, /:(plac\w+)/, ":" + a.G$ + "input-$1")]
+                                        }), (0, o.JG)(e, {
+                                            props: [(0, i.gx)(t, /:(plac\w+)/, ":" + a.uj + "$1")]
+                                        }), (0, o.JG)(e, {
+                                            props: [(0, i.gx)(t, /:(plac\w+)/, a.MS + "input-$1")]
                                         })], n)
                                 }
                                 return ""
-                            }).join("")
-                    }
-                }],
-                L = function(e) {
-                    var t, r, o, a, h, x = e.key;
-                    if ("css" === x) {
-                        var O = document.querySelectorAll("style[data-emotion]:not([data-s])");
-                        Array.prototype.forEach.call(O, function(e) {
-                            -1 !== e.getAttribute("data-emotion").indexOf(" ") && (document.head.appendChild(e), e.setAttribute("data-s", ""))
-                        })
+                            })
                     }
-                    var A = e.stylisPlugins || G,
-                        C = {},
-                        j = [];
-                    a = e.container || document.head, Array.prototype.forEach.call(document.querySelectorAll('style[data-emotion^="' + x + ' "]'), function(e) {
-                        for (var t = e.getAttribute("data-emotion").split(" "), r = 1; r < t.length; r++) C[t[r]] = !0;
-                        j.push(e)
-                    });
-                    var E = (r = (t = [W, N].concat(A, [M, (o = function(e) {
-                            h.insert(e)
-                        }, function(e) {
-                            !e.root && (e = e.return) && o(e)
-                        })])).length, function(e, n, o, i) {
-                            for (var a = "", s = 0; s < r; s++) a += t[s](e, n, o, i) || "";
-                            return a
-                        }),
-                        T = function(e) {
-                            var t, r;
-                            return _((r = function e(t, r, n, o, a, h, x, w, O) {
-                                for (var A, C = 0, j = 0, E = x, T = 0, _ = 0, M = 0, I = 1, z = 1, F = 1, K = 0, W = "", N = a, G = h, L = o, H = W; z;) switch (M = K, K = k()) {
-                                    case 40:
-                                        if (108 != M && 58 == c(H, E - 1)) {
-                                            -1 != u(H += s(S(K), "&", "&\f"), "&\f") && (F = -1);
-                                            break
-                                        }
-                                    case 34:
-                                    case 39:
-                                    case 91:
-                                        H += S(K);
-                                        break;
-                                    case 9:
-                                    case 10:
-                                    case 13:
-                                    case 32:
-                                        H += function(e) {
-                                            for (; g = Z();)
-                                                if (g < 33) k();
-                                                else break;
-                                            return $(e) > 2 || $(g) > 3 ? "" : " "
-                                        }(M);
-                                        break;
-                                    case 92:
-                                        H += function(e, t) {
-                                            for (var r; --t && k() && !(g < 48) && !(g > 102) && (!(g > 57) || !(g < 65)) && (!(g > 70) || !(g < 97)););
-                                            return r = y + (t < 6 && 32 == Z() && 32 == k()), l(b, e, r)
-                                        }(y - 1, 7);
-                                        continue;
-                                    case 47:
-                                        switch (Z()) {
-                                            case 42:
-                                            case 47:
-                                                p(v(A = function(e, t) {
-                                                    for (; k();)
-                                                        if (e + g === 57) break;
-                                                        else if (e + g === 84 && 47 === Z()) break;
-                                                    return "/*" + l(b, t, y - 1) + "*" + i(47 === e ? e : k())
-                                                }(k(), y), r, n, P, i(g), l(A, 2, -2), 0), O);
-                                                break;
-                                            default:
-                                                H += "/"
-                                        }
-                                        break;
-                                    case 123 * I:
-                                        w[C++] = f(H) * F;
-                                    case 125 * I:
-                                    case 59:
-                                    case 0:
-                                        switch (K) {
-                                            case 0:
-                                            case 125:
-                                                z = 0;
-                                            case 59 + j:
-                                                _ > 0 && f(H) - E && p(_ > 32 ? B(H + ";", o, n, E - 1) : B(s(H, " ", "") + ";", o, n, E - 2), O);
-                                                break;
-                                            case 59:
-                                                H += ";";
-                                            default:
-                                                if (p(L = R(H, r, n, C, j, a, w, W, N = [], G = [], E), h), 123 === K) {
-                                                    if (0 === j) e(H, r, L, L, N, h, E, w, G);
-                                                    else switch (99 === T && 110 === c(H, 3) ? 100 : T) {
-                                                        case 100:
-                                                        case 109:
-                                                        case 115:
-                                                            e(t, L, L, o && p(R(t, L, L, 0, 0, a, w, W, a, N = [], E), G), a, G, E, w, o ? N : G);
-                                                            break;
-                                                        default:
-                                                            e(H, L, L, L, [""], G, 0, w, G)
-                                                    }
-                                                }
-                                        }
-                                        C = j = _ = 0, I = F = 1, W = H = "", E = x;
-                                        break;
-                                    case 58:
-                                        E = 1 + f(H), _ = M;
-                                    default:
-                                        if (I < 1) {
-                                            if (123 == K) --I;
-                                            else if (125 == K && 0 == I++ && 125 == (g = y > 0 ? c(b, --y) : 0, m--, 10 === g && (m = 1, d--), g)) continue
-                                        }
-                                        switch (H += i(K), K * I) {
-                                            case 38:
-                                                F = j > 0 ? 1 : (H += "\f", -1);
-                                                break;
-                                            case 44:
-                                                w[C++] = (f(H) - 1) * F, F = 1;
-                                                break;
-                                            case 64:
-                                                45 === Z() && (H += S(k())), T = Z(), j = E = f(W = H += function(e) {
-                                                    for (; !$(Z());) k();
-                                                    return l(b, e, y)
-                                                }(y)), K++;
-                                                break;
-                                            case 45:
-                                                45 === M && 2 == f(H) && (I = 0)
-                                        }
-                                }
-                                return h
-                            }("", null, null, null, [""], t = w(t = e), 0, [0], t), b = "", r), E)
-                        },
-                        I = {
-                            key: x,
-                            sheet: new n({
-                                key: x,
-                                container: a,
-                                nonce: e.nonce,
-                                speedy: e.speedy,
-                                prepend: e.prepend,
-                                insertionPoint: e.insertionPoint
-                            }),
-                            nonce: e.nonce,
-                            inserted: C,
-                            registered: {},
-                            insert: function(e, t, r, n) {
-                                h = r, T(e ? e + "{" + t.styles + "}" : t.styles), n && (I.inserted[t.name] = !0)
-                            }
-                        };
-                    return I.sheet.hydrate(j), I
+                }];
+            t.Z = function(e) {
+                var t = e.key;
+                if ("css" === t) {
+                    var r = document.querySelectorAll("style[data-emotion]:not([data-s])");
+                    Array.prototype.forEach.call(r, function(e) {
+                        -1 !== e.getAttribute("data-emotion").indexOf(" ") && (document.head.appendChild(e), e.setAttribute("data-s", ""))
+                    })
                 }
+                var o = e.stylisPlugins || h,
+                    i = {},
+                    a = [];
+                l = e.container || document.head, Array.prototype.forEach.call(document.querySelectorAll('style[data-emotion^="' + t + ' "]'), function(e) {
+                    for (var t = e.getAttribute("data-emotion").split(" "), r = 1; r < t.length; r++) i[t[r]] = !0;
+                    a.push(e)
+                });
+                var l, f, p = [u.P, (0, s.cD)(function(e) {
+                        f.insert(e)
+                    })],
+                    g = (0, s.qR)([d, m].concat(o, p)),
+                    y = {
+                        key: t,
+                        sheet: new n.m({
+                            key: t,
+                            container: l,
+                            nonce: e.nonce,
+                            speedy: e.speedy,
+                            prepend: e.prepend,
+                            insertionPoint: e.insertionPoint
+                        }),
+                        nonce: e.nonce,
+                        inserted: i,
+                        registered: {},
+                        insert: function(e, t, r, n) {
+                            var o;
+                            f = r, o = e ? e + "{" + t.styles + "}" : t.styles, (0, u.q)((0, c.MY)(o), g), n && (y.inserted[t.name] = !0)
+                        }
+                    };
+                return y.sheet.hydrate(a), y
+            }
         },
         5042: function(e, t) {
             "use strict";
             t.Z = function(e) {
                 var t = Object.create(null);
                 return function(r) {
                     return void 0 === t[r] && (t[r] = e(r)), t[r]
@@ -544,85 +245,85 @@
         2443: function(e, t, r) {
             "use strict";
             r.d(t, {
                 C: function() {
                     return a
                 },
                 T: function() {
-                    return u
+                    return s
                 },
                 w: function() {
-                    return s
+                    return u
                 }
             });
             var n = r(7294),
-                o = r(8417);
+                o = r(4697);
             r(8137), r(7278);
             var i = (0, n.createContext)("undefined" != typeof HTMLElement ? (0, o.Z)({
                     key: "css"
                 }) : null),
                 a = i.Provider,
-                s = function(e) {
+                u = function(e) {
                     return (0, n.forwardRef)(function(t, r) {
                         return e(t, (0, n.useContext)(i), r)
                     })
                 },
-                u = (0, n.createContext)({})
+                s = (0, n.createContext)({})
         },
         917: function(e, t, r) {
             "use strict";
             r.d(t, {
                 F4: function() {
                     return l
                 },
                 iv: function() {
                     return c
                 },
                 xB: function() {
-                    return u
+                    return s
                 }
             });
             var n = r(7294);
-            r(8417);
+            r(4697);
             var o = r(2443);
             r(8679);
             var i = r(444),
                 a = r(8137),
-                s = r(7278),
-                u = (0, o.w)(function(e, t) {
+                u = r(7278),
+                s = (0, o.w)(function(e, t) {
                     var r = e.styles,
-                        u = (0, a.O)([r], void 0, (0, n.useContext)(o.T)),
+                        s = (0, a.O)([r], void 0, (0, n.useContext)(o.T)),
                         c = (0, n.useRef)();
-                    return (0, s.j)(function() {
+                    return (0, u.j)(function() {
                         var e = t.key + "-global",
                             r = new t.sheet.constructor({
                                 key: e,
                                 nonce: t.sheet.nonce,
                                 container: t.sheet.container,
                                 speedy: t.sheet.isSpeedy
                             }),
                             n = !1,
-                            o = document.querySelector('style[data-emotion="' + e + " " + u.name + '"]');
+                            o = document.querySelector('style[data-emotion="' + e + " " + s.name + '"]');
                         return t.sheet.tags.length && (r.before = t.sheet.tags[0]), null !== o && (n = !0, o.setAttribute("data-emotion", e), r.hydrate([o])), c.current = [r, n],
                             function() {
                                 r.flush()
                             }
-                    }, [t]), (0, s.j)(function() {
+                    }, [t]), (0, u.j)(function() {
                         var e = c.current,
                             r = e[0];
                         if (e[1]) {
                             e[1] = !1;
                             return
                         }
-                        if (void 0 !== u.next && (0, i.My)(t, u.next, !0), r.tags.length) {
+                        if (void 0 !== s.next && (0, i.My)(t, s.next, !0), r.tags.length) {
                             var n = r.tags[r.tags.length - 1].nextElementSibling;
                             r.before = n, r.flush()
                         }
-                        t.insert("", u, r, !1)
-                    }, [t, u.name]), null
+                        t.insert("", s, r, !1)
+                    }, [t, s.name]), null
                 });
 
             function c() {
                 for (var e = arguments.length, t = Array(e), r = 0; r < e; r++) t[r] = arguments[r];
                 return (0, a.O)(t)
             }
             var l = function() {
@@ -701,30 +402,30 @@
                     strokeDasharray: 1,
                     strokeDashoffset: 1,
                     strokeMiterlimit: 1,
                     strokeOpacity: 1,
                     strokeWidth: 1
                 },
                 a = r(5042),
-                s = /[A-Z]|^ms/g,
-                u = /_EMO_([^_]+?)_([^]*?)_EMO_/g,
+                u = /[A-Z]|^ms/g,
+                s = /_EMO_([^_]+?)_([^]*?)_EMO_/g,
                 c = function(e) {
                     return 45 === e.charCodeAt(1)
                 },
                 l = function(e) {
                     return null != e && "boolean" != typeof e
                 },
                 f = (0, a.Z)(function(e) {
-                    return c(e) ? e : e.replace(s, "-$&").toLowerCase()
+                    return c(e) ? e : e.replace(u, "-$&").toLowerCase()
                 }),
                 p = function(e, t) {
                     switch (e) {
                         case "animation":
                         case "animationName":
-                            if ("string" == typeof t) return t.replace(u, function(e, t, r) {
+                            if ("string" == typeof t) return t.replace(s, function(e, t, r) {
                                 return n = {
                                     name: t,
                                     styles: r,
                                     next: n
                                 }, t
                             })
                     }
@@ -758,74 +459,116 @@
                             if (Array.isArray(r))
                                 for (var o = 0; o < r.length; o++) n += d(e, t, r[o]) + ";";
                             else
                                 for (var i in r) {
                                     var a = r[i];
                                     if ("object" != typeof a) null != t && void 0 !== t[a] ? n += i + "{" + t[a] + "}" : l(a) && (n += f(i) + ":" + p(i, a) + ";");
                                     else if (Array.isArray(a) && "string" == typeof a[0] && (null == t || void 0 === t[a[0]]))
-                                        for (var s = 0; s < a.length; s++) l(a[s]) && (n += f(i) + ":" + p(i, a[s]) + ";");
+                                        for (var u = 0; u < a.length; u++) l(a[u]) && (n += f(i) + ":" + p(i, a[u]) + ";");
                                     else {
-                                        var u = d(e, t, a);
+                                        var s = d(e, t, a);
                                         switch (i) {
                                             case "animation":
                                             case "animationName":
-                                                n += f(i) + ":" + u + ";";
+                                                n += f(i) + ":" + s + ";";
                                                 break;
                                             default:
-                                                n += i + "{" + u + "}"
+                                                n += i + "{" + s + "}"
                                         }
                                     }
                                 }
                             return n
                         }(e, t, r);
                     case "function":
                         if (void 0 !== e) {
                             var i = n,
                                 a = r(e);
                             return n = i, d(e, t, a)
                         }
                 }
                 if (null == t) return r;
-                var s = t[r];
-                return void 0 !== s ? s : r
+                var u = t[r];
+                return void 0 !== u ? u : r
             }
             var m = /label:\s*([^\s;\n{]+)\s*(;|$)/g,
                 h = function(e, t, r) {
                     if (1 === e.length && "object" == typeof e[0] && null !== e[0] && void 0 !== e[0].styles) return e[0];
                     var i, a = !0,
-                        s = "";
+                        u = "";
                     n = void 0;
-                    var u = e[0];
-                    null == u || void 0 === u.raw ? (a = !1, s += d(r, t, u)) : s += u[0];
-                    for (var c = 1; c < e.length; c++) s += d(r, t, e[c]), a && (s += u[c]);
+                    var s = e[0];
+                    null == s || void 0 === s.raw ? (a = !1, u += d(r, t, s)) : u += s[0];
+                    for (var c = 1; c < e.length; c++) u += d(r, t, e[c]), a && (u += s[c]);
                     m.lastIndex = 0;
-                    for (var l = ""; null !== (i = m.exec(s));) l += "-" + i[1];
+                    for (var l = ""; null !== (i = m.exec(u));) l += "-" + i[1];
                     return {
-                        name: o(s) + l,
-                        styles: s,
+                        name: o(u) + l,
+                        styles: u,
                         next: n
                     }
                 }
         },
+        1526: function(e, t, r) {
+            "use strict";
+            r.d(t, {
+                m: function() {
+                    return n
+                }
+            });
+            var n = function() {
+                function e(e) {
+                    var t = this;
+                    this._insertTag = function(e) {
+                        var r;
+                        r = 0 === t.tags.length ? t.insertionPoint ? t.insertionPoint.nextSibling : t.prepend ? t.container.firstChild : t.before : t.tags[t.tags.length - 1].nextSibling, t.container.insertBefore(e, r), t.tags.push(e)
+                    }, this.isSpeedy = void 0 === e.speedy || e.speedy, this.tags = [], this.ctr = 0, this.nonce = e.nonce, this.key = e.key, this.container = e.container, this.prepend = e.prepend, this.insertionPoint = e.insertionPoint, this.before = null
+                }
+                var t = e.prototype;
+                return t.hydrate = function(e) {
+                    e.forEach(this._insertTag)
+                }, t.insert = function(e) {
+                    if (this.ctr % (this.isSpeedy ? 65e3 : 1) == 0) {
+                        var t;
+                        this._insertTag(((t = document.createElement("style")).setAttribute("data-emotion", this.key), void 0 !== this.nonce && t.setAttribute("nonce", this.nonce), t.appendChild(document.createTextNode("")), t.setAttribute("data-s", ""), t))
+                    }
+                    var r = this.tags[this.tags.length - 1];
+                    if (this.isSpeedy) {
+                        var n = function(e) {
+                            if (e.sheet) return e.sheet;
+                            for (var t = 0; t < document.styleSheets.length; t++)
+                                if (document.styleSheets[t].ownerNode === e) return document.styleSheets[t]
+                        }(r);
+                        try {
+                            n.insertRule(e, n.cssRules.length)
+                        } catch (e) {}
+                    } else r.appendChild(document.createTextNode(e));
+                    this.ctr++
+                }, t.flush = function() {
+                    this.tags.forEach(function(e) {
+                        return e.parentNode && e.parentNode.removeChild(e)
+                    }), this.tags = [], this.ctr = 0
+                }, e
+            }()
+        },
         7278: function(e, t, r) {
             "use strict";
             r.d(t, {
                 L: function() {
                     return a
                 },
                 j: function() {
-                    return s
+                    return u
                 }
             });
             var n, o = r(7294),
                 i = !!(n || (n = r.t(o, 2))).useInsertionEffect && (n || (n = r.t(o, 2))).useInsertionEffect,
                 a = i || function(e) {
                     return e()
                 },
-                s = i || o.useLayoutEffect
+                u = i || o.useLayoutEffect
         },
         444: function(e, t, r) {
             "use strict";
 
             function n(e, t, r) {
                 var n = "";
                 return r.split(" ").forEach(function(r) {
@@ -852,19 +595,19 @@
                     var n = e.key + "-" + t.name;
                     if (void 0 === e.inserted[t.name]) {
                         var i = t;
                         do e.insert(t === i ? "." + n : "", i, e.sheet, !0), i = i.next; while (void 0 !== i)
                     }
                 }
         },
-        2287: function(e, t, r) {
+        7297: function(e, t, r) {
             "use strict";
             r.d(t, {
                 Z: function() {
-                    return u
+                    return f
                 }
             });
             var n = r(7462);
             r(7294);
             var o = r(917),
                 i = r(5893);
 
@@ -873,18 +616,32 @@
                     styles: t,
                     defaultTheme: r = {}
                 } = e;
                 return (0, i.jsx)(o.xB, {
                     styles: "function" == typeof t ? e => t(null == e || 0 === Object.keys(e).length ? r : e) : t
                 })
             }
-            var s = r(247),
-                u = function(e) {
-                    return (0, i.jsx)(a, (0, n.Z)({}, e, {
-                        defaultTheme: s.Z
+            var u = r(6682),
+                s = function({
+                    styles: e,
+                    themeId: t,
+                    defaultTheme: r = {}
+                }) {
+                    let n = (0, u.Z)(r),
+                        o = "function" == typeof e ? e(t && n[t] || n) : e;
+                    return (0, i.jsx)(a, {
+                        styles: o
+                    })
+                },
+                c = r(247),
+                l = r(606),
+                f = function(e) {
+                    return (0, i.jsx)(s, (0, n.Z)({}, e, {
+                        defaultTheme: c.Z,
+                        themeId: l.Z
                     }))
                 }
         },
         7036: function(e, t) {
             "use strict";
             t.Z = {
                 50: "#fafafa",
@@ -910,16 +667,16 @@
                     return R
                 }
             });
             var n = r(7462),
                 o = r(3366),
                 i = r(1387),
                 a = r(9766),
-                s = r(6500),
-                u = r(4920),
+                u = r(6500),
+                s = r(4920),
                 c = r(6523),
                 l = r(1796),
                 f = {
                     black: "#000",
                     white: "#fff"
                 },
                 p = r(7036),
@@ -967,15 +724,15 @@
                     800: "#ef6c00",
                     900: "#e65100",
                     A100: "#ffd180",
                     A200: "#ffab40",
                     A400: "#ff9100",
                     A700: "#ff6d00"
                 },
-                y = {
+                g = {
                     50: "#e3f2fd",
                     100: "#bbdefb",
                     200: "#90caf9",
                     300: "#64b5f6",
                     400: "#42a5f5",
                     500: "#2196f3",
                     600: "#1e88e5",
@@ -983,15 +740,15 @@
                     800: "#1565c0",
                     900: "#0d47a1",
                     A100: "#82b1ff",
                     A200: "#448aff",
                     A400: "#2979ff",
                     A700: "#2962ff"
                 },
-                g = {
+                y = {
                     50: "#e1f5fe",
                     100: "#b3e5fc",
                     200: "#81d4fa",
                     300: "#4fc3f7",
                     400: "#29b6f6",
                     500: "#03a9f4",
                     600: "#039be5",
@@ -1041,15 +798,15 @@
                         disabledBackground: "rgba(0, 0, 0, 0.12)",
                         disabledOpacity: .38,
                         focus: "rgba(0, 0, 0, 0.12)",
                         focusOpacity: .12,
                         activatedOpacity: .12
                     }
                 },
-                k = {
+                $ = {
                     text: {
                         primary: f.white,
                         secondary: "rgba(255, 255, 255, 0.7)",
                         disabled: "rgba(255, 255, 255, 0.5)",
                         icon: "rgba(255, 255, 255, 0.5)"
                     },
                     divider: "rgba(255, 255, 255, 0.12)",
@@ -1068,119 +825,119 @@
                         disabledOpacity: .38,
                         focus: "rgba(255, 255, 255, 0.12)",
                         focusOpacity: .12,
                         activatedOpacity: .24
                     }
                 };
 
-            function Z(e, t, r, n) {
+            function k(e, t, r, n) {
                 let o = n.light || n,
                     i = n.dark || 1.5 * n;
                 e[t] || (e.hasOwnProperty(r) ? e[t] = e[r] : "light" === t ? e.light = (0, l.$n)(e.main, o) : "dark" === t && (e.dark = (0, l._j)(e.main, i)))
             }
-            let $ = ["fontFamily", "fontSize", "fontWeightLight", "fontWeightRegular", "fontWeightMedium", "fontWeightBold", "htmlFontSize", "allVariants", "pxToRem"],
-                w = {
+            let w = ["fontFamily", "fontSize", "fontWeightLight", "fontWeightRegular", "fontWeightMedium", "fontWeightBold", "htmlFontSize", "allVariants", "pxToRem"],
+                S = {
                     textTransform: "uppercase"
                 },
-                S = '"Roboto", "Helvetica", "Arial", sans-serif';
+                Z = '"Roboto", "Helvetica", "Arial", sans-serif';
 
             function O(...e) {
                 return `${e[0]}px ${e[1]}px ${e[2]}px ${e[3]}px rgba(0,0,0,0.2),${e[4]}px ${e[5]}px ${e[6]}px ${e[7]}px rgba(0,0,0,0.14),${e[8]}px ${e[9]}px ${e[10]}px ${e[11]}px rgba(0,0,0,0.12)`
             }
             let A = ["none", O(0, 2, 1, -1, 0, 1, 1, 0, 0, 1, 3, 0), O(0, 3, 1, -2, 0, 2, 2, 0, 0, 1, 5, 0), O(0, 3, 3, -2, 0, 3, 4, 0, 0, 1, 8, 0), O(0, 2, 4, -1, 0, 4, 5, 0, 0, 1, 10, 0), O(0, 3, 5, -1, 0, 5, 8, 0, 0, 1, 14, 0), O(0, 3, 5, -1, 0, 6, 10, 0, 0, 1, 18, 0), O(0, 4, 5, -2, 0, 7, 10, 1, 0, 2, 16, 1), O(0, 5, 5, -3, 0, 8, 10, 1, 0, 3, 14, 2), O(0, 5, 6, -3, 0, 9, 12, 1, 0, 3, 16, 2), O(0, 6, 6, -3, 0, 10, 14, 1, 0, 4, 18, 3), O(0, 6, 7, -4, 0, 11, 15, 1, 0, 4, 20, 3), O(0, 7, 8, -4, 0, 12, 17, 2, 0, 5, 22, 4), O(0, 7, 8, -4, 0, 13, 19, 2, 0, 5, 24, 4), O(0, 7, 9, -4, 0, 14, 21, 2, 0, 5, 26, 4), O(0, 8, 9, -5, 0, 15, 22, 2, 0, 6, 28, 5), O(0, 8, 10, -5, 0, 16, 24, 2, 0, 6, 30, 5), O(0, 8, 11, -5, 0, 17, 26, 2, 0, 6, 32, 5), O(0, 9, 11, -5, 0, 18, 28, 2, 0, 7, 34, 6), O(0, 9, 12, -6, 0, 19, 29, 2, 0, 7, 36, 6), O(0, 10, 13, -6, 0, 20, 31, 3, 0, 8, 38, 7), O(0, 10, 13, -6, 0, 21, 33, 3, 0, 8, 40, 7), O(0, 10, 14, -6, 0, 22, 35, 3, 0, 8, 42, 7), O(0, 11, 14, -7, 0, 23, 36, 3, 0, 9, 44, 8), O(0, 11, 15, -7, 0, 24, 38, 3, 0, 9, 46, 8)],
-                C = ["duration", "easing", "delay"],
-                P = {
+                j = ["duration", "easing", "delay"],
+                C = {
                     easeInOut: "cubic-bezier(0.4, 0, 0.2, 1)",
                     easeOut: "cubic-bezier(0.0, 0, 0.2, 1)",
                     easeIn: "cubic-bezier(0.4, 0, 1, 1)",
                     sharp: "cubic-bezier(0.4, 0, 0.6, 1)"
                 },
-                j = {
+                P = {
                     shortest: 150,
                     shorter: 200,
                     short: 250,
                     standard: 300,
                     complex: 375,
                     enteringScreen: 225,
                     leavingScreen: 195
                 };
 
-            function E(e) {
+            function G(e) {
                 return `${Math.round(e)}ms`
             }
 
-            function T(e) {
+            function M(e) {
                 if (!e) return 0;
                 let t = e / 36;
                 return Math.round((4 + 15 * t ** .25 + t / 5) * 10)
             }
-            var _ = {
+            var E = {
                 mobileStepper: 1e3,
                 fab: 1050,
                 speedDial: 1050,
                 appBar: 1100,
                 drawer: 1200,
                 modal: 1300,
                 snackbar: 1400,
                 tooltip: 1500
             };
-            let M = ["breakpoints", "mixins", "spacing", "palette", "transitions", "typography", "shape"];
+            let T = ["breakpoints", "mixins", "spacing", "palette", "transitions", "typography", "shape"];
             var R = function(e = {}, ...t) {
                 var r;
                 let {
                     mixins: O = {},
                     palette: R = {},
-                    transitions: B = {},
-                    typography: I = {}
-                } = e, z = (0, o.Z)(e, M);
+                    transitions: _ = {},
+                    typography: F = {}
+                } = e, K = (0, o.Z)(e, T);
                 if (e.vars) throw Error((0, i.Z)(18));
-                let F = function(e) {
+                let I = function(e) {
                         let {
                             mode: t = "light",
                             contrastThreshold: r = 3,
-                            tonalOffset: s = .2
-                        } = e, u = (0, o.Z)(e, v), c = e.primary || function(e = "light") {
+                            tonalOffset: u = .2
+                        } = e, s = (0, o.Z)(e, v), c = e.primary || function(e = "light") {
                             return "dark" === e ? {
-                                main: y[200],
-                                light: y[50],
-                                dark: y[400]
+                                main: g[200],
+                                light: g[50],
+                                dark: g[400]
                             } : {
-                                main: y[700],
-                                light: y[400],
-                                dark: y[800]
+                                main: g[700],
+                                light: g[400],
+                                dark: g[800]
                             }
-                        }(t), $ = e.secondary || function(e = "light") {
+                        }(t), w = e.secondary || function(e = "light") {
                             return "dark" === e ? {
                                 main: d[200],
                                 light: d[50],
                                 dark: d[400]
                             } : {
                                 main: d[500],
                                 light: d[300],
                                 dark: d[700]
                             }
-                        }(t), w = e.error || function(e = "light") {
+                        }(t), S = e.error || function(e = "light") {
                             return "dark" === e ? {
                                 main: m[500],
                                 light: m[300],
                                 dark: m[700]
                             } : {
                                 main: m[700],
                                 light: m[400],
                                 dark: m[800]
                             }
-                        }(t), S = e.info || function(e = "light") {
+                        }(t), Z = e.info || function(e = "light") {
                             return "dark" === e ? {
-                                main: g[400],
-                                light: g[300],
-                                dark: g[700]
+                                main: y[400],
+                                light: y[300],
+                                dark: y[700]
                             } : {
-                                main: g[700],
-                                light: g[500],
-                                dark: g[900]
+                                main: y[700],
+                                light: y[500],
+                                dark: y[900]
                             }
                         }(t), O = e.success || function(e = "light") {
                             return "dark" === e ? {
                                 main: b[400],
                                 light: b[300],
                                 dark: b[700]
                             } : {
@@ -1196,237 +953,222 @@
                             } : {
                                 main: "#ed6c02",
                                 light: h[500],
                                 dark: h[900]
                             }
                         }(t);
 
-                        function C(e) {
-                            let t = (0, l.mi)(e, k.text.primary) >= r ? k.text.primary : x.text.primary;
+                        function j(e) {
+                            let t = (0, l.mi)(e, $.text.primary) >= r ? $.text.primary : x.text.primary;
                             return t
                         }
-                        let P = ({
+                        let C = ({
                                 color: e,
                                 name: t,
                                 mainShade: r = 500,
                                 lightShade: o = 300,
                                 darkShade: a = 700
                             }) => {
                                 if (!(e = (0, n.Z)({}, e)).main && e[r] && (e.main = e[r]), !e.hasOwnProperty("main")) throw Error((0, i.Z)(11, t ? ` (${t})` : "", r));
                                 if ("string" != typeof e.main) throw Error((0, i.Z)(12, t ? ` (${t})` : "", JSON.stringify(e.main)));
-                                return Z(e, "light", o, s), Z(e, "dark", a, s), e.contrastText || (e.contrastText = C(e.main)), e
+                                return k(e, "light", o, u), k(e, "dark", a, u), e.contrastText || (e.contrastText = j(e.main)), e
                             },
-                            j = (0, a.Z)((0, n.Z)({
+                            P = (0, a.Z)((0, n.Z)({
                                 common: (0, n.Z)({}, f),
                                 mode: t,
-                                primary: P({
+                                primary: C({
                                     color: c,
                                     name: "primary"
                                 }),
-                                secondary: P({
-                                    color: $,
+                                secondary: C({
+                                    color: w,
                                     name: "secondary",
                                     mainShade: "A400",
                                     lightShade: "A200",
                                     darkShade: "A700"
                                 }),
-                                error: P({
-                                    color: w,
+                                error: C({
+                                    color: S,
                                     name: "error"
                                 }),
-                                warning: P({
+                                warning: C({
                                     color: A,
                                     name: "warning"
                                 }),
-                                info: P({
-                                    color: S,
+                                info: C({
+                                    color: Z,
                                     name: "info"
                                 }),
-                                success: P({
+                                success: C({
                                     color: O,
                                     name: "success"
                                 }),
                                 grey: p.Z,
                                 contrastThreshold: r,
-                                getContrastText: C,
-                                augmentColor: P,
-                                tonalOffset: s
+                                getContrastText: j,
+                                augmentColor: C,
+                                tonalOffset: u
                             }, {
-                                dark: k,
+                                dark: $,
                                 light: x
-                            } [t]), u);
-                        return j
+                            } [t]), s);
+                        return P
                     }(R),
-                    K = (0, s.Z)(e),
-                    W = (0, a.Z)(K, {
-                        mixins: (r = K.breakpoints, (0, n.Z)({
+                    z = (0, u.Z)(e),
+                    B = (0, a.Z)(z, {
+                        mixins: (r = z.breakpoints, (0, n.Z)({
                             toolbar: {
                                 minHeight: 56,
                                 [r.up("xs")]: {
                                     "@media (orientation: landscape)": {
                                         minHeight: 48
                                     }
                                 },
                                 [r.up("sm")]: {
                                     minHeight: 64
                                 }
                             }
                         }, O)),
-                        palette: F,
+                        palette: I,
                         shadows: A.slice(),
                         typography: function(e, t) {
                             let r = "function" == typeof t ? t(e) : t,
                                 {
-                                    fontFamily: i = S,
-                                    fontSize: s = 14,
-                                    fontWeightLight: u = 300,
+                                    fontFamily: i = Z,
+                                    fontSize: u = 14,
+                                    fontWeightLight: s = 300,
                                     fontWeightRegular: c = 400,
                                     fontWeightMedium: l = 500,
                                     fontWeightBold: f = 700,
                                     htmlFontSize: p = 16,
                                     allVariants: d,
                                     pxToRem: m
                                 } = r,
-                                h = (0, o.Z)(r, $),
-                                y = s / 14,
-                                g = m || (e => `${e/p*y}rem`),
+                                h = (0, o.Z)(r, w),
+                                g = u / 14,
+                                y = m || (e => `${e/p*g}rem`),
                                 b = (e, t, r, o, a) => (0, n.Z)({
                                     fontFamily: i,
                                     fontWeight: e,
-                                    fontSize: g(t),
+                                    fontSize: y(t),
                                     lineHeight: r
-                                }, i === S ? {
+                                }, i === Z ? {
                                     letterSpacing: `${Math.round(1e5*(o/t))/1e5}em`
                                 } : {}, a, d),
                                 v = {
-                                    h1: b(u, 96, 1.167, -1.5),
-                                    h2: b(u, 60, 1.2, -.5),
+                                    h1: b(s, 96, 1.167, -1.5),
+                                    h2: b(s, 60, 1.2, -.5),
                                     h3: b(c, 48, 1.167, 0),
                                     h4: b(c, 34, 1.235, .25),
                                     h5: b(c, 24, 1.334, 0),
                                     h6: b(l, 20, 1.6, .15),
                                     subtitle1: b(c, 16, 1.75, .15),
                                     subtitle2: b(l, 14, 1.57, .1),
                                     body1: b(c, 16, 1.5, .15),
                                     body2: b(c, 14, 1.43, .15),
-                                    button: b(l, 14, 1.75, .4, w),
+                                    button: b(l, 14, 1.75, .4, S),
                                     caption: b(c, 12, 1.66, .4),
-                                    overline: b(c, 12, 2.66, 1, w),
+                                    overline: b(c, 12, 2.66, 1, S),
                                     inherit: {
                                         fontFamily: "inherit",
                                         fontWeight: "inherit",
                                         fontSize: "inherit",
                                         lineHeight: "inherit",
                                         letterSpacing: "inherit"
                                     }
                                 };
                             return (0, a.Z)((0, n.Z)({
                                 htmlFontSize: p,
-                                pxToRem: g,
+                                pxToRem: y,
                                 fontFamily: i,
-                                fontSize: s,
-                                fontWeightLight: u,
+                                fontSize: u,
+                                fontWeightLight: s,
                                 fontWeightRegular: c,
                                 fontWeightMedium: l,
                                 fontWeightBold: f
                             }, v), h, {
                                 clone: !1
                             })
-                        }(F, I),
+                        }(I, F),
                         transitions: function(e) {
-                            let t = (0, n.Z)({}, P, e.easing),
-                                r = (0, n.Z)({}, j, e.duration),
+                            let t = (0, n.Z)({}, C, e.easing),
+                                r = (0, n.Z)({}, P, e.duration),
                                 i = (e = ["all"], n = {}) => {
                                     let {
                                         duration: i = r.standard,
                                         easing: a = t.easeInOut,
-                                        delay: s = 0
+                                        delay: u = 0
                                     } = n;
-                                    return (0, o.Z)(n, C), (Array.isArray(e) ? e : [e]).map(e => `${e} ${"string"==typeof i?i:E(i)} ${a} ${"string"==typeof s?s:E(s)}`).join(",")
+                                    return (0, o.Z)(n, j), (Array.isArray(e) ? e : [e]).map(e => `${e} ${"string"==typeof i?i:G(i)} ${a} ${"string"==typeof u?u:G(u)}`).join(",")
                                 };
                             return (0, n.Z)({
-                                getAutoHeightDuration: T,
+                                getAutoHeightDuration: M,
                                 create: i
                             }, e, {
                                 easing: t,
                                 duration: r
                             })
-                        }(B),
-                        zIndex: (0, n.Z)({}, _)
+                        }(_),
+                        zIndex: (0, n.Z)({}, E)
                     });
-                return W = (0, a.Z)(W, z), (W = t.reduce((e, t) => (0, a.Z)(e, t), W)).unstable_sxConfig = (0, n.Z)({}, u.Z, null == z ? void 0 : z.unstable_sxConfig), W.unstable_sx = function(e) {
+                return B = (0, a.Z)(B, K), (B = t.reduce((e, t) => (0, a.Z)(e, t), B)).unstable_sxConfig = (0, n.Z)({}, s.Z, null == K ? void 0 : K.unstable_sxConfig), B.unstable_sx = function(e) {
                     return (0, c.Z)({
                         sx: e,
                         theme: this
                     })
-                }, W
+                }, B
             }
         },
         247: function(e, t, r) {
             "use strict";
             var n = r(1919);
             let o = (0, n.Z)();
             t.Z = o
         },
+        606: function(e, t) {
+            "use strict";
+            t.Z = "$$material"
+        },
         1657: function(e, t, r) {
             "use strict";
             r.d(t, {
                 Z: function() {
-                    return i
+                    return a
                 }
             });
             var n = r(9628),
-                o = r(247);
+                o = r(247),
+                i = r(606);
 
-            function i({
+            function a({
                 props: e,
                 name: t
             }) {
                 return (0, n.Z)({
                     props: e,
                     name: t,
-                    defaultTheme: o.Z
+                    defaultTheme: o.Z,
+                    themeId: i.Z
                 })
             }
         },
-        4819: function(e, t, r) {
-            "use strict";
-            var n = r(7294);
-            let o = n.createContext(null);
-            t.Z = o
-        },
-        6760: function(e, t, r) {
-            "use strict";
-            r.d(t, {
-                Z: function() {
-                    return i
-                }
-            });
-            var n = r(7294),
-                o = r(4819);
-
-            function i() {
-                let e = n.useContext(o.Z);
-                return e
-            }
-        },
         5408: function(e, t, r) {
             "use strict";
             r.d(t, {
                 L7: function() {
-                    return u
+                    return s
                 },
                 P$: function() {
                     return l
                 },
                 VO: function() {
                     return o
                 },
                 W8: function() {
-                    return s
+                    return u
                 },
                 dt: function() {
                     return c
                 },
                 k9: function() {
                     return a
                 }
@@ -1460,35 +1202,35 @@
                         return n
                     }, {})
                 }
                 let a = r(t);
                 return a
             }
 
-            function s(e = {}) {
+            function u(e = {}) {
                 var t;
                 let r = null == (t = e.keys) ? void 0 : t.reduce((t, r) => {
                     let n = e.up(r);
                     return t[n] = {}, t
                 }, {});
                 return r || {}
             }
 
-            function u(e, t) {
+            function s(e, t) {
                 return e.reduce((e, t) => {
                     let r = e[t],
                         n = !r || 0 === Object.keys(r).length;
                     return n && delete e[t], e
                 }, t)
             }
 
             function c(e, ...t) {
-                let r = s(e),
+                let r = u(e),
                     o = [r, ...t].reduce((e, t) => (0, n.Z)(e, t), {});
-                return u(Object.keys(r), o)
+                return s(Object.keys(r), o)
             }
 
             function l({
                 values: e,
                 breakpoints: t,
                 base: r
             }) {
@@ -1516,15 +1258,15 @@
                 Fq: function() {
                     return c
                 },
                 _j: function() {
                     return l
                 },
                 mi: function() {
-                    return u
+                    return s
                 }
             });
             var n = r(1387);
 
             function o(e, t = 0, r = 1) {
                 return Math.min(Math.max(t, e), r)
             }
@@ -1558,31 +1300,31 @@
                     colorSpace: r
                 } = e, {
                     values: n
                 } = e;
                 return -1 !== t.indexOf("rgb") ? n = n.map((e, t) => t < 3 ? parseInt(e, 10) : e) : -1 !== t.indexOf("hsl") && (n[1] = `${n[1]}%`, n[2] = `${n[2]}%`), `${t}(${n=-1!==t.indexOf("color")?`${r} ${n.join(" ")}`:`${n.join(", ")}`})`
             }
 
-            function s(e) {
+            function u(e) {
                 let t = "hsl" === (e = i(e)).type || "hsla" === e.type ? i(function(e) {
                     e = i(e);
                     let {
                         values: t
-                    } = e, r = t[0], n = t[1] / 100, o = t[2] / 100, s = n * Math.min(o, 1 - o), u = (e, t = (e + r / 30) % 12) => o - s * Math.max(Math.min(t - 3, 9 - t, 1), -1), c = "rgb", l = [Math.round(255 * u(0)), Math.round(255 * u(8)), Math.round(255 * u(4))];
+                    } = e, r = t[0], n = t[1] / 100, o = t[2] / 100, u = n * Math.min(o, 1 - o), s = (e, t = (e + r / 30) % 12) => o - u * Math.max(Math.min(t - 3, 9 - t, 1), -1), c = "rgb", l = [Math.round(255 * s(0)), Math.round(255 * s(8)), Math.round(255 * s(4))];
                     return "hsla" === e.type && (c += "a", l.push(t[3])), a({
                         type: c,
                         values: l
                     })
                 }(e)).values : e.values;
                 return Number((.2126 * (t = t.map(t => ("color" !== e.type && (t /= 255), t <= .03928 ? t / 12.92 : ((t + .055) / 1.055) ** 2.4)))[0] + .7152 * t[1] + .0722 * t[2]).toFixed(3))
             }
 
-            function u(e, t) {
-                let r = s(e),
-                    n = s(t);
+            function s(e, t) {
+                let r = u(e),
+                    n = u(t);
                 return (Math.max(r, n) + .05) / (Math.min(r, n) + .05)
             }
 
             function c(e, t) {
                 return e = i(e), t = o(t), ("rgb" === e.type || "hsl" === e.type) && (e.type += "a"), "color" === e.type ? e.values[3] = `/${t}` : e.values[3] = t, a(e)
             }
 
@@ -1609,48 +1351,48 @@
                     return d
                 }
             });
             var n = r(7462),
                 o = r(3366),
                 i = r(9766);
             let a = ["values", "unit", "step"],
-                s = e => {
+                u = e => {
                     let t = Object.keys(e).map(t => ({
                         key: t,
                         val: e[t]
                     })) || [];
                     return t.sort((e, t) => e.val - t.val), t.reduce((e, t) => (0, n.Z)({}, e, {
                         [t.key]: t.val
                     }), {})
                 };
-            var u = {
+            var s = {
                     borderRadius: 4
                 },
                 c = r(8700),
                 l = r(6523),
                 f = r(4920);
             let p = ["breakpoints", "palette", "spacing", "shape"];
             var d = function(e = {}, ...t) {
                 let {
                     breakpoints: r = {},
                     palette: d = {},
                     spacing: m,
                     shape: h = {}
-                } = e, y = (0, o.Z)(e, p), g = function(e) {
+                } = e, g = (0, o.Z)(e, p), y = function(e) {
                     let {
                         values: t = {
                             xs: 0,
                             sm: 600,
                             md: 900,
                             lg: 1200,
                             xl: 1536
                         },
                         unit: r = "px",
                         step: i = 5
-                    } = e, u = (0, o.Z)(e, a), c = s(t), l = Object.keys(c);
+                    } = e, s = (0, o.Z)(e, a), c = u(t), l = Object.keys(c);
 
                     function f(e) {
                         let n = "number" == typeof t[e] ? t[e] : e;
                         return `@media (min-width:${n}${r})`
                     }
 
                     function p(e) {
@@ -1672,39 +1414,39 @@
                             return l.indexOf(e) + 1 < l.length ? d(e, l[l.indexOf(e) + 1]) : f(e)
                         },
                         not: function(e) {
                             let t = l.indexOf(e);
                             return 0 === t ? f(l[1]) : t === l.length - 1 ? p(l[t]) : d(e, l[l.indexOf(e) + 1]).replace("@media", "@media not all and")
                         },
                         unit: r
-                    }, u)
+                    }, s)
                 }(r), b = function(e = 8) {
                     if (e.mui) return e;
                     let t = (0, c.hB)({
                             spacing: e
                         }),
                         r = (...e) => {
                             let r = 0 === e.length ? [1] : e;
                             return r.map(e => {
                                 let r = t(e);
                                 return "number" == typeof r ? `${r}px` : r
                             }).join(" ")
                         };
                     return r.mui = !0, r
                 }(m), v = (0, i.Z)({
-                    breakpoints: g,
+                    breakpoints: y,
                     direction: "ltr",
                     components: {},
                     palette: (0, n.Z)({
                         mode: "light"
                     }, d),
                     spacing: b,
-                    shape: (0, n.Z)({}, u, h)
-                }, y);
-                return (v = t.reduce((e, t) => (0, i.Z)(e, t), v)).unstable_sxConfig = (0, n.Z)({}, f.Z, null == y ? void 0 : y.unstable_sxConfig), v.unstable_sx = function(e) {
+                    shape: (0, n.Z)({}, s, h)
+                }, g);
+                return (v = t.reduce((e, t) => (0, i.Z)(e, t), v)).unstable_sxConfig = (0, n.Z)({}, f.Z, null == g ? void 0 : g.unstable_sxConfig), v.unstable_sx = function(e) {
                     return (0, l.Z)({
                         sx: e,
                         theme: this
                     })
                 }, v
             }
         },
@@ -1726,50 +1468,50 @@
                 eI: function() {
                     return d
                 },
                 NA: function() {
                     return h
                 },
                 e6: function() {
-                    return g
+                    return y
                 },
                 o3: function() {
                     return b
                 }
             });
             var n = r(5408),
                 o = r(4844),
                 i = r(7730);
             let a = {
                     m: "margin",
                     p: "padding"
                 },
-                s = {
+                u = {
                     t: "Top",
                     r: "Right",
                     b: "Bottom",
                     l: "Left",
                     x: ["Left", "Right"],
                     y: ["Top", "Bottom"]
                 },
-                u = {
+                s = {
                     marginX: "mx",
                     marginY: "my",
                     paddingX: "px",
                     paddingY: "py"
                 },
                 c = function(e) {
                     let t = {};
                     return r => (void 0 === t[r] && (t[r] = e(r)), t[r])
                 }(e => {
                     if (e.length > 2) {
-                        if (!u[e]) return [e];
-                        e = u[e]
+                        if (!s[e]) return [e];
+                        e = s[e]
                     }
-                    let [t, r] = e.split(""), n = a[t], o = s[r] || "";
+                    let [t, r] = e.split(""), n = a[t], o = u[r] || "";
                     return Array.isArray(o) ? o.map(e => n + e) : [n + o]
                 }),
                 l = ["m", "mt", "mr", "mb", "ml", "mx", "my", "margin", "marginTop", "marginRight", "marginBottom", "marginLeft", "marginX", "marginY", "marginInline", "marginInlineStart", "marginInlineEnd", "marginBlock", "marginBlockStart", "marginBlockEnd"],
                 f = ["p", "pt", "pr", "pb", "pl", "px", "py", "padding", "paddingTop", "paddingRight", "paddingBottom", "paddingLeft", "paddingX", "paddingY", "paddingInline", "paddingInlineStart", "paddingInlineEnd", "paddingBlock", "paddingBlockStart", "paddingBlockEnd"],
                 p = [...l, ...f];
 
             function d(e, t, r, n) {
@@ -1784,37 +1526,37 @@
 
             function h(e, t) {
                 if ("string" == typeof t || null == t) return t;
                 let r = e(Math.abs(t));
                 return t >= 0 ? r : "number" == typeof r ? -r : `-${r}`
             }
 
-            function y(e, t) {
+            function g(e, t) {
                 let r = m(e.theme);
                 return Object.keys(e).map(o => (function(e, t, r, o) {
                     if (-1 === t.indexOf(r)) return null;
                     let i = c(r),
                         a = e => i.reduce((t, r) => (t[r] = h(o, e), t), {}),
-                        s = e[r];
-                    return (0, n.k9)(e, s, a)
+                        u = e[r];
+                    return (0, n.k9)(e, u, a)
                 })(e, t, o, r)).reduce(i.Z, {})
             }
 
-            function g(e) {
-                return y(e, l)
+            function y(e) {
+                return g(e, l)
             }
 
             function b(e) {
-                return y(e, f)
+                return g(e, f)
             }
 
             function v(e) {
-                return y(e, p)
+                return g(e, p)
             }
-            g.propTypes = {}, g.filterProps = l, b.propTypes = {}, b.filterProps = f, v.propTypes = {}, v.filterProps = p
+            y.propTypes = {}, y.filterProps = l, b.propTypes = {}, b.filterProps = f, v.propTypes = {}, v.filterProps = p
         },
         4844: function(e, t, r) {
             "use strict";
             r.d(t, {
                 DW: function() {
                     return i
                 },
@@ -1838,263 +1580,263 @@
                 let o;
                 return o = "function" == typeof e ? e(r) : Array.isArray(e) ? e[r] || n : i(e, r) || n, t && (o = t(o, n, e)), o
             }
             t.ZP = function(e) {
                 let {
                     prop: t,
                     cssProperty: r = e.prop,
-                    themeKey: s,
-                    transform: u
+                    themeKey: u,
+                    transform: s
                 } = e, c = e => {
                     if (null == e[t]) return null;
                     let c = e[t],
                         l = e.theme,
-                        f = i(l, s) || {},
+                        f = i(l, u) || {},
                         p = e => {
-                            let o = a(f, u, e);
-                            return (e === o && "string" == typeof e && (o = a(f, u, `${t}${"default"===e?"":(0,n.Z)(e)}`, e)), !1 === r) ? o : {
+                            let o = a(f, s, e);
+                            return (e === o && "string" == typeof e && (o = a(f, s, `${t}${"default"===e?"":(0,n.Z)(e)}`, e)), !1 === r) ? o : {
                                 [r]: o
                             }
                         };
                     return (0, o.k9)(e, c, p)
                 };
                 return c.propTypes = {}, c.filterProps = [t], c
             }
         },
         4920: function(e, t, r) {
             "use strict";
             r.d(t, {
                 Z: function() {
-                    return H
+                    return D
                 }
             });
             var n = r(8700),
                 o = r(4844),
                 i = r(7730),
                 a = function(...e) {
                     let t = e.reduce((e, t) => (t.filterProps.forEach(r => {
                             e[r] = t
                         }), e), {}),
                         r = e => Object.keys(e).reduce((r, n) => t[n] ? (0, i.Z)(r, t[n](e)) : r, {});
                     return r.propTypes = {}, r.filterProps = e.reduce((e, t) => e.concat(t.filterProps), []), r
                 },
-                s = r(5408);
+                u = r(5408);
 
-            function u(e) {
+            function s(e) {
                 return "number" != typeof e ? e : `${e}px solid`
             }
             let c = (0, o.ZP)({
                     prop: "border",
                     themeKey: "borders",
-                    transform: u
+                    transform: s
                 }),
                 l = (0, o.ZP)({
                     prop: "borderTop",
                     themeKey: "borders",
-                    transform: u
+                    transform: s
                 }),
                 f = (0, o.ZP)({
                     prop: "borderRight",
                     themeKey: "borders",
-                    transform: u
+                    transform: s
                 }),
                 p = (0, o.ZP)({
                     prop: "borderBottom",
                     themeKey: "borders",
-                    transform: u
+                    transform: s
                 }),
                 d = (0, o.ZP)({
                     prop: "borderLeft",
                     themeKey: "borders",
-                    transform: u
+                    transform: s
                 }),
                 m = (0, o.ZP)({
                     prop: "borderColor",
                     themeKey: "palette"
                 }),
                 h = (0, o.ZP)({
                     prop: "borderTopColor",
                     themeKey: "palette"
                 }),
-                y = (0, o.ZP)({
+                g = (0, o.ZP)({
                     prop: "borderRightColor",
                     themeKey: "palette"
                 }),
-                g = (0, o.ZP)({
+                y = (0, o.ZP)({
                     prop: "borderBottomColor",
                     themeKey: "palette"
                 }),
                 b = (0, o.ZP)({
                     prop: "borderLeftColor",
                     themeKey: "palette"
                 }),
                 v = e => {
                     if (void 0 !== e.borderRadius && null !== e.borderRadius) {
                         let t = (0, n.eI)(e.theme, "shape.borderRadius", 4, "borderRadius"),
                             r = e => ({
                                 borderRadius: (0, n.NA)(t, e)
                             });
-                        return (0, s.k9)(e, e.borderRadius, r)
+                        return (0, u.k9)(e, e.borderRadius, r)
                     }
                     return null
                 };
-            v.propTypes = {}, v.filterProps = ["borderRadius"], a(c, l, f, p, d, m, h, y, g, b, v);
+            v.propTypes = {}, v.filterProps = ["borderRadius"], a(c, l, f, p, d, m, h, g, y, b, v);
             let x = e => {
                 if (void 0 !== e.gap && null !== e.gap) {
                     let t = (0, n.eI)(e.theme, "spacing", 8, "gap"),
                         r = e => ({
                             gap: (0, n.NA)(t, e)
                         });
-                    return (0, s.k9)(e, e.gap, r)
+                    return (0, u.k9)(e, e.gap, r)
                 }
                 return null
             };
             x.propTypes = {}, x.filterProps = ["gap"];
-            let k = e => {
+            let $ = e => {
                 if (void 0 !== e.columnGap && null !== e.columnGap) {
                     let t = (0, n.eI)(e.theme, "spacing", 8, "columnGap"),
                         r = e => ({
                             columnGap: (0, n.NA)(t, e)
                         });
-                    return (0, s.k9)(e, e.columnGap, r)
+                    return (0, u.k9)(e, e.columnGap, r)
                 }
                 return null
             };
-            k.propTypes = {}, k.filterProps = ["columnGap"];
-            let Z = e => {
+            $.propTypes = {}, $.filterProps = ["columnGap"];
+            let k = e => {
                 if (void 0 !== e.rowGap && null !== e.rowGap) {
                     let t = (0, n.eI)(e.theme, "spacing", 8, "rowGap"),
                         r = e => ({
                             rowGap: (0, n.NA)(t, e)
                         });
-                    return (0, s.k9)(e, e.rowGap, r)
+                    return (0, u.k9)(e, e.rowGap, r)
                 }
                 return null
             };
-            Z.propTypes = {}, Z.filterProps = ["rowGap"];
-            let $ = (0, o.ZP)({
+            k.propTypes = {}, k.filterProps = ["rowGap"];
+            let w = (0, o.ZP)({
                     prop: "gridColumn"
                 }),
-                w = (0, o.ZP)({
+                S = (0, o.ZP)({
                     prop: "gridRow"
                 }),
-                S = (0, o.ZP)({
+                Z = (0, o.ZP)({
                     prop: "gridAutoFlow"
                 }),
                 O = (0, o.ZP)({
                     prop: "gridAutoColumns"
                 }),
                 A = (0, o.ZP)({
                     prop: "gridAutoRows"
                 }),
-                C = (0, o.ZP)({
+                j = (0, o.ZP)({
                     prop: "gridTemplateColumns"
                 }),
-                P = (0, o.ZP)({
+                C = (0, o.ZP)({
                     prop: "gridTemplateRows"
                 }),
-                j = (0, o.ZP)({
+                P = (0, o.ZP)({
                     prop: "gridTemplateAreas"
                 }),
-                E = (0, o.ZP)({
+                G = (0, o.ZP)({
                     prop: "gridArea"
                 });
 
-            function T(e, t) {
+            function M(e, t) {
                 return "grey" === t ? t : e
             }
-            a(x, k, Z, $, w, S, O, A, C, P, j, E);
-            let _ = (0, o.ZP)({
+            a(x, $, k, w, S, Z, O, A, j, C, P, G);
+            let E = (0, o.ZP)({
                     prop: "color",
                     themeKey: "palette",
-                    transform: T
+                    transform: M
                 }),
-                M = (0, o.ZP)({
+                T = (0, o.ZP)({
                     prop: "bgcolor",
                     cssProperty: "backgroundColor",
                     themeKey: "palette",
-                    transform: T
+                    transform: M
                 }),
                 R = (0, o.ZP)({
                     prop: "backgroundColor",
                     themeKey: "palette",
-                    transform: T
+                    transform: M
                 });
 
-            function B(e) {
+            function _(e) {
                 return e <= 1 && 0 !== e ? `${100*e}%` : e
             }
-            a(_, M, R);
-            let I = (0, o.ZP)({
+            a(E, T, R);
+            let F = (0, o.ZP)({
                     prop: "width",
-                    transform: B
+                    transform: _
                 }),
-                z = e => {
+                K = e => {
                     if (void 0 !== e.maxWidth && null !== e.maxWidth) {
                         let t = t => {
                             var r, n, o;
-                            let i = (null == (r = e.theme) ? void 0 : null == (n = r.breakpoints) ? void 0 : null == (o = n.values) ? void 0 : o[t]) || s.VO[t];
+                            let i = (null == (r = e.theme) ? void 0 : null == (n = r.breakpoints) ? void 0 : null == (o = n.values) ? void 0 : o[t]) || u.VO[t];
                             return {
-                                maxWidth: i || B(t)
+                                maxWidth: i || _(t)
                             }
                         };
-                        return (0, s.k9)(e, e.maxWidth, t)
+                        return (0, u.k9)(e, e.maxWidth, t)
                     }
                     return null
                 };
-            z.filterProps = ["maxWidth"];
-            let F = (0, o.ZP)({
+            K.filterProps = ["maxWidth"];
+            let I = (0, o.ZP)({
                     prop: "minWidth",
-                    transform: B
+                    transform: _
                 }),
-                K = (0, o.ZP)({
+                z = (0, o.ZP)({
                     prop: "height",
-                    transform: B
+                    transform: _
                 }),
-                W = (0, o.ZP)({
+                B = (0, o.ZP)({
                     prop: "maxHeight",
-                    transform: B
+                    transform: _
                 }),
-                N = (0, o.ZP)({
+                W = (0, o.ZP)({
                     prop: "minHeight",
-                    transform: B
+                    transform: _
                 });
             (0, o.ZP)({
                 prop: "size",
                 cssProperty: "width",
-                transform: B
+                transform: _
             }), (0, o.ZP)({
                 prop: "size",
                 cssProperty: "height",
-                transform: B
+                transform: _
             });
-            let G = (0, o.ZP)({
+            let q = (0, o.ZP)({
                 prop: "boxSizing"
             });
-            a(I, z, F, K, W, N, G);
-            let L = {
+            a(F, K, I, z, B, W, q);
+            let N = {
                 border: {
                     themeKey: "borders",
-                    transform: u
+                    transform: s
                 },
                 borderTop: {
                     themeKey: "borders",
-                    transform: u
+                    transform: s
                 },
                 borderRight: {
                     themeKey: "borders",
-                    transform: u
+                    transform: s
                 },
                 borderBottom: {
                     themeKey: "borders",
-                    transform: u
+                    transform: s
                 },
                 borderLeft: {
                     themeKey: "borders",
-                    transform: u
+                    transform: s
                 },
                 borderColor: {
                     themeKey: "palette"
                 },
                 borderTopColor: {
                     themeKey: "palette"
                 },
@@ -2109,24 +1851,24 @@
                 },
                 borderRadius: {
                     themeKey: "shape.borderRadius",
                     style: v
                 },
                 color: {
                     themeKey: "palette",
-                    transform: T
+                    transform: M
                 },
                 bgcolor: {
                     themeKey: "palette",
                     cssProperty: "backgroundColor",
-                    transform: T
+                    transform: M
                 },
                 backgroundColor: {
                     themeKey: "palette",
-                    transform: T
+                    transform: M
                 },
                 p: {
                     style: n.o3
                 },
                 pt: {
                     style: n.o3
                 },
@@ -2270,18 +2012,18 @@
                 alignSelf: {},
                 justifyItems: {},
                 justifySelf: {},
                 gap: {
                     style: x
                 },
                 rowGap: {
-                    style: Z
+                    style: k
                 },
                 columnGap: {
-                    style: k
+                    style: $
                 },
                 gridColumn: {},
                 gridRow: {},
                 gridAutoFlow: {},
                 gridAutoColumns: {},
                 gridAutoRows: {},
                 gridTemplateColumns: {},
@@ -2296,30 +2038,30 @@
                 right: {},
                 bottom: {},
                 left: {},
                 boxShadow: {
                     themeKey: "shadows"
                 },
                 width: {
-                    transform: B
+                    transform: _
                 },
                 maxWidth: {
-                    style: z
+                    style: K
                 },
                 minWidth: {
-                    transform: B
+                    transform: _
                 },
                 height: {
-                    transform: B
+                    transform: _
                 },
                 maxHeight: {
-                    transform: B
+                    transform: _
                 },
                 minHeight: {
-                    transform: B
+                    transform: _
                 },
                 boxSizing: {},
                 fontFamily: {
                     themeKey: "typography"
                 },
                 fontSize: {
                     themeKey: "typography"
@@ -2335,99 +2077,99 @@
                 lineHeight: {},
                 textAlign: {},
                 typography: {
                     cssProperty: !1,
                     themeKey: "typography"
                 }
             };
-            var H = L
+            var D = N
         },
         6523: function(e, t, r) {
             "use strict";
             var n = r(8320),
                 o = r(7730),
                 i = r(4844),
                 a = r(5408),
-                s = r(4920);
-            let u = function() {
+                u = r(4920);
+            let s = function() {
                 function e(e, t, r, o) {
-                    let s = {
+                    let u = {
                             [e]: t,
                             theme: r
                         },
-                        u = o[e];
-                    if (!u) return {
+                        s = o[e];
+                    if (!s) return {
                         [e]: t
                     };
                     let {
                         cssProperty: c = e,
                         themeKey: l,
                         transform: f,
                         style: p
-                    } = u;
+                    } = s;
                     if (null == t) return null;
                     if ("typography" === l && "inherit" === t) return {
                         [e]: t
                     };
                     let d = (0, i.DW)(r, l) || {};
-                    if (p) return p(s);
+                    if (p) return p(u);
                     let m = t => {
                         let r = (0, i.Jq)(d, f, t);
                         return (t === r && "string" == typeof t && (r = (0, i.Jq)(d, f, `${e}${"default"===t?"":(0,n.Z)(t)}`, t)), !1 === c) ? r : {
                             [c]: r
                         }
                     };
-                    return (0, a.k9)(s, t, m)
+                    return (0, a.k9)(u, t, m)
                 }
                 return function t(r) {
                     var n;
                     let {
                         sx: i,
-                        theme: u = {}
+                        theme: s = {}
                     } = r || {};
                     if (!i) return null;
-                    let c = null != (n = u.unstable_sxConfig) ? n : s.Z;
+                    let c = null != (n = s.unstable_sxConfig) ? n : u.Z;
 
                     function l(r) {
                         let n = r;
-                        if ("function" == typeof r) n = r(u);
+                        if ("function" == typeof r) n = r(s);
                         else if ("object" != typeof r) return r;
                         if (!n) return null;
-                        let i = (0, a.W8)(u.breakpoints),
-                            s = Object.keys(i),
+                        let i = (0, a.W8)(s.breakpoints),
+                            u = Object.keys(i),
                             l = i;
                         return Object.keys(n).forEach(r => {
                             var i;
-                            let s = "function" == typeof(i = n[r]) ? i(u) : i;
-                            if (null != s) {
-                                if ("object" == typeof s) {
-                                    if (c[r]) l = (0, o.Z)(l, e(r, s, u, c));
+                            let u = "function" == typeof(i = n[r]) ? i(s) : i;
+                            if (null != u) {
+                                if ("object" == typeof u) {
+                                    if (c[r]) l = (0, o.Z)(l, e(r, u, s, c));
                                     else {
                                         let e = (0, a.k9)({
-                                            theme: u
-                                        }, s, e => ({
+                                            theme: s
+                                        }, u, e => ({
                                             [r]: e
                                         }));
                                         (function(...e) {
                                             let t = e.reduce((e, t) => e.concat(Object.keys(t)), []),
                                                 r = new Set(t);
                                             return e.every(e => r.size === Object.keys(e).length)
-                                        })(e, s) ? l[r] = t({
-                                            sx: s,
-                                            theme: u
+                                        })(e, u) ? l[r] = t({
+                                            sx: u,
+                                            theme: s
                                         }): l = (0, o.Z)(l, e)
                                     }
-                                } else l = (0, o.Z)(l, e(r, s, u, c))
+                                } else l = (0, o.Z)(l, e(r, u, s, c))
                             }
-                        }), (0, a.L7)(s, l)
+                        }), (0, a.L7)(u, l)
                     }
                     return Array.isArray(i) ? i.map(l) : l(i)
                 }
             }();
-            u.filterProps = ["sx"], t.Z = u
+            s.filterProps = ["sx"], t.Z = s
         },
         6682: function(e, t, r) {
             "use strict";
             var n = r(6500),
                 o = r(4168);
             let i = (0, n.Z)();
             t.Z = function(e = i) {
@@ -2461,30 +2203,33 @@
             });
             var n = r(539),
                 o = r(6682);
 
             function i({
                 props: e,
                 name: t,
-                defaultTheme: r
+                defaultTheme: r,
+                themeId: i
             }) {
-                let i = (0, o.Z)(r),
-                    a = (0, n.Z)({
-                        theme: i,
-                        name: t,
-                        props: e
-                    });
-                return a
+                let a = (0, o.Z)(r);
+                i && (a = a[i] || a);
+                let u = (0, n.Z)({
+                    theme: a,
+                    name: t,
+                    props: e
+                });
+                return u
             }
         },
         4168: function(e, t, r) {
             "use strict";
-            var n = r(6760);
+            var n = r(7294),
+                o = r(2443);
             t.Z = function(e = null) {
-                let t = (0, n.Z)();
+                let t = n.useContext(o.T);
                 return t && 0 !== Object.keys(t).length ? t : e
             }
         },
         8320: function(e, t, r) {
             "use strict";
             r.d(t, {
                 Z: function() {
@@ -2547,18 +2292,18 @@
                 Z: function() {
                     return function e(t, r) {
                         let o = (0, n.Z)({}, r);
                         return Object.keys(t).forEach(i => {
                             if (i.toString().match(/^(components|slots)$/)) o[i] = (0, n.Z)({}, t[i], o[i]);
                             else if (i.toString().match(/^(componentsProps|slotProps)$/)) {
                                 let a = t[i] || {},
-                                    s = r[i];
-                                o[i] = {}, s && Object.keys(s) ? a && Object.keys(a) ? (o[i] = (0, n.Z)({}, s), Object.keys(a).forEach(t => {
-                                    o[i][t] = e(a[t], s[t])
-                                })) : o[i] = s : o[i] = a
+                                    u = r[i];
+                                o[i] = {}, u && Object.keys(u) ? a && Object.keys(a) ? (o[i] = (0, n.Z)({}, u), Object.keys(a).forEach(t => {
+                                    o[i][t] = e(a[t], u[t])
+                                })) : o[i] = u : o[i] = a
                             } else void 0 === o[i] && (o[i] = t[i])
                         }), o
                     }
                 }
             });
             var n = r(7462)
         },
@@ -2591,46 +2336,46 @@
                     $$typeof: !0,
                     compare: !0,
                     defaultProps: !0,
                     displayName: !0,
                     propTypes: !0,
                     type: !0
                 },
-                s = {};
+                u = {};
 
-            function u(e) {
-                return n.isMemo(e) ? a : s[e.$$typeof] || o
+            function s(e) {
+                return n.isMemo(e) ? a : u[e.$$typeof] || o
             }
-            s[n.ForwardRef] = {
+            u[n.ForwardRef] = {
                 $$typeof: !0,
                 render: !0,
                 defaultProps: !0,
                 displayName: !0,
                 propTypes: !0
-            }, s[n.Memo] = a;
+            }, u[n.Memo] = a;
             var c = Object.defineProperty,
                 l = Object.getOwnPropertyNames,
                 f = Object.getOwnPropertySymbols,
                 p = Object.getOwnPropertyDescriptor,
                 d = Object.getPrototypeOf,
                 m = Object.prototype;
             e.exports = function e(t, r, n) {
                 if ("string" != typeof r) {
                     if (m) {
                         var o = d(r);
                         o && o !== m && e(t, o, n)
                     }
                     var a = l(r);
                     f && (a = a.concat(f(r)));
-                    for (var s = u(t), h = u(r), y = 0; y < a.length; ++y) {
-                        var g = a[y];
-                        if (!i[g] && !(n && n[g]) && !(h && h[g]) && !(s && s[g])) {
-                            var b = p(r, g);
+                    for (var u = s(t), h = s(r), g = 0; g < a.length; ++g) {
+                        var y = a[g];
+                        if (!i[y] && !(n && n[y]) && !(h && h[y]) && !(u && u[y])) {
+                            var b = p(r, y);
                             try {
-                                c(t, g, b)
+                                c(t, y, b)
                             } catch (e) {}
                         }
                     }
                 }
                 return t
             }
         },
@@ -2645,282 +2390,537 @@
              * LICENSE file in the root directory of this source tree.
              */
             var r = "function" == typeof Symbol && Symbol.for,
                 n = r ? Symbol.for("react.element") : 60103,
                 o = r ? Symbol.for("react.portal") : 60106,
                 i = r ? Symbol.for("react.fragment") : 60107,
                 a = r ? Symbol.for("react.strict_mode") : 60108,
-                s = r ? Symbol.for("react.profiler") : 60114,
-                u = r ? Symbol.for("react.provider") : 60109,
+                u = r ? Symbol.for("react.profiler") : 60114,
+                s = r ? Symbol.for("react.provider") : 60109,
                 c = r ? Symbol.for("react.context") : 60110,
                 l = r ? Symbol.for("react.async_mode") : 60111,
                 f = r ? Symbol.for("react.concurrent_mode") : 60111,
                 p = r ? Symbol.for("react.forward_ref") : 60112,
                 d = r ? Symbol.for("react.suspense") : 60113,
                 m = r ? Symbol.for("react.suspense_list") : 60120,
                 h = r ? Symbol.for("react.memo") : 60115,
-                y = r ? Symbol.for("react.lazy") : 60116,
-                g = r ? Symbol.for("react.block") : 60121,
+                g = r ? Symbol.for("react.lazy") : 60116,
+                y = r ? Symbol.for("react.block") : 60121,
                 b = r ? Symbol.for("react.fundamental") : 60117,
                 v = r ? Symbol.for("react.responder") : 60118,
                 x = r ? Symbol.for("react.scope") : 60119;
 
-            function k(e) {
+            function $(e) {
                 if ("object" == typeof e && null !== e) {
                     var t = e.$$typeof;
                     switch (t) {
                         case n:
                             switch (e = e.type) {
                                 case l:
                                 case f:
                                 case i:
-                                case s:
+                                case u:
                                 case a:
                                 case d:
                                     return e;
                                 default:
                                     switch (e = e && e.$$typeof) {
                                         case c:
                                         case p:
-                                        case y:
+                                        case g:
                                         case h:
-                                        case u:
+                                        case s:
                                             return e;
                                         default:
                                             return t
                                     }
                             }
                         case o:
                             return t
                     }
                 }
             }
 
-            function Z(e) {
-                return k(e) === f
+            function k(e) {
+                return $(e) === f
             }
-            t.AsyncMode = l, t.ConcurrentMode = f, t.ContextConsumer = c, t.ContextProvider = u, t.Element = n, t.ForwardRef = p, t.Fragment = i, t.Lazy = y, t.Memo = h, t.Portal = o, t.Profiler = s, t.StrictMode = a, t.Suspense = d, t.isAsyncMode = function(e) {
-                return Z(e) || k(e) === l
-            }, t.isConcurrentMode = Z, t.isContextConsumer = function(e) {
-                return k(e) === c
+            t.AsyncMode = l, t.ConcurrentMode = f, t.ContextConsumer = c, t.ContextProvider = s, t.Element = n, t.ForwardRef = p, t.Fragment = i, t.Lazy = g, t.Memo = h, t.Portal = o, t.Profiler = u, t.StrictMode = a, t.Suspense = d, t.isAsyncMode = function(e) {
+                return k(e) || $(e) === l
+            }, t.isConcurrentMode = k, t.isContextConsumer = function(e) {
+                return $(e) === c
             }, t.isContextProvider = function(e) {
-                return k(e) === u
+                return $(e) === s
             }, t.isElement = function(e) {
                 return "object" == typeof e && null !== e && e.$$typeof === n
             }, t.isForwardRef = function(e) {
-                return k(e) === p
+                return $(e) === p
             }, t.isFragment = function(e) {
-                return k(e) === i
+                return $(e) === i
             }, t.isLazy = function(e) {
-                return k(e) === y
+                return $(e) === g
             }, t.isMemo = function(e) {
-                return k(e) === h
+                return $(e) === h
             }, t.isPortal = function(e) {
-                return k(e) === o
+                return $(e) === o
             }, t.isProfiler = function(e) {
-                return k(e) === s
+                return $(e) === u
             }, t.isStrictMode = function(e) {
-                return k(e) === a
+                return $(e) === a
             }, t.isSuspense = function(e) {
-                return k(e) === d
+                return $(e) === d
             }, t.isValidElementType = function(e) {
-                return "string" == typeof e || "function" == typeof e || e === i || e === f || e === s || e === a || e === d || e === m || "object" == typeof e && null !== e && (e.$$typeof === y || e.$$typeof === h || e.$$typeof === u || e.$$typeof === c || e.$$typeof === p || e.$$typeof === b || e.$$typeof === v || e.$$typeof === x || e.$$typeof === g)
-            }, t.typeOf = k
+                return "string" == typeof e || "function" == typeof e || e === i || e === f || e === u || e === a || e === d || e === m || "object" == typeof e && null !== e && (e.$$typeof === g || e.$$typeof === h || e.$$typeof === s || e.$$typeof === c || e.$$typeof === p || e.$$typeof === b || e.$$typeof === v || e.$$typeof === x || e.$$typeof === y)
+            }, t.typeOf = $
         },
         1296: function(e, t, r) {
             "use strict";
             e.exports = r(6103)
         },
         6840: function(e, t, r) {
             (window.__NEXT_P = window.__NEXT_P || []).push(["/_app", function() {
-                return r(2711)
+                return r(8131)
             }])
         },
         8103: function(e, t, r) {
             "use strict";
             r.d(t, {
                 m: function() {
-                    return s
+                    return u
                 },
                 r: function() {
-                    return u
+                    return s
                 }
             });
             var n = r(5893),
                 o = r(7294);
             let i = (0, o.createContext)(void 0),
                 a = (0, o.createContext)(null),
-                s = e => {
+                u = e => {
                     let {
                         children: t
-                    } = e, [r, s] = (0, o.useState)();
+                    } = e, [r, u] = (0, o.useState)();
                     return (0, n.jsx)(a.Provider, {
-                        value: s,
+                        value: u,
                         children: (0, n.jsx)(i.Provider, {
                             value: r,
                             children: t
                         })
                     })
                 },
-                u = () => {
+                s = () => {
                     let e = (0, o.useContext)(i),
                         t = (0, o.useContext)(a);
                     if (null === t) throw Error();
                     return [e, t]
                 }
         },
-        2711: function(e, t, r) {
+        8131: function(e, t, r) {
             "use strict";
             let n;
             r.r(t), r.d(t, {
                 default: function() {
-                    return B
+                    return Q
                 }
             });
             var o = r(5893),
                 i = r(7294),
                 a = r(2443),
-                s = r(8417);
+                u = r(1526),
+                s = r(6411),
+                c = r(6686),
+                l = r(7563),
+                f = r(211),
+                p = r(8160),
+                d = r(2190),
+                m = function(e, t, r) {
+                    for (var n = 0, o = 0; n = o, o = (0, s.fj)(), 38 === n && 12 === o && (t[r] = 1), !(0, s.r)(o);)(0, s.lp)();
+                    return (0, s.tP)(e, s.FK)
+                },
+                h = function(e, t) {
+                    var r = -1,
+                        n = 44;
+                    do switch ((0, s.r)(n)) {
+                        case 0:
+                            38 === n && 12 === (0, s.fj)() && (t[r] = 1), e[r] += m(s.FK - 1, t, r);
+                            break;
+                        case 2:
+                            e[r] += (0, s.iF)(n);
+                            break;
+                        case 4:
+                            if (44 === n) {
+                                e[++r] = 58 === (0, s.fj)() ? "&\f" : "", t[r] = e[r].length;
+                                break
+                            }
+                        default:
+                            e[r] += (0, c.Dp)(n)
+                    }
+                    while (n = (0, s.lp)());
+                    return e
+                },
+                g = new WeakMap,
+                y = function(e) {
+                    if ("rule" === e.type && e.parent && !(e.length < 1)) {
+                        for (var t = e.value, r = e.parent, n = e.column === r.column && e.line === r.line;
+                            "rule" !== r.type;)
+                            if (!(r = r.parent)) return;
+                        if ((1 !== e.props.length || 58 === t.charCodeAt(0) || g.get(r)) && !n) {
+                            g.set(e, !0);
+                            for (var o = [], i = (0, s.cE)(h((0, s.un)(t), o)), a = r.props, u = 0, c = 0; u < i.length; u++)
+                                for (var l = 0; l < a.length; l++, c++) e.props[c] = o[u] ? i[u].replace(/&\f/g, a[l]) : a[l] + " " + i[u]
+                        }
+                    }
+                },
+                b = function(e) {
+                    if ("decl" === e.type) {
+                        var t = e.value;
+                        108 === t.charCodeAt(0) && 98 === t.charCodeAt(2) && (e.return = "", e.value = "")
+                    }
+                },
+                v = [function(e, t, r, n) {
+                    if (e.length > -1 && !e.return) switch (e.type) {
+                        case l.h5:
+                            e.return = function e(t, r) {
+                                switch ((0, c.vp)(t, r)) {
+                                    case 5103:
+                                        return l.G$ + "print-" + t + t;
+                                    case 5737:
+                                    case 4201:
+                                    case 3177:
+                                    case 3433:
+                                    case 1641:
+                                    case 4457:
+                                    case 2921:
+                                    case 5572:
+                                    case 6356:
+                                    case 5844:
+                                    case 3191:
+                                    case 6645:
+                                    case 3005:
+                                    case 6391:
+                                    case 5879:
+                                    case 5623:
+                                    case 6135:
+                                    case 4599:
+                                    case 4855:
+                                    case 4215:
+                                    case 6389:
+                                    case 5109:
+                                    case 5365:
+                                    case 5621:
+                                    case 3829:
+                                        return l.G$ + t + t;
+                                    case 5349:
+                                    case 4246:
+                                    case 4810:
+                                    case 6968:
+                                    case 2756:
+                                        return l.G$ + t + l.uj + t + l.MS + t + t;
+                                    case 6828:
+                                    case 4268:
+                                        return l.G$ + t + l.MS + t + t;
+                                    case 6165:
+                                        return l.G$ + t + l.MS + "flex-" + t + t;
+                                    case 5187:
+                                        return l.G$ + t + (0, c.gx)(t, /(\w+).+(:[^]+)/, l.G$ + "box-$1$2" + l.MS + "flex-$1$2") + t;
+                                    case 5443:
+                                        return l.G$ + t + l.MS + "flex-item-" + (0, c.gx)(t, /flex-|-self/, "") + t;
+                                    case 4675:
+                                        return l.G$ + t + l.MS + "flex-line-pack" + (0, c.gx)(t, /align-content|flex-|-self/, "") + t;
+                                    case 5548:
+                                        return l.G$ + t + l.MS + (0, c.gx)(t, "shrink", "negative") + t;
+                                    case 5292:
+                                        return l.G$ + t + l.MS + (0, c.gx)(t, "basis", "preferred-size") + t;
+                                    case 6060:
+                                        return l.G$ + "box-" + (0, c.gx)(t, "-grow", "") + l.G$ + t + l.MS + (0, c.gx)(t, "grow", "positive") + t;
+                                    case 4554:
+                                        return l.G$ + (0, c.gx)(t, /([^-])(transform)/g, "$1" + l.G$ + "$2") + t;
+                                    case 6187:
+                                        return (0, c.gx)((0, c.gx)((0, c.gx)(t, /(zoom-|grab)/, l.G$ + "$1"), /(image-set)/, l.G$ + "$1"), t, "") + t;
+                                    case 5495:
+                                    case 3959:
+                                        return (0, c.gx)(t, /(image-set\([^]*)/, l.G$ + "$1$`$1");
+                                    case 4968:
+                                        return (0, c.gx)((0, c.gx)(t, /(.+:)(flex-)?(.*)/, l.G$ + "box-pack:$3" + l.MS + "flex-pack:$3"), /s.+-b[^;]+/, "justify") + l.G$ + t + t;
+                                    case 4095:
+                                    case 3583:
+                                    case 4068:
+                                    case 2532:
+                                        return (0, c.gx)(t, /(.+)-inline(.+)/, l.G$ + "$1$2") + t;
+                                    case 8116:
+                                    case 7059:
+                                    case 5753:
+                                    case 5535:
+                                    case 5445:
+                                    case 5701:
+                                    case 4933:
+                                    case 4677:
+                                    case 5533:
+                                    case 5789:
+                                    case 5021:
+                                    case 4765:
+                                        if ((0, c.to)(t) - 1 - r > 6) switch ((0, c.uO)(t, r + 1)) {
+                                            case 109:
+                                                if (45 !== (0, c.uO)(t, r + 4)) break;
+                                            case 102:
+                                                return (0, c.gx)(t, /(.+:)(.+)-([^]+)/, "$1" + l.G$ + "$2-$3$1" + l.uj + (108 == (0, c.uO)(t, r + 3) ? "$3" : "$2-$3")) + t;
+                                            case 115:
+                                                return ~(0, c.Cw)(t, "stretch") ? e((0, c.gx)(t, "stretch", "fill-available"), r) + t : t
+                                        }
+                                        break;
+                                    case 4949:
+                                        if (115 !== (0, c.uO)(t, r + 1)) break;
+                                    case 6444:
+                                        switch ((0, c.uO)(t, (0, c.to)(t) - 3 - (~(0, c.Cw)(t, "!important") && 10))) {
+                                            case 107:
+                                                return (0, c.gx)(t, ":", ":" + l.G$) + t;
+                                            case 101:
+                                                return (0, c.gx)(t, /(.+:)([^;!]+)(;|!.+)?/, "$1" + l.G$ + (45 === (0, c.uO)(t, 14) ? "inline-" : "") + "box$3$1" + l.G$ + "$2$3$1" + l.MS + "$2box$3") + t
+                                        }
+                                        break;
+                                    case 5936:
+                                        switch ((0, c.uO)(t, r + 11)) {
+                                            case 114:
+                                                return l.G$ + t + l.MS + (0, c.gx)(t, /[svh]\w+-[tblr]{2}/, "tb") + t;
+                                            case 108:
+                                                return l.G$ + t + l.MS + (0, c.gx)(t, /[svh]\w+-[tblr]{2}/, "tb-rl") + t;
+                                            case 45:
+                                                return l.G$ + t + l.MS + (0, c.gx)(t, /[svh]\w+-[tblr]{2}/, "lr") + t
+                                        }
+                                        return l.G$ + t + l.MS + t + t
+                                }
+                                return t
+                            }(e.value, e.length);
+                            break;
+                        case l.lK:
+                            return (0, f.q)([(0, s.JG)(e, {
+                                value: (0, c.gx)(e.value, "@", "@" + l.G$)
+                            })], n);
+                        case l.Fr:
+                            if (e.length) return (0, c.$e)(e.props, function(t) {
+                                switch ((0, c.EQ)(t, /(::plac\w+|:read-\w+)/)) {
+                                    case ":read-only":
+                                    case ":read-write":
+                                        return (0, f.q)([(0, s.JG)(e, {
+                                            props: [(0, c.gx)(t, /:(read-\w+)/, ":" + l.uj + "$1")]
+                                        })], n);
+                                    case "::placeholder":
+                                        return (0, f.q)([(0, s.JG)(e, {
+                                            props: [(0, c.gx)(t, /:(plac\w+)/, ":" + l.G$ + "input-$1")]
+                                        }), (0, s.JG)(e, {
+                                            props: [(0, c.gx)(t, /:(plac\w+)/, ":" + l.uj + "$1")]
+                                        }), (0, s.JG)(e, {
+                                            props: [(0, c.gx)(t, /:(plac\w+)/, l.MS + "input-$1")]
+                                        })], n)
+                                }
+                                return ""
+                            })
+                    }
+                }];
 
-            function u(e) {
+            function x(e) {
                 let {
                     injectFirst: t,
                     children: r
                 } = e;
                 return t && n ? (0, o.jsx)(a.C, {
                     value: n,
                     children: r
                 }) : r
             }
-            "object" == typeof document && (n = (0, s.Z)({
+            "object" == typeof document && (n = function(e) {
+                var t = e.key;
+                if ("css" === t) {
+                    var r = document.querySelectorAll("style[data-emotion]:not([data-s])");
+                    Array.prototype.forEach.call(r, function(e) {
+                        -1 !== e.getAttribute("data-emotion").indexOf(" ") && (document.head.appendChild(e), e.setAttribute("data-s", ""))
+                    })
+                }
+                var n = e.stylisPlugins || v,
+                    o = {},
+                    i = [];
+                a = e.container || document.head, Array.prototype.forEach.call(document.querySelectorAll('style[data-emotion^="' + t + ' "]'), function(e) {
+                    for (var t = e.getAttribute("data-emotion").split(" "), r = 1; r < t.length; r++) o[t[r]] = !0;
+                    i.push(e)
+                });
+                var a, s, c = [f.P, (0, p.cD)(function(e) {
+                        s.insert(e)
+                    })],
+                    l = (0, p.qR)([y, b].concat(n, c)),
+                    m = {
+                        key: t,
+                        sheet: new u.m({
+                            key: t,
+                            container: a,
+                            nonce: e.nonce,
+                            speedy: e.speedy,
+                            prepend: e.prepend,
+                            insertionPoint: e.insertionPoint
+                        }),
+                        nonce: e.nonce,
+                        inserted: o,
+                        registered: {},
+                        insert: function(e, t, r, n) {
+                            var o;
+                            s = r, o = e ? e + "{" + t.styles + "}" : t.styles, (0, f.q)((0, d.MY)(o), l), n && (m.inserted[t.name] = !0)
+                        }
+                    };
+                return m.sheet.hydrate(i), m
+            }({
                 key: "css",
                 prepend: !0
             }));
-            var c = r(7462),
-                l = r(4819),
-                f = r(6760);
-            let p = "function" == typeof Symbol && Symbol.for;
-            var d = p ? Symbol.for("mui.nested") : "__THEME_NESTED__",
-                m = function(e) {
+            var $ = r(7462),
+                k = r(3366);
+            let w = i.createContext(null);
+
+            function S() {
+                let e = i.useContext(w);
+                return e
+            }
+            let Z = "function" == typeof Symbol && Symbol.for;
+            var O = Z ? Symbol.for("mui.nested") : "__THEME_NESTED__",
+                A = function(e) {
                     let {
                         children: t,
                         theme: r
-                    } = e, n = (0, f.Z)(), a = i.useMemo(() => {
+                    } = e, n = S(), a = i.useMemo(() => {
                         let e = null === n ? r : function(e, t) {
                             if ("function" == typeof t) {
                                 let r = t(e);
                                 return r
                             }
-                            return (0, c.Z)({}, e, t)
+                            return (0, $.Z)({}, e, t)
                         }(n, r);
-                        return null != e && (e[d] = null !== n), e
+                        return null != e && (e[O] = null !== n), e
                     }, [r, n]);
-                    return (0, o.jsx)(l.Z.Provider, {
+                    return (0, o.jsx)(w.Provider, {
                         value: a,
                         children: t
                     })
                 },
-                h = r(6682);
-            let y = {};
+                j = r(4168);
+            let C = {};
 
-            function g(e) {
-                let t = (0, h.Z)();
-                return (0, o.jsx)(a.T.Provider, {
-                    value: "object" == typeof t ? t : y,
-                    children: e.children
-                })
+            function P(e, t, r, n = !1) {
+                return i.useMemo(() => {
+                    let o = e && t[e] || t;
+                    if ("function" == typeof r) {
+                        let i = r(o),
+                            a = e ? (0, $.Z)({}, t, {
+                                [e]: i
+                            }) : i;
+                        return n ? () => a : a
+                    }
+                    return e ? (0, $.Z)({}, t, {
+                        [e]: r
+                    }) : (0, $.Z)({}, t, r)
+                }, [e, t, r, n])
             }
-            var b = function(e) {
+            var G = function(e) {
                     let {
                         children: t,
-                        theme: r
-                    } = e;
-                    return (0, o.jsx)(m, {
                         theme: r,
-                        children: (0, o.jsx)(g, {
+                        themeId: n
+                    } = e, i = (0, j.Z)(C), u = S() || C, s = P(n, i, r), c = P(n, u, r, !0);
+                    return (0, o.jsx)(A, {
+                        theme: c,
+                        children: (0, o.jsx)(a.T.Provider, {
+                            value: s,
                             children: t
                         })
                     })
                 },
-                v = r(1657),
-                x = r(2287);
-            let k = (e, t) => (0, c.Z)({
+                M = r(606);
+            let E = ["theme"];
+
+            function T(e) {
+                let {
+                    theme: t
+                } = e, r = (0, k.Z)(e, E), n = t[M.Z];
+                return (0, o.jsx)(G, (0, $.Z)({}, r, {
+                    themeId: n ? M.Z : void 0,
+                    theme: n || t
+                }))
+            }
+            var R = r(1657),
+                _ = r(7297);
+            let F = (e, t) => (0, $.Z)({
                     WebkitFontSmoothing: "antialiased",
                     MozOsxFontSmoothing: "grayscale",
                     boxSizing: "border-box",
                     WebkitTextSizeAdjust: "100%"
                 }, t && !e.vars && {
                     colorScheme: e.palette.mode
                 }),
-                Z = e => (0, c.Z)({
+                K = e => (0, $.Z)({
                     color: (e.vars || e).palette.text.primary
                 }, e.typography.body1, {
                     backgroundColor: (e.vars || e).palette.background.default,
                     "@media print": {
                         backgroundColor: (e.vars || e).palette.common.white
                     }
                 }),
-                $ = (e, t = !1) => {
+                I = (e, t = !1) => {
                     var r, n;
                     let o = {};
                     t && e.colorSchemes && Object.entries(e.colorSchemes).forEach(([t, r]) => {
                         var n;
                         o[e.getColorSchemeSelector(t).replace(/\s*&/, "")] = {
                             colorScheme: null == (n = r.palette) ? void 0 : n.mode
                         }
                     });
-                    let i = (0, c.Z)({
-                            html: k(e, t),
+                    let i = (0, $.Z)({
+                            html: F(e, t),
                             "*, *::before, *::after": {
                                 boxSizing: "inherit"
                             },
                             "strong, b": {
                                 fontWeight: e.typography.fontWeightBold
                             },
-                            body: (0, c.Z)({
+                            body: (0, $.Z)({
                                 margin: 0
-                            }, Z(e), {
+                            }, K(e), {
                                 "&::backdrop": {
                                     backgroundColor: (e.vars || e).palette.background.default
                                 }
                             })
                         }, o),
                         a = null == (r = e.components) ? void 0 : null == (n = r.MuiCssBaseline) ? void 0 : n.styleOverrides;
                     return a && (i = [i, a]), i
                 };
-            var w = function(e) {
-                    let t = (0, v.Z)({
+            var z = function(e) {
+                    let t = (0, R.Z)({
                             props: e,
                             name: "MuiCssBaseline"
                         }),
                         {
                             children: r,
                             enableColorScheme: n = !1
                         } = t;
                     return (0, o.jsxs)(i.Fragment, {
-                        children: [(0, o.jsx)(x.Z, {
-                            styles: e => $(e, n)
+                        children: [(0, o.jsx)(_.Z, {
+                            styles: e => I(e, n)
                         }), r]
                     })
                 },
-                S = r(9008),
-                O = r.n(S);
+                B = r(9008),
+                W = r.n(B);
             r(5314);
-            var A = r(8103),
-                C = r(1919),
-                P = r(1387);
+            var q = r(8103),
+                N = r(1919),
+                D = r(1387);
 
-            function j(e) {
+            function L(e) {
                 return String(parseFloat(e)).length === String(e).length
             }
 
-            function E(e) {
+            function H(e) {
                 return parseFloat(e)
             }
-            var T = {
+            var J = {
                     50: "#ede7f6",
                     100: "#d1c4e9",
                     200: "#b39ddb",
                     300: "#9575cd",
                     400: "#7e57c2",
                     500: "#673ab7",
                     600: "#5e35b1",
@@ -2928,26 +2928,26 @@
                     800: "#4527a0",
                     900: "#311b92",
                     A100: "#b388ff",
                     A200: "#7c4dff",
                     A400: "#651fff",
                     A700: "#6200ea"
                 },
-                _ = r(7036);
-            let M = (0, C.Z)({
+                U = r(7036);
+            let Y = (0, N.Z)({
                 palette: {
                     mode: "dark",
                     primary: {
-                        dark: T[800],
-                        main: T[700],
-                        light: T[600]
+                        dark: J[800],
+                        main: J[700],
+                        light: J[600]
                     },
-                    secondary: T,
+                    secondary: J,
                     background: {
-                        default: _.Z[900],
+                        default: U.Z[900],
                         paper: "#212121"
                     },
                     contrastThreshold: 3,
                     tonalOffset: .2
                 },
                 components: {
                     MuiCard: {
@@ -2979,49 +2979,49 @@
                             root: {
                                 justifyContent: "flex-end"
                             }
                         }
                     }
                 }
             });
-            var R = M = function(e, t = {}) {
+            var X = Y = function(e, t = {}) {
                 var r;
                 let {
                     breakpoints: n = ["sm", "md", "lg"],
                     disableAlign: o = !1,
                     factor: i = 2,
                     variants: a = ["h1", "h2", "h3", "h4", "h5", "h6", "subtitle1", "subtitle2", "body1", "body2", "caption", "button", "overline"]
-                } = t, s = (0, c.Z)({}, e);
-                s.typography = (0, c.Z)({}, s.typography);
-                let u = s.typography,
-                    l = (r = u.htmlFontSize, (e, t) => {
+                } = t, u = (0, $.Z)({}, e);
+                u.typography = (0, $.Z)({}, u.typography);
+                let s = u.typography,
+                    c = (r = s.htmlFontSize, (e, t) => {
                         let n = String(e).match(/[\d.\-+]*\s*(.*)/)[1] || "";
                         if (n === t) return e;
-                        let o = E(e);
-                        "px" !== n && ("em" === n ? o = E(e) * E(r) : "rem" === n && (o = E(e) * E(r)));
+                        let o = H(e);
+                        "px" !== n && ("em" === n ? o = H(e) * H(r) : "rem" === n && (o = H(e) * H(r)));
                         let i = o;
                         if ("px" !== t) {
-                            if ("em" === t) i = o / E(r);
+                            if ("em" === t) i = o / H(r);
                             else {
                                 if ("rem" !== t) return e;
-                                i = o / E(r)
+                                i = o / H(r)
                             }
                         }
                         return parseFloat(i.toFixed(5)) + t
                     }),
-                    f = n.map(e => s.breakpoints.values[e]);
+                    l = n.map(e => u.breakpoints.values[e]);
                 return a.forEach(e => {
-                    let t = u[e],
-                        r = parseFloat(l(t.fontSize, "rem"));
+                    let t = s[e],
+                        r = parseFloat(c(t.fontSize, "rem"));
                     if (r <= 1) return;
                     let {
                         lineHeight: n
                     } = t;
-                    if (!j(n) && !o) throw Error((0, P.Z)(6));
-                    j(n) || (n = parseFloat(l(n, "rem")) / parseFloat(r));
+                    if (!L(n) && !o) throw Error((0, D.Z)(6));
+                    L(n) || (n = parseFloat(c(n, "rem")) / parseFloat(r));
                     let a = null;
                     o || (a = e => (function({
                         size: e,
                         grid: t
                     }) {
                         let r = e - e % t,
                             n = r + t;
@@ -3033,69 +3033,69 @@
                             pixels: t,
                             htmlFontSize: r
                         }) {
                             return t / (e * r)
                         }({
                             pixels: 4,
                             lineHeight: n,
-                            htmlFontSize: u.htmlFontSize
+                            htmlFontSize: s.htmlFontSize
                         })
-                    })), u[e] = (0, c.Z)({}, t, function({
+                    })), s[e] = (0, $.Z)({}, t, function({
                         cssProperty: e,
                         min: t,
                         max: r,
                         unit: n = "rem",
                         breakpoints: o = [600, 900, 1200],
                         transform: i = null
                     }) {
                         let a = {
                                 [e]: `${t}${n}`
                             },
-                            s = (r - t) / o[o.length - 1];
+                            u = (r - t) / o[o.length - 1];
                         return o.forEach(r => {
-                            let o = t + s * r;
+                            let o = t + u * r;
                             null !== i && (o = i(o)), a[`@media (min-width:${r}px)`] = {
                                 [e]: `${Math.round(1e4*o)/1e4}${n}`
                             }
                         }), a
                     }({
                         cssProperty: "fontSize",
                         min: 1 + (r - 1) / i,
                         max: r,
                         unit: "rem",
-                        breakpoints: f,
+                        breakpoints: l,
                         transform: a
                     }))
-                }), s
-            }(M);
+                }), u
+            }(Y);
             r(9409);
-            var B = function(e) {
+            var Q = function(e) {
                 let {
                     Component: t,
                     pageProps: r
                 } = e;
                 return (0, i.useEffect)(() => {
                     document.documentElement.lang = "en-GB";
                     let e = document.querySelector("#jss-server-side");
                     (null == e ? void 0 : e.parentElement) && e.parentElement.removeChild(e)
                 }, []), (0, o.jsxs)(o.Fragment, {
-                    children: [(0, o.jsxs)(O(), {
+                    children: [(0, o.jsxs)(W(), {
                         children: [(0, o.jsx)("title", {
                             children: "System Bridge"
                         }), (0, o.jsx)("meta", {
                             name: "viewport",
                             content: "minimum-scale=1, initial-scale=1, width=device-width"
                         })]
-                    }), (0, o.jsx)(u, {
+                    }), (0, o.jsx)(x, {
                         injectFirst: !0,
-                        children: (0, o.jsx)(b, {
-                            theme: R,
-                            children: (0, o.jsx)(A.m, {
+                        children: (0, o.jsx)(T, {
+                            theme: X,
+                            children: (0, o.jsx)(q.m, {
                                 children: (0, o.jsxs)(o.Fragment, {
-                                    children: [(0, o.jsx)(w, {}), (0, o.jsx)(t, {
+                                    children: [(0, o.jsx)(z, {}), (0, o.jsx)(t, {
                                         ...r
                                     })]
                                 })
                             })
                         })
                     })]
                 })
@@ -3135,14 +3135,504 @@
                 return o
             }
             r.d(t, {
                 Z: function() {
                     return n
                 }
             })
+        },
+        7563: function(e, t, r) {
+            "use strict";
+            r.d(t, {
+                Ab: function() {
+                    return a
+                },
+                Fr: function() {
+                    return u
+                },
+                G$: function() {
+                    return i
+                },
+                K$: function() {
+                    return c
+                },
+                MS: function() {
+                    return n
+                },
+                h5: function() {
+                    return s
+                },
+                lK: function() {
+                    return l
+                },
+                uj: function() {
+                    return o
+                }
+            });
+            var n = "-ms-",
+                o = "-moz-",
+                i = "-webkit-",
+                a = "comm",
+                u = "rule",
+                s = "decl",
+                c = "@import",
+                l = "@keyframes"
+        },
+        8160: function(e, t, r) {
+            "use strict";
+            r.d(t, {
+                cD: function() {
+                    return i
+                },
+                qR: function() {
+                    return o
+                }
+            });
+            var n = r(6686);
+
+            function o(e) {
+                var t = (0, n.Ei)(e);
+                return function(r, n, o, i) {
+                    for (var a = "", u = 0; u < t; u++) a += e[u](r, n, o, i) || "";
+                    return a
+                }
+            }
+
+            function i(e) {
+                return function(t) {
+                    !t.root && (t = t.return) && e(t)
+                }
+            }
+        },
+        2190: function(e, t, r) {
+            "use strict";
+            r.d(t, {
+                MY: function() {
+                    return a
+                }
+            });
+            var n = r(7563),
+                o = r(6686),
+                i = r(6411);
+
+            function a(e) {
+                return (0, i.cE)(function e(t, r, a, c, l, f, p, d, m) {
+                    for (var h, g = 0, y = 0, b = p, v = 0, x = 0, $ = 0, k = 1, w = 1, S = 1, Z = 0, O = "", A = l, j = f, C = c, P = O; w;) switch ($ = Z, Z = (0, i.lp)()) {
+                        case 40:
+                            if (108 != $ && 58 == (0, o.uO)(P, b - 1)) {
+                                -1 != (0, o.Cw)(P += (0, o.gx)((0, i.iF)(Z), "&", "&\f"), "&\f") && (S = -1);
+                                break
+                            }
+                        case 34:
+                        case 39:
+                        case 91:
+                            P += (0, i.iF)(Z);
+                            break;
+                        case 9:
+                        case 10:
+                        case 13:
+                        case 32:
+                            P += (0, i.Qb)($);
+                            break;
+                        case 92:
+                            P += (0, i.kq)((0, i.Ud)() - 1, 7);
+                            continue;
+                        case 47:
+                            switch ((0, i.fj)()) {
+                                case 42:
+                                case 47:
+                                    (0, o.R3)((h = (0, i.q6)((0, i.lp)(), (0, i.Ud)()), (0, i.dH)(h, r, a, n.Ab, (0, o.Dp)((0, i.Tb)()), (0, o.tb)(h, 2, -2), 0)), m);
+                                    break;
+                                default:
+                                    P += "/"
+                            }
+                            break;
+                        case 123 * k:
+                            d[g++] = (0, o.to)(P) * S;
+                        case 125 * k:
+                        case 59:
+                        case 0:
+                            switch (Z) {
+                                case 0:
+                                case 125:
+                                    w = 0;
+                                case 59 + y:
+                                    x > 0 && (0, o.to)(P) - b && (0, o.R3)(x > 32 ? s(P + ";", c, a, b - 1) : s((0, o.gx)(P, " ", "") + ";", c, a, b - 2), m);
+                                    break;
+                                case 59:
+                                    P += ";";
+                                default:
+                                    if ((0, o.R3)(C = u(P, r, a, g, y, l, d, O, A = [], j = [], b), f), 123 === Z) {
+                                        if (0 === y) e(P, r, C, C, A, f, b, d, j);
+                                        else switch (99 === v && 110 === (0, o.uO)(P, 3) ? 100 : v) {
+                                            case 100:
+                                            case 109:
+                                            case 115:
+                                                e(t, C, C, c && (0, o.R3)(u(t, C, C, 0, 0, l, d, O, l, A = [], b), j), l, j, b, d, c ? A : j);
+                                                break;
+                                            default:
+                                                e(P, C, C, C, [""], j, 0, d, j)
+                                        }
+                                    }
+                            }
+                            g = y = x = 0, k = S = 1, O = P = "", b = p;
+                            break;
+                        case 58:
+                            b = 1 + (0, o.to)(P), x = $;
+                        default:
+                            if (k < 1) {
+                                if (123 == Z) --k;
+                                else if (125 == Z && 0 == k++ && 125 == (0, i.mp)()) continue
+                            }
+                            switch (P += (0, o.Dp)(Z), Z * k) {
+                                case 38:
+                                    S = y > 0 ? 1 : (P += "\f", -1);
+                                    break;
+                                case 44:
+                                    d[g++] = ((0, o.to)(P) - 1) * S, S = 1;
+                                    break;
+                                case 64:
+                                    45 === (0, i.fj)() && (P += (0, i.iF)((0, i.lp)())), v = (0, i.fj)(), y = b = (0, o.to)(O = P += (0, i.QU)((0, i.Ud)())), Z++;
+                                    break;
+                                case 45:
+                                    45 === $ && 2 == (0, o.to)(P) && (k = 0)
+                            }
+                    }
+                    return f
+                }("", null, null, null, [""], e = (0, i.un)(e), 0, [0], e))
+            }
+
+            function u(e, t, r, a, u, s, c, l, f, p, d) {
+                for (var m = u - 1, h = 0 === u ? s : [""], g = (0, o.Ei)(h), y = 0, b = 0, v = 0; y < a; ++y)
+                    for (var x = 0, $ = (0, o.tb)(e, m + 1, m = (0, o.Wn)(b = c[y])), k = e; x < g; ++x)(k = (0, o.fy)(b > 0 ? h[x] + " " + $ : (0, o.gx)($, /&\f/g, h[x]))) && (f[v++] = k);
+                return (0, i.dH)(e, t, r, 0 === u ? n.Fr : l, f, p, d)
+            }
+
+            function s(e, t, r, a) {
+                return (0, i.dH)(e, t, r, n.h5, (0, o.tb)(e, 0, a), (0, o.tb)(e, a + 1, -1), a)
+            }
+        },
+        211: function(e, t, r) {
+            "use strict";
+            r.d(t, {
+                P: function() {
+                    return a
+                },
+                q: function() {
+                    return i
+                }
+            });
+            var n = r(7563),
+                o = r(6686);
+
+            function i(e, t) {
+                for (var r = "", n = (0, o.Ei)(e), i = 0; i < n; i++) r += t(e[i], i, e, t) || "";
+                return r
+            }
+
+            function a(e, t, r, a) {
+                switch (e.type) {
+                    case n.K$:
+                    case n.h5:
+                        return e.return = e.return || e.value;
+                    case n.Ab:
+                        return "";
+                    case n.lK:
+                        return e.return = e.value + "{" + i(e.children, a) + "}";
+                    case n.Fr:
+                        e.value = e.props.join(",")
+                }
+                return (0, o.to)(r = i(e.children, a)) ? e.return = e.value + "{" + r + "}" : ""
+            }
+        },
+        6411: function(e, t, r) {
+            "use strict";
+            r.d(t, {
+                FK: function() {
+                    return u
+                },
+                JG: function() {
+                    return f
+                },
+                QU: function() {
+                    return Z
+                },
+                Qb: function() {
+                    return k
+                },
+                Tb: function() {
+                    return p
+                },
+                Ud: function() {
+                    return g
+                },
+                cE: function() {
+                    return x
+                },
+                dH: function() {
+                    return l
+                },
+                fj: function() {
+                    return h
+                },
+                iF: function() {
+                    return $
+                },
+                kq: function() {
+                    return w
+                },
+                lp: function() {
+                    return m
+                },
+                mp: function() {
+                    return d
+                },
+                q6: function() {
+                    return S
+                },
+                r: function() {
+                    return b
+                },
+                tP: function() {
+                    return y
+                },
+                un: function() {
+                    return v
+                }
+            });
+            var n = r(6686),
+                o = 1,
+                i = 1,
+                a = 0,
+                u = 0,
+                s = 0,
+                c = "";
+
+            function l(e, t, r, n, a, u, s) {
+                return {
+                    value: e,
+                    root: t,
+                    parent: r,
+                    type: n,
+                    props: a,
+                    children: u,
+                    line: o,
+                    column: i,
+                    length: s,
+                    return: ""
+                }
+            }
+
+            function f(e, t) {
+                return (0, n.f0)(l("", null, null, "", null, null, 0), e, {
+                    length: -e.length
+                }, t)
+            }
+
+            function p() {
+                return s
+            }
+
+            function d() {
+                return s = u > 0 ? (0, n.uO)(c, --u) : 0, i--, 10 === s && (i = 1, o--), s
+            }
+
+            function m() {
+                return s = u < a ? (0, n.uO)(c, u++) : 0, i++, 10 === s && (i = 1, o++), s
+            }
+
+            function h() {
+                return (0, n.uO)(c, u)
+            }
+
+            function g() {
+                return u
+            }
+
+            function y(e, t) {
+                return (0, n.tb)(c, e, t)
+            }
+
+            function b(e) {
+                switch (e) {
+                    case 0:
+                    case 9:
+                    case 10:
+                    case 13:
+                    case 32:
+                        return 5;
+                    case 33:
+                    case 43:
+                    case 44:
+                    case 47:
+                    case 62:
+                    case 64:
+                    case 126:
+                    case 59:
+                    case 123:
+                    case 125:
+                        return 4;
+                    case 58:
+                        return 3;
+                    case 34:
+                    case 39:
+                    case 40:
+                    case 91:
+                        return 2;
+                    case 41:
+                    case 93:
+                        return 1
+                }
+                return 0
+            }
+
+            function v(e) {
+                return o = i = 1, a = (0, n.to)(c = e), u = 0, []
+            }
+
+            function x(e) {
+                return c = "", e
+            }
+
+            function $(e) {
+                return (0, n.fy)(y(u - 1, function e(t) {
+                    for (; m();) switch (s) {
+                        case t:
+                            return u;
+                        case 34:
+                        case 39:
+                            34 !== t && 39 !== t && e(s);
+                            break;
+                        case 40:
+                            41 === t && e(t);
+                            break;
+                        case 92:
+                            m()
+                    }
+                    return u
+                }(91 === e ? e + 2 : 40 === e ? e + 1 : e)))
+            }
+
+            function k(e) {
+                for (; s = h();)
+                    if (s < 33) m();
+                    else break;
+                return b(e) > 2 || b(s) > 3 ? "" : " "
+            }
+
+            function w(e, t) {
+                for (; --t && m() && !(s < 48) && !(s > 102) && (!(s > 57) || !(s < 65)) && (!(s > 70) || !(s < 97)););
+                return y(e, u + (t < 6 && 32 == h() && 32 == m()))
+            }
+
+            function S(e, t) {
+                for (; m();)
+                    if (e + s === 57) break;
+                    else if (e + s === 84 && 47 === h()) break;
+                return "/*" + y(t, u - 1) + "*" + (0, n.Dp)(47 === e ? e : m())
+            }
+
+            function Z(e) {
+                for (; !b(h());) m();
+                return y(e, u)
+            }
+        },
+        6686: function(e, t, r) {
+            "use strict";
+            r.d(t, {
+                $e: function() {
+                    return g
+                },
+                Cw: function() {
+                    return l
+                },
+                Dp: function() {
+                    return o
+                },
+                EQ: function() {
+                    return s
+                },
+                Ei: function() {
+                    return m
+                },
+                R3: function() {
+                    return h
+                },
+                Wn: function() {
+                    return n
+                },
+                f0: function() {
+                    return i
+                },
+                fy: function() {
+                    return u
+                },
+                gx: function() {
+                    return c
+                },
+                tb: function() {
+                    return p
+                },
+                to: function() {
+                    return d
+                },
+                uO: function() {
+                    return f
+                },
+                vp: function() {
+                    return a
+                }
+            });
+            var n = Math.abs,
+                o = String.fromCharCode,
+                i = Object.assign;
+
+            function a(e, t) {
+                return 45 ^ f(e, 0) ? (((t << 2 ^ f(e, 0)) << 2 ^ f(e, 1)) << 2 ^ f(e, 2)) << 2 ^ f(e, 3) : 0
+            }
+
+            function u(e) {
+                return e.trim()
+            }
+
+            function s(e, t) {
+                return (e = t.exec(e)) ? e[0] : e
+            }
+
+            function c(e, t, r) {
+                return e.replace(t, r)
+            }
+
+            function l(e, t) {
+                return e.indexOf(t)
+            }
+
+            function f(e, t) {
+                return 0 | e.charCodeAt(t)
+            }
+
+            function p(e, t, r) {
+                return e.slice(t, r)
+            }
+
+            function d(e) {
+                return e.length
+            }
+
+            function m(e) {
+                return e.length
+            }
+
+            function h(e, t) {
+                return t.push(e), e
+            }
+
+            function g(e, t) {
+                return e.map(t).join("")
+            }
         }
     },
     function(e) {
         var t = function(t) {
             return e(e.s = t)
         };
         e.O(0, [774, 179], function() {
```

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/openon-4be476ff83910730.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/openon-4be476ff83910730.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/setup-58dc331f38afcee4.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/setup-58dc331f38afcee4.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/pages/app/data-5b613fd056889656.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/pages/app/data-5b613fd056889656.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/pages/app/notification-7c4c891692a1e4f4.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/pages/app/notification-7c4c891692a1e4f4.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/pages/app/player/audio-843238cdca1b0dca.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/pages/app/player/audio-843238cdca1b0dca.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/pages/app/player/video-3aa85bafaac31d57.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/pages/app/player/video-3aa85bafaac31d57.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/pages/app/settings-c25cd256e27b2200.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/pages/app/settings-c25cd256e27b2200.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/pages/index-f934b9a030f633a0.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/pages/index-f934b9a030f633a0.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/reactPlayerDailyMotion.da042b36db7662eb.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/reactPlayerDailyMotion.da042b36db7662eb.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/reactPlayerFacebook.3663ffcf10139668.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/reactPlayerFacebook.3663ffcf10139668.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/reactPlayerFilePlayer.812fbc47cf3ccebc.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/reactPlayerFilePlayer.812fbc47cf3ccebc.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/reactPlayerKaltura.46641a0f37607223.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/reactPlayerKaltura.46641a0f37607223.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/reactPlayerMixcloud.258ac8431338b78a.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/reactPlayerMixcloud.258ac8431338b78a.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/reactPlayerPreview.9b535aa9cbcb0a91.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/reactPlayerPreview.9b535aa9cbcb0a91.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/reactPlayerSoundCloud.60e72fefd71eeb25.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/reactPlayerSoundCloud.60e72fefd71eeb25.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/reactPlayerStreamable.c374322fbd4a05d5.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/reactPlayerStreamable.c374322fbd4a05d5.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/reactPlayerTwitch.52035ec5fd363953.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/reactPlayerTwitch.52035ec5fd363953.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/reactPlayerVidyard.8c3ec4a7a5b4aac4.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/reactPlayerVidyard.8c3ec4a7a5b4aac4.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/reactPlayerVimeo.5a5700a7f86e58a2.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/reactPlayerVimeo.5a5700a7f86e58a2.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/reactPlayerWistia.29aa97668baf75ea.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/reactPlayerWistia.29aa97668baf75ea.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/reactPlayerYouTube.77a6d75e3f5e95ef.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/reactPlayerYouTube.77a6d75e3f5e95ef.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/chunks/webpack-0eb9c66c948301b2.js` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/chunks/webpack-0eb9c66c948301b2.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/css/12f80ebf97adb4a5.css` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/css/12f80ebf97adb4a5.css`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/media/roboto-all-400-normal.2e9e9400.woff` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/media/roboto-all-400-normal.2e9e9400.woff`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.2d9c9d60.woff2` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.2d9c9d60.woff2`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.d7827ae3.woff2` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.d7827ae3.woff2`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.63e6dc18.woff2` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.63e6dc18.woff2`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/media/roboto-greek-ext-400-normal.2b547ded.woff2` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/media/roboto-greek-ext-400-normal.2b547ded.woff2`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/media/roboto-latin-400-normal.f2894edc.woff2` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/media/roboto-latin-400-normal.f2894edc.woff2`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/media/roboto-latin-ext-400-normal.21abc8c8.woff2` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/media/roboto-latin-ext-400-normal.21abc8c8.woff2`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/_next/static/media/roboto-vietnamese-400-normal.c95fc061.woff2` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/_next/static/media/roboto-vietnamese-400-normal.c95fc061.woff2`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/app/bridges/openon.html` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/app/bridges/openon.html`

 * *Files 3% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Open URL On - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/12f80ebf97adb4a5.css" as="style"/><link rel="stylesheet" href="/_next/static/css/12f80ebf97adb4a5.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-0eb9c66c948301b2.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-4dcb7f9b52833aba.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d073359675509c25.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-8433e2a32ffe1264.js" defer=""></script><script src="/_next/static/chunks/792-98bcf34693c3b84b.js" defer=""></script><script src="/_next/static/chunks/316-6f37cda59ad7df64.js" defer=""></script><script src="/_next/static/chunks/699-a9d1dd5afe8ccb50.js" defer=""></script><script src="/_next/static/chunks/154-539d3d9bf657b776.js" defer=""></script><script src="/_next/static/chunks/804-851168188e16a507.js" defer=""></script><script src="/_next/static/chunks/pages/app/bridges/openon-4be476ff83910730.js" defer=""></script><script src="/_next/static/XS-5P8XtA7Eb2ws6Mgd-Q/_buildManifest.js" defer=""></script><script src="/_next/static/XS-5P8XtA7Eb2ws6Mgd-Q/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css 1qsxih2">.css-1qsxih2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1qsxih2{padding-left:24px;padding-right:24px;}}@media (min-width:1200px){.css-1qsxih2{max-width:1200px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthLg css-1qsxih2"><style data-emotion="css jybjss">.css-jybjss{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;margin:80px 0px 64px;}</style><div class="MuiGrid-root MuiGrid-container css-jybjss"><style data-emotion="css a5m0jp animation-61bdi0">.css-a5m0jp{display:inline-block;color:#512da8;-webkit-animation:animation-61bdi0 1.4s linear infinite;animation:animation-61bdi0 1.4s linear infinite;}@-webkit-keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}@keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}</style><span class="MuiCircularProgress-root MuiCircularProgress-indeterminate MuiCircularProgress-colorPrimary css-a5m0jp" style="width:40px;height:40px" role="progressbar"><style data-emotion="css 13o7eu2">.css-13o7eu2{display:block;}</style><svg class="MuiCircularProgress-svg css-13o7eu2" viewBox="22 22 44 44"><style data-emotion="css 14891ef animation-1p2h4ri">.css-14891ef{stroke:currentColor;stroke-dasharray:80px,200px;stroke-dashoffset:0;-webkit-animation:animation-1p2h4ri 1.4s ease-in-out infinite;animation:animation-1p2h4ri 1.4s ease-in-out infinite;}@-webkit-keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}@keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}</style><circle class="MuiCircularProgress-circle MuiCircularProgress-circleIndeterminate css-14891ef" cx="44" cy="44" r="20.2" fill="none" stroke-width="3.6"></circle></svg></span></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/bridges/openon","query":{},"buildId":"XS-5P8XtA7Eb2ws6Mgd-Q","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Open URL On - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/12f80ebf97adb4a5.css" as="style"/><link rel="stylesheet" href="/_next/static/css/12f80ebf97adb4a5.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-0eb9c66c948301b2.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-4dcb7f9b52833aba.js" defer=""></script><script src="/_next/static/chunks/pages/_app-3c2428351a583313.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-12358b6301524be4.js" defer=""></script><script src="/_next/static/chunks/792-98bcf34693c3b84b.js" defer=""></script><script src="/_next/static/chunks/316-6f37cda59ad7df64.js" defer=""></script><script src="/_next/static/chunks/699-5a81a459894f5a37.js" defer=""></script><script src="/_next/static/chunks/154-539d3d9bf657b776.js" defer=""></script><script src="/_next/static/chunks/804-0a6dab4d173f5c2e.js" defer=""></script><script src="/_next/static/chunks/pages/app/bridges/openon-4be476ff83910730.js" defer=""></script><script src="/_next/static/sp5R1Ft1Y5yEAP_a5YQcA/_buildManifest.js" defer=""></script><script src="/_next/static/sp5R1Ft1Y5yEAP_a5YQcA/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css 1qsxih2">.css-1qsxih2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1qsxih2{padding-left:24px;padding-right:24px;}}@media (min-width:1200px){.css-1qsxih2{max-width:1200px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthLg css-1qsxih2"><style data-emotion="css jybjss">.css-jybjss{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;margin:80px 0px 64px;}</style><div class="MuiGrid-root MuiGrid-container css-jybjss"><style data-emotion="css a5m0jp animation-61bdi0">.css-a5m0jp{display:inline-block;color:#512da8;-webkit-animation:animation-61bdi0 1.4s linear infinite;animation:animation-61bdi0 1.4s linear infinite;}@-webkit-keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}@keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}</style><span class="MuiCircularProgress-root MuiCircularProgress-indeterminate MuiCircularProgress-colorPrimary css-a5m0jp" style="width:40px;height:40px" role="progressbar"><style data-emotion="css 13o7eu2">.css-13o7eu2{display:block;}</style><svg class="MuiCircularProgress-svg css-13o7eu2" viewBox="22 22 44 44"><style data-emotion="css 14891ef animation-1p2h4ri">.css-14891ef{stroke:currentColor;stroke-dasharray:80px,200px;stroke-dashoffset:0;-webkit-animation:animation-1p2h4ri 1.4s ease-in-out infinite;animation:animation-1p2h4ri 1.4s ease-in-out infinite;}@-webkit-keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}@keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}</style><circle class="MuiCircularProgress-circle MuiCircularProgress-circleIndeterminate css-14891ef" cx="44" cy="44" r="20.2" fill="none" stroke-width="3.6"></circle></svg></span></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/bridges/openon","query":{},"buildId":"sp5R1Ft1Y5yEAP_a5YQcA","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/app/bridges/setup.html` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/app/bridges/setup.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Bridges - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/12f80ebf97adb4a5.css" as="style"/><link rel="stylesheet" href="/_next/static/css/12f80ebf97adb4a5.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-0eb9c66c948301b2.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-4dcb7f9b52833aba.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d073359675509c25.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-8433e2a32ffe1264.js" defer=""></script><script src="/_next/static/chunks/792-98bcf34693c3b84b.js" defer=""></script><script src="/_next/static/chunks/316-6f37cda59ad7df64.js" defer=""></script><script src="/_next/static/chunks/699-a9d1dd5afe8ccb50.js" defer=""></script><script src="/_next/static/chunks/154-539d3d9bf657b776.js" defer=""></script><script src="/_next/static/chunks/767-9a32bf4c99b35e92.js" defer=""></script><script src="/_next/static/chunks/pages/app/bridges/setup-58dc331f38afcee4.js" defer=""></script><script src="/_next/static/XS-5P8XtA7Eb2ws6Mgd-Q/_buildManifest.js" defer=""></script><script src="/_next/static/XS-5P8XtA7Eb2ws6Mgd-Q/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css 1qsxih2">.css-1qsxih2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1qsxih2{padding-left:24px;padding-right:24px;}}@media (min-width:1200px){.css-1qsxih2{max-width:1200px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthLg css-1qsxih2"><style data-emotion="css jybjss">.css-jybjss{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;margin:80px 0px 64px;}</style><div class="MuiGrid-root MuiGrid-container css-jybjss"><style data-emotion="css a5m0jp animation-61bdi0">.css-a5m0jp{display:inline-block;color:#512da8;-webkit-animation:animation-61bdi0 1.4s linear infinite;animation:animation-61bdi0 1.4s linear infinite;}@-webkit-keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}@keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}</style><span class="MuiCircularProgress-root MuiCircularProgress-indeterminate MuiCircularProgress-colorPrimary css-a5m0jp" style="width:40px;height:40px" role="progressbar"><style data-emotion="css 13o7eu2">.css-13o7eu2{display:block;}</style><svg class="MuiCircularProgress-svg css-13o7eu2" viewBox="22 22 44 44"><style data-emotion="css 14891ef animation-1p2h4ri">.css-14891ef{stroke:currentColor;stroke-dasharray:80px,200px;stroke-dashoffset:0;-webkit-animation:animation-1p2h4ri 1.4s ease-in-out infinite;animation:animation-1p2h4ri 1.4s ease-in-out infinite;}@-webkit-keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}@keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}</style><circle class="MuiCircularProgress-circle MuiCircularProgress-circleIndeterminate css-14891ef" cx="44" cy="44" r="20.2" fill="none" stroke-width="3.6"></circle></svg></span></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/bridges/setup","query":{},"buildId":"XS-5P8XtA7Eb2ws6Mgd-Q","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Bridges - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/12f80ebf97adb4a5.css" as="style"/><link rel="stylesheet" href="/_next/static/css/12f80ebf97adb4a5.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-0eb9c66c948301b2.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-4dcb7f9b52833aba.js" defer=""></script><script src="/_next/static/chunks/pages/_app-3c2428351a583313.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-12358b6301524be4.js" defer=""></script><script src="/_next/static/chunks/792-98bcf34693c3b84b.js" defer=""></script><script src="/_next/static/chunks/316-6f37cda59ad7df64.js" defer=""></script><script src="/_next/static/chunks/699-5a81a459894f5a37.js" defer=""></script><script src="/_next/static/chunks/154-539d3d9bf657b776.js" defer=""></script><script src="/_next/static/chunks/767-9a32bf4c99b35e92.js" defer=""></script><script src="/_next/static/chunks/pages/app/bridges/setup-58dc331f38afcee4.js" defer=""></script><script src="/_next/static/sp5R1Ft1Y5yEAP_a5YQcA/_buildManifest.js" defer=""></script><script src="/_next/static/sp5R1Ft1Y5yEAP_a5YQcA/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css 1qsxih2">.css-1qsxih2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1qsxih2{padding-left:24px;padding-right:24px;}}@media (min-width:1200px){.css-1qsxih2{max-width:1200px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthLg css-1qsxih2"><style data-emotion="css jybjss">.css-jybjss{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;margin:80px 0px 64px;}</style><div class="MuiGrid-root MuiGrid-container css-jybjss"><style data-emotion="css a5m0jp animation-61bdi0">.css-a5m0jp{display:inline-block;color:#512da8;-webkit-animation:animation-61bdi0 1.4s linear infinite;animation:animation-61bdi0 1.4s linear infinite;}@-webkit-keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}@keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}</style><span class="MuiCircularProgress-root MuiCircularProgress-indeterminate MuiCircularProgress-colorPrimary css-a5m0jp" style="width:40px;height:40px" role="progressbar"><style data-emotion="css 13o7eu2">.css-13o7eu2{display:block;}</style><svg class="MuiCircularProgress-svg css-13o7eu2" viewBox="22 22 44 44"><style data-emotion="css 14891ef animation-1p2h4ri">.css-14891ef{stroke:currentColor;stroke-dasharray:80px,200px;stroke-dashoffset:0;-webkit-animation:animation-1p2h4ri 1.4s ease-in-out infinite;animation:animation-1p2h4ri 1.4s ease-in-out infinite;}@-webkit-keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}@keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}</style><circle class="MuiCircularProgress-circle MuiCircularProgress-circleIndeterminate css-14891ef" cx="44" cy="44" r="20.2" fill="none" stroke-width="3.6"></circle></svg></span></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/bridges/setup","query":{},"buildId":"sp5R1Ft1Y5yEAP_a5YQcA","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/app/data.html` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/app/data.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Data - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/12f80ebf97adb4a5.css" as="style"/><link rel="stylesheet" href="/_next/static/css/12f80ebf97adb4a5.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-0eb9c66c948301b2.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-4dcb7f9b52833aba.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d073359675509c25.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/29107295-661baa9a9eae34db.js" defer=""></script><script src="/_next/static/chunks/134-8433e2a32ffe1264.js" defer=""></script><script src="/_next/static/chunks/316-6f37cda59ad7df64.js" defer=""></script><script src="/_next/static/chunks/716-d1503f71e8e3fa88.js" defer=""></script><script src="/_next/static/chunks/pages/app/data-5b613fd056889656.js" defer=""></script><script src="/_next/static/XS-5P8XtA7Eb2ws6Mgd-Q/_buildManifest.js" defer=""></script><script src="/_next/static/XS-5P8XtA7Eb2ws6Mgd-Q/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css hnqd2s">.css-hnqd2s{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-hnqd2s{position:absolute;}}</style><style data-emotion="css 1gtczq1">.css-1gtczq1{background-color:#212121;color:#fff;-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:none;background-image:linear-gradient(rgba(255, 255, 255, 0), rgba(255, 255, 255, 0));display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-1gtczq1{position:absolute;}}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation0 MuiAppBar-root MuiAppBar-colorTransparent MuiAppBar-positionFixed mui-fixed css-1gtczq1"><style data-emotion="css 1wbqjz2">.css-1wbqjz2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;padding:0px;}@media (min-width:600px){.css-1wbqjz2{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1wbqjz2{max-width:1536px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthXl css-1wbqjz2"><style data-emotion="css y3hjov">.css-y3hjov{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;min-height:50px;max-height:50px;padding:0px;-webkit-flex:1;-ms-flex:1;flex:1;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:nowrap;-webkit-flex-wrap:nowrap;-ms-flex-wrap:nowrap;flex-wrap:nowrap;}@media (min-width:600px){.css-y3hjov{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-y3hjov{min-height:48px;}}}@media (min-width:600px){.css-y3hjov{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular css-y3hjov"><style data-emotion="css 1wxaqej">.css-1wxaqej{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}</style><div class="MuiGrid-root MuiGrid-item css-1wxaqej"><style data-emotion="css 1x6trl3">.css-1x6trl3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1x6trl3:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1x6trl3:hover{background-color:transparent;}}.css-1x6trl3.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 1o7udr7">.css-1o7udr7{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1o7udr7::-moz-focus-inner{border-style:none;}.css-1o7udr7.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-1o7udr7{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-1o7udr7:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1o7udr7:hover{background-color:transparent;}}.css-1o7udr7.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><a class="MuiButtonBase-root MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium css-1o7udr7" tabindex="0" href="https://system-bridge.timmo.dev" target="_blank"><style data-emotion="css 1lcbag5">.css-1lcbag5{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5625rem;line-height:1.235;letter-spacing:0.00735em;color:#fff;text-transform:none;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;}@media (min-width:600px){.css-1lcbag5{font-size:1.8219rem;}}@media (min-width:900px){.css-1lcbag5{font-size:2.0243rem;}}@media (min-width:1200px){.css-1lcbag5{font-size:2.0243rem;}}</style><div class="MuiTypography-root MuiTypography-h4 css-1lcbag5">System Bridge</div></a></div></div></div></header><style data-emotion="css 1pm3cft">.css-1pm3cft{height:144px;}</style><div class="MuiBox-root css-1pm3cft"></div><style data-emotion="css 1ekb41w">.css-1ekb41w{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1ekb41w{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1ekb41w{max-width:1536px;}}</style><article class="MuiContainer-root MuiContainer-maxWidthXl css-1ekb41w"><style data-emotion="css stiot1">.css-stiot1{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;margin-top:-16px;width:calc(100% + 16px);margin-left:-16px;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;padding:16px;}.css-stiot1>.MuiGrid-item{max-width:none;}.css-stiot1>.MuiGrid-item{padding-top:16px;}.css-stiot1>.MuiGrid-item{padding-left:16px;}</style><div class="MuiGrid-root MuiGrid-container MuiGrid-spacing-xs-2 MuiGrid-direction-xs-column css-stiot1"><style data-emotion="css 1ag80em">.css-1ag80em{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}@media (min-width:600px){.css-1ag80em{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:900px){.css-1ag80em{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:1200px){.css-1ag80em{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:1536px){.css-1ag80em{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}</style><div class="MuiGrid-root MuiGrid-container MuiGrid-item MuiGrid-grid-xs-true css-1ag80em"><style data-emotion="css 1wxaqej">.css-1wxaqej{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}</style><div class="MuiGrid-root MuiGrid-item css-1wxaqej"><style data-emotion="css 6x4ics">.css-6x4ics{overflow:hidden;min-height:48px;-webkit-overflow-scrolling:touch;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;}@media (max-width:599.95px){.css-6x4ics .MuiTabs-scrollButtons{display:none;}}</style><div class="MuiTabs-root MuiTabs-vertical css-6x4ics"><style data-emotion="css oqr85h">.css-oqr85h{overflow-x:auto;overflow-y:hidden;scrollbar-width:none;}.css-oqr85h::-webkit-scrollbar{display:none;}</style><div style="width:99px;height:99px;position:absolute;top:-9999px;overflow:scroll" class="MuiTabs-hideScrollbar css-oqr85h"></div><style data-emotion="css ccrt04">.css-ccrt04{position:relative;display:inline-block;-webkit-flex:1 1 auto;-ms-flex:1 1 auto;flex:1 1 auto;white-space:nowrap;scrollbar-width:none;overflow-y:auto;overflow-x:hidden;}.css-ccrt04::-webkit-scrollbar{display:none;}</style><div class="MuiTabs-scroller MuiTabs-hideScrollbar MuiTabs-scrollableY css-ccrt04" style="overflow:hidden;margin-right:0"><style data-emotion="css j7qwjs">.css-j7qwjs{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;}</style><div aria-orientation="vertical" class="MuiTabs-flexContainer MuiTabs-flexContainerVertical css-j7qwjs" role="tablist"><style data-emotion="css y235a3">.css-y235a3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.25;letter-spacing:0.02857em;text-transform:uppercase;max-width:360px;min-width:90px;position:relative;min-height:48px;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;padding:12px 16px;overflow:hidden;white-space:normal;text-align:center;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;color:rgba(255, 255, 255, 0.7);}.css-y235a3.Mui-selected{color:#512da8;}.css-y235a3.Mui-disabled{color:rgba(255, 255, 255, 0.5);}</style><style data-emotion="css yt5x7b">.css-yt5x7b{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.25;letter-spacing:0.02857em;text-transform:uppercase;max-width:360px;min-width:90px;position:relative;min-height:48px;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;padding:12px 16px;overflow:hidden;white-space:normal;text-align:center;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;color:rgba(255, 255, 255, 0.7);}.css-yt5x7b::-moz-focus-inner{border-style:none;}.css-yt5x7b.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-yt5x7b{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-yt5x7b.Mui-selected{color:#512da8;}.css-yt5x7b.Mui-disabled{color:rgba(255, 255, 255, 0.5);}</style><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary Mui-selected css-yt5x7b" tabindex="0" type="button" role="tab" aria-selected="true" id="scrollable-auto-tab-0" aria-controls="scrollable-auto-tabpanel-0">Battery<style data-emotion="css 14srzcc">.css-14srzcc{position:absolute;height:100%;bottom:0;width:2px;-webkit-transition:all 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:all 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;background-color:#512da8;right:0;}</style><span class="MuiTabs-indicator css-14srzcc"></span></button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-1" aria-controls="scrollable-auto-tabpanel-1">CPU</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-2" aria-controls="scrollable-auto-tabpanel-2">Disk</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-3" aria-controls="scrollable-auto-tabpanel-3">Display</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-4" aria-controls="scrollable-auto-tabpanel-4">GPU</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-5" aria-controls="scrollable-auto-tabpanel-5">Memory</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-6" aria-controls="scrollable-auto-tabpanel-6">Network</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-7" aria-controls="scrollable-auto-tabpanel-7">Sensors</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-8" aria-controls="scrollable-auto-tabpanel-8">System</button></div></div></div></div><style data-emotion="css kxu0dz">.css-kxu0dz{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}@media (min-width:600px){.css-kxu0dz{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:900px){.css-kxu0dz{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:1200px){.css-kxu0dz{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:1536px){.css-kxu0dz{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}</style><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-true css-kxu0dz"><style data-emotion="css iaoeqv">.css-iaoeqv{padding:16px;padding:24px 32px;}.css-iaoeqv:last-child{padding-bottom:24px;}.css-iaoeqv:last-child{padding-bottom:16px;}</style><div class="MuiCardContent-root css-iaoeqv"><style data-emotion="css 177hlju">.css-177hlju{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5625rem;line-height:1.235;letter-spacing:0.00735em;margin-bottom:0.35em;}@media (min-width:600px){.css-177hlju{font-size:1.8219rem;}}@media (min-width:900px){.css-177hlju{font-size:2.0243rem;}}@media (min-width:1200px){.css-177hlju{font-size:2.0243rem;}}</style><h3 class="MuiTypography-root MuiTypography-h4 MuiTypography-gutterBottom css-177hlju">Battery</h3></div></div></div></div></article></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/data","query":{},"buildId":"XS-5P8XtA7Eb2ws6Mgd-Q","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Data - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/12f80ebf97adb4a5.css" as="style"/><link rel="stylesheet" href="/_next/static/css/12f80ebf97adb4a5.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-0eb9c66c948301b2.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-4dcb7f9b52833aba.js" defer=""></script><script src="/_next/static/chunks/pages/_app-3c2428351a583313.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/29107295-661baa9a9eae34db.js" defer=""></script><script src="/_next/static/chunks/134-12358b6301524be4.js" defer=""></script><script src="/_next/static/chunks/316-6f37cda59ad7df64.js" defer=""></script><script src="/_next/static/chunks/716-d1503f71e8e3fa88.js" defer=""></script><script src="/_next/static/chunks/pages/app/data-5b613fd056889656.js" defer=""></script><script src="/_next/static/sp5R1Ft1Y5yEAP_a5YQcA/_buildManifest.js" defer=""></script><script src="/_next/static/sp5R1Ft1Y5yEAP_a5YQcA/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css hnqd2s">.css-hnqd2s{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-hnqd2s{position:absolute;}}</style><style data-emotion="css 1gtczq1">.css-1gtczq1{background-color:#212121;color:#fff;-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:none;background-image:linear-gradient(rgba(255, 255, 255, 0), rgba(255, 255, 255, 0));display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-1gtczq1{position:absolute;}}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation0 MuiAppBar-root MuiAppBar-colorTransparent MuiAppBar-positionFixed mui-fixed css-1gtczq1"><style data-emotion="css 1wbqjz2">.css-1wbqjz2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;padding:0px;}@media (min-width:600px){.css-1wbqjz2{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1wbqjz2{max-width:1536px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthXl css-1wbqjz2"><style data-emotion="css y3hjov">.css-y3hjov{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;min-height:50px;max-height:50px;padding:0px;-webkit-flex:1;-ms-flex:1;flex:1;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:nowrap;-webkit-flex-wrap:nowrap;-ms-flex-wrap:nowrap;flex-wrap:nowrap;}@media (min-width:600px){.css-y3hjov{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-y3hjov{min-height:48px;}}}@media (min-width:600px){.css-y3hjov{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular css-y3hjov"><style data-emotion="css 1wxaqej">.css-1wxaqej{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}</style><div class="MuiGrid-root MuiGrid-item css-1wxaqej"><style data-emotion="css 1x6trl3">.css-1x6trl3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1x6trl3:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1x6trl3:hover{background-color:transparent;}}.css-1x6trl3.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 1o7udr7">.css-1o7udr7{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1o7udr7::-moz-focus-inner{border-style:none;}.css-1o7udr7.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-1o7udr7{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-1o7udr7:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1o7udr7:hover{background-color:transparent;}}.css-1o7udr7.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><a class="MuiButtonBase-root MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium css-1o7udr7" tabindex="0" href="https://system-bridge.timmo.dev" target="_blank"><style data-emotion="css 1lcbag5">.css-1lcbag5{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5625rem;line-height:1.235;letter-spacing:0.00735em;color:#fff;text-transform:none;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;}@media (min-width:600px){.css-1lcbag5{font-size:1.8219rem;}}@media (min-width:900px){.css-1lcbag5{font-size:2.0243rem;}}@media (min-width:1200px){.css-1lcbag5{font-size:2.0243rem;}}</style><div class="MuiTypography-root MuiTypography-h4 css-1lcbag5">System Bridge</div></a></div></div></div></header><style data-emotion="css 1pm3cft">.css-1pm3cft{height:144px;}</style><div class="MuiBox-root css-1pm3cft"></div><style data-emotion="css 1ekb41w">.css-1ekb41w{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1ekb41w{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1ekb41w{max-width:1536px;}}</style><article class="MuiContainer-root MuiContainer-maxWidthXl css-1ekb41w"><style data-emotion="css stiot1">.css-stiot1{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;margin-top:-16px;width:calc(100% + 16px);margin-left:-16px;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;padding:16px;}.css-stiot1>.MuiGrid-item{max-width:none;}.css-stiot1>.MuiGrid-item{padding-top:16px;}.css-stiot1>.MuiGrid-item{padding-left:16px;}</style><div class="MuiGrid-root MuiGrid-container MuiGrid-spacing-xs-2 MuiGrid-direction-xs-column css-stiot1"><style data-emotion="css 1ag80em">.css-1ag80em{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}@media (min-width:600px){.css-1ag80em{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:900px){.css-1ag80em{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:1200px){.css-1ag80em{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:1536px){.css-1ag80em{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}</style><div class="MuiGrid-root MuiGrid-container MuiGrid-item MuiGrid-grid-xs-true css-1ag80em"><style data-emotion="css 1wxaqej">.css-1wxaqej{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}</style><div class="MuiGrid-root MuiGrid-item css-1wxaqej"><style data-emotion="css 6x4ics">.css-6x4ics{overflow:hidden;min-height:48px;-webkit-overflow-scrolling:touch;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;}@media (max-width:599.95px){.css-6x4ics .MuiTabs-scrollButtons{display:none;}}</style><div class="MuiTabs-root MuiTabs-vertical css-6x4ics"><style data-emotion="css oqr85h">.css-oqr85h{overflow-x:auto;overflow-y:hidden;scrollbar-width:none;}.css-oqr85h::-webkit-scrollbar{display:none;}</style><div style="width:99px;height:99px;position:absolute;top:-9999px;overflow:scroll" class="MuiTabs-hideScrollbar css-oqr85h"></div><style data-emotion="css ccrt04">.css-ccrt04{position:relative;display:inline-block;-webkit-flex:1 1 auto;-ms-flex:1 1 auto;flex:1 1 auto;white-space:nowrap;scrollbar-width:none;overflow-y:auto;overflow-x:hidden;}.css-ccrt04::-webkit-scrollbar{display:none;}</style><div class="MuiTabs-scroller MuiTabs-hideScrollbar MuiTabs-scrollableY css-ccrt04" style="overflow:hidden;margin-right:0"><style data-emotion="css j7qwjs">.css-j7qwjs{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;}</style><div aria-orientation="vertical" class="MuiTabs-flexContainer MuiTabs-flexContainerVertical css-j7qwjs" role="tablist"><style data-emotion="css y235a3">.css-y235a3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.25;letter-spacing:0.02857em;text-transform:uppercase;max-width:360px;min-width:90px;position:relative;min-height:48px;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;padding:12px 16px;overflow:hidden;white-space:normal;text-align:center;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;color:rgba(255, 255, 255, 0.7);}.css-y235a3.Mui-selected{color:#512da8;}.css-y235a3.Mui-disabled{color:rgba(255, 255, 255, 0.5);}</style><style data-emotion="css yt5x7b">.css-yt5x7b{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.25;letter-spacing:0.02857em;text-transform:uppercase;max-width:360px;min-width:90px;position:relative;min-height:48px;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;padding:12px 16px;overflow:hidden;white-space:normal;text-align:center;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;color:rgba(255, 255, 255, 0.7);}.css-yt5x7b::-moz-focus-inner{border-style:none;}.css-yt5x7b.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-yt5x7b{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-yt5x7b.Mui-selected{color:#512da8;}.css-yt5x7b.Mui-disabled{color:rgba(255, 255, 255, 0.5);}</style><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary Mui-selected css-yt5x7b" tabindex="0" type="button" role="tab" aria-selected="true" id="scrollable-auto-tab-0" aria-controls="scrollable-auto-tabpanel-0">Battery<style data-emotion="css 14srzcc">.css-14srzcc{position:absolute;height:100%;bottom:0;width:2px;-webkit-transition:all 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:all 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;background-color:#512da8;right:0;}</style><span class="MuiTabs-indicator css-14srzcc"></span></button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-1" aria-controls="scrollable-auto-tabpanel-1">CPU</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-2" aria-controls="scrollable-auto-tabpanel-2">Disk</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-3" aria-controls="scrollable-auto-tabpanel-3">Display</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-4" aria-controls="scrollable-auto-tabpanel-4">GPU</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-5" aria-controls="scrollable-auto-tabpanel-5">Memory</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-6" aria-controls="scrollable-auto-tabpanel-6">Network</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-7" aria-controls="scrollable-auto-tabpanel-7">Sensors</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-8" aria-controls="scrollable-auto-tabpanel-8">System</button></div></div></div></div><style data-emotion="css kxu0dz">.css-kxu0dz{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}@media (min-width:600px){.css-kxu0dz{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:900px){.css-kxu0dz{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:1200px){.css-kxu0dz{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:1536px){.css-kxu0dz{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}</style><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-true css-kxu0dz"><style data-emotion="css iaoeqv">.css-iaoeqv{padding:16px;padding:24px 32px;}.css-iaoeqv:last-child{padding-bottom:24px;}.css-iaoeqv:last-child{padding-bottom:16px;}</style><div class="MuiCardContent-root css-iaoeqv"><style data-emotion="css 177hlju">.css-177hlju{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5625rem;line-height:1.235;letter-spacing:0.00735em;margin-bottom:0.35em;}@media (min-width:600px){.css-177hlju{font-size:1.8219rem;}}@media (min-width:900px){.css-177hlju{font-size:2.0243rem;}}@media (min-width:1200px){.css-177hlju{font-size:2.0243rem;}}</style><h3 class="MuiTypography-root MuiTypography-h4 MuiTypography-gutterBottom css-177hlju">Battery</h3></div></div></div></div></article></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/data","query":{},"buildId":"sp5R1Ft1Y5yEAP_a5YQcA","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/app/notification.html` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/app/notification.html`

 * *Files 6% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Notification - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/12f80ebf97adb4a5.css" as="style"/><link rel="stylesheet" href="/_next/static/css/12f80ebf97adb4a5.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-0eb9c66c948301b2.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-4dcb7f9b52833aba.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d073359675509c25.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-8433e2a32ffe1264.js" defer=""></script><script src="/_next/static/chunks/154-539d3d9bf657b776.js" defer=""></script><script src="/_next/static/chunks/pages/app/notification-7c4c891692a1e4f4.js" defer=""></script><script src="/_next/static/XS-5P8XtA7Eb2ws6Mgd-Q/_buildManifest.js" defer=""></script><script src="/_next/static/XS-5P8XtA7Eb2ws6Mgd-Q/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css vvp5f9">.css-vvp5f9{text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-vvp5f9:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-vvp5f9:hover{background-color:transparent;}}.css-vvp5f9.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 17pbrtl">.css-17pbrtl{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-17pbrtl::-moz-focus-inner{border-style:none;}.css-17pbrtl.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-17pbrtl{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-17pbrtl:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-17pbrtl:hover{background-color:transparent;}}.css-17pbrtl.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><button class="MuiButtonBase-root MuiIconButton-root MuiIconButton-sizeSmall css-17pbrtl" tabindex="0" type="button"><svg viewBox="0 0 24 24" style="width:1.5rem;height:1.5rem" role="presentation"><path d="M19,6.41L17.59,5L12,10.59L6.41,5L5,6.41L10.59,12L5,17.59L6.41,19L12,13.41L17.59,19L19,17.59L13.41,12L19,6.41Z" style="fill:currentColor"></path></svg></button><style data-emotion="css tqjkiw">.css-tqjkiw{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-content:center;-ms-flex-line-pack:center;align-content:center;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;}</style><div class="MuiStack-root css-tqjkiw" style="height:100vh;width:100%;overflow:hidden"><style data-emotion="css 1vj4tmr">.css-1vj4tmr{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-align-content:center;-ms-flex-line-pack:center;align-content:center;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;}</style><div class="MuiStack-root css-1vj4tmr" style="padding:8px 8px 8px"><style data-emotion="css qtssx">.css-qtssx{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.25rem;line-height:1.334;letter-spacing:0em;margin:0px 8px;}@media (min-width:600px){.css-qtssx{font-size:1.3118rem;}}@media (min-width:900px){.css-qtssx{font-size:1.4993rem;}}@media (min-width:1200px){.css-qtssx{font-size:1.4993rem;}}</style><h1 class="MuiTypography-root MuiTypography-h5 css-qtssx"></h1></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/notification","query":{},"buildId":"XS-5P8XtA7Eb2ws6Mgd-Q","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Notification - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/12f80ebf97adb4a5.css" as="style"/><link rel="stylesheet" href="/_next/static/css/12f80ebf97adb4a5.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-0eb9c66c948301b2.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-4dcb7f9b52833aba.js" defer=""></script><script src="/_next/static/chunks/pages/_app-3c2428351a583313.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-12358b6301524be4.js" defer=""></script><script src="/_next/static/chunks/154-539d3d9bf657b776.js" defer=""></script><script src="/_next/static/chunks/pages/app/notification-7c4c891692a1e4f4.js" defer=""></script><script src="/_next/static/sp5R1Ft1Y5yEAP_a5YQcA/_buildManifest.js" defer=""></script><script src="/_next/static/sp5R1Ft1Y5yEAP_a5YQcA/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css vvp5f9">.css-vvp5f9{text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-vvp5f9:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-vvp5f9:hover{background-color:transparent;}}.css-vvp5f9.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 17pbrtl">.css-17pbrtl{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-17pbrtl::-moz-focus-inner{border-style:none;}.css-17pbrtl.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-17pbrtl{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-17pbrtl:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-17pbrtl:hover{background-color:transparent;}}.css-17pbrtl.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><button class="MuiButtonBase-root MuiIconButton-root MuiIconButton-sizeSmall css-17pbrtl" tabindex="0" type="button"><svg viewBox="0 0 24 24" style="width:1.5rem;height:1.5rem" role="presentation"><path d="M19,6.41L17.59,5L12,10.59L6.41,5L5,6.41L10.59,12L5,17.59L6.41,19L12,13.41L17.59,19L19,17.59L13.41,12L19,6.41Z" style="fill:currentColor"></path></svg></button><style data-emotion="css tqjkiw">.css-tqjkiw{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-content:center;-ms-flex-line-pack:center;align-content:center;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;}</style><div class="MuiStack-root css-tqjkiw" style="height:100vh;width:100%;overflow:hidden"><style data-emotion="css 1vj4tmr">.css-1vj4tmr{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-align-content:center;-ms-flex-line-pack:center;align-content:center;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;}</style><div class="MuiStack-root css-1vj4tmr" style="padding:8px 8px 8px"><style data-emotion="css qtssx">.css-qtssx{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.25rem;line-height:1.334;letter-spacing:0em;margin:0px 8px;}@media (min-width:600px){.css-qtssx{font-size:1.3118rem;}}@media (min-width:900px){.css-qtssx{font-size:1.4993rem;}}@media (min-width:1200px){.css-qtssx{font-size:1.4993rem;}}</style><h1 class="MuiTypography-root MuiTypography-h5 css-qtssx"></h1></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/notification","query":{},"buildId":"sp5R1Ft1Y5yEAP_a5YQcA","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/app/player/audio.html` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/app/player/video.html`

 * *Files 3% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Audio Player - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/12f80ebf97adb4a5.css" as="style"/><link rel="stylesheet" href="/_next/static/css/12f80ebf97adb4a5.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-0eb9c66c948301b2.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-4dcb7f9b52833aba.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d073359675509c25.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/29107295-661baa9a9eae34db.js" defer=""></script><script src="/_next/static/chunks/75fc9c18-25984afe689afff4.js" defer=""></script><script src="/_next/static/chunks/134-8433e2a32ffe1264.js" defer=""></script><script src="/_next/static/chunks/792-98bcf34693c3b84b.js" defer=""></script><script src="/_next/static/chunks/386-37509ae1b5f18ec9.js" defer=""></script><script src="/_next/static/chunks/142-595d06bd435adc4d.js" defer=""></script><script src="/_next/static/chunks/pages/app/player/audio-843238cdca1b0dca.js" defer=""></script><script src="/_next/static/XS-5P8XtA7Eb2ws6Mgd-Q/_buildManifest.js" defer=""></script><script src="/_next/static/XS-5P8XtA7Eb2ws6Mgd-Q/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css vvp5f9">.css-vvp5f9{text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-vvp5f9:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-vvp5f9:hover{background-color:transparent;}}.css-vvp5f9.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 17pbrtl">.css-17pbrtl{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-17pbrtl::-moz-focus-inner{border-style:none;}.css-17pbrtl.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-17pbrtl{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-17pbrtl:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-17pbrtl:hover{background-color:transparent;}}.css-17pbrtl.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><button class="MuiButtonBase-root MuiIconButton-root MuiIconButton-sizeSmall css-17pbrtl" tabindex="0" type="button"><svg viewBox="0 0 24 24" style="width:1.5rem;height:1.5rem" role="presentation"><path d="M19,6.41L17.59,5L12,10.59L6.41,5L5,6.41L10.59,12L5,17.59L6.41,19L12,13.41L17.59,19L19,17.59L13.41,12L19,6.41Z" style="fill:currentColor"></path></svg></button></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/player/audio","query":{},"buildId":"XS-5P8XtA7Eb2ws6Mgd-Q","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Video Player - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/12f80ebf97adb4a5.css" as="style"/><link rel="stylesheet" href="/_next/static/css/12f80ebf97adb4a5.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-0eb9c66c948301b2.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-4dcb7f9b52833aba.js" defer=""></script><script src="/_next/static/chunks/pages/_app-3c2428351a583313.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/29107295-661baa9a9eae34db.js" defer=""></script><script src="/_next/static/chunks/75fc9c18-25984afe689afff4.js" defer=""></script><script src="/_next/static/chunks/134-12358b6301524be4.js" defer=""></script><script src="/_next/static/chunks/792-98bcf34693c3b84b.js" defer=""></script><script src="/_next/static/chunks/386-37509ae1b5f18ec9.js" defer=""></script><script src="/_next/static/chunks/142-595d06bd435adc4d.js" defer=""></script><script src="/_next/static/chunks/pages/app/player/video-3aa85bafaac31d57.js" defer=""></script><script src="/_next/static/sp5R1Ft1Y5yEAP_a5YQcA/_buildManifest.js" defer=""></script><script src="/_next/static/sp5R1Ft1Y5yEAP_a5YQcA/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css vvp5f9">.css-vvp5f9{text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-vvp5f9:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-vvp5f9:hover{background-color:transparent;}}.css-vvp5f9.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 17pbrtl">.css-17pbrtl{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-17pbrtl::-moz-focus-inner{border-style:none;}.css-17pbrtl.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-17pbrtl{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-17pbrtl:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-17pbrtl:hover{background-color:transparent;}}.css-17pbrtl.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><button class="MuiButtonBase-root MuiIconButton-root MuiIconButton-sizeSmall css-17pbrtl" tabindex="0" type="button"><svg viewBox="0 0 24 24" style="width:1.5rem;height:1.5rem" role="presentation"><path d="M19,6.41L17.59,5L12,10.59L6.41,5L5,6.41L10.59,12L5,17.59L6.41,19L12,13.41L17.59,19L19,17.59L13.41,12L19,6.41Z" style="fill:currentColor"></path></svg></button></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/player/video","query":{},"buildId":"sp5R1Ft1Y5yEAP_a5YQcA","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/app/player/video.html` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/app/player/audio.html`

 * *Files 7% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Video Player - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/12f80ebf97adb4a5.css" as="style"/><link rel="stylesheet" href="/_next/static/css/12f80ebf97adb4a5.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-0eb9c66c948301b2.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-4dcb7f9b52833aba.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d073359675509c25.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/29107295-661baa9a9eae34db.js" defer=""></script><script src="/_next/static/chunks/75fc9c18-25984afe689afff4.js" defer=""></script><script src="/_next/static/chunks/134-8433e2a32ffe1264.js" defer=""></script><script src="/_next/static/chunks/792-98bcf34693c3b84b.js" defer=""></script><script src="/_next/static/chunks/386-37509ae1b5f18ec9.js" defer=""></script><script src="/_next/static/chunks/142-595d06bd435adc4d.js" defer=""></script><script src="/_next/static/chunks/pages/app/player/video-3aa85bafaac31d57.js" defer=""></script><script src="/_next/static/XS-5P8XtA7Eb2ws6Mgd-Q/_buildManifest.js" defer=""></script><script src="/_next/static/XS-5P8XtA7Eb2ws6Mgd-Q/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css vvp5f9">.css-vvp5f9{text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-vvp5f9:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-vvp5f9:hover{background-color:transparent;}}.css-vvp5f9.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 17pbrtl">.css-17pbrtl{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-17pbrtl::-moz-focus-inner{border-style:none;}.css-17pbrtl.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-17pbrtl{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-17pbrtl:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-17pbrtl:hover{background-color:transparent;}}.css-17pbrtl.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><button class="MuiButtonBase-root MuiIconButton-root MuiIconButton-sizeSmall css-17pbrtl" tabindex="0" type="button"><svg viewBox="0 0 24 24" style="width:1.5rem;height:1.5rem" role="presentation"><path d="M19,6.41L17.59,5L12,10.59L6.41,5L5,6.41L10.59,12L5,17.59L6.41,19L12,13.41L17.59,19L19,17.59L13.41,12L19,6.41Z" style="fill:currentColor"></path></svg></button></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/player/video","query":{},"buildId":"XS-5P8XtA7Eb2ws6Mgd-Q","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Audio Player - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/12f80ebf97adb4a5.css" as="style"/><link rel="stylesheet" href="/_next/static/css/12f80ebf97adb4a5.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-0eb9c66c948301b2.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-4dcb7f9b52833aba.js" defer=""></script><script src="/_next/static/chunks/pages/_app-3c2428351a583313.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/29107295-661baa9a9eae34db.js" defer=""></script><script src="/_next/static/chunks/75fc9c18-25984afe689afff4.js" defer=""></script><script src="/_next/static/chunks/134-12358b6301524be4.js" defer=""></script><script src="/_next/static/chunks/792-98bcf34693c3b84b.js" defer=""></script><script src="/_next/static/chunks/386-37509ae1b5f18ec9.js" defer=""></script><script src="/_next/static/chunks/142-595d06bd435adc4d.js" defer=""></script><script src="/_next/static/chunks/pages/app/player/audio-843238cdca1b0dca.js" defer=""></script><script src="/_next/static/sp5R1Ft1Y5yEAP_a5YQcA/_buildManifest.js" defer=""></script><script src="/_next/static/sp5R1Ft1Y5yEAP_a5YQcA/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css vvp5f9">.css-vvp5f9{text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-vvp5f9:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-vvp5f9:hover{background-color:transparent;}}.css-vvp5f9.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 17pbrtl">.css-17pbrtl{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-17pbrtl::-moz-focus-inner{border-style:none;}.css-17pbrtl.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-17pbrtl{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-17pbrtl:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-17pbrtl:hover{background-color:transparent;}}.css-17pbrtl.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><button class="MuiButtonBase-root MuiIconButton-root MuiIconButton-sizeSmall css-17pbrtl" tabindex="0" type="button"><svg viewBox="0 0 24 24" style="width:1.5rem;height:1.5rem" role="presentation"><path d="M19,6.41L17.59,5L12,10.59L6.41,5L5,6.41L10.59,12L5,17.59L6.41,19L12,13.41L17.59,19L19,17.59L13.41,12L19,6.41Z" style="fill:currentColor"></path></svg></button></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/player/audio","query":{},"buildId":"sp5R1Ft1Y5yEAP_a5YQcA","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/app/settings.html` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/app/settings.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Settings - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/12f80ebf97adb4a5.css" as="style"/><link rel="stylesheet" href="/_next/static/css/12f80ebf97adb4a5.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-0eb9c66c948301b2.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-4dcb7f9b52833aba.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d073359675509c25.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/29107295-661baa9a9eae34db.js" defer=""></script><script src="/_next/static/chunks/134-8433e2a32ffe1264.js" defer=""></script><script src="/_next/static/chunks/792-98bcf34693c3b84b.js" defer=""></script><script src="/_next/static/chunks/316-6f37cda59ad7df64.js" defer=""></script><script src="/_next/static/chunks/699-a9d1dd5afe8ccb50.js" defer=""></script><script src="/_next/static/chunks/804-851168188e16a507.js" defer=""></script><script src="/_next/static/chunks/767-9a32bf4c99b35e92.js" defer=""></script><script src="/_next/static/chunks/826-b7f8eabaf3afc6d5.js" defer=""></script><script src="/_next/static/chunks/pages/app/settings-c25cd256e27b2200.js" defer=""></script><script src="/_next/static/XS-5P8XtA7Eb2ws6Mgd-Q/_buildManifest.js" defer=""></script><script src="/_next/static/XS-5P8XtA7Eb2ws6Mgd-Q/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css hnqd2s">.css-hnqd2s{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-hnqd2s{position:absolute;}}</style><style data-emotion="css 1gtczq1">.css-1gtczq1{background-color:#212121;color:#fff;-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:none;background-image:linear-gradient(rgba(255, 255, 255, 0), rgba(255, 255, 255, 0));display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-1gtczq1{position:absolute;}}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation0 MuiAppBar-root MuiAppBar-colorTransparent MuiAppBar-positionFixed mui-fixed css-1gtczq1"><style data-emotion="css 1wbqjz2">.css-1wbqjz2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;padding:0px;}@media (min-width:600px){.css-1wbqjz2{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1wbqjz2{max-width:1536px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthXl css-1wbqjz2"><style data-emotion="css y3hjov">.css-y3hjov{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;min-height:50px;max-height:50px;padding:0px;-webkit-flex:1;-ms-flex:1;flex:1;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:nowrap;-webkit-flex-wrap:nowrap;-ms-flex-wrap:nowrap;flex-wrap:nowrap;}@media (min-width:600px){.css-y3hjov{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-y3hjov{min-height:48px;}}}@media (min-width:600px){.css-y3hjov{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular css-y3hjov"><style data-emotion="css 1wxaqej">.css-1wxaqej{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}</style><div class="MuiGrid-root MuiGrid-item css-1wxaqej"><style data-emotion="css 1x6trl3">.css-1x6trl3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1x6trl3:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1x6trl3:hover{background-color:transparent;}}.css-1x6trl3.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 1o7udr7">.css-1o7udr7{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1o7udr7::-moz-focus-inner{border-style:none;}.css-1o7udr7.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-1o7udr7{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-1o7udr7:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1o7udr7:hover{background-color:transparent;}}.css-1o7udr7.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><a class="MuiButtonBase-root MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium css-1o7udr7" tabindex="0" href="https://system-bridge.timmo.dev" target="_blank"><style data-emotion="css 1lcbag5">.css-1lcbag5{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5625rem;line-height:1.235;letter-spacing:0.00735em;color:#fff;text-transform:none;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;}@media (min-width:600px){.css-1lcbag5{font-size:1.8219rem;}}@media (min-width:900px){.css-1lcbag5{font-size:2.0243rem;}}@media (min-width:1200px){.css-1lcbag5{font-size:2.0243rem;}}</style><div class="MuiTypography-root MuiTypography-h4 css-1lcbag5">System Bridge</div></a></div></div></div></header><style data-emotion="css 1pm3cft">.css-1pm3cft{height:144px;}</style><div class="MuiBox-root css-1pm3cft"></div><style data-emotion="css 1ekb41w">.css-1ekb41w{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1ekb41w{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1ekb41w{max-width:1536px;}}</style><article class="MuiContainer-root MuiContainer-maxWidthXl css-1ekb41w"><style data-emotion="css hm04cy">.css-hm04cy{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;margin-top:-16px;width:calc(100% + 16px);margin-left:-16px;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;margin-bottom:64px;padding:16px;}.css-hm04cy>.MuiGrid-item{max-width:none;}.css-hm04cy>.MuiGrid-item{padding-top:16px;}.css-hm04cy>.MuiGrid-item{padding-left:16px;}</style><div class="MuiGrid-root MuiGrid-container MuiGrid-spacing-xs-2 MuiGrid-direction-xs-column css-hm04cy"><style data-emotion="css 8uezpq">.css-8uezpq{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;margin:16px 0px 80px;}</style><div class="MuiGrid-root MuiGrid-container css-8uezpq"><style data-emotion="css a5m0jp animation-61bdi0">.css-a5m0jp{display:inline-block;color:#512da8;-webkit-animation:animation-61bdi0 1.4s linear infinite;animation:animation-61bdi0 1.4s linear infinite;}@-webkit-keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}@keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}</style><span class="MuiCircularProgress-root MuiCircularProgress-indeterminate MuiCircularProgress-colorPrimary css-a5m0jp" style="width:40px;height:40px" role="progressbar"><style data-emotion="css 13o7eu2">.css-13o7eu2{display:block;}</style><svg class="MuiCircularProgress-svg css-13o7eu2" viewBox="22 22 44 44"><style data-emotion="css 14891ef animation-1p2h4ri">.css-14891ef{stroke:currentColor;stroke-dasharray:80px,200px;stroke-dashoffset:0;-webkit-animation:animation-1p2h4ri 1.4s ease-in-out infinite;animation:animation-1p2h4ri 1.4s ease-in-out infinite;}@-webkit-keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}@keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}</style><circle class="MuiCircularProgress-circle MuiCircularProgress-circleIndeterminate css-14891ef" cx="44" cy="44" r="20.2" fill="none" stroke-width="3.6"></circle></svg></span></div></div></article></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/settings","query":{},"buildId":"XS-5P8XtA7Eb2ws6Mgd-Q","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Settings - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/12f80ebf97adb4a5.css" as="style"/><link rel="stylesheet" href="/_next/static/css/12f80ebf97adb4a5.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-0eb9c66c948301b2.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-4dcb7f9b52833aba.js" defer=""></script><script src="/_next/static/chunks/pages/_app-3c2428351a583313.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/29107295-661baa9a9eae34db.js" defer=""></script><script src="/_next/static/chunks/134-12358b6301524be4.js" defer=""></script><script src="/_next/static/chunks/792-98bcf34693c3b84b.js" defer=""></script><script src="/_next/static/chunks/316-6f37cda59ad7df64.js" defer=""></script><script src="/_next/static/chunks/699-5a81a459894f5a37.js" defer=""></script><script src="/_next/static/chunks/804-0a6dab4d173f5c2e.js" defer=""></script><script src="/_next/static/chunks/767-9a32bf4c99b35e92.js" defer=""></script><script src="/_next/static/chunks/826-b7f8eabaf3afc6d5.js" defer=""></script><script src="/_next/static/chunks/pages/app/settings-c25cd256e27b2200.js" defer=""></script><script src="/_next/static/sp5R1Ft1Y5yEAP_a5YQcA/_buildManifest.js" defer=""></script><script src="/_next/static/sp5R1Ft1Y5yEAP_a5YQcA/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css hnqd2s">.css-hnqd2s{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-hnqd2s{position:absolute;}}</style><style data-emotion="css 1gtczq1">.css-1gtczq1{background-color:#212121;color:#fff;-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:none;background-image:linear-gradient(rgba(255, 255, 255, 0), rgba(255, 255, 255, 0));display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-1gtczq1{position:absolute;}}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation0 MuiAppBar-root MuiAppBar-colorTransparent MuiAppBar-positionFixed mui-fixed css-1gtczq1"><style data-emotion="css 1wbqjz2">.css-1wbqjz2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;padding:0px;}@media (min-width:600px){.css-1wbqjz2{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1wbqjz2{max-width:1536px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthXl css-1wbqjz2"><style data-emotion="css y3hjov">.css-y3hjov{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;min-height:50px;max-height:50px;padding:0px;-webkit-flex:1;-ms-flex:1;flex:1;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:nowrap;-webkit-flex-wrap:nowrap;-ms-flex-wrap:nowrap;flex-wrap:nowrap;}@media (min-width:600px){.css-y3hjov{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-y3hjov{min-height:48px;}}}@media (min-width:600px){.css-y3hjov{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular css-y3hjov"><style data-emotion="css 1wxaqej">.css-1wxaqej{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}</style><div class="MuiGrid-root MuiGrid-item css-1wxaqej"><style data-emotion="css 1x6trl3">.css-1x6trl3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1x6trl3:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1x6trl3:hover{background-color:transparent;}}.css-1x6trl3.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 1o7udr7">.css-1o7udr7{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1o7udr7::-moz-focus-inner{border-style:none;}.css-1o7udr7.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-1o7udr7{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-1o7udr7:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1o7udr7:hover{background-color:transparent;}}.css-1o7udr7.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><a class="MuiButtonBase-root MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium css-1o7udr7" tabindex="0" href="https://system-bridge.timmo.dev" target="_blank"><style data-emotion="css 1lcbag5">.css-1lcbag5{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5625rem;line-height:1.235;letter-spacing:0.00735em;color:#fff;text-transform:none;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;}@media (min-width:600px){.css-1lcbag5{font-size:1.8219rem;}}@media (min-width:900px){.css-1lcbag5{font-size:2.0243rem;}}@media (min-width:1200px){.css-1lcbag5{font-size:2.0243rem;}}</style><div class="MuiTypography-root MuiTypography-h4 css-1lcbag5">System Bridge</div></a></div></div></div></header><style data-emotion="css 1pm3cft">.css-1pm3cft{height:144px;}</style><div class="MuiBox-root css-1pm3cft"></div><style data-emotion="css 1ekb41w">.css-1ekb41w{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1ekb41w{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1ekb41w{max-width:1536px;}}</style><article class="MuiContainer-root MuiContainer-maxWidthXl css-1ekb41w"><style data-emotion="css hm04cy">.css-hm04cy{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;margin-top:-16px;width:calc(100% + 16px);margin-left:-16px;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;margin-bottom:64px;padding:16px;}.css-hm04cy>.MuiGrid-item{max-width:none;}.css-hm04cy>.MuiGrid-item{padding-top:16px;}.css-hm04cy>.MuiGrid-item{padding-left:16px;}</style><div class="MuiGrid-root MuiGrid-container MuiGrid-spacing-xs-2 MuiGrid-direction-xs-column css-hm04cy"><style data-emotion="css 8uezpq">.css-8uezpq{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;margin:16px 0px 80px;}</style><div class="MuiGrid-root MuiGrid-container css-8uezpq"><style data-emotion="css a5m0jp animation-61bdi0">.css-a5m0jp{display:inline-block;color:#512da8;-webkit-animation:animation-61bdi0 1.4s linear infinite;animation:animation-61bdi0 1.4s linear infinite;}@-webkit-keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}@keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}</style><span class="MuiCircularProgress-root MuiCircularProgress-indeterminate MuiCircularProgress-colorPrimary css-a5m0jp" style="width:40px;height:40px" role="progressbar"><style data-emotion="css 13o7eu2">.css-13o7eu2{display:block;}</style><svg class="MuiCircularProgress-svg css-13o7eu2" viewBox="22 22 44 44"><style data-emotion="css 14891ef animation-1p2h4ri">.css-14891ef{stroke:currentColor;stroke-dasharray:80px,200px;stroke-dashoffset:0;-webkit-animation:animation-1p2h4ri 1.4s ease-in-out infinite;animation:animation-1p2h4ri 1.4s ease-in-out infinite;}@-webkit-keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}@keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}</style><circle class="MuiCircularProgress-circle MuiCircularProgress-circleIndeterminate css-14891ef" cx="44" cy="44" r="20.2" fill="none" stroke-width="3.6"></circle></svg></span></div></div></article></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/settings","query":{},"buildId":"sp5R1Ft1Y5yEAP_a5YQcA","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/favicon.svg` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/favicon.svg`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend/out/index.html` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend/out/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Placeholder - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/12f80ebf97adb4a5.css" as="style"/><link rel="stylesheet" href="/_next/static/css/12f80ebf97adb4a5.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-0eb9c66c948301b2.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-4dcb7f9b52833aba.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d073359675509c25.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-8433e2a32ffe1264.js" defer=""></script><script src="/_next/static/chunks/pages/index-f934b9a030f633a0.js" defer=""></script><script src="/_next/static/XS-5P8XtA7Eb2ws6Mgd-Q/_buildManifest.js" defer=""></script><script src="/_next/static/XS-5P8XtA7Eb2ws6Mgd-Q/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css hnqd2s">.css-hnqd2s{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-hnqd2s{position:absolute;}}</style><style data-emotion="css 1gtczq1">.css-1gtczq1{background-color:#212121;color:#fff;-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:none;background-image:linear-gradient(rgba(255, 255, 255, 0), rgba(255, 255, 255, 0));display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-1gtczq1{position:absolute;}}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation0 MuiAppBar-root MuiAppBar-colorTransparent MuiAppBar-positionFixed mui-fixed css-1gtczq1"><style data-emotion="css 1wbqjz2">.css-1wbqjz2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;padding:0px;}@media (min-width:600px){.css-1wbqjz2{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1wbqjz2{max-width:1536px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthXl css-1wbqjz2"><style data-emotion="css y3hjov">.css-y3hjov{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;min-height:50px;max-height:50px;padding:0px;-webkit-flex:1;-ms-flex:1;flex:1;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:nowrap;-webkit-flex-wrap:nowrap;-ms-flex-wrap:nowrap;flex-wrap:nowrap;}@media (min-width:600px){.css-y3hjov{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-y3hjov{min-height:48px;}}}@media (min-width:600px){.css-y3hjov{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular css-y3hjov"><style data-emotion="css 1wxaqej">.css-1wxaqej{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}</style><div class="MuiGrid-root MuiGrid-item css-1wxaqej"><style data-emotion="css 1x6trl3">.css-1x6trl3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1x6trl3:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1x6trl3:hover{background-color:transparent;}}.css-1x6trl3.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 1o7udr7">.css-1o7udr7{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1o7udr7::-moz-focus-inner{border-style:none;}.css-1o7udr7.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-1o7udr7{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-1o7udr7:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1o7udr7:hover{background-color:transparent;}}.css-1o7udr7.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><a class="MuiButtonBase-root MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium css-1o7udr7" tabindex="0" href="https://system-bridge.timmo.dev" target="_blank"><style data-emotion="css 1lcbag5">.css-1lcbag5{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5625rem;line-height:1.235;letter-spacing:0.00735em;color:#fff;text-transform:none;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;}@media (min-width:600px){.css-1lcbag5{font-size:1.8219rem;}}@media (min-width:900px){.css-1lcbag5{font-size:2.0243rem;}}@media (min-width:1200px){.css-1lcbag5{font-size:2.0243rem;}}</style><div class="MuiTypography-root MuiTypography-h4 css-1lcbag5">System Bridge</div></a></div></div></div></header><style data-emotion="css 1pm3cft">.css-1pm3cft{height:144px;}</style><div class="MuiBox-root css-1pm3cft"></div><style data-emotion="css 1ekb41w">.css-1ekb41w{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1ekb41w{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1ekb41w{max-width:1536px;}}</style><article class="MuiContainer-root MuiContainer-maxWidthXl css-1ekb41w"></article></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"XS-5P8XtA7Eb2ws6Mgd-Q","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Placeholder - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/12f80ebf97adb4a5.css" as="style"/><link rel="stylesheet" href="/_next/static/css/12f80ebf97adb4a5.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js"></script><script src="/_next/static/chunks/webpack-0eb9c66c948301b2.js" defer=""></script><script src="/_next/static/chunks/framework-2c79e2a64abdb08b.js" defer=""></script><script src="/_next/static/chunks/main-4dcb7f9b52833aba.js" defer=""></script><script src="/_next/static/chunks/pages/_app-3c2428351a583313.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-12358b6301524be4.js" defer=""></script><script src="/_next/static/chunks/pages/index-f934b9a030f633a0.js" defer=""></script><script src="/_next/static/sp5R1Ft1Y5yEAP_a5YQcA/_buildManifest.js" defer=""></script><script src="/_next/static/sp5R1Ft1Y5yEAP_a5YQcA/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css hnqd2s">.css-hnqd2s{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-hnqd2s{position:absolute;}}</style><style data-emotion="css 1gtczq1">.css-1gtczq1{background-color:#212121;color:#fff;-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:none;background-image:linear-gradient(rgba(255, 255, 255, 0), rgba(255, 255, 255, 0));display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-1gtczq1{position:absolute;}}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation0 MuiAppBar-root MuiAppBar-colorTransparent MuiAppBar-positionFixed mui-fixed css-1gtczq1"><style data-emotion="css 1wbqjz2">.css-1wbqjz2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;padding:0px;}@media (min-width:600px){.css-1wbqjz2{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1wbqjz2{max-width:1536px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthXl css-1wbqjz2"><style data-emotion="css y3hjov">.css-y3hjov{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;min-height:50px;max-height:50px;padding:0px;-webkit-flex:1;-ms-flex:1;flex:1;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:nowrap;-webkit-flex-wrap:nowrap;-ms-flex-wrap:nowrap;flex-wrap:nowrap;}@media (min-width:600px){.css-y3hjov{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-y3hjov{min-height:48px;}}}@media (min-width:600px){.css-y3hjov{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular css-y3hjov"><style data-emotion="css 1wxaqej">.css-1wxaqej{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}</style><div class="MuiGrid-root MuiGrid-item css-1wxaqej"><style data-emotion="css 1x6trl3">.css-1x6trl3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1x6trl3:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1x6trl3:hover{background-color:transparent;}}.css-1x6trl3.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 1o7udr7">.css-1o7udr7{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1o7udr7::-moz-focus-inner{border-style:none;}.css-1o7udr7.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-1o7udr7{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-1o7udr7:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1o7udr7:hover{background-color:transparent;}}.css-1o7udr7.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><a class="MuiButtonBase-root MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium css-1o7udr7" tabindex="0" href="https://system-bridge.timmo.dev" target="_blank"><style data-emotion="css 1lcbag5">.css-1lcbag5{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5625rem;line-height:1.235;letter-spacing:0.00735em;color:#fff;text-transform:none;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;}@media (min-width:600px){.css-1lcbag5{font-size:1.8219rem;}}@media (min-width:900px){.css-1lcbag5{font-size:2.0243rem;}}@media (min-width:1200px){.css-1lcbag5{font-size:2.0243rem;}}</style><div class="MuiTypography-root MuiTypography-h4 css-1lcbag5">System Bridge</div></a></div></div></div></header><style data-emotion="css 1pm3cft">.css-1pm3cft{height:144px;}</style><div class="MuiBox-root css-1pm3cft"></div><style data-emotion="css 1ekb41w">.css-1ekb41w{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1ekb41w{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1ekb41w{max-width:1536px;}}</style><article class="MuiContainer-root MuiContainer-maxWidthXl css-1ekb41w"></article></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"sp5R1Ft1Y5yEAP_a5YQcA","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.6.3.dev6/systembridgefrontend.egg-info/SOURCES.txt` & `systembridgefrontend-3.6.3.dev7/systembridgefrontend.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,27 @@
 systembridgefrontend.egg-info/PKG-INFO
 systembridgefrontend.egg-info/SOURCES.txt
 systembridgefrontend.egg-info/dependency_links.txt
 systembridgefrontend.egg-info/top_level.txt
 systembridgefrontend/out/404.html
 systembridgefrontend/out/favicon.svg
 systembridgefrontend/out/index.html
-systembridgefrontend/out/_next/static/XS-5P8XtA7Eb2ws6Mgd-Q/_buildManifest.js
-systembridgefrontend/out/_next/static/XS-5P8XtA7Eb2ws6Mgd-Q/_ssgManifest.js
-systembridgefrontend/out/_next/static/chunks/134-8433e2a32ffe1264.js
+systembridgefrontend/out/_next/static/chunks/134-12358b6301524be4.js
 systembridgefrontend/out/_next/static/chunks/142-595d06bd435adc4d.js
 systembridgefrontend/out/_next/static/chunks/154-539d3d9bf657b776.js
 systembridgefrontend/out/_next/static/chunks/171.d9b946d3f22277f9.js
 systembridgefrontend/out/_next/static/chunks/29107295-661baa9a9eae34db.js
 systembridgefrontend/out/_next/static/chunks/316-6f37cda59ad7df64.js
 systembridgefrontend/out/_next/static/chunks/386-37509ae1b5f18ec9.js
-systembridgefrontend/out/_next/static/chunks/699-a9d1dd5afe8ccb50.js
+systembridgefrontend/out/_next/static/chunks/699-5a81a459894f5a37.js
 systembridgefrontend/out/_next/static/chunks/716-d1503f71e8e3fa88.js
 systembridgefrontend/out/_next/static/chunks/75fc9c18-25984afe689afff4.js
 systembridgefrontend/out/_next/static/chunks/767-9a32bf4c99b35e92.js
 systembridgefrontend/out/_next/static/chunks/792-98bcf34693c3b84b.js
-systembridgefrontend/out/_next/static/chunks/804-851168188e16a507.js
+systembridgefrontend/out/_next/static/chunks/804-0a6dab4d173f5c2e.js
 systembridgefrontend/out/_next/static/chunks/826-b7f8eabaf3afc6d5.js
 systembridgefrontend/out/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js
 systembridgefrontend/out/_next/static/chunks/framework-2c79e2a64abdb08b.js
 systembridgefrontend/out/_next/static/chunks/main-4dcb7f9b52833aba.js
 systembridgefrontend/out/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerDailyMotion.da042b36db7662eb.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerFacebook.3663ffcf10139668.js
@@ -39,15 +37,15 @@
 systembridgefrontend/out/_next/static/chunks/reactPlayerStreamable.c374322fbd4a05d5.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerTwitch.52035ec5fd363953.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerVidyard.8c3ec4a7a5b4aac4.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerVimeo.5a5700a7f86e58a2.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerWistia.29aa97668baf75ea.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerYouTube.77a6d75e3f5e95ef.js
 systembridgefrontend/out/_next/static/chunks/webpack-0eb9c66c948301b2.js
-systembridgefrontend/out/_next/static/chunks/pages/_app-d073359675509c25.js
+systembridgefrontend/out/_next/static/chunks/pages/_app-3c2428351a583313.js
 systembridgefrontend/out/_next/static/chunks/pages/_error-54de1933a164a1ff.js
 systembridgefrontend/out/_next/static/chunks/pages/index-f934b9a030f633a0.js
 systembridgefrontend/out/_next/static/chunks/pages/app/data-5b613fd056889656.js
 systembridgefrontend/out/_next/static/chunks/pages/app/notification-7c4c891692a1e4f4.js
 systembridgefrontend/out/_next/static/chunks/pages/app/settings-c25cd256e27b2200.js
 systembridgefrontend/out/_next/static/chunks/pages/app/bridges/openon-4be476ff83910730.js
 systembridgefrontend/out/_next/static/chunks/pages/app/bridges/setup-58dc331f38afcee4.js
@@ -58,14 +56,16 @@
 systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.2d9c9d60.woff2
 systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.d7827ae3.woff2
 systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.63e6dc18.woff2
 systembridgefrontend/out/_next/static/media/roboto-greek-ext-400-normal.2b547ded.woff2
 systembridgefrontend/out/_next/static/media/roboto-latin-400-normal.f2894edc.woff2
 systembridgefrontend/out/_next/static/media/roboto-latin-ext-400-normal.21abc8c8.woff2
 systembridgefrontend/out/_next/static/media/roboto-vietnamese-400-normal.c95fc061.woff2
+systembridgefrontend/out/_next/static/sp5R1Ft1Y5yEAP_a5YQcA/_buildManifest.js
+systembridgefrontend/out/_next/static/sp5R1Ft1Y5yEAP_a5YQcA/_ssgManifest.js
 systembridgefrontend/out/app/data.html
 systembridgefrontend/out/app/notification.html
 systembridgefrontend/out/app/settings.html
 systembridgefrontend/out/app/bridges/openon.html
 systembridgefrontend/out/app/bridges/setup.html
 systembridgefrontend/out/app/player/audio.html
 systembridgefrontend/out/app/player/video.html
```

