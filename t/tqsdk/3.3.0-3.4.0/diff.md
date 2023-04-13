# Comparing `tmp/tqsdk-3.3.0.tar.gz` & `tmp/tqsdk-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tqsdk-3.3.0.tar", last modified: Tue Nov 22 08:53:34 2022, max compression
+gzip compressed data, was "dist/tqsdk-3.4.0.tar", last modified: Thu Apr 13 07:33:18 2023, max compression
```

## Comparing `tqsdk-3.3.0.tar` & `tqsdk-3.4.0.tar`

### file list

```diff
@@ -1,200 +1,200 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 08:53:34.000000 tqsdk-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11335 2022-11-22 08:52:35.000000 tqsdk-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-11-22 08:53:34.000000 tqsdk-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5278 2022-11-22 08:52:35.000000 tqsdk-3.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-11-22 08:52:35.000000 tqsdk-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2247 2022-11-22 08:52:35.000000 tqsdk-3.3.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     5725 2022-11-22 08:53:34.000000 tqsdk-3.3.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 08:53:34.000000 tqsdk-3.3.0/tqsdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-22 08:53:34.000000 tqsdk-3.3.0/tqsdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-11-22 08:53:34.000000 tqsdk-3.3.0/tqsdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-22 08:53:34.000000 tqsdk-3.3.0/tqsdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5284 2022-11-22 08:53:34.000000 tqsdk-3.3.0/tqsdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-22 08:53:34.000000 tqsdk-3.3.0/tqsdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)     5725 2022-11-22 08:53:34.000000 tqsdk-3.3.0/tqsdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-22 08:53:34.000000 tqsdk-3.3.0/tqsdk.egg-info/entry_points.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 08:53:34.000000 tqsdk-3.3.0/tqsdk/
--rw-r--r--   0 runner    (1001) docker     (121)    20372 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/objs_not_entity.py
--rw-r--r--   0 runner    (1001) docker     (121)    12660 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/risk_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 08:53:34.000000 tqsdk-3.3.0/tqsdk/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/__pyinstaller/hook-tqsdk.py
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3270 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/trading_status.py
--rw-r--r--   0 runner    (1001) docker     (121)    52985 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/tafunc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 08:53:34.000000 tqsdk-3.3.0/tqsdk/lib/
--rw-r--r--   0 runner    (1001) docker     (121)    10550 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/lib/target_pos_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (121)     4674 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2196 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/lib/notify.py
--rw-r--r--   0 runner    (1001) docker     (121)    38277 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/lib/target_pos_task.py
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20805 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/connect.py
--rw-r--r--   0 runner    (1001) docker     (121)     6099 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/stockprofit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 08:53:34.000000 tqsdk-3.3.0/tqsdk/tradeable/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 08:53:34.000000 tqsdk-3.3.0/tqsdk/tradeable/sim/
--rw-r--r--   0 runner    (1001) docker     (121)    18113 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/tradeable/sim/basesim.py
--rw-r--r--   0 runner    (1001) docker     (121)    11943 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/tradeable/sim/trade_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     8523 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/tradeable/sim/tqsim_stock.py
--rw-r--r--   0 runner    (1001) docker     (121)    35956 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/tradeable/sim/trade_future.py
--rw-r--r--   0 runner    (1001) docker     (121)     5083 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/tradeable/sim/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    27585 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/tradeable/sim/trade_stock.py
--rw-r--r--   0 runner    (1001) docker     (121)    10665 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/tradeable/sim/tqsim.py
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/tradeable/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15130 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/tradeable/mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/tradeable/tradeable.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 08:53:34.000000 tqsdk-3.3.0/tqsdk/tradeable/otg/
--rw-r--r--   0 runner    (1001) docker     (121)     4640 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/tradeable/otg/tqaccount.py
--rw-r--r--   0 runner    (1001) docker     (121)     3794 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/tradeable/otg/tqkq.py
--rw-r--r--   0 runner    (1001) docker     (121)     4259 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/tradeable/otg/base_otg.py
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/tradeable/otg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/tradeable/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 08:53:34.000000 tqsdk-3.3.0/tqsdk/tools/
--rw-r--r--   0 runner    (1001) docker     (121)    22148 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/tools/downloader.py
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/tools/dead_ins.lzma
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 08:53:34.000000 tqsdk-3.3.0/tqsdk/backtest/
--rw-r--r--   0 runner    (1001) docker     (121)     4816 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/backtest/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    42136 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/backtest/backtest.py
--rw-r--r--   0 runner    (1001) docker     (121)     6687 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/backtest/replay.py
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/backtest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6864 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/rangeset.py
--rw-r--r--   0 runner    (1001) docker     (121)     9392 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/trade_extension.py
--rw-r--r--   0 runner    (1001) docker     (121)     1769 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/log.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 08:53:34.000000 tqsdk-3.3.0/tqsdk/web/
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-11-22 08:52:36.000000 tqsdk-3.3.0/tqsdk/web/service-worker.js
--rw-r--r--   0 runner    (1001) docker     (121)     3153 2022-11-22 08:52:36.000000 tqsdk-3.3.0/tqsdk/web/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)     2095 2022-11-22 08:52:36.000000 tqsdk-3.3.0/tqsdk/web/index.html
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-11-22 08:52:36.000000 tqsdk-3.3.0/tqsdk/web/manifest.json
--rw-r--r--   0 runner    (1001) docker     (121)   246120 2022-11-22 08:52:36.000000 tqsdk-3.3.0/tqsdk/web/d3.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     1216 2022-11-22 08:52:36.000000 tqsdk-3.3.0/tqsdk/web/precache-manifest.7ed60b69dab01cdb0c64836489ab6e0d.js
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-22 08:52:36.000000 tqsdk-3.3.0/tqsdk/web/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 08:53:34.000000 tqsdk-3.3.0/tqsdk/web/css/
--rw-r--r--   0 runner    (1001) docker     (121)   279508 2022-11-22 08:52:36.000000 tqsdk-3.3.0/tqsdk/web/css/chunk-vendors.c93e9127.css
--rw-r--r--   0 runner    (1001) docker     (121)     5764 2022-11-22 08:52:36.000000 tqsdk-3.3.0/tqsdk/web/css/app.d72d8978.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 08:53:34.000000 tqsdk-3.3.0/tqsdk/web/fonts/
--rw-r--r--   0 runner    (1001) docker     (121)   197664 2022-11-22 08:52:36.000000 tqsdk-3.3.0/tqsdk/web/fonts/ionicons.d535a25a.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    82216 2022-11-22 08:52:36.000000 tqsdk-3.3.0/tqsdk/web/fonts/ionicons.143146fa.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   197740 2022-11-22 08:52:36.000000 tqsdk-3.3.0/tqsdk/web/fonts/ionicons.99ac3308.woff
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 08:53:34.000000 tqsdk-3.3.0/tqsdk/web/img/
--rw-r--r--   0 runner    (1001) docker     (121)   555353 2022-11-22 08:52:37.000000 tqsdk-3.3.0/tqsdk/web/img/ionicons.a2c4a261.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 08:53:34.000000 tqsdk-3.3.0/tqsdk/web/img/icons/
--rw-r--r--   0 runner    (1001) docker     (121)     2925 2022-11-22 08:52:37.000000 tqsdk-3.3.0/tqsdk/web/img/icons/apple-touch-icon-72x72.png
--rw-r--r--   0 runner    (1001) docker     (121)     2628 2022-11-22 08:52:37.000000 tqsdk-3.3.0/tqsdk/web/img/icons/apple-touch-icon-60x60.png
--rw-r--r--   0 runner    (1001) docker     (121)     6269 2022-11-22 08:52:38.000000 tqsdk-3.3.0/tqsdk/web/img/icons/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (121)     2578 2022-11-22 08:52:37.000000 tqsdk-3.3.0/tqsdk/web/img/icons/apple-touch-icon-57x57.png
--rw-r--r--   0 runner    (1001) docker     (121)     3492 2022-11-22 08:52:37.000000 tqsdk-3.3.0/tqsdk/web/img/icons/favicon-96x96.png
--rw-r--r--   0 runner    (1001) docker     (121)     2925 2022-11-22 08:52:37.000000 tqsdk-3.3.0/tqsdk/web/img/icons/android-icon-72x72.png
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-11-22 08:52:37.000000 tqsdk-3.3.0/tqsdk/web/img/icons/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (121)     8235 2022-11-22 08:52:37.000000 tqsdk-3.3.0/tqsdk/web/img/icons/apple-touch-icon-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (121)     3153 2022-11-22 08:52:37.000000 tqsdk-3.3.0/tqsdk/web/img/icons/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)     1200 2022-11-22 08:52:38.000000 tqsdk-3.3.0/tqsdk/web/img/icons/notes
--rw-r--r--   0 runner    (1001) docker     (121)     4557 2022-11-22 08:52:37.000000 tqsdk-3.3.0/tqsdk/web/img/icons/apple-touch-icon-114x114.png
--rw-r--r--   0 runner    (1001) docker     (121)     3012 2022-11-22 08:52:37.000000 tqsdk-3.3.0/tqsdk/web/img/icons/apple-touch-icon-76x76.png
--rw-r--r--   0 runner    (1001) docker     (121)     8235 2022-11-22 08:52:37.000000 tqsdk-3.3.0/tqsdk/web/img/icons/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (121)     2890 2022-11-22 08:52:38.000000 tqsdk-3.3.0/tqsdk/web/img/icons/ms-icon-70x70.png
--rw-r--r--   0 runner    (1001) docker     (121)      720 2022-11-22 08:52:37.000000 tqsdk-3.3.0/tqsdk/web/img/icons/manifest.json
--rw-r--r--   0 runner    (1001) docker     (121)     4774 2022-11-22 08:52:37.000000 tqsdk-3.3.0/tqsdk/web/img/icons/apple-touch-icon-120x120.png
--rw-r--r--   0 runner    (1001) docker     (121)     5930 2022-11-22 08:52:37.000000 tqsdk-3.3.0/tqsdk/web/img/icons/apple-touch-icon-144x144.png
--rw-r--r--   0 runner    (1001) docker     (121)     2344 2022-11-22 08:52:37.000000 tqsdk-3.3.0/tqsdk/web/img/icons/android-icon-48x48.png
--rw-r--r--   0 runner    (1001) docker     (121)     7785 2022-11-22 08:52:37.000000 tqsdk-3.3.0/tqsdk/web/img/icons/apple-touch-icon-180x180.png
--rw-r--r--   0 runner    (1001) docker     (121)     5930 2022-11-22 08:52:36.000000 tqsdk-3.3.0/tqsdk/web/img/icons/android-icon-144x144.png
--rw-r--r--   0 runner    (1001) docker     (121)     6325 2022-11-22 08:52:37.000000 tqsdk-3.3.0/tqsdk/web/img/icons/apple-touch-icon-152x152.png
--rw-r--r--   0 runner    (1001) docker     (121)     3492 2022-11-22 08:52:37.000000 tqsdk-3.3.0/tqsdk/web/img/icons/android-icon-96x96.png
--rw-r--r--   0 runner    (1001) docker     (121)     3153 2022-11-22 08:52:37.000000 tqsdk-3.3.0/tqsdk/web/img/icons/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (121)    16757 2022-11-22 08:52:38.000000 tqsdk-3.3.0/tqsdk/web/img/icons/ms-icon-310x310.png
--rw-r--r--   0 runner    (1001) docker     (121)     1424 2022-11-22 08:52:37.000000 tqsdk-3.3.0/tqsdk/web/img/icons/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (121)     7490 2022-11-22 08:52:37.000000 tqsdk-3.3.0/tqsdk/web/img/icons/android-icon-192x192.png
--rw-r--r--   0 runner    (1001) docker     (121)     7490 2022-11-22 08:52:36.000000 tqsdk-3.3.0/tqsdk/web/img/icons/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (121)     5930 2022-11-22 08:52:38.000000 tqsdk-3.3.0/tqsdk/web/img/icons/msapplication-icon-144x144.png.png
--rw-r--r--   0 runner    (1001) docker     (121)     2073 2022-11-22 08:52:37.000000 tqsdk-3.3.0/tqsdk/web/img/icons/android-icon-36x36.png
--rw-r--r--   0 runner    (1001) docker     (121)     6269 2022-11-22 08:52:38.000000 tqsdk-3.3.0/tqsdk/web/img/icons/ms-icon-150x150.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 08:53:34.000000 tqsdk-3.3.0/tqsdk/web/js/
--rw-r--r--   0 runner    (1001) docker     (121)  1787845 2022-11-22 08:52:39.000000 tqsdk-3.3.0/tqsdk/web/js/chunk-vendors.d7fceff6.js
--rw-r--r--   0 runner    (1001) docker     (121)    62759 2022-11-22 08:52:38.000000 tqsdk-3.3.0/tqsdk/web/js/app.2c843c86.js
--rw-r--r--   0 runner    (1001) docker     (121)     7881 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)    10044 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/data_extension.py
--rw-r--r--   0 runner    (1001) docker     (121)    19843 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/tqwebhelper.py
--rw-r--r--   0 runner    (1001) docker     (121)    23481 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/data_series.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15785 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/ins_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/entity.py
--rw-r--r--   0 runner    (1001) docker     (121)      796 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/datetime_state.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 08:53:34.000000 tqsdk-3.3.0/tqsdk/algorithm/
--rw-r--r--   0 runner    (1001) docker     (121)    15605 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/algorithm/twap.py
--rw-r--r--   0 runner    (1001) docker     (121)    15935 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/algorithm/time_table_generater.py
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5865 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 08:53:34.000000 tqsdk-3.3.0/tqsdk/demo/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 08:53:34.000000 tqsdk-3.3.0/tqsdk/demo/tutorial/
--rw-r--r--   0 runner    (1001) docker     (121)     1055 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/tutorial/downloader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1430 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/tutorial/t95.py
--rw-r--r--   0 runner    (1001) docker     (121)     1193 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/tutorial/t60.py
--rw-r--r--   0 runner    (1001) docker     (121)     1283 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/tutorial/t20.py
--rw-r--r--   0 runner    (1001) docker     (121)     1149 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/tutorial/t96.py
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/tutorial/t70.py
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/tutorial/t92.py
--rw-r--r--   0 runner    (1001) docker     (121)     1589 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/tutorial/t71.py
--rw-r--r--   0 runner    (1001) docker     (121)      720 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/tutorial/t72.py
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/tutorial/t40.py
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/tutorial/underlying_symbol.py
--rw-r--r--   0 runner    (1001) docker     (121)     1216 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/tutorial/t30.py
--rw-r--r--   0 runner    (1001) docker     (121)      762 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/tutorial/t90.py
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/tutorial/t93.py
--rw-r--r--   0 runner    (1001) docker     (121)      853 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/tutorial/t94.py
--rw-r--r--   0 runner    (1001) docker     (121)      698 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/tutorial/t41.py
--rw-r--r--   0 runner    (1001) docker     (121)     1350 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/tutorial/t80.py
--rw-r--r--   0 runner    (1001) docker     (121)     1266 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/tutorial/backtest.py
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/tutorial/replay.py
--rw-r--r--   0 runner    (1001) docker     (121)     1294 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/tutorial/replay2.py
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/tutorial/t10.py
--rw-r--r--   0 runner    (1001) docker     (121)     1398 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/tutorial/t91.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-22 08:52:39.000000 tqsdk-3.3.0/tqsdk/demo/tutorial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1932 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/download_orders.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 08:53:34.000000 tqsdk-3.3.0/tqsdk/demo/option_tutorial/
--rw-r--r--   0 runner    (1001) docker     (121)     1243 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/option_tutorial/o70.py
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/option_tutorial/o40.py
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/option_tutorial/o71.py
--rw-r--r--   0 runner    (1001) docker     (121)     1017 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/option_tutorial/o20.py
--rw-r--r--   0 runner    (1001) docker     (121)     2060 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/option_tutorial/o74.py
--rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/option_tutorial/o30.py
--rw-r--r--   0 runner    (1001) docker     (121)      510 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/option_tutorial/o10.py
--rw-r--r--   0 runner    (1001) docker     (121)      642 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/option_tutorial/o73.py
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/option_tutorial/o41.py
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/option_tutorial/o72.py
--rw-r--r--   0 runner    (1001) docker     (121)      679 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/option_tutorial/o60.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-22 08:52:39.000000 tqsdk-3.3.0/tqsdk/demo/option_tutorial/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 08:53:34.000000 tqsdk-3.3.0/tqsdk/demo/example/
--rw-r--r--   0 runner    (1001) docker     (121)     5201 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/example/rbreaker2.py
--rw-r--r--   0 runner    (1001) docker     (121)     3172 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/example/gridtrading_async.py
--rw-r--r--   0 runner    (1001) docker     (121)     2131 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/example/momentum.py
--rw-r--r--   0 runner    (1001) docker     (121)     2033 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/example/dualthrust.py
--rw-r--r--   0 runner    (1001) docker     (121)     2779 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/example/aberration.py
--rw-r--r--   0 runner    (1001) docker     (121)     7794 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/example/turtle.py
--rw-r--r--   0 runner    (1001) docker     (121)     5277 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/example/vwap.py
--rw-r--r--   0 runner    (1001) docker     (121)     3180 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/example/fairy_four_price.py
--rw-r--r--   0 runner    (1001) docker     (121)     5493 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/example/random_forest.py
--rw-r--r--   0 runner    (1001) docker     (121)     3851 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/example/escalator.py
--rw-r--r--   0 runner    (1001) docker     (121)     4596 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/example/rbreaker.py
--rw-r--r--   0 runner    (1001) docker     (121)     1359 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/example/doublema.py
--rw-r--r--   0 runner    (1001) docker     (121)     4153 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/example/gridtrading.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-22 08:52:39.000000 tqsdk-3.3.0/tqsdk/demo/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1493 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/multiaccount.py
--rw-r--r--   0 runner    (1001) docker     (121)      690 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/ta.py
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/demo/ta_option.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-22 08:52:39.000000 tqsdk-3.3.0/tqsdk/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   207959 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/api.py
--rw-r--r--   0 runner    (1001) docker     (121)    20440 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/report.py
--rw-r--r--   0 runner    (1001) docker     (121)     3478 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5400 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/baseApi.py
--rw-r--r--   0 runner    (1001) docker     (121)    37146 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/objs.py
--rw-r--r--   0 runner    (1001) docker     (121)     9254 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/multiaccount.py
--rw-r--r--   0 runner    (1001) docker     (121)    91538 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/ta.py
--rw-r--r--   0 runner    (1001) docker     (121)     4910 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/channel.py
--rw-r--r--   0 runner    (1001) docker     (121)     3827 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/symbols.py
--rw-r--r--   0 runner    (1001) docker     (121)     7136 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/diff.py
--rw-r--r--   0 runner    (1001) docker     (121)   132245 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/expired_quotes.json.lzma
--rw-r--r--   0 runner    (1001) docker     (121)     4949 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/datetime.py
--rw-r--r--   0 runner    (1001) docker     (121)     1439 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/risk_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     4366 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/calendar.py
--rw-r--r--   0 runner    (1001) docker     (121)     3876 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/baseModule.py
--rw-r--r--   0 runner    (1001) docker     (121)      603 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3962 2022-11-22 08:52:35.000000 tqsdk-3.3.0/tqsdk/utils_symbols.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 07:33:18.000000 tqsdk-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     5725 2023-04-13 07:33:18.000000 tqsdk-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5278 2023-04-13 07:32:38.000000 tqsdk-3.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 07:33:18.000000 tqsdk-3.4.0/tqsdk/
+-rw-r--r--   0 runner    (1001) docker     (122)     4949 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 07:33:18.000000 tqsdk-3.4.0/tqsdk/tradeable/
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/tradeable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 07:33:18.000000 tqsdk-3.4.0/tqsdk/tradeable/sim/
+-rw-r--r--   0 runner    (1001) docker     (122)    11943 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/tradeable/sim/trade_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/tradeable/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8523 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/tradeable/sim/tqsim_stock.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18113 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/tradeable/sim/basesim.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27585 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/tradeable/sim/trade_stock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5083 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/tradeable/sim/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10665 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/tradeable/sim/tqsim.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35956 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/tradeable/sim/trade_future.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1259 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/tradeable/tradeable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 07:33:18.000000 tqsdk-3.4.0/tqsdk/tradeable/otg/
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/tradeable/otg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3524 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/tradeable/otg/tqaccount.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3794 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/tradeable/otg/tqkq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5078 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/tradeable/otg/base_otg.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15130 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/tradeable/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      603 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9254 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/multiaccount.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20372 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/objs_not_entity.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37146 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/objs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    52985 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/tafunc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 07:33:18.000000 tqsdk-3.4.0/tqsdk/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/__pyinstaller/hook-tqsdk.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3827 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/symbols.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 07:33:18.000000 tqsdk-3.4.0/tqsdk/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15935 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/algorithm/time_table_generater.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15605 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/algorithm/twap.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 07:33:18.000000 tqsdk-3.4.0/tqsdk/backtest/
+-rw-r--r--   0 runner    (1001) docker     (122)      162 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/backtest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6687 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/backtest/replay.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4816 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/backtest/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42136 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/backtest/backtest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7959 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 07:33:18.000000 tqsdk-3.4.0/tqsdk/web/
+-rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/web/service-worker.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 07:33:18.000000 tqsdk-3.4.0/tqsdk/web/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     5764 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/web/css/app.d72d8978.css
+-rw-r--r--   0 runner    (1001) docker     (122)   279508 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/web/css/chunk-vendors.c93e9127.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 07:33:18.000000 tqsdk-3.4.0/tqsdk/web/img/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 07:33:18.000000 tqsdk-3.4.0/tqsdk/web/img/icons/
+-rw-r--r--   0 runner    (1001) docker     (122)      281 2023-04-13 07:32:39.000000 tqsdk-3.4.0/tqsdk/web/img/icons/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     2628 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/web/img/icons/apple-touch-icon-60x60.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5930 2023-04-13 07:32:39.000000 tqsdk-3.4.0/tqsdk/web/img/icons/msapplication-icon-144x144.png.png
+-rw-r--r--   0 runner    (1001) docker     (122)    16757 2023-04-13 07:32:39.000000 tqsdk-3.4.0/tqsdk/web/img/icons/ms-icon-310x310.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2578 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/web/img/icons/apple-touch-icon-57x57.png
+-rw-r--r--   0 runner    (1001) docker     (122)     6269 2023-04-13 07:32:39.000000 tqsdk-3.4.0/tqsdk/web/img/icons/ms-icon-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4774 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/web/img/icons/apple-touch-icon-120x120.png
+-rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/web/img/icons/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3153 2023-04-13 07:32:39.000000 tqsdk-3.4.0/tqsdk/web/img/icons/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (122)     3012 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/web/img/icons/apple-touch-icon-76x76.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1200 2023-04-13 07:32:39.000000 tqsdk-3.4.0/tqsdk/web/img/icons/notes
+-rw-r--r--   0 runner    (1001) docker     (122)     5930 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/web/img/icons/android-icon-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3492 2023-04-13 07:32:39.000000 tqsdk-3.4.0/tqsdk/web/img/icons/favicon-96x96.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2890 2023-04-13 07:32:39.000000 tqsdk-3.4.0/tqsdk/web/img/icons/ms-icon-70x70.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5930 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/web/img/icons/apple-touch-icon-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4557 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/web/img/icons/apple-touch-icon-114x114.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2925 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/web/img/icons/apple-touch-icon-72x72.png
+-rw-r--r--   0 runner    (1001) docker     (122)     7785 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/web/img/icons/apple-touch-icon-180x180.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2344 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/web/img/icons/android-icon-48x48.png
+-rw-r--r--   0 runner    (1001) docker     (122)     6325 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/web/img/icons/apple-touch-icon-152x152.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2073 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/web/img/icons/android-icon-36x36.png
+-rw-r--r--   0 runner    (1001) docker     (122)     7490 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/web/img/icons/android-icon-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (122)      720 2023-04-13 07:32:39.000000 tqsdk-3.4.0/tqsdk/web/img/icons/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3153 2023-04-13 07:32:39.000000 tqsdk-3.4.0/tqsdk/web/img/icons/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3492 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/web/img/icons/android-icon-96x96.png
+-rw-r--r--   0 runner    (1001) docker     (122)     7490 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/web/img/icons/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2925 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/web/img/icons/android-icon-72x72.png
+-rw-r--r--   0 runner    (1001) docker     (122)     6269 2023-04-13 07:32:39.000000 tqsdk-3.4.0/tqsdk/web/img/icons/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1424 2023-04-13 07:32:39.000000 tqsdk-3.4.0/tqsdk/web/img/icons/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/web/img/icons/apple-touch-icon-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (122)   555353 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/web/img/ionicons.a2c4a261.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     1216 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/web/precache-manifest.7ed60b69dab01cdb0c64836489ab6e0d.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 07:33:18.000000 tqsdk-3.4.0/tqsdk/web/js/
+-rw-r--r--   0 runner    (1001) docker     (122)  1787845 2023-04-13 07:32:39.000000 tqsdk-3.4.0/tqsdk/web/js/chunk-vendors.d7fceff6.js
+-rw-r--r--   0 runner    (1001) docker     (122)    62759 2023-04-13 07:32:39.000000 tqsdk-3.4.0/tqsdk/web/js/app.2c843c86.js
+-rw-r--r--   0 runner    (1001) docker     (122)     3153 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/web/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/web/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      565 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/web/manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 07:33:18.000000 tqsdk-3.4.0/tqsdk/web/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)   197740 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/web/fonts/ionicons.99ac3308.woff
+-rw-r--r--   0 runner    (1001) docker     (122)    82216 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/web/fonts/ionicons.143146fa.woff2
+-rw-r--r--   0 runner    (1001) docker     (122)   197664 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/web/fonts/ionicons.d535a25a.ttf
+-rw-r--r--   0 runner    (1001) docker     (122)     2095 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/web/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)   246120 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/web/d3.min.js
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15785 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/ins_schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)   132245 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/expired_quotes.json.lzma
+-rw-r--r--   0 runner    (1001) docker     (122)     7136 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)   207941 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19843 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/tqwebhelper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1769 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3962 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/utils_symbols.py
+-rw-r--r--   0 runner    (1001) docker     (122)      796 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/datetime_state.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 07:33:18.000000 tqsdk-3.4.0/tqsdk/tools/
+-rw-r--r--   0 runner    (1001) docker     (122)      636 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/tools/dead_ins.lzma
+-rw-r--r--   0 runner    (1001) docker     (122)      122 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22148 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/tools/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5400 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/baseApi.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20440 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/report.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1105 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/entity.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23481 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/data_series.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21986 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/connect.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12660 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/risk_rule.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6925 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/sm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4910 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/channel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5865 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4366 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3876 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/baseModule.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 07:33:18.000000 tqsdk-3.4.0/tqsdk/lib/
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38277 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/lib/target_pos_task.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2196 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/lib/notify.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4674 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10550 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/lib/target_pos_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6099 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/stockprofit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6864 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/rangeset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3270 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/trading_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/risk_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 07:33:18.000000 tqsdk-3.4.0/tqsdk/demo/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 07:32:39.000000 tqsdk-3.4.0/tqsdk/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/multiaccount.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 07:33:18.000000 tqsdk-3.4.0/tqsdk/demo/example/
+-rw-r--r--   0 runner    (1001) docker     (122)     2131 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/example/momentum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2779 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/example/aberration.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 07:32:39.000000 tqsdk-3.4.0/tqsdk/demo/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3180 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/example/fairy_four_price.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5493 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/example/random_forest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2033 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/example/dualthrust.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4153 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/example/gridtrading.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3851 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/example/escalator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4596 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/example/rbreaker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5201 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/example/rbreaker2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5277 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/example/vwap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/example/doublema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7794 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/example/turtle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3172 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/example/gridtrading_async.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/download_orders.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 07:33:18.000000 tqsdk-3.4.0/tqsdk/demo/option_tutorial/
+-rw-r--r--   0 runner    (1001) docker     (122)     1563 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/option_tutorial/o30.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 07:32:39.000000 tqsdk-3.4.0/tqsdk/demo/option_tutorial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      568 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/option_tutorial/o41.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2060 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/option_tutorial/o74.py
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/option_tutorial/o10.py
+-rw-r--r--   0 runner    (1001) docker     (122)      642 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/option_tutorial/o73.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1243 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/option_tutorial/o70.py
+-rw-r--r--   0 runner    (1001) docker     (122)      679 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/option_tutorial/o60.py
+-rw-r--r--   0 runner    (1001) docker     (122)      574 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/option_tutorial/o72.py
+-rw-r--r--   0 runner    (1001) docker     (122)      544 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/option_tutorial/o71.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/option_tutorial/o20.py
+-rw-r--r--   0 runner    (1001) docker     (122)      681 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/option_tutorial/o40.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 07:33:18.000000 tqsdk-3.4.0/tqsdk/demo/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (122)     1294 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/tutorial/replay2.py
+-rw-r--r--   0 runner    (1001) docker     (122)      698 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/tutorial/t41.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1589 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/tutorial/t71.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 07:32:39.000000 tqsdk-3.4.0/tqsdk/demo/tutorial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1149 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/tutorial/t96.py
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/tutorial/t90.py
+-rw-r--r--   0 runner    (1001) docker     (122)      853 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/tutorial/t94.py
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/tutorial/underlying_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1398 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/tutorial/t91.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1430 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/tutorial/t95.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/tutorial/t70.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1086 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/tutorial/t92.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1050 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/tutorial/t40.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/tutorial/t20.py
+-rw-r--r--   0 runner    (1001) docker     (122)      720 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/tutorial/t72.py
+-rw-r--r--   0 runner    (1001) docker     (122)      552 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/tutorial/replay.py
+-rw-r--r--   0 runner    (1001) docker     (122)      473 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/tutorial/t10.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1216 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/tutorial/t30.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1088 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/tutorial/t93.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1350 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/tutorial/t80.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1055 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/tutorial/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1266 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/tutorial/backtest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/tutorial/t60.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/ta_option.py
+-rw-r--r--   0 runner    (1001) docker     (122)      690 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/demo/ta.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10044 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/data_extension.py
+-rw-r--r--   0 runner    (1001) docker     (122)    91538 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/ta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9392 2023-04-13 07:32:38.000000 tqsdk-3.4.0/tqsdk/trade_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 07:33:18.000000 tqsdk-3.4.0/tqsdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5725 2023-04-13 07:33:18.000000 tqsdk-3.4.0/tqsdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-04-13 07:33:18.000000 tqsdk-3.4.0/tqsdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-04-13 07:33:18.000000 tqsdk-3.4.0/tqsdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     5268 2023-04-13 07:33:18.000000 tqsdk-3.4.0/tqsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-04-13 07:33:18.000000 tqsdk-3.4.0/tqsdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 07:33:18.000000 tqsdk-3.4.0/tqsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-04-13 07:33:18.000000 tqsdk-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)    11335 2023-04-13 07:32:38.000000 tqsdk-3.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      200 2023-04-13 07:32:38.000000 tqsdk-3.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-04-13 07:32:38.000000 tqsdk-3.4.0/setup.py
```

### Comparing `tqsdk-3.3.0/LICENSE` & `tqsdk-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/README.md` & `tqsdk-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/PKG-INFO` & `tqsdk-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tqsdk
-Version: 3.3.0
+Version: 3.4.0
 Summary: TianQin SDK
 Home-page: https://www.shinnytech.com/tqsdk
 Author: TianQin
 Author-email: tianqincn@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tqsdk-3.3.0/tqsdk.egg-info/SOURCES.txt` & `tqsdk-3.4.0/tqsdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,28 +25,28 @@
 tqsdk/multiaccount.py
 tqsdk/objs.py
 tqsdk/objs_not_entity.py
 tqsdk/rangeset.py
 tqsdk/report.py
 tqsdk/risk_manager.py
 tqsdk/risk_rule.py
