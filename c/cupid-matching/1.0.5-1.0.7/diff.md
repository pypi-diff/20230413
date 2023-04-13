# Comparing `tmp/cupid_matching-1.0.5.tar.gz` & `tmp/cupid_matching-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cupid_matching-1.0.5.tar", max compression
+gzip compressed data, was "cupid_matching-1.0.7.tar", max compression
```

## Comparing `cupid_matching-1.0.5.tar` & `cupid_matching-1.0.7.tar`

### file list

```diff
@@ -1,101 +1,1722 @@
--rw-r--r--   0        0        0     2226 2023-04-12 19:22:08.495691 cupid_matching-1.0.5/README.md
--rw-r--r--   0        0        0      176 2023-04-01 13:41:41.834338 cupid_matching-1.0.5/cupid_matching/.idea/.gitignore
--rw-r--r--   0        0        0      539 2023-04-01 14:33:58.454731 cupid_matching-1.0.5/cupid_matching/.idea/cupid_matching.iml
--rw-r--r--   0        0        0     1446 2023-04-01 14:28:21.412476 cupid_matching-1.0.5/cupid_matching/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2023-04-01 14:28:21.442115 cupid_matching-1.0.5/cupid_matching/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      198 2023-04-01 14:28:21.437713 cupid_matching-1.0.5/cupid_matching/.idea/misc.xml
--rw-r--r--   0        0        0      280 2023-04-01 14:28:21.431899 cupid_matching-1.0.5/cupid_matching/.idea/modules.xml
--rw-r--r--   0        0        0      183 2023-04-01 14:28:21.446055 cupid_matching-1.0.5/cupid_matching/.idea/vcs.xml
--rw-r--r--   0        0        0      368 2023-04-01 14:33:58.460060 cupid_matching-1.0.5/cupid_matching/.idea/webResources.xml
--rw-r--r--   0        0        0        1 2023-04-02 19:21:40.197779 cupid_matching-1.0.5/cupid_matching/__init__.py
--rw-r--r--   0        0        0     9374 2023-04-12 19:23:11.716207 cupid_matching-1.0.5/cupid_matching/choo_siow.py
--rw-r--r--   0        0        0     5656 2023-04-02 13:02:37.271948 cupid_matching-1.0.5/cupid_matching/choo_siow_gender_heteroskedastic.py
--rw-r--r--   0        0        0     6283 2023-04-02 19:11:25.395323 cupid_matching-1.0.5/cupid_matching/choo_siow_heteroskedastic.py
--rw-r--r--   0        0        0    14162 2023-04-02 13:02:37.272889 cupid_matching-1.0.5/cupid_matching/cupid_streamlit.py
--rw-r--r--   0        0        0       51 2023-03-24 00:22:09.620449 cupid_matching-1.0.5/cupid_matching/docs/choo_siow.md
--rw-r--r--   0        0        0       97 2023-03-24 00:21:48.848158 cupid_matching-1.0.5/cupid_matching/docs/choo_siow_gender_heteroskedastic.md
--rw-r--r--   0        0        0       83 2023-03-24 00:22:03.727712 cupid_matching-1.0.5/cupid_matching/docs/choo_siow_heteroskedastic.md
--rw-r--r--   0        0        0      285 2023-03-24 00:22:15.196968 cupid_matching-1.0.5/cupid_matching/docs/cupid_streamlit.md
--rw-r--r--   0        0        0       46 2023-03-24 00:22:19.670499 cupid_matching-1.0.5/cupid_matching/docs/entropy.md
--rw-r--r--   0        0        0       63 2023-04-02 13:02:37.273230 cupid_matching-1.0.5/cupid_matching/docs/example_choosiow.md
--rw-r--r--   0        0        0       69 2023-04-02 13:02:37.273547 cupid_matching-1.0.5/cupid_matching/docs/example_nestedlogit.md
--rw-r--r--   0        0        0     2226 2023-04-12 19:25:51.647057 cupid_matching-1.0.5/cupid_matching/docs/index.md
--rw-r--r--   0        0        0       57 2023-03-24 00:22:52.962261 cupid_matching-1.0.5/cupid_matching/docs/ipfp_solvers.md
--rw-r--r--   0        0        0       61 2023-03-24 00:22:57.157065 cupid_matching-1.0.5/cupid_matching/docs/matching_utils.md
--rw-r--r--   0        0        0       57 2023-03-24 00:23:07.925133 cupid_matching-1.0.5/cupid_matching/docs/min_distance.md
--rw-r--r--   0        0        0       69 2023-03-24 00:23:01.182377 cupid_matching-1.0.5/cupid_matching/docs/min_distance_utils.md
--rw-r--r--   0        0        0       59 2023-03-24 00:27:46.673143 cupid_matching-1.0.5/cupid_matching/docs/model_classes.md
--rw-r--r--   0        0        0       58 2023-03-24 00:23:19.684703 cupid_matching-1.0.5/cupid_matching/docs/nested_logit.md
--rw-r--r--   0        0        0       55 2023-03-24 00:27:33.384226 cupid_matching-1.0.5/cupid_matching/docs/poisson_glm.md
--rw-r--r--   0        0        0       67 2023-03-24 00:27:42.792605 cupid_matching-1.0.5/cupid_matching/docs/poisson_glm_utils.md
--rw-r--r--   0        0        0       43 2023-03-24 00:27:23.096924 cupid_matching-1.0.5/cupid_matching/docs/utils.md
--rw-r--r--   0        0        0    11551 2023-04-02 19:15:11.050530 cupid_matching-1.0.5/cupid_matching/entropy.py
--rw-r--r--   0        0        0     3499 2023-04-02 19:12:57.727887 cupid_matching-1.0.5/cupid_matching/example_choosiow.py
--rw-r--r--   0        0        0     4133 2023-04-02 19:13:08.597638 cupid_matching-1.0.5/cupid_matching/example_nestedlogit.py
--rw-r--r--   0        0        0    26548 2023-04-02 19:13:28.516760 cupid_matching-1.0.5/cupid_matching/ipfp_solvers.py
--rw-r--r--   0        0        0     8743 2023-04-02 13:02:37.290279 cupid_matching-1.0.5/cupid_matching/matching_utils.py
--rw-r--r--   0        0        0    11551 2023-04-02 19:13:54.856938 cupid_matching-1.0.5/cupid_matching/min_distance.py
--rw-r--r--   0        0        0     5260 2023-04-02 19:13:40.696373 cupid_matching-1.0.5/cupid_matching/min_distance_utils.py
--rw-r--r--   0        0        0     1873 2023-04-02 13:02:37.291292 cupid_matching-1.0.5/cupid_matching/mkdocs.yml
--rw-r--r--   0        0        0    16277 2023-04-02 19:15:11.063645 cupid_matching-1.0.5/cupid_matching/model_classes.py
--rw-r--r--   0        0        0      369 2023-04-02 19:14:11.059995 cupid_matching-1.0.5/cupid_matching/mypy.ini
--rw-r--r--   0        0        0     9515 2023-04-02 19:15:11.064847 cupid_matching-1.0.5/cupid_matching/nested_logit.py
--rw-r--r--   0        0        0     7401 2023-04-02 19:15:11.067470 cupid_matching-1.0.5/cupid_matching/poisson_glm.py
--rw-r--r--   0        0        0     6544 2023-04-02 19:14:50.571051 cupid_matching-1.0.5/cupid_matching/poisson_glm_utils.py
--rw-r--r--   0        0        0    17888 2023-04-12 19:26:29.373052 cupid_matching-1.0.5/cupid_matching/site/404.html
--rw-r--r--   0        0        0      704 2023-04-12 19:26:29.309599 cupid_matching-1.0.5/cupid_matching/site/assets/_mkdocstrings.css
--rw-r--r--   0        0        0     1870 2023-04-12 19:26:29.310373 cupid_matching-1.0.5/cupid_matching/site/assets/images/favicon.png
--rw-r--r--   0        0        0    17074 2023-04-12 19:26:29.311600 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.ar.min.js
--rw-r--r--   0        0        0     4654 2023-04-12 19:26:29.312037 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.da.min.js
--rw-r--r--   0        0        0     6119 2023-04-12 19:26:29.312251 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.de.min.js
--rw-r--r--   0        0        0     6208 2023-04-12 19:26:29.312426 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.du.min.js
--rw-r--r--   0        0        0    11499 2023-04-12 19:26:29.312902 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.es.min.js
--rw-r--r--   0        0        0     9342 2023-04-12 19:26:29.313341 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.fi.min.js
--rw-r--r--   0        0        0    10669 2023-04-12 19:26:29.313561 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.fr.min.js
--rw-r--r--   0        0        0     3383 2023-04-12 19:26:29.314020 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.hi.min.js
--rw-r--r--   0        0        0     9437 2023-04-12 19:26:29.314355 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.hu.min.js
--rw-r--r--   0        0        0    11232 2023-04-12 19:26:29.314561 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.it.min.js
--rw-r--r--   0        0        0     2313 2023-04-12 19:26:29.314763 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.ja.min.js
--rw-r--r--   0        0        0       36 2023-04-12 19:26:29.315037 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.jp.min.js
--rw-r--r--   0        0        0     7973 2023-04-12 19:26:29.315327 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.ko.min.js
--rw-r--r--   0        0        0      817 2023-04-12 19:26:29.315576 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.multi.min.js
--rw-r--r--   0        0        0     6026 2023-04-12 19:26:29.315839 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.nl.min.js
--rw-r--r--   0        0        0     4754 2023-04-12 19:26:29.316052 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.no.min.js
--rw-r--r--   0        0        0    10171 2023-04-12 19:26:29.316272 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.pt.min.js
--rw-r--r--   0        0        0    10958 2023-04-12 19:26:29.316522 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.ro.min.js
--rw-r--r--   0        0        0    10331 2023-04-12 19:26:29.316751 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.ru.min.js
--rw-r--r--   0        0        0     3647 2023-04-12 19:26:29.317000 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
--rw-r--r--   0        0        0     4523 2023-04-12 19:26:29.317173 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.sv.min.js
--rw-r--r--   0        0        0     2406 2023-04-12 19:26:29.317357 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.ta.min.js
--rw-r--r--   0        0        0     1031 2023-04-12 19:26:29.317572 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.th.min.js
--rw-r--r--   0        0        0    15009 2023-04-12 19:26:29.318097 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.tr.min.js
--rw-r--r--   0        0        0      784 2023-04-12 19:26:29.318370 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.vi.min.js
--rw-r--r--   0        0        0     2062 2023-04-12 19:26:29.318588 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.zh.min.js
--rw-r--r--   0        0        0    22878 2023-04-12 19:26:29.318822 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/tinyseg.js
--rw-r--r--   0        0        0   677455 2023-04-12 19:26:29.319181 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/wordcut.js
--rw-r--r--   0        0        0    38916 2023-04-12 19:26:29.319522 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/workers/search.208ed371.min.js
--rw-r--r--   0        0        0   209901 2023-04-12 19:26:29.319816 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/workers/search.208ed371.min.js.map
--rw-r--r--   0        0        0    12355 2023-04-12 19:26:29.320580 cupid_matching-1.0.5/cupid_matching/site/assets/stylesheets/palette.a0c5b2b5.min.css
--rw-r--r--   0        0        0     3646 2023-04-12 19:26:29.320794 cupid_matching-1.0.5/cupid_matching/site/assets/stylesheets/palette.a0c5b2b5.min.css.map
--rw-r--r--   0        0        0    56388 2023-04-12 19:26:29.397202 cupid_matching-1.0.5/cupid_matching/site/choo_siow/index.html
--rw-r--r--   0        0        0    61309 2023-04-12 19:26:29.411120 cupid_matching-1.0.5/cupid_matching/site/choo_siow_gender_heteroskedastic/index.html
--rw-r--r--   0        0        0    67113 2023-04-12 19:26:29.427864 cupid_matching-1.0.5/cupid_matching/site/choo_siow_heteroskedastic/index.html
--rw-r--r--   0        0        0    19453 2023-04-12 19:26:29.428738 cupid_matching-1.0.5/cupid_matching/site/cupid_streamlit/index.html
--rw-r--r--   0        0        0    52734 2023-04-12 19:26:29.439005 cupid_matching-1.0.5/cupid_matching/site/entropy/index.html
--rw-r--r--   0        0        0    24288 2023-04-12 19:26:29.383321 cupid_matching-1.0.5/cupid_matching/site/index.html
--rw-r--r--   0        0        0   171028 2023-04-12 19:26:29.510337 cupid_matching-1.0.5/cupid_matching/site/ipfp_solvers/index.html
--rw-r--r--   0        0        0    33535 2023-04-12 19:26:29.516154 cupid_matching-1.0.5/cupid_matching/site/matching_utils/index.html
--rw-r--r--   0        0        0    73534 2023-04-12 19:26:29.536810 cupid_matching-1.0.5/cupid_matching/site/min_distance/index.html
--rw-r--r--   0        0        0    48540 2023-04-12 19:26:29.548044 cupid_matching-1.0.5/cupid_matching/site/min_distance_utils/index.html
--rw-r--r--   0        0        0   158026 2023-04-12 19:26:29.603190 cupid_matching-1.0.5/cupid_matching/site/model_classes/index.html
--rw-r--r--   0        0        0    80301 2023-04-12 19:26:29.625018 cupid_matching-1.0.5/cupid_matching/site/nested_logit/index.html
--rw-r--r--   0        0        0      864 2023-04-12 19:26:29.310029 cupid_matching-1.0.5/cupid_matching/site/objects.inv
--rw-r--r--   0        0        0    70696 2023-04-12 19:26:29.645184 cupid_matching-1.0.5/cupid_matching/site/poisson_glm/index.html
--rw-r--r--   0        0        0    52629 2023-04-12 19:26:29.657841 cupid_matching-1.0.5/cupid_matching/site/poisson_glm_utils/index.html
--rw-r--r--   0        0        0   179908 2023-04-12 19:26:29.695697 cupid_matching-1.0.5/cupid_matching/site/search/search_index.json
--rw-r--r--   0        0        0     3235 2023-04-12 19:26:29.374434 cupid_matching-1.0.5/cupid_matching/site/sitemap.xml
--rw-r--r--   0        0        0      354 2023-04-12 19:26:29.374610 cupid_matching-1.0.5/cupid_matching/site/sitemap.xml.gz
--rw-r--r--   0        0        0   120234 2023-04-12 19:26:29.694954 cupid_matching-1.0.5/cupid_matching/site/utils/index.html
--rw-r--r--   0        0        0    12373 2023-04-02 19:15:05.244218 cupid_matching-1.0.5/cupid_matching/utils.py
--rw-r--r--   0        0        0      969 2023-04-12 19:22:27.062349 cupid_matching-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     2969 1970-01-01 00:00:00.000000 cupid_matching-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     2321 2023-04-13 19:10:22.350881 cupid_matching-1.0.7/README.md
+-rw-r--r--   0        0        0     6148 2023-04-03 19:49:27.937336 cupid_matching-1.0.7/cupid_matching/.DS_Store
+-rw-r--r--   0        0        0      176 2023-04-01 13:41:41.834338 cupid_matching-1.0.7/cupid_matching/.idea/.gitignore
+-rw-r--r--   0        0        0      539 2023-04-01 14:33:58.454731 cupid_matching-1.0.7/cupid_matching/.idea/cupid_matching.iml
+-rw-r--r--   0        0        0     1446 2023-04-01 14:28:21.412476 cupid_matching-1.0.7/cupid_matching/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2023-04-01 14:28:21.442115 cupid_matching-1.0.7/cupid_matching/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      198 2023-04-01 14:28:21.437713 cupid_matching-1.0.7/cupid_matching/.idea/misc.xml
+-rw-r--r--   0        0        0      280 2023-04-01 14:28:21.431899 cupid_matching-1.0.7/cupid_matching/.idea/modules.xml
+-rw-r--r--   0        0        0      183 2023-04-01 14:28:21.446055 cupid_matching-1.0.7/cupid_matching/.idea/vcs.xml
+-rw-r--r--   0        0        0      368 2023-04-01 14:33:58.460060 cupid_matching-1.0.7/cupid_matching/.idea/webResources.xml
+-rw-r--r--   0        0        0     7536 2023-04-01 22:41:08.541782 cupid_matching-1.0.7/cupid_matching/.idea/workspace.xml
+-rw-r--r--   0        0        0       34 2023-03-24 00:10:22.896173 cupid_matching-1.0.7/cupid_matching/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0        2 2023-03-31 20:06:15.815653 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/@plugins_snapshot.json
+-rw-r--r--   0        0        0     8533 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/__future__.data.json
+-rw-r--r--   0        0        0     1723 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/__future__.meta.json
+-rw-r--r--   0        0        0     2266 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/__main__.data.json
+-rw-r--r--   0        0        0     1690 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/__main__.meta.json
+-rw-r--r--   0        0        0   193710 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_ast.data.json
+-rw-r--r--   0        0        0     1811 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_ast.meta.json
+-rw-r--r--   0        0        0    57330 2023-03-26 00:13:29.546583 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_codecs.data.json
+-rw-r--r--   0        0        0     1857 2023-03-26 00:13:29.546903 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_codecs.meta.json
+-rw-r--r--   0        0        0    19803 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_collections_abc.data.json
+-rw-r--r--   0        0        0     1765 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_collections_abc.meta.json
+-rw-r--r--   0        0        0    11687 2023-03-24 00:33:08.242231 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_compression.data.json
+-rw-r--r--   0        0        0     1537 2023-03-24 00:33:08.242423 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_compression.meta.json
+-rw-r--r--   0        0        0    21518 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_csv.data.json
+-rw-r--r--   0        0        0     1820 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_csv.meta.json
+-rw-r--r--   0        0        0     3216 2023-03-26 00:13:29.544331 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_ctypes.data.json
+-rw-r--r--   0        0        0     1767 2023-03-26 00:13:29.544643 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_ctypes.meta.json
+-rw-r--r--   0        0        0   209809 2023-03-24 00:33:08.226273 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_curses.data.json
+-rw-r--r--   0        0        0     1545 2023-03-24 00:33:08.226582 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_curses.meta.json
+-rw-r--r--   0        0        0   186643 2023-03-26 00:13:34.785852 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_decimal.data.json
+-rw-r--r--   0        0        0     1812 2023-03-26 00:13:34.786283 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_decimal.meta.json
+-rw-r--r--   0        0        0   122130 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_operator.data.json
+-rw-r--r--   0        0        0     1779 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_operator.meta.json
+-rw-r--r--   0        0        0     6702 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_random.data.json
+-rw-r--r--   0        0        0     1717 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_random.meta.json
+-rw-r--r--   0        0        0    99552 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_socket.data.json
+-rw-r--r--   0        0        0     1841 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_socket.meta.json
+-rw-r--r--   0        0        0    21636 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_stat.data.json
+-rw-r--r--   0        0        0     1728 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_stat.meta.json
+-rw-r--r--   0        0        0    26000 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_thread.data.json
+-rw-r--r--   0        0        0     1809 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_thread.meta.json
+-rw-r--r--   0        0        0    97013 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1889 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0    14346 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_warnings.data.json
+-rw-r--r--   0        0        0     1694 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_warnings.meta.json
+-rw-r--r--   0        0        0    30012 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_weakref.data.json
+-rw-r--r--   0        0        0     1793 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_weakref.meta.json
+-rw-r--r--   0        0        0    55252 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_weakrefset.data.json
+-rw-r--r--   0        0        0     1799 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/_weakrefset.meta.json
+-rw-r--r--   0        0        0    22398 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/abc.data.json
+-rw-r--r--   0        0        0     1753 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/abc.meta.json
+-rw-r--r--   0        0        0   165859 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/argparse.data.json
+-rw-r--r--   0        0        0     1856 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/argparse.meta.json
+-rw-r--r--   0        0        0    66415 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/array.data.json
+-rw-r--r--   0        0        0     1820 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/array.meta.json
+-rw-r--r--   0        0        0   149483 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/ast.data.json
+-rw-r--r--   0        0        0     1860 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/ast.meta.json
+-rw-r--r--   0        0        0    11609 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/__init__.data.json
+-rw-r--r--   0        0        0     2133 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/__init__.meta.json
+-rw-r--r--   0        0        0   108563 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/base_events.data.json
+-rw-r--r--   0        0        0     2080 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/base_events.meta.json
+-rw-r--r--   0        0        0    27666 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/coroutines.data.json
+-rw-r--r--   0        0        0     1798 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/coroutines.meta.json
+-rw-r--r--   0        0        0   210031 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/events.data.json
+-rw-r--r--   0        0        0     2118 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/events.meta.json
+-rw-r--r--   0        0        0     9803 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/exceptions.data.json
+-rw-r--r--   0        0        0     1747 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/exceptions.meta.json
+-rw-r--r--   0        0        0    40152 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/futures.data.json
+-rw-r--r--   0        0        0     1938 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/futures.meta.json
+-rw-r--r--   0        0        0    29212 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/locks.data.json
+-rw-r--r--   0        0        0     1889 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/locks.meta.json
+-rw-r--r--   0        0        0    18739 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/protocols.data.json
+-rw-r--r--   0        0        0     1841 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/protocols.meta.json
+-rw-r--r--   0        0        0    25226 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/queues.data.json
+-rw-r--r--   0        0        0     1777 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/queues.meta.json
+-rw-r--r--   0        0        0     5100 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/runners.data.json
+-rw-r--r--   0        0        0     1836 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/runners.meta.json
+-rw-r--r--   0        0        0     4172 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/selector_events.data.json
+-rw-r--r--   0        0        0     1815 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/selector_events.meta.json
+-rw-r--r--   0        0        0    37972 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/streams.data.json
+-rw-r--r--   0        0        0     1947 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/streams.meta.json
+-rw-r--r--   0        0        0    26110 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/subprocess.data.json
+-rw-r--r--   0        0        0     1957 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/subprocess.meta.json
+-rw-r--r--   0        0        0   109221 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/tasks.data.json
+-rw-r--r--   0        0        0     1938 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/tasks.meta.json
+-rw-r--r--   0        0        0     6124 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/threads.data.json
+-rw-r--r--   0        0        0     1757 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/threads.meta.json
+-rw-r--r--   0        0        0    29800 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/transports.data.json
+-rw-r--r--   0        0        0     1804 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/transports.meta.json
+-rw-r--r--   0        0        0    63976 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/unix_events.data.json
+-rw-r--r--   0        0        0     1922 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/asyncio/unix_events.meta.json
+-rw-r--r--   0        0        0     6876 2023-03-24 00:33:08.293024 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/atexit.data.json
+-rw-r--r--   0        0        0     1521 2023-03-24 00:33:08.293214 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/atexit.meta.json
+-rw-r--r--   0        0        0   223621 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/attr/__init__.data.json
+-rw-r--r--   0        0        0     1930 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/attr/__init__.meta.json
+-rw-r--r--   0        0        0     4320 2023-03-26 00:13:34.354724 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/attr/_cmp.data.json
+-rw-r--r--   0        0        0     1672 2023-03-26 00:13:34.355096 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/attr/_cmp.meta.json
+-rw-r--r--   0        0        0     3311 2023-03-26 00:13:34.354000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/attr/_typing_compat.data.json
+-rw-r--r--   0        0        0     1692 2023-03-26 00:13:34.354215 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/attr/_typing_compat.meta.json
+-rw-r--r--   0        0        0     7637 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/attr/_version_info.data.json
+-rw-r--r--   0        0        0     1691 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/attr/_version_info.meta.json
+-rw-r--r--   0        0        0     9098 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/attr/converters.data.json
+-rw-r--r--   0        0        0     1698 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/attr/converters.meta.json
+-rw-r--r--   0        0        0    11099 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/attr/exceptions.data.json
+-rw-r--r--   0        0        0     1684 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/attr/exceptions.meta.json
+-rw-r--r--   0        0        0     3904 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/attr/filters.data.json
+-rw-r--r--   0        0        0     1692 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/attr/filters.meta.json
+-rw-r--r--   0        0        0     8436 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/attr/setters.data.json
+-rw-r--r--   0        0        0     1692 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/attr/setters.meta.json
+-rw-r--r--   0        0        0    45671 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/attr/validators.data.json
+-rw-r--r--   0        0        0     1734 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/attr/validators.meta.json
+-rw-r--r--   0        0        0    13545 2023-03-24 00:33:08.329875 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/base64.data.json
+-rw-r--r--   0        0        0     1543 2023-03-24 00:33:08.330150 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/base64.meta.json
+-rw-r--r--   0        0        0    15400 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/binascii.data.json
+-rw-r--r--   0        0        0     1818 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/binascii.meta.json
+-rw-r--r--   0        0        0  1141247 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/builtins.data.json
+-rw-r--r--   0        0        0     1917 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/builtins.meta.json
+-rw-r--r--   0        0        0    62654 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/calendar.data.json
+-rw-r--r--   0        0        0     1810 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/calendar.meta.json
+-rw-r--r--   0        0        0     8399 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/click/__init__.data.json
+-rw-r--r--   0        0        0     1889 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/click/__init__.meta.json
+-rw-r--r--   0        0        0    51443 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/click/_compat.data.json
+-rw-r--r--   0        0        0     1950 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/click/_compat.meta.json
+-rw-r--r--   0        0        0    48731 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/click/_termui_impl.data.json
+-rw-r--r--   0        0        0     2228 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/click/_termui_impl.meta.json
+-rw-r--r--   0        0        0     5845 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/click/_textwrap.data.json
+-rw-r--r--   0        0        0     1772 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/click/_textwrap.meta.json
+-rw-r--r--   0        0        0   197021 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/click/core.data.json
+-rw-r--r--   0        0        0     2286 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/click/core.meta.json
+-rw-r--r--   0        0        0    61474 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/click/decorators.data.json
+-rw-r--r--   0        0        0     1978 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/click/decorators.meta.json
+-rw-r--r--   0        0        0    30027 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/click/exceptions.data.json
+-rw-r--r--   0        0        0     1906 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/click/exceptions.meta.json
+-rw-r--r--   0        0        0    19110 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/click/formatting.data.json
+-rw-r--r--   0        0        0     1922 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/click/formatting.meta.json
+-rw-r--r--   0        0        0     7702 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/click/globals.data.json
+-rw-r--r--   0        0        0     1749 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/click/globals.meta.json
+-rw-r--r--   0        0        0    31268 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/click/parser.data.json
+-rw-r--r--   0        0        0     1938 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/click/parser.meta.json
+-rw-r--r--   0        0        0    36601 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/click/shell_completion.data.json
+-rw-r--r--   0        0        0     1997 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/click/shell_completion.meta.json
+-rw-r--r--   0        0        0    25539 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/click/termui.data.json
+-rw-r--r--   0        0        0     2113 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/click/termui.meta.json
+-rw-r--r--   0        0        0    88334 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/click/types.data.json
+-rw-r--r--   0        0        0     2135 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/click/types.meta.json
+-rw-r--r--   0        0        0    34946 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/click/utils.data.json
+-rw-r--r--   0        0        0     2014 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/click/utils.meta.json
+-rw-r--r--   0        0        0   134251 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/codecs.data.json
+-rw-r--r--   0        0        0     1871 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/codecs.meta.json
+-rw-r--r--   0        0        0   446304 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/collections/__init__.data.json
+-rw-r--r--   0        0        0     1900 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/collections/__init__.meta.json
+-rw-r--r--   0        0        0     4078 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/collections/abc.data.json
+-rw-r--r--   0        0        0     1731 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/collections/abc.meta.json
+-rw-r--r--   0        0        0     8295 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/colorsys.data.json
+-rw-r--r--   0        0        0     1692 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/colorsys.meta.json
+-rw-r--r--   0        0        0     1701 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/concurrent/__init__.data.json
+-rw-r--r--   0        0        0     1703 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/concurrent/__init__.meta.json
+-rw-r--r--   0        0        0     4942 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/concurrent/futures/__init__.data.json
+-rw-r--r--   0        0        0     1862 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/concurrent/futures/__init__.meta.json
+-rw-r--r--   0        0        0    65940 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/concurrent/futures/_base.data.json
+-rw-r--r--   0        0        0     1861 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/concurrent/futures/_base.meta.json
+-rw-r--r--   0        0        0    65236 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/concurrent/futures/process.data.json
+-rw-r--r--   0        0        0     2105 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/concurrent/futures/process.meta.json
+-rw-r--r--   0        0        0    23845 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/concurrent/futures/thread.data.json
+-rw-r--r--   0        0        0     1906 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/concurrent/futures/thread.meta.json
+-rw-r--r--   0        0        0   135261 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/configparser.data.json
+-rw-r--r--   0        0        0     1811 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/configparser.meta.json
+-rw-r--r--   0        0        0   113709 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/contextlib.data.json
+-rw-r--r--   0        0        0     1795 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/contextlib.meta.json
+-rw-r--r--   0        0        0    41358 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/contextvars.data.json
+-rw-r--r--   0        0        0     1799 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/contextvars.meta.json
+-rw-r--r--   0        0        0     5981 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/copy.data.json
+-rw-r--r--   0        0        0     1683 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/copy.meta.json
+-rw-r--r--   0        0        0    13018 2023-03-26 00:13:34.335416 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/copyreg.data.json
+-rw-r--r--   0        0        0     1761 2023-03-26 00:13:34.335692 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/copyreg.meta.json
+-rw-r--r--   0        0        0    32485 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/csv.data.json
+-rw-r--r--   0        0        0     1786 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/csv.meta.json
+-rw-r--r--   0        0        0   140977 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1863 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0    59518 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/ctypes/wintypes.data.json
+-rw-r--r--   0        0        0     1751 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/ctypes/wintypes.meta.json
+-rw-r--r--   0        0        0     1886 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/cupid_matching/__init__.data.json
+-rw-r--r--   0        0        0     1627 2023-03-26 00:20:01.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/cupid_matching/__init__.meta.json
+-rw-r--r--   0        0        0    19942 2023-03-31 00:13:20.670231 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/cupid_matching/choo_siow.data.json
+-rw-r--r--   0        0        0     1973 2023-03-31 00:13:35.679368 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/cupid_matching/choo_siow.meta.json
+-rw-r--r--   0        0        0    11868 2023-03-26 00:15:21.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/cupid_matching/choo_siow_gender_heteroskedastic.data.json
+-rw-r--r--   0        0        0     1960 2023-03-26 00:15:21.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/cupid_matching/choo_siow_gender_heteroskedastic.meta.json
+-rw-r--r--   0        0        0    11469 2023-03-26 00:15:38.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/cupid_matching/choo_siow_heteroskedastic.data.json
+-rw-r--r--   0        0        0     1987 2023-03-26 00:15:38.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/cupid_matching/choo_siow_heteroskedastic.meta.json
+-rw-r--r--   0        0        0    26170 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/cupid_matching/entropy.data.json
+-rw-r--r--   0        0        0     1950 2023-03-26 00:15:04.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/cupid_matching/entropy.meta.json
+-rw-r--r--   0        0        0    14219 2023-03-31 00:09:30.605965 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/cupid_matching/example_choosiow.data.json
+-rw-r--r--   0        0        0     2268 2023-03-31 20:06:15.715703 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/cupid_matching/example_choosiow.meta.json
+-rw-r--r--   0        0        0    41751 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/cupid_matching/ipfp_solvers.data.json
+-rw-r--r--   0        0        0     2171 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/cupid_matching/ipfp_solvers.meta.json
+-rw-r--r--   0        0        0    23713 2023-03-31 00:08:02.284018 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/cupid_matching/matching_utils.data.json
+-rw-r--r--   0        0        0     2060 2023-03-31 00:08:38.022513 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/cupid_matching/matching_utils.meta.json
+-rw-r--r--   0        0        0     6582 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/cupid_matching/min_distance.data.json
+-rw-r--r--   0        0        0     2090 2023-03-31 00:01:19.623758 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/cupid_matching/min_distance.meta.json
+-rw-r--r--   0        0        0    18530 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/cupid_matching/min_distance_utils.data.json
+-rw-r--r--   0        0        0     1761 2023-03-31 00:04:47.598975 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/cupid_matching/min_distance_utils.meta.json
+-rw-r--r--   0        0        0    30249 2023-03-26 00:19:58.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/cupid_matching/model_classes.data.json
+-rw-r--r--   0        0        0     2073 2023-03-30 20:37:53.188328 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/cupid_matching/model_classes.meta.json
+-rw-r--r--   0        0        0    14091 2023-03-30 19:44:48.506574 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/cupid_matching/nested_logit.data.json
+-rw-r--r--   0        0        0     1976 2023-03-30 20:20:57.768148 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/cupid_matching/nested_logit.meta.json
+-rw-r--r--   0        0        0     4723 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/cupid_matching/poisson_glm.data.json
+-rw-r--r--   0        0        0     2083 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/cupid_matching/poisson_glm.meta.json
+-rw-r--r--   0        0        0    26002 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/cupid_matching/poisson_glm_utils.data.json
+-rw-r--r--   0        0        0     1979 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/cupid_matching/poisson_glm_utils.meta.json
+-rw-r--r--   0        0        0    52498 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/cupid_matching/utils.data.json
+-rw-r--r--   0        0        0     2031 2023-03-30 21:15:39.004804 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/cupid_matching/utils.meta.json
+-rw-r--r--   0        0        0    36090 2023-03-24 00:33:08.700532 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/curses/__init__.data.json
+-rw-r--r--   0        0        0     1548 2023-03-24 00:33:08.700758 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/curses/__init__.meta.json
+-rw-r--r--   0        0        0    63289 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/dataclasses.data.json
+-rw-r--r--   0        0        0     1813 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/dataclasses.meta.json
+-rw-r--r--   0        0        0   154595 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/datetime.data.json
+-rw-r--r--   0        0        0     1767 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/datetime.meta.json
+-rw-r--r--   0        0        0     5337 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/decimal.data.json
+-rw-r--r--   0        0        0     1708 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/decimal.meta.json
+-rw-r--r--   0        0        0    63796 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/difflib.data.json
+-rw-r--r--   0        0        0     1764 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/difflib.meta.json
+-rw-r--r--   0        0        0    44121 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/dis.data.json
+-rw-r--r--   0        0        0     1800 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/dis.meta.json
+-rw-r--r--   0        0        0     1693 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/distutils/__init__.data.json
+-rw-r--r--   0        0        0     1701 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/distutils/__init__.meta.json
+-rw-r--r--   0        0        0     3146 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/distutils/spawn.data.json
+-rw-r--r--   0        0        0     1706 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/distutils/spawn.meta.json
+-rw-r--r--   0        0        0    73586 2023-03-24 00:33:09.975572 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/doctest.data.json
+-rw-r--r--   0        0        0     1546 2023-03-24 00:33:09.975824 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/doctest.meta.json
+-rw-r--r--   0        0        0     8164 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/email/__init__.data.json
+-rw-r--r--   0        0        0     1792 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/email/__init__.meta.json
+-rw-r--r--   0        0        0    13316 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/email/charset.data.json
+-rw-r--r--   0        0        0     1728 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/email/charset.meta.json
+-rw-r--r--   0        0        0     7938 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1763 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    27029 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/email/errors.data.json
+-rw-r--r--   0        0        0     1735 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/email/errors.meta.json
+-rw-r--r--   0        0        0    10030 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/email/header.data.json
+-rw-r--r--   0        0        0     1748 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/email/header.meta.json
+-rw-r--r--   0        0        0    86532 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/email/message.data.json
+-rw-r--r--   0        0        0     1866 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/email/message.meta.json
+-rw-r--r--   0        0        0    33615 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/email/policy.data.json
+-rw-r--r--   0        0        0     1821 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/email/policy.meta.json
+-rw-r--r--   0        0        0    21539 2023-03-24 00:33:08.825139 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/email/utils.data.json
+-rw-r--r--   0        0        0     1595 2023-03-24 00:33:08.825355 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/email/utils.meta.json
+-rw-r--r--   0        0        0    66878 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/enum.data.json
+-rw-r--r--   0        0        0     1785 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/enum.meta.json
+-rw-r--r--   0        0        0    21276 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/errno.data.json
+-rw-r--r--   0        0        0     1746 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/errno.meta.json
+-rw-r--r--   0        0        0     6702 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/fnmatch.data.json
+-rw-r--r--   0        0        0     1714 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/fnmatch.meta.json
+-rw-r--r--   0        0        0    95820 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/fractions.data.json
+-rw-r--r--   0        0        0     1833 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/fractions.meta.json
+-rw-r--r--   0        0        0   139322 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/functools.data.json
+-rw-r--r--   0        0        0     1794 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/functools.meta.json
+-rw-r--r--   0        0        0    17518 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/gc.data.json
+-rw-r--r--   0        0        0     1766 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/gc.meta.json
+-rw-r--r--   0        0        0    24438 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/genericpath.data.json
+-rw-r--r--   0        0        0     1782 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/genericpath.meta.json
+-rw-r--r--   0        0        0     4118 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/getpass.data.json
+-rw-r--r--   0        0        0     1689 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/getpass.meta.json
+-rw-r--r--   0        0        0    58377 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/gettext.data.json
+-rw-r--r--   0        0        0     1801 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/gettext.meta.json
+-rw-r--r--   0        0        0    11610 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/__init__.data.json
+-rw-r--r--   0        0        0     2229 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/__init__.meta.json
+-rw-r--r--   0        0        0    94624 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/cmd.data.json
+-rw-r--r--   0        0        0     2161 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/cmd.meta.json
+-rw-r--r--   0        0        0    16991 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/compat.data.json
+-rw-r--r--   0        0        0     1860 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/compat.meta.json
+-rw-r--r--   0        0        0    70918 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/config.data.json
+-rw-r--r--   0        0        0     2222 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/config.meta.json
+-rw-r--r--   0        0        0     8500 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/db.data.json
+-rw-r--r--   0        0        0     1809 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/db.meta.json
+-rw-r--r--   0        0        0    44019 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/diff.data.json
+-rw-r--r--   0        0        0     2230 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/diff.meta.json
+-rw-r--r--   0        0        0    26547 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/exc.data.json
+-rw-r--r--   0        0        0     1932 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/exc.meta.json
+-rw-r--r--   0        0        0     2289 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/index/__init__.data.json
+-rw-r--r--   0        0        0     1727 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/index/__init__.meta.json
+-rw-r--r--   0        0        0    68238 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/index/base.data.json
+-rw-r--r--   0        0        0     2696 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/index/base.meta.json
+-rw-r--r--   0        0        0    19414 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/index/fun.data.json
+-rw-r--r--   0        0        0     2286 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/index/fun.meta.json
+-rw-r--r--   0        0        0    54611 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/index/typ.data.json
+-rw-r--r--   0        0        0     2038 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/index/typ.meta.json
+-rw-r--r--   0        0        0    14692 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/index/util.data.json
+-rw-r--r--   0        0        0     2051 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/index/util.meta.json
+-rw-r--r--   0        0        0     3806 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/objects/__init__.data.json
+-rw-r--r--   0        0        0     2108 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/objects/__init__.meta.json
+-rw-r--r--   0        0        0    29422 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/objects/base.data.json
+-rw-r--r--   0        0        0     2277 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/objects/base.meta.json
+-rw-r--r--   0        0        0     6454 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/objects/blob.data.json
+-rw-r--r--   0        0        0     1851 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/objects/blob.meta.json
+-rw-r--r--   0        0        0    42768 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/objects/commit.data.json
+-rw-r--r--   0        0        0     2418 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/objects/commit.meta.json
+-rw-r--r--   0        0        0    13624 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/objects/fun.data.json
+-rw-r--r--   0        0        0     1896 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/objects/fun.meta.json
+-rw-r--r--   0        0        0     1768 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/objects/submodule/__init__.data.json
+-rw-r--r--   0        0        0     1704 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/objects/submodule/__init__.meta.json
+-rw-r--r--   0        0        0    68535 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/objects/submodule/base.data.json
+-rw-r--r--   0        0        0     2644 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/objects/submodule/base.meta.json
+-rw-r--r--   0        0        0    13516 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/objects/submodule/root.data.json
+-rw-r--r--   0        0        0     2410 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/objects/submodule/root.meta.json
+-rw-r--r--   0        0        0    12286 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/objects/submodule/util.data.json
+-rw-r--r--   0        0        0     2362 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/objects/submodule/util.meta.json
+-rw-r--r--   0        0        0     9168 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/objects/tag.data.json
+-rw-r--r--   0        0        0     2013 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/objects/tag.meta.json
+-rw-r--r--   0        0        0    39730 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/objects/tree.data.json
+-rw-r--r--   0        0        0     2231 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/objects/tree.meta.json
+-rw-r--r--   0        0        0    95020 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/objects/util.data.json
+-rw-r--r--   0        0        0     2344 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/objects/util.meta.json
+-rw-r--r--   0        0        0     2571 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/refs/__init__.data.json
+-rw-r--r--   0        0        0     1826 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/refs/__init__.meta.json
+-rw-r--r--   0        0        0    18553 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/refs/head.data.json
+-rw-r--r--   0        0        0     2206 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/refs/head.meta.json
+-rw-r--r--   0        0        0    42003 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/refs/log.data.json
+-rw-r--r--   0        0        0     2160 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/refs/log.meta.json
+-rw-r--r--   0        0        0    18680 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/refs/reference.data.json
+-rw-r--r--   0        0        0     2157 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/refs/reference.meta.json
+-rw-r--r--   0        0        0    10734 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/refs/remote.data.json
+-rw-r--r--   0        0        0     1979 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/refs/remote.meta.json
+-rw-r--r--   0        0        0    62889 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/refs/symbolic.data.json
+-rw-r--r--   0        0        0     2392 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/refs/symbolic.meta.json
+-rw-r--r--   0        0        0    13602 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/refs/tag.data.json
+-rw-r--r--   0        0        0     2072 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/refs/tag.meta.json
+-rw-r--r--   0        0        0    88392 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/remote.data.json
+-rw-r--r--   0        0        0     2552 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/remote.meta.json
+-rw-r--r--   0        0        0     1754 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/repo/__init__.data.json
+-rw-r--r--   0        0        0     1701 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/repo/__init__.meta.json
+-rw-r--r--   0        0        0   113367 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/repo/base.data.json
+-rw-r--r--   0        0        0     2753 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/repo/base.meta.json
+-rw-r--r--   0        0        0    12926 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/repo/fun.data.json
+-rw-r--r--   0        0        0     2490 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/repo/fun.meta.json
+-rw-r--r--   0        0        0    12850 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/types.data.json
+-rw-r--r--   0        0        0     1786 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/types.meta.json
+-rw-r--r--   0        0        0   116599 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/util.data.json
+-rw-r--r--   0        0        0     2393 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/git/util.meta.json
+-rw-r--r--   0        0        0    10323 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/glob.data.json
+-rw-r--r--   0        0        0     1755 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/glob.meta.json
+-rw-r--r--   0        0        0    46028 2023-03-24 00:33:08.706805 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/gzip.data.json
+-rw-r--r--   0        0        0     1615 2023-03-24 00:33:08.707126 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/gzip.meta.json
+-rw-r--r--   0        0        0    30047 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/hashlib.data.json
+-rw-r--r--   0        0        0     1840 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/hashlib.meta.json
+-rw-r--r--   0        0        0    12366 2023-03-24 00:33:08.231680 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/heapq.data.json
+-rw-r--r--   0        0        0     1511 2023-03-24 00:33:08.231868 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/heapq.meta.json
+-rw-r--r--   0        0        0    18362 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/hmac.data.json
+-rw-r--r--   0        0        0     1849 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/hmac.meta.json
+-rw-r--r--   0        0        0     4601 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/html/__init__.data.json
+-rw-r--r--   0        0        0     1692 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/html/__init__.meta.json
+-rw-r--r--   0        0        0     2995 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/html/entities.data.json
+-rw-r--r--   0        0        0     1702 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/html/entities.meta.json
+-rw-r--r--   0        0        0    19707 2023-03-24 00:33:08.703443 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/http/__init__.data.json
+-rw-r--r--   0        0        0     1590 2023-03-24 00:33:08.703699 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/http/__init__.meta.json
+-rw-r--r--   0        0        0    64975 2023-03-24 00:33:08.911213 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/http/client.data.json
+-rw-r--r--   0        0        0     1651 2023-03-24 00:33:08.911418 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/http/client.meta.json
+-rw-r--r--   0        0        0    29585 2023-03-24 00:33:08.308792 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/http/cookies.data.json
+-rw-r--r--   0        0        0     1570 2023-03-24 00:33:08.309022 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/http/cookies.meta.json
+-rw-r--r--   0        0        0     9461 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/imghdr.data.json
+-rw-r--r--   0        0        0     1744 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/imghdr.meta.json
+-rw-r--r--   0        0        0     6724 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1766 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    75569 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/importlib/abc.data.json
+-rw-r--r--   0        0        0     1849 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/importlib/abc.meta.json
+-rw-r--r--   0        0        0    69970 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1925 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    97936 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1931 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    12974 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1748 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    82375 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/importlib_metadata/__init__.data.json
+-rw-r--r--   0        0        0     2532 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/importlib_metadata/__init__.meta.json
+-rw-r--r--   0        0        0     7079 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/importlib_metadata/_adapters.data.json
+-rw-r--r--   0        0        0     2008 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/importlib_metadata/_adapters.meta.json
+-rw-r--r--   0        0        0    24836 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/importlib_metadata/_collections.data.json
+-rw-r--r--   0        0        0     1803 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/importlib_metadata/_collections.meta.json
+-rw-r--r--   0        0        0     6087 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/importlib_metadata/_compat.data.json
+-rw-r--r--   0        0        0     1767 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/importlib_metadata/_compat.meta.json
+-rw-r--r--   0        0        0     2330 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/importlib_metadata/_functools.data.json
+-rw-r--r--   0        0        0     1769 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/importlib_metadata/_functools.meta.json
+-rw-r--r--   0        0        0     2314 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/importlib_metadata/_itertools.data.json
+-rw-r--r--   0        0        0     1861 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/importlib_metadata/_itertools.meta.json
+-rw-r--r--   0        0        0    20089 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/importlib_metadata/_meta.data.json
+-rw-r--r--   0        0        0     1738 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/importlib_metadata/_meta.meta.json
+-rw-r--r--   0        0        0     3598 2023-03-26 00:13:35.270572 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/importlib_metadata/_py39compat.data.json
+-rw-r--r--   0        0        0     1778 2023-03-26 00:13:35.270946 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/importlib_metadata/_py39compat.meta.json
+-rw-r--r--   0        0        0     5913 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/importlib_metadata/_text.data.json
+-rw-r--r--   0        0        0     1835 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/importlib_metadata/_text.meta.json
+-rw-r--r--   0        0        0   370620 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/inspect.data.json
+-rw-r--r--   0        0        0     1844 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/inspect.meta.json
+-rw-r--r--   0        0        0    93297 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/io.data.json
+-rw-r--r--   0        0        0     1876 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/io.meta.json
+-rw-r--r--   0        0        0   292387 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/itertools.data.json
+-rw-r--r--   0        0        0     1796 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/itertools.meta.json
+-rw-r--r--   0        0        0    16899 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/json/__init__.data.json
+-rw-r--r--   0        0        0     1781 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/json/__init__.meta.json
+-rw-r--r--   0        0        0    15866 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/json/decoder.data.json
+-rw-r--r--   0        0        0     1725 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/json/decoder.meta.json
+-rw-r--r--   0        0        0    11888 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/json/encoder.data.json
+-rw-r--r--   0        0        0     1737 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/json/encoder.meta.json
+-rw-r--r--   0        0        0    10180 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/linecache.data.json
+-rw-r--r--   0        0        0     1754 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/linecache.meta.json
+-rw-r--r--   0        0        0    35009 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/locale.data.json
+-rw-r--r--   0        0        0     1798 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/locale.meta.json
+-rw-r--r--   0        0        0   154306 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/logging/__init__.data.json
+-rw-r--r--   0        0        0     1889 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/logging/__init__.meta.json
+-rw-r--r--   0        0        0    75364 2023-03-24 00:33:08.951159 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/logging/handlers.data.json
+-rw-r--r--   0        0        0     1739 2023-03-24 00:33:08.951619 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/logging/handlers.meta.json
+-rw-r--r--   0        0        0     2660 2023-03-26 00:13:35.201449 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/__init__.data.json
+-rw-r--r--   0        0        0     1711 2023-03-26 00:13:35.201999 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/__init__.meta.json
+-rw-r--r--   0        0        0     2238 2023-03-26 00:13:34.704258 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/_compat.data.json
+-rw-r--r--   0        0        0     1770 2023-03-26 00:13:34.704668 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/_compat.meta.json
+-rw-r--r--   0        0        0     5115 2023-03-26 00:13:34.328133 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/_punycode.data.json
+-rw-r--r--   0        0        0     1837 2023-03-26 00:13:34.328527 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/_punycode.meta.json
+-rw-r--r--   0        0        0     1744 2023-03-26 00:13:34.328945 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/common/__init__.data.json
+-rw-r--r--   0        0        0     1697 2023-03-26 00:13:34.329370 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/common/__init__.meta.json
+-rw-r--r--   0        0        0     1924 2023-03-26 00:13:34.697644 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/common/entities.data.json
+-rw-r--r--   0        0        0     1774 2023-03-26 00:13:34.698031 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/common/entities.meta.json
+-rw-r--r--   0        0        0     1865 2023-03-26 00:13:34.322693 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/common/html_blocks.data.json
+-rw-r--r--   0        0        0     1714 2023-03-26 00:13:34.322941 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/common/html_blocks.meta.json
+-rw-r--r--   0        0        0     5411 2023-03-26 00:13:34.321727 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/common/html_re.data.json
+-rw-r--r--   0        0        0     1734 2023-03-26 00:13:34.322180 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/common/html_re.meta.json
+-rw-r--r--   0        0        0     6261 2023-03-26 00:13:35.198922 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/common/normalize_url.data.json
+-rw-r--r--   0        0        0     2000 2023-03-26 00:13:35.199527 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/common/normalize_url.meta.json
+-rw-r--r--   0        0        0    15438 2023-03-26 00:13:34.946088 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/common/utils.data.json
+-rw-r--r--   0        0        0     1896 2023-03-26 00:13:34.946457 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/common/utils.meta.json
+-rw-r--r--   0        0        0     2817 2023-03-26 00:13:35.195811 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/helpers/__init__.data.json
+-rw-r--r--   0        0        0     1845 2023-03-26 00:13:35.196197 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/helpers/__init__.meta.json
+-rw-r--r--   0        0        0     5696 2023-03-26 00:13:35.030599 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/helpers/parse_link_destination.data.json
+-rw-r--r--   0        0        0     1802 2023-03-26 00:13:35.031132 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/helpers/parse_link_destination.meta.json
+-rw-r--r--   0        0        0     2547 2023-03-26 00:13:35.194368 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/helpers/parse_link_label.data.json
+-rw-r--r--   0        0        0     1900 2023-03-26 00:13:35.194789 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/helpers/parse_link_label.meta.json
+-rw-r--r--   0        0        0     5856 2023-03-26 00:13:35.027634 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/helpers/parse_link_title.data.json
+-rw-r--r--   0        0        0     1790 2023-03-26 00:13:35.028204 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/helpers/parse_link_title.meta.json
+-rw-r--r--   0        0        0    27407 2023-03-26 00:13:35.200484 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/main.data.json
+-rw-r--r--   0        0        0     2499 2023-03-26 00:13:35.200956 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/main.meta.json
+-rw-r--r--   0        0        0     6421 2023-03-26 00:13:35.197836 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/parser_block.data.json
+-rw-r--r--   0        0        0     2409 2023-03-26 00:13:35.198249 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/parser_block.meta.json
+-rw-r--r--   0        0        0     5356 2023-03-26 00:13:35.195248 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/parser_core.data.json
+-rw-r--r--   0        0        0     2083 2023-03-26 00:13:35.195518 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/parser_core.meta.json
+-rw-r--r--   0        0        0     7763 2023-03-26 00:13:35.196945 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/parser_inline.data.json
+-rw-r--r--   0        0        0     2513 2023-03-26 00:13:35.197330 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/parser_inline.meta.json
+-rw-r--r--   0        0        0     4548 2023-03-26 00:13:34.702779 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/presets/__init__.data.json
+-rw-r--r--   0        0        0     1831 2023-03-26 00:13:34.703316 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/presets/__init__.meta.json
+-rw-r--r--   0        0        0     1830 2023-03-26 00:13:34.326115 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/presets/commonmark.data.json
+-rw-r--r--   0        0        0     1715 2023-03-26 00:13:34.326357 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/presets/commonmark.meta.json
+-rw-r--r--   0        0        0     1806 2023-03-26 00:13:34.325135 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/presets/default.data.json
+-rw-r--r--   0        0        0     1709 2023-03-26 00:13:34.325437 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/presets/default.meta.json
+-rw-r--r--   0        0        0     1782 2023-03-26 00:13:34.324317 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/presets/zero.data.json
+-rw-r--r--   0        0        0     1703 2023-03-26 00:13:34.324602 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/presets/zero.meta.json
+-rw-r--r--   0        0        0    22321 2023-03-26 00:13:35.038870 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/renderer.data.json
+-rw-r--r--   0        0        0     1974 2023-03-26 00:13:35.039452 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/renderer.meta.json
+-rw-r--r--   0        0        0    26281 2023-03-26 00:13:35.166315 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/ruler.data.json
+-rw-r--r--   0        0        0     1947 2023-03-26 00:13:35.166749 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/ruler.meta.json
+-rw-r--r--   0        0        0     3958 2023-03-26 00:13:35.192419 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/__init__.data.json
+-rw-r--r--   0        0        0     2213 2023-03-26 00:13:35.192972 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/__init__.meta.json
+-rw-r--r--   0        0        0     3156 2023-03-26 00:13:35.184176 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/blockquote.data.json
+-rw-r--r--   0        0        0     2003 2023-03-26 00:13:35.184769 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/blockquote.meta.json
+-rw-r--r--   0        0        0     2857 2023-03-26 00:13:35.183157 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/code.data.json
+-rw-r--r--   0        0        0     1845 2023-03-26 00:13:35.183599 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/code.meta.json
+-rw-r--r--   0        0        0     2870 2023-03-26 00:13:35.182393 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/fence.data.json
+-rw-r--r--   0        0        0     1848 2023-03-26 00:13:35.182800 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/fence.meta.json
+-rw-r--r--   0        0        0     3117 2023-03-26 00:13:35.181647 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/heading.data.json
+-rw-r--r--   0        0        0     2000 2023-03-26 00:13:35.182044 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/heading.meta.json
+-rw-r--r--   0        0        0     2938 2023-03-26 00:13:35.180958 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/hr.data.json
+-rw-r--r--   0        0        0     1905 2023-03-26 00:13:35.181274 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/hr.meta.json
+-rw-r--r--   0        0        0     4228 2023-03-26 00:13:35.180356 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/html_block.data.json
+-rw-r--r--   0        0        0     2102 2023-03-26 00:13:35.180659 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/html_block.meta.json
+-rw-r--r--   0        0        0     3005 2023-03-26 00:13:35.179741 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/lheading.data.json
+-rw-r--r--   0        0        0     1980 2023-03-26 00:13:35.180033 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/lheading.meta.json
+-rw-r--r--   0        0        0     5541 2023-03-26 00:13:35.179097 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/list.data.json
+-rw-r--r--   0        0        0     2084 2023-03-26 00:13:35.179429 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/list.meta.json
+-rw-r--r--   0        0        0     3018 2023-03-26 00:13:35.178477 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/paragraph.data.json
+-rw-r--r--   0        0        0     1917 2023-03-26 00:13:35.178727 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/paragraph.meta.json
+-rw-r--r--   0        0        0     3494 2023-03-26 00:13:35.177979 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/reference.data.json
+-rw-r--r--   0        0        0     2009 2023-03-26 00:13:35.178217 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/reference.meta.json
+-rw-r--r--   0        0        0    15095 2023-03-26 00:13:35.168633 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/state_block.data.json
+-rw-r--r--   0        0        0     1889 2023-03-26 00:13:35.168938 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/state_block.meta.json
+-rw-r--r--   0        0        0     4568 2023-03-26 00:13:35.177270 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/table.data.json
+-rw-r--r--   0        0        0     1995 2023-03-26 00:13:35.177647 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_block/table.meta.json
+-rw-r--r--   0        0        0     3303 2023-03-26 00:13:35.193444 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_core/__init__.data.json
+-rw-r--r--   0        0        0     2005 2023-03-26 00:13:35.193933 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_core/__init__.meta.json
+-rw-r--r--   0        0        0     2440 2023-03-26 00:13:35.190239 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_core/block.data.json
+-rw-r--r--   0        0        0     1870 2023-03-26 00:13:35.190802 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_core/block.meta.json
+-rw-r--r--   0        0        0     2356 2023-03-26 00:13:35.189364 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_core/inline.data.json
+-rw-r--r--   0        0        0     1874 2023-03-26 00:13:35.189820 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_core/inline.meta.json
+-rw-r--r--   0        0        0     5499 2023-03-26 00:13:35.188306 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_core/linkify.data.json
+-rw-r--r--   0        0        0     2003 2023-03-26 00:13:35.188885 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_core/linkify.meta.json
+-rw-r--r--   0        0        0     3060 2023-03-26 00:13:35.187283 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_core/normalize.data.json
+-rw-r--r--   0        0        0     1817 2023-03-26 00:13:35.187768 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_core/normalize.meta.json
+-rw-r--r--   0        0        0     8849 2023-03-26 00:13:35.185383 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_core/replacements.data.json
+-rw-r--r--   0        0        0     1949 2023-03-26 00:13:35.185879 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_core/replacements.meta.json
+-rw-r--r--   0        0        0     5686 2023-03-26 00:13:35.186361 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_core/smartquotes.data.json
+-rw-r--r--   0        0        0     2015 2023-03-26 00:13:35.186806 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_core/smartquotes.meta.json
+-rw-r--r--   0        0        0     4895 2023-03-26 00:13:35.169337 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_core/state_core.data.json
+-rw-r--r--   0        0        0     1868 2023-03-26 00:13:35.169670 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_core/state_core.meta.json
+-rw-r--r--   0        0        0     4261 2023-03-26 00:13:35.191396 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/__init__.data.json
+-rw-r--r--   0        0        0     2336 2023-03-26 00:13:35.191840 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/__init__.meta.json
+-rw-r--r--   0        0        0     3119 2023-03-26 00:13:35.175685 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/autolink.data.json
+-rw-r--r--   0        0        0     1851 2023-03-26 00:13:35.175898 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/autolink.meta.json
+-rw-r--r--   0        0        0     2814 2023-03-26 00:13:35.175202 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/backticks.data.json
+-rw-r--r--   0        0        0     1854 2023-03-26 00:13:35.175433 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/backticks.meta.json
+-rw-r--r--   0        0        0     3502 2023-03-26 00:13:35.174694 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/balance_pairs.data.json
+-rw-r--r--   0        0        0     1806 2023-03-26 00:13:35.174958 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/balance_pairs.meta.json
+-rw-r--r--   0        0        0     3744 2023-03-26 00:13:35.176693 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/emphasis.data.json
+-rw-r--r--   0        0        0     1901 2023-03-26 00:13:35.176946 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/emphasis.meta.json
+-rw-r--r--   0        0        0     3519 2023-03-26 00:13:35.174171 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/entity.data.json
+-rw-r--r--   0        0        0     2033 2023-03-26 00:13:35.174393 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/entity.meta.json
+-rw-r--r--   0        0        0     3090 2023-03-26 00:13:35.173649 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/escape.data.json
+-rw-r--r--   0        0        0     1883 2023-03-26 00:13:35.173916 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/escape.meta.json
+-rw-r--r--   0        0        0     3399 2023-03-26 00:13:35.173129 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/html_inline.data.json
+-rw-r--r--   0        0        0     1906 2023-03-26 00:13:35.173368 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/html_inline.meta.json
+-rw-r--r--   0        0        0     2929 2023-03-26 00:13:35.172339 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/image.data.json
+-rw-r--r--   0        0        0     1991 2023-03-26 00:13:35.172799 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/image.meta.json
+-rw-r--r--   0        0        0     2707 2023-03-26 00:13:35.171848 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/link.data.json
+-rw-r--r--   0        0        0     1942 2023-03-26 00:13:35.172084 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/link.meta.json
+-rw-r--r--   0        0        0     3094 2023-03-26 00:13:35.171354 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/newline.data.json
+-rw-r--r--   0        0        0     1885 2023-03-26 00:13:35.171598 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/newline.meta.json
+-rw-r--r--   0        0        0    38094 2023-03-26 00:13:35.167623 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/state_inline.data.json
+-rw-r--r--   0        0        0     2013 2023-03-26 00:13:35.168040 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/state_inline.meta.json
+-rw-r--r--   0        0        0     4517 2023-03-26 00:13:35.176219 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/strikethrough.data.json
+-rw-r--r--   0        0        0     1882 2023-03-26 00:13:35.176431 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/strikethrough.meta.json
+-rw-r--r--   0        0        0     2893 2023-03-26 00:13:35.170654 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/text.data.json
+-rw-r--r--   0        0        0     1788 2023-03-26 00:13:35.171004 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/text.meta.json
+-rw-r--r--   0        0        0     2648 2023-03-26 00:13:35.170037 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/text_collapse.data.json
+-rw-r--r--   0        0        0     1862 2023-03-26 00:13:35.170304 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/rules_inline/text_collapse.meta.json
+-rw-r--r--   0        0        0    24990 2023-03-26 00:13:34.957331 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/token.data.json
+-rw-r--r--   0        0        0     1959 2023-03-26 00:13:34.957714 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/token.meta.json
+-rw-r--r--   0        0        0    32194 2023-03-26 00:13:34.701622 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/utils.data.json
+-rw-r--r--   0        0        0     1792 2023-03-26 00:13:34.702039 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/markdown_it/utils.meta.json
+-rw-r--r--   0        0        0     7022 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/marshal.data.json
+-rw-r--r--   0        0        0     1817 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/marshal.meta.json
+-rw-r--r--   0        0        0    56212 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/math.data.json
+-rw-r--r--   0        0        0     1770 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/math.meta.json
+-rw-r--r--   0        0        0     3581 2023-03-26 00:13:35.031927 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/mdurl/__init__.data.json
+-rw-r--r--   0        0        0     1789 2023-03-26 00:13:35.032492 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/mdurl/__init__.meta.json
+-rw-r--r--   0        0        0     5037 2023-03-26 00:13:34.696335 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/mdurl/_decode.data.json
+-rw-r--r--   0        0        0     1887 2023-03-26 00:13:34.696773 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/mdurl/_decode.meta.json
+-rw-r--r--   0        0        0     4664 2023-03-26 00:13:34.691750 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/mdurl/_encode.data.json
+-rw-r--r--   0        0        0     1809 2023-03-26 00:13:34.692113 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/mdurl/_encode.meta.json
+-rw-r--r--   0        0        0     2420 2023-03-26 00:13:34.941038 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/mdurl/_format.data.json
+-rw-r--r--   0        0        0     1720 2023-03-26 00:13:34.941544 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/mdurl/_format.meta.json
+-rw-r--r--   0        0        0    13572 2023-03-26 00:13:34.938741 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/mdurl/_parse.data.json
+-rw-r--r--   0        0        0     1902 2023-03-26 00:13:34.939219 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/mdurl/_parse.meta.json
+-rw-r--r--   0        0        0    28653 2023-03-26 00:13:34.688064 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/mdurl/_url.data.json
+-rw-r--r--   0        0        0     1693 2023-03-26 00:13:34.688461 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/mdurl/_url.meta.json
+-rw-r--r--   0        0        0    16653 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/mimetypes.data.json
+-rw-r--r--   0        0        0     1765 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/mimetypes.meta.json
+-rw-r--r--   0        0        0    29398 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/mmap.data.json
+-rw-r--r--   0        0        0     1819 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/mmap.meta.json
+-rw-r--r--   0        0        0     1681 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/msvcrt.data.json
+-rw-r--r--   0        0        0     1729 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/msvcrt.meta.json
+-rw-r--r--   0        0        0    34101 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/__init__.data.json
+-rw-r--r--   0        0        0     2174 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/__init__.meta.json
+-rw-r--r--   0        0        0    33273 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/connection.data.json
+-rw-r--r--   0        0        0     1929 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/connection.meta.json
+-rw-r--r--   0        0        0   103632 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/context.data.json
+-rw-r--r--   0        0        0     2338 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/context.meta.json
+-rw-r--r--   0        0        0   160925 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/managers.data.json
+-rw-r--r--   0        0        0     1971 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/managers.meta.json
+-rw-r--r--   0        0        0    56174 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/pool.data.json
+-rw-r--r--   0        0        0     1817 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/pool.meta.json
+-rw-r--r--   0        0        0     9821 2023-03-26 00:13:35.045882 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/popen_fork.data.json
+-rw-r--r--   0        0        0     1804 2023-03-26 00:13:35.046398 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/popen_fork.meta.json
+-rw-r--r--   0        0        0     6245 2023-03-26 00:13:35.236763 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/popen_forkserver.data.json
+-rw-r--r--   0        0        0     1846 2023-03-26 00:13:35.237096 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/popen_forkserver.meta.json
+-rw-r--r--   0        0        0     6966 2023-03-26 00:13:35.235943 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/popen_spawn_posix.data.json
+-rw-r--r--   0        0        0     1848 2023-03-26 00:13:35.236346 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/popen_spawn_posix.meta.json
+-rw-r--r--   0        0        0     2174 2023-03-26 00:13:35.043965 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/popen_spawn_win32.data.json
+-rw-r--r--   0        0        0     1818 2023-03-26 00:13:35.044410 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/popen_spawn_win32.meta.json
+-rw-r--r--   0        0        0    19244 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/process.data.json
+-rw-r--r--   0        0        0     1781 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/process.meta.json
+-rw-r--r--   0        0        0    21490 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/queues.data.json
+-rw-r--r--   0        0        0     1785 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/queues.meta.json
+-rw-r--r--   0        0        0    31446 2023-03-26 00:13:35.234761 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/reduction.data.json
+-rw-r--r--   0        0        0     1991 2023-03-26 00:13:35.235355 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/reduction.meta.json
+-rw-r--r--   0        0        0    31858 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/shared_memory.data.json
+-rw-r--r--   0        0        0     1835 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/shared_memory.meta.json
+-rw-r--r--   0        0        0    73307 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/sharedctypes.data.json
+-rw-r--r--   0        0        0     1906 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/sharedctypes.meta.json
+-rw-r--r--   0        0        0    10733 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/spawn.data.json
+-rw-r--r--   0        0        0     1757 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/spawn.meta.json
+-rw-r--r--   0        0        0    27930 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/synchronize.data.json
+-rw-r--r--   0        0        0     1871 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/synchronize.meta.json
+-rw-r--r--   0        0        0    25680 2023-03-26 00:13:34.959930 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/util.data.json
+-rw-r--r--   0        0        0     1889 2023-03-26 00:13:34.960296 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/multiprocessing/util.meta.json
+-rw-r--r--   0        0        0    86302 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numbers.data.json
+-rw-r--r--   0        0        0     1689 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numbers.meta.json
+-rw-r--r--   0        0        0  2421905 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/__init__.data.json
+-rw-r--r--   0        0        0     3371 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/__init__.meta.json
+-rw-r--r--   0        0        0     5414 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/_pytesttester.data.json
+-rw-r--r--   0        0        0     1717 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/_pytesttester.meta.json
+-rw-r--r--   0        0        0    22920 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/_typing/__init__.data.json
+-rw-r--r--   0        0        0     2096 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/_typing/__init__.meta.json
+-rw-r--r--   0        0        0     4030 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/_typing/_add_docstring.data.json
+-rw-r--r--   0        0        0     1876 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/_typing/_add_docstring.meta.json
+-rw-r--r--   0        0        0    27511 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/_typing/_array_like.data.json
+-rw-r--r--   0        0        0     1867 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/_typing/_array_like.meta.json
+-rw-r--r--   0        0        0   282284 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/_typing/_callable.data.json
+-rw-r--r--   0        0        0     1907 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/_typing/_callable.meta.json
+-rw-r--r--   0        0        0    45448 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/_typing/_char_codes.data.json
+-rw-r--r--   0        0        0     1704 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/_typing/_char_codes.meta.json
+-rw-r--r--   0        0        0    33086 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/_typing/_dtype_like.data.json
+-rw-r--r--   0        0        0     1855 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/_typing/_dtype_like.meta.json
+-rw-r--r--   0        0        0     6267 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/_typing/_extended_precision.data.json
+-rw-r--r--   0        0        0     1761 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/_typing/_extended_precision.meta.json
+-rw-r--r--   0        0        0    37579 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/_typing/_generic_alias.data.json
+-rw-r--r--   0        0        0     1906 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/_typing/_generic_alias.meta.json
+-rw-r--r--   0        0        0     4798 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/_typing/_nbit.data.json
+-rw-r--r--   0        0        0     1691 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/_typing/_nbit.meta.json
+-rw-r--r--   0        0        0    18116 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/_typing/_nested_sequence.data.json
+-rw-r--r--   0        0        0     1762 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/_typing/_nested_sequence.meta.json
+-rw-r--r--   0        0        0     6416 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/_typing/_scalars.data.json
+-rw-r--r--   0        0        0     1713 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/_typing/_scalars.meta.json
+-rw-r--r--   0        0        0     2539 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/_typing/_shape.data.json
+-rw-r--r--   0        0        0     1693 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/_typing/_shape.meta.json
+-rw-r--r--   0        0        0   283387 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/_typing/_ufunc.data.json
+-rw-r--r--   0        0        0     1913 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/_typing/_ufunc.meta.json
+-rw-r--r--   0        0        0     2043 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/_version.data.json
+-rw-r--r--   0        0        0     1720 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/_version.meta.json
+-rw-r--r--   0        0        0     5478 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/compat/__init__.data.json
+-rw-r--r--   0        0        0     1747 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/compat/__init__.meta.json
+-rw-r--r--   0        0        0     6378 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/compat/_inspect.data.json
+-rw-r--r--   0        0        0     1806 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/compat/_inspect.meta.json
+-rw-r--r--   0        0        0    12882 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/compat/py3k.data.json
+-rw-r--r--   0        0        0     1973 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/compat/py3k.meta.json
+-rw-r--r--   0        0        0     1680 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/__init__.data.json
+-rw-r--r--   0        0        0     1684 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/__init__.meta.json
+-rw-r--r--   0        0        0    14899 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/_asarray.data.json
+-rw-r--r--   0        0        0     1828 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/_asarray.meta.json
+-rw-r--r--   0        0        0    23856 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/_internal.data.json
+-rw-r--r--   0        0        0     1752 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/_internal.meta.json
+-rw-r--r--   0        0        0     5260 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/_type_aliases.data.json
+-rw-r--r--   0        0        0     1717 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/_type_aliases.meta.json
+-rw-r--r--   0        0        0    12223 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/_ufunc_config.data.json
+-rw-r--r--   0        0        0     1743 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/_ufunc_config.meta.json
+-rw-r--r--   0        0        0    30585 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/arrayprint.data.json
+-rw-r--r--   0        0        0     1796 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/arrayprint.meta.json
+-rw-r--r--   0        0        0   184203 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/defchararray.data.json
+-rw-r--r--   0        0        0     1849 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/defchararray.meta.json
+-rw-r--r--   0        0        0    39308 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/einsumfunc.data.json
+-rw-r--r--   0        0        0     1874 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/einsumfunc.meta.json
+-rw-r--r--   0        0        0   361315 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/fromnumeric.data.json
+-rw-r--r--   0        0        0     1896 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/fromnumeric.meta.json
+-rw-r--r--   0        0        0    53986 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/function_base.data.json
+-rw-r--r--   0        0        0     1855 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/function_base.meta.json
+-rw-r--r--   0        0        0   328547 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/multiarray.data.json
+-rw-r--r--   0        0        0     1954 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/multiarray.meta.json
+-rw-r--r--   0        0        0   214165 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/numeric.data.json
+-rw-r--r--   0        0        0     1898 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/numeric.meta.json
+-rw-r--r--   0        0        0    49786 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/numerictypes.data.json
+-rw-r--r--   0        0        0     1964 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/numerictypes.meta.json
+-rw-r--r--   0        0        0    27436 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/overrides.data.json
+-rw-r--r--   0        0        0     1969 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/overrides.meta.json
+-rw-r--r--   0        0        0    57493 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/records.data.json
+-rw-r--r--   0        0        0     1913 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/records.meta.json
+-rw-r--r--   0        0        0    57514 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/shape_base.data.json
+-rw-r--r--   0        0        0     1873 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/shape_base.meta.json
+-rw-r--r--   0        0        0     3341 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/umath.data.json
+-rw-r--r--   0        0        0     1744 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/core/umath.meta.json
+-rw-r--r--   0        0        0   122428 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/ctypeslib.data.json
+-rw-r--r--   0        0        0     1990 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/ctypeslib.meta.json
+-rw-r--r--   0        0        0     4677 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/fft/__init__.data.json
+-rw-r--r--   0        0        0     1768 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/fft/__init__.meta.json
+-rw-r--r--   0        0        0    20509 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/fft/_pocketfft.data.json
+-rw-r--r--   0        0        0     1835 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/fft/_pocketfft.meta.json
+-rw-r--r--   0        0        0    23676 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/fft/helper.data.json
+-rw-r--r--   0        0        0     1802 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/fft/helper.meta.json
+-rw-r--r--   0        0        0    26198 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/__init__.data.json
+-rw-r--r--   0        0        0     2402 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/__init__.meta.json
+-rw-r--r--   0        0        0     9746 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/_version.data.json
+-rw-r--r--   0        0        0     1691 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/_version.meta.json
+-rw-r--r--   0        0        0    19706 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/arraypad.data.json
+-rw-r--r--   0        0        0     1807 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/arraypad.meta.json
+-rw-r--r--   0        0        0   168368 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/arraysetops.data.json
+-rw-r--r--   0        0        0     1813 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/arraysetops.meta.json
+-rw-r--r--   0        0        0    28208 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/arrayterator.data.json
+-rw-r--r--   0        0        0     1799 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/arrayterator.meta.json
+-rw-r--r--   0        0        0     7697 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/format.data.json
+-rw-r--r--   0        0        0     1686 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/format.meta.json
+-rw-r--r--   0        0        0   244009 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/function_base.data.json
+-rw-r--r--   0        0        0     2008 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/function_base.meta.json
+-rw-r--r--   0        0        0     9712 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/histograms.data.json
+-rw-r--r--   0        0        0     1819 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/histograms.meta.json
+-rw-r--r--   0        0        0    69132 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/index_tricks.data.json
+-rw-r--r--   0        0        0     1909 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/index_tricks.meta.json
+-rw-r--r--   0        0        0    51587 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/mixins.data.json
+-rw-r--r--   0        0        0     1701 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/mixins.meta.json
+-rw-r--r--   0        0        0    97165 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/nanfunctions.data.json
+-rw-r--r--   0        0        0     1923 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/nanfunctions.meta.json
+-rw-r--r--   0        0        0   105441 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/npyio.data.json
+-rw-r--r--   0        0        0     2039 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/npyio.meta.json
+-rw-r--r--   0        0        0   105129 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/polynomial.data.json
+-rw-r--r--   0        0        0     1812 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/polynomial.meta.json
+-rw-r--r--   0        0        0    67786 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/scimath.data.json
+-rw-r--r--   0        0        0     1804 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/scimath.meta.json
+-rw-r--r--   0        0        0    96870 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/shape_base.data.json
+-rw-r--r--   0        0        0     1925 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/shape_base.meta.json
+-rw-r--r--   0        0        0    25590 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/stride_tricks.data.json
+-rw-r--r--   0        0        0     1841 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/stride_tricks.meta.json
+-rw-r--r--   0        0        0    83910 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/twodim_base.data.json
+-rw-r--r--   0        0        0     1874 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/twodim_base.meta.json
+-rw-r--r--   0        0        0   106065 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/type_check.data.json
+-rw-r--r--   0        0        0     1873 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/type_check.meta.json
+-rw-r--r--   0        0        0    27144 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/ufunclike.data.json
+-rw-r--r--   0        0        0     1808 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/ufunclike.meta.json
+-rw-r--r--   0        0        0    28586 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/utils.data.json
+-rw-r--r--   0        0        0     1788 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/lib/utils.meta.json
+-rw-r--r--   0        0        0     5785 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/linalg/__init__.data.json
+-rw-r--r--   0        0        0     1747 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/linalg/__init__.meta.json
+-rw-r--r--   0        0        0   117226 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/linalg/linalg.data.json
+-rw-r--r--   0        0        0     1858 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/linalg/linalg.meta.json
+-rw-r--r--   0        0        0    29906 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/ma/__init__.data.json
+-rw-r--r--   0        0        0     1758 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/ma/__init__.meta.json
+-rw-r--r--   0        0        0   148307 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/ma/core.data.json
+-rw-r--r--   0        0        0     1780 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/ma/core.meta.json
+-rw-r--r--   0        0        0    25456 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/ma/extras.data.json
+-rw-r--r--   0        0        0     1760 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/ma/extras.meta.json
+-rw-r--r--   0        0        0    15603 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/ma/mrecords.data.json
+-rw-r--r--   0        0        0     1746 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/ma/mrecords.meta.json
+-rw-r--r--   0        0        0     3019 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/matrixlib/__init__.data.json
+-rw-r--r--   0        0        0     1773 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/matrixlib/__init__.meta.json
+-rw-r--r--   0        0        0     6757 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/matrixlib/defmatrix.data.json
+-rw-r--r--   0        0        0     1880 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/matrixlib/defmatrix.meta.json
+-rw-r--r--   0        0        0     4444 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/polynomial/__init__.data.json
+-rw-r--r--   0        0        0     1938 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/polynomial/__init__.meta.json
+-rw-r--r--   0        0        0    29448 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/polynomial/_polybase.data.json
+-rw-r--r--   0        0        0     1707 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/polynomial/_polybase.meta.json
+-rw-r--r--   0        0        0    18024 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/polynomial/chebyshev.data.json
+-rw-r--r--   0        0        0     1794 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/polynomial/chebyshev.meta.json
+-rw-r--r--   0        0        0    15533 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/polynomial/hermite.data.json
+-rw-r--r--   0        0        0     1790 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/polynomial/hermite.meta.json
+-rw-r--r--   0        0        0    15586 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/polynomial/hermite_e.data.json
+-rw-r--r--   0        0        0     1794 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/polynomial/hermite_e.meta.json
+-rw-r--r--   0        0        0    15361 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/polynomial/laguerre.data.json
+-rw-r--r--   0        0        0     1792 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/polynomial/laguerre.meta.json
+-rw-r--r--   0        0        0    15361 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/polynomial/legendre.data.json
+-rw-r--r--   0        0        0     1792 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/polynomial/legendre.meta.json
+-rw-r--r--   0        0        0    14340 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/polynomial/polynomial.data.json
+-rw-r--r--   0        0        0     1796 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/polynomial/polynomial.meta.json
+-rw-r--r--   0        0        0     5080 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/polynomial/polyutils.data.json
+-rw-r--r--   0        0        0     1707 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/polynomial/polyutils.meta.json
+-rw-r--r--   0        0        0    10596 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/random/__init__.data.json
+-rw-r--r--   0        0        0     1939 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/random/__init__.meta.json
+-rw-r--r--   0        0        0   275132 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/random/_generator.data.json
+-rw-r--r--   0        0        0     1939 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/random/_generator.meta.json
+-rw-r--r--   0        0        0    11488 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/random/_mt19937.data.json
+-rw-r--r--   0        0        0     1847 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/random/_mt19937.meta.json
+-rw-r--r--   0        0        0    16790 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/random/_pcg64.data.json
+-rw-r--r--   0        0        0     1752 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/random/_pcg64.meta.json
+-rw-r--r--   0        0        0    12381 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/random/_philox.data.json
+-rw-r--r--   0        0        0     1845 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/random/_philox.meta.json
+-rw-r--r--   0        0        0     9750 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/random/_sfc64.data.json
+-rw-r--r--   0        0        0     1766 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/random/_sfc64.meta.json
+-rw-r--r--   0        0        0    73561 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/random/bit_generator.data.json
+-rw-r--r--   0        0        0     1904 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/random/bit_generator.meta.json
+-rw-r--r--   0        0        0   351985 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/random/mtrand.data.json
+-rw-r--r--   0        0        0     1908 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/random/mtrand.meta.json
+-rw-r--r--   0        0        0     9368 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/testing/__init__.data.json
+-rw-r--r--   0        0        0     1776 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/testing/__init__.meta.json
+-rw-r--r--   0        0        0     1776 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/testing/_private/__init__.data.json
+-rw-r--r--   0        0        0     1705 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/testing/_private/__init__.meta.json
+-rw-r--r--   0        0        0   124418 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/testing/_private/utils.data.json
+-rw-r--r--   0        0        0     2086 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/testing/_private/utils.meta.json
+-rw-r--r--   0        0        0     3098 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/typing/__init__.data.json
+-rw-r--r--   0        0        0     1784 2023-03-26 00:13:30.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/typing/__init__.meta.json
+-rw-r--r--   0        0        0     3560 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/version.data.json
+-rw-r--r--   0        0        0     1752 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/numpy/version.meta.json
+-rw-r--r--   0        0        0     6700 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/opcode.data.json
+-rw-r--r--   0        0        0     1750 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/opcode.meta.json
+-rw-r--r--   0        0        0    51076 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/operator.data.json
+-rw-r--r--   0        0        0     1774 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/operator.meta.json
+-rw-r--r--   0        0        0   351910 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/os/__init__.data.json
+-rw-r--r--   0        0        0     1934 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/os/__init__.meta.json
+-rw-r--r--   0        0        0     5357 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/os/path.data.json
+-rw-r--r--   0        0        0     1723 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/os/path.meta.json
+-rw-r--r--   0        0        0     3259 2023-03-24 00:33:08.332130 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/packaging/__about__.data.json
+-rw-r--r--   0        0        0     1513 2023-03-24 00:33:08.332307 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/packaging/__about__.meta.json
+-rw-r--r--   0        0        0     3503 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/packaging/__init__.data.json
+-rw-r--r--   0        0        0     1681 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/packaging/__init__.meta.json
+-rw-r--r--   0        0        0    15159 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/packaging/_structures.data.json
+-rw-r--r--   0        0        0     1713 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/packaging/_structures.meta.json
+-rw-r--r--   0        0        0    71022 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/packaging/version.data.json
+-rw-r--r--   0        0        0     1924 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/packaging/version.meta.json
+-rw-r--r--   0        0        0    96612 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/pathlib.data.json
+-rw-r--r--   0        0        0     1885 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/pathlib.meta.json
+-rw-r--r--   0        0        0    48578 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/pickle.data.json
+-rw-r--r--   0        0        0     1821 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/pickle.meta.json
+-rw-r--r--   0        0        0    30250 2023-03-24 00:33:08.234375 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/pkgutil.data.json
+-rw-r--r--   0        0        0     1587 2023-03-24 00:33:08.234588 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/pkgutil.meta.json
+-rw-r--r--   0        0        0    38194 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/platform.data.json
+-rw-r--r--   0        0        0     1726 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/platform.meta.json
+-rw-r--r--   0        0        0    82146 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/posixpath.data.json
+-rw-r--r--   0        0        0     1815 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/posixpath.meta.json
+-rw-r--r--   0        0        0     8260 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/pty.data.json
+-rw-r--r--   0        0        0     1748 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/pty.meta.json
+-rw-r--r--   0        0        0   113333 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/pydoc.data.json
+-rw-r--r--   0        0        0     1803 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/pydoc.meta.json
+-rw-r--r--   0        0        0    33319 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/queue.data.json
+-rw-r--r--   0        0        0     1754 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/queue.meta.json
+-rw-r--r--   0        0        0    45145 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/random.data.json
+-rw-r--r--   0        0        0     1801 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/random.meta.json
+-rw-r--r--   0        0        0   182959 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/re.data.json
+-rw-r--r--   0        0        0     1907 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/re.meta.json
+-rw-r--r--   0        0        0    18010 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/reprlib.data.json
+-rw-r--r--   0        0        0     1778 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/reprlib.meta.json
+-rw-r--r--   0        0        0     9126 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/__init__.data.json
+-rw-r--r--   0        0        0     1863 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/__init__.meta.json
+-rw-r--r--   0        0        0     8318 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/__main__.data.json
+-rw-r--r--   0        0        0     2154 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/__main__.meta.json
+-rw-r--r--   0        0        0     1948 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_cell_widths.data.json
+-rw-r--r--   0        0        0     1690 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_cell_widths.meta.json
+-rw-r--r--   0        0        0     1759 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_emoji_codes.data.json
+-rw-r--r--   0        0        0     1691 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_emoji_codes.meta.json
+-rw-r--r--   0        0        0     4481 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_emoji_replace.data.json
+-rw-r--r--   0        0        0     1747 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_emoji_replace.meta.json
+-rw-r--r--   0        0        0     2539 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_export_format.data.json
+-rw-r--r--   0        0        0     1693 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_export_format.meta.json
+-rw-r--r--   0        0        0     2306 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_extension.data.json
+-rw-r--r--   0        0        0     1769 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_extension.meta.json
+-rw-r--r--   0        0        0     2488 2023-03-26 00:13:34.787247 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_fileno.data.json
+-rw-r--r--   0        0        0     1697 2023-03-26 00:13:34.787510 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_fileno.meta.json
+-rw-r--r--   0        0        0    15312 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_inspect.data.json
+-rw-r--r--   0        0        0     2047 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_inspect.meta.json
+-rw-r--r--   0        0        0     8941 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_log_render.data.json
+-rw-r--r--   0        0        0     1877 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_log_render.meta.json
+-rw-r--r--   0        0        0     6328 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_loop.data.json
+-rw-r--r--   0        0        0     1694 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_loop.meta.json
+-rw-r--r--   0        0        0    16768 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_null_file.data.json
+-rw-r--r--   0        0        0     1719 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_null_file.meta.json
+-rw-r--r--   0        0        0     2290 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_palettes.data.json
+-rw-r--r--   0        0        0     1705 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_palettes.meta.json
+-rw-r--r--   0        0        0     2212 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_pick.data.json
+-rw-r--r--   0        0        0     1673 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_pick.meta.json
+-rw-r--r--   0        0        0    10962 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_ratio.data.json
+-rw-r--r--   0        0        0     1831 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_ratio.meta.json
+-rw-r--r--   0        0        0     1826 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_spinners.data.json
+-rw-r--r--   0        0        0     1684 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_spinners.meta.json
+-rw-r--r--   0        0        0     6122 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_stack.data.json
+-rw-r--r--   0        0        0     1675 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_stack.meta.json
+-rw-r--r--   0        0        0     3088 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_timer.data.json
+-rw-r--r--   0        0        0     1730 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_timer.meta.json
+-rw-r--r--   0        0        0    57564 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_win32_console.data.json
+-rw-r--r--   0        0        0     1992 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_win32_console.meta.json
+-rw-r--r--   0        0        0     7305 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_windows.data.json
+-rw-r--r--   0        0        0     1798 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_windows.meta.json
+-rw-r--r--   0        0        0     3297 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_windows_renderer.data.json
+-rw-r--r--   0        0        0     1785 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_windows_renderer.meta.json
+-rw-r--r--   0        0        0     4369 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_wrap.data.json
+-rw-r--r--   0        0        0     1889 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/_wrap.meta.json
+-rw-r--r--   0        0        0     4896 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/abc.data.json
+-rw-r--r--   0        0        0     1769 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/abc.meta.json
+-rw-r--r--   0        0        0    24794 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/align.data.json
+-rw-r--r--   0        0        0     2038 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/align.meta.json
+-rw-r--r--   0        0        0    26527 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/ansi.data.json
+-rw-r--r--   0        0        0     2118 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/ansi.meta.json
+-rw-r--r--   0        0        0    21994 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/box.data.json
+-rw-r--r--   0        0        0     1954 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/box.meta.json
+-rw-r--r--   0        0        0     9223 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/cells.data.json
+-rw-r--r--   0        0        0     1796 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/cells.meta.json
+-rw-r--r--   0        0        0    58324 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/color.data.json
+-rw-r--r--   0        0        0     2194 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/color.meta.json
+-rw-r--r--   0        0        0    21961 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/color_triplet.data.json
+-rw-r--r--   0        0        0     1690 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/color_triplet.meta.json
+-rw-r--r--   0        0        0    11070 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/columns.data.json
+-rw-r--r--   0        0        0     2182 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/columns.meta.json
+-rw-r--r--   0        0        0   186847 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/console.data.json
+-rw-r--r--   0        0        0     3053 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/console.meta.json
+-rw-r--r--   0        0        0     6278 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/constrain.data.json
+-rw-r--r--   0        0        0     1828 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/constrain.meta.json
+-rw-r--r--   0        0        0    21205 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/containers.data.json
+-rw-r--r--   0        0        0     1884 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/containers.meta.json
+-rw-r--r--   0        0        0    23721 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/control.data.json
+-rw-r--r--   0        0        0     1936 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/control.meta.json
+-rw-r--r--   0        0        0     3941 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/default_styles.data.json
+-rw-r--r--   0        0        0     2104 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/default_styles.meta.json
+-rw-r--r--   0        0        0    11474 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/emoji.data.json
+-rw-r--r--   0        0        0     2019 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/emoji.meta.json
+-rw-r--r--   0        0        0     8738 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/errors.data.json
+-rw-r--r--   0        0        0     1676 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/errors.meta.json
+-rw-r--r--   0        0        0     9182 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/file_proxy.data.json
+-rw-r--r--   0        0        0     1911 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/file_proxy.meta.json
+-rw-r--r--   0        0        0    15677 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/highlighter.data.json
+-rw-r--r--   0        0        0     1961 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/highlighter.meta.json
+-rw-r--r--   0        0        0    10567 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/json.data.json
+-rw-r--r--   0        0        0     2065 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/json.meta.json
+-rw-r--r--   0        0        0    10569 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/jupyter.data.json
+-rw-r--r--   0        0        0     1902 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/jupyter.meta.json
+-rw-r--r--   0        0        0    29952 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/live.data.json
+-rw-r--r--   0        0        0     2404 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/live.meta.json
+-rw-r--r--   0        0        0     9724 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/live_render.data.json
+-rw-r--r--   0        0        0     1889 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/live_render.meta.json
+-rw-r--r--   0        0        0    70924 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/markdown.data.json
+-rw-r--r--   0        0        0     2386 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/markdown.meta.json
+-rw-r--r--   0        0        0    27131 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/markup.data.json
+-rw-r--r--   0        0        0     2182 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/markup.meta.json
+-rw-r--r--   0        0        0    24993 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/measure.data.json
+-rw-r--r--   0        0        0     1964 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/measure.meta.json
+-rw-r--r--   0        0        0    13387 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/padding.data.json
+-rw-r--r--   0        0        0     1951 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/padding.meta.json
+-rw-r--r--   0        0        0     6426 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/pager.data.json
+-rw-r--r--   0        0        0     1860 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/pager.meta.json
+-rw-r--r--   0        0        0     9629 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/palette.data.json
+-rw-r--r--   0        0        0     2099 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/palette.meta.json
+-rw-r--r--   0        0        0    18465 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/panel.data.json
+-rw-r--r--   0        0        0     2069 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/panel.meta.json
+-rw-r--r--   0        0        0   119636 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/pretty.data.json
+-rw-r--r--   0        0        0     2275 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/pretty.meta.json
+-rw-r--r--   0        0        0     3686 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/protocol.data.json
+-rw-r--r--   0        0        0     1801 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/protocol.meta.json
+-rw-r--r--   0        0        0    16692 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/region.data.json
+-rw-r--r--   0        0        0     1675 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/region.meta.json
+-rw-r--r--   0        0        0    21469 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/repr.data.json
+-rw-r--r--   0        0        0     1868 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/repr.meta.json
+-rw-r--r--   0        0        0     9054 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/rule.data.json
+-rw-r--r--   0        0        0     1937 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/rule.meta.json
+-rw-r--r--   0        0        0     4556 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/scope.data.json
+-rw-r--r--   0        0        0     1955 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/scope.meta.json
+-rw-r--r--   0        0        0     5794 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/screen.data.json
+-rw-r--r--   0        0        0     1776 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/screen.meta.json
+-rw-r--r--   0        0        0   104321 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/segment.data.json
+-rw-r--r--   0        0        0     2104 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/segment.meta.json
+-rw-r--r--   0        0        0    10929 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/spinner.data.json
+-rw-r--r--   0        0        0     2089 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/spinner.meta.json
+-rw-r--r--   0        0        0    13397 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/status.data.json
+-rw-r--r--   0        0        0     1872 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/status.meta.json
+-rw-r--r--   0        0        0    59267 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/style.data.json
+-rw-r--r--   0        0        0     2047 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/style.meta.json
+-rw-r--r--   0        0        0     6501 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/styled.data.json
+-rw-r--r--   0        0        0     1876 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/styled.meta.json
+-rw-r--r--   0        0        0    80766 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/syntax.data.json
+-rw-r--r--   0        0        0     2467 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/syntax.meta.json
+-rw-r--r--   0        0        0    82010 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/table.data.json
+-rw-r--r--   0        0        0     2326 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/table.meta.json
+-rw-r--r--   0        0        0     6941 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/terminal_theme.data.json
+-rw-r--r--   0        0        0     1742 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/terminal_theme.meta.json
+-rw-r--r--   0        0        0    93178 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/text.data.json
+-rw-r--r--   0        0        0     2352 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/text.meta.json
+-rw-r--r--   0        0        0    15049 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/theme.data.json
+-rw-r--r--   0        0        0     1935 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/theme.meta.json
+-rw-r--r--   0        0        0     1847 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/themes.data.json
+-rw-r--r--   0        0        0     1746 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/themes.meta.json
+-rw-r--r--   0        0        0    51566 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/traceback.data.json
+-rw-r--r--   0        0        0     2448 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/rich/traceback.meta.json
+-rw-r--r--   0        0        0     9600 2023-03-24 00:33:08.232672 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/runpy.data.json
+-rw-r--r--   0        0        0     1540 2023-03-24 00:33:08.232853 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/runpy.meta.json
+-rw-r--r--   0        0        0     7090 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/secrets.data.json
+-rw-r--r--   0        0        0     1738 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/secrets.meta.json
+-rw-r--r--   0        0        0    26327 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/select.data.json
+-rw-r--r--   0        0        0     1788 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/select.meta.json
+-rw-r--r--   0        0        0    60552 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/selectors.data.json
+-rw-r--r--   0        0        0     1843 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/selectors.meta.json
+-rw-r--r--   0        0        0    17828 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/shlex.data.json
+-rw-r--r--   0        0        0     1772 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/shlex.meta.json
+-rw-r--r--   0        0        0    77642 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/shutil.data.json
+-rw-r--r--   0        0        0     1786 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/shutil.meta.json
+-rw-r--r--   0        0        0    34601 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/signal.data.json
+-rw-r--r--   0        0        0     1802 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/signal.meta.json
+-rw-r--r--   0        0        0    88591 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/socket.data.json
+-rw-r--r--   0        0        0     1894 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/socket.meta.json
+-rw-r--r--   0        0        0    15241 2023-03-26 00:13:29.482092 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/sre_compile.data.json
+-rw-r--r--   0        0        0     1751 2023-03-26 00:13:29.483122 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/sre_compile.meta.json
+-rw-r--r--   0        0        0    30295 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/sre_constants.data.json
+-rw-r--r--   0        0        0     1763 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/sre_constants.meta.json
+-rw-r--r--   0        0        0    53745 2023-03-26 00:13:29.479485 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/sre_parse.data.json
+-rw-r--r--   0        0        0     1815 2023-03-26 00:13:29.480046 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/sre_parse.meta.json
+-rw-r--r--   0        0        0   204523 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/ssl.data.json
+-rw-r--r--   0        0        0     1896 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/ssl.meta.json
+-rw-r--r--   0        0        0     7131 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/stat.data.json
+-rw-r--r--   0        0        0     1698 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/stat.meta.json
+-rw-r--r--   0        0        0   114247 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/__init__.data.json
+-rw-r--r--   0        0        0     4548 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/__init__.meta.json
+-rw-r--r--   0        0        0    38223 2023-03-24 00:33:11.235567 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/app_session.data.json
+-rw-r--r--   0        0        0     2871 2023-03-24 00:33:11.236153 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/app_session.meta.json
+-rw-r--r--   0        0        0     6267 2023-03-24 00:33:11.184072 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/beta_util.data.json
+-rw-r--r--   0        0        0     3342 2023-03-24 00:33:11.184298 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/beta_util.meta.json
+-rw-r--r--   0        0        0     5147 2023-03-24 00:33:11.196584 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/caching/__init__.data.json
+-rw-r--r--   0        0        0     3441 2023-03-24 00:33:11.196842 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/caching/__init__.meta.json
+-rw-r--r--   0        0        0    12287 2023-03-24 00:33:11.161229 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/caching/cache_errors.data.json
+-rw-r--r--   0        0        0     1648 2023-03-24 00:33:11.161484 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/caching/cache_errors.meta.json
+-rw-r--r--   0        0        0    25111 2023-03-24 00:33:11.183505 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/caching/cache_utils.data.json
+-rw-r--r--   0        0        0     3717 2023-03-24 00:33:11.183755 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/caching/cache_utils.meta.json
+-rw-r--r--   0        0        0    19603 2023-03-24 00:33:11.175281 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/caching/hashing.data.json
+-rw-r--r--   0        0        0     2384 2023-03-24 00:33:11.175553 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/caching/hashing.meta.json
+-rw-r--r--   0        0        0    50384 2023-03-24 00:33:11.193544 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/caching/memo_decorator.data.json
+-rw-r--r--   0        0        0     2027 2023-03-24 00:33:11.193781 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/caching/memo_decorator.meta.json
+-rw-r--r--   0        0        0    38434 2023-03-24 00:33:11.192508 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/caching/singleton_decorator.data.json
+-rw-r--r--   0        0        0     1798 2023-03-24 00:33:11.192767 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/caching/singleton_decorator.meta.json
+-rw-r--r--   0        0        0     2885 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/case_converters.data.json
+-rw-r--r--   0        0        0     1819 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/case_converters.meta.json
+-rw-r--r--   0        0        0     2185 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/code_util.data.json
+-rw-r--r--   0        0        0     1787 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/code_util.meta.json
+-rw-r--r--   0        0        0     1744 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/commands/__init__.data.json
+-rw-r--r--   0        0        0     1699 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/commands/__init__.meta.json
+-rw-r--r--   0        0        0     3562 2023-03-26 00:13:37.420195 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/commands/execution_control.data.json
+-rw-r--r--   0        0        0     1968 2023-03-26 00:13:37.420613 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/commands/execution_control.meta.json
+-rw-r--r--   0        0        0    16913 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/commands/page_config.data.json
+-rw-r--r--   0        0        0     2353 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/commands/page_config.meta.json
+-rw-r--r--   0        0        0     7357 2023-03-26 00:13:37.423152 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/commands/query_params.data.json
+-rw-r--r--   0        0        0     2044 2023-03-26 00:13:37.423532 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/commands/query_params.meta.json
+-rw-r--r--   0        0        0     1357 2023-03-24 00:33:08.290021 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/components/__init__.data.json
+-rw-r--r--   0        0        0     1493 2023-03-24 00:33:08.290207 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/components/__init__.meta.json
+-rw-r--r--   0        0        0     3250 2023-03-24 00:33:11.233959 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/components/v1/__init__.data.json
+-rw-r--r--   0        0        0     3345 2023-03-24 00:33:11.234486 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/components/v1/__init__.meta.json
+-rw-r--r--   0        0        0     6382 2023-03-24 00:33:11.224336 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/components/v1/component_arrow.data.json
+-rw-r--r--   0        0        0     1746 2023-03-24 00:33:11.225051 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/components/v1/component_arrow.meta.json
+-rw-r--r--   0        0        0    27360 2023-03-24 00:33:11.233213 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/components/v1/components.data.json
+-rw-r--r--   0        0        0     4180 2023-03-24 00:33:11.233587 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/components/v1/components.meta.json
+-rw-r--r--   0        0        0    29269 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/config.data.json
+-rw-r--r--   0        0        0     2263 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/config.meta.json
+-rw-r--r--   0        0        0    15521 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/config_option.data.json
+-rw-r--r--   0        0        0     2021 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/config_option.meta.json
+-rw-r--r--   0        0        0     4578 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/config_util.data.json
+-rw-r--r--   0        0        0     1862 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/config_util.meta.json
+-rw-r--r--   0        0        0    28996 2023-03-24 00:33:11.229307 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/credentials.data.json
+-rw-r--r--   0        0        0     1888 2023-03-24 00:33:11.230186 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/credentials.meta.json
+-rw-r--r--   0        0        0    34252 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/cursor.data.json
+-rw-r--r--   0        0        0     1863 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/cursor.meta.json
+-rw-r--r--   0        0        0    75557 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/delta_generator.data.json
+-rw-r--r--   0        0        0     4519 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/delta_generator.meta.json
+-rw-r--r--   0        0        0    16198 2023-03-26 00:13:37.381681 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/deprecation_util.data.json
+-rw-r--r--   0        0        0     3713 2023-03-26 00:13:37.381997 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/deprecation_util.meta.json
+-rw-r--r--   0        0        0     1767 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/development.data.json
+-rw-r--r--   0        0        0     1696 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/development.meta.json
+-rw-r--r--   0        0        0     5352 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/echo.data.json
+-rw-r--r--   0        0        0     1914 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/echo.meta.json
+-rw-r--r--   0        0        0     2339 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/__init__.data.json
+-rw-r--r--   0        0        0     1700 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/__init__.meta.json
+-rw-r--r--   0        0        0    12100 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/alert.data.json
+-rw-r--r--   0        0        0     3738 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/alert.meta.json
+-rw-r--r--   0        0        0    21585 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/arrow.data.json
+-rw-r--r--   0        0        0     3970 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/arrow.meta.json
+-rw-r--r--   0        0        0    26183 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/arrow_altair.data.json
+-rw-r--r--   0        0        0     4067 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/arrow_altair.meta.json
+-rw-r--r--   0        0        0    10690 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/arrow_vega_lite.data.json
+-rw-r--r--   0        0        0     4056 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/arrow_vega_lite.meta.json
+-rw-r--r--   0        0        0     5751 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/balloons.data.json
+-rw-r--r--   0        0        0     3654 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/balloons.meta.json
+-rw-r--r--   0        0        0     8407 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/bokeh_chart.data.json
+-rw-r--r--   0        0        0     3844 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/bokeh_chart.meta.json
+-rw-r--r--   0        0        0    23639 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/button.data.json
+-rw-r--r--   0        0        0     4199 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/button.meta.json
+-rw-r--r--   0        0        0    17690 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/camera_input.data.json
+-rw-r--r--   0        0        0     4044 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/camera_input.meta.json
+-rw-r--r--   0        0        0    16413 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/checkbox.data.json
+-rw-r--r--   0        0        0     3902 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/checkbox.meta.json
+-rw-r--r--   0        0        0    16942 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/color_picker.data.json
+-rw-r--r--   0        0        0     4066 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/color_picker.meta.json
+-rw-r--r--   0        0        0    47722 2023-03-26 00:13:37.432111 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/data_editor.data.json
+-rw-r--r--   0        0        0     4323 2023-03-26 00:13:37.432887 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/data_editor.meta.json
+-rw-r--r--   0        0        0    24938 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/dataframe_selector.data.json
+-rw-r--r--   0        0        0     3676 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/dataframe_selector.meta.json
+-rw-r--r--   0        0        0     9889 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/deck_gl_json_chart.data.json
+-rw-r--r--   0        0        0     3790 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/deck_gl_json_chart.meta.json
+-rw-r--r--   0        0        0     9550 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/doc_string.data.json
+-rw-r--r--   0        0        0     3836 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/doc_string.meta.json
+-rw-r--r--   0        0        0     4812 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/empty.data.json
+-rw-r--r--   0        0        0     3607 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/empty.meta.json
+-rw-r--r--   0        0        0    12639 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/exception.data.json
+-rw-r--r--   0        0        0     3913 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/exception.meta.json
+-rw-r--r--   0        0        0    37030 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/file_uploader.data.json
+-rw-r--r--   0        0        0     4203 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/file_uploader.meta.json
+-rw-r--r--   0        0        0    28764 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/form.data.json
+-rw-r--r--   0        0        0     3910 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/form.meta.json
+-rw-r--r--   0        0        0     9193 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/graphviz_chart.data.json
+-rw-r--r--   0        0        0     3935 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/graphviz_chart.meta.json
+-rw-r--r--   0        0        0    10380 2023-03-26 00:13:37.401938 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/heading.data.json
+-rw-r--r--   0        0        0     3714 2023-03-26 00:13:37.402350 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/heading.meta.json
+-rw-r--r--   0        0        0     9416 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/iframe.data.json
+-rw-r--r--   0        0        0     3650 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/iframe.meta.json
+-rw-r--r--   0        0        0    27006 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/image.data.json
+-rw-r--r--   0        0        0     4317 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/image.meta.json
+-rw-r--r--   0        0        0     7184 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/json.data.json
+-rw-r--r--   0        0        0     3871 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/json.meta.json
+-rw-r--r--   0        0        0    14359 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/layouts.data.json
+-rw-r--r--   0        0        0     3768 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/layouts.meta.json
+-rw-r--r--   0        0        0    17515 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/legacy_altair.data.json
+-rw-r--r--   0        0        0     4015 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/legacy_altair.meta.json
+-rw-r--r--   0        0        0    37328 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/legacy_data_frame.data.json
+-rw-r--r--   0        0        0     4210 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/legacy_data_frame.meta.json
+-rw-r--r--   0        0        0     9896 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/legacy_vega_lite.data.json
+-rw-r--r--   0        0        0     4027 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/legacy_vega_lite.meta.json
+-rw-r--r--   0        0        0     1776 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/lib/__init__.data.json
+-rw-r--r--   0        0        0     1707 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/lib/__init__.meta.json
+-rw-r--r--   0        0        0     2482 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/lib/dicttools.data.json
+-rw-r--r--   0        0        0     1755 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/lib/dicttools.meta.json
+-rw-r--r--   0        0        0    13495 2023-03-26 00:13:34.547467 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/lib/streamlit_plotly_theme.data.json
+-rw-r--r--   0        0        0     1814 2023-03-26 00:13:34.547859 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/lib/streamlit_plotly_theme.meta.json
+-rw-r--r--   0        0        0    11719 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/map.data.json
+-rw-r--r--   0        0        0     3985 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/map.meta.json
+-rw-r--r--   0        0        0    11870 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/markdown.data.json
+-rw-r--r--   0        0        0     3731 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/markdown.meta.json
+-rw-r--r--   0        0        0    17601 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/media.data.json
+-rw-r--r--   0        0        0     4282 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/media.meta.json
+-rw-r--r--   0        0        0    17986 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/metric.data.json
+-rw-r--r--   0        0        0     3961 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/metric.meta.json
+-rw-r--r--   0        0        0    33284 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/multiselect.data.json
+-rw-r--r--   0        0        0     4030 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/multiselect.meta.json
+-rw-r--r--   0        0        0    20638 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/number_input.data.json
+-rw-r--r--   0        0        0     4135 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/number_input.meta.json
+-rw-r--r--   0        0        0    16593 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/plotly_chart.data.json
+-rw-r--r--   0        0        0     4478 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/plotly_chart.meta.json
+-rw-r--r--   0        0        0     7025 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/progress.data.json
+-rw-r--r--   0        0        0     3801 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/progress.meta.json
+-rw-r--r--   0        0        0    11709 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/pyplot.data.json
+-rw-r--r--   0        0        0     4035 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/pyplot.meta.json
+-rw-r--r--   0        0        0    23192 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/radio.data.json
+-rw-r--r--   0        0        0     4077 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/radio.meta.json
+-rw-r--r--   0        0        0    29955 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/select_slider.data.json
+-rw-r--r--   0        0        0     4087 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/select_slider.meta.json
+-rw-r--r--   0        0        0    23468 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/selectbox.data.json
+-rw-r--r--   0        0        0     4085 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/selectbox.meta.json
+-rw-r--r--   0        0        0     3425 2023-03-26 00:13:37.394260 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/show.data.json
+-rw-r--r--   0        0        0     3731 2023-03-26 00:13:37.394655 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/show.meta.json
+-rw-r--r--   0        0        0    34759 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/slider.data.json
+-rw-r--r--   0        0        0     4238 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/slider.meta.json
+-rw-r--r--   0        0        0     5567 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/snow.data.json
+-rw-r--r--   0        0        0     3646 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/snow.meta.json
+-rw-r--r--   0        0        0     3415 2023-03-26 00:13:37.422434 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/spinner.data.json
+-rw-r--r--   0        0        0     3904 2023-03-26 00:13:37.422751 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/spinner.meta.json
+-rw-r--r--   0        0        0     5858 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/text.data.json
+-rw-r--r--   0        0        0     3709 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/text.meta.json
+-rw-r--r--   0        0        0    28974 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/text_widgets.data.json
+-rw-r--r--   0        0        0     4059 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/text_widgets.meta.json
+-rw-r--r--   0        0        0    43633 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/time_widgets.data.json
+-rw-r--r--   0        0        0     4055 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/time_widgets.meta.json
+-rw-r--r--   0        0        0     7402 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/utils.data.json
+-rw-r--r--   0        0        0     3804 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/utils.meta.json
+-rw-r--r--   0        0        0     7967 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/write.data.json
+-rw-r--r--   0        0        0     4137 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/elements/write.meta.json
+-rw-r--r--   0        0        0     1749 2023-03-26 00:13:34.621890 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/emojis.data.json
+-rw-r--r--   0        0        0     1688 2023-03-26 00:13:34.622285 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/emojis.meta.json
+-rw-r--r--   0        0        0     3539 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/env_util.data.json
+-rw-r--r--   0        0        0     1916 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/env_util.meta.json
+-rw-r--r--   0        0        0     4816 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/error_util.data.json
+-rw-r--r--   0        0        0     3998 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/error_util.meta.json
+-rw-r--r--   0        0        0    14122 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/errors.data.json
+-rw-r--r--   0        0        0     1790 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/errors.meta.json
+-rw-r--r--   0        0        0    10558 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/file_util.data.json
+-rw-r--r--   0        0        0     2019 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/file_util.meta.json
+-rw-r--r--   0        0        0     4750 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/folder_black_list.data.json
+-rw-r--r--   0        0        0     1829 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/folder_black_list.meta.json
+-rw-r--r--   0        0        0    17523 2023-03-24 00:33:11.167304 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/forward_msg_cache.data.json
+-rw-r--r--   0        0        0     1926 2023-03-24 00:33:11.167577 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/forward_msg_cache.meta.json
+-rw-r--r--   0        0        0     9129 2023-03-24 00:33:11.167906 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/forward_msg_queue.data.json
+-rw-r--r--   0        0        0     1716 2023-03-24 00:33:11.168291 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/forward_msg_queue.meta.json
+-rw-r--r--   0        0        0    12587 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/git_util.data.json
+-rw-r--r--   0        0        0     1877 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/git_util.meta.json
+-rw-r--r--   0        0        0     1684 2023-03-24 00:33:11.230825 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/hello/Hello.data.json
+-rw-r--r--   0        0        0     3432 2023-03-24 00:33:11.231328 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/hello/Hello.meta.json
+-rw-r--r--   0        0        0     1322 2023-03-24 00:33:08.326679 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/hello/__init__.data.json
+-rw-r--r--   0        0        0     1483 2023-03-24 00:33:08.326887 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/hello/__init__.meta.json
+-rw-r--r--   0        0        0    25656 2023-03-24 00:33:11.169916 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/in_memory_file_manager.data.json
+-rw-r--r--   0        0        0     1947 2023-03-24 00:33:11.170159 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/in_memory_file_manager.meta.json
+-rw-r--r--   0        0        0     8447 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/js_number.data.json
+-rw-r--r--   0        0        0     1821 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/js_number.meta.json
+-rw-r--r--   0        0        0     1923 2023-03-24 00:33:11.197063 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/legacy_caching/__init__.data.json
+-rw-r--r--   0        0        0     1544 2023-03-24 00:33:11.197278 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/legacy_caching/__init__.meta.json
+-rw-r--r--   0        0        0    81624 2023-03-24 00:33:11.195463 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/legacy_caching/caching.data.json
+-rw-r--r--   0        0        0     4084 2023-03-24 00:33:11.195710 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/legacy_caching/caching.meta.json
+-rw-r--r--   0        0        0    67319 2023-03-24 00:33:11.177361 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/legacy_caching/hashing.data.json
+-rw-r--r--   0        0        0     2600 2023-03-24 00:33:11.177632 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/legacy_caching/hashing.meta.json
+-rw-r--r--   0        0        0     6303 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/logger.data.json
+-rw-r--r--   0        0        0     1960 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/logger.meta.json
+-rw-r--r--   0        0        0     3048 2023-03-24 00:33:08.740984 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/magic.data.json
+-rw-r--r--   0        0        0     1571 2023-03-24 00:33:08.741375 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/magic.meta.json
+-rw-r--r--   0        0        0     7174 2023-03-24 00:33:11.227597 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/metrics_util.data.json
+-rw-r--r--   0        0        0     1631 2023-03-24 00:33:11.228235 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/metrics_util.meta.json
+-rw-r--r--   0        0        0     5633 2023-03-24 00:33:11.166511 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/net_util.data.json
+-rw-r--r--   0        0        0     1717 2023-03-24 00:33:11.166808 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/net_util.meta.json
+-rw-r--r--   0        0        0     5266 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Alert_pb2.data.json
+-rw-r--r--   0        0        0     1728 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Alert_pb2.meta.json
+-rw-r--r--   0        0        0     4861 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/AppPage_pb2.data.json
+-rw-r--r--   0        0        0     1732 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/AppPage_pb2.meta.json
+-rw-r--r--   0        0        0     5318 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/ArrowNamedDataSet_pb2.data.json
+-rw-r--r--   0        0        0     1816 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/ArrowNamedDataSet_pb2.meta.json
+-rw-r--r--   0        0        0     5502 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/ArrowVegaLiteChart_pb2.data.json
+-rw-r--r--   0        0        0     1867 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/ArrowVegaLiteChart_pb2.meta.json
+-rw-r--r--   0        0        0     6184 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Arrow_pb2.data.json
+-rw-r--r--   0        0        0     1728 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Arrow_pb2.meta.json
+-rw-r--r--   0        0        0     4795 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Audio_pb2.data.json
+-rw-r--r--   0        0        0     1728 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Audio_pb2.meta.json
+-rw-r--r--   0        0        0     5000 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/BackMsg_pb2.data.json
+-rw-r--r--   0        0        0     1802 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/BackMsg_pb2.meta.json
+-rw-r--r--   0        0        0     4894 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Balloons_pb2.data.json
+-rw-r--r--   0        0        0     1734 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Balloons_pb2.meta.json
+-rw-r--r--   0        0        0     8125 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Block_pb2.data.json
+-rw-r--r--   0        0        0     1822 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Block_pb2.meta.json
+-rw-r--r--   0        0        0     4960 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/BokehChart_pb2.data.json
+-rw-r--r--   0        0        0     1738 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/BokehChart_pb2.meta.json
+-rw-r--r--   0        0        0     4828 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Button_pb2.data.json
+-rw-r--r--   0        0        0     1730 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Button_pb2.meta.json
+-rw-r--r--   0        0        0     5154 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/CameraInput_pb2.data.json
+-rw-r--r--   0        0        0     1821 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/CameraInput_pb2.meta.json
+-rw-r--r--   0        0        0     5055 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Checkbox_pb2.data.json
+-rw-r--r--   0        0        0     1815 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Checkbox_pb2.meta.json
+-rw-r--r--   0        0        0     5134 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/ClientState_pb2.data.json
+-rw-r--r--   0        0        0     1811 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/ClientState_pb2.meta.json
+-rw-r--r--   0        0        0     5154 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/ColorPicker_pb2.data.json
+-rw-r--r--   0        0        0     1821 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/ColorPicker_pb2.meta.json
+-rw-r--r--   0        0        0    11485 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Common_pb2.data.json
+-rw-r--r--   0        0        0     1731 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Common_pb2.meta.json
+-rw-r--r--   0        0        0     8890 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Components_pb2.data.json
+-rw-r--r--   0        0        0     1739 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Components_pb2.meta.json
+-rw-r--r--   0        0        0    18358 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/DataFrame_pb2.data.json
+-rw-r--r--   0        0        0     1802 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/DataFrame_pb2.meta.json
+-rw-r--r--   0        0        0     5088 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/DateInput_pb2.data.json
+-rw-r--r--   0        0        0     1817 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/DateInput_pb2.meta.json
+-rw-r--r--   0        0        0     5125 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/DeckGlJsonChart_pb2.data.json
+-rw-r--r--   0        0        0     1748 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/DeckGlJsonChart_pb2.meta.json
+-rw-r--r--   0        0        0     5345 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Delta_pb2.data.json
+-rw-r--r--   0        0        0     1924 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Delta_pb2.meta.json
+-rw-r--r--   0        0        0     4927 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/DocString_pb2.data.json
+-rw-r--r--   0        0        0     1736 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/DocString_pb2.meta.json
+-rw-r--r--   0        0        0     5092 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/DownloadButton_pb2.data.json
+-rw-r--r--   0        0        0     1746 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/DownloadButton_pb2.meta.json
+-rw-r--r--   0        0        0    10485 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Element_pb2.data.json
+-rw-r--r--   0        0        0     3459 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Element_pb2.meta.json
+-rw-r--r--   0        0        0     4795 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Empty_pb2.data.json
+-rw-r--r--   0        0        0     1728 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Empty_pb2.meta.json
+-rw-r--r--   0        0        0     4927 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Exception_pb2.data.json
+-rw-r--r--   0        0        0     1736 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Exception_pb2.meta.json
+-rw-r--r--   0        0        0     4861 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Favicon_pb2.data.json
+-rw-r--r--   0        0        0     1732 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Favicon_pb2.meta.json
+-rw-r--r--   0        0        0     5187 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/FileUploader_pb2.data.json
+-rw-r--r--   0        0        0     1823 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/FileUploader_pb2.meta.json
+-rw-r--r--   0        0        0     8895 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/ForwardMsg_pb2.data.json
+-rw-r--r--   0        0        0     2186 2023-03-26 00:13:36.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/ForwardMsg_pb2.meta.json
+-rw-r--r--   0        0        0     5353 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/GitInfo_pb2.data.json
+-rw-r--r--   0        0        0     1732 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/GitInfo_pb2.meta.json
+-rw-r--r--   0        0        0     5059 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/GraphVizChart_pb2.data.json
+-rw-r--r--   0        0        0     1744 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/GraphVizChart_pb2.meta.json
+-rw-r--r--   0        0        0     4861 2023-03-26 00:13:34.563723 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Heading_pb2.data.json
+-rw-r--r--   0        0        0     1732 2023-03-26 00:13:34.564231 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Heading_pb2.meta.json
+-rw-r--r--   0        0        0     4828 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/IFrame_pb2.data.json
+-rw-r--r--   0        0        0     1823 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/IFrame_pb2.meta.json
+-rw-r--r--   0        0        0     5716 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Image_pb2.data.json
+-rw-r--r--   0        0        0     1728 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Image_pb2.meta.json
+-rw-r--r--   0        0        0     4762 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Json_pb2.data.json
+-rw-r--r--   0        0        0     1726 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Json_pb2.meta.json
+-rw-r--r--   0        0        0     5977 2023-03-26 00:13:34.528173 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/LabelVisibilityMessage_pb2.data.json
+-rw-r--r--   0        0        0     1762 2023-03-26 00:13:34.528567 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/LabelVisibilityMessage_pb2.meta.json
+-rw-r--r--   0        0        0     5377 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Markdown_pb2.data.json
+-rw-r--r--   0        0        0     1734 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Markdown_pb2.meta.json
+-rw-r--r--   0        0        0     5985 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Metric_pb2.data.json
+-rw-r--r--   0        0        0     1811 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Metric_pb2.meta.json
+-rw-r--r--   0        0        0     5154 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/MultiSelect_pb2.data.json
+-rw-r--r--   0        0        0     1821 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/MultiSelect_pb2.meta.json
+-rw-r--r--   0        0        0     5161 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/NamedDataSet_pb2.data.json
+-rw-r--r--   0        0        0     1810 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/NamedDataSet_pb2.meta.json
+-rw-r--r--   0        0        0    11120 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/NewSession_pb2.data.json
+-rw-r--r--   0        0        0     1850 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/NewSession_pb2.meta.json
+-rw-r--r--   0        0        0     5667 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/NumberInput_pb2.data.json
+-rw-r--r--   0        0        0     1915 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/NumberInput_pb2.meta.json
+-rw-r--r--   0        0        0     6490 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/PageConfig_pb2.data.json
+-rw-r--r--   0        0        0     1738 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/PageConfig_pb2.meta.json
+-rw-r--r--   0        0        0     4894 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/PageInfo_pb2.data.json
+-rw-r--r--   0        0        0     1734 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/PageInfo_pb2.meta.json
+-rw-r--r--   0        0        0     5026 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/PageNotFound_pb2.data.json
+-rw-r--r--   0        0        0     1742 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/PageNotFound_pb2.meta.json
+-rw-r--r--   0        0        0     6889 2023-03-26 00:13:34.673552 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/PageProfile_pb2.data.json
+-rw-r--r--   0        0        0     1741 2023-03-26 00:13:34.673892 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/PageProfile_pb2.meta.json
+-rw-r--r--   0        0        0     5157 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/PagesChanged_pb2.data.json
+-rw-r--r--   0        0        0     1808 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/PagesChanged_pb2.meta.json
+-rw-r--r--   0        0        0     5932 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/PlotlyChart_pb2.data.json
+-rw-r--r--   0        0        0     1740 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/PlotlyChart_pb2.meta.json
+-rw-r--r--   0        0        0     4894 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Progress_pb2.data.json
+-rw-r--r--   0        0        0     1734 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Progress_pb2.meta.json
+-rw-r--r--   0        0        0     4956 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Radio_pb2.data.json
+-rw-r--r--   0        0        0     1809 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Radio_pb2.meta.json
+-rw-r--r--   0        0        0     5952 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/RootContainer_pb2.data.json
+-rw-r--r--   0        0        0     1778 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/RootContainer_pb2.meta.json
+-rw-r--r--   0        0        0     5088 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Selectbox_pb2.data.json
+-rw-r--r--   0        0        0     1817 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Selectbox_pb2.meta.json
+-rw-r--r--   0        0        0     5161 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/SessionEvent_pb2.data.json
+-rw-r--r--   0        0        0     1810 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/SessionEvent_pb2.meta.json
+-rw-r--r--   0        0        0     4491 2023-03-24 00:33:08.644534 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/SessionState_pb2.data.json
+-rw-r--r--   0        0        0     1563 2023-03-24 00:33:08.644878 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/SessionState_pb2.meta.json
+-rw-r--r--   0        0        0     5059 2023-03-26 00:13:34.629158 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/SessionStatus_pb2.data.json
+-rw-r--r--   0        0        0     1744 2023-03-26 00:13:34.629557 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/SessionStatus_pb2.meta.json
+-rw-r--r--   0        0        0     5943 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Slider_pb2.data.json
+-rw-r--r--   0        0        0     1905 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Slider_pb2.meta.json
+-rw-r--r--   0        0        0     4762 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Snow_pb2.data.json
+-rw-r--r--   0        0        0     1726 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Snow_pb2.meta.json
+-rw-r--r--   0        0        0     4861 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Spinner_pb2.data.json
+-rw-r--r--   0        0        0     1732 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Spinner_pb2.meta.json
+-rw-r--r--   0        0        0     5055 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/TextArea_pb2.data.json
+-rw-r--r--   0        0        0     1815 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/TextArea_pb2.meta.json
+-rw-r--r--   0        0        0     5577 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/TextInput_pb2.data.json
+-rw-r--r--   0        0        0     1817 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/TextInput_pb2.meta.json
+-rw-r--r--   0        0        0     4762 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Text_pb2.data.json
+-rw-r--r--   0        0        0     1726 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Text_pb2.meta.json
+-rw-r--r--   0        0        0     5088 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/TimeInput_pb2.data.json
+-rw-r--r--   0        0        0     1817 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/TimeInput_pb2.meta.json
+-rw-r--r--   0        0        0     5335 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/VegaLiteChart_pb2.data.json
+-rw-r--r--   0        0        0     1856 2023-03-26 00:13:35.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/VegaLiteChart_pb2.meta.json
+-rw-r--r--   0        0        0     5260 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Video_pb2.data.json
+-rw-r--r--   0        0        0     1728 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/Video_pb2.meta.json
+-rw-r--r--   0        0        0     6267 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/WidgetStates_pb2.data.json
+-rw-r--r--   0        0        0     1943 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/WidgetStates_pb2.meta.json
+-rw-r--r--   0        0        0     1720 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/__init__.data.json
+-rw-r--r--   0        0        0     1693 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/__init__.meta.json
+-rw-r--r--   0        0        0    23305 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/openmetrics_data_model_pb2.data.json
+-rw-r--r--   0        0        0     1890 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/proto/openmetrics_data_model_pb2.meta.json
+-rw-r--r--   0        0        0     3622 2023-03-26 00:13:37.475226 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/__init__.data.json
+-rw-r--r--   0        0        0     1778 2023-03-26 00:13:37.475447 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/__init__.meta.json
+-rw-r--r--   0        0        0    47947 2023-03-26 00:13:37.416393 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/app_session.data.json
+-rw-r--r--   0        0        0     3440 2023-03-26 00:13:37.416722 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/app_session.meta.json
+-rw-r--r--   0        0        0    11952 2023-03-26 00:13:37.470050 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/__init__.data.json
+-rw-r--r--   0        0        0     3939 2023-03-26 00:13:37.470406 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/__init__.meta.json
+-rw-r--r--   0        0        0    62627 2023-03-26 00:13:37.467437 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/cache_data_api.data.json
+-rw-r--r--   0        0        0     4580 2023-03-26 00:13:37.467777 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/cache_data_api.meta.json
+-rw-r--r--   0        0        0    20074 2023-03-26 00:13:37.393520 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/cache_errors.data.json
+-rw-r--r--   0        0        0     1889 2023-03-26 00:13:37.393840 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/cache_errors.meta.json
+-rw-r--r--   0        0        0    60641 2023-03-26 00:13:37.466040 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/cache_resource_api.data.json
+-rw-r--r--   0        0        0     4290 2023-03-26 00:13:37.466429 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/cache_resource_api.meta.json
+-rw-r--r--   0        0        0     4153 2023-03-26 00:13:34.647066 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/cache_type.data.json
+-rw-r--r--   0        0        0     1743 2023-03-26 00:13:34.647439 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/cache_type.meta.json
+-rw-r--r--   0        0        0    36688 2023-03-26 00:13:37.425161 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/cache_utils.data.json
+-rw-r--r--   0        0        0     2469 2023-03-26 00:13:37.425418 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/cache_utils.meta.json
+-rw-r--r--   0        0        0    60878 2023-03-26 00:13:37.414680 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/cached_message_replay.data.json
+-rw-r--r--   0        0        0     4502 2023-03-26 00:13:37.415002 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/cached_message_replay.meta.json
+-rw-r--r--   0        0        0    22736 2023-03-26 00:13:37.396721 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/hashing.data.json
+-rw-r--r--   0        0        0     2646 2023-03-26 00:13:37.397214 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/hashing.meta.json
+-rw-r--r--   0        0        0     2679 2023-03-26 00:13:35.004924 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/storage/__init__.data.json
+-rw-r--r--   0        0        0     1797 2023-03-26 00:13:35.005393 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/storage/__init__.meta.json
+-rw-r--r--   0        0        0    25069 2023-03-26 00:13:34.881357 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/storage/cache_storage_protocol.data.json
+-rw-r--r--   0        0        0     1838 2023-03-26 00:13:34.881717 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/storage/cache_storage_protocol.meta.json
+-rw-r--r--   0        0        0    11536 2023-03-26 00:13:37.397861 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/storage/dummy_cache_storage.data.json
+-rw-r--r--   0        0        0     1925 2023-03-26 00:13:37.398299 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/storage/dummy_cache_storage.meta.json
+-rw-r--r--   0        0        0    19726 2023-03-26 00:13:37.378167 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.data.json
+-rw-r--r--   0        0        0     2203 2023-03-26 00:13:37.378498 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.meta.json
+-rw-r--r--   0        0        0    32388 2023-03-26 00:13:37.355764 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/credentials.data.json
+-rw-r--r--   0        0        0     2164 2023-03-26 00:13:37.356181 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/credentials.meta.json
+-rw-r--r--   0        0        0    20508 2023-03-26 00:13:37.359680 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/forward_msg_cache.data.json
+-rw-r--r--   0        0        0     2154 2023-03-26 00:13:37.360349 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/forward_msg_cache.meta.json
+-rw-r--r--   0        0        0    10750 2023-03-26 00:13:37.345044 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/forward_msg_queue.data.json
+-rw-r--r--   0        0        0     1911 2023-03-26 00:13:37.345464 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/forward_msg_queue.meta.json
+-rw-r--r--   0        0        0     2426 2023-03-26 00:13:37.474663 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/legacy_caching/__init__.data.json
+-rw-r--r--   0        0        0     1778 2023-03-26 00:13:37.474947 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/legacy_caching/__init__.meta.json
+-rw-r--r--   0        0        0   110850 2023-03-26 00:13:37.472220 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/legacy_caching/caching.data.json
+-rw-r--r--   0        0        0     4531 2023-03-26 00:13:37.472574 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/legacy_caching/caching.meta.json
+-rw-r--r--   0        0        0    71781 2023-03-26 00:13:37.380485 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/legacy_caching/hashing.data.json
+-rw-r--r--   0        0        0     2807 2023-03-26 00:13:37.380985 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/legacy_caching/hashing.meta.json
+-rw-r--r--   0        0        0    17093 2023-03-26 00:13:37.346718 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/media_file_manager.data.json
+-rw-r--r--   0        0        0     2043 2023-03-26 00:13:37.347131 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/media_file_manager.meta.json
+-rw-r--r--   0        0        0    10898 2023-03-26 00:13:34.539053 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/media_file_storage.data.json
+-rw-r--r--   0        0        0     1770 2023-03-26 00:13:34.539564 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/media_file_storage.meta.json
+-rw-r--r--   0        0        0     8150 2023-03-26 00:13:37.436038 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/memory_session_storage.data.json
+-rw-r--r--   0        0        0     1838 2023-03-26 00:13:37.436984 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/memory_session_storage.meta.json
+-rw-r--r--   0        0        0    36631 2023-03-26 00:13:37.361370 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/metrics_util.data.json
+-rw-r--r--   0        0        0     2411 2023-03-26 00:13:37.361930 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/metrics_util.meta.json
+-rw-r--r--   0        0        0    77488 2023-03-26 00:13:37.473898 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/runtime.data.json
+-rw-r--r--   0        0        0     3195 2023-03-26 00:13:37.474283 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/runtime.meta.json
+-rw-r--r--   0        0        0     7560 2023-03-26 00:13:37.362673 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/runtime_util.data.json
+-rw-r--r--   0        0        0     2061 2023-03-26 00:13:37.363439 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/runtime_util.meta.json
+-rw-r--r--   0        0        0     7309 2023-03-26 00:13:34.537538 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/script_data.data.json
+-rw-r--r--   0        0        0     1814 2023-03-26 00:13:34.537921 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/script_data.meta.json
+-rw-r--r--   0        0        0     2995 2023-03-26 00:13:37.415328 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/scriptrunner/__init__.data.json
+-rw-r--r--   0        0        0     1896 2023-03-26 00:13:37.415570 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/scriptrunner/__init__.meta.json
+-rw-r--r--   0        0        0     4709 2023-03-26 00:13:34.816131 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/scriptrunner/magic.data.json
+-rw-r--r--   0        0        0     1898 2023-03-26 00:13:34.816601 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/scriptrunner/magic.meta.json
+-rw-r--r--   0        0        0    21983 2023-03-26 00:13:37.410985 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/scriptrunner/script_requests.data.json
+-rw-r--r--   0        0        0     1924 2023-03-26 00:13:37.411314 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/scriptrunner/script_requests.meta.json
+-rw-r--r--   0        0        0    27392 2023-03-26 00:13:37.411974 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/scriptrunner/script_run_context.data.json
+-rw-r--r--   0        0        0     4113 2023-03-26 00:13:37.412362 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/scriptrunner/script_run_context.meta.json
+-rw-r--r--   0        0        0    34061 2023-03-26 00:13:37.413129 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/scriptrunner/script_runner.data.json
+-rw-r--r--   0        0        0     4846 2023-03-26 00:13:37.413544 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/scriptrunner/script_runner.meta.json
+-rw-r--r--   0        0        0    32814 2023-03-26 00:13:37.395426 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/secrets.data.json
+-rw-r--r--   0        0        0     3996 2023-03-26 00:13:37.395975 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/secrets.meta.json
+-rw-r--r--   0        0        0    41402 2023-03-26 00:13:37.426412 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/session_manager.data.json
+-rw-r--r--   0        0        0     1977 2023-03-26 00:13:37.426935 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/session_manager.meta.json
+-rw-r--r--   0        0        0     3424 2023-03-26 00:13:37.409874 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/state/__init__.data.json
+-rw-r--r--   0        0        0     1948 2023-03-26 00:13:37.410309 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/state/__init__.meta.json
+-rw-r--r--   0        0        0    35149 2023-03-26 00:13:37.404119 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/state/common.data.json
+-rw-r--r--   0        0        0     2628 2023-03-26 00:13:37.404509 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/state/common.meta.json
+-rw-r--r--   0        0        0    16743 2023-03-26 00:13:37.408116 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/state/safe_session_state.data.json
+-rw-r--r--   0        0        0     1892 2023-03-26 00:13:37.408556 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/state/safe_session_state.meta.json
+-rw-r--r--   0        0        0    68877 2023-03-26 00:13:37.406818 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/state/session_state.data.json
+-rw-r--r--   0        0        0     4324 2023-03-26 00:13:37.407274 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/state/session_state.meta.json
+-rw-r--r--   0        0        0    16631 2023-03-26 00:13:37.409097 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/state/session_state_proxy.data.json
+-rw-r--r--   0        0        0     2281 2023-03-26 00:13:37.409450 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/state/session_state_proxy.meta.json
+-rw-r--r--   0        0        0    12465 2023-03-26 00:13:37.405151 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/state/widgets.data.json
+-rw-r--r--   0        0        0     2280 2023-03-26 00:13:37.405603 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/state/widgets.meta.json
+-rw-r--r--   0        0        0    25062 2023-03-26 00:13:34.878273 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/stats.data.json
+-rw-r--r--   0        0        0     1782 2023-03-26 00:13:34.878954 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/stats.meta.json
+-rw-r--r--   0        0        0    37701 2023-03-26 00:13:37.348080 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/uploaded_file_manager.data.json
+-rw-r--r--   0        0        0     2019 2023-03-26 00:13:37.348361 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/uploaded_file_manager.meta.json
+-rw-r--r--   0        0        0    15599 2023-03-26 00:13:37.434572 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/websocket_session_manager.data.json
+-rw-r--r--   0        0        0     2143 2023-03-26 00:13:37.435379 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/runtime/websocket_session_manager.meta.json
+-rw-r--r--   0        0        0     2462 2023-03-24 00:33:11.200361 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/scriptrunner/__init__.data.json
+-rw-r--r--   0        0        0     1646 2023-03-24 00:33:11.200611 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/scriptrunner/__init__.meta.json
+-rw-r--r--   0        0        0    28532 2023-03-24 00:33:11.198312 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/scriptrunner/script_requests.data.json
+-rw-r--r--   0        0        0     1730 2023-03-24 00:33:11.198540 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/scriptrunner/script_requests.meta.json
+-rw-r--r--   0        0        0    26413 2023-03-24 00:33:11.199038 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/scriptrunner/script_run_context.data.json
+-rw-r--r--   0        0        0     3732 2023-03-24 00:33:11.199282 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/scriptrunner/script_run_context.meta.json
+-rw-r--r--   0        0        0    32645 2023-03-24 00:33:11.199840 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/scriptrunner/script_runner.data.json
+-rw-r--r--   0        0        0     4156 2023-03-24 00:33:11.200115 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/scriptrunner/script_runner.meta.json
+-rw-r--r--   0        0        0    21735 2023-03-24 00:33:11.190414 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/secrets.data.json
+-rw-r--r--   0        0        0     3682 2023-03-24 00:33:11.190603 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/secrets.meta.json
+-rw-r--r--   0        0        0     1329 2023-03-24 00:33:08.330510 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/server/__init__.data.json
+-rw-r--r--   0        0        0     1485 2023-03-24 00:33:08.330745 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/server/__init__.meta.json
+-rw-r--r--   0        0        0    20265 2023-03-24 00:33:11.180646 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/server/routes.data.json
+-rw-r--r--   0        0        0     1995 2023-03-24 00:33:11.180899 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/server/routes.meta.json
+-rw-r--r--   0        0        0    49588 2023-03-24 00:33:11.237224 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/server/server.data.json
+-rw-r--r--   0        0        0     3456 2023-03-24 00:33:11.237625 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/server/server.meta.json
+-rw-r--r--   0        0        0    10330 2023-03-24 00:33:11.174487 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/server/server_util.data.json
+-rw-r--r--   0        0        0     1865 2023-03-24 00:33:11.174765 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/server/server_util.meta.json
+-rw-r--r--   0        0        0     8995 2023-03-24 00:33:11.231924 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/server/upload_file_request_handler.data.json
+-rw-r--r--   0        0        0     1916 2023-03-24 00:33:11.232397 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/server/upload_file_request_handler.meta.json
+-rw-r--r--   0        0        0    14813 2023-03-24 00:33:11.175978 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/session_data.data.json
+-rw-r--r--   0        0        0     1794 2023-03-24 00:33:11.176250 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/session_data.meta.json
+-rw-r--r--   0        0        0     9102 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/source_util.data.json
+-rw-r--r--   0        0        0     2058 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/source_util.meta.json
+-rw-r--r--   0        0        0     2887 2023-03-24 00:33:11.197493 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/state/__init__.data.json
+-rw-r--r--   0        0        0     1649 2023-03-24 00:33:11.197721 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/state/__init__.meta.json
+-rw-r--r--   0        0        0    13652 2023-03-24 00:33:11.191613 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/state/safe_session_state.data.json
+-rw-r--r--   0        0        0     1648 2023-03-24 00:33:11.191856 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/state/safe_session_state.meta.json
+-rw-r--r--   0        0        0   121394 2023-03-24 00:33:11.186461 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/state/session_state.data.json
+-rw-r--r--   0        0        0     3939 2023-03-24 00:33:11.186737 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/state/session_state.meta.json
+-rw-r--r--   0        0        0    12548 2023-03-24 00:33:11.196058 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/state/session_state_proxy.data.json
+-rw-r--r--   0        0        0     1858 2023-03-24 00:33:11.196305 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/state/session_state_proxy.meta.json
+-rw-r--r--   0        0        0    15052 2023-03-24 00:33:11.191001 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/state/widgets.data.json
+-rw-r--r--   0        0        0     2617 2023-03-24 00:33:11.191238 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/state/widgets.meta.json
+-rw-r--r--   0        0        0    28441 2023-03-24 00:33:11.155373 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/stats.data.json
+-rw-r--r--   0        0        0     1691 2023-03-24 00:33:11.155677 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/stats.meta.json
+-rw-r--r--   0        0        0    10753 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/string_util.data.json
+-rw-r--r--   0        0        0     1963 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/string_util.meta.json
+-rw-r--r--   0        0        0    79236 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/type_util.data.json
+-rw-r--r--   0        0        0     4219 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/type_util.meta.json
+-rw-r--r--   0        0        0    34194 2023-03-24 00:33:11.169034 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/uploaded_file_manager.data.json
+-rw-r--r--   0        0        0     1751 2023-03-24 00:33:11.169352 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/uploaded_file_manager.meta.json
+-rw-r--r--   0        0        0     3012 2023-03-24 00:33:10.296766 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/url_util.data.json
+-rw-r--r--   0        0        0     1622 2023-03-24 00:33:10.297013 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/url_util.meta.json
+-rw-r--r--   0        0        0     9557 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/user_info.data.json
+-rw-r--r--   0        0        0     1869 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/user_info.meta.json
+-rw-r--r--   0        0        0    12803 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/util.data.json
+-rw-r--r--   0        0        0     2021 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/util.meta.json
+-rw-r--r--   0        0        0     1728 2023-03-26 00:13:34.463357 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/vendor/__init__.data.json
+-rw-r--r--   0        0        0     1693 2023-03-26 00:13:34.463796 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/vendor/__init__.meta.json
+-rw-r--r--   0        0        0     1792 2023-03-26 00:13:34.464360 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/vendor/ipython/__init__.data.json
+-rw-r--r--   0        0        0     1709 2023-03-26 00:13:34.464728 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/vendor/ipython/__init__.meta.json
+-rw-r--r--   0        0        0     5474 2023-03-26 00:13:37.345826 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/vendor/ipython/modified_sys_path.data.json
+-rw-r--r--   0        0        0     1801 2023-03-26 00:13:37.346158 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/vendor/ipython/modified_sys_path.meta.json
+-rw-r--r--   0        0        0     5468 2023-03-26 00:13:37.350918 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/version.data.json
+-rw-r--r--   0        0        0     1899 2023-03-26 00:13:37.351172 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/version.meta.json
+-rw-r--r--   0        0        0     2273 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/watcher/__init__.data.json
+-rw-r--r--   0        0        0     1788 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/watcher/__init__.meta.json
+-rw-r--r--   0        0        0    34028 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/watcher/event_based_path_watcher.data.json
+-rw-r--r--   0        0        0     2074 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/watcher/event_based_path_watcher.meta.json
+-rw-r--r--   0        0        0    34345 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/watcher/local_sources_watcher.data.json
+-rw-r--r--   0        0        0     2252 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/watcher/local_sources_watcher.meta.json
+-rw-r--r--   0        0        0    11709 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/watcher/path_watcher.data.json
+-rw-r--r--   0        0        0     2010 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/watcher/path_watcher.meta.json
+-rw-r--r--   0        0        0    12311 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/watcher/polling_path_watcher.data.json
+-rw-r--r--   0        0        0     2017 2023-03-26 00:13:37.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/watcher/polling_path_watcher.meta.json
+-rw-r--r--   0        0        0     6346 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/watcher/util.data.json
+-rw-r--r--   0        0        0     1892 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/streamlit/watcher/util.meta.json
+-rw-r--r--   0        0        0    28943 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/string.data.json
+-rw-r--r--   0        0        0     1800 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/string.meta.json
+-rw-r--r--   0        0        0    16772 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/struct.data.json
+-rw-r--r--   0        0        0     1797 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/struct.meta.json
+-rw-r--r--   0        0        0   173211 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/subprocess.data.json
+-rw-r--r--   0        0        0     1875 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/subprocess.meta.json
+-rw-r--r--   0        0        0   152188 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/sys.data.json
+-rw-r--r--   0        0        0     1854 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/sys.meta.json
+-rw-r--r--   0        0        0   130362 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tempfile.data.json
+-rw-r--r--   0        0        0     1819 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tempfile.meta.json
+-rw-r--r--   0        0        0    51912 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/termios.data.json
+-rw-r--r--   0        0        0     1750 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/termios.meta.json
+-rw-r--r--   0        0        0    21203 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/textwrap.data.json
+-rw-r--r--   0        0        0     1730 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/textwrap.meta.json
+-rw-r--r--   0        0        0    70566 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/threading.data.json
+-rw-r--r--   0        0        0     1785 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/threading.meta.json
+-rw-r--r--   0        0        0    46632 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/time.data.json
+-rw-r--r--   0        0        0     1744 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/time.meta.json
+-rw-r--r--   0        0        0    13162 2023-03-26 00:13:34.667375 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/timeit.data.json
+-rw-r--r--   0        0        0     1740 2023-03-26 00:13:34.667708 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/timeit.meta.json
+-rw-r--r--   0        0        0    16375 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/token.data.json
+-rw-r--r--   0        0        0     1721 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/token.meta.json
+-rw-r--r--   0        0        0    53728 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tokenize.data.json
+-rw-r--r--   0        0        0     1804 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tokenize.meta.json
+-rw-r--r--   0        0        0     1954 2023-03-24 00:33:08.349397 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/__init__.data.json
+-rw-r--r--   0        0        0     1499 2023-03-24 00:33:08.349676 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/__init__.meta.json
+-rw-r--r--   0        0        0     1465 2023-03-24 00:33:08.236672 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/_locale_data.data.json
+-rw-r--r--   0        0        0     1516 2023-03-24 00:33:08.236854 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/_locale_data.meta.json
+-rw-r--r--   0        0        0    10429 2023-03-24 00:33:10.587668 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/autoreload.data.json
+-rw-r--r--   0        0        0     1965 2023-03-24 00:33:10.588033 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/autoreload.meta.json
+-rw-r--r--   0        0        0    24381 2023-03-24 00:33:10.548472 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/concurrent.data.json
+-rw-r--r--   0        0        0     1811 2023-03-24 00:33:10.548777 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/concurrent.meta.json
+-rw-r--r--   0        0        0    28919 2023-03-24 00:33:10.319187 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/escape.data.json
+-rw-r--r--   0        0        0     1793 2023-03-24 00:33:10.319467 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/escape.meta.json
+-rw-r--r--   0        0        0    53776 2023-03-24 00:33:10.551047 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/gen.data.json
+-rw-r--r--   0        0        0     2037 2023-03-24 00:33:10.551230 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/gen.meta.json
+-rw-r--r--   0        0        0    49762 2023-03-24 00:33:10.573685 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/http1connection.data.json
+-rw-r--r--   0        0        0     2107 2023-03-24 00:33:10.574016 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/http1connection.meta.json
+-rw-r--r--   0        0        0    59349 2023-03-24 00:33:10.624283 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/httpclient.data.json
+-rw-r--r--   0        0        0     2129 2023-03-24 00:33:10.624687 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/httpclient.meta.json
+-rw-r--r--   0        0        0    34361 2023-03-24 00:33:10.630821 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/httpserver.data.json
+-rw-r--r--   0        0        0     1855 2023-03-24 00:33:10.631150 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/httpserver.meta.json
+-rw-r--r--   0        0        0   106247 2023-03-24 00:33:10.463357 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/httputil.data.json
+-rw-r--r--   0        0        0     2122 2023-03-24 00:33:10.463652 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/httputil.meta.json
+-rw-r--r--   0        0        0    61006 2023-03-24 00:33:10.549929 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/ioloop.data.json
+-rw-r--r--   0        0        0     2182 2023-03-24 00:33:10.550179 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/ioloop.meta.json
+-rw-r--r--   0        0        0    72931 2023-03-24 00:33:10.553182 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/iostream.data.json
+-rw-r--r--   0        0        0     2237 2023-03-24 00:33:10.553412 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/iostream.meta.json
+-rw-r--r--   0        0        0    24382 2023-03-24 00:33:10.444086 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/locale.data.json
+-rw-r--r--   0        0        0     1855 2023-03-24 00:33:10.444396 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/locale.meta.json
+-rw-r--r--   0        0        0    33199 2023-03-24 00:33:10.593650 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/locks.data.json
+-rw-r--r--   0        0        0     1859 2023-03-24 00:33:10.594000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/locks.meta.json
+-rw-r--r--   0        0        0     9113 2023-03-24 00:33:10.380448 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/log.data.json
+-rw-r--r--   0        0        0     1834 2023-03-24 00:33:10.380730 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/log.meta.json
+-rw-r--r--   0        0        0    30772 2023-03-24 00:33:10.551805 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/netutil.data.json
+-rw-r--r--   0        0        0     1915 2023-03-24 00:33:10.552049 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/netutil.meta.json
+-rw-r--r--   0        0        0    38708 2023-03-24 00:33:10.381446 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/options.data.json
+-rw-r--r--   0        0        0     1804 2023-03-24 00:33:10.381656 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/options.meta.json
+-rw-r--r--   0        0        0     1329 2023-03-24 00:33:08.293522 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/platform/__init__.data.json
+-rw-r--r--   0        0        0     1483 2023-03-24 00:33:08.293705 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/platform/__init__.meta.json
+-rw-r--r--   0        0        0    50976 2023-03-24 00:33:10.554192 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/platform/asyncio.data.json
+-rw-r--r--   0        0        0     2053 2023-03-24 00:33:10.554376 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/platform/asyncio.meta.json
+-rw-r--r--   0        0        0    18440 2023-03-24 00:33:10.554801 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/process.data.json
+-rw-r--r--   0        0        0     2080 2023-03-24 00:33:10.555045 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/process.meta.json
+-rw-r--r--   0        0        0    35458 2023-03-24 00:33:10.599406 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/queues.data.json
+-rw-r--r--   0        0        0     1913 2023-03-24 00:33:10.599665 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/queues.meta.json
+-rw-r--r--   0        0        0    53735 2023-03-24 00:33:10.643375 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/routing.data.json
+-rw-r--r--   0        0        0     1864 2023-03-24 00:33:10.643867 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/routing.meta.json
+-rw-r--r--   0        0        0    46153 2023-03-24 00:33:10.625460 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/simple_httpclient.data.json
+-rw-r--r--   0        0        0     2323 2023-03-24 00:33:10.625763 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/simple_httpclient.meta.json
+-rw-r--r--   0        0        0    27644 2023-03-24 00:33:10.581631 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/tcpclient.data.json
+-rw-r--r--   0        0        0     2026 2023-03-24 00:33:10.581934 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/tcpclient.meta.json
+-rw-r--r--   0        0        0    13544 2023-03-24 00:33:10.558702 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/tcpserver.data.json
+-rw-r--r--   0        0        0     2010 2023-03-24 00:33:10.558953 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/tcpserver.meta.json
+-rw-r--r--   0        0        0    80175 2023-03-24 00:33:10.430612 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/template.data.json
+-rw-r--r--   0        0        0     1867 2023-03-24 00:33:10.430920 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/template.meta.json
+-rw-r--r--   0        0        0    39039 2023-03-24 00:33:10.305088 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/util.data.json
+-rw-r--r--   0        0        0     1818 2023-03-24 00:33:10.305375 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/util.meta.json
+-rw-r--r--   0        0        0   207670 2023-03-24 00:33:10.709553 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/web.data.json
+-rw-r--r--   0        0        0     2681 2023-03-24 00:33:10.709881 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/web.meta.json
+-rw-r--r--   0        0        0   127545 2023-03-24 00:33:10.732419 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/websocket.data.json
+-rw-r--r--   0        0        0     2474 2023-03-24 00:33:10.732776 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tornado/websocket.meta.json
+-rw-r--r--   0        0        0    56300 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/traceback.data.json
+-rw-r--r--   0        0        0     1794 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/traceback.meta.json
+-rw-r--r--   0        0        0     5335 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tty.data.json
+-rw-r--r--   0        0        0     1722 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/tty.meta.json
+-rw-r--r--   0        0        0   248545 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/types.data.json
+-rw-r--r--   0        0        0     1826 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/types.meta.json
+-rw-r--r--   0        0        0   444990 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/typing.data.json
+-rw-r--r--   0        0        0     1892 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/typing.meta.json
+-rw-r--r--   0        0        0    73993 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/typing_extensions.data.json
+-rw-r--r--   0        0        0     1816 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/typing_extensions.meta.json
+-rw-r--r--   0        0        0    46042 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/unicodedata.data.json
+-rw-r--r--   0        0        0     1758 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/unicodedata.meta.json
+-rw-r--r--   0        0        0     6507 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/unittest/__init__.data.json
+-rw-r--r--   0        0        0     1943 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/unittest/__init__.meta.json
+-rw-r--r--   0        0        0    26183 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/unittest/_log.data.json
+-rw-r--r--   0        0        0     1791 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/unittest/_log.meta.json
+-rw-r--r--   0        0        0     8318 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/unittest/async_case.data.json
+-rw-r--r--   0        0        0     1822 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/unittest/async_case.meta.json
+-rw-r--r--   0        0        0   225925 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/unittest/case.data.json
+-rw-r--r--   0        0        0     1942 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/unittest/case.meta.json
+-rw-r--r--   0        0        0    15918 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/unittest/loader.data.json
+-rw-r--r--   0        0        0     1853 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/unittest/loader.meta.json
+-rw-r--r--   0        0        0    12791 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/unittest/main.data.json
+-rw-r--r--   0        0        0     1862 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/unittest/main.meta.json
+-rw-r--r--   0        0        0   162909 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/unittest/mock.data.json
+-rw-r--r--   0        0        0     1824 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/unittest/mock.meta.json
+-rw-r--r--   0        0        0    22446 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/unittest/result.data.json
+-rw-r--r--   0        0        0     1809 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/unittest/result.meta.json
+-rw-r--r--   0        0        0    11707 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/unittest/runner.data.json
+-rw-r--r--   0        0        0     1852 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/unittest/runner.meta.json
+-rw-r--r--   0        0        0    12369 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/unittest/signals.data.json
+-rw-r--r--   0        0        0     1804 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/unittest/signals.meta.json
+-rw-r--r--   0        0        0    12262 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/unittest/suite.data.json
+-rw-r--r--   0        0        0     1825 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/unittest/suite.meta.json
+-rw-r--r--   0        0        0     1669 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/urllib/__init__.data.json
+-rw-r--r--   0        0        0     1695 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/urllib/__init__.meta.json
+-rw-r--r--   0        0        0   166627 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/urllib/parse.data.json
+-rw-r--r--   0        0        0     1801 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/urllib/parse.meta.json
+-rw-r--r--   0        0        0    36729 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/uuid.data.json
+-rw-r--r--   0        0        0     1824 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/uuid.meta.json
+-rw-r--r--   0        0        0    24197 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/warnings.data.json
+-rw-r--r--   0        0        0     1812 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/warnings.meta.json
+-rw-r--r--   0        0        0     1664 2023-03-26 00:13:34.521808 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/watchdog/__init__.data.json
+-rw-r--r--   0        0        0     1679 2023-03-26 00:13:34.522180 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/watchdog/__init__.meta.json
+-rw-r--r--   0        0        0    46367 2023-03-26 00:13:34.997032 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/watchdog/events.data.json
+-rw-r--r--   0        0        0     1929 2023-03-26 00:13:34.997400 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/watchdog/events.meta.json
+-rw-r--r--   0        0        0     3080 2023-03-26 00:13:36.411419 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/watchdog/observers/__init__.data.json
+-rw-r--r--   0        0        0     1973 2023-03-26 00:13:36.412251 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/watchdog/observers/__init__.meta.json
+-rw-r--r--   0        0        0    30099 2023-03-26 00:13:35.052601 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/watchdog/observers/api.data.json
+-rw-r--r--   0        0        0     1928 2023-03-26 00:13:35.053337 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/watchdog/observers/api.meta.json
+-rw-r--r--   0        0        0    15395 2023-03-26 00:13:35.249745 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/watchdog/observers/fsevents.data.json
+-rw-r--r--   0        0        0     2102 2023-03-26 00:13:35.250108 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/watchdog/observers/fsevents.meta.json
+-rw-r--r--   0        0        0    31402 2023-03-26 00:13:35.254307 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/watchdog/observers/kqueue.data.json
+-rw-r--r--   0        0        0     2025 2023-03-26 00:13:35.254861 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/watchdog/observers/kqueue.meta.json
+-rw-r--r--   0        0        0     9060 2023-03-26 00:13:35.256351 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/watchdog/observers/polling.data.json
+-rw-r--r--   0        0        0     1945 2023-03-26 00:13:35.256796 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/watchdog/observers/polling.meta.json
+-rw-r--r--   0        0        0     8256 2023-03-26 00:13:34.799645 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/watchdog/utils/__init__.data.json
+-rw-r--r--   0        0        0     1765 2023-03-26 00:13:34.799912 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/watchdog/utils/__init__.meta.json
+-rw-r--r--   0        0        0     3828 2023-03-26 00:13:34.985625 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/watchdog/utils/bricks.data.json
+-rw-r--r--   0        0        0     1735 2023-03-26 00:13:34.986057 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/watchdog/utils/bricks.meta.json
+-rw-r--r--   0        0        0    25330 2023-03-26 00:13:34.963896 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/watchdog/utils/dirsnapshot.data.json
+-rw-r--r--   0        0        0     1897 2023-03-26 00:13:34.964347 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/watchdog/utils/dirsnapshot.meta.json
+-rw-r--r--   0        0        0     2944 2023-03-26 00:13:34.795141 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/watchdog/utils/patterns.data.json
+-rw-r--r--   0        0        0     1752 2023-03-26 00:13:34.795405 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/watchdog/utils/patterns.meta.json
+-rw-r--r--   0        0        0     4705 2023-03-26 00:13:34.730814 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/watchdog/utils/platform.data.json
+-rw-r--r--   0        0        0     1737 2023-03-26 00:13:34.731189 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/watchdog/utils/platform.meta.json
+-rw-r--r--   0        0        0    58616 2023-03-26 00:13:34.556028 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/wave.data.json
+-rw-r--r--   0        0        0     1809 2023-03-26 00:13:34.556412 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/wave.meta.json
+-rw-r--r--   0        0        0   156352 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/weakref.data.json
+-rw-r--r--   0        0        0     1818 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/weakref.meta.json
+-rw-r--r--   0        0        0    30313 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/webbrowser.data.json
+-rw-r--r--   0        0        0     1782 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/webbrowser.meta.json
+-rw-r--r--   0        0        0    75700 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/zipfile.data.json
+-rw-r--r--   0        0        0     1880 2023-03-26 00:13:29.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/zipfile.meta.json
+-rw-r--r--   0        0        0    18708 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/zlib.data.json
+-rw-r--r--   0        0        0     1829 2023-03-26 00:13:34.000000 cupid_matching-1.0.7/cupid_matching/.mypy_cache/3.10/zlib.meta.json
+-rw-r--r--   0        0        0      190 2023-03-24 00:10:22.896312 cupid_matching-1.0.7/cupid_matching/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       37 2023-04-01 14:40:13.598825 cupid_matching-1.0.7/cupid_matching/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2023-04-01 14:40:13.598920 cupid_matching-1.0.7/cupid_matching/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2023-04-01 14:40:13.598719 cupid_matching-1.0.7/cupid_matching/.pytest_cache/README.md
+-rw-r--r--   0        0        0       68 2023-04-01 14:40:13.599181 cupid_matching-1.0.7/cupid_matching/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0       56 2023-04-01 14:40:35.466759 cupid_matching-1.0.7/cupid_matching/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2023-04-01 14:40:35.467039 cupid_matching-1.0.7/cupid_matching/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        1 2023-04-02 19:21:40.197779 cupid_matching-1.0.7/cupid_matching/__init__.py
+-rw-r--r--   0        0        0     9400 2023-04-13 19:06:23.097168 cupid_matching-1.0.7/cupid_matching/choo_siow.py
+-rw-r--r--   0        0        0     5656 2023-04-02 13:02:37.271948 cupid_matching-1.0.7/cupid_matching/choo_siow_gender_heteroskedastic.py
+-rw-r--r--   0        0        0     6283 2023-04-02 19:11:25.395323 cupid_matching-1.0.7/cupid_matching/choo_siow_heteroskedastic.py
+-rw-r--r--   0        0        0    14162 2023-04-02 13:02:37.272889 cupid_matching-1.0.7/cupid_matching/cupid_streamlit.py
+-rw-r--r--   0        0        0       51 2023-03-24 00:22:09.620449 cupid_matching-1.0.7/cupid_matching/docs/choo_siow.md
+-rw-r--r--   0        0        0       97 2023-03-24 00:21:48.848158 cupid_matching-1.0.7/cupid_matching/docs/choo_siow_gender_heteroskedastic.md
+-rw-r--r--   0        0        0       83 2023-03-24 00:22:03.727712 cupid_matching-1.0.7/cupid_matching/docs/choo_siow_heteroskedastic.md
+-rw-r--r--   0        0        0      285 2023-03-24 00:22:15.196968 cupid_matching-1.0.7/cupid_matching/docs/cupid_streamlit.md
+-rw-r--r--   0        0        0       46 2023-03-24 00:22:19.670499 cupid_matching-1.0.7/cupid_matching/docs/entropy.md
+-rw-r--r--   0        0        0       63 2023-04-02 13:02:37.273230 cupid_matching-1.0.7/cupid_matching/docs/example_choosiow.md
+-rw-r--r--   0        0        0       69 2023-04-02 13:02:37.273547 cupid_matching-1.0.7/cupid_matching/docs/example_nestedlogit.md
+-rw-r--r--   0        0        0     2321 2023-04-13 19:10:29.782351 cupid_matching-1.0.7/cupid_matching/docs/index.md
+-rw-r--r--   0        0        0       57 2023-03-24 00:22:52.962261 cupid_matching-1.0.7/cupid_matching/docs/ipfp_solvers.md
+-rw-r--r--   0        0        0       61 2023-03-24 00:22:57.157065 cupid_matching-1.0.7/cupid_matching/docs/matching_utils.md
+-rw-r--r--   0        0        0       57 2023-03-24 00:23:07.925133 cupid_matching-1.0.7/cupid_matching/docs/min_distance.md
+-rw-r--r--   0        0        0       69 2023-03-24 00:23:01.182377 cupid_matching-1.0.7/cupid_matching/docs/min_distance_utils.md
+-rw-r--r--   0        0        0       59 2023-03-24 00:27:46.673143 cupid_matching-1.0.7/cupid_matching/docs/model_classes.md
+-rw-r--r--   0        0        0       58 2023-03-24 00:23:19.684703 cupid_matching-1.0.7/cupid_matching/docs/nested_logit.md
+-rw-r--r--   0        0        0       55 2023-03-24 00:27:33.384226 cupid_matching-1.0.7/cupid_matching/docs/poisson_glm.md
+-rw-r--r--   0        0        0       67 2023-03-24 00:27:42.792605 cupid_matching-1.0.7/cupid_matching/docs/poisson_glm_utils.md
+-rw-r--r--   0        0        0       43 2023-03-24 00:27:23.096924 cupid_matching-1.0.7/cupid_matching/docs/utils.md
+-rw-r--r--   0        0        0    11551 2023-04-02 19:15:11.050530 cupid_matching-1.0.7/cupid_matching/entropy.py
+-rw-r--r--   0        0        0     3531 2023-04-13 19:09:36.869069 cupid_matching-1.0.7/cupid_matching/example_choosiow.py
+-rw-r--r--   0        0        0     4133 2023-04-02 19:13:08.597638 cupid_matching-1.0.7/cupid_matching/example_nestedlogit.py
+-rw-r--r--   0        0        0    26548 2023-04-02 19:13:28.516760 cupid_matching-1.0.7/cupid_matching/ipfp_solvers.py
+-rw-r--r--   0        0        0     8744 2023-04-13 19:02:11.316261 cupid_matching-1.0.7/cupid_matching/matching_utils.py
+-rw-r--r--   0        0        0    11551 2023-04-02 19:13:54.856938 cupid_matching-1.0.7/cupid_matching/min_distance.py
+-rw-r--r--   0        0        0     5260 2023-04-02 19:13:40.696373 cupid_matching-1.0.7/cupid_matching/min_distance_utils.py
+-rw-r--r--   0        0        0     1873 2023-04-02 13:02:37.291292 cupid_matching-1.0.7/cupid_matching/mkdocs.yml
+-rw-r--r--   0        0        0    16277 2023-04-02 19:15:11.063645 cupid_matching-1.0.7/cupid_matching/model_classes.py
+-rw-r--r--   0        0        0      369 2023-04-02 19:14:11.059995 cupid_matching-1.0.7/cupid_matching/mypy.ini
+-rw-r--r--   0        0        0     9515 2023-04-02 19:15:11.064847 cupid_matching-1.0.7/cupid_matching/nested_logit.py
+-rw-r--r--   0        0        0     7401 2023-04-02 19:15:11.067470 cupid_matching-1.0.7/cupid_matching/poisson_glm.py
+-rw-r--r--   0        0        0     6544 2023-04-02 19:14:50.571051 cupid_matching-1.0.7/cupid_matching/poisson_glm_utils.py
+-rw-r--r--   0        0        0    17888 2023-04-13 17:38:40.800414 cupid_matching-1.0.7/cupid_matching/site/404.html
+-rw-r--r--   0        0        0      704 2023-04-13 17:38:40.738846 cupid_matching-1.0.7/cupid_matching/site/assets/_mkdocstrings.css
+-rw-r--r--   0        0        0     1870 2023-04-13 17:38:40.739462 cupid_matching-1.0.7/cupid_matching/site/assets/images/favicon.png
+-rw-r--r--   0        0        0   113254 2023-04-13 17:38:40.739717 cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/bundle.407015b8.min.js
+-rw-r--r--   0        0        0   950772 2023-04-13 17:38:40.740168 cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/bundle.407015b8.min.js.map
+-rw-r--r--   0        0        0    17074 2023-04-13 17:38:40.740488 cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.ar.min.js
+-rw-r--r--   0        0        0     4654 2023-04-13 17:38:40.740717 cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.da.min.js
+-rw-r--r--   0        0        0     6119 2023-04-13 17:38:40.740985 cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.de.min.js
+-rw-r--r--   0        0        0     6208 2023-04-13 17:38:40.741223 cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.du.min.js
+-rw-r--r--   0        0        0    11499 2023-04-13 17:38:40.741554 cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.es.min.js
+-rw-r--r--   0        0        0     9342 2023-04-13 17:38:40.741847 cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.fi.min.js
+-rw-r--r--   0        0        0    10669 2023-04-13 17:38:40.742074 cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.fr.min.js
+-rw-r--r--   0        0        0     3383 2023-04-13 17:38:40.742279 cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.hi.min.js
+-rw-r--r--   0        0        0     9437 2023-04-13 17:38:40.742506 cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.hu.min.js
+-rw-r--r--   0        0        0    11232 2023-04-13 17:38:40.742925 cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.it.min.js
+-rw-r--r--   0        0        0     2313 2023-04-13 17:38:40.743163 cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.ja.min.js
+-rw-r--r--   0        0        0       36 2023-04-13 17:38:40.743404 cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.jp.min.js
+-rw-r--r--   0        0        0     7973 2023-04-13 17:38:40.743615 cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.ko.min.js
+-rw-r--r--   0        0        0      817 2023-04-13 17:38:40.744047 cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.multi.min.js
+-rw-r--r--   0        0        0     6026 2023-04-13 17:38:40.744350 cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.nl.min.js
+-rw-r--r--   0        0        0     4754 2023-04-13 17:38:40.744583 cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.no.min.js
+-rw-r--r--   0        0        0    10171 2023-04-13 17:38:40.744799 cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.pt.min.js
+-rw-r--r--   0        0        0    10958 2023-04-13 17:38:40.744965 cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.ro.min.js
+-rw-r--r--   0        0        0    10331 2023-04-13 17:38:40.745144 cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.ru.min.js
+-rw-r--r--   0        0        0     3647 2023-04-13 17:38:40.745369 cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
+-rw-r--r--   0        0        0     4523 2023-04-13 17:38:40.745556 cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.sv.min.js
+-rw-r--r--   0        0        0     2406 2023-04-13 17:38:40.745733 cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.ta.min.js
+-rw-r--r--   0        0        0     1031 2023-04-13 17:38:40.745896 cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.th.min.js
+-rw-r--r--   0        0        0    15009 2023-04-13 17:38:40.746294 cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.tr.min.js
+-rw-r--r--   0        0        0      784 2023-04-13 17:38:40.746526 cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.vi.min.js
+-rw-r--r--   0        0        0     2062 2023-04-13 17:38:40.746713 cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.zh.min.js
+-rw-r--r--   0        0        0    22878 2023-04-13 17:38:40.746964 cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/tinyseg.js
+-rw-r--r--   0        0        0   677455 2023-04-13 17:38:40.747315 cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/wordcut.js
+-rw-r--r--   0        0        0    38916 2023-04-13 17:38:40.747560 cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/workers/search.208ed371.min.js
+-rw-r--r--   0        0        0   209901 2023-04-13 17:38:40.747802 cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/workers/search.208ed371.min.js.map
+-rw-r--r--   0        0        0   113417 2023-04-13 17:38:40.748064 cupid_matching-1.0.7/cupid_matching/site/assets/stylesheets/main.7a7fce14.min.css
+-rw-r--r--   0        0        0    38957 2023-04-13 17:38:40.748263 cupid_matching-1.0.7/cupid_matching/site/assets/stylesheets/main.7a7fce14.min.css.map
+-rw-r--r--   0        0        0    12355 2023-04-13 17:38:40.748441 cupid_matching-1.0.7/cupid_matching/site/assets/stylesheets/palette.a0c5b2b5.min.css
+-rw-r--r--   0        0        0     3646 2023-04-13 17:38:40.748643 cupid_matching-1.0.7/cupid_matching/site/assets/stylesheets/palette.a0c5b2b5.min.css.map
+-rw-r--r--   0        0        0    56388 2023-04-13 17:38:40.822437 cupid_matching-1.0.7/cupid_matching/site/choo_siow/index.html
+-rw-r--r--   0        0        0    61309 2023-04-13 17:38:40.836416 cupid_matching-1.0.7/cupid_matching/site/choo_siow_gender_heteroskedastic/index.html
+-rw-r--r--   0        0        0    67113 2023-04-13 17:38:40.853319 cupid_matching-1.0.7/cupid_matching/site/choo_siow_heteroskedastic/index.html
+-rw-r--r--   0        0        0    19453 2023-04-13 17:38:40.854153 cupid_matching-1.0.7/cupid_matching/site/cupid_streamlit/index.html
+-rw-r--r--   0        0        0    52734 2023-04-13 17:38:40.863760 cupid_matching-1.0.7/cupid_matching/site/entropy/index.html
+-rw-r--r--   0        0        0    33047 2023-04-13 17:38:40.868763 cupid_matching-1.0.7/cupid_matching/site/example_choosiow/index.html
+-rw-r--r--   0        0        0    40108 2023-04-13 17:38:40.876280 cupid_matching-1.0.7/cupid_matching/site/example_nestedlogit/index.html
+-rw-r--r--   0        0        0    24691 2023-04-13 17:38:40.809070 cupid_matching-1.0.7/cupid_matching/site/index.html
+-rw-r--r--   0        0        0   171028 2023-04-13 17:38:40.932202 cupid_matching-1.0.7/cupid_matching/site/ipfp_solvers/index.html
+-rw-r--r--   0        0        0    33535 2023-04-13 17:38:40.937827 cupid_matching-1.0.7/cupid_matching/site/matching_utils/index.html
+-rw-r--r--   0        0        0    73534 2023-04-13 17:38:40.958010 cupid_matching-1.0.7/cupid_matching/site/min_distance/index.html
+-rw-r--r--   0        0        0    48540 2023-04-13 17:38:40.969561 cupid_matching-1.0.7/cupid_matching/site/min_distance_utils/index.html
+-rw-r--r--   0        0        0   158026 2023-04-13 17:38:41.025442 cupid_matching-1.0.7/cupid_matching/site/model_classes/index.html
+-rw-r--r--   0        0        0    80301 2023-04-13 17:38:41.047356 cupid_matching-1.0.7/cupid_matching/site/nested_logit/index.html
+-rw-r--r--   0        0        0      864 2023-04-13 17:38:40.739163 cupid_matching-1.0.7/cupid_matching/site/objects.inv
+-rw-r--r--   0        0        0    70696 2023-04-13 17:38:41.068101 cupid_matching-1.0.7/cupid_matching/site/poisson_glm/index.html
+-rw-r--r--   0        0        0    52629 2023-04-13 17:38:41.080736 cupid_matching-1.0.7/cupid_matching/site/poisson_glm_utils/index.html
+-rw-r--r--   0        0        0   180005 2023-04-13 17:38:41.116311 cupid_matching-1.0.7/cupid_matching/site/search/search_index.json
+-rw-r--r--   0        0        0     3235 2023-04-13 17:38:40.750319 cupid_matching-1.0.7/cupid_matching/site/sitemap.xml
+-rw-r--r--   0        0        0      354 2023-04-13 17:38:40.750481 cupid_matching-1.0.7/cupid_matching/site/sitemap.xml.gz
+-rw-r--r--   0        0        0   120234 2023-04-13 17:38:41.115705 cupid_matching-1.0.7/cupid_matching/site/utils/index.html
+-rw-r--r--   0        0        0    12373 2023-04-02 19:15:05.244218 cupid_matching-1.0.7/cupid_matching/utils.py
+-rw-r--r--   0        0        0      969 2023-04-13 19:09:51.820794 cupid_matching-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3064 1970-01-01 00:00:00.000000 cupid_matching-1.0.7/PKG-INFO
```

### Comparing `cupid_matching-1.0.5/README.md` & `cupid_matching-1.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -39,7 +39,13 @@
 ## Release notes
 ### version 1.0.4
 * added an optional bias-correction for the minimum distance estimator in the Choo and Siow homoskedastic model, to help with cases when the matching patterns vary a lot across cells.
 * added two complete examples: [example_choosiow.py](example_choosiow.md) and [example_nestedlogit.py](example_nestedlogit.md).
 
 ### version 1,0.5
 * simplified the bias-correction for the minimum distance estimator in the Choo and Siow homoskedastic model.
