# Comparing `tmp/pybi-next-0.4.0.tar.gz` & `tmp/pybi-next-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybi-next-0.4.0.tar", last modified: Tue Apr 11 11:15:51 2023, max compression
+gzip compressed data, was "pybi-next-0.4.1.tar", last modified: Thu Apr 13 15:29:47 2023, max compression
```

## Comparing `pybi-next-0.4.0.tar` & `pybi-next-0.4.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 11:15:51.260890 pybi-next-0.4.0/
--rw-rw-rw-   0        0        0     1088 2022-03-21 14:09:44.000000 pybi-next-0.4.0/LICENSE
--rw-rw-rw-   0        0        0      477 2023-04-11 11:15:51.259921 pybi-next-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     2112 2023-03-15 11:07:57.000000 pybi-next-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 11:15:51.125437 pybi-next-0.4.0/pybi/
--rw-rw-rw-   0        0        0     1653 2023-04-11 10:54:25.000000 pybi-next-0.4.0/pybi/__index.py
--rw-rw-rw-   0        0        0       49 2023-04-11 11:13:39.000000 pybi-next-0.4.0/pybi/__init__.py
--rw-rw-rw-   0        0        0    18405 2023-04-11 10:54:25.000000 pybi-next-0.4.0/pybi/app.py
-drwxrwxrwx   0        0        0        0 2023-04-11 11:15:51.134387 pybi-next-0.4.0/pybi/core/
--rw-rw-rw-   0        0        0       81 2023-03-15 11:07:57.000000 pybi-next-0.4.0/pybi/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 11:15:51.145745 pybi-next-0.4.0/pybi/core/components/
--rw-rw-rw-   0        0        0      631 2023-03-30 15:24:18.000000 pybi-next-0.4.0/pybi/core/components/__init__.py
--rw-rw-rw-   0        0        0     2118 2023-03-29 14:36:39.000000 pybi-next-0.4.0/pybi/core/components/component.py
--rw-rw-rw-   0        0        0      532 2023-03-30 15:24:18.000000 pybi-next-0.4.0/pybi/core/components/componentTag.py
--rw-rw-rw-   0        0        0     7854 2023-04-11 10:54:25.000000 pybi-next-0.4.0/pybi/core/components/containerComponent.py
--rw-rw-rw-   0        0        0      406 2023-03-29 16:16:41.000000 pybi-next-0.4.0/pybi/core/components/mermaid.py
-drwxrwxrwx   0        0        0        0 2023-04-11 11:15:51.163697 pybi-next-0.4.0/pybi/core/components/reactiveComponent/
--rw-rw-rw-   0        0        0      214 2023-03-30 06:02:37.000000 pybi-next-0.4.0/pybi/core/components/reactiveComponent/__init__.py
--rw-rw-rw-   0        0        0     1341 2023-03-15 11:07:57.000000 pybi-next-0.4.0/pybi/core/components/reactiveComponent/base.py
--rw-rw-rw-   0        0        0     5142 2023-04-11 10:54:25.000000 pybi-next-0.4.0/pybi/core/components/reactiveComponent/echarts.py
--rw-rw-rw-   0        0        0      695 2023-03-29 18:02:26.000000 pybi-next-0.4.0/pybi/core/components/reactiveComponent/input.py
--rw-rw-rw-   0        0        0      695 2023-03-15 11:07:57.000000 pybi-next-0.4.0/pybi/core/components/reactiveComponent/markdown.py
--rw-rw-rw-   0        0        0      644 2023-03-30 06:02:37.000000 pybi-next-0.4.0/pybi/core/components/reactiveComponent/numberSlider.py
--rw-rw-rw-   0        0        0      930 2023-03-15 11:07:57.000000 pybi-next-0.4.0/pybi/core/components/reactiveComponent/slicer.py
--rw-rw-rw-   0        0        0     1224 2023-03-15 11:07:57.000000 pybi-next-0.4.0/pybi/core/components/reactiveComponent/table.py
--rw-rw-rw-   0        0        0      428 2023-03-15 11:07:57.000000 pybi-next-0.4.0/pybi/core/components/reactiveComponent/textValue.py
--rw-rw-rw-   0        0        0     1008 2023-04-11 10:54:25.000000 pybi-next-0.4.0/pybi/core/components/staticComponent.py
--rw-rw-rw-   0        0        0     6135 2023-03-15 11:07:57.000000 pybi-next-0.4.0/pybi/core/dataSource.py
--rw-rw-rw-   0        0        0     5349 2023-04-11 10:54:25.000000 pybi-next-0.4.0/pybi/core/sql.py
-drwxrwxrwx   0        0        0        0 2023-04-11 11:15:51.169712 pybi-next-0.4.0/pybi/core/styles/
--rw-rw-rw-   0        0        0      714 2023-02-15 14:58:33.000000 pybi-next-0.4.0/pybi/core/styles/__init__.py
--rw-rw-rw-   0        0        0     3552 2023-02-15 04:29:42.000000 pybi-next-0.4.0/pybi/core/styles/styles.py
-drwxrwxrwx   0        0        0        0 2023-04-11 11:15:51.178657 pybi-next-0.4.0/pybi/core/styles/tailwindStyles/
--rw-rw-rw-   0        0        0        0 2023-02-15 15:24:16.000000 pybi-next-0.4.0/pybi/core/styles/tailwindStyles/__init__.py
--rw-rw-rw-   0        0        0     1069 2023-02-15 14:58:33.000000 pybi-next-0.4.0/pybi/core/styles/tailwindStyles/boxShadow.py
--rw-rw-rw-   0        0        0      578 2023-02-15 14:58:33.000000 pybi-next-0.4.0/pybi/core/styles/tailwindStyles/textAlign.py
--rw-rw-rw-   0        0        0    21147 2023-02-15 14:58:33.000000 pybi-next-0.4.0/pybi/core/styles/tailwindStyles/textColor.py
--rw-rw-rw-   0        0        0     1458 2023-02-15 14:58:33.000000 pybi-next-0.4.0/pybi/core/styles/tailwindStyles/textSize.py
--rw-rw-rw-   0        0        0       95 2023-01-31 06:42:57.000000 pybi-next-0.4.0/pybi/core/styles/utils.py
--rw-rw-rw-   0        0        0     3602 2023-04-11 10:54:25.000000 pybi-next-0.4.0/pybi/core/uiResource.py
--rw-rw-rw-   0        0        0     1461 2023-04-11 10:54:25.000000 pybi-next-0.4.0/pybi/core/webResources.py
-drwxrwxrwx   0        0        0        0 2023-04-11 11:15:51.193617 pybi-next-0.4.0/pybi/easyEcharts/
--rw-rw-rw-   0        0        0     1944 2023-04-11 10:54:25.000000 pybi-next-0.4.0/pybi/easyEcharts/__init__.py
--rw-rw-rw-   0        0        0     3222 2023-04-11 11:03:46.000000 pybi-next-0.4.0/pybi/easyEcharts/bar.py
--rw-rw-rw-   0        0        0     3592 2023-04-11 11:04:22.000000 pybi-next-0.4.0/pybi/easyEcharts/base.py
--rw-rw-rw-   0        0        0     3334 2023-04-11 11:04:42.000000 pybi-next-0.4.0/pybi/easyEcharts/line.py
--rw-rw-rw-   0        0        0     1723 2023-04-11 10:54:25.000000 pybi-next-0.4.0/pybi/easyEcharts/map.py
--rw-rw-rw-   0        0        0     2468 2023-04-11 11:04:47.000000 pybi-next-0.4.0/pybi/easyEcharts/pie.py
--rw-rw-rw-   0        0        0     1965 2023-04-11 11:04:51.000000 pybi-next-0.4.0/pybi/easyEcharts/scatter.py
--rw-rw-rw-   0        0        0     2598 2023-04-11 11:03:46.000000 pybi-next-0.4.0/pybi/easyEcharts/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-11 11:15:51.199603 pybi-next-0.4.0/pybi/icons/
--rw-rw-rw-   0        0        0        0 2023-04-11 10:54:25.000000 pybi-next-0.4.0/pybi/icons/__init__.py
--rw-rw-rw-   0        0        0      700 2023-04-11 10:54:25.000000 pybi-next-0.4.0/pybi/icons/iconManager.py
--rw-rw-rw-   0        0        0   923783 2023-04-11 10:54:25.000000 pybi-next-0.4.0/pybi/icons/material_icons.py
-drwxrwxrwx   0        0        0        0 2023-04-11 11:15:51.230519 pybi-next-0.4.0/pybi/static/
--rw-rw-rw-   0        0        0  1022898 2023-03-14 04:09:02.000000 pybi-next-0.4.0/pybi/static/echarts.min.js
--rw-rw-rw-   0        0        0      468 2023-04-07 14:51:23.000000 pybi-next-0.4.0/pybi/static/echartsCps-style.css
--rw-rw-rw-   0        0        0    27467 2023-04-07 14:51:23.000000 pybi-next-0.4.0/pybi/static/echartsCps.iife.js
--rw-rw-rw-   0        0        0   119709 2023-04-07 14:51:23.000000 pybi-next-0.4.0/pybi/static/elementCps-style.css
--rw-rw-rw-   0        0        0   349813 2023-04-07 14:51:23.000000 pybi-next-0.4.0/pybi/static/elementCps.iife.js
--rw-rw-rw-   0        0        0  2778154 2023-04-07 14:51:23.000000 pybi-next-0.4.0/pybi/static/mermaidCps.iife.js
--rw-rw-rw-   0        0        0   582522 2023-04-06 17:22:15.000000 pybi-next-0.4.0/pybi/static/province_map_full.json
--rw-rw-rw-   0        0        0     2000 2023-04-07 14:51:23.000000 pybi-next-0.4.0/pybi/static/sysApp-style.css
--rw-rw-rw-   0        0        0  1012054 2023-04-07 14:51:23.000000 pybi-next-0.4.0/pybi/static/sysApp.iife.js
--rw-rw-rw-   0        0        0   125849 2023-03-23 06:49:54.000000 pybi-next-0.4.0/pybi/static/vue.global.prod.min.js
-drwxrwxrwx   0        0        0        0 2023-04-11 11:15:51.232513 pybi-next-0.4.0/pybi/template/
--rw-rw-rw-   0        0        0     1535 2023-04-11 10:54:25.000000 pybi-next-0.4.0/pybi/template/index.html
-drwxrwxrwx   0        0        0        0 2023-04-11 11:15:51.248470 pybi-next-0.4.0/pybi/utils/
--rw-rw-rw-   0        0        0        0 2022-05-17 15:58:12.000000 pybi-next-0.4.0/pybi/utils/__init__.py
--rw-rw-rw-   0        0        0     1545 2023-02-16 03:08:31.000000 pybi-next-0.4.0/pybi/utils/dataSourceUtils.py
--rw-rw-rw-   0        0        0     3056 2023-03-29 14:36:39.000000 pybi-next-0.4.0/pybi/utils/data_gen.py
--rw-rw-rw-   0        0        0     1624 2023-02-11 14:46:57.000000 pybi-next-0.4.0/pybi/utils/dictUtils.py
--rw-rw-rw-   0        0        0     1931 2023-03-18 09:54:06.000000 pybi-next-0.4.0/pybi/utils/echarts_opts_utils.py
--rw-rw-rw-   0        0        0      851 2022-05-17 15:58:12.000000 pybi-next-0.4.0/pybi/utils/helper.py
--rw-rw-rw-   0        0        0   116803 2022-05-17 15:58:12.000000 pybi-next-0.4.0/pybi/utils/markdown2.py
--rw-rw-rw-   0        0        0     2883 2023-03-15 11:07:57.000000 pybi-next-0.4.0/pybi/utils/pyecharts_utils.py
--rw-rw-rw-   0        0        0     1398 2023-03-15 11:07:57.000000 pybi-next-0.4.0/pybi/utils/sql.py
-drwxrwxrwx   0        0        0        0 2023-04-11 11:15:51.258893 pybi-next-0.4.0/pybi_next.egg-info/
--rw-rw-rw-   0        0        0      477 2023-04-11 11:15:50.000000 pybi-next-0.4.0/pybi_next.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2201 2023-04-11 11:15:50.000000 pybi-next-0.4.0/pybi_next.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 11:15:50.000000 pybi-next-0.4.0/pybi_next.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-15 04:57:05.000000 pybi-next-0.4.0/pybi_next.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       25 2023-04-11 11:15:50.000000 pybi-next-0.4.0/pybi_next.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-11 11:15:50.000000 pybi-next-0.4.0/pybi_next.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 11:15:51.260890 pybi-next-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1590 2023-03-29 14:36:39.000000 pybi-next-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 15:29:47.487250 pybi-next-0.4.1/
+-rw-rw-rw-   0        0        0     1088 2022-03-21 14:09:44.000000 pybi-next-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0      477 2023-04-13 15:29:47.475634 pybi-next-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2112 2023-03-15 11:07:57.000000 pybi-next-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 15:29:47.086263 pybi-next-0.4.1/pybi/
+-rw-rw-rw-   0        0        0     1653 2023-04-11 10:54:25.000000 pybi-next-0.4.1/pybi/__index.py
+-rw-rw-rw-   0        0        0       49 2023-04-13 15:29:16.000000 pybi-next-0.4.1/pybi/__init__.py
+-rw-rw-rw-   0        0        0    18405 2023-04-11 10:54:25.000000 pybi-next-0.4.1/pybi/app.py
+drwxrwxrwx   0        0        0        0 2023-04-13 15:29:47.134252 pybi-next-0.4.1/pybi/core/
+-rw-rw-rw-   0        0        0       81 2023-03-15 11:07:57.000000 pybi-next-0.4.1/pybi/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 15:29:47.170912 pybi-next-0.4.1/pybi/core/components/
+-rw-rw-rw-   0        0        0      631 2023-03-30 15:24:18.000000 pybi-next-0.4.1/pybi/core/components/__init__.py
+-rw-rw-rw-   0        0        0     2118 2023-03-29 14:36:39.000000 pybi-next-0.4.1/pybi/core/components/component.py
+-rw-rw-rw-   0        0        0      532 2023-03-30 15:24:18.000000 pybi-next-0.4.1/pybi/core/components/componentTag.py
+-rw-rw-rw-   0        0        0     7870 2023-04-11 12:28:53.000000 pybi-next-0.4.1/pybi/core/components/containerComponent.py
+-rw-rw-rw-   0        0        0      406 2023-03-29 16:16:41.000000 pybi-next-0.4.1/pybi/core/components/mermaid.py
+drwxrwxrwx   0        0        0        0 2023-04-13 15:29:47.213806 pybi-next-0.4.1/pybi/core/components/reactiveComponent/
+-rw-rw-rw-   0        0        0      214 2023-03-30 06:02:37.000000 pybi-next-0.4.1/pybi/core/components/reactiveComponent/__init__.py
+-rw-rw-rw-   0        0        0     1341 2023-03-15 11:07:57.000000 pybi-next-0.4.1/pybi/core/components/reactiveComponent/base.py
+-rw-rw-rw-   0        0        0     5142 2023-04-11 10:54:25.000000 pybi-next-0.4.1/pybi/core/components/reactiveComponent/echarts.py
+-rw-rw-rw-   0        0        0      695 2023-03-29 18:02:26.000000 pybi-next-0.4.1/pybi/core/components/reactiveComponent/input.py
+-rw-rw-rw-   0        0        0      695 2023-03-15 11:07:57.000000 pybi-next-0.4.1/pybi/core/components/reactiveComponent/markdown.py
+-rw-rw-rw-   0        0        0      644 2023-03-30 06:02:37.000000 pybi-next-0.4.1/pybi/core/components/reactiveComponent/numberSlider.py
+-rw-rw-rw-   0        0        0      930 2023-03-15 11:07:57.000000 pybi-next-0.4.1/pybi/core/components/reactiveComponent/slicer.py
+-rw-rw-rw-   0        0        0     1224 2023-03-15 11:07:57.000000 pybi-next-0.4.1/pybi/core/components/reactiveComponent/table.py
+-rw-rw-rw-   0        0        0      428 2023-03-15 11:07:57.000000 pybi-next-0.4.1/pybi/core/components/reactiveComponent/textValue.py
+-rw-rw-rw-   0        0        0     1008 2023-04-11 10:54:25.000000 pybi-next-0.4.1/pybi/core/components/staticComponent.py
+-rw-rw-rw-   0        0        0     6135 2023-03-15 11:07:57.000000 pybi-next-0.4.1/pybi/core/dataSource.py
+-rw-rw-rw-   0        0        0     5349 2023-04-11 10:54:25.000000 pybi-next-0.4.1/pybi/core/sql.py
+drwxrwxrwx   0        0        0        0 2023-04-13 15:29:47.222782 pybi-next-0.4.1/pybi/core/styles/
+-rw-rw-rw-   0        0        0      714 2023-02-15 14:58:33.000000 pybi-next-0.4.1/pybi/core/styles/__init__.py
+-rw-rw-rw-   0        0        0     3552 2023-02-15 04:29:42.000000 pybi-next-0.4.1/pybi/core/styles/styles.py
+drwxrwxrwx   0        0        0        0 2023-04-13 15:29:47.233752 pybi-next-0.4.1/pybi/core/styles/tailwindStyles/
+-rw-rw-rw-   0        0        0        0 2023-02-15 15:24:16.000000 pybi-next-0.4.1/pybi/core/styles/tailwindStyles/__init__.py
+-rw-rw-rw-   0        0        0     1069 2023-02-15 14:58:33.000000 pybi-next-0.4.1/pybi/core/styles/tailwindStyles/boxShadow.py
+-rw-rw-rw-   0        0        0      578 2023-02-15 14:58:33.000000 pybi-next-0.4.1/pybi/core/styles/tailwindStyles/textAlign.py
+-rw-rw-rw-   0        0        0    21147 2023-02-15 14:58:33.000000 pybi-next-0.4.1/pybi/core/styles/tailwindStyles/textColor.py
+-rw-rw-rw-   0        0        0     1458 2023-02-15 14:58:33.000000 pybi-next-0.4.1/pybi/core/styles/tailwindStyles/textSize.py
+-rw-rw-rw-   0        0        0       95 2023-01-31 06:42:57.000000 pybi-next-0.4.1/pybi/core/styles/utils.py
+-rw-rw-rw-   0        0        0     3602 2023-04-11 10:54:25.000000 pybi-next-0.4.1/pybi/core/uiResource.py
+-rw-rw-rw-   0        0        0     1461 2023-04-11 10:54:25.000000 pybi-next-0.4.1/pybi/core/webResources.py
+drwxrwxrwx   0        0        0        0 2023-04-13 15:29:47.248740 pybi-next-0.4.1/pybi/easyEcharts/
+-rw-rw-rw-   0        0        0     2090 2023-04-13 15:22:20.000000 pybi-next-0.4.1/pybi/easyEcharts/__init__.py
+-rw-rw-rw-   0        0        0     3350 2023-04-13 15:22:20.000000 pybi-next-0.4.1/pybi/easyEcharts/bar.py
+-rw-rw-rw-   0        0        0     3592 2023-04-11 11:04:22.000000 pybi-next-0.4.1/pybi/easyEcharts/base.py
+-rw-rw-rw-   0        0        0     3462 2023-04-13 15:22:20.000000 pybi-next-0.4.1/pybi/easyEcharts/line.py
+-rw-rw-rw-   0        0        0     1723 2023-04-11 10:54:25.000000 pybi-next-0.4.1/pybi/easyEcharts/map.py
+-rw-rw-rw-   0        0        0     2468 2023-04-11 11:04:47.000000 pybi-next-0.4.1/pybi/easyEcharts/pie.py
+-rw-rw-rw-   0        0        0     1965 2023-04-11 11:04:51.000000 pybi-next-0.4.1/pybi/easyEcharts/scatter.py
+-rw-rw-rw-   0        0        0     2598 2023-04-11 11:03:46.000000 pybi-next-0.4.1/pybi/easyEcharts/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 15:29:47.253699 pybi-next-0.4.1/pybi/icons/
+-rw-rw-rw-   0        0        0        0 2023-04-11 10:54:25.000000 pybi-next-0.4.1/pybi/icons/__init__.py
+-rw-rw-rw-   0        0        0      700 2023-04-11 10:54:25.000000 pybi-next-0.4.1/pybi/icons/iconManager.py
+-rw-rw-rw-   0        0        0   923783 2023-04-11 10:54:25.000000 pybi-next-0.4.1/pybi/icons/material_icons.py
+drwxrwxrwx   0        0        0        0 2023-04-13 15:29:47.414827 pybi-next-0.4.1/pybi/static/
+-rw-rw-rw-   0        0        0  1022898 2023-03-14 04:09:02.000000 pybi-next-0.4.1/pybi/static/echarts.min.js
+-rw-rw-rw-   0        0        0      468 2023-04-07 14:51:23.000000 pybi-next-0.4.1/pybi/static/echartsCps-style.css
+-rw-rw-rw-   0        0        0    27467 2023-04-07 14:51:23.000000 pybi-next-0.4.1/pybi/static/echartsCps.iife.js
+-rw-rw-rw-   0        0        0   119709 2023-04-07 14:51:23.000000 pybi-next-0.4.1/pybi/static/elementCps-style.css
+-rw-rw-rw-   0        0        0   349813 2023-04-07 14:51:23.000000 pybi-next-0.4.1/pybi/static/elementCps.iife.js
+-rw-rw-rw-   0        0        0  2778154 2023-04-07 14:51:23.000000 pybi-next-0.4.1/pybi/static/mermaidCps.iife.js
+-rw-rw-rw-   0        0        0   582522 2023-04-06 17:22:15.000000 pybi-next-0.4.1/pybi/static/province_map_full.json
+-rw-rw-rw-   0        0        0     2000 2023-04-07 14:51:23.000000 pybi-next-0.4.1/pybi/static/sysApp-style.css
+-rw-rw-rw-   0        0        0  1012054 2023-04-07 14:51:23.000000 pybi-next-0.4.1/pybi/static/sysApp.iife.js
+-rw-rw-rw-   0        0        0   125849 2023-03-23 06:49:54.000000 pybi-next-0.4.1/pybi/static/vue.global.prod.min.js
+drwxrwxrwx   0        0        0        0 2023-04-13 15:29:47.416821 pybi-next-0.4.1/pybi/template/
+-rw-rw-rw-   0        0        0     1535 2023-04-11 10:54:25.000000 pybi-next-0.4.1/pybi/template/index.html
+drwxrwxrwx   0        0        0        0 2023-04-13 15:29:47.434802 pybi-next-0.4.1/pybi/utils/
+-rw-rw-rw-   0        0        0        0 2022-05-17 15:58:12.000000 pybi-next-0.4.1/pybi/utils/__init__.py
+-rw-rw-rw-   0        0        0     1545 2023-02-16 03:08:31.000000 pybi-next-0.4.1/pybi/utils/dataSourceUtils.py
+-rw-rw-rw-   0        0        0     3056 2023-03-29 14:36:39.000000 pybi-next-0.4.1/pybi/utils/data_gen.py
+-rw-rw-rw-   0        0        0     1624 2023-02-11 14:46:57.000000 pybi-next-0.4.1/pybi/utils/dictUtils.py
+-rw-rw-rw-   0        0        0     1931 2023-03-18 09:54:06.000000 pybi-next-0.4.1/pybi/utils/echarts_opts_utils.py
+-rw-rw-rw-   0        0        0      851 2022-05-17 15:58:12.000000 pybi-next-0.4.1/pybi/utils/helper.py
+-rw-rw-rw-   0        0        0   116803 2022-05-17 15:58:12.000000 pybi-next-0.4.1/pybi/utils/markdown2.py
+-rw-rw-rw-   0        0        0     2883 2023-03-15 11:07:57.000000 pybi-next-0.4.1/pybi/utils/pyecharts_utils.py
+-rw-rw-rw-   0        0        0     1398 2023-03-15 11:07:57.000000 pybi-next-0.4.1/pybi/utils/sql.py
+drwxrwxrwx   0        0        0        0 2023-04-13 15:29:47.473612 pybi-next-0.4.1/pybi_next.egg-info/
+-rw-rw-rw-   0        0        0      477 2023-04-13 15:29:45.000000 pybi-next-0.4.1/pybi_next.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2201 2023-04-13 15:29:46.000000 pybi-next-0.4.1/pybi_next.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 15:29:45.000000 pybi-next-0.4.1/pybi_next.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-02-15 04:57:05.000000 pybi-next-0.4.1/pybi_next.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       25 2023-04-13 15:29:45.000000 pybi-next-0.4.1/pybi_next.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-13 15:29:45.000000 pybi-next-0.4.1/pybi_next.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 15:29:47.488067 pybi-next-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1590 2023-03-29 14:36:39.000000 pybi-next-0.4.1/setup.py
```

### Comparing `pybi-next-0.4.0/LICENSE` & `pybi-next-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/README.md` & `pybi-next-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/__index.py` & `pybi-next-0.4.1/pybi/__index.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/app.py` & `pybi-next-0.4.1/pybi/app.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/core/components/__init__.py` & `pybi-next-0.4.1/pybi/core/components/__init__.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/core/components/component.py` & `pybi-next-0.4.1/pybi/core/components/component.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/core/components/componentTag.py` & `pybi-next-0.4.1/pybi/core/components/componentTag.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/core/components/containerComponent.py` & `pybi-next-0.4.1/pybi/core/components/containerComponent.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,40 +75,40 @@
 
     def _to_json_dict(self):
         data = super()._to_json_dict()
         data["areas"] = GridBoxComponent.areas_array2str(self.__areas)
 
         areas_cols_len = max(map(len, self.__areas))
         cols_size = GridBoxComponent.padded_grid_template(
-            self.__columns_sizes, areas_cols_len
+            self.__columns_sizes, areas_cols_len, "1fr"
         )
 
         areas_rows_len = len(self.__areas)
         rows_size = GridBoxComponent.padded_grid_template(
             self.__rows_sizes, areas_rows_len
         )
 
         data["gridTemplateColumns"] = " ".join(cols_size)
         data["gridTemplateRows"] = " ".join(rows_size)
 
         return data
 
     @staticmethod