+tqsdk/sm.py
 tqsdk/stockprofit.py
 tqsdk/symbols.py
 tqsdk/ta.py
 tqsdk/tafunc.py
 tqsdk/tqwebhelper.py
 tqsdk/trade_extension.py
 tqsdk/trading_status.py
 tqsdk/utils.py
 tqsdk/utils_symbols.py
 tqsdk.egg-info/PKG-INFO
 tqsdk.egg-info/SOURCES.txt
 tqsdk.egg-info/dependency_links.txt
 tqsdk.egg-info/entry_points.txt
-tqsdk.egg-info/not-zip-safe
 tqsdk.egg-info/requires.txt
 tqsdk.egg-info/top_level.txt
 tqsdk/__pyinstaller/__init__.py
 tqsdk/__pyinstaller/hook-tqsdk.py
 tqsdk/algorithm/__init__.py
 tqsdk/algorithm/time_table_generater.py
 tqsdk/algorithm/twap.py
```

### Comparing `tqsdk-3.3.0/tqsdk.egg-info/PKG-INFO` & `tqsdk-3.4.0/tqsdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tqsdk
-Version: 3.3.0
+Version: 3.4.0
 Summary: TianQin SDK
 Home-page: https://www.shinnytech.com/tqsdk
 Author: TianQin
 Author-email: tianqincn@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tqsdk-3.3.0/tqsdk/objs_not_entity.py` & `tqsdk-3.4.0/tqsdk/objs_not_entity.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/risk_rule.py` & `tqsdk-3.4.0/tqsdk/risk_rule.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/trading_status.py` & `tqsdk-3.4.0/tqsdk/trading_status.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/tafunc.py` & `tqsdk-3.4.0/tqsdk/tafunc.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/lib/target_pos_scheduler.py` & `tqsdk-3.4.0/tqsdk/lib/target_pos_scheduler.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/lib/utils.py` & `tqsdk-3.4.0/tqsdk/lib/utils.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/lib/notify.py` & `tqsdk-3.4.0/tqsdk/lib/notify.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/lib/target_pos_task.py` & `tqsdk-3.4.0/tqsdk/lib/target_pos_task.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/connect.py` & `tqsdk-3.4.0/tqsdk/connect.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,31 @@
 
 import asyncio
 import json
 import random
 import ssl
 import time
 import warnings