+
+### version 1.0.6
+* corrected typo.
+
+### version 1.0.7
+* fixed error in bias-correction term.
```

### Comparing `cupid_matching-1.0.5/cupid_matching/.idea/cupid_matching.iml` & `cupid_matching-1.0.7/cupid_matching/.idea/cupid_matching.iml`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/.idea/inspectionProfiles/Project_Default.xml` & `cupid_matching-1.0.7/cupid_matching/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/choo_siow.py` & `cupid_matching-1.0.7/cupid_matching/choo_siow.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     Returns:
         the (X,Y) matrix of the first derivative of the entropy
         if hessian is True, the (X,Y,X,Y) array of the second derivative
             wrt $(\\mu,\\mu)$
           and the (X,Y,X+Y) second derivatives
             wrt $(\\mu,(n,m))$
     """
-    muxy, mux0, mu0y, n, m = muhat.unpack()
+    muxy, mux0, mu0y, *_ = muhat.unpack()
     n_households = np.sum(muxy) + np.sum(mux0) + np.sum(mu0y)
 
     muxy_corr = muxy + (1.0-muxy/n_households)/2.0
     logxy = np.log(muxy_corr)
     mux0_corr = mux0 + (1.0-mux0/n_households)/2.0
     logx0 = np.log(mux0_corr)
     mu0y_corr = mu0y + (1.0-mu0y/n_households)/2.0
@@ -120,14 +120,15 @@
     der_xy = -2.0 * logxy + log0y
     der_xy += logx0.reshape((-1, 1))
     if not hessian:
         return der_xy
     else:  # we compute the Hessians
         X, Y = muxy.shape
         f_corr = 1.0-1.0/n_households/2.0
+        print(f"{f_corr=}")
         derlogxy = f_corr / muxy_corr
         derlogx0 = f_corr / mux0_corr
         derlog0y = f_corr / mu0y_corr
         der2_xyzt = np.zeros((X, Y, X, Y))
         der2_xyr = np.zeros((X, Y, X + Y))
         for x in range(X):
             dlogx0 = derlogx0[x]
```