-    def padded_grid_template(sizes: List[str], real_size: int):
+    def padded_grid_template(sizes: List[str], real_size: int, pad="auto"):
         """
-        >>> sizes = ['1rf']
+        >>> sizes = ['1fr']
         >>> real_size = 3
         >>> padded_grid_template(sizes,real_size)
-        >>> ['1rf','auto','auto']
+        >>> ['1fr','auto','auto']
         """
         diff_len = real_size - len(sizes)
         sizes = sizes.copy()
 
         if diff_len > 0:
-            sizes.extend(["auto"] * diff_len)
+            sizes.extend([pad] * diff_len)
         return sizes
 
     @staticmethod
     def areas_array2str(areas_array: List[List[str]]):
         """
         >>> input = [
             ["sc1", "sc2"],
```

### Comparing `pybi-next-0.4.0/pybi/core/components/reactiveComponent/base.py` & `pybi-next-0.4.1/pybi/core/components/reactiveComponent/base.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/core/components/reactiveComponent/echarts.py` & `pybi-next-0.4.1/pybi/core/components/reactiveComponent/echarts.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/core/components/reactiveComponent/input.py` & `pybi-next-0.4.1/pybi/core/components/reactiveComponent/input.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/core/components/reactiveComponent/markdown.py` & `pybi-next-0.4.1/pybi/core/components/reactiveComponent/markdown.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/core/components/reactiveComponent/numberSlider.py` & `pybi-next-0.4.1/pybi/core/components/reactiveComponent/numberSlider.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/core/components/reactiveComponent/slicer.py` & `pybi-next-0.4.1/pybi/core/components/reactiveComponent/slicer.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/core/components/reactiveComponent/table.py` & `pybi-next-0.4.1/pybi/core/components/reactiveComponent/table.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/core/components/staticComponent.py` & `pybi-next-0.4.1/pybi/core/components/staticComponent.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/core/dataSource.py` & `pybi-next-0.4.1/pybi/core/dataSource.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/core/sql.py` & `pybi-next-0.4.1/pybi/core/sql.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/core/styles/__init__.py` & `pybi-next-0.4.1/pybi/core/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/core/styles/styles.py` & `pybi-next-0.4.1/pybi/core/styles/styles.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/core/styles/tailwindStyles/boxShadow.py` & `pybi-next-0.4.1/pybi/core/styles/tailwindStyles/boxShadow.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/core/styles/tailwindStyles/textAlign.py` & `pybi-next-0.4.1/pybi/core/styles/tailwindStyles/textAlign.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/core/styles/tailwindStyles/textColor.py` & `pybi-next-0.4.1/pybi/core/styles/tailwindStyles/textColor.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/core/styles/tailwindStyles/textSize.py` & `pybi-next-0.4.1/pybi/core/styles/tailwindStyles/textSize.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/core/uiResource.py` & `pybi-next-0.4.1/pybi/core/uiResource.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/core/webResources.py` & `pybi-next-0.4.1/pybi/core/webResources.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/easyEcharts/__init__.py` & `pybi-next-0.4.1/pybi/easyEcharts/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,27 +33,31 @@
     def make_line(
         self,
         data: DataSourceTable,
         x: str,
         y: str,
         color: Optional[str] = None,
         agg="round(avg(${}),2)",
+        order: Optional[str] = None,
     ):
-        return LineChart(data, x, y, color, agg)
+        order = order or x
+        return LineChart(data, x, y, order, color, agg)
 
     def make_bar(
         self,
         data: DataSourceTable,
         *,
         x: str,
         y: str,
         color: Optional[str] = None,
         agg="round(avg(${}),2)",
+        order: Optional[str] = None,
     ):
-        return BarChart(data, x, y, color, agg)
+        order = order or x
+        return BarChart(data, x, y, order, color, agg)
 
     def make_pie(
         self,
         data: DataSourceTable,
         *,
         name: str,
         value: str,
```

### Comparing `pybi-next-0.4.0/pybi/easyEcharts/bar.py` & `pybi-next-0.4.1/pybi/easyEcharts/bar.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,21 +14,23 @@
 
 class BarChart(BaseChart):
     def __init__(
         self,
         data: DataSourceTable,
         x: str,
         y: str,
+        order: str,
         color: Optional[str] = None,
         agg="round(avg(${}),2)",
     ):
         super().__init__()
         self.data = data
         self.x = x
         self.y = y
+        self.order = order or x
         self.color = color
         self.agg = agg
         self._reverse_axis = False
         self._series_configs = {}
 
     def reverse_axis(self):
         self._reverse_axis = True
@@ -55,54 +57,54 @@
             "series": [],
         }
         base_opt.update(opts)
 
         sql = ""
         agg_field = f"{sqlUtils.apply_agg(self.agg, self.y)} as {self.y}"
         if self.color:
-            sql = f"select {self.x},{agg_field},{self.color} from {self.data} group by {self.color},{self.x}"
+            sql = f"select {self.x},{agg_field},{self.color},{self.order} from {self.data} group by {self.color},{self.x}"
         else:
-            sql = f"select {self.x},{agg_field} from {self.data} group by {self.x}"
+            sql = f"select {self.x},{agg_field},{self.order} from {self.data} group by {self.x}"
 
         dv = pbi.set_dataView(sql)
 
         if self.color:
             row_map_x, row_map_y = "r[fields[0]]", "r[fields[1]]"
             if self._reverse_axis:
                 row_map_x, row_map_y = row_map_y, row_map_x
 
             base_opt["series"] = pbi.sql(
-                f"select {self.x},{self.y},{self.color} from {dv}"
+                f"select {self.x},{self.y},{self.color} from {dv} order by {self.order}"
             ).split_group(
                 self.color,
                 f"""
                 const data = rows.map(r=> [{row_map_x},{row_map_y}])
                 return {{id:key,data,type:'bar',name:key,universalTransition: {{enabled: true, divideShape: 'clone'}}}}""",
             )
         else:
             base_opt["series"].append(
                 {
                     "name": self.x,
                     "type": "bar",
                     "id": self.x,
                     "data": pbi.sql(
-                        f"select {self.y} as value,{self.x} as groupId from {dv}"
+                        f"select {self.y} as value,{self.x} as groupId from {dv} order by {self.order}"
                     ),
                     "universalTransition": {"enabled": True, "divideShape": "clone"},
                 }
             )
 
         catAxis = base_opt["xAxis"][0]
         valueAxis = base_opt["yAxis"][0]
 
         if self._reverse_axis:
             catAxis, valueAxis = valueAxis, catAxis
 
         catAxis["data"] = pbi.sql(
-            f"select distinct {self.x} from {dv} order by {self.x}"
+            f"select distinct {self.x} from {dv} order by {self.order}"
         ).toflatlist()
         catAxis["type"] = "category"
         valueAxis["type"] = "value"
 
         base_opt = self._post_options(base_opt)
 
         return base_opt, self._updateInfos, []
```

### Comparing `pybi-next-0.4.0/pybi/easyEcharts/base.py` & `pybi-next-0.4.1/pybi/easyEcharts/base.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/easyEcharts/line.py` & `pybi-next-0.4.1/pybi/easyEcharts/line.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,21 +11,23 @@
 
 class LineChart(BaseChart):
     def __init__(
         self,
         data: DataSourceTable,
         x: str,
         y: str,
+        order: str,
         color: Optional[str] = None,
         agg="round(avg(${}),2)",
     ):
         super().__init__()
         self.data = data
         self.x = x
         self.y = y
+        self.order = order or x
         self.color = color
         self.agg = agg
         self._series_configs = {}
         self._xAxis = {}
 
     def stack(self):
         self._series_configs["stack"] = "Total"
@@ -59,47 +61,47 @@
             "series": [],
         }
         base_opt.update(opts)
 
         sql = ""
         agg_field = f"{sqlUtils.apply_agg(self.agg, self.y)} as {self.y}"
         if self.color:
-            sql = f"select {self.x},{agg_field},{self.color} from {self.data} group by {self.color},{self.x}"
+            sql = f"select {self.x},{agg_field},{self.color},{self.order} from {self.data} group by {self.color},{self.x}"
         else:
-            sql = f"select {self.x},{agg_field} from {self.data} group by {self.x}"
+            sql = f"select {self.x},{agg_field},{self.order} from {self.data} group by {self.x}"
 
         dv = pbi.set_dataView(sql)
 
         if self.color:
             base_opt["series"] = pbi.sql(
-                f"select {self.x},{self.y},{self.color} from {dv}"
+                f"select {self.x},{self.y},{self.color} from {dv} order by {self.order}"
             ).split_group(
                 self.color,
                 """
                 const data = rows.map(r=> [r[fields[0]],r[fields[1]]])
                 return {id:key,data,type:'line',name:key,universalTransition: {enabled: true}}""",
             )
         else:
             base_opt["series"].append(
                 {
                     "name": self.x,
                     "id": self.x,
                     "universalTransition": {"enabled": True, "divideShape": "clone"},
                     "type": "line",
                     "data": pbi.sql(
-                        f"select {self.y} as value,{self.x} as groupId from {dv}"
+                        f"select {self.y} as value,{self.x} as groupId from {dv} order by {self.order}"
                     ),
                 }
             )
 
         catAxis = base_opt["xAxis"][0]
         valueAxis = base_opt["yAxis"][0]
 
         catAxis["data"] = pbi.sql(
-            f"select distinct {self.x} from {dv} order by {self.x}"
+            f"select distinct {self.x} from {dv} order by {self.order}"
         ).toflatlist()
         catAxis.update(self._xAxis)
         # catAxis["axisLabel"] = {"formatter": "{value}月"}
         catAxis["boundaryGap"] = False
         valueAxis["type"] = "value"
 
         opts["tooltip"] = {
```

### Comparing `pybi-next-0.4.0/pybi/easyEcharts/map.py` & `pybi-next-0.4.1/pybi/easyEcharts/map.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/easyEcharts/pie.py` & `pybi-next-0.4.1/pybi/easyEcharts/pie.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/easyEcharts/scatter.py` & `pybi-next-0.4.1/pybi/easyEcharts/scatter.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/easyEcharts/utils.py` & `pybi-next-0.4.1/pybi/easyEcharts/utils.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/icons/iconManager.py` & `pybi-next-0.4.1/pybi/icons/iconManager.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/icons/material_icons.py` & `pybi-next-0.4.1/pybi/icons/material_icons.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/static/echarts.min.js` & `pybi-next-0.4.1/pybi/static/echarts.min.js`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/static/echartsCps.iife.js` & `pybi-next-0.4.1/pybi/static/echartsCps.iife.js`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/static/elementCps-style.css` & `pybi-next-0.4.1/pybi/static/elementCps-style.css`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/static/elementCps.iife.js` & `pybi-next-0.4.1/pybi/static/elementCps.iife.js`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/static/mermaidCps.iife.js` & `pybi-next-0.4.1/pybi/static/mermaidCps.iife.js`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/static/province_map_full.json` & `pybi-next-0.4.1/pybi/static/province_map_full.json`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/static/sysApp-style.css` & `pybi-next-0.4.1/pybi/static/sysApp-style.css`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/static/sysApp.iife.js` & `pybi-next-0.4.1/pybi/static/sysApp.iife.js`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/static/vue.global.prod.min.js` & `pybi-next-0.4.1/pybi/static/vue.global.prod.min.js`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/template/index.html` & `pybi-next-0.4.1/pybi/template/index.html`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/utils/dataSourceUtils.py` & `pybi-next-0.4.1/pybi/utils/dataSourceUtils.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/utils/data_gen.py` & `pybi-next-0.4.1/pybi/utils/data_gen.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/utils/dictUtils.py` & `pybi-next-0.4.1/pybi/utils/dictUtils.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/utils/echarts_opts_utils.py` & `pybi-next-0.4.1/pybi/utils/echarts_opts_utils.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/utils/helper.py` & `pybi-next-0.4.1/pybi/utils/helper.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/utils/markdown2.py` & `pybi-next-0.4.1/pybi/utils/markdown2.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/utils/pyecharts_utils.py` & `pybi-next-0.4.1/pybi/utils/pyecharts_utils.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi/utils/sql.py` & `pybi-next-0.4.1/pybi/utils/sql.py`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/pybi_next.egg-info/SOURCES.txt` & `pybi-next-0.4.1/pybi_next.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybi-next-0.4.0/setup.py` & `pybi-next-0.4.1/setup.py`

 * *Files identical despite different names*