+import base64
 from abc import abstractmethod
 from datetime import datetime
 from logging import Logger
 from queue import Queue
 from typing import Optional
+from urllib.parse import urlparse
 
 import certifi
 import websockets
 from shinny_structlog import ShinnyLoggerAdapter
 
 from tqsdk.diff import _merge_diff, _get_obj
 from tqsdk.entity import Entity
 from tqsdk.exceptions import TqBacktestPermissionError
 from tqsdk.utils import _generate_uuid
+from tqsdk.sm import SMContext, NullContext
 
 """
 优化代码结构，修改为
 
 TqConnect 
 （负责连接 websocket 连接，从服务器收到数据发回下游，从下游收到指令包发给上游，生成连接建立、连接断开的通知发给下游）
  ｜  ｜
@@ -110,124 +113,135 @@
         # 调整代码位置，方便 monkey patch
         self._ins_list_max_length = 100000  # subscribe_quote 最大长度
         self._subscribed_per_seconds = 100  # 每秒 subscribe_quote 请求次数限制
         self._subscribed_queue = Queue(self._subscribed_per_seconds)
 
         self._keywords["extra_headers"] = self._api._base_headers
         self._keywords["create_protocol"] = TqWebSocketClientProtocol
-        if url.startswith("wss://"):
+        url_info = urlparse(url)
+        cm = NullContext()
+        if url_info.scheme == "wss":
             ssl_context = ssl.create_default_context()
             ssl_context.load_verify_locations(certifi.where())
             self._keywords["ssl"] = ssl_context
+        elif url_info.scheme.startswith("sm"):
+            sm_info = url_info.path.split("/", 4)
+            cm = SMContext(self._logger, self._api, url_info.scheme, sm_info[1], base64.urlsafe_b64decode(sm_info[2]).decode("utf-8"), base64.urlsafe_b64decode(sm_info[3]).decode("utf-8"))
+            url_info = url_info._replace(scheme="ws", path="/".join(sm_info[:1]+sm_info[4:]))
+
         count = 0
-        while True:
-            try:
-                if not self._first_connect:
+        async with cm:
+            while True:
+                try:
+                    if isinstance(cm, SMContext):
+                        addr = await cm.get_addr()
+                        url = url_info._replace(netloc=addr).geturl()
+                    if not self._first_connect:
+                        notify_id = _generate_uuid()
+                        notify = {
+                            "type": "MESSAGE",
+                            "level": "WARNING",
+                            "code": 2019112910,
+                            "conn_id": self._conn_id,
+                            "content": f"开始与 {url} 的重新建立网络连接",
+                            "url": url
+                        }
+                        self._logger.debug("websocket connection connecting")
+                        await recv_chan.send({
+                            "aid": "rtn_data",
+                            "data": [{
+                                "notify": {
+                                    notify_id: notify
+                                }
+                            }]
+                        })
+                    async with websockets.connect(url, **self._keywords) as client:
+                        # 发送网络连接建立的通知，code = 2019112901
+                        notify_id = _generate_uuid()
+                        notify = {
+                            "type": "MESSAGE",
+                            "level": "INFO",
+                            "code": 2019112901,
+                            "conn_id": self._conn_id,
+                            "content": "与 %s 的网络连接已建立" % url,
+                            "url": url
+                        }
+                        if not self._first_connect:  # 如果不是第一次连接, 即为重连
+                            # 发送网络连接重新建立的通知，code = 2019112902
+                            notify["code"] = 2019112902
+                            notify["level"] = "WARNING"
+                            notify["content"] = "与 %s 的网络连接已恢复" % url
+                            self._logger.debug("websocket reconnected")
+                        else:
+                            self._logger.debug("websocket connected")
+                        # 发送网络连接建立的通知，code = 2019112901 or 2019112902，这里区分了第一次连接和重连
+                        await self._api._wait_until_idle()
+                        await recv_chan.send({
+                            "aid": "rtn_data",
+                            "data": [{
+                                "notify": {
+                                    notify_id: notify
+                                }
+                            }]
+                        })
+                        count = 0
+                        self._api._reconnect_timer.set_count(count)
+                        send_task = self._api.create_task(self._send_handler(send_chan, client))
+                        try:
+                            async for msg in client:
+                                pack = json.loads(msg)
+                                await self._api._wait_until_idle()
+                                self._logger.debug("websocket received data", pack=msg)
+                                await recv_chan.send(pack)
+                        finally:
+                            self._logger.debug("websocket connection info", current_time=time.time(),
+                                               start_read_message=client.reader._start_read_message,
+                                               read_size=client.reader._read_size)
+                            send_task.cancel()
+                            await send_task
+                # 希望做到的效果是遇到网络问题可以断线重连, 但是可能抛出的例外太多了(TimeoutError,socket.gaierror等), 又没有文档或工具可以理出 try 代码中所有可能遇到的例外
+                # 而这里的 except 又需要处理所有子函数及子函数的子函数等等可能抛出的例外, 因此这里只能遇到问题之后再补, 并且无法避免 false positive 和 false negative
+                except (websockets.exceptions.ConnectionClosed, websockets.exceptions.InvalidStatusCode, websockets.exceptions.InvalidURI,
+                        websockets.exceptions.InvalidState, websockets.exceptions.ProtocolError, OSError, EOFError,
+                        TqBacktestPermissionError) as e:
+                    in_ops_time = datetime.now().hour == 19 and 0 <= datetime.now().minute <= 30
+                    # 发送网络连接断开的通知，code = 2019112911
                     notify_id = _generate_uuid()
                     notify = {
                         "type": "MESSAGE",
                         "level": "WARNING",
-                        "code": 2019112910,
-                        "conn_id": self._conn_id,
-                        "content": f"开始与 {url} 的重新建立网络连接",
-                        "url": url
-                    }
-                    self._logger.debug("websocket connection connecting")
-                    await recv_chan.send({
-                        "aid": "rtn_data",
-                        "data": [{
-                            "notify": {
-                                notify_id: notify
-                            }
-                        }]
-                    })
-                async with websockets.connect(url, **self._keywords) as client:
-                    # 发送网络连接建立的通知，code = 2019112901
-                    notify_id = _generate_uuid()
-                    notify = {
-                        "type": "MESSAGE",
-                        "level": "INFO",
-                        "code": 2019112901,
+                        "code": 2019112911,
                         "conn_id": self._conn_id,
-                        "content": "与 %s 的网络连接已建立" % url,
+                        "content": f"与 {url} 的网络连接断开，请检查客户端及网络是否正常",
                         "url": url
                     }
-                    if not self._first_connect:  # 如果不是第一次连接, 即为重连
-                        # 发送网络连接重新建立的通知，code = 2019112902
-                        notify["code"] = 2019112902
-                        notify["level"] = "WARNING"
-                        notify["content"] = "与 %s 的网络连接已恢复" % url
-                        self._logger.debug("websocket reconnected")
-                    else:
-                        self._logger.debug("websocket connected")
-                    # 发送网络连接建立的通知，code = 2019112901 or 2019112902，这里区分了第一次连接和重连
-                    await self._api._wait_until_idle()
+                    if in_ops_time:
+                        notify['content'] += '，每日 19:00-19:30 为日常运维时间，请稍后再试'
+                    self._logger.debug("websocket connection closed", error=str(e))
                     await recv_chan.send({
                         "aid": "rtn_data",
                         "data": [{
                             "notify": {
                                 notify_id: notify
                             }
                         }]
                     })
-                    count = 0
+                    if isinstance(e, TqBacktestPermissionError):
+                        # 如果错误类型是用户无回测权限，直接返回
+                        raise
+                    if self._first_connect and in_ops_time:
+                        raise Exception(f'与 {url} 的连接失败，每日 19:00-19:30 为日常运维时间，请稍后再试')
+                    if self._first_connect:
+                        self._first_connect = False
+                    # 下次重连的时间距离现在当前时间秒数，会等待相应的时间，否则立即发起重连
+                    sleep_seconds = self._api._reconnect_timer.timer - time.time()
+                    if sleep_seconds > 0:
+                        await asyncio.sleep(sleep_seconds)
+                    count += 1
                     self._api._reconnect_timer.set_count(count)
-                    send_task = self._api.create_task(self._send_handler(send_chan, client))
-                    try:
-                        async for msg in client:
-                            pack = json.loads(msg)
-                            await self._api._wait_until_idle()
-                            self._logger.debug("websocket received data", pack=msg)
-                            await recv_chan.send(pack)
-                    finally:
-                        self._logger.debug("websocket connection info", current_time=time.time(),
-                                           start_read_message=client.reader._start_read_message,
-                                           read_size=client.reader._read_size)
-                        send_task.cancel()
-                        await send_task
-            # 希望做到的效果是遇到网络问题可以断线重连, 但是可能抛出的例外太多了(TimeoutError,socket.gaierror等), 又没有文档或工具可以理出 try 代码中所有可能遇到的例外
-            # 而这里的 except 又需要处理所有子函数及子函数的子函数等等可能抛出的例外, 因此这里只能遇到问题之后再补, 并且无法避免 false positive 和 false negative
-            except (websockets.exceptions.ConnectionClosed, websockets.exceptions.InvalidStatusCode,
-                    websockets.exceptions.InvalidState, websockets.exceptions.ProtocolError, OSError, EOFError,
-                    TqBacktestPermissionError) as e:
-                in_ops_time = datetime.now().hour == 19 and 0 <= datetime.now().minute <= 30
-                # 发送网络连接断开的通知，code = 2019112911
-                notify_id = _generate_uuid()
-                notify = {
-                    "type": "MESSAGE",
-                    "level": "WARNING",
-                    "code": 2019112911,
-                    "conn_id": self._conn_id,
-                    "content": f"与 {url} 的网络连接断开，请检查客户端及网络是否正常",
-                    "url": url
-                }
-                if in_ops_time:
-                    notify['content'] += '，每日 19:00-19:30 为日常运维时间，请稍后再试'
-                self._logger.debug("websocket connection closed", error=str(e))
-                await recv_chan.send({
-                    "aid": "rtn_data",
-                    "data": [{
-                        "notify": {
-                            notify_id: notify
-                        }
-                    }]
-                })
-                if isinstance(e, TqBacktestPermissionError):
-                    # 如果错误类型是用户无回测权限，直接返回
-                    raise
-                if self._first_connect and in_ops_time:
-                    raise Exception(f'与 {url} 的连接失败，每日 19:00-19:30 为日常运维时间，请稍后再试')
-                if self._first_connect:
-                    self._first_connect = False
-                # 下次重连的时间距离现在当前时间秒数，会等待相应的时间，否则立即发起重连
-                sleep_seconds = self._api._reconnect_timer.timer - time.time()
-                if sleep_seconds > 0:
-                    await asyncio.sleep(sleep_seconds)
-                count += 1
-                self._api._reconnect_timer.set_count(count)
 
     async def _send_handler(self, send_chan, client):
         """websocket客户端数据发送协程"""
         try:
             async for pack in send_chan:
                 if pack.get("aid") == "subscribe_quote":
                     if len(pack.get("ins_list", "")) > self._ins_list_max_length:
```

### Comparing `tqsdk-3.3.0/tqsdk/stockprofit.py` & `tqsdk-3.4.0/tqsdk/stockprofit.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/tradeable/sim/basesim.py` & `tqsdk-3.4.0/tqsdk/tradeable/sim/basesim.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/tradeable/sim/trade_base.py` & `tqsdk-3.4.0/tqsdk/tradeable/sim/trade_base.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/tradeable/sim/tqsim_stock.py` & `tqsdk-3.4.0/tqsdk/tradeable/sim/tqsim_stock.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/tradeable/sim/trade_future.py` & `tqsdk-3.4.0/tqsdk/tradeable/sim/trade_future.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/tradeable/sim/utils.py` & `tqsdk-3.4.0/tqsdk/tradeable/sim/utils.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/tradeable/sim/trade_stock.py` & `tqsdk-3.4.0/tqsdk/tradeable/sim/trade_stock.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/tradeable/sim/tqsim.py` & `tqsdk-3.4.0/tqsdk/tradeable/sim/tqsim.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/tradeable/mixin.py` & `tqsdk-3.4.0/tqsdk/tradeable/mixin.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/tradeable/tradeable.py` & `tqsdk-3.4.0/tqsdk/tradeable/tradeable.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/tradeable/otg/tqkq.py` & `tqsdk-3.4.0/tqsdk/tradeable/otg/tqkq.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/tradeable/otg/base_otg.py` & `tqsdk-3.4.0/tqsdk/tradeable/otg/base_otg.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 #!usr/bin/env python3
 # -*- coding:utf-8 -*-
 __author__ = 'yanqiong'
 
 import hashlib
+import base64
+from urllib.parse import urlparse
 from typing import Optional
 
 from tqsdk.tradeable.mixin import FutureMixin, StockMixin
 from tqsdk.tradeable.tradeable import Tradeable
 
 
 class BaseOtg(Tradeable):
-    def __init__(self, broker_id: str, account_id: str, password: str, td_url: Optional[str] = None) -> None:
+    def __init__(self, broker_id: str, account_id: str, password: str, td_url: Optional[str] = None, sm: bool = False) -> None:
         if not isinstance(broker_id, str):
             raise Exception("broker_id 参数类型应该是 str")
         if not isinstance(account_id, str):
             raise Exception("account_id 参数类型应该是 str")
         if not isinstance(password, str):
             raise Exception("password 参数类型应该是 str")
         self._broker_id = broker_id.strip()  # 期货公司（用户登录 rsp_login 填的）
         self._account_id = account_id.strip()  # 期货账户 （用户登录 rsp_login 填的）
         self._password = password
         self._td_url = td_url
+        self._sm = sm
 
         super(BaseOtg, self).__init__()
 
     def _get_account_key(self):
         s = self._broker_id + self._account_id
         return hashlib.md5(s.encode('utf-8')).hexdigest()
 
@@ -54,19 +57,27 @@
     def _update_otg_info(self, api):
         """更新 otg 登录需要的基本信息"""
         if self._td_url:
             return
         if api._td_url:
             self._td_url = api._td_url
         else:
-            self._td_url, account_type = api._auth._get_td_url(self._broker_id, self._account_id)
+            self._td_url, account_type, sm_type, sm_config = api._auth._get_td_url(self._broker_id, self._account_id)
             if account_type == "FUTURE":
                 assert isinstance(self, FutureMixin)
             else:
                 assert isinstance(self, StockMixin)
+            if self._sm and sm_type and sm_config:
+                url_account = base64.urlsafe_b64encode(self._account_id.encode("utf-8")).decode("utf-8")
+                url_password = base64.urlsafe_b64encode(self._password.encode("utf-8")).decode("utf-8")
+                url_info = urlparse(self._td_url)
+                # http://example.org -> http://example.org/smcfg/smuser/smpasswd
+                # http://example.org/ -> http://example.org/smcfg/smuser/smpasswd/
+                # http://example.org/foo/bar -> http://example.org/smcfg/smuser/smpasswd/foo/bar
+                self._td_url = url_info._replace(scheme=sm_type, path=f"/{sm_config}/{url_account}/{url_password}{url_info.path}").geturl()
 
     async def _run(self, api, api_send_chan, api_recv_chan, md_send_chan, md_recv_chan, td_send_chan, td_recv_chan):
         self._api = api
         self._api_send_chan = api_send_chan
         self._api_recv_chan = api_recv_chan
         self._md_send_chan = md_send_chan
         self._md_recv_chan = md_recv_chan
```

### Comparing `tqsdk-3.3.0/tqsdk/tools/downloader.py` & `tqsdk-3.4.0/tqsdk/tools/downloader.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/tools/dead_ins.lzma` & `tqsdk-3.4.0/tqsdk/tools/dead_ins.lzma`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/backtest/utils.py` & `tqsdk-3.4.0/tqsdk/backtest/utils.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/backtest/backtest.py` & `tqsdk-3.4.0/tqsdk/backtest/backtest.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/backtest/replay.py` & `tqsdk-3.4.0/tqsdk/backtest/replay.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/rangeset.py` & `tqsdk-3.4.0/tqsdk/rangeset.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/trade_extension.py` & `tqsdk-3.4.0/tqsdk/trade_extension.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/log.py` & `tqsdk-3.4.0/tqsdk/log.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/service-worker.js` & `tqsdk-3.4.0/tqsdk/web/service-worker.js`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/favicon.ico` & `tqsdk-3.4.0/tqsdk/web/img/icons/favicon.ico`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/index.html` & `tqsdk-3.4.0/tqsdk/web/index.html`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/manifest.json` & `tqsdk-3.4.0/tqsdk/web/manifest.json`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/d3.min.js` & `tqsdk-3.4.0/tqsdk/web/d3.min.js`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/precache-manifest.7ed60b69dab01cdb0c64836489ab6e0d.js` & `tqsdk-3.4.0/tqsdk/web/precache-manifest.7ed60b69dab01cdb0c64836489ab6e0d.js`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/css/chunk-vendors.c93e9127.css` & `tqsdk-3.4.0/tqsdk/web/css/chunk-vendors.c93e9127.css`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/css/app.d72d8978.css` & `tqsdk-3.4.0/tqsdk/web/css/app.d72d8978.css`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/fonts/ionicons.d535a25a.ttf` & `tqsdk-3.4.0/tqsdk/web/fonts/ionicons.d535a25a.ttf`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/fonts/ionicons.143146fa.woff2` & `tqsdk-3.4.0/tqsdk/web/fonts/ionicons.143146fa.woff2`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/fonts/ionicons.99ac3308.woff` & `tqsdk-3.4.0/tqsdk/web/fonts/ionicons.99ac3308.woff`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/img/ionicons.a2c4a261.svg` & `tqsdk-3.4.0/tqsdk/web/img/ionicons.a2c4a261.svg`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/img/icons/apple-touch-icon-72x72.png` & `tqsdk-3.4.0/tqsdk/web/img/icons/apple-touch-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/img/icons/apple-touch-icon-60x60.png` & `tqsdk-3.4.0/tqsdk/web/img/icons/apple-touch-icon-60x60.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/img/icons/mstile-150x150.png` & `tqsdk-3.4.0/tqsdk/web/img/icons/ms-icon-150x150.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/img/icons/apple-touch-icon-57x57.png` & `tqsdk-3.4.0/tqsdk/web/img/icons/apple-touch-icon-57x57.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/img/icons/favicon-96x96.png` & `tqsdk-3.4.0/tqsdk/web/img/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/img/icons/android-icon-72x72.png` & `tqsdk-3.4.0/tqsdk/web/img/icons/android-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/img/icons/apple-touch-icon-precomposed.png` & `tqsdk-3.4.0/tqsdk/web/img/icons/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/img/icons/favicon.ico` & `tqsdk-3.4.0/tqsdk/web/img/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/img/icons/notes` & `tqsdk-3.4.0/tqsdk/web/img/icons/notes`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/img/icons/apple-touch-icon-114x114.png` & `tqsdk-3.4.0/tqsdk/web/img/icons/apple-touch-icon-114x114.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/img/icons/apple-touch-icon-76x76.png` & `tqsdk-3.4.0/tqsdk/web/img/icons/apple-touch-icon-76x76.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/img/icons/apple-touch-icon.png` & `tqsdk-3.4.0/tqsdk/web/img/icons/apple-touch-icon-precomposed.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/img/icons/ms-icon-70x70.png` & `tqsdk-3.4.0/tqsdk/web/img/icons/ms-icon-70x70.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/img/icons/manifest.json` & `tqsdk-3.4.0/tqsdk/web/img/icons/manifest.json`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/img/icons/apple-touch-icon-120x120.png` & `tqsdk-3.4.0/tqsdk/web/img/icons/apple-touch-icon-120x120.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/img/icons/apple-touch-icon-144x144.png` & `tqsdk-3.4.0/tqsdk/web/img/icons/msapplication-icon-144x144.png.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/img/icons/android-icon-48x48.png` & `tqsdk-3.4.0/tqsdk/web/img/icons/android-icon-48x48.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/img/icons/apple-touch-icon-180x180.png` & `tqsdk-3.4.0/tqsdk/web/img/icons/apple-touch-icon-180x180.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/img/icons/android-icon-144x144.png` & `tqsdk-3.4.0/tqsdk/web/img/icons/android-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/img/icons/apple-touch-icon-152x152.png` & `tqsdk-3.4.0/tqsdk/web/img/icons/apple-touch-icon-152x152.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/img/icons/android-icon-96x96.png` & `tqsdk-3.4.0/tqsdk/web/img/icons/android-icon-96x96.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/img/icons/favicon-32x32.png` & `tqsdk-3.4.0/tqsdk/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/img/icons/ms-icon-310x310.png` & `tqsdk-3.4.0/tqsdk/web/img/icons/ms-icon-310x310.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/img/icons/favicon-16x16.png` & `tqsdk-3.4.0/tqsdk/web/img/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/img/icons/android-icon-192x192.png` & `tqsdk-3.4.0/tqsdk/web/img/icons/android-icon-192x192.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/img/icons/android-chrome-192x192.png` & `tqsdk-3.4.0/tqsdk/web/img/icons/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/img/icons/msapplication-icon-144x144.png.png` & `tqsdk-3.4.0/tqsdk/web/img/icons/apple-touch-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/img/icons/android-icon-36x36.png` & `tqsdk-3.4.0/tqsdk/web/img/icons/android-icon-36x36.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/img/icons/ms-icon-150x150.png` & `tqsdk-3.4.0/tqsdk/web/img/icons/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/js/chunk-vendors.d7fceff6.js` & `tqsdk-3.4.0/tqsdk/web/js/chunk-vendors.d7fceff6.js`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/web/js/app.2c843c86.js` & `tqsdk-3.4.0/tqsdk/web/js/app.2c843c86.js`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/auth.py` & `tqsdk-3.4.0/tqsdk/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,15 +113,15 @@
                            headers=response.headers, reason=response.reason, text=response.text)
         if response.status_code != 200:
             raise Exception(f"不支持该期货公司 - {broker_id}，请联系期货公司。")
         broker_list = json.loads(response.content)
         if "TQ" not in broker_list[broker_id]["category"]:
             raise Exception(f"该期货公司 - {broker_id} 暂不支持 TqSdk 登录，请联系期货公司。")
 
-        return broker_list[broker_id]["url"], broker_list[broker_id].get('broker_type', 'FUTURE')
+        return broker_list[broker_id]["url"], broker_list[broker_id].get('broker_type', 'FUTURE'), broker_list[broker_id].get('smtype'), broker_list[broker_id].get('smconfig')
 
     def _get_md_url(self, stock, backtest):
         """获取行情网关地址"""
         url = f"https://api.shinnytech.com/ns"
         params = {"stock": str(stock).lower(), "backtest": str(backtest).lower()}
         self._logger.debug("request md url", url=url, params=params, method="POST")
         response = requests.get(url=url, params=params, headers=self._base_headers, timeout=30)
```

### Comparing `tqsdk-3.3.0/tqsdk/data_extension.py` & `tqsdk-3.4.0/tqsdk/data_extension.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/tqwebhelper.py` & `tqsdk-3.4.0/tqsdk/tqwebhelper.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/data_series.py` & `tqsdk-3.4.0/tqsdk/data_series.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/ins_schema.py` & `tqsdk-3.4.0/tqsdk/ins_schema.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/entity.py` & `tqsdk-3.4.0/tqsdk/entity.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/datetime_state.py` & `tqsdk-3.4.0/tqsdk/datetime_state.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/algorithm/twap.py` & `tqsdk-3.4.0/tqsdk/algorithm/twap.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/algorithm/time_table_generater.py` & `tqsdk-3.4.0/tqsdk/algorithm/time_table_generater.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/utils.py` & `tqsdk-3.4.0/tqsdk/utils.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/tutorial/downloader.py` & `tqsdk-3.4.0/tqsdk/demo/tutorial/downloader.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/tutorial/t95.py` & `tqsdk-3.4.0/tqsdk/demo/tutorial/t95.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/tutorial/t60.py` & `tqsdk-3.4.0/tqsdk/demo/tutorial/t60.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/tutorial/t20.py` & `tqsdk-3.4.0/tqsdk/demo/tutorial/t20.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/tutorial/t96.py` & `tqsdk-3.4.0/tqsdk/demo/tutorial/t96.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/tutorial/t70.py` & `tqsdk-3.4.0/tqsdk/demo/tutorial/t70.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/tutorial/t92.py` & `tqsdk-3.4.0/tqsdk/demo/tutorial/t92.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/tutorial/t71.py` & `tqsdk-3.4.0/tqsdk/demo/tutorial/t71.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/tutorial/t72.py` & `tqsdk-3.4.0/tqsdk/demo/tutorial/t72.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/tutorial/t40.py` & `tqsdk-3.4.0/tqsdk/demo/tutorial/t40.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/tutorial/t30.py` & `tqsdk-3.4.0/tqsdk/demo/tutorial/t30.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/tutorial/t90.py` & `tqsdk-3.4.0/tqsdk/demo/tutorial/t90.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/tutorial/t93.py` & `tqsdk-3.4.0/tqsdk/demo/tutorial/t93.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/tutorial/t94.py` & `tqsdk-3.4.0/tqsdk/demo/tutorial/t94.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/tutorial/t41.py` & `tqsdk-3.4.0/tqsdk/demo/tutorial/t41.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/tutorial/t80.py` & `tqsdk-3.4.0/tqsdk/demo/tutorial/t80.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/tutorial/backtest.py` & `tqsdk-3.4.0/tqsdk/demo/tutorial/backtest.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/tutorial/replay.py` & `tqsdk-3.4.0/tqsdk/demo/tutorial/replay.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/tutorial/replay2.py` & `tqsdk-3.4.0/tqsdk/demo/tutorial/replay2.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/tutorial/t91.py` & `tqsdk-3.4.0/tqsdk/demo/tutorial/t91.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/download_orders.py` & `tqsdk-3.4.0/tqsdk/demo/download_orders.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/option_tutorial/o70.py` & `tqsdk-3.4.0/tqsdk/demo/option_tutorial/o70.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/option_tutorial/o40.py` & `tqsdk-3.4.0/tqsdk/demo/option_tutorial/o40.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/option_tutorial/o71.py` & `tqsdk-3.4.0/tqsdk/demo/option_tutorial/o71.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/option_tutorial/o20.py` & `tqsdk-3.4.0/tqsdk/demo/option_tutorial/o20.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/option_tutorial/o74.py` & `tqsdk-3.4.0/tqsdk/demo/option_tutorial/o74.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/option_tutorial/o30.py` & `tqsdk-3.4.0/tqsdk/demo/option_tutorial/o30.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/option_tutorial/o73.py` & `tqsdk-3.4.0/tqsdk/demo/option_tutorial/o73.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/option_tutorial/o41.py` & `tqsdk-3.4.0/tqsdk/demo/option_tutorial/o41.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/option_tutorial/o72.py` & `tqsdk-3.4.0/tqsdk/demo/option_tutorial/o72.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/option_tutorial/o60.py` & `tqsdk-3.4.0/tqsdk/demo/option_tutorial/o60.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/example/rbreaker2.py` & `tqsdk-3.4.0/tqsdk/demo/example/rbreaker2.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/example/gridtrading_async.py` & `tqsdk-3.4.0/tqsdk/demo/example/gridtrading_async.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/example/momentum.py` & `tqsdk-3.4.0/tqsdk/demo/example/momentum.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/example/dualthrust.py` & `tqsdk-3.4.0/tqsdk/demo/example/dualthrust.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/example/aberration.py` & `tqsdk-3.4.0/tqsdk/demo/example/aberration.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/example/turtle.py` & `tqsdk-3.4.0/tqsdk/demo/example/turtle.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/example/vwap.py` & `tqsdk-3.4.0/tqsdk/demo/example/vwap.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/example/fairy_four_price.py` & `tqsdk-3.4.0/tqsdk/demo/example/fairy_four_price.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/example/random_forest.py` & `tqsdk-3.4.0/tqsdk/demo/example/random_forest.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/example/escalator.py` & `tqsdk-3.4.0/tqsdk/demo/example/escalator.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/example/rbreaker.py` & `tqsdk-3.4.0/tqsdk/demo/example/rbreaker.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/example/doublema.py` & `tqsdk-3.4.0/tqsdk/demo/example/doublema.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/example/gridtrading.py` & `tqsdk-3.4.0/tqsdk/demo/example/gridtrading.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/multiaccount.py` & `tqsdk-3.4.0/tqsdk/demo/multiaccount.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/ta.py` & `tqsdk-3.4.0/tqsdk/demo/ta.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/demo/ta_option.py` & `tqsdk-3.4.0/tqsdk/demo/ta_option.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/api.py` & `tqsdk-3.4.0/tqsdk/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1199,15 +1199,15 @@
             单状态: ALIVE, 已成交: 0 手
             单状态: ALIVE, 已成交: 0 手
             单状态: FINISHED, 已成交: 3 手
             ...
 
         Example4::
 
-            # 多账户模式下, 使用不同期货公司交易账户进行下单操作
+            # 多账户模式下, 分别获取各账户的成交记录
             from tqsdk import TqApi, TqAuth, TqMultiAccount
 
             account1 = TqAccount("H海通期货", "123456", "123456")
             account2 = TqAccount("H宏源期货", "123456", "123456")
             with TqApi(TqMultiAccount([account1, account2]), auth=TqAuth("信易账户", "账户密码")) as api:
                 order1 = api.insert_order(symbol="DCE.m2101", direction="BUY", offset="OPEN", volume=3, account=account1)
                 order2 = api.insert_order(symbol="DCE.m2103", direction="BUY", offset="OPEN", volume=3, account=account2)
```

### Comparing `tqsdk-3.3.0/tqsdk/report.py` & `tqsdk-3.4.0/tqsdk/report.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/exceptions.py` & `tqsdk-3.4.0/tqsdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/baseApi.py` & `tqsdk-3.4.0/tqsdk/baseApi.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/objs.py` & `tqsdk-3.4.0/tqsdk/objs.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/multiaccount.py` & `tqsdk-3.4.0/tqsdk/multiaccount.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/ta.py` & `tqsdk-3.4.0/tqsdk/ta.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/channel.py` & `tqsdk-3.4.0/tqsdk/channel.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/symbols.py` & `tqsdk-3.4.0/tqsdk/symbols.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/diff.py` & `tqsdk-3.4.0/tqsdk/diff.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/expired_quotes.json.lzma` & `tqsdk-3.4.0/tqsdk/expired_quotes.json.lzma`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/datetime.py` & `tqsdk-3.4.0/tqsdk/datetime.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/risk_manager.py` & `tqsdk-3.4.0/tqsdk/risk_manager.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/calendar.py` & `tqsdk-3.4.0/tqsdk/calendar.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/baseModule.py` & `tqsdk-3.4.0/tqsdk/baseModule.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/__init__.py` & `tqsdk-3.4.0/tqsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.3.0/tqsdk/utils_symbols.py` & `tqsdk-3.4.0/tqsdk/utils_symbols.py`

 * *Files identical despite different names*

