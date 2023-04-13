# Comparing `tmp/mkdocs-risonia-theme-0.1.5.tar.gz` & `tmp/mkdocs-risonia-theme-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-risonia-theme-0.1.5.tar", last modified: Fri Jan 20 15:57:37 2023, max compression
+gzip compressed data, was "mkdocs-risonia-theme-0.1.6.tar", last modified: Thu Apr 13 14:42:33 2023, max compression
```

## Comparing `mkdocs-risonia-theme-0.1.5.tar` & `mkdocs-risonia-theme-0.1.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-01-20 15:57:37.253249 mkdocs-risonia-theme-0.1.5/
--rw-rw-rw-   0        0        0     2361 2022-09-13 18:26:48.000000 mkdocs-risonia-theme-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      167 2022-11-20 18:59:01.000000 mkdocs-risonia-theme-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     6653 2023-01-20 15:57:37.253249 mkdocs-risonia-theme-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     4832 2023-01-19 20:02:30.000000 mkdocs-risonia-theme-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-01-20 15:57:37.053242 mkdocs-risonia-theme-0.1.5/mkdocs_risonia_theme.egg-info/
--rw-rw-rw-   0        0        0     6653 2023-01-20 15:57:36.000000 mkdocs-risonia-theme-0.1.5/mkdocs_risonia_theme.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      882 2023-01-20 15:57:36.000000 mkdocs-risonia-theme-0.1.5/mkdocs_risonia_theme.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-20 15:57:36.000000 mkdocs-risonia-theme-0.1.5/mkdocs_risonia_theme.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      212 2023-01-20 15:57:36.000000 mkdocs-risonia-theme-0.1.5/mkdocs_risonia_theme.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-11-20 18:56:22.000000 mkdocs-risonia-theme-0.1.5/mkdocs_risonia_theme.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       22 2023-01-20 15:57:36.000000 mkdocs-risonia-theme-0.1.5/mkdocs_risonia_theme.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-01-20 15:57:36.000000 mkdocs-risonia-theme-0.1.5/mkdocs_risonia_theme.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-01-20 15:57:37.096244 mkdocs-risonia-theme-0.1.5/risonia_theme/
--rw-rw-rw-   0        0        0      118 2022-10-16 15:57:02.000000 mkdocs-risonia-theme-0.1.5/risonia_theme/404.html
--rw-rw-rw-   0        0        0        0 2018-08-03 17:13:25.000000 mkdocs-risonia-theme-0.1.5/risonia_theme/__init__.py
--rw-rw-rw-   0        0        0    20599 2023-01-20 15:54:10.000000 mkdocs-risonia-theme-0.1.5/risonia_theme/base.html
-drwxrwxrwx   0        0        0        0 2023-01-20 15:57:37.173244 mkdocs-risonia-theme-0.1.5/risonia_theme/css/
--rw-rw-rw-   0        0        0      742 2022-12-21 17:43:32.000000 mkdocs-risonia-theme-0.1.5/risonia_theme/css/theme.css
--rw-rw-rw-   0        0        0     1787 2022-11-24 18:22:21.000000 mkdocs-risonia-theme-0.1.5/risonia_theme/css/w3-theme-dark.css
--rw-rw-rw-   0        0        0     1787 2022-11-24 18:22:26.000000 mkdocs-risonia-theme-0.1.5/risonia_theme/css/w3-theme-light.css
--rw-rw-rw-   0        0        0     3872 2022-11-24 18:22:09.000000 mkdocs-risonia-theme-0.1.5/risonia_theme/css/w3-theme.css
--rw-rw-rw-   0        0        0    23427 2022-05-04 16:10:46.000000 mkdocs-risonia-theme-0.1.5/risonia_theme/css/w3.css
-drwxrwxrwx   0        0        0        0 2023-01-20 15:57:37.190243 mkdocs-risonia-theme-0.1.5/risonia_theme/img/
--rw-rw-rw-   0        0        0     7406 2022-11-20 17:26:30.000000 mkdocs-risonia-theme-0.1.5/risonia_theme/img/favicon.ico
-drwxrwxrwx   0        0        0        0 2023-01-20 15:57:37.228242 mkdocs-risonia-theme-0.1.5/risonia_theme/js/
--rw-rw-rw-   0        0        0     2246 2022-11-25 18:35:17.000000 mkdocs-risonia-theme-0.1.5/risonia_theme/js/theme.js
--rw-rw-rw-   0        0        0       25 2018-08-03 17:13:25.000000 mkdocs-risonia-theme-0.1.5/risonia_theme/main.html
--rw-rw-rw-   0        0        0      113 2022-12-04 19:17:07.000000 mkdocs-risonia-theme-0.1.5/risonia_theme/mkdocs_theme.yml
-drwxrwxrwx   0        0        0        0 2023-01-20 15:57:37.229244 mkdocs-risonia-theme-0.1.5/risonia_theme/plugins/
--rw-rw-rw-   0        0        0        0 2018-08-03 17:13:25.000000 mkdocs-risonia-theme-0.1.5/risonia_theme/plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-20 15:57:37.235242 mkdocs-risonia-theme-0.1.5/risonia_theme/plugins/classes/
--rw-rw-rw-   0        0        0        0 2020-03-27 04:57:31.000000 mkdocs-risonia-theme-0.1.5/risonia_theme/plugins/classes/__init__.py
--rw-rw-rw-   0        0        0     2759 2022-12-04 19:21:29.000000 mkdocs-risonia-theme-0.1.5/risonia_theme/plugins/classes/plugin.py
-drwxrwxrwx   0        0        0        0 2023-01-20 15:57:37.252249 mkdocs-risonia-theme-0.1.5/risonia_theme/plugins/color/
--rw-rw-rw-   0        0        0        0 2020-03-27 04:57:31.000000 mkdocs-risonia-theme-0.1.5/risonia_theme/plugins/color/__init__.py
--rw-rw-rw-   0        0        0    14004 2022-12-11 12:05:50.000000 mkdocs-risonia-theme-0.1.5/risonia_theme/plugins/color/plugin.py
--rw-rw-rw-   0        0        0       42 2023-01-20 15:57:37.253249 mkdocs-risonia-theme-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1197 2023-01-19 20:02:22.000000 mkdocs-risonia-theme-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:42:33.648480 mkdocs-risonia-theme-0.1.6/
+-rw-rw-rw-   0        0        0     2361 2022-09-13 18:26:48.000000 mkdocs-risonia-theme-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0      167 2022-11-20 18:59:01.000000 mkdocs-risonia-theme-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     6653 2023-04-13 14:42:33.648480 mkdocs-risonia-theme-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4832 2023-01-21 09:48:23.000000 mkdocs-risonia-theme-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 14:42:33.634475 mkdocs-risonia-theme-0.1.6/mkdocs_risonia_theme.egg-info/
+-rw-rw-rw-   0        0        0     6653 2023-04-13 14:42:33.000000 mkdocs-risonia-theme-0.1.6/mkdocs_risonia_theme.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      882 2023-04-13 14:42:33.000000 mkdocs-risonia-theme-0.1.6/mkdocs_risonia_theme.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 14:42:33.000000 mkdocs-risonia-theme-0.1.6/mkdocs_risonia_theme.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      212 2023-04-13 14:42:33.000000 mkdocs-risonia-theme-0.1.6/mkdocs_risonia_theme.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-11-20 18:56:22.000000 mkdocs-risonia-theme-0.1.6/mkdocs_risonia_theme.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       22 2023-04-13 14:42:33.000000 mkdocs-risonia-theme-0.1.6/mkdocs_risonia_theme.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-13 14:42:33.000000 mkdocs-risonia-theme-0.1.6/mkdocs_risonia_theme.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 14:42:33.638480 mkdocs-risonia-theme-0.1.6/risonia_theme/
+-rw-rw-rw-   0        0        0      118 2022-10-16 15:57:02.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/404.html
+-rw-rw-rw-   0        0        0        0 2018-08-03 17:13:25.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/__init__.py
+-rw-rw-rw-   0        0        0    20666 2023-04-13 14:34:04.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/base.html
+drwxrwxrwx   0        0        0        0 2023-04-13 14:42:33.641481 mkdocs-risonia-theme-0.1.6/risonia_theme/css/
+-rw-rw-rw-   0        0        0     1171 2023-04-13 14:07:49.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/css/theme.css
+-rw-rw-rw-   0        0        0     1787 2022-11-24 18:22:21.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/css/w3-theme-dark.css
+-rw-rw-rw-   0        0        0     1787 2022-11-24 18:22:26.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/css/w3-theme-light.css
+-rw-rw-rw-   0        0        0     3872 2023-04-13 13:34:56.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/css/w3-theme.css
+-rw-rw-rw-   0        0        0    23427 2022-05-04 16:10:46.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/css/w3.css
+drwxrwxrwx   0        0        0        0 2023-04-13 14:42:33.642481 mkdocs-risonia-theme-0.1.6/risonia_theme/img/
+-rw-rw-rw-   0        0        0     7406 2022-11-20 17:26:30.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/img/favicon.ico
+drwxrwxrwx   0        0        0        0 2023-04-13 14:42:33.643478 mkdocs-risonia-theme-0.1.6/risonia_theme/js/
+-rw-rw-rw-   0        0        0     2246 2022-11-25 18:35:17.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/js/theme.js
+-rw-rw-rw-   0        0        0       25 2018-08-03 17:13:25.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/main.html
+-rw-rw-rw-   0        0        0      133 2023-04-13 14:33:26.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/mkdocs_theme.yml
+drwxrwxrwx   0        0        0        0 2023-04-13 14:42:33.645480 mkdocs-risonia-theme-0.1.6/risonia_theme/plugins/
+-rw-rw-rw-   0        0        0        0 2018-08-03 17:13:25.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:42:33.646480 mkdocs-risonia-theme-0.1.6/risonia_theme/plugins/classes/
+-rw-rw-rw-   0        0        0        0 2020-03-27 04:57:31.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/plugins/classes/__init__.py
+-rw-rw-rw-   0        0        0     2759 2022-12-04 19:21:29.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/plugins/classes/plugin.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:42:33.647478 mkdocs-risonia-theme-0.1.6/risonia_theme/plugins/color/
+-rw-rw-rw-   0        0        0        0 2020-03-27 04:57:31.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/plugins/color/__init__.py
+-rw-rw-rw-   0        0        0    14004 2022-12-11 12:05:50.000000 mkdocs-risonia-theme-0.1.6/risonia_theme/plugins/color/plugin.py
+-rw-rw-rw-   0        0        0       42 2023-04-13 14:42:33.649483 mkdocs-risonia-theme-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1197 2023-01-21 09:48:12.000000 mkdocs-risonia-theme-0.1.6/setup.py
```

### Comparing `mkdocs-risonia-theme-0.1.5/LICENSE` & `mkdocs-risonia-theme-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-risonia-theme-0.1.5/PKG-INFO` & `mkdocs-risonia-theme-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-risonia-theme
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple theme for MkDocs using using the w3.css framework and configurable color schemes
 Home-page: https://github.com/unverbuggt/mkdocs-risonia-theme
 Author: René Rüthlein
 License: MIT
 Description: # mkdocs-risonia-theme
         
         [![PyPI Version](https://img.shields.io/pypi/v/mkdocs-risonia-theme.svg)](https://pypi.org/project/mkdocs-risonia-theme/)
@@ -56,15 +56,15 @@
         ```
         
         Install the package from source with pip:
         
         ```bash
         cd mkdocs-risonia-theme/
         python setup.py sdist bdist_wheel
-        pip install dist/mkdocs_risonia_theme-0.1.5-py3-none-any.whl
+        pip install dist/mkdocs_risonia_theme-0.1.6-py3-none-any.whl
         ```
         
         ## Configuration
         
         Enable the theme and plugins in your `mkdocs.yml`:
         
         ```yaml
```

### Comparing `mkdocs-risonia-theme-0.1.5/README.md` & `mkdocs-risonia-theme-0.1.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 ```
 
 Install the package from source with pip:
 
 ```bash
 cd mkdocs-risonia-theme/
 python setup.py sdist bdist_wheel
-pip install dist/mkdocs_risonia_theme-0.1.5-py3-none-any.whl
+pip install dist/mkdocs_risonia_theme-0.1.6-py3-none-any.whl
 ```
 
 ## Configuration
 
 Enable the theme and plugins in your `mkdocs.yml`:
 
 ```yaml
```

### Comparing `mkdocs-risonia-theme-0.1.5/mkdocs_risonia_theme.egg-info/PKG-INFO` & `mkdocs-risonia-theme-0.1.6/mkdocs_risonia_theme.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-risonia-theme
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple theme for MkDocs using using the w3.css framework and configurable color schemes
 Home-page: https://github.com/unverbuggt/mkdocs-risonia-theme
 Author: René Rüthlein
 License: MIT
 Description: # mkdocs-risonia-theme
         
         [![PyPI Version](https://img.shields.io/pypi/v/mkdocs-risonia-theme.svg)](https://pypi.org/project/mkdocs-risonia-theme/)
@@ -56,15 +56,15 @@
         ```
         
         Install the package from source with pip:
         
         ```bash
         cd mkdocs-risonia-theme/
         python setup.py sdist bdist_wheel
-        pip install dist/mkdocs_risonia_theme-0.1.5-py3-none-any.whl
+        pip install dist/mkdocs_risonia_theme-0.1.6-py3-none-any.whl
         ```
         
         ## Configuration
         
         Enable the theme and plugins in your `mkdocs.yml`:
         
         ```yaml
```

### Comparing `mkdocs-risonia-theme-0.1.5/mkdocs_risonia_theme.egg-info/SOURCES.txt` & `mkdocs-risonia-theme-0.1.6/mkdocs_risonia_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-risonia-theme-0.1.5/risonia_theme/base.html` & `mkdocs-risonia-theme-0.1.6/risonia_theme/base.html`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,15 @@
     <button class="w3-button w3-theme-d1 w3-hover-theme w3-padding-small w3-hide-large no-print" onclick="w3_open()"><svg class="svg-2em"><use xlink:href="#open-menu" /></svg></button>
     {%- endif %}
   </div>
   <div class="w3-cell w3-cell-middle w3-padding-24" style="width:0;">
     <span style="height:2em;display:inline-block;padding:16px 0px;">&nbsp;</span>
   </div>
   <div class="w3-cell w3-cell-middle">
-    <span class="w3-left">{% if page.title %}{% if page.meta.title %}{{ page.meta.title }}{% else %}{{ page.title }}{% endif %}{% endif %}</span>
+    <span class="w3-left" id="title-top">{% if page.title %}{% if page.meta.title %}{{ page.meta.title }}{% else %}{{ page.title }}{% endif %}{% endif %}</span>
   </div>
   <div class="w3-cell w3-cell-middle" style="width:0;">
     <button class="w3-button w3-theme-d1 w3-hover-theme w3-padding-small w3-left w3-hide no-print" onclick="topFunction()" id="myToTop"><svg class="svg-1em"><use xlink:href="#to-top" /></svg></button>
   </div>
   <div class="w3-cell w3-cell-middle">
     <button class="w3-button w3-theme-d1 w3-hover-theme w3-padding-small w3-right no-print" onclick="toggleTheme(themeItem)" id="myThemeToggle"><svg class="svg-1em"><use xlink:href="#theme-toggle" /></svg></button> 
     {%- if 'search' in config.plugins %}
@@ -174,23 +174,22 @@
     <button class="w3-button w3-theme w3-hover-theme w3-padding-small" style="background-color: transparent!important;"><img src="{{ config.theme.logo | url }}" class="svg-2em"></button>
   </div>
   {%- endif %}
   <div class="w3-cell w3-cell-middle w3-padding-24" style="width:0;">
     <span style="height:2em;display:inline-block;padding:16px 0px;">&nbsp;</span>
   </div>
   <div class="w3-cell w3-cell-middle">
-    <span class="w3-left">{% if page.title %}{% if page.meta.title %}{{ page.meta.title }}{% else %}{{ page.title }}{% endif %}{% endif %}</span>
+    <span class="w3-left" id="title-head">{% if page.title %}{% if page.meta.title %}{{ page.meta.title }}{% else %}{{ page.title }}{% endif %}{% endif %}</span>
   </div>
 </header>
 
 {%- block site_nav %}
 {%- if nav|length>1 %}
-<nav class="w3-sidebar w3-bar-block w3-collapse w3-animate-left w3-theme-l4" style="z-index:3;width:300px;" id="mySidebar">
+<nav class="w3-sidebar w3-bar-block w3-collapse{% if config.theme.toc_sidebar %}-custom{% endif %} w3-animate-left w3-theme-l4" style="z-index:3;width:300px;" id="mySidebar">
   <div id="myNav" style="font-weight: bold;">
-    <a class="w3-bar-item w3-padding-16 w3-button w3-hover-theme w3-theme-l1 w3-hide-large w3-large w3-right-align" href="javascript:void(0)" onclick="w3_close()"><svg class="svg-1em"><use xlink:href="#close-menu" /></svg></a>
 {%- set accid = namespace(value=1, hidden=true, hidden2=true) %}
 {%- for nav_item in nav %}
   {%- if nav_item.children %}
     {%- set accid.hidden = true %}
     {%- set accid.hidden2 = true %}
     {%- for nav_item in nav_item.children %}
       {%- if nav_item.active %}
@@ -254,26 +253,26 @@
     </a>
   {%- endif %}
 {%- endfor %}
   </div>
   <div class="w3-container w3-large" style="height: 8em;" >&nbsp;</div>
 </nav>
 
-<div class="w3-overlay w3-hide-large w3-animate-opacity" onclick="w3_close()" style="cursor:pointer;" id="myOverlay"></div>
+<div class="w3-overlay w3-hide{% if config.theme.toc_sidebar %}-huge{% else %}-large{% endif %} w3-animate-opacity" onclick="w3_close()" style="cursor:pointer;" id="myOverlay"></div>
 {%- endif %}
 {%- endblock %}
 
 {%- set toc_check = namespace(anchors=0) %}
 {%- for toc_item in page.toc %}
   {%- set toc_check.anchors = toc_check.anchors + 1 %}
   {%- for toc_item in toc_item.children %}
     {% set toc_check.anchors = toc_check.anchors + 1 %}
   {%- endfor %}
 {%- endfor %}
-{%- if toc_check.anchors > 1 %}
+{%- if toc_check.anchors > 1 and config.theme.toc_sidebar %}
 <nav class="w3-sidebar w3-bar-block w3-collapse w3-animate-right w3-theme-l4" style="z-index:3;width:300px;right:0;" id="myTocbar">
   <div id="myToc">
   {%- for toc_item in page.toc %}
   <a href="{{ toc_item.url }}" class="w3-bar-item w3-button w3-hover-theme w3-theme-l4">{{ toc_item.title }}</a>
     {%- for toc_item in toc_item.children %}
     <a href="{{ toc_item.url }}" class="w3-bar-item w3-small w3-button w3-hover-theme w3-theme-l4">{{ toc_item.title }}</a>
       {%- for toc_item in toc_item.children %}
@@ -282,20 +281,20 @@
     {%- endfor %}
   {%- endfor %}
   </div>
   <div class="w3-container w3-large" style="height: 8em;" >&nbsp;</div>
 </nav>
 {%- endif %}
 
-<div class="w3-main" style="margin-left:300px;{% if toc_check.anchors > 1 %} margin-right:300px;{% endif %}">
+<div class="w3-main{% if config.theme.toc_sidebar %}-custom{% endif %}" style="margin-left:300px;{% if toc_check.anchors > 1 and config.theme.toc_sidebar %} margin-right:300px;{% endif %}">
 
 <div class="w3-container" style="padding: 32px;">
   <div class="w3-right w3-margin-bottom no-print">
   {%- if toc_check.anchors > 1 %}
-    <div class="w3-dropdown-hover w3-hide-large" id="myTocButton" style="z-index:1;">
+    <div class="w3-dropdown-hover{% if config.theme.toc_sidebar %} w3-hide-large{% endif %}" id="myTocButton" style="z-index:1;">
       <button class="w3-button w3-hover-theme w3-theme-l3 w3-hover-theme"><svg class="svg-1em"><use xlink:href="#toc" /></svg></button>
       <div class="w3-dropdown-content w3-bar-block" style="right:0;">
       {%- for toc_item in page.toc %}
         <a href="{{ toc_item.url }}" class="w3-bar-item w3-button w3-hover-theme w3-theme-l3">{{ toc_item.title }}</a>
         {%- for toc_item in toc_item.children %}
         <a href="{{ toc_item.url }}" class="w3-bar-item w3-small w3-button w3-hover-theme w3-theme-l3">{{ toc_item.title }}</a>
           {%- for toc_item in toc_item.children %}
```

#### html2text {}

```diff
@@ -41,15 +41,15 @@
  {%- if config.theme.logo %}
 [{{ config.theme.logo | url }}]
 {%- endif %}
  
 {% if page.title %}{% if page.meta.title %}{{ page.meta.title }}{% else %}{
 { page.title }}{% endif %}{% endif %}
  {%- block site_nav %} {%- if nav|length>1 %}
- {%- set accid = namespace(value=1, hidden=true, hidden2=true) %} {%- for
+{%- set accid = namespace(value=1, hidden=true, hidden2=true) %} {%- for
 nav_item in nav %} {%- if nav_item.children %} {%- set accid.hidden = true %}
 {%- set accid.hidden2 = true %} {%- for nav_item in nav_item.children %} {%- if
 nav_item.active %} {%- set accid.hidden = false %} {%- endif %} {%- if
 nav_item.children %} {%- for nav_item in nav_item.children %} {%- if
 nav_item.active %} {%- set accid.hidden = false %} {%- set accid.hidden2 =
 false %} {%- endif %} {%- endfor %} {%- endif %} {%- endfor %} {%- if
 nav_item.children[0].is_index %} {{_nav_item.title_}}{%_if_nav_item.children
@@ -70,15 +70,15 @@
 {%- endif %} {%- else %} {{_nav_item.title_}}{%_if_nav_item.encrypted_%}_{%
 endif_%} {%- endif %} {%- endfor %}
  
 {%- endif %} {%- endblock %} {%- set toc_check = namespace(anchors=0) %} {%-
 for toc_item in page.toc %} {%- set toc_check.anchors = toc_check.anchors + 1
 %} {%- for toc_item in toc_item.children %} {% set toc_check.anchors =
 toc_check.anchors + 1 %} {%- endfor %} {%- endfor %} {%- if toc_check.anchors >
-1 %}
+1 and config.theme.toc_sidebar %}
 {%- for toc_item in page.toc %} {{_toc_item.title_}} {%- for toc_item in
 toc_item.children %} {{_toc_item.title_}} {%- for toc_item in toc_item.children
 %} {{_toc_item.title_}} {%- endfor %} {%- endfor %} {%- endfor %}
  
  {%- endif %}
 {%- if toc_check.anchors > 1 %}
 {%- for toc_item in page.toc %} {{_toc_item.title_}} {%- for toc_item in
```

### Comparing `mkdocs-risonia-theme-0.1.5/risonia_theme/css/w3-theme-dark.css` & `mkdocs-risonia-theme-0.1.6/risonia_theme/css/w3-theme-dark.css`

 * *Files identical despite different names*

### Comparing `mkdocs-risonia-theme-0.1.5/risonia_theme/css/w3-theme-light.css` & `mkdocs-risonia-theme-0.1.6/risonia_theme/css/w3-theme-light.css`

 * *Files identical despite different names*

### Comparing `mkdocs-risonia-theme-0.1.5/risonia_theme/css/w3-theme.css` & `mkdocs-risonia-theme-0.1.6/risonia_theme/css/w3-theme.css`

 * *Files identical despite different names*

### Comparing `mkdocs-risonia-theme-0.1.5/risonia_theme/css/w3.css` & `mkdocs-risonia-theme-0.1.6/risonia_theme/css/w3.css`

 * *Files identical despite different names*

### Comparing `mkdocs-risonia-theme-0.1.5/risonia_theme/img/favicon.ico` & `mkdocs-risonia-theme-0.1.6/risonia_theme/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `mkdocs-risonia-theme-0.1.5/risonia_theme/js/theme.js` & `mkdocs-risonia-theme-0.1.6/risonia_theme/js/theme.js`

 * *Files identical despite different names*

### Comparing `mkdocs-risonia-theme-0.1.5/risonia_theme/plugins/classes/plugin.py` & `mkdocs-risonia-theme-0.1.6/risonia_theme/plugins/classes/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs-risonia-theme-0.1.5/risonia_theme/plugins/color/plugin.py` & `mkdocs-risonia-theme-0.1.6/risonia_theme/plugins/color/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs-risonia-theme-0.1.5/setup.py` & `mkdocs-risonia-theme-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup, find_packages
 
-VERSION = '0.1.5'
+VERSION = '0.1.6'
 
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     with open(file_path) as file:
         content = file.read()
     return content if content else 'no content read'
```