### Comparing `cupid_matching-1.0.5/cupid_matching/choo_siow_gender_heteroskedastic.py` & `cupid_matching-1.0.7/cupid_matching/choo_siow_gender_heteroskedastic.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/choo_siow_heteroskedastic.py` & `cupid_matching-1.0.7/cupid_matching/choo_siow_heteroskedastic.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/cupid_streamlit.py` & `cupid_matching-1.0.7/cupid_matching/cupid_streamlit.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/docs/index.md` & `cupid_matching-1.0.7/cupid_matching/docs/index.md`

 * *Files 8% similar despite different names*

```diff
@@ -39,7 +39,13 @@
 ## Release notes
 ### version 1.0.4
 * added an optional bias-correction for the minimum distance estimator in the Choo and Siow homoskedastic model, to help with cases when the matching patterns vary a lot across cells.
 * added two complete examples: [example_choosiow.py](example_choosiow.md) and [example_nestedlogit.py](example_nestedlogit.md).
 
 ### version 1,0.5
 * simplified the bias-correction for the minimum distance estimator in the Choo and Siow homoskedastic model.
+
+### version 1.0.6
+* corrected typo.
+
+### version 1.0.7
+* fixed error in bias-correction term.
```

### Comparing `cupid_matching-1.0.5/cupid_matching/entropy.py` & `cupid_matching-1.0.7/cupid_matching/entropy.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/example_choosiow.py` & `cupid_matching-1.0.7/cupid_matching/example_choosiow.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,16 +65,17 @@
     """
     print_stars(f"    {title}")
     mde_results = estimate_semilinear_mde(mus_sim, phi_bases, entropy)
     mde_discrepancy = mde_results.print_results(true_coeffs=betas_true)
     return mde_discrepancy
 
 
+n_households = 100_000
 choo_siow_instance, phi_bases, betas_true = create_choosiow_population(10, 8, 5)
-mus_sim = choo_siow_instance.simulate(1e5)
+mus_sim = choo_siow_instance.simulate(n_households)
 
 # we estimate using forur variants of the minimum distance estimator
 mde_discrepancy = mde_estimate(
     mus_sim,
     phi_bases,
     betas_true,
     entropy_choo_siow,
```

### Comparing `cupid_matching-1.0.5/cupid_matching/example_nestedlogit.py` & `cupid_matching-1.0.7/cupid_matching/example_nestedlogit.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/ipfp_solvers.py` & `cupid_matching-1.0.7/cupid_matching/ipfp_solvers.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/matching_utils.py` & `cupid_matching-1.0.7/cupid_matching/matching_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
         iy += 1
     var_munm = jac @ var_muhat @ jac.T
 
     return n_households * var_muhat, n_households * var_munm
 
 
 def _variance_diagonal(var_muhat: np.ndarray, X: int, Y: int) -> Matching:
-    """extracts the variances of muxy, mux0,mu0y
+    """extracts the variances of muxy, mux0, mu0y
 
     Args:
         var_muhat: the variance of muhat as returned by _variance_muhat
         X: the number of types of men
         Y: the number of types of women
 
     Returns:
```

### Comparing `cupid_matching-1.0.5/cupid_matching/min_distance.py` & `cupid_matching-1.0.7/cupid_matching/min_distance.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/min_distance_utils.py` & `cupid_matching-1.0.7/cupid_matching/min_distance_utils.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/mkdocs.yml` & `cupid_matching-1.0.7/cupid_matching/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/model_classes.py` & `cupid_matching-1.0.7/cupid_matching/model_classes.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/nested_logit.py` & `cupid_matching-1.0.7/cupid_matching/nested_logit.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/poisson_glm.py` & `cupid_matching-1.0.7/cupid_matching/poisson_glm.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/poisson_glm_utils.py` & `cupid_matching-1.0.7/cupid_matching/poisson_glm_utils.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/404.html` & `cupid_matching-1.0.7/cupid_matching/site/404.html`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/_mkdocstrings.css` & `cupid_matching-1.0.7/cupid_matching/site/assets/_mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/images/favicon.png` & `cupid_matching-1.0.7/cupid_matching/site/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.ar.min.js` & `cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.ar.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.da.min.js` & `cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.da.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.de.min.js` & `cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.de.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.du.min.js` & `cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.du.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.es.min.js` & `cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.es.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.fi.min.js` & `cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.fi.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.fr.min.js` & `cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.fr.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.hi.min.js` & `cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.hi.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.hu.min.js` & `cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.hu.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.it.min.js` & `cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.it.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.ja.min.js` & `cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.ja.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.ko.min.js` & `cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.ko.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.multi.min.js` & `cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.multi.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.nl.min.js` & `cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.nl.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.no.min.js` & `cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.no.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.pt.min.js` & `cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.pt.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.ro.min.js` & `cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.ro.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.ru.min.js` & `cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.ru.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js` & `cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.sv.min.js` & `cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.sv.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.ta.min.js` & `cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.ta.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.th.min.js` & `cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.th.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.tr.min.js` & `cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.tr.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.vi.min.js` & `cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.vi.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.zh.min.js` & `cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/min/lunr.zh.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/tinyseg.js` & `cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/tinyseg.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/wordcut.js` & `cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/lunr/wordcut.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/workers/search.208ed371.min.js` & `cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/workers/search.208ed371.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/workers/search.208ed371.min.js.map` & `cupid_matching-1.0.7/cupid_matching/site/assets/javascripts/workers/search.208ed371.min.js.map`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/stylesheets/palette.a0c5b2b5.min.css` & `cupid_matching-1.0.7/cupid_matching/site/assets/stylesheets/palette.a0c5b2b5.min.css`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/assets/stylesheets/palette.a0c5b2b5.min.css.map` & `cupid_matching-1.0.7/cupid_matching/site/assets/stylesheets/palette.a0c5b2b5.min.css.map`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/choo_siow/index.html` & `cupid_matching-1.0.7/cupid_matching/site/choo_siow/index.html`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/choo_siow_gender_heteroskedastic/index.html` & `cupid_matching-1.0.7/cupid_matching/site/choo_siow_gender_heteroskedastic/index.html`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/choo_siow_heteroskedastic/index.html` & `cupid_matching-1.0.7/cupid_matching/site/choo_siow_heteroskedastic/index.html`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/cupid_streamlit/index.html` & `cupid_matching-1.0.7/cupid_matching/site/cupid_streamlit/index.html`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/entropy/index.html` & `cupid_matching-1.0.7/cupid_matching/site/entropy/index.html`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/index.html` & `cupid_matching-1.0.7/cupid_matching/site/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -332,14 +332,21 @@
           <li class="md-nav__item">
   <a href="#version-105" class="md-nav__link">
     version 1,0.5
   </a>
   
 </li>
         
+          <li class="md-nav__item">
+  <a href="#version-106" class="md-nav__link">
+    version 1.0.6
+  </a>
+  
+</li>
+        
       </ul>
     </nav>
   
 </li>
       
     </ul>
   
@@ -682,14 +689,21 @@
           <li class="md-nav__item">
   <a href="#version-105" class="md-nav__link">
     version 1,0.5
   </a>
   
 </li>
         
+          <li class="md-nav__item">
+  <a href="#version-106" class="md-nav__link">
+    version 1.0.6
+  </a>
+  
+</li>
+        
       </ul>
     </nav>
   
 </li>
       
     </ul>
   
@@ -747,14 +761,18 @@
 <li>added an optional bias-correction for the minimum distance estimator in the Choo and Siow homoskedastic model, to help with cases when the matching patterns vary a lot across cells.</li>
 <li>added two complete examples: <a href="example_choosiow/">example_choosiow.py</a> and <a href="example_nestedlogit/">example_nestedlogit.py</a>.</li>
 </ul>
 <h3 id="version-105">version 1,0.5<a class="headerlink" href="#version-105" title="Permanent link">&para;</a></h3>
 <ul>
 <li>simplified the bias-correction for the minimum distance estimator in the Choo and Siow homoskedastic model.</li>
 </ul>
+<h3 id="version-106">version 1.0.6<a class="headerlink" href="#version-106" title="Permanent link">&para;</a></h3>
+<ul>
+<li>corrected typo.</li>
+</ul>
 
 
 
 
 
                 
               </article>
```

#### html2text {}

```diff
@@ -27,14 +27,15 @@
           o Installation
           o Importing_functions_from_the_package
           o Examples
           o Warnings
           o Release_notes
                 # version_1.0.4
                 # version_1,0.5
+                # version_1.0.6
     * ⁰  API Reference      API Reference
           o Minimum_Distance_Estimator
           o Utilities_for_MDE
           o Poisson_estimator
           o Utilities_for_Poisson
           o Entropy_utilities
           o Choo-Siow_homoskedastic
@@ -52,14 +53,15 @@
     * Installation
     * Importing_functions_from_the_package
     * Examples
     * Warnings
     * Release_notes
           o version_1.0.4
           o version_1,0.5
+          o version_1.0.6
 ****** cupid_matching¶ ******
 
 A Python package to solve, simulate and estimate separable matching models
     * Free software: MIT license
     * Documentation: https://bsalanie.github.io/cupid_matching
     * See also: An_interactive_Streamlit_app
 ***** Installation¶ *****
@@ -86,9 +88,11 @@
       the Choo and Siow homoskedastic model, to help with cases when the
       matching patterns vary a lot across cells.
     * added two complete examples: example_choosiow.py and
       example_nestedlogit.py.
 **** version 1,0.5¶ ****
     * simplified the bias-correction for the minimum distance estimator in the
       Choo and Siow homoskedastic model.
+**** version 1.0.6¶ ****
+    * corrected typo.
 
 Made with Material_for_MkDocs
```

### Comparing `cupid_matching-1.0.5/cupid_matching/site/ipfp_solvers/index.html` & `cupid_matching-1.0.7/cupid_matching/site/ipfp_solvers/index.html`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/matching_utils/index.html` & `cupid_matching-1.0.7/cupid_matching/site/matching_utils/index.html`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/min_distance/index.html` & `cupid_matching-1.0.7/cupid_matching/site/min_distance/index.html`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/min_distance_utils/index.html` & `cupid_matching-1.0.7/cupid_matching/site/min_distance_utils/index.html`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/model_classes/index.html` & `cupid_matching-1.0.7/cupid_matching/site/model_classes/index.html`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/nested_logit/index.html` & `cupid_matching-1.0.7/cupid_matching/site/nested_logit/index.html`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/objects.inv` & `cupid_matching-1.0.7/cupid_matching/site/objects.inv`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/poisson_glm/index.html` & `cupid_matching-1.0.7/cupid_matching/site/poisson_glm/index.html`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/poisson_glm_utils/index.html` & `cupid_matching-1.0.7/cupid_matching/site/poisson_glm_utils/index.html`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/site/search/search_index.json` & `cupid_matching-1.0.7/cupid_matching/site/search/search_index.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9972527472527473%*

 * *Differences: {"'docs'": "{insert: [(8, OrderedDict([('location', '#version-106'), ('title', 'version 1.0.6'), "*

 * *           "('text', '<ul> <li>corrected typo.</li> </ul>')]))]}"}*

```diff
@@ -46,14 +46,19 @@
         },
         {
             "location": "#version-105",
             "text": "<ul> <li>simplified the bias-correction for the minimum distance estimator in the Choo and Siow homoskedastic model.</li> </ul>",
             "title": "version 1,0.5"
         },
         {
+            "location": "#version-106",
+            "text": "<ul> <li>corrected typo.</li> </ul>",
+            "title": "version 1.0.6"
+        },
+        {
             "location": "choo_siow/",
             "text": "<p>The components of the derivative of the entropy for the Choo and Siow homoskedastic model.</p>",
             "title": "<code>choo_siow</code> module"
         },
         {
             "location": "choo_siow/#cupid_matching.choo_siow.e0_fun_choo_siow",
             "text": "<p>Returns the values of e_0 for the Choo and Siow model.</p> <p>Parameters:</p> Name Type Description Default <code>muhat</code> <code>Matching</code> <p>a Matching</p> required <p>Returns:</p> Type Description <code>np.ndarray</code> <p>the (X,Y) matrix of the first derivative of the entropy</p> Source code in <code>cupid_matching/choo_siow.py</code> <pre><code>def e0_fun_choo_siow(muhat: Matching) -&gt; np.ndarray:\n\"\"\"Returns the values of $e_0$ for the Choo and Siow model.\n\n    Args:\n        muhat: a Matching\n\n    Returns:\n        the (X,Y) matrix of the first derivative of the entropy\n    \"\"\"\n    entropy_res = _entropy_choo_siow(muhat, deriv=1)\n    return entropy_res[1]\n</code></pre>",
```

### Comparing `cupid_matching-1.0.5/cupid_matching/site/sitemap.xml` & `cupid_matching-1.0.7/cupid_matching/site/sitemap.xml`

 * *Files 2% similar despite different names*

#### Comparing `cupid_matching-1.0.5/cupid_matching/site/sitemap.xml` & `cupid_matching-1.0.7/cupid_matching/site/sitemap.xml`

```diff
@@ -1,88 +1,88 @@
 <?xml version="1.0" encoding="utf-8"?>
 <urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/</loc>
-    <lastmod>2023-04-12</lastmod>
+    <lastmod>2023-04-13</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/choo_siow/</loc>
-    <lastmod>2023-04-12</lastmod>
+    <lastmod>2023-04-13</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/choo_siow_gender_heteroskedastic/</loc>
-    <lastmod>2023-04-12</lastmod>
+    <lastmod>2023-04-13</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/choo_siow_heteroskedastic/</loc>
-    <lastmod>2023-04-12</lastmod>
+    <lastmod>2023-04-13</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/cupid_streamlit/</loc>
-    <lastmod>2023-04-12</lastmod>
+    <lastmod>2023-04-13</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/entropy/</loc>
-    <lastmod>2023-04-12</lastmod>
+    <lastmod>2023-04-13</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/example_choosiow/</loc>
-    <lastmod>2023-04-12</lastmod>
+    <lastmod>2023-04-13</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/example_nestedlogit/</loc>
-    <lastmod>2023-04-12</lastmod>
+    <lastmod>2023-04-13</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/ipfp_solvers/</loc>
-    <lastmod>2023-04-12</lastmod>
+    <lastmod>2023-04-13</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/matching_utils/</loc>
-    <lastmod>2023-04-12</lastmod>
+    <lastmod>2023-04-13</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/min_distance/</loc>
-    <lastmod>2023-04-12</lastmod>
+    <lastmod>2023-04-13</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/min_distance_utils/</loc>
-    <lastmod>2023-04-12</lastmod>
+    <lastmod>2023-04-13</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/model_classes/</loc>
-    <lastmod>2023-04-12</lastmod>
+    <lastmod>2023-04-13</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/nested_logit/</loc>
-    <lastmod>2023-04-12</lastmod>
+    <lastmod>2023-04-13</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/poisson_glm/</loc>
-    <lastmod>2023-04-12</lastmod>
+    <lastmod>2023-04-13</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/poisson_glm_utils/</loc>
-    <lastmod>2023-04-12</lastmod>
+    <lastmod>2023-04-13</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/utils/</loc>
-    <lastmod>2023-04-12</lastmod>
+    <lastmod>2023-04-13</lastmod>
     <changefreq>daily</changefreq>
   </url>
 </urlset>
```

### Comparing `cupid_matching-1.0.5/cupid_matching/site/utils/index.html` & `cupid_matching-1.0.7/cupid_matching/site/utils/index.html`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/cupid_matching/utils.py` & `cupid_matching-1.0.7/cupid_matching/utils.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.5/pyproject.toml` & `cupid_matching-1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cupid_matching"
-version = "1.0.5"
+version = "1.0.7"
 description = "Solves, simulates, and estimates separable matching TU models"
 authors = ["Bernard Salanie <bsalanie@columbia.edu>"]
 readme = "README.md"
 packages = [{include = "cupid_matching"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `cupid_matching-1.0.5/PKG-INFO` & `cupid_matching-1.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cupid-matching
-Version: 1.0.5
+Version: 1.0.7
 Summary: Solves, simulates, and estimates separable matching TU models
 Author: Bernard Salanie
 Author-email: bsalanie@columbia.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -61,7 +61,13 @@
 ### version 1.0.4
 * added an optional bias-correction for the minimum distance estimator in the Choo and Siow homoskedastic model, to help with cases when the matching patterns vary a lot across cells.
 * added two complete examples: [example_choosiow.py](example_choosiow.md) and [example_nestedlogit.py](example_nestedlogit.md).
 
 ### version 1,0.5
 * simplified the bias-correction for the minimum distance estimator in the Choo and Siow homoskedastic model.
 
+### version 1.0.6
+* corrected typo.
+
+### version 1.0.7
+* fixed error in bias-correction term.
+
```

