# Comparing `tmp/pywikibot-8.0.3.tar.gz` & `tmp/pywikibot-8.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywikibot-8.0.3.tar", last modified: Wed Mar 29 11:28:05 2023, max compression
+gzip compressed data, was "pywikibot-8.0.4.tar", last modified: Thu Apr 13 11:27:17 2023, max compression
```

## Comparing `pywikibot-8.0.3.tar` & `pywikibot-8.0.4.tar`

### file list

```diff
@@ -1,310 +1,311 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 11:28:05.419319 pywikibot-8.0.3/
--rw-rw-rw-   0        0        0     4115 2023-03-05 15:17:59.000000 pywikibot-8.0.3/AUTHORS.rst
--rw-rw-rw-   0        0        0     1086 2023-03-05 15:17:59.000000 pywikibot-8.0.3/LICENSE
--rw-rw-rw-   0        0        0       40 2023-03-05 15:17:59.000000 pywikibot-8.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0    14330 2023-03-29 11:28:05.418319 pywikibot-8.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     5495 2023-03-05 15:17:59.000000 pywikibot-8.0.3/README.rst
--rw-rw-rw-   0        0        0     6055 2023-03-05 15:17:59.000000 pywikibot-8.0.3/make_dist.py
-drwxrwxrwx   0        0        0        0 2023-03-29 11:28:04.518638 pywikibot-8.0.3/pywikibot/
--rw-rw-rw-   0        0        0    55733 2023-03-29 09:58:23.000000 pywikibot-8.0.3/pywikibot/__init__.py
--rw-rw-rw-   0        0        0      794 2023-03-29 10:43:35.000000 pywikibot-8.0.3/pywikibot/__metadata__.py
--rw-rw-rw-   0        0        0     1886 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/_wbtypes.py
--rw-rw-rw-   0        0        0     4476 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/backports.py
--rw-rw-rw-   0        0        0    95911 2023-03-25 14:04:48.000000 pywikibot-8.0.3/pywikibot/bot.py
--rw-rw-rw-   0        0        0    21207 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/bot_choice.py
-drwxrwxrwx   0        0        0        0 2023-03-29 11:28:04.559498 pywikibot-8.0.3/pywikibot/comms/
--rw-rw-rw-   0        0        0      121 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/comms/__init__.py
--rw-rw-rw-   0        0        0    15749 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/comms/eventstreams.py
--rw-rw-rw-   0        0        0    19142 2023-03-29 09:58:23.000000 pywikibot-8.0.3/pywikibot/comms/http.py
--rw-rw-rw-   0        0        0    46157 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/config.py
--rw-rw-rw-   0        0        0    46135 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/cosmetic_changes.py
--rw-rw-rw-   0        0        0     2090 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/daemonize.py
-drwxrwxrwx   0        0        0        0 2023-03-29 11:28:04.595402 pywikibot-8.0.3/pywikibot/data/
--rw-rw-rw-   0        0        0      160 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 11:28:04.601385 pywikibot-8.0.3/pywikibot/data/api/
--rw-rw-rw-   0        0        0     3174 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/data/api/__init__.py
--rw-rw-rw-   0        0        0    41816 2023-03-05 19:02:40.000000 pywikibot-8.0.3/pywikibot/data/api/_generators.py
--rw-rw-rw-   0        0        0     7398 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/data/api/_optionset.py
--rw-rw-rw-   0        0        0    23233 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/data/api/_paraminfo.py
--rw-rw-rw-   0        0        0    53055 2023-03-29 09:58:23.000000 pywikibot-8.0.3/pywikibot/data/api/_requests.py
--rw-rw-rw-   0        0        0    14143 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/data/memento.py
--rw-rw-rw-   0        0        0     2919 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/data/mysql.py
--rw-rw-rw-   0        0        0     8969 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/data/sparql.py
--rw-rw-rw-   0        0        0     3970 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/data/wikistats.py
--rw-rw-rw-   0        0        0    96943 2023-03-29 09:58:23.000000 pywikibot-8.0.3/pywikibot/date.py
--rw-rw-rw-   0        0        0    24879 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/diff.py
--rw-rw-rw-   0        0        0     2054 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/echo.py
--rw-rw-rw-   0        0        0     7830 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/editor.py
--rw-rw-rw-   0        0        0    20031 2023-03-29 09:58:23.000000 pywikibot-8.0.3/pywikibot/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-03-29 11:28:04.814849 pywikibot-8.0.3/pywikibot/families/
--rw-rw-rw-   0        0        0      118 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/families/__init__.py
--rw-rw-rw-   0        0        0     4303 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/families/commons_family.py
--rw-rw-rw-   0        0        0      443 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/families/foundation_family.py
--rw-rw-rw-   0        0        0      463 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/families/i18n_family.py
--rw-rw-rw-   0        0        0      355 2023-01-01 14:42:07.000000 pywikibot-8.0.3/pywikibot/families/incubator_family.py
--rw-rw-rw-   0        0        0      662 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/families/lingualibre_family.py
--rw-rw-rw-   0        0        0      401 2023-01-01 14:42:07.000000 pywikibot-8.0.3/pywikibot/families/mediawiki_family.py
--rw-rw-rw-   0        0        0      593 2023-01-01 14:42:07.000000 pywikibot-8.0.3/pywikibot/families/meta_family.py
--rw-rw-rw-   0        0        0     1330 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/families/osm_family.py
--rw-rw-rw-   0        0        0      369 2023-01-01 14:42:07.000000 pywikibot-8.0.3/pywikibot/families/outreach_family.py
--rw-rw-rw-   0        0        0      361 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/families/species_family.py
--rw-rw-rw-   0        0        0      638 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/families/vikidia_family.py
--rw-rw-rw-   0        0        0     2418 2023-03-29 10:43:35.000000 pywikibot-8.0.3/pywikibot/families/wikibooks_family.py
--rw-rw-rw-   0        0        0     3782 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/families/wikidata_family.py
--rw-rw-rw-   0        0        0     1742 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/families/wikihow_family.py
--rw-rw-rw-   0        0        0     1009 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/families/wikimania_family.py
--rw-rw-rw-   0        0        0      777 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/families/wikimediachapter_family.py
--rw-rw-rw-   0        0        0     1825 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/families/wikinews_family.py
--rw-rw-rw-   0        0        0    10721 2023-03-29 10:43:35.000000 pywikibot-8.0.3/pywikibot/families/wikipedia_family.py
--rw-rw-rw-   0        0        0     2886 2023-03-29 10:43:35.000000 pywikibot-8.0.3/pywikibot/families/wikiquote_family.py
--rw-rw-rw-   0        0        0     5335 2023-03-25 16:56:51.000000 pywikibot-8.0.3/pywikibot/families/wikisource_family.py
--rw-rw-rw-   0        0        0      495 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/families/wikispore_family.py
--rw-rw-rw-   0        0        0      425 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/families/wikitech_family.py
--rw-rw-rw-   0        0        0     1150 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/families/wikiversity_family.py
--rw-rw-rw-   0        0        0     1027 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/families/wikivoyage_family.py
--rw-rw-rw-   0        0        0     3827 2023-03-29 10:43:35.000000 pywikibot-8.0.3/pywikibot/families/wiktionary_family.py
--rw-rw-rw-   0        0        0     2404 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/families/wowwiki_family.py
--rw-rw-rw-   0        0        0    37565 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/family.py
--rw-rw-rw-   0        0        0    33191 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/fixes.py
--rw-rw-rw-   0        0        0    20119 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/flow.py
--rw-rw-rw-   0        0        0    28565 2023-03-08 17:08:55.000000 pywikibot-8.0.3/pywikibot/i18n.py
--rw-rw-rw-   0        0        0     8343 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/interwiki_graph.py
--rw-rw-rw-   0        0        0    13245 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/logentries.py
--rw-rw-rw-   0        0        0    12508 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/logging.py
--rw-rw-rw-   0        0        0    22815 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/login.py
-drwxrwxrwx   0        0        0        0 2023-03-29 11:28:04.829789 pywikibot-8.0.3/pywikibot/page/
--rw-rw-rw-   0        0        0     2350 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/page/__init__.py
--rw-rw-rw-   0        0        0    86837 2023-03-29 09:58:23.000000 pywikibot-8.0.3/pywikibot/page/_basepage.py
--rw-rw-rw-   0        0        0    14617 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/page/_category.py
--rw-rw-rw-   0        0        0    19000 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/page/_collections.py
--rw-rw-rw-   0        0        0     2183 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/page/_decorators.py
--rw-rw-rw-   0        0        0    14648 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/page/_filepage.py
--rw-rw-rw-   0        0        0    29601 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/page/_links.py
--rw-rw-rw-   0        0        0     8515 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/page/_page.py
--rw-rw-rw-   0        0        0     2997 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/page/_revision.py
--rw-rw-rw-   0        0        0     4049 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/page/_toolforge.py
--rw-rw-rw-   0        0        0    16348 2023-03-24 15:15:52.000000 pywikibot-8.0.3/pywikibot/page/_user.py
--rw-rw-rw-   0        0        0    86179 2023-03-29 09:58:23.000000 pywikibot-8.0.3/pywikibot/page/_wikibase.py
-drwxrwxrwx   0        0        0        0 2023-03-29 11:28:04.868038 pywikibot-8.0.3/pywikibot/pagegenerators/
--rw-rw-rw-   0        0        0    28720 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/pagegenerators/__init__.py
--rw-rw-rw-   0        0        0    40342 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/pagegenerators/_factory.py
--rw-rw-rw-   0        0        0    19272 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/pagegenerators/_filters.py
--rw-rw-rw-   0        0        0    44438 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/pagegenerators/_generators.py
--rw-rw-rw-   0        0        0     3938 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/plural.py
--rw-rw-rw-   0        0        0    48779 2023-03-29 09:58:23.000000 pywikibot-8.0.3/pywikibot/proofreadpage.py
-drwxrwxrwx   0        0        0        0 2023-03-29 11:28:04.942840 pywikibot-8.0.3/pywikibot/scripts/
--rw-rw-rw-   0        0        0      882 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/scripts/__init__.py
--rw-rw-rw-   0        0        0    10348 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/scripts/generate_family_file.py
--rw-rw-rw-   0        0        0    19989 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/scripts/generate_user_files.py
-drwxrwxrwx   0        0        0        0 2023-03-29 11:28:04.949823 pywikibot-8.0.3/pywikibot/scripts/i18n/
--rw-rw-rw-   0        0        0      309 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 11:28:05.312601 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/
--rw-rw-rw-   0        0        0      127 2022-08-26 10:26:37.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ab.json
--rw-rw-rw-   0        0        0      475 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/af.json
--rw-rw-rw-   0        0        0      121 2022-04-07 08:52:21.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/an.json
--rw-rw-rw-   0        0        0     1190 2022-04-28 20:36:35.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ar.json
--rw-rw-rw-   0        0        0      131 2022-04-07 08:52:21.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/arc.json
--rw-rw-rw-   0        0        0     1006 2022-04-28 20:36:35.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ast.json
--rw-rw-rw-   0        0        0      129 2022-04-28 20:36:35.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/av.json
--rw-rw-rw-   0        0        0      150 2022-04-07 08:52:21.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/awa.json
--rw-rw-rw-   0        0        0      864 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/az.json
--rw-rw-rw-   0        0        0      945 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/azb.json
--rw-rw-rw-   0        0        0     1325 2022-04-28 20:36:35.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ba.json
--rw-rw-rw-   0        0        0      176 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/bar.json
--rw-rw-rw-   0        0        0      950 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/bcc.json
--rw-rw-rw-   0        0        0     1450 2022-04-28 20:36:35.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/be-tarask.json
--rw-rw-rw-   0        0        0      857 2022-04-28 20:36:35.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/be.json
--rw-rw-rw-   0        0        0      498 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/bg.json
--rw-rw-rw-   0        0        0      169 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/bjn.json
--rw-rw-rw-   0        0        0      605 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/bn.json
--rw-rw-rw-   0        0        0      179 2022-04-07 08:52:21.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/bo.json
--rw-rw-rw-   0        0        0     1011 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/br.json
--rw-rw-rw-   0        0        0      962 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/bs.json
--rw-rw-rw-   0        0        0     1164 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ca.json
--rw-rw-rw-   0        0        0      944 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ce.json
--rw-rw-rw-   0        0        0      731 2022-08-26 10:26:37.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ckb.json
--rw-rw-rw-   0        0        0     1142 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/cs.json
--rw-rw-rw-   0        0        0      978 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/csb.json
--rw-rw-rw-   0        0        0      723 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/cy.json
--rw-rw-rw-   0        0        0      986 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/da.json
--rw-rw-rw-   0        0        0     1031 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/de.json
--rw-rw-rw-   0        0        0      991 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/diq.json
--rw-rw-rw-   0        0        0     1604 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/el.json
--rw-rw-rw-   0        0        0      993 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/en.json
--rw-rw-rw-   0        0        0     1084 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/eo.json
--rw-rw-rw-   0        0        0     1167 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/es.json
--rw-rw-rw-   0        0        0      297 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/et.json
--rw-rw-rw-   0        0        0     1009 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/eu.json
--rw-rw-rw-   0        0        0     1384 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/fa.json
--rw-rw-rw-   0        0        0      660 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/fi.json
--rw-rw-rw-   0        0        0      775 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/fo.json
--rw-rw-rw-   0        0        0     1252 2022-08-26 10:26:37.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/fr.json
--rw-rw-rw-   0        0        0      191 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/frp.json
--rw-rw-rw-   0        0        0      954 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/frr.json
--rw-rw-rw-   0        0        0       95 2022-04-07 08:52:21.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/fy.json
--rw-rw-rw-   0        0        0      104 2022-04-07 08:52:21.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ga.json
--rw-rw-rw-   0        0        0     1046 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/gl.json
--rw-rw-rw-   0        0        0      752 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/gsw.json
--rw-rw-rw-   0        0        0      669 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/hak.json
--rw-rw-rw-   0        0        0      821 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/haw.json
--rw-rw-rw-   0        0        0     1155 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/he.json
--rw-rw-rw-   0        0        0     1659 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/hi.json
--rw-rw-rw-   0        0        0      167 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/hr.json
--rw-rw-rw-   0        0        0      556 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/hsb.json
--rw-rw-rw-   0        0        0      973 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/hu.json
--rw-rw-rw-   0        0        0      259 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/hy.json
--rw-rw-rw-   0        0        0     1049 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ia.json
--rw-rw-rw-   0        0        0     1112 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/id.json
--rw-rw-rw-   0        0        0      167 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ie.json
--rw-rw-rw-   0        0        0      114 2022-04-07 08:52:21.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ig.json
--rw-rw-rw-   0        0        0      184 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ilo.json
--rw-rw-rw-   0        0        0      977 2022-08-26 10:26:37.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/io.json
--rw-rw-rw-   0        0        0      695 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/is.json
--rw-rw-rw-   0        0        0     1029 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/it.json
--rw-rw-rw-   0        0        0     1076 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ja.json
--rw-rw-rw-   0        0        0      162 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/jv.json
--rw-rw-rw-   0        0        0      542 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/kab.json
--rw-rw-rw-   0        0        0     1027 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/kk.json
--rw-rw-rw-   0        0        0     1381 2022-04-07 08:52:21.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/km.json
--rw-rw-rw-   0        0        0      993 2022-04-07 08:52:21.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/kn.json
--rw-rw-rw-   0        0        0     1106 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ko.json
--rw-rw-rw-   0        0        0     1372 2023-01-09 09:17:09.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/krc.json
--rw-rw-rw-   0        0        0     1154 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ksh.json
--rw-rw-rw-   0        0        0      282 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ku.json
--rw-rw-rw-   0        0        0      331 2022-04-07 08:52:21.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ky.json
--rw-rw-rw-   0        0        0      100 2022-04-07 08:52:21.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/la.json
--rw-rw-rw-   0        0        0      954 2022-08-26 10:26:37.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/lb.json
--rw-rw-rw-   0        0        0      173 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/li.json
--rw-rw-rw-   0        0        0      174 2022-04-07 08:52:21.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/lki.json
--rw-rw-rw-   0        0        0      925 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/lt.json
--rw-rw-rw-   0        0        0      656 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/lv.json
--rw-rw-rw-   0        0        0      718 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/map-bms.json
--rw-rw-rw-   0        0        0      930 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/mg.json
--rw-rw-rw-   0        0        0      639 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/min.json
--rw-rw-rw-   0        0        0     1316 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/mk.json
--rw-rw-rw-   0        0        0     1943 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ml.json
--rw-rw-rw-   0        0        0      168 2022-04-07 08:52:21.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/mni.json
--rw-rw-rw-   0        0        0      267 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/mr.json
--rw-rw-rw-   0        0        0      932 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ms.json
--rw-rw-rw-   0        0        0      169 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/mt.json
--rw-rw-rw-   0        0        0     1292 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/my.json
--rw-rw-rw-   0        0        0     1015 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/nan.json
--rw-rw-rw-   0        0        0      967 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/nb.json
--rw-rw-rw-   0        0        0      949 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/nds-nl.json
--rw-rw-rw-   0        0        0      163 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/nds.json
--rw-rw-rw-   0        0        0     1522 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ne.json
--rw-rw-rw-   0        0        0      891 2022-04-07 08:52:21.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/new.json
--rw-rw-rw-   0        0        0      994 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/nl.json
--rw-rw-rw-   0        0        0      196 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/nn.json
--rw-rw-rw-   0        0        0     1301 2022-08-26 10:26:37.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/nqo.json
--rw-rw-rw-   0        0        0      114 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/nyn.json
--rw-rw-rw-   0        0        0      190 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/oc.json
--rw-rw-rw-   0        0        0      258 2022-04-07 08:52:21.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/olo.json
--rw-rw-rw-   0        0        0      154 2022-04-07 08:52:21.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/or.json
--rw-rw-rw-   0        0        0      216 2022-04-07 08:52:21.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/pa.json
--rw-rw-rw-   0        0        0      100 2022-04-07 08:52:21.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/pdc.json
--rw-rw-rw-   0        0        0      102 2022-04-07 08:52:21.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/pfl.json
--rw-rw-rw-   0        0        0      975 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/pl.json
--rw-rw-rw-   0        0        0      830 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/pms.json
--rw-rw-rw-   0        0        0     1034 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/pt-br.json
--rw-rw-rw-   0        0        0     1151 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/pt.json
--rw-rw-rw-   0        0        0     1690 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/qqq.json
--rw-rw-rw-   0        0        0     1113 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ro.json
--rw-rw-rw-   0        0        0     1545 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ru.json
--rw-rw-rw-   0        0        0      149 2022-04-07 08:52:21.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/scn.json
--rw-rw-rw-   0        0        0      713 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/sco.json
--rw-rw-rw-   0        0        0      311 2022-04-07 08:52:21.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/sd.json
--rw-rw-rw-   0        0        0      551 2022-04-07 08:52:21.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/sh.json
--rw-rw-rw-   0        0        0      485 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/si.json
--rw-rw-rw-   0        0        0     1012 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/sk.json
--rw-rw-rw-   0        0        0      156 2022-04-07 08:52:21.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/skr-arab.json
--rw-rw-rw-   0        0        0     1044 2023-01-09 09:17:09.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/sl.json
--rw-rw-rw-   0        0        0      127 2022-04-07 08:52:21.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/sms.json
--rw-rw-rw-   0        0        0      691 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/so.json
--rw-rw-rw-   0        0        0      416 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/sq.json
--rw-rw-rw-   0        0        0     1402 2022-08-26 10:26:37.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/sr.json
--rw-rw-rw-   0        0        0      313 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/su.json
--rw-rw-rw-   0        0        0     1013 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/sv.json
--rw-rw-rw-   0        0        0      650 2022-04-07 08:52:21.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/sw.json
--rw-rw-rw-   0        0        0      124 2022-04-07 08:52:21.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/szl.json
--rw-rw-rw-   0        0        0      625 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ta.json
--rw-rw-rw-   0        0        0     1346 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/te.json
--rw-rw-rw-   0        0        0     1374 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/th.json
--rw-rw-rw-   0        0        0      101 2022-04-07 08:52:21.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/tk.json
--rw-rw-rw-   0        0        0      183 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/tl.json
--rw-rw-rw-   0        0        0     1074 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/tly.json
--rw-rw-rw-   0        0        0     1125 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/tr.json
--rw-rw-rw-   0        0        0      279 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/tt.json
--rw-rw-rw-   0        0        0     1380 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/uk.json
--rw-rw-rw-   0        0        0      789 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ur.json
--rw-rw-rw-   0        0        0      174 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/uz.json
--rw-rw-rw-   0        0        0      217 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/vec.json
--rw-rw-rw-   0        0        0      121 2022-04-07 08:52:22.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/vep.json
--rw-rw-rw-   0        0        0     1071 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/vi.json
--rw-rw-rw-   0        0        0      116 2022-04-07 08:52:22.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/vo.json
--rw-rw-rw-   0        0        0      182 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/war.json
--rw-rw-rw-   0        0        0      424 2022-04-15 15:42:25.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/yi.json
--rw-rw-rw-   0        0        0      808 2022-04-07 08:52:22.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/yue.json
--rw-rw-rw-   0        0        0     1042 2022-04-28 20:36:36.000000 pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/zh.json
--rw-rw-rw-   0        0        0     6093 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/scripts/login.py
--rw-rw-rw-   0        0        0     3246 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/scripts/preload_sites.py
--rw-rw-rw-   0        0        0     1791 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/scripts/shell.py
--rw-rw-rw-   0        0        0     3313 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/scripts/version.py
--rw-rw-rw-   0        0        0    18491 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/scripts/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-03-29 11:28:05.328558 pywikibot-8.0.3/pywikibot/site/
--rw-rw-rw-   0        0        0      744 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/site/__init__.py
--rw-rw-rw-   0        0        0   111842 2023-03-29 09:58:23.000000 pywikibot-8.0.3/pywikibot/site/_apisite.py
--rw-rw-rw-   0        0        0    15756 2023-03-29 09:58:23.000000 pywikibot-8.0.3/pywikibot/site/_basesite.py
--rw-rw-rw-   0        0        0    38276 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/site/_datasite.py
--rw-rw-rw-   0        0        0     4254 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/site/_decorators.py
--rw-rw-rw-   0        0        0    27978 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/site/_extensions.py
--rw-rw-rw-   0        0        0    92439 2023-03-29 09:58:23.000000 pywikibot-8.0.3/pywikibot/site/_generators.py
--rw-rw-rw-   0        0        0     3003 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/site/_interwikimap.py
--rw-rw-rw-   0        0        0    14558 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/site/_namespace.py
--rw-rw-rw-   0        0        0     1667 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/site/_obsoletesites.py
--rw-rw-rw-   0        0        0    14354 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/site/_siteinfo.py
--rw-rw-rw-   0        0        0     4703 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/site/_tokenwallet.py
--rw-rw-rw-   0        0        0    25321 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/site/_upload.py
--rw-rw-rw-   0        0        0    10800 2023-03-29 09:58:23.000000 pywikibot-8.0.3/pywikibot/site_detect.py
-drwxrwxrwx   0        0        0        0 2023-03-29 11:28:05.351496 pywikibot-8.0.3/pywikibot/specialbots/
--rw-rw-rw-   0        0        0      371 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/specialbots/__init__.py
--rw-rw-rw-   0        0        0     3109 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/specialbots/_unlink.py
--rw-rw-rw-   0        0        0    20247 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/specialbots/_upload.py
--rw-rw-rw-   0        0        0    84825 2023-03-29 10:43:35.000000 pywikibot-8.0.3/pywikibot/textlib.py
--rw-rw-rw-   0        0        0    12074 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/throttle.py
--rw-rw-rw-   0        0        0    15061 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/time.py
--rw-rw-rw-   0        0        0     3267 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/titletranslate.py
-drwxrwxrwx   0        0        0        0 2023-03-29 11:28:05.376430 pywikibot-8.0.3/pywikibot/tools/
--rw-rw-rw-   0        0        0    27088 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/tools/__init__.py
--rw-rw-rw-   0        0        0    25467 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/tools/_deprecate.py
--rw-rw-rw-   0        0        0     1205 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/tools/_logging.py
--rw-rw-rw-   0        0        0    22207 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/tools/_unidata.py
--rw-rw-rw-   0        0        0     3116 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/tools/chars.py
--rw-rw-rw-   0        0        0     8765 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/tools/collections.py
--rw-rw-rw-   0        0        0    11075 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/tools/djvu.py
--rw-rw-rw-   0        0        0     4021 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/tools/formatter.py
--rw-rw-rw-   0        0        0     9745 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/tools/itertools.py
--rw-rw-rw-   0        0        0     7334 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/tools/threading.py
-drwxrwxrwx   0        0        0        0 2023-03-29 11:28:05.410342 pywikibot-8.0.3/pywikibot/userinterfaces/
--rw-rw-rw-   0        0        0      870 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/userinterfaces/__init__.py
--rw-rw-rw-   0        0        0     1906 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/userinterfaces/_interface_base.py
--rw-rw-rw-   0        0        0     2687 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/userinterfaces/buffer_interface.py
--rw-rw-rw-   0        0        0    21724 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/userinterfaces/gui.py
--rw-rw-rw-   0        0        0      457 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/userinterfaces/terminal_interface.py
--rw-rw-rw-   0        0        0    24536 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/userinterfaces/terminal_interface_base.py
--rw-rw-rw-   0        0        0     2114 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/userinterfaces/terminal_interface_unix.py
--rw-rw-rw-   0        0        0     2012 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/userinterfaces/terminal_interface_win32.py
--rw-rw-rw-   0        0        0    90310 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/userinterfaces/transliteration.py
--rw-rw-rw-   0        0        0    16698 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/version.py
--rw-rw-rw-   0        0        0     7366 2023-03-05 15:17:59.000000 pywikibot-8.0.3/pywikibot/xmlreader.py
-drwxrwxrwx   0        0        0        0 2023-03-29 11:28:04.548526 pywikibot-8.0.3/pywikibot.egg-info/
--rw-rw-rw-   0        0        0    14330 2023-03-29 11:28:04.000000 pywikibot-8.0.3/pywikibot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10406 2023-03-29 11:28:04.000000 pywikibot-8.0.3/pywikibot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-29 11:28:04.000000 pywikibot-8.0.3/pywikibot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-03-29 11:28:04.000000 pywikibot-8.0.3/pywikibot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     1228 2023-03-29 11:28:04.000000 pywikibot-8.0.3/pywikibot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-29 11:28:04.000000 pywikibot-8.0.3/pywikibot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-29 11:28:05.419319 pywikibot-8.0.3/setup.cfg
--rw-rw-rw-   0        0        0    13116 2023-03-05 15:17:59.000000 pywikibot-8.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-29 11:28:05.417325 pywikibot-8.0.3/tests/
--rw-rw-rw-   0        0        0     2792 2023-03-29 09:58:23.000000 pywikibot-8.0.3/tests/tests_tests.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:27:17.018679 pywikibot-8.0.4/
+-rw-rw-rw-   0        0        0     4115 2023-04-10 16:20:49.000000 pywikibot-8.0.4/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1086 2023-04-10 16:20:49.000000 pywikibot-8.0.4/LICENSE
+-rw-rw-rw-   0        0        0       40 2023-04-10 16:20:49.000000 pywikibot-8.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    14465 2023-04-13 11:27:17.018679 pywikibot-8.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5495 2023-04-10 16:20:49.000000 pywikibot-8.0.4/README.rst
+-rw-rw-rw-   0        0        0     6057 2023-04-13 11:26:42.000000 pywikibot-8.0.4/make_dist.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:27:15.715347 pywikibot-8.0.4/pywikibot/
+-rw-rw-rw-   0        0        0    55733 2023-04-13 10:49:37.000000 pywikibot-8.0.4/pywikibot/__init__.py
+-rw-rw-rw-   0        0        0      794 2023-04-13 10:49:37.000000 pywikibot-8.0.4/pywikibot/__metadata__.py
+-rw-rw-rw-   0        0        0     1886 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/_wbtypes.py
+-rw-rw-rw-   0        0        0     4476 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/backports.py
+-rw-rw-rw-   0        0        0    95911 2023-04-13 10:49:37.000000 pywikibot-8.0.4/pywikibot/bot.py
+-rw-rw-rw-   0        0        0    21207 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/bot_choice.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:27:15.755242 pywikibot-8.0.4/pywikibot/comms/
+-rw-rw-rw-   0        0        0      121 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/comms/__init__.py
+-rw-rw-rw-   0        0        0    15749 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/comms/eventstreams.py
+-rw-rw-rw-   0        0        0    19142 2023-04-13 10:49:37.000000 pywikibot-8.0.4/pywikibot/comms/http.py
+-rw-rw-rw-   0        0        0    46157 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/config.py
+-rw-rw-rw-   0        0        0    46135 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/cosmetic_changes.py
+-rw-rw-rw-   0        0        0     2090 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/daemonize.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:27:15.793140 pywikibot-8.0.4/pywikibot/data/
+-rw-rw-rw-   0        0        0      160 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:27:15.798128 pywikibot-8.0.4/pywikibot/data/api/
+-rw-rw-rw-   0        0        0     3174 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/data/api/__init__.py
+-rw-rw-rw-   0        0        0    41816 2023-04-10 17:33:59.000000 pywikibot-8.0.4/pywikibot/data/api/_generators.py
+-rw-rw-rw-   0        0        0     7398 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/data/api/_optionset.py
+-rw-rw-rw-   0        0        0    23233 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/data/api/_paraminfo.py
+-rw-rw-rw-   0        0        0    53223 2023-04-13 10:49:37.000000 pywikibot-8.0.4/pywikibot/data/api/_requests.py
+-rw-rw-rw-   0        0        0    14143 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/data/memento.py
+-rw-rw-rw-   0        0        0     2919 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/data/mysql.py
+-rw-rw-rw-   0        0        0     8969 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/data/sparql.py
+-rw-rw-rw-   0        0        0     3970 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/data/wikistats.py
+-rw-rw-rw-   0        0        0    96943 2023-04-13 10:49:37.000000 pywikibot-8.0.4/pywikibot/date.py
+-rw-rw-rw-   0        0        0    24879 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/diff.py
+-rw-rw-rw-   0        0        0     2054 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/echo.py
+-rw-rw-rw-   0        0        0     7830 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/editor.py
+-rw-rw-rw-   0        0        0    20031 2023-04-13 10:49:37.000000 pywikibot-8.0.4/pywikibot/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:27:16.027319 pywikibot-8.0.4/pywikibot/families/
+-rw-rw-rw-   0        0        0      118 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/__init__.py
+-rw-rw-rw-   0        0        0     4303 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/commons_family.py
+-rw-rw-rw-   0        0        0      443 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/foundation_family.py
+-rw-rw-rw-   0        0        0      463 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/i18n_family.py
+-rw-rw-rw-   0        0        0      355 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/incubator_family.py
+-rw-rw-rw-   0        0        0      662 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/lingualibre_family.py
+-rw-rw-rw-   0        0        0      401 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/mediawiki_family.py
+-rw-rw-rw-   0        0        0      593 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/meta_family.py
+-rw-rw-rw-   0        0        0     1330 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/osm_family.py
+-rw-rw-rw-   0        0        0      369 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/outreach_family.py
+-rw-rw-rw-   0        0        0      361 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/species_family.py
+-rw-rw-rw-   0        0        0      638 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/vikidia_family.py
+-rw-rw-rw-   0        0        0     2418 2023-04-13 08:33:09.000000 pywikibot-8.0.4/pywikibot/families/wikibooks_family.py
+-rw-rw-rw-   0        0        0     3782 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/wikidata_family.py
+-rw-rw-rw-   0        0        0     1742 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/wikihow_family.py
+-rw-rw-rw-   0        0        0     1009 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/wikimania_family.py
+-rw-rw-rw-   0        0        0      777 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/wikimediachapter_family.py
+-rw-rw-rw-   0        0        0     1825 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/wikinews_family.py
+-rw-rw-rw-   0        0        0    10721 2023-04-13 08:33:09.000000 pywikibot-8.0.4/pywikibot/families/wikipedia_family.py
+-rw-rw-rw-   0        0        0     2886 2023-04-13 08:33:09.000000 pywikibot-8.0.4/pywikibot/families/wikiquote_family.py
+-rw-rw-rw-   0        0        0     5335 2023-04-13 08:33:09.000000 pywikibot-8.0.4/pywikibot/families/wikisource_family.py
+-rw-rw-rw-   0        0        0      495 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/wikispore_family.py
+-rw-rw-rw-   0        0        0      425 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/wikitech_family.py
+-rw-rw-rw-   0        0        0     1150 2023-04-13 08:33:09.000000 pywikibot-8.0.4/pywikibot/families/wikiversity_family.py
+-rw-rw-rw-   0        0        0     1027 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/wikivoyage_family.py
+-rw-rw-rw-   0        0        0     3827 2023-04-13 08:33:09.000000 pywikibot-8.0.4/pywikibot/families/wiktionary_family.py
+-rw-rw-rw-   0        0        0     2404 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/wowwiki_family.py
+-rw-rw-rw-   0        0        0    37565 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/family.py
+-rw-rw-rw-   0        0        0    33191 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/fixes.py
+-rw-rw-rw-   0        0        0    20119 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/flow.py
+-rw-rw-rw-   0        0        0    28565 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/i18n.py
+-rw-rw-rw-   0        0        0     8343 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/interwiki_graph.py
+-rw-rw-rw-   0        0        0    13245 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/logentries.py
+-rw-rw-rw-   0        0        0    12508 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/logging.py
+-rw-rw-rw-   0        0        0    22815 2023-04-10 16:39:25.000000 pywikibot-8.0.4/pywikibot/login.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:27:16.039289 pywikibot-8.0.4/pywikibot/page/
+-rw-rw-rw-   0        0        0     2350 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/page/__init__.py
+-rw-rw-rw-   0        0        0    86837 2023-04-13 10:49:37.000000 pywikibot-8.0.4/pywikibot/page/_basepage.py
+-rw-rw-rw-   0        0        0    14617 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/page/_category.py
+-rw-rw-rw-   0        0        0    19000 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/page/_collections.py
+-rw-rw-rw-   0        0        0     2183 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/page/_decorators.py
+-rw-rw-rw-   0        0        0    14648 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/page/_filepage.py
+-rw-rw-rw-   0        0        0    29601 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/page/_links.py
+-rw-rw-rw-   0        0        0     8515 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/page/_page.py
+-rw-rw-rw-   0        0        0     2997 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/page/_revision.py
+-rw-rw-rw-   0        0        0     4049 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/page/_toolforge.py
+-rw-rw-rw-   0        0        0    16348 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/page/_user.py
+-rw-rw-rw-   0        0        0    86179 2023-04-13 10:49:37.000000 pywikibot-8.0.4/pywikibot/page/_wikibase.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:27:16.076221 pywikibot-8.0.4/pywikibot/pagegenerators/
+-rw-rw-rw-   0        0        0    28720 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/pagegenerators/__init__.py
+-rw-rw-rw-   0        0        0    40342 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/pagegenerators/_factory.py
+-rw-rw-rw-   0        0        0    19272 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/pagegenerators/_filters.py
+-rw-rw-rw-   0        0        0    44438 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/pagegenerators/_generators.py
+-rw-rw-rw-   0        0        0     3938 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/plural.py
+-rw-rw-rw-   0        0        0    48779 2023-04-13 10:49:37.000000 pywikibot-8.0.4/pywikibot/proofreadpage.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:27:16.140020 pywikibot-8.0.4/pywikibot/scripts/
+-rw-rw-rw-   0        0        0      882 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/scripts/__init__.py
+-rw-rw-rw-   0        0        0    10348 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/scripts/generate_family_file.py
+-rw-rw-rw-   0        0        0    19989 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/scripts/generate_user_files.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:27:16.147999 pywikibot-8.0.4/pywikibot/scripts/i18n/
+-rw-rw-rw-   0        0        0      309 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:27:16.929915 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/
+-rw-rw-rw-   0        0        0      166 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ab.json
+-rw-rw-rw-   0        0        0      511 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/af.json
+-rw-rw-rw-   0        0        0      121 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/an.json
+-rw-rw-rw-   0        0        0     1227 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ar.json
+-rw-rw-rw-   0        0        0      131 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/arc.json
+-rw-rw-rw-   0        0        0     1042 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ast.json
+-rw-rw-rw-   0        0        0      163 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/av.json
+-rw-rw-rw-   0        0        0      150 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/awa.json
+-rw-rw-rw-   0        0        0      898 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/az.json
+-rw-rw-rw-   0        0        0      982 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/azb.json
+-rw-rw-rw-   0        0        0     1362 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ba.json
+-rw-rw-rw-   0        0        0      210 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/bar.json
+-rw-rw-rw-   0        0        0      989 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/bcc.json
+-rw-rw-rw-   0        0        0     1491 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/be-tarask.json
+-rw-rw-rw-   0        0        0      894 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/be.json
+-rw-rw-rw-   0        0        0      535 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/bg.json
+-rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/bjn.json
+-rw-rw-rw-   0        0        0      642 2023-04-06 12:04:37.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/bn.json
+-rw-rw-rw-   0        0        0      179 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/bo.json
+-rw-rw-rw-   0        0        0     1048 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/br.json
+-rw-rw-rw-   0        0        0      998 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/bs.json
+-rw-rw-rw-   0        0        0     1198 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ca.json
+-rw-rw-rw-   0        0        0      981 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ce.json
+-rw-rw-rw-   0        0        0      768 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ckb.json
+-rw-rw-rw-   0        0        0     1178 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/cs.json
+-rw-rw-rw-   0        0        0     1013 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/csb.json
+-rw-rw-rw-   0        0        0      995 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/cy.json
+-rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/da.json
+-rw-rw-rw-   0        0        0     1065 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/de.json
+-rw-rw-rw-   0        0        0     1025 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/diq.json
+-rw-rw-rw-   0        0        0     1647 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/el.json
+-rw-rw-rw-   0        0        0     1027 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/en.json
+-rw-rw-rw-   0        0        0     1121 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/eo.json
+-rw-rw-rw-   0        0        0     1203 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/es.json
+-rw-rw-rw-   0        0        0      333 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/et.json
+-rw-rw-rw-   0        0        0     1043 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/eu.json
+-rw-rw-rw-   0        0        0     1424 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/fa.json
+-rw-rw-rw-   0        0        0      660 2022-04-15 15:42:25.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/fi.json
+-rw-rw-rw-   0        0        0      812 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/fo.json
+-rw-rw-rw-   0        0        0     1291 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/fr.json
+-rw-rw-rw-   0        0        0      227 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/frp.json
+-rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/frr.json
+-rw-rw-rw-   0        0        0       95 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/fy.json
+-rw-rw-rw-   0        0        0      104 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ga.json
+-rw-rw-rw-   0        0        0     1082 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/gl.json
+-rw-rw-rw-   0        0        0      786 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/gsw.json
+-rw-rw-rw-   0        0        0      711 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/hak.json
+-rw-rw-rw-   0        0        0      858 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/haw.json
+-rw-rw-rw-   0        0        0     1192 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/he.json
+-rw-rw-rw-   0        0        0     1699 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/hi.json
+-rw-rw-rw-   0        0        0      201 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/hr.json
+-rw-rw-rw-   0        0        0      593 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/hsb.json
+-rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/hu.json
+-rw-rw-rw-   0        0        0      259 2022-04-15 15:42:25.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/hy.json
+-rw-rw-rw-   0        0        0     1085 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ia.json
+-rw-rw-rw-   0        0        0     1146 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/id.json
+-rw-rw-rw-   0        0        0      205 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ie.json
+-rw-rw-rw-   0        0        0      114 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ig.json
+-rw-rw-rw-   0        0        0      220 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ilo.json
+-rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/io.json
+-rw-rw-rw-   0        0        0      735 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/is.json
+-rw-rw-rw-   0        0        0     1063 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/it.json
+-rw-rw-rw-   0        0        0     1125 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ja.json
+-rw-rw-rw-   0        0        0      196 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/jv.json
+-rw-rw-rw-   0        0        0      581 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/kab.json
+-rw-rw-rw-   0        0        0     1068 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/kk.json
+-rw-rw-rw-   0        0        0     1381 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/km.json
+-rw-rw-rw-   0        0        0      993 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/kn.json
+-rw-rw-rw-   0        0        0     1140 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ko.json
+-rw-rw-rw-   0        0        0     1409 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/krc.json
+-rw-rw-rw-   0        0        0     1188 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ksh.json
+-rw-rw-rw-   0        0        0      318 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ku.json
+-rw-rw-rw-   0        0        0      331 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ky.json
+-rw-rw-rw-   0        0        0      100 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/la.json
+-rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/lb.json
+-rw-rw-rw-   0        0        0      209 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/li.json
+-rw-rw-rw-   0        0        0      174 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/lki.json
+-rw-rw-rw-   0        0        0      963 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/lt.json
+-rw-rw-rw-   0        0        0      691 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/lv.json
+-rw-rw-rw-   0        0        0      752 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/map-bms.json
+-rw-rw-rw-   0        0        0      967 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/mg.json
+-rw-rw-rw-   0        0        0      673 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/min.json
+-rw-rw-rw-   0        0        0     1353 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/mk.json
+-rw-rw-rw-   0        0        0     1943 2022-04-28 20:36:36.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ml.json
+-rw-rw-rw-   0        0        0      168 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/mni.json
+-rw-rw-rw-   0        0        0      267 2022-04-15 15:42:25.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/mr.json
+-rw-rw-rw-   0        0        0      968 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ms.json
+-rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/mt.json
+-rw-rw-rw-   0        0        0     1335 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/my.json
+-rw-rw-rw-   0        0        0     1049 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/nan.json
+-rw-rw-rw-   0        0        0     1003 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/nb.json
+-rw-rw-rw-   0        0        0      983 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/nds-nl.json
+-rw-rw-rw-   0        0        0      197 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/nds.json
+-rw-rw-rw-   0        0        0     1562 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ne.json
+-rw-rw-rw-   0        0        0      891 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/new.json
+-rw-rw-rw-   0        0        0     1037 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/nl.json
+-rw-rw-rw-   0        0        0      232 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/nn.json
+-rw-rw-rw-   0        0        0     1344 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/nqo.json
+-rw-rw-rw-   0        0        0      148 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/nyn.json
+-rw-rw-rw-   0        0        0      226 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/oc.json
+-rw-rw-rw-   0        0        0      258 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/olo.json
+-rw-rw-rw-   0        0        0      154 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/or.json
+-rw-rw-rw-   0        0        0      216 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/pa.json
+-rw-rw-rw-   0        0        0      157 2023-04-06 12:04:37.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/pdc.json
+-rw-rw-rw-   0        0        0      102 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/pfl.json
+-rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/pl.json
+-rw-rw-rw-   0        0        0      870 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/pms.json
+-rw-rw-rw-   0        0        0     1070 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/pt-br.json
+-rw-rw-rw-   0        0        0     1187 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/pt.json
+-rw-rw-rw-   0        0        0     1749 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/qqq.json
+-rw-rw-rw-   0        0        0     1149 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ro.json
+-rw-rw-rw-   0        0        0     1582 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ru.json
+-rw-rw-rw-   0        0        0      149 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/scn.json
+-rw-rw-rw-   0        0        0      749 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sco.json
+-rw-rw-rw-   0        0        0      311 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sd.json
+-rw-rw-rw-   0        0        0      551 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sh.json
+-rw-rw-rw-   0        0        0      528 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/si.json
+-rw-rw-rw-   0        0        0     1046 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sk.json
+-rw-rw-rw-   0        0        0      193 2023-04-06 12:04:37.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/skr-arab.json
+-rw-rw-rw-   0        0        0     1078 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sl.json
+-rw-rw-rw-   0        0        0      127 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sms.json
+-rw-rw-rw-   0        0        0      725 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/so.json
+-rw-rw-rw-   0        0        0      452 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sq.json
+-rw-rw-rw-   0        0        0     1439 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sr.json
+-rw-rw-rw-   0        0        0      347 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/su.json
+-rw-rw-rw-   0        0        0     1047 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sv.json
+-rw-rw-rw-   0        0        0      650 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sw.json
+-rw-rw-rw-   0        0        0      124 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/szl.json
+-rw-rw-rw-   0        0        0      683 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ta.json
+-rw-rw-rw-   0        0        0     1390 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/te.json
+-rw-rw-rw-   0        0        0      101 2023-04-06 12:04:37.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/tg.json
+-rw-rw-rw-   0        0        0     1414 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/th.json
+-rw-rw-rw-   0        0        0      155 2023-04-06 12:04:37.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/tk.json
+-rw-rw-rw-   0        0        0      219 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/tl.json
+-rw-rw-rw-   0        0        0     1115 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/tly.json
+-rw-rw-rw-   0        0        0     1159 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/tr.json
+-rw-rw-rw-   0        0        0      316 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/tt.json
+-rw-rw-rw-   0        0        0     1417 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/uk.json
+-rw-rw-rw-   0        0        0      789 2022-04-28 20:36:36.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ur.json
+-rw-rw-rw-   0        0        0      208 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/uz.json
+-rw-rw-rw-   0        0        0      253 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/vec.json
+-rw-rw-rw-   0        0        0      121 2022-04-07 08:52:22.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/vep.json
+-rw-rw-rw-   0        0        0     1105 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/vi.json
+-rw-rw-rw-   0        0        0      116 2022-04-07 08:52:22.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/vo.json
+-rw-rw-rw-   0        0        0      218 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/war.json
+-rw-rw-rw-   0        0        0      461 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/yi.json
+-rw-rw-rw-   0        0        0      850 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/yue.json
+-rw-rw-rw-   0        0        0     1084 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/zh.json
+-rw-rw-rw-   0        0        0     6093 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/scripts/login.py
+-rw-rw-rw-   0        0        0     3246 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/scripts/preload_sites.py
+-rw-rw-rw-   0        0        0     1791 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/scripts/shell.py
+-rw-rw-rw-   0        0        0     3313 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/scripts/version.py
+-rw-rw-rw-   0        0        0    18491 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/scripts/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:27:16.943879 pywikibot-8.0.4/pywikibot/site/
+-rw-rw-rw-   0        0        0      744 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/site/__init__.py
+-rw-rw-rw-   0        0        0   112319 2023-04-13 10:49:37.000000 pywikibot-8.0.4/pywikibot/site/_apisite.py
+-rw-rw-rw-   0        0        0    15756 2023-04-13 10:49:37.000000 pywikibot-8.0.4/pywikibot/site/_basesite.py
+-rw-rw-rw-   0        0        0    38276 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/site/_datasite.py
+-rw-rw-rw-   0        0        0     4254 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/site/_decorators.py
+-rw-rw-rw-   0        0        0    27978 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/site/_extensions.py
+-rw-rw-rw-   0        0        0    92439 2023-04-13 10:49:37.000000 pywikibot-8.0.4/pywikibot/site/_generators.py
+-rw-rw-rw-   0        0        0     3003 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/site/_interwikimap.py
+-rw-rw-rw-   0        0        0    14558 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/site/_namespace.py
+-rw-rw-rw-   0        0        0     1667 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/site/_obsoletesites.py
+-rw-rw-rw-   0        0        0    14354 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/site/_siteinfo.py
+-rw-rw-rw-   0        0        0     4703 2023-04-13 10:49:37.000000 pywikibot-8.0.4/pywikibot/site/_tokenwallet.py
+-rw-rw-rw-   0        0        0    25321 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/site/_upload.py
+-rw-rw-rw-   0        0        0    10800 2023-04-13 10:49:37.000000 pywikibot-8.0.4/pywikibot/site_detect.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:27:16.967813 pywikibot-8.0.4/pywikibot/specialbots/
+-rw-rw-rw-   0        0        0      371 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/specialbots/__init__.py
+-rw-rw-rw-   0        0        0     3109 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/specialbots/_unlink.py
+-rw-rw-rw-   0        0        0    20247 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/specialbots/_upload.py
+-rw-rw-rw-   0        0        0    84825 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/textlib.py
+-rw-rw-rw-   0        0        0    12074 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/throttle.py
+-rw-rw-rw-   0        0        0    15061 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/time.py
+-rw-rw-rw-   0        0        0     3267 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/titletranslate.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:27:16.994741 pywikibot-8.0.4/pywikibot/tools/
+-rw-rw-rw-   0        0        0    27088 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/tools/__init__.py
+-rw-rw-rw-   0        0        0    25467 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/tools/_deprecate.py
+-rw-rw-rw-   0        0        0     1205 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/tools/_logging.py
+-rw-rw-rw-   0        0        0    22207 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/tools/_unidata.py
+-rw-rw-rw-   0        0        0     3116 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/tools/chars.py
+-rw-rw-rw-   0        0        0     8765 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/tools/collections.py
+-rw-rw-rw-   0        0        0    11075 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/tools/djvu.py
+-rw-rw-rw-   0        0        0     4021 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/tools/formatter.py
+-rw-rw-rw-   0        0        0     9745 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/tools/itertools.py
+-rw-rw-rw-   0        0        0     7334 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/tools/threading.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:27:17.016683 pywikibot-8.0.4/pywikibot/userinterfaces/
+-rw-rw-rw-   0        0        0      870 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/userinterfaces/__init__.py
+-rw-rw-rw-   0        0        0     1906 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/userinterfaces/_interface_base.py
+-rw-rw-rw-   0        0        0     2687 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/userinterfaces/buffer_interface.py
+-rw-rw-rw-   0        0        0    21724 2023-04-13 10:49:37.000000 pywikibot-8.0.4/pywikibot/userinterfaces/gui.py
+-rw-rw-rw-   0        0        0      457 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/userinterfaces/terminal_interface.py
+-rw-rw-rw-   0        0        0    24536 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/userinterfaces/terminal_interface_base.py
+-rw-rw-rw-   0        0        0     2114 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/userinterfaces/terminal_interface_unix.py
+-rw-rw-rw-   0        0        0     2012 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/userinterfaces/terminal_interface_win32.py
+-rw-rw-rw-   0        0        0    90310 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/userinterfaces/transliteration.py
+-rw-rw-rw-   0        0        0    16698 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/version.py
+-rw-rw-rw-   0        0        0     7366 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/xmlreader.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:27:15.744272 pywikibot-8.0.4/pywikibot.egg-info/
+-rw-rw-rw-   0        0        0    14465 2023-04-13 11:27:15.000000 pywikibot-8.0.4/pywikibot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10447 2023-04-13 11:27:15.000000 pywikibot-8.0.4/pywikibot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 11:27:15.000000 pywikibot-8.0.4/pywikibot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-04-13 11:27:15.000000 pywikibot-8.0.4/pywikibot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0     1228 2023-04-13 11:27:15.000000 pywikibot-8.0.4/pywikibot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-13 11:27:15.000000 pywikibot-8.0.4/pywikibot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 11:27:17.019676 pywikibot-8.0.4/setup.cfg
+-rw-rw-rw-   0        0        0    13116 2023-04-13 08:00:35.000000 pywikibot-8.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 11:27:17.017712 pywikibot-8.0.4/tests/
+-rw-rw-rw-   0        0        0     2792 2023-04-13 10:49:37.000000 pywikibot-8.0.4/tests/tests_tests.py
```

### Comparing `pywikibot-8.0.3/AUTHORS.rst` & `pywikibot-8.0.4/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/LICENSE` & `pywikibot-8.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/PKG-INFO` & `pywikibot-8.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywikibot
-Version: 8.0.3
+Version: 8.0.4
 Summary: Python MediaWiki Bot Framework
 Home-page: https://www.mediawiki.org/wiki/Manual:Pywikibot
 Download-URL: https://pywikibot.toolforge.org/
 Maintainer: The Pywikibot team
 Maintainer-email: pywikibot@lists.wikimedia.org
 License: MIT License
 Project-URL: Documentation, https://doc.wikimedia.org/pywikibot/stable/
@@ -257,15 +257,17 @@
 
 Roadmap
 =======
 
 Current release
 ---------------
 
-* Add support for ckb-wiktionary (T332093)
+* L10N Updates
+* Minimal needed mwparserfromhell was decreased to 0.5.2 (T326498, T327600)
+* No longer lazy load password cookies (T271858, T326779, T329132, T330488, T331315)
 
 
 Deprecations
 ------------
 
 * 8.0.0: Timestamp.clone()method is deprecated
   in favour of ``Timestamp.replace()`` method.
```

### Comparing `pywikibot-8.0.3/README.rst` & `pywikibot-8.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/make_dist.py` & `pywikibot-8.0.4/make_dist.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
     if nodist:
         local, remote = False, False
 
     if remote and 'dev' in __version__:
         warning('Distribution must not be a developmental release to upload.')
         remote = False
 
-    sys.argv = [sys.argv[0], 'sdist', 'bdist_wheel']
+    sys.argv = [sys.argv[0], 'sdist']#, 'bdist_wheel']
     return local, remote, clear, upgrade, nodist
 
 
 def main() -> None:  # pragma: no cover
     """Script entry point."""
     args = handle_args()
     SetupPywikibot(*args).run()
```

### Comparing `pywikibot-8.0.3/pywikibot/__init__.py` & `pywikibot-8.0.4/pywikibot/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/__metadata__.py` & `pywikibot-8.0.4/pywikibot/__metadata__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Distributed under the terms of the MIT license.
 #
 from time import strftime
 
 
 __name__ = 'pywikibot'
-__version__ = '8.0.3'
+__version__ = '8.0.4'
 __description__ = 'Python MediaWiki Bot Framework'
 __maintainer__ = 'The Pywikibot team'
 __maintainer_email__ = 'pywikibot@lists.wikimedia.org'
 __license__ = 'MIT License'
 __url__ = 'https://www.mediawiki.org/wiki/Manual:Pywikibot'
 __download_url__ = 'https://pywikibot.toolforge.org/'
 __copyright__ = '(C) Pywikibot team, 2003-' + strftime('%Y')
```

### Comparing `pywikibot-8.0.3/pywikibot/_wbtypes.py` & `pywikibot-8.0.4/pywikibot/_wbtypes.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/backports.py` & `pywikibot-8.0.4/pywikibot/backports.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/bot.py` & `pywikibot-8.0.4/pywikibot/bot.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/bot_choice.py` & `pywikibot-8.0.4/pywikibot/bot_choice.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/comms/eventstreams.py` & `pywikibot-8.0.4/pywikibot/comms/eventstreams.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/comms/http.py` & `pywikibot-8.0.4/pywikibot/comms/http.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/config.py` & `pywikibot-8.0.4/pywikibot/config.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/cosmetic_changes.py` & `pywikibot-8.0.4/pywikibot/cosmetic_changes.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/daemonize.py` & `pywikibot-8.0.4/pywikibot/daemonize.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/data/api/__init__.py` & `pywikibot-8.0.4/pywikibot/data/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/data/api/_generators.py` & `pywikibot-8.0.4/pywikibot/data/api/_generators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/data/api/_optionset.py` & `pywikibot-8.0.4/pywikibot/data/api/_optionset.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/data/api/_paraminfo.py` & `pywikibot-8.0.4/pywikibot/data/api/_paraminfo.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/data/api/_requests.py` & `pywikibot-8.0.4/pywikibot/data/api/_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -943,16 +943,19 @@
         pywikibot.data.api._invalidate_superior_cookies(self.site.family)
         # update tokens
         tokens = self.site.tokens.update_tokens(self._params['token'])
         self._params['token'] = tokens
         return True
 
     def submit(self) -> dict:
-        """
-        Submit a query and parse the response.
+        """Submit a query and parse the response.
+
+        .. versionchanged:: 8.0.4
+           in addition to *readapidenied* also try to login when API
+           response is *notloggedin*.
 
         :return: a dict containing data retrieved from api.php
         """
         self._add_defaults()
         use_get = self._use_get()
         retries = 0
         while True:
@@ -1038,16 +1041,16 @@
                 self.wait()
                 continue
 
             if code == 'ratelimited':
                 self._ratelimited()
                 continue
 
-            # If readapidenied is returned try to login
-            if code == 'readapidenied' \
+            # If notloggedin or readapidenied is returned try to login
+            if code in ('notloggedin', 'readapidenied') \
                and self.site._loginstatus in (LoginStatus.NOT_ATTEMPTED,
                                               LoginStatus.NOT_LOGGED_IN):
                 self.site.login()
                 continue
 
             if self._bad_token(code):
                 continue
```

### Comparing `pywikibot-8.0.3/pywikibot/data/memento.py` & `pywikibot-8.0.4/pywikibot/data/memento.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/data/mysql.py` & `pywikibot-8.0.4/pywikibot/data/mysql.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/data/sparql.py` & `pywikibot-8.0.4/pywikibot/data/sparql.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/data/wikistats.py` & `pywikibot-8.0.4/pywikibot/data/wikistats.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/date.py` & `pywikibot-8.0.4/pywikibot/date.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/diff.py` & `pywikibot-8.0.4/pywikibot/diff.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/echo.py` & `pywikibot-8.0.4/pywikibot/echo.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/editor.py` & `pywikibot-8.0.4/pywikibot/editor.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/exceptions.py` & `pywikibot-8.0.4/pywikibot/exceptions.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/families/commons_family.py` & `pywikibot-8.0.4/pywikibot/families/commons_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/families/lingualibre_family.py` & `pywikibot-8.0.4/pywikibot/families/lingualibre_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/families/meta_family.py` & `pywikibot-8.0.4/pywikibot/families/meta_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/families/osm_family.py` & `pywikibot-8.0.4/pywikibot/families/osm_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/families/vikidia_family.py` & `pywikibot-8.0.4/pywikibot/families/vikidia_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/families/wikibooks_family.py` & `pywikibot-8.0.4/pywikibot/families/wikibooks_family.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     languages_by_size = [
         'en', 'vi', 'hu', 'de', 'fr', 'it', 'ja', 'pt', 'es', 'nl', 'pl', 'id',
         'he', 'fi', 'zh', 'fa', 'az', 'sq', 'ru', 'ca', 'eu', 'th', 'cs', 'da',
         'ko', 'ba', 'sv', 'gl', 'hi', 'sr', 'uk', 'hr', 'no', 'tr', 'sa', 'ar',
         'ta', 'bn', 'eo', 'sk', 'is', 'ro', 'si', 'bg', 'ms', 'mk', 'ka', 'tt',
         'lt', 'el', 'li', 'sl', 'tl', 'ur', 'km', 'la', 'mr', 'kk', 'te', 'et',
-        'be', 'shn', 'ia', 'ml', 'oc', 'hy', 'pa', 'ne', 'cv', 'tg', 'ku',
+        'be', 'ia', 'shn', 'ml', 'oc', 'hy', 'pa', 'ne', 'cv', 'tg', 'ku',
         'fy', 'af', 'bs', 'cy', 'mg', 'ky',
     ]
 
     category_redirect_templates = {
         '_default': (),
         'ar': ('تحويل تصنيف',),
         'en': ('Category redirect',),
```

### Comparing `pywikibot-8.0.3/pywikibot/families/wikidata_family.py` & `pywikibot-8.0.4/pywikibot/families/wikidata_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/families/wikihow_family.py` & `pywikibot-8.0.4/pywikibot/families/wikihow_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/families/wikimania_family.py` & `pywikibot-8.0.4/pywikibot/families/wikimania_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/families/wikimediachapter_family.py` & `pywikibot-8.0.4/pywikibot/families/wikimediachapter_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/families/wikinews_family.py` & `pywikibot-8.0.4/pywikibot/families/wikinews_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/families/wikipedia_family.py` & `pywikibot-8.0.4/pywikibot/families/wikipedia_family.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,37 +30,37 @@
         'ja', 'zh', 'vi', 'war', 'uk', 'ar', 'pt', 'fa', 'ca', 'sr', 'id',
         'ko', 'no', 'ce', 'fi', 'hu', 'cs', 'tr', 'tt', 'sh', 'ro',
         'zh-min-nan', 'eu', 'ms', 'eo', 'he', 'hy', 'da', 'bg', 'cy', 'sk',
         'azb', 'et', 'kk', 'be', 'simple', 'min', 'uz', 'el', 'hr', 'lt', 'gl',
         'az', 'ur', 'sl', 'ka', 'nn', 'hi', 'th', 'ta', 'la', 'bn', 'mk',
         'ast', 'zh-yue', 'lld', 'lv', 'tg', 'af', 'my', 'mg', 'bs', 'mr', 'sq',
         'oc', 'nds', 'ml', 'be-tarask', 'te', 'ky', 'br', 'sw', 'jv', 'new',
-        'vec', 'ht', 'pnb', 'pms', 'ba', 'lb', 'su', 'ku', 'ga', 'lmo', 'szl',
-        'is', 'fy', 'cv', 'ckb', 'tl', 'pa', 'an', 'wuu', 'diq', 'io', 'sco',
-        'vo', 'yo', 'ne', 'gu', 'kn', 'als', 'ia', 'avk', 'bar', 'scn', 'bpy',
-        'crh', 'ha', 'qu', 'mn', 'nv', 'xmf', 'si', 'ban', 'ps', 'bat-smg',
-        'frr', 'os', 'or', 'sah', 'cdo', 'gd', 'bug', 'yi', 'ilo', 'sd', 'am',
-        'nap', 'li', 'gor', 'hsb', 'fo', 'map-bms', 'mai', 'mzn', 'ig', 'bcl',
-        'eml', 'shn', 'ace', 'zh-classical', 'sa', 'wa', 'ie', 'as', 'lij',
-        'zu', 'mhr', 'hyw', 'hif', 'mrj', 'sn', 'bjn', 'mni', 'km', 'hak',
-        'tum', 'roa-tara', 'so', 'pam', 'rue', 'nso', 'bh', 'sat', 'se', 'myv',
-        'mi', 'vls', 'nds-nl', 'nah', 'sc', 'kw', 'glk', 'vep', 'kab', 'tk',
-        'gan', 'ary', 'co', 'dag', 'fiu-vro', 'bo', 'ab', 'gv', 'skr', 'frp',
-        'zea', 'ug', 'udm', 'pcd', 'kv', 'csb', 'rw', 'mt', 'gn', 'smn', 'ay',
-        'nrm', 'lez', 'lfn', 'stq', 'olo', 'lo', 'mwl', 'ang', 'fur', 'rm',
-        'lad', 'gom', 'koi', 'tyv', 'ext', 'dsb', 'av', 'dty', 'ln', 'kaa',
-        'pap', 'cbk-zam', 'dv', 'ksh', 'mdf', 'gag', 'bxr', 'ks', 'pfl', 'tw',
-        'lg', 'pi', 'za', 'pag', 'szy', 'haw', 'awa', 'tay', 'blk', 'inh',
-        'krc', 'xal', 'pdc', 'to', 'atj', 'arc', 'tcy', 'mnw', 'jam', 'kbp',
-        'na', 'wo', 'kbd', 'nia', 'nov', 'ki', 'nqo', 'bi', 'shi', 'tpi',
-        'tet', 'jbo', 'roa-rup', 'xh', 'fj', 'lbe', 'kg', 'om', 'ty', 'guw',
-        'cu', 'trv', 'srn', 'sm', 'gcr', 'alt', 'chr', 'ltg', 'ny', 'tn',
-        'mad', 'st', 'pih', 'got', 'ee', 'ami', 'rmy', 'bm', 've', 'ff', 'ts',
-        'chy', 'ss', 'rn', 'kcg', 'ak', 'pcm', 'ch', 'ik', 'pnt', 'guc', 'ady',
-        'iu', 'pwn', 'sg', 'din', 'ti', 'kl', 'dz', 'gur', 'cr', 'anp',
+        'vec', 'pnb', 'ht', 'pms', 'ba', 'lb', 'su', 'ku', 'ga', 'lmo', 'szl',
+        'is', 'fy', 'cv', 'ckb', 'pa', 'tl', 'an', 'wuu', 'diq', 'io', 'sco',
+        'vo', 'yo', 'ne', 'ia', 'gu', 'kn', 'als', 'avk', 'bar', 'scn', 'bpy',
+        'ha', 'crh', 'qu', 'nv', 'mn', 'xmf', 'si', 'ban', 'ps', 'frr',
+        'bat-smg', 'os', 'or', 'sah', 'cdo', 'gd', 'bug', 'yi', 'sd', 'ilo',
+        'am', 'nap', 'mzn', 'li', 'gor', 'hsb', 'fo', 'map-bms', 'ig', 'mai',
+        'bcl', 'eml', 'shn', 'ace', 'zh-classical', 'sa', 'wa', 'as', 'ie',
+        'lij', 'zu', 'mhr', 'hyw', 'hif', 'mrj', 'sn', 'bjn', 'mni', 'tum',
+        'km', 'hak', 'roa-tara', 'so', 'pam', 'rue', 'nso', 'bh', 'sat', 'se',
+        'myv', 'mi', 'vls', 'nds-nl', 'nah', 'sc', 'kw', 'glk', 'vep', 'kab',
+        'tk', 'gan', 'ary', 'co', 'dag', 'fiu-vro', 'bo', 'ab', 'gv', 'skr',
+        'ug', 'zea', 'frp', 'rw', 'udm', 'pcd', 'kv', 'csb', 'mt', 'gn', 'smn',
+        'ay', 'nrm', 'lez', 'lfn', 'olo', 'stq', 'mwl', 'lo', 'ang', 'fur',
+        'rm', 'lad', 'gom', 'koi', 'ext', 'tyv', 'dsb', 'av', 'ln', 'dty',
+        'kaa', 'pap', 'cbk-zam', 'dv', 'mdf', 'ksh', 'tw', 'gag', 'ks', 'bxr',
+        'pfl', 'lg', 'za', 'pi', 'pag', 'szy', 'haw', 'awa', 'tay', 'blk',
+        'inh', 'krc', 'xal', 'pdc', 'to', 'atj', 'arc', 'tcy', 'mnw', 'jam',
+        'kbp', 'na', 'wo', 'kbd', 'nia', 'nov', 'shi', 'ki', 'nqo', 'bi',
+        'anp', 'tpi', 'tet', 'jbo', 'roa-rup', 'xh', 'fj', 'kg', 'lbe', 'om',
+        'ty', 'guw', 'cu', 'trv', 'srn', 'sm', 'alt', 'gcr', 'chr', 'ltg',
+        'tn', 'ny', 'mad', 'st', 'pih', 'got', 'ee', 'ami', 'rmy', 'bm', 'ff',
+        've', 'ts', 'chy', 'ss', 'kcg', 'rn', 'pcm', 'ch', 'ik', 'pnt', 'guc',
+        'ady', 'iu', 'ak', 'pwn', 'sg', 'din', 'ti', 'kl', 'dz', 'gur', 'cr',
     ]
 
     # Sites we want to edit but not count as real languages
     test_codes = ['test', 'test2']
 
     # Templates that indicate a category redirect
     # Redirects to these templates are automatically included
```

### Comparing `pywikibot-8.0.3/pywikibot/families/wikiquote_family.py` & `pywikibot-8.0.4/pywikibot/families/wikiquote_family.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,31 +13,31 @@
     """Family class for Wikiquote."""
 
     name = 'wikiquote'
 
     closed_wikis = [
         # https://noc.wikimedia.org/conf/highlight.php?file=dblists/closed.dblist
         'am', 'ang', 'ast', 'bm', 'co', 'cr', 'ga', 'kk', 'kr', 'ks', 'kw',
-        'lb', 'na', 'nds', 'qu', 'simple', 'tk', 'tt', 'ug', 'vo', 'za',
+        'lb', 'na', 'nds', 'qu', 'simple', 'tk', 'tt', 'ug', 'vo', 'wo', 'za',
         'zh-min-nan',
     ]
 
     removed_wikis = [
         # https://noc.wikimedia.org/conf/highlight.php?file=dblists/deleted.dblist
         'als', 'tokipona',
     ]
 
     languages_by_size = [
         'it', 'en', 'pl', 'ru', 'cs', 'et', 'pt', 'fa', 'uk', 'he', 'de', 'fr',
-        'es', 'tr', 'eo', 'sk', 'bs', 'az', 'ca', 'fi', 'sr', 'sl', 'zh', 'lt',
-        'ar', 'bg', 'su', 'hy', 'hr', 'el', 'nn', 'id', 'sv', 'li', 'hu', 'ko',
+        'es', 'tr', 'eo', 'sk', 'bs', 'az', 'ca', 'fi', 'sr', 'zh', 'sl', 'lt',
+        'ar', 'su', 'bg', 'hy', 'hr', 'id', 'el', 'nn', 'sv', 'li', 'hu', 'ko',
         'nl', 'sah', 'ja', 'la', 'ta', 'hi', 'gl', 'gu', 'ur', 'ig', 'be',
         'te', 'guw', 'vi', 'tl', 'cy', 'no', 'bn', 'sq', 'ml', 'as', 'kn',
         'ro', 'eu', 'ku', 'uz', 'ka', 'da', 'sa', 'is', 'bcl', 'br', 'th',
-        'mr', 'af', 'wo', 'ky',
+        'mr', 'af', 'ky',
     ]
 
     category_redirect_templates = {
         '_default': (),
         'ar': ('تحويل تصنيف',),
         'en': ('Category redirect',),
         'ro': ('Redirect categorie',),
```

### Comparing `pywikibot-8.0.3/pywikibot/families/wikisource_family.py` & `pywikibot-8.0.4/pywikibot/families/wikisource_family.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     removed_wikis = [
         # https://noc.wikimedia.org/conf/highlight.php?file=dblists/deleted.dblist
         'tokipona',
     ]
 
     languages_by_size = [
         'pl', 'en', 'ru', 'de', 'fr', 'zh', 'he', 'it', 'uk', 'ar', 'es',
-        'mul', 'cs', 'gu', 'sr', 'pt', 'fa', 'sv', 'bn', 'hu', 'ko', 'ta',
+        'mul', 'gu', 'cs', 'sr', 'pt', 'fa', 'sv', 'bn', 'hu', 'ko', 'ta',
         'ml', 'sa', 'te', 'sl', 'tr', 'vi', 'hy', 'la', 'el', 'ja', 'ro', 'fi',
-        'nl', 'nap', 'be', 'az', 'ca', 'hr', 'br', 'kn', 'no', 'th', 'id',
+        'nl', 'nap', 'be', 'az', 'ca', 'hr', 'br', 'kn', 'no', 'id', 'th',
         'hi', 'eo', 'is', 'vec', 'cy', 'ban', 'pms', 'mr', 'lij', 'da', 'et',
         'mk', 'as', 'yi', 'bg', 'jv', 'wa', 'li', 'lt', 'pa', 'eu', 'or', 'gl',
         'bs', 'sah', 'sk', 'zh-min-nan', 'fo',
     ]
 
     # Sites we want to edit but not count as real languages
     test_codes = ['beta']
```

### Comparing `pywikibot-8.0.3/pywikibot/families/wikiversity_family.py` & `pywikibot-8.0.4/pywikibot/families/wikiversity_family.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class Family(family.SubdomainFamily, family.WikimediaFamily):
 
     """Family class for Wikiversity."""
 
     name = 'wikiversity'
 
     languages_by_size = [
-        'de', 'en', 'fr', 'zh', 'it', 'ru', 'cs', 'pt', 'es', 'ar', 'sl', 'sv',
+        'de', 'en', 'fr', 'zh', 'it', 'ru', 'cs', 'pt', 'es', 'sl', 'ar', 'sv',
         'fi', 'el', 'hi', 'ko', 'ja',
     ]
 
     test_codes = ['beta']
 
     @classproperty
     def code_aliases(cls):
```

### Comparing `pywikibot-8.0.3/pywikibot/families/wikivoyage_family.py` & `pywikibot-8.0.4/pywikibot/families/wikivoyage_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/families/wiktionary_family.py` & `pywikibot-8.0.4/pywikibot/families/wiktionary_family.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,28 +29,28 @@
     removed_wikis = [
         # https://noc.wikimedia.org/conf/highlight.php?file=dblists/deleted.dblist
         'als', 'ba', 'dk', 'mo', 'tlh', 'tokipona',
     ]
 
     languages_by_size = [
         'en', 'fr', 'mg', 'zh', 'ru', 'de', 'es', 'sh', 'sv', 'nl', 'el', 'pl',
-        'ku', 'lt', 'ca', 'it', 'hu', 'fi', 'ta', 'tr', 'ja', 'io', 'hy', 'ko',
-        'pt', 'kn', 'vi', 'sr', 'th', 'hi', 'ro', 'no', 'id', 'et', 'cs', 'ml',
-        'skr', 'my', 'uz', 'li', 'or', 'eo', 'te', 'fa', 'gl', 'ar', 'oc',
-        'jv', 'az', 'uk', 'eu', 'sg', 'is', 'ast', 'br', 'bn', 'da', 'mnw',
-        'lo', 'simple', 'la', 'hr', 'sk', 'fj', 'shn', 'ky', 'wa', 'bg', 'tg',
-        'ur', 'ps', 'cy', 'lmo', 'he', 'vo', 'om', 'sl', 'af', 'zh-min-nan',
-        'scn', 'ms', 'tl', 'pa', 'fy', 'sw', 'nn', 'ka', 'min', 'lv', 'sq',
-        'nds', 'gor', 'lb', 'co', 'mn', 'pnb', 'bs', 'nah', 'yue', 'sa', 'kk',
-        'km', 'vec', 'be', 'diq', 'tk', 'mk', 'nia', 'sm', 'hsb', 'ks', 'shy',
-        'su', 'gd', 'bcl', 'ga', 'an', 'gom', 'mr', 'wo', 'mni', 'bjn', 'ia',
-        'ang', 'mt', 'fo', 'sd', 'tt', 'gn', 'so', 'ie', 'mi', 'csb', 'ha',
-        'ug', 'si', 'guw', 'st', 'hif', 'roa-rup', 'jbo', 'kl', 'zu', 'ay',
-        'yi', 'ln', 'gu', 'na', 'gv', 'kw', 'tpi', 'am', 'ne', 'rw', 'ts',
-        'ig', 'qu', 'ss', 'iu', 'chr', 'dv', 'ti', 'tn', 'ckb',
+        'ku', 'lt', 'ca', 'it', 'hu', 'fi', 'ta', 'tr', 'pt', 'ja', 'io', 'hy',
+        'ko', 'kn', 'vi', 'sr', 'th', 'hi', 'ro', 'no', 'id', 'et', 'cs',
+        'skr', 'ml', 'my', 'uz', 'li', 'or', 'eo', 'te', 'fa', 'gl', 'ar',
+        'oc', 'jv', 'az', 'uk', 'eu', 'sg', 'is', 'ast', 'br', 'bn', 'da',
+        'mnw', 'lo', 'simple', 'la', 'hr', 'sk', 'shn', 'fj', 'ky', 'wa', 'bg',
+        'tg', 'ur', 'ps', 'cy', 'lmo', 'he', 'vo', 'om', 'sl', 'af',
+        'zh-min-nan', 'scn', 'ms', 'tl', 'pa', 'fy', 'sw', 'ka', 'nn', 'min',
+        'lv', 'sq', 'nds', 'gor', 'lb', 'co', 'mn', 'pnb', 'bs', 'nah', 'yue',
+        'sa', 'kk', 'km', 'ckb', 'vec', 'be', 'diq', 'tk', 'mk', 'nia', 'sm',
+        'hsb', 'ks', 'shy', 'su', 'gd', 'bcl', 'ga', 'an', 'gom', 'mr', 'wo',
+        'mni', 'bjn', 'ia', 'ang', 'mt', 'fo', 'sd', 'tt', 'gn', 'so', 'ie',
+        'mi', 'csb', 'ha', 'ug', 'si', 'guw', 'st', 'hif', 'roa-rup', 'jbo',
+        'kl', 'zu', 'ay', 'yi', 'ln', 'gu', 'na', 'gv', 'kw', 'tpi', 'am',
+        'ne', 'rw', 'ts', 'ig', 'qu', 'ss', 'iu', 'chr', 'dv', 'ti', 'tn',
     ]
 
     category_redirect_templates = {
         '_default': (),
         'ar': ('تحويل تصنيف',),
         'zh': ('分类重定向',),
     }
```

### Comparing `pywikibot-8.0.3/pywikibot/families/wowwiki_family.py` & `pywikibot-8.0.4/pywikibot/families/wowwiki_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/family.py` & `pywikibot-8.0.4/pywikibot/family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/fixes.py` & `pywikibot-8.0.4/pywikibot/fixes.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/flow.py` & `pywikibot-8.0.4/pywikibot/flow.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/i18n.py` & `pywikibot-8.0.4/pywikibot/i18n.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/interwiki_graph.py` & `pywikibot-8.0.4/pywikibot/interwiki_graph.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/logentries.py` & `pywikibot-8.0.4/pywikibot/logentries.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/logging.py` & `pywikibot-8.0.4/pywikibot/logging.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/login.py` & `pywikibot-8.0.4/pywikibot/login.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/page/__init__.py` & `pywikibot-8.0.4/pywikibot/page/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/page/_basepage.py` & `pywikibot-8.0.4/pywikibot/page/_basepage.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/page/_category.py` & `pywikibot-8.0.4/pywikibot/page/_category.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/page/_collections.py` & `pywikibot-8.0.4/pywikibot/page/_collections.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/page/_decorators.py` & `pywikibot-8.0.4/pywikibot/page/_decorators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/page/_filepage.py` & `pywikibot-8.0.4/pywikibot/page/_filepage.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/page/_links.py` & `pywikibot-8.0.4/pywikibot/page/_links.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/page/_page.py` & `pywikibot-8.0.4/pywikibot/page/_page.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/page/_revision.py` & `pywikibot-8.0.4/pywikibot/page/_revision.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/page/_toolforge.py` & `pywikibot-8.0.4/pywikibot/page/_toolforge.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/page/_user.py` & `pywikibot-8.0.4/pywikibot/page/_user.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/page/_wikibase.py` & `pywikibot-8.0.4/pywikibot/page/_wikibase.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/pagegenerators/__init__.py` & `pywikibot-8.0.4/pywikibot/pagegenerators/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/pagegenerators/_factory.py` & `pywikibot-8.0.4/pywikibot/pagegenerators/_factory.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/pagegenerators/_filters.py` & `pywikibot-8.0.4/pywikibot/pagegenerators/_filters.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/pagegenerators/_generators.py` & `pywikibot-8.0.4/pywikibot/pagegenerators/_generators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/plural.py` & `pywikibot-8.0.4/pywikibot/plural.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/proofreadpage.py` & `pywikibot-8.0.4/pywikibot/proofreadpage.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/scripts/__init__.py` & `pywikibot-8.0.4/pywikibot/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/scripts/generate_family_file.py` & `pywikibot-8.0.4/pywikibot/scripts/generate_family_file.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/scripts/generate_user_files.py` & `pywikibot-8.0.4/pywikibot/scripts/generate_user_files.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ar.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ar.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'بوت:'"}*

```diff
@@ -5,14 +5,15 @@
             "OsamaK",
             "TTMTT",
             "Zaher kadour",
             "Zanatos",
             "\u062f\u064a\u0641\u064a\u062f"
         ]
     },
+    "pywikibot-bot-prefix": "\u0628\u0648\u062a:",
     "pywikibot-cosmetic-changes": "\u060c \u062a\u063a\u064a\u064a\u0631\u0627\u062a \u062a\u062c\u0645\u064a\u0644\u064a\u0629",
     "pywikibot-enter-category-name": "\u0641\u0636\u0644\u0627 \u0623\u062f\u062e\u0644 \u0627\u0633\u0645 \u0627\u0644\u062a\u0635\u0646\u064a\u0641:",
     "pywikibot-enter-file-links-processing": "\u0627\u0644\u0648\u0635\u0644\u0627\u062a \u0644\u0623\u064a \u0635\u0641\u062d\u0629 \u0645\u0644\u0641 \u064a\u0646\u0628\u063a\u064a \u0623\u0646 \u062a\u062a\u0645 \u0645\u0639\u0627\u0644\u062c\u062a\u0647\u0627\u061f",
     "pywikibot-enter-finished-browser": "\u0627\u0636\u063a\u0637 Enter \u0639\u0646\u062f \u0627\u0644\u0627\u0646\u062a\u0647\u0627\u0621 \u0641\u064a \u0627\u0644\u0645\u062a\u0635\u0641\u062d.",
     "pywikibot-enter-namespace-number": "\u0627\u0644\u0631\u062c\u0627\u0621 \u0625\u062f\u062e\u0627\u0644 \u0646\u0637\u0627\u0642 \u0628\u0631\u0642\u0645\u0647:",
     "pywikibot-enter-new-text": "\u0641\u0636\u0644\u0627 \u0623\u062f\u062e\u0644 \u0627\u0644\u0646\u0635 \u0627\u0644\u062c\u062f\u064a\u062f:",
     "pywikibot-enter-page-processing": "\u0627\u0644\u0635\u0641\u062d\u0629 \u0627\u0644\u062a\u064a \u062a\u0646\u0628\u063a\u064a \u0645\u0639\u0627\u0644\u062c\u062a\u0647\u0627\u061f",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ast.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ast.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Robó:'"}*

```diff
@@ -1,14 +1,15 @@
 {
     "@metadata": {
         "authors": [
             "Esbardu",
             "Xuacu"
         ]
     },
+    "pywikibot-bot-prefix": "Rob\u00f3:",
     "pywikibot-cosmetic-changes": "; cambios cosm\u00e9ticos",
     "pywikibot-enter-category-name": "Escribi'l nome de categor\u00eda:",
     "pywikibot-enter-file-links-processing": "\u00bfQu\u00e9 enllaces a p\u00e1xina de ficheru hai que procesar?",
     "pywikibot-enter-finished-browser": "Calca la tecla Intro cuando acabes nel navegador.",
     "pywikibot-enter-namespace-number": "Escribi un espaciu de nomes pol so n\u00famberu:",
     "pywikibot-enter-new-text": "Escribi'l testu nuevu:",
     "pywikibot-enter-page-processing": "\u00bfQue p\u00e1xina hai que procesar?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/az.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/az.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9090909090909091%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Bot:'"}*

```diff
@@ -2,14 +2,15 @@
     "@metadata": {
         "authors": [
             "AZISS",
             "Khutuck",
             "Vago"
         ]
     },
+    "pywikibot-bot-prefix": "Bot:",
     "pywikibot-cosmetic-changes": "; kosmetik d\u0259yi\u015fm\u0259l\u0259r",
     "pywikibot-enter-category-name": "Z\u0259hm\u0259t olmasa, kateqoriyan\u0131n ad\u0131n\u0131 daxil edin:",
     "pywikibot-enter-file-links-processing": "\u015e\u0259kill\u0259rin hans\u0131 s\u0259hif\u0259sinin istinadlar\u0131n\u0131 emal etm\u0259k laz\u0131md\u0131r?",
     "pywikibot-enter-finished-browser": "Brauzerd\u0259 i\u015finizi bitirdikd\u0259n sonra Enter d\u00fcym\u0259sin\u0259 bas\u0131n.",
     "pywikibot-enter-namespace-number": "Z\u0259hm\u0259t olmasa, ad sah\u0259sinin n\u00f6mr\u0259sini daxil edin:",
     "pywikibot-enter-new-text": "Z\u0259hm\u0259t olmasa, yeni m\u0259tni daxil edin:",
     "pywikibot-enter-page-processing": "Hans\u0131 s\u0259hif\u0259 emal edilm\u0259lidir?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/azb.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/azb.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9090909090909091%*

 * *Differences: {"'pywikibot-bot-prefix'": "'بوت:'"}*

```diff
@@ -1,14 +1,15 @@
 {
     "@metadata": {
         "authors": [
             "Amir a57",
             "E THP"
         ]
     },
+    "pywikibot-bot-prefix": "\u0628\u0648\u062a:",
     "pywikibot-cosmetic-changes": "\u061b \u0632\u0646\u06af\u06cc\u0646\u0644\u0634\u062f\u06cc\u0631\u0645\u0647",
     "pywikibot-enter-category-name": "\u0628\u0624\u0644\u0645\u0647 \u0622\u062f\u06cc\u0646 \u06cc\u0627\u0632\u06cc\u0646:",
     "pywikibot-enter-file-links-processing": "\u0628\u0627\u063a\u0644\u0627\u0646\u062a\u06cc \u0627\u0648\u0686\u0648\u0646 \u0647\u0627\u0646\u0633\u06cc \u0634\u06a9\u06cc\u0644 \u06af\u0631\u06a9 \u067e\u0631\u062f\u0627\u062e\u062a \u0627\u0648\u0644\u0648\u0646\u0627\u061f",
     "pywikibot-enter-finished-browser": "\u0622\u062e\u062a\u0627\u0631\u06cc\u0634 \u0628\u0631\u0646\u0627\u0645\u0647 \u0633\u06cc \u0627\u06cc\u0646\u062a\u0626\u0631 \u062f\u0648\u06cc\u0645\u0647\u200c\u0633\u06cc\u0646\u0647 \u0645\u062a\u0628\u0648\u0627\u062a \u0628\u06cc\u062a\u0646 \u0632\u0627\u0645\u0627\u0646",
     "pywikibot-enter-namespace-number": "\u0622\u062f \u0622\u0644\u0627\u0646 (\u0646\u0648\u0645\u0631\u0647 \u0633\u06cc)\u060c \u062f\u0627\u062e\u06cc\u0644 \u0639\u0644\u0627\u0648\u0647 \u0627\u0626\u062f\u06cc\u0646:",
     "pywikibot-enter-new-text": "\u06cc\u0626\u0646\u06cc \u06cc\u0627\u0632\u06cc\u0646\u06cc \u0622\u0631\u062a\u06cc\u0631\u06cc\u0646",
     "pywikibot-enter-page-processing": "\u0647\u0627\u0646\u0633\u06cc \u0635\u062d\u06cc\u0641\u0647 \u06af\u0631\u06a9 \u067e\u0631\u062f\u0627\u062e\u062a \u0627\u0648\u0644\u0648\u0646\u0627\u061f",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ba.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ba.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Бот:'"}*

```diff
@@ -2,14 +2,15 @@
     "@metadata": {
         "authors": [
             "Haqmar",
             "MR973",
             "Sagan"
         ]
     },
+    "pywikibot-bot-prefix": "\u0411\u043e\u0442:",
     "pywikibot-cosmetic-changes": "; \u043a\u043e\u0441\u043c\u0435\u0442\u0438\u043a \u04af\u0499\u0433\u04d9\u0440\u0442\u0435\u04af\u0499\u04d9\u0440",
     "pywikibot-enter-category-name": "\u041a\u0430\u0442\u0435\u0433\u043e\u0440\u0438\u044f \u0438\u0441\u0435\u043c\u0435\u043d \u044f\u0499\u044b\u0493\u044b\u0499:",
     "pywikibot-enter-file-links-processing": "\u0424\u0430\u0439\u043b\u0434\u044b\u04a3 \u04a1\u0430\u0439\u04bb\u044b \u0431\u0438\u0442\u0435\u043d\u04d9 \u04bb\u044b\u043b\u0442\u0430\u043d\u043c\u0430\u043d\u043c\u0430\u043b\u0430\u0440  \u044d\u0448\u043a\u04d9\u0440\u0442\u0435\u043b\u0435\u0440\u0433\u04d9 \u0442\u0435\u0439\u0435\u0448?",
     "pywikibot-enter-finished-browser": "\u0411\u0440\u0430\u0443\u0437\u0435\u0440\u0499\u0430 \u044d\u0448 \u0442\u0430\u043c\u0430\u043c\u043b\u0430\u043d\u0493\u0430\u043d\u0434\u0430\u043d \u04bb\u0443\u04a3 Enter \u0442\u04e9\u0439\u043c\u04d9\u04bb\u0435\u043d\u04d9 \u0431\u0430\u04ab\u044b\u0493\u044b\u0499.",
     "pywikibot-enter-namespace-number": "\u0418\u0441\u0435\u043c \u0430\u0440\u0430\u0443\u044b\u0493\u044b \u043d\u043e\u043c\u0435\u0440\u044b\u043d \u044f\u0499\u044b\u0493\u044b\u0499:",
     "pywikibot-enter-new-text": "\u042f\u04a3\u044b \u0442\u0435\u043a\u0441\u0442 \u044f\u0499\u044b\u0493\u044b\u0499:",
     "pywikibot-enter-page-processing": "\u04a0\u0430\u0439\u04bb\u044b \u0431\u0438\u0442 \u044d\u0448\u043a\u04d9\u0440\u0442\u0435\u043b\u0435\u0440\u0433\u04d9 \u0442\u0435\u0439\u0435\u0448?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/bcc.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/bcc.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9090909090909091%*

 * *Differences: {"'pywikibot-bot-prefix'": "'ربات:'"}*

```diff
@@ -1,13 +1,14 @@
 {
     "@metadata": {
         "authors": [
             "Baloch Afghanistan"
         ]
     },
+    "pywikibot-bot-prefix": "\u0631\u0628\u0627\u062a:",
     "pywikibot-cosmetic-changes": "\u061b \u0632\u06cc\u0628\u0627\u0633\u0627\u0632\u06cc",
     "pywikibot-enter-category-name": "\u0644\u0637\u0641\u0627\u064b \u0646\u0627\u0645 \u0631\u062f\u0647 \u0631\u0627 \u0648\u0627\u0631\u062f \u06a9\u0646\u06cc\u062f:",
     "pywikibot-enter-file-links-processing": "\u067e\u06cc\u0648\u0646\u062f \u0628\u0647 \u06a9\u062f\u0627\u0645 \u067e\u0631\u0648\u0646\u062f\u0647 \u0628\u0627\u06cc\u062f \u067e\u0631\u062f\u0627\u0632\u0634 \u0634\u0648\u062f\u061f",
     "pywikibot-enter-finished-browser": "\u0647\u0646\u06af\u0627\u0645\u06cc \u06a9\u0647 \u062f\u0631 \u0645\u0631\u0648\u0631\u06af\u0631 \u067e\u0627\u06cc\u0627\u0646 \u06cc\u0627\u0641\u062a \u062f\u06a9\u0645\u0647\u0654 \u0627\u06cc\u0646\u062a\u0631 \u0631\u0627 \u0628\u0641\u0634\u0627\u0631\u06cc\u062f.",
     "pywikibot-enter-namespace-number": "\u0644\u0637\u0641\u0627\u064b \u0634\u0645\u0627\u0631\u0647\u0654 \u06cc\u06a9 \u0641\u0636\u0627\u06cc \u0646\u0627\u0645 \u0631\u0627 \u0648\u0627\u0631\u062f \u06a9\u0646\u06cc\u062f:",
     "pywikibot-enter-new-text": "\u0644\u0637\u0641\u0627\u064b \u0645\u062a\u0646 \u062c\u062f\u06cc\u062f \u0631\u0627 \u0648\u0627\u0631\u062f \u06a9\u0646\u06cc\u062f:",
     "pywikibot-enter-page-processing": "\u06a9\u062f\u0627\u0645 \u0635\u0641\u062d\u0647 \u0628\u0627\u06cc\u062f \u067e\u0631\u062f\u0627\u0632\u0634 \u0634\u0648\u062f\u061f",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/be-tarask.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/be-tarask.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Робат:'"}*

```diff
@@ -4,14 +4,15 @@
             "Dmitry Nikitin",
             "EugeneZelenko",
             "Jim-by",
             "Red Winged Duck",
             "Renessaince"
         ]
     },
+    "pywikibot-bot-prefix": "\u0420\u043e\u0431\u0430\u0442:",
     "pywikibot-cosmetic-changes": "; \u043a\u0430\u0441\u043c\u044d\u0442\u044b\u0447\u043d\u044b\u044f \u0437\u044c\u043c\u0435\u043d\u044b",
     "pywikibot-enter-category-name": "\u041a\u0430\u043b\u0456 \u043b\u0430\u0441\u043a\u0430, \u0443\u0432\u044f\u0434\u0437\u0456\u0446\u0435 \u043d\u0430\u0437\u0432\u0443 \u043a\u0430\u0442\u044d\u0433\u043e\u0440\u044b\u0456:",
     "pywikibot-enter-file-links-processing": "\u0421\u043f\u0430\u0441\u044b\u043b\u043a\u0456 \u043d\u0430 \u044f\u043a\u0456 \u0444\u0430\u0439\u043b \u043f\u0430\u0442\u0440\u044d\u0431\u043d\u0430 \u0430\u043f\u0440\u0430\u0446\u0430\u0432\u0430\u0446\u044c?",
     "pywikibot-enter-finished-browser": "\u041d\u0430\u0446\u0456\u0441\u044c\u043d\u0456\u0446\u0435 Enter, \u043a\u0430\u043b\u0456 \u0441\u043a\u043e\u043d\u0447\u044b\u0446\u0435 \u0440\u044d\u0434\u0430\u0433\u0430\u0432\u0430\u043d\u044c\u043d\u0435 \u045e \u0431\u0440\u043e\u045e\u0437\u044d\u0440\u044b.",
     "pywikibot-enter-namespace-number": "\u041a\u0430\u043b\u0456 \u043b\u0430\u0441\u043a\u0430, \u0443\u0432\u044f\u0434\u0437\u0456\u0446\u0435 \u043d\u0443\u043c\u0430\u0440 \u043f\u0440\u0430\u0441\u0442\u043e\u0440\u044b \u0456\u043c\u0451\u043d\u0430\u045e:",
     "pywikibot-enter-new-text": "\u041a\u0430\u043b\u0456 \u043b\u0430\u0441\u043a\u0430, \u0443\u0432\u044f\u0434\u0437\u0456\u0446\u0435 \u043d\u043e\u0432\u044b \u0442\u044d\u043a\u0441\u0442:",
     "pywikibot-enter-page-processing": "\u042f\u043a\u0443\u044e \u0441\u0442\u0430\u0440\u043e\u043d\u043a\u0443 \u043f\u0430\u0442\u0440\u044d\u0431\u043d\u0430 \u0430\u043f\u0440\u0430\u0446\u0430\u0432\u0430\u0446\u044c?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/be.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/be.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Бот:'"}*

```diff
@@ -3,14 +3,15 @@
         "authors": [
             "Francesco Cosoleto",
             "LexArt",
             "Mechanizatar",
             "Yury Tarasievich"
         ]
     },
+    "pywikibot-bot-prefix": "\u0411\u043e\u0442:",
     "pywikibot-cosmetic-changes": "; \u0434\u0440\u043e\u0431\u043d\u044b\u044f \u0437\u043c\u0435\u043d\u044b",
     "pywikibot-enter-category-name": "\u041a\u0430\u043b\u0456 \u043b\u0430\u0441\u043a\u0430, \u0443\u0432\u044f\u0434\u0437\u0456\u0446\u0435 \u043d\u0430\u0437\u0432\u0443 \u043a\u0430\u0442\u044d\u0433\u043e\u0440\u044b\u0456:",
     "pywikibot-enter-namespace-number": "\u041a\u0430\u043b\u0456 \u043b\u0430\u0441\u043a\u0430, \u0443\u0432\u044f\u0434\u0437\u0456\u0446\u0435 \u043d\u0443\u043c\u0430\u0440 \u043f\u0440\u0430\u0441\u0442\u043e\u0440\u044b \u0456\u043c\u0451\u043d\u0430\u045e:",
     "pywikibot-enter-new-text": "\u041a\u0430\u043b\u0456 \u043b\u0430\u0441\u043a\u0430, \u0443\u0432\u044f\u0434\u0437\u0456\u0446\u0435 \u043d\u043e\u0432\u044b \u0442\u044d\u043a\u0441\u0442:",
     "pywikibot-fixes-fckeditor": "\u0420\u043e\u0431\u0430\u0442: \u0412\u044b\u043f\u0440\u0430\u045e\u043b\u0435\u043d\u043d\u0435 HTML-\u043a\u043e\u0434\u0430 \u0440\u044d\u0434\u0430\u043a\u0442\u0430\u0440\u0430 \u0444\u0430\u0440\u043c\u0430\u0442\u0430\u0432\u0430\u043d\u0430\u0433\u0430 \u0442\u044d\u043a\u0441\u0442\u0443",
     "pywikibot-fixes-html": "\u0411\u043e\u0442: \u043a\u0430\u0440\u044d\u043a\u0446\u044b\u044f HTML",
     "pywikibot-fixes-isbn": "\u0440\u043e\u0431\u0430\u0442 \u0430\u0444\u043e\u0440\u043c\u0456\u045e ISBN",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/bn.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/bn.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'pywikibot-bot-prefix'": "'বট:'"}*

```diff
@@ -6,12 +6,13 @@
             "Tahmid",
             "Tahmid02016",
             "Tauhid16",
             "Wikitanvir",
             "\u0986\u09ab\u09a4\u09be\u09ac\u09c1\u099c\u09cd\u099c\u09be\u09ae\u09be\u09a8"
         ]
     },
+    "pywikibot-bot-prefix": "\u09ac\u099f:",
     "pywikibot-cosmetic-changes": "; \u09b8\u099c\u09cd\u099c\u09be \u09aa\u09b0\u09bf\u09ac\u09b0\u09cd\u09a4\u09a8",
     "pywikibot-enter-category-name": "\u09ac\u09bf\u09b7\u09af\u09bc\u09b6\u09cd\u09b0\u09c7\u09a3\u09c0\u09b0 \u09a8\u09be\u09ae \u09aa\u09cd\u09b0\u09ac\u09c7\u09b6 \u0995\u09b0\u09be\u09a8:",
     "pywikibot-enter-new-text": "\u09a6\u09af\u09bc\u09be \u0995\u09b0\u09c7 \u09a8\u09a4\u09c1\u09a8 \u09ac\u09be\u0995\u09cd\u09af \u09b2\u09bf\u0996\u09c1\u09a8:",
     "pywikibot-fixes-isbn": "\u09ac\u099f: \u0986\u0987\u098f\u09b8\u09ac\u09bf\u098f\u09a8 \u09ac\u09bf\u09a8\u09cd\u09af\u09be\u09b8 \u09a0\u09bf\u0995 \u0995\u09b0\u09c7\u099b\u09c7"
 }
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/br.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/br.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Robot :'"}*

```diff
@@ -1,14 +1,15 @@
 {
     "@metadata": {
         "authors": [
             "Fulup",
             "Gwenn-Ael"
         ]
     },
+    "pywikibot-bot-prefix": "Robot :",
     "pywikibot-cosmetic-changes": "; Kemmo\u00f9 dister",
     "pywikibot-enter-category-name": "Ebarzhit anv ar rummad, mar plij",
     "pywikibot-enter-file-links-processing": "Liammo\u00f9 war-zu ar bajenn a vefe mat pledi\u00f1 ganti?",
     "pywikibot-enter-finished-browser": "Ebarzhit war Kas ur wech m'ho peus echuet er merdeer.",
     "pywikibot-enter-namespace-number": "Ebarzhit un takad anvio\u00f9 dre e niverenn",
     "pywikibot-enter-new-text": "Ebarzhit an destenn nevez, mar plij:",
     "pywikibot-enter-page-processing": "Gant peseurt pajenn e ranker pledi\u00f1 ?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/bs.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/bs.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Robot:'"}*

```diff
@@ -4,14 +4,15 @@
             "CERminator",
             "Edinwiki",
             "KWiki",
             "Srdjan m",
             "Sr\u0111an"
         ]
     },
+    "pywikibot-bot-prefix": "Robot:",
     "pywikibot-cosmetic-changes": "; kozmeti\u010dke promjene",
     "pywikibot-enter-category-name": "Unesite naziv kategorije:",
     "pywikibot-enter-file-links-processing": "Veze prema kojoj stranici da se obrade?",
     "pywikibot-enter-finished-browser": "Pritisnite \"Enter\" kada zavr\u0161ite u pregledniku.",
     "pywikibot-enter-namespace-number": "Unesite broj imenskog prostora:",
     "pywikibot-enter-new-text": "Unesite novi tekst:",
     "pywikibot-enter-page-processing": "Koja bi stranica trebala biti obra\u0111ena?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ca.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ca.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Bot:'"}*

```diff
@@ -9,14 +9,15 @@
             "Mguix",
             "Pitort",
             "SMP",
             "Toniher",
             "XVEC"
         ]
     },
+    "pywikibot-bot-prefix": "Bot:",
     "pywikibot-cosmetic-changes": "; canvis est\u00e8tics",
     "pywikibot-enter-category-name": "Si us plau introdueix el nom de la categoria :",
     "pywikibot-enter-file-links-processing": "Els enlla\u00e7os a quina p\u00e0gina del fitxer s'haurien de processar?",
     "pywikibot-enter-finished-browser": "Premeu Retorn quan h\u00e0giu acabat amb el navegador.",
     "pywikibot-enter-namespace-number": "Introdu\u00efu un espai de noms pel seu n\u00famero:",
     "pywikibot-enter-new-text": "Si us plau, introdu\u00efu el nou text:",
     "pywikibot-enter-page-processing": "Quina p\u00e0gina ha de ser processada?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ce.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ce.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9090909090909091%*

 * *Differences: {"'pywikibot-bot-prefix'": "'бот:'"}*

```diff
@@ -1,13 +1,14 @@
 {
     "@metadata": {
         "authors": [
             "\u0423\u043c\u0430\u0440"
         ]
     },
+    "pywikibot-bot-prefix": "\u0431\u043e\u0442:",
     "pywikibot-cosmetic-changes": "; \u043a\u043e\u0441\u043c\u0435\u0442\u0438\u043a\u0438\u0439\u043d \u0445\u0438\u0439\u0446\u0430\u043c",
     "pywikibot-enter-category-name": "\u0414\u0435\u0445\u0430\u0440 \u0434\u043e, \u0434\u04c0\u0430\u0439\u0430\u0437\u0439\u0435 \u043a\u0430\u0442\u0435\u0433\u043e\u0440\u0438\u043d \u0446\u04c0\u0435:",
     "pywikibot-enter-file-links-processing": "\u041c\u0443\u044c\u043b\u0445\u0430\u0447\u0443 \u0444\u0430\u0439\u043b\u0430\u043d \u0445\u044c\u0430\u0436\u043e\u0440\u0433\u0430\u0448 \u043a\u0435\u0447\u0439\u0430\u043d \u0439\u0435\u0437\u0430\u0448 \u0439\u0443?",
     "pywikibot-enter-finished-browser": "\u0411\u0440\u0430\u0443\u0437\u0435\u0440 \u0447\u043e\u0445\u044c \u0445\u0438\u0439\u0446\u0430\u043c \u0431\u0438\u043d\u0447\u0443\u043b\u0442\u04c0\u0435\u0445\u044c\u0430 \u0442\u0430\u04c0\u0430\u0435 Enter.",
     "pywikibot-enter-namespace-number": "\u0414\u0435\u0445\u0430\u0440 \u0434\u043e, \u0446\u04c0\u0435\u0440\u0438\u0439\u043d \u043c\u0435\u0442\u0442\u0438\u0438\u0433\u0438\u0439\u043d \u043b\u043e\u044c\u043c\u0430\u0440 \u0439\u0430\u0437\u0439\u0435:",
     "pywikibot-enter-new-text": "\u0414\u0435\u0445\u0430\u0440 \u0434\u043e, \u043a\u0435\u0440\u043b\u0430 \u0439\u043e\u0437\u0430 \u0439\u0430\u0437\u0434\u0435:",
     "pywikibot-enter-page-processing": "\u041c\u0443\u044c\u043b\u0445\u0430 \u0430\u0433\u04c0\u043e \u043a\u0435\u0447\u0439\u0430\u043d \u0439\u0435\u0437\u0430\u0448 \u0439\u0443?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ckb.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ckb.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8888888888888888%*

 * *Differences: {"'pywikibot-bot-prefix'": "'بۆت:'"}*

```diff
@@ -2,14 +2,15 @@
     "@metadata": {
         "authors": [
             "Aram",
             "Asoxor",
             "\u0626\u0627\u0631\u0627\u0645 \u0628\u06a9\u0631"
         ]
     },
+    "pywikibot-bot-prefix": "\u0628\u06c6\u062a:",
     "pywikibot-cosmetic-changes": "\u061b \u062f\u06d5\u0633\u062a\u06a9\u0627\u0631\u06cc\u06cc \u062c\u0648\u0627\u0646\u06a9\u0627\u0631\u06cc",
     "pywikibot-enter-category-name": "\u062a\u06a9\u0627\u06cc\u06d5 \u0646\u0627\u0648\u06cc \u067e\u06c6\u0644\u06d5\u06a9\u06d5 \u0628\u0646\u0648\u0648\u0633\u06d5:",
     "pywikibot-enter-finished-browser": "\u06a9\u0627\u062a\u06ce\u06a9 \u0644\u06d5 \u0648\u06ce\u0628\u06af\u06d5\u0695\u06d5\u06a9\u06d5 \u062a\u06d5\u0648\u0627\u0648 \u0628\u0648\u0648\u060c \u0626\u06cc\u0646\u062a\u06d5\u0631 \u062f\u0627\u06af\u0631\u06d5.",
     "pywikibot-enter-new-text": "\u062a\u06a9\u0627\u06cc\u06d5 \u062f\u06d5\u0642\u06d5 \u0646\u0648\u06ce\u06cc\u06d5\u06a9\u06d5 \u062f\u0627\u062e\u0644 \u0628\u06a9\u06d5:",
     "pywikibot-fixes-html": "\u0628\u06c6\u062a: \u06af\u06c6\u0695\u06cc\u0646\u06cc/\u0686\u0627\u06a9\u06a9\u0631\u062f\u0646\u06cc \u0626\u06d5\u06cc\u0686 \u062a\u06cc \u0626\u06ce\u0645 \u0626\u06ce\u06b5",
     "pywikibot-fixes-isbn": "\u0628\u06c6\u062a: \u0695\u0627\u0633\u062a\u06a9\u0631\u062f\u0646\u06d5\u0648\u06d5\u06cc \u0634\u06ce\u0648\u0627\u0632\u06cc ISBN",
     "pywikibot-fixes-syntax": "\u0628\u06c6\u062a: \u0686\u0627\u06a9\u06a9\u0631\u062f\u0646\u06cc \u0634\u06ce\u0648\u0627\u0632\u06cc \u0646\u0648\u0648\u0633\u06cc\u0646\u06cc \u0648\u06cc\u06a9\u06cc"
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/cs.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/cs.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'robot:'"}*

```diff
@@ -8,14 +8,15 @@
             "Mat\u011bj Such\u00e1nek",
             "Mormegil",
             "Patriccck",
             "Patrik L.",
             "Tcho\u0159"
         ]
     },
+    "pywikibot-bot-prefix": "robot:",
     "pywikibot-cosmetic-changes": "; kosmetick\u00e9 \u00fapravy",
     "pywikibot-enter-category-name": "Pros\u00edm, zadejte jm\u00e9no kategorie:",
     "pywikibot-enter-file-links-processing": "Odkazy na kterou str\u00e1nku se souborem maj\u00ed b\u00fdt zpracov\u00e1ny?",
     "pywikibot-enter-finished-browser": "Po ukon\u010den\u00ed pr\u00e1ce v prohl\u00ed\u017ee\u010di zm\u00e1\u010dkn\u011bte Enter.",
     "pywikibot-enter-namespace-number": "Pros\u00edm, zadejte \u010d\u00edslo jmenn\u00e9ho prostoru:",
     "pywikibot-enter-new-text": "Pros\u00edm zadejte nov\u00fd text:",
     "pywikibot-enter-page-processing": "Kter\u00e1 str\u00e1nka m\u00e1 b\u00fdt zpracov\u00e1na?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/csb.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/csb.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Bòt:'"}*

```diff
@@ -1,13 +1,14 @@
 {
     "@metadata": {
         "authors": [
             "Kaszeba"
         ]
     },
+    "pywikibot-bot-prefix": "B\u00f2t:",
     "pywikibot-cosmetic-changes": "; k\u00f2smeticzn\u00e9 zmian\u00eb",
     "pywikibot-enter-category-name": "Wpisz\u00eb miono kateg\u00f2r\u00ebji",
     "pywikibot-enter-file-links-processing": "L\u00ebnczi do starn\u00eb cht\u00ebrneg\u00f2 lopka maj\u0105 b\u00ebc przerobione?",
     "pywikibot-enter-finished-browser": "Wc\u00ebsni Enter jak przez\u00e9rnik \u00f2przestanie robic.",
     "pywikibot-enter-namespace-number": "Prosz\u00e3 wpisac numer ruma mion\u00f3w:",
     "pywikibot-enter-new-text": "Prosz\u00e3 wpisac nowi tekst:",
     "pywikibot-enter-page-processing": "Jak\u00f4 strana m\u00f4 b\u00ebc przerobion\u00f4?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/cy.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/hsb.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.38636363636363635%*

 * *Differences: {"'@metadata'": "{'authors': ['Michawiki']}",*

 * * "'pywikibot-bot-prefix'": "'Boćik:'",*

 * * "'pywikibot-cosmetic-changes'": "'; kosmetiske změny'",*

 * * "'pywikibot-enter-category-name'": "'Prošu zapodaj mjeno kategorije:'",*

 * * "'pywikibot-enter-finished-browser'": "'Tłóč zapodawansku tastu po skónčenju wobhladowaka.'",*

 * * "'pywikibot-enter-namespace-number'": "'Prošu zapodaj čisło mjenoweho ruma:'",*

 * * "'pywikibot-enter-new-text'": "'Proš zapodaj nowy tekst:'",*

 * * "'pywikibot-enter-page-processing'": "'Kotra strona ma so př […]*

```diff
@@ -1,18 +1,15 @@
 {
     "@metadata": {
         "authors": [
-            "Lloffiwr",
-            "Robin Owain",
-            "Xxglennxx"
+            "Michawiki"
         ]
     },
-    "pywikibot-cosmetic-changes": "; Newidiadau i ymddangosiad y dudalen",
-    "pywikibot-enter-category-name": "Nodwch enw'r categori:",
-    "pywikibot-enter-file-links-processing": "I ba dudalen ffeil y dylid prosesu'r dolenni?",
-    "pywikibot-enter-finished-browser": "Pwyswch Enter ar \u00f4l gorffen pori.",
-    "pywikibot-enter-namespace-number": "Nodwch rif y \"namespace\"",
-    "pywikibot-enter-new-text": "Nodwch y testun newydd",
-    "pywikibot-enter-page-processing": "Pa dudalen ddylem ei phrosesu?",
-    "pywikibot-enter-xml-filename": "Nodwch enwffeil y gronfa XML",
-    "pywikibot-fixes-isbn": "Robot: Yn fformatio'r rhif ISBN"
+    "pywikibot-bot-prefix": "Bo\u0107ik:",
+    "pywikibot-cosmetic-changes": "; kosmetiske zm\u011bny",
+    "pywikibot-enter-category-name": "Pro\u0161u zapodaj mjeno kategorije:",
+    "pywikibot-enter-finished-browser": "T\u0142\u00f3\u010d zapodawansku tastu po sk\u00f3n\u010denju wobhladowaka.",
+    "pywikibot-enter-namespace-number": "Pro\u0161u zapodaj \u010dis\u0142o mjenoweho ruma:",
+    "pywikibot-enter-new-text": "Pro\u0161 zapodaj nowy tekst:",
+    "pywikibot-enter-page-processing": "Kotra strona ma so p\u0159ed\u017a\u011b\u0142a\u0107?",
+    "pywikibot-fixes-isbn": "Bo\u0107ik: ISBN so formatuje"
 }
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/da.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/da.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Robot:'"}*

```diff
@@ -5,14 +5,15 @@
             "Joedalton",
             "Kaare",
             "MGA73",
             "Peter Alberti",
             "Steenth"
         ]
     },
+    "pywikibot-bot-prefix": "Robot:",
     "pywikibot-cosmetic-changes": "; kosmetiske \u00e6ndringer",
     "pywikibot-enter-category-name": "Skriv kategorinavnet:",
     "pywikibot-enter-file-links-processing": "Links til hvilken fil side der skal behandles?",
     "pywikibot-enter-finished-browser": "Tryk Enter n\u00e5r browserredigeringerne er f\u00e6rdige.",
     "pywikibot-enter-namespace-number": "Angiv et navnerum via dets nummer:",
     "pywikibot-enter-new-text": "Skriv den nye tekst:",
     "pywikibot-enter-page-processing": "Hvilken side skal behandles?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/de.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/de.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Bot:'"}*

```diff
@@ -3,14 +3,15 @@
         "authors": [
             "Daniel Herding",
             "Metalhead64",
             "Se4598",
             "Xqt"
         ]
     },
+    "pywikibot-bot-prefix": "Bot:",
     "pywikibot-cosmetic-changes": "; kosmetische \u00c4nderungen",
     "pywikibot-enter-category-name": "Bitte Name der Kategorie eingeben:",
     "pywikibot-enter-file-links-processing": "Links zu welcher Dateiseite sollen bearbeitet werden?",
     "pywikibot-enter-finished-browser": "Enter dr\u00fccken nach dem Beenden des Browsers.",
     "pywikibot-enter-namespace-number": "Bitte gib die Nummer des Namensraums ein:",
     "pywikibot-enter-new-text": "Bitte gib den neuen Text ein:",
     "pywikibot-enter-page-processing": "Welche Seite soll bearbeitet werden?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/diq.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/diq.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Bot:'"}*

```diff
@@ -3,14 +3,15 @@
         "authors": [
             "Erdemaslancan",
             "G\u0131rd",
             "Kumkumuk",
             "Mirzali"
         ]
     },
+    "pywikibot-bot-prefix": "Bot:",
     "pywikibot-cosmetic-changes": "; kozmetik vurnay\u0131\u015fi",
     "pywikibot-enter-category-name": "Namey\u00ea kategoriye c\u0131 kew\u00ea:",
     "pywikibot-enter-file-links-processing": "G\u0131rey\u00ea kamci pela res\u0131man wa b\u0131gureniyo?",
     "pywikibot-enter-finished-browser": "C\u0131geyrayo\u011fi de ke qediya gocega enteri b\u0131t\u0131kne",
     "pywikibot-enter-namespace-number": "Numrey\u00ea c\u0131 ra yew name c\u0131 kew\u00ea:",
     "pywikibot-enter-new-text": "Nu\u015ftey\u00ea newey c\u0131 kew\u00ea:",
     "pywikibot-enter-page-processing": "Kamci pele wa b\u0131nu\u015fiyo?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/el.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/el.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Ρομπότ:'"}*

```diff
@@ -4,14 +4,15 @@
             "Evropi",
             "Geraki",
             "GhotuoIncubator",
             "Glavkos",
             "Protnet"
         ]
     },
+    "pywikibot-bot-prefix": "\u03a1\u03bf\u03bc\u03c0\u03cc\u03c4:",
     "pywikibot-cosmetic-changes": ".",
     "pywikibot-enter-category-name": "\u03a0\u03b1\u03c1\u03b1\u03ba\u03b1\u03bb\u03bf\u03cd\u03bc\u03b5 \u03b5\u03b9\u03c3\u03b1\u03b3\u03ac\u03b3\u03b5\u03c4\u03b5 \u03c4\u03bf \u03cc\u03bd\u03bf\u03bc\u03b1 \u03c4\u03b7\u03c2 \u03ba\u03b1\u03c4\u03b7\u03b3\u03bf\u03c1\u03af\u03b1\u03c2:",
     "pywikibot-enter-file-links-processing": "\u03a3\u03c5\u03bd\u03b4\u03ad\u03c3\u03b5\u03b9\u03c2 \u03c0\u03c1\u03bf\u03c2 \u03c0\u03bf\u03b9\u03b1 \u03c3\u03b5\u03bb\u03af\u03b4\u03b1 \u03b1\u03c1\u03c7\u03b5\u03af\u03bf\u03c5 \u03bd\u03b1 \u03c5\u03c0\u03bf\u03b2\u03bb\u03b7\u03b8\u03bf\u03cd\u03bd \u03c3\u03b5 \u03b5\u03c0\u03b5\u03be\u03b5\u03c1\u03b3\u03b1\u03c3\u03af\u03b1;",
     "pywikibot-enter-finished-browser": "\u03a0\u03b9\u03ad\u03c3\u03c4\u03b5 \u03c4\u03bf \u03c0\u03bb\u03ae\u03ba\u03c4\u03c1\u03bf Enter, \u03cc\u03c4\u03b1\u03bd \u03c4\u03b5\u03bb\u03b5\u03b9\u03ce\u03c3\u03b5\u03b9 \u03c3\u03c4\u03bf \u03c0\u03c1\u03cc\u03b3\u03c1\u03b1\u03bc\u03bc\u03b1 \u03c0\u03b5\u03c1\u03b9\u03ae\u03b3\u03b7\u03c3\u03b7\u03c2.",
     "pywikibot-enter-namespace-number": "\u03a0\u03b1\u03c1\u03b1\u03ba\u03b1\u03bb\u03bf\u03cd\u03bc\u03b5 \u03b5\u03b9\u03c3\u03b1\u03b3\u03ac\u03b3\u03b5\u03c4\u03b5 \u03bf\u03bd\u03bf\u03bc\u03b1\u03c4\u03bf\u03c7\u03ce\u03c1\u03bf \u03bc\u03ad\u03c3\u03c9 \u03c4\u03bf\u03c5 \u03b1\u03c1\u03b9\u03b8\u03bc\u03bf\u03cd \u03c4\u03bf\u03c5:",
     "pywikibot-enter-new-text": "\u03a0\u03b1\u03c1\u03b1\u03ba\u03b1\u03bb\u03bf\u03cd\u03bc\u03b5 \u03c0\u03bb\u03b7\u03ba\u03c4\u03c1\u03bf\u03bb\u03bf\u03b3\u03ae\u03c3\u03c4\u03b5 \u03c4\u03bf \u03bd\u03ad\u03bf \u03ba\u03b5\u03af\u03bc\u03b5\u03bd\u03bf:",
     "pywikibot-enter-page-processing": "\u03a0\u03bf\u03b9\u03b1 \u03c3\u03b5\u03bb\u03af\u03b4\u03b1 \u03bd\u03b1 \u03c5\u03c0\u03bf\u03b2\u03bb\u03b7\u03b8\u03b5\u03af \u03c3\u03b5 \u03b5\u03c0\u03b5\u03be\u03b5\u03c1\u03b3\u03b1\u03c3\u03af\u03b1;",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/en.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/en.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Bot:'"}*

```diff
@@ -5,14 +5,15 @@
             "Huji",
             "Siebrand",
             "Revi",
             "Russell Blau",
             "Xqt"
         ]
     },
+    "pywikibot-bot-prefix": "Bot:",
     "pywikibot-cosmetic-changes": "; cosmetic changes",
     "pywikibot-enter-category-name": "Please enter the category name:",
     "pywikibot-enter-file-links-processing": "Links to which file page should be processed?",
     "pywikibot-enter-finished-browser": "Press Enter when finished in browser.",
     "pywikibot-enter-namespace-number": "Please enter a namespace by its number:",
     "pywikibot-enter-new-text": "Please enter the new text:",
     "pywikibot-enter-page-processing": "Which page should be processed?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/eo.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/eo.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Roboto:'"}*

```diff
@@ -6,14 +6,15 @@
             "KuboF",
             "Mihxil",
             "Mirin",
             "Objectivesea",
             "Remux"
         ]
     },
+    "pywikibot-bot-prefix": "Roboto:",
     "pywikibot-cosmetic-changes": "; kosmetikaj \u015dan\u011doj",
     "pywikibot-enter-category-name": "Bonvolu enmeti la nomon de kategorio:",
     "pywikibot-enter-file-links-processing": "Ligiloj al kiu dosieropa\u011do estu prilaboritaj?",
     "pywikibot-enter-finished-browser": "Post laborfino en la retumilo, premu Enter.",
     "pywikibot-enter-namespace-number": "Bonvolu enmeti nomspacon per ties numero:",
     "pywikibot-enter-new-text": "Bonvolu enmeti la novan tekston:",
     "pywikibot-enter-page-processing": "Kiu pa\u011do estu prilaborita?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/es.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/es.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Robot:'"}*

```diff
@@ -9,14 +9,15 @@
             "Josuert",
             "Macofe",
             "MarcoAurelio",
             "Ovruni",
             "Xqt"
         ]
     },
+    "pywikibot-bot-prefix": "Robot:",
     "pywikibot-cosmetic-changes": "; cambios superficiales",
     "pywikibot-enter-category-name": "Escribe el nombre de la categor\u00eda:",
     "pywikibot-enter-file-links-processing": "\u00bfA qu\u00e9 p\u00e1gina de archivo se deben procesar los enlaces?",
     "pywikibot-enter-finished-browser": "Presiona la tecla Enter cuando termine en el navegador.",
     "pywikibot-enter-namespace-number": "Escribe un espacio de nombres seg\u00fan su n\u00famero:",
     "pywikibot-enter-new-text": "Escribe el texto nuevo:",
     "pywikibot-enter-page-processing": "\u00bfQu\u00e9 p\u00e1gina se debe procesar?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/eu.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/eu.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Bot:'"}*

```diff
@@ -3,14 +3,15 @@
         "authors": [
             "An13sa",
             "EukeneFL",
             "Subi",
             "Xabier Armendaritz"
         ]
     },
+    "pywikibot-bot-prefix": "Bot:",
     "pywikibot-cosmetic-changes": "; aldaketa kosmetikoak",
     "pywikibot-enter-category-name": "Mesedez, sar ezazu kategoriaren izena:",
     "pywikibot-enter-file-links-processing": "Zer fitxategirako linkak prozesatu beharko lirateke?",
     "pywikibot-enter-finished-browser": "Arakatzailearekin amaitu eta gero sakatu ENTER",
     "pywikibot-enter-namespace-number": "Mesedez idatzi izen-espazioa bere zenbakiarekin batera:",
     "pywikibot-enter-new-text": "Mesedez, sar ezazu testu berria:",
     "pywikibot-enter-page-processing": "Zein orrialde prozesatu behar da?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/fa.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/fa.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'ربات::'"}*

```diff
@@ -6,14 +6,15 @@
             "Huji",
             "Ladsgroup",
             "Mjbmr",
             "Reza1615",
             "ZxxZxxZ"
         ]
     },
+    "pywikibot-bot-prefix": "\u0631\u0628\u0627\u062a::",
     "pywikibot-cosmetic-changes": "\u061b \u0632\u06cc\u0628\u0627\u0633\u0627\u0632\u06cc",
     "pywikibot-enter-category-name": "\u0644\u0637\u0641\u0627\u064b \u0646\u0627\u0645 \u0631\u062f\u0647 \u0631\u0627 \u0648\u0627\u0631\u062f \u06a9\u0646\u06cc\u062f:",
     "pywikibot-enter-file-links-processing": "\u067e\u06cc\u0648\u0646\u062f \u0628\u0647 \u06a9\u062f\u0627\u0645 \u067e\u0631\u0648\u0646\u062f\u0647 \u0628\u0627\u06cc\u062f \u067e\u0631\u062f\u0627\u0632\u0634 \u0634\u0648\u062f\u061f",
     "pywikibot-enter-finished-browser": "\u0647\u0646\u06af\u0627\u0645\u06cc \u06a9\u0647 \u062f\u0631 \u0645\u0631\u0648\u0631\u06af\u0631 \u067e\u0627\u06cc\u0627\u0646 \u06cc\u0627\u0641\u062a \u062f\u06a9\u0645\u0647\u0654 \u0627\u06cc\u0646\u062a\u0631 \u0631\u0627 \u0628\u0641\u0634\u0627\u0631\u06cc\u062f.",
     "pywikibot-enter-namespace-number": "\u0644\u0637\u0641\u0627\u064b \u0634\u0645\u0627\u0631\u0647\u0654 \u06cc\u06a9 \u0641\u0636\u0627\u06cc \u0646\u0627\u0645 \u0631\u0627 \u0648\u0627\u0631\u062f \u06a9\u0646\u06cc\u062f:",
     "pywikibot-enter-new-text": "\u0644\u0637\u0641\u0627\u064b \u0645\u062a\u0646 \u062c\u062f\u06cc\u062f \u0631\u0627 \u0648\u0627\u0631\u062f \u06a9\u0646\u06cc\u062f:",
     "pywikibot-enter-page-processing": "\u06a9\u062f\u0627\u0645 \u0635\u0641\u062d\u0647 \u0628\u0627\u06cc\u062f \u067e\u0631\u062f\u0627\u0632\u0634 \u0634\u0648\u062f\u061f",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/fi.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/fi.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/fo.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/fo.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9090909090909091%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Bottur:'"}*

```diff
@@ -1,13 +1,14 @@
 {
     "@metadata": {
         "authors": [
             "EileenSanda"
         ]
     },
+    "pywikibot-bot-prefix": "Bottur:",
     "pywikibot-cosmetic-changes": "; broytingar av \u00fatsj\u00f3nd",
     "pywikibot-enter-category-name": "Vinarliga skriva b\u00f3lkanavni\u00f0:",
     "pywikibot-enter-file-links-processing": "Sl\u00f3\u00f0ir til hv\u00f8rja f\u00edlus\u00ed\u00f0u skulu vi\u00f0gerast?",
     "pywikibot-enter-finished-browser": "Tr\u00fdst \u00e1 Enter t\u00e1 t\u00fa ert li\u00f0ug/ur at r\u00e6tta \u00ed brovsaranum.",
     "pywikibot-enter-namespace-number": "Vinarliga skriva eitt navnar\u00fam vi\u00f0 tilhoyrandi nummari:",
     "pywikibot-enter-new-text": "Vinarliga skriva n\u00fdggja tekstin:",
     "pywikibot-enter-page-processing": "Hv\u00f8r s\u00ed\u00f0a skal vi\u00f0gerast?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/fr.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/fr.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Robot\\u202f:'"}*

```diff
@@ -9,14 +9,15 @@
             "Tavernier",
             "Thibaut120094",
             "Urhixidur",
             "Verdy p",
             "Wladek92"
         ]
     },
+    "pywikibot-bot-prefix": "Robot\u202f:",
     "pywikibot-cosmetic-changes": "; changements cosm\u00e9tiques",
     "pywikibot-enter-category-name": "Veuillez saisir le nom de la cat\u00e9gorie\u202f:",
     "pywikibot-enter-file-links-processing": "Liens vers la page de fichier qu\u2019il faudrait traiter\u202f?",
     "pywikibot-enter-finished-browser": "Appuyez sur Entr\u00e9e une fois que vous avez fini dans le navigateur.",
     "pywikibot-enter-namespace-number": "Veuillez entrer un espace de noms par son num\u00e9ro\u202f:",
     "pywikibot-enter-new-text": "Veuillez entrer le nouveau texte\u202f:",
     "pywikibot-enter-page-processing": "Quelle page faut-il traiter\u202f?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/frr.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/frr.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Bot:'"}*

```diff
@@ -1,13 +1,14 @@
 {
     "@metadata": {
         "authors": [
             "Murma174"
         ]
     },
+    "pywikibot-bot-prefix": "Bot:",
     "pywikibot-cosmetic-changes": "; kosmeetisk feranrangen",
     "pywikibot-enter-category-name": "Du di n\u00f6\u00f6m faan det kategorii iin:",
     "pywikibot-enter-file-links-processing": "Faan h\u00fck datei-sidj skel a widjerfeerangen bewerket wurd?",
     "pywikibot-enter-finished-browser": "Trak Enter, wan di browser klaar as.",
     "pywikibot-enter-namespace-number": "Du det numer faan di n\u00f6\u00f6mr\u00fcm iin:",
     "pywikibot-enter-new-text": "Du di nei tekst iin:",
     "pywikibot-enter-page-processing": "H\u00fcn sidj skal bewerket wurd?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/gl.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/gl.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Robot:'"}*

```diff
@@ -2,14 +2,15 @@
     "@metadata": {
         "authors": [
             "Banjo",
             "Gallaecio",
             "Toli\u00f1o"
         ]
     },
+    "pywikibot-bot-prefix": "Robot:",
     "pywikibot-cosmetic-changes": "; cambios est\u00e9tica",
     "pywikibot-enter-category-name": "Insira o nome da categor\u00eda:",
     "pywikibot-enter-file-links-processing": "As ligaz\u00f3ns a que p\u00e1xina de ficheiro se deben procesar?",
     "pywikibot-enter-finished-browser": "Prema na tecla \"Intro\" cando remate no navegador.",
     "pywikibot-enter-namespace-number": "Insira un espazo de nomes segundo o seu n\u00famero:",
     "pywikibot-enter-new-text": "Insira o novo texto:",
     "pywikibot-enter-page-processing": "Que p\u00e1xina se debe procesar?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/gsw.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/gsw.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9090909090909091%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Bot:'"}*

```diff
@@ -1,14 +1,15 @@
 {
     "@metadata": {
         "authors": [
             "Als-Chl\u00e4mens",
             "Als-Holder"
         ]
     },
+    "pywikibot-bot-prefix": "Bot:",
     "pywikibot-cosmetic-changes": "; oberfl\u00e4chlichi \u00c4nderige",
     "pywikibot-enter-category-name": "Bitte gib dr Name vu dr Kategori yy:",
     "pywikibot-enter-file-links-processing": "Vu wellere Dateisyte solle d Link bearbeitet w\u00e4re?",
     "pywikibot-enter-finished-browser": "Druck noch eme Zuemache vum Browsewr uf \u00abEnter\u00bb.",
     "pywikibot-enter-namespace-number": "Bitte gib d Nummere vum Namensruum yy:",
     "pywikibot-enter-new-text": "Bitte gib dr nei Text yy:",
     "pywikibot-enter-page-processing": "Weli Syte soll bearbeitet w\u00e4re?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/hak.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/hak.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9090909090909091%*

 * *Differences: {"'pywikibot-bot-prefix'": "'機械人：'"}*

```diff
@@ -1,14 +1,15 @@
 {
     "@metadata": {
         "authors": [
             "EagerLin",
             "Jetlag"
         ]
     },
+    "pywikibot-bot-prefix": "\u6a5f\u68b0\u4eba\uff1a",
     "pywikibot-cosmetic-changes": ";\u6574\u6f54\u5316\u66f4\u6539",
     "pywikibot-enter-category-name": "\u8acb\u8f38\u5165\u5206\u985e\u540d\u7a31\uff1a",
     "pywikibot-enter-file-links-processing": "\u54ea\u96bb\u5716\u50cf\u4e2a\u9023\u63a5\u9700\u8981\u8655\u7406\uff1f",
     "pywikibot-enter-finished-browser": "\u641e\u6382\u5f8c\u8acb\u64b3\u4e0bEnter\u9375\u3002",
     "pywikibot-enter-namespace-number": "\u8acb\u8f38\u5165\u540d\u5b57\u7a7a\u9593\u7de8\u865f\uff1a",
     "pywikibot-enter-new-text": "\u8acb\u8f38\u5165\u65b0\u6587\u5b57\uff1a",
     "pywikibot-enter-page-processing": "\u54ea\u96bb\u9801\u9762\u9700\u8981\u8655\u7406\uff1f",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/haw.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/haw.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9090909090909091%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Lopako:'"}*

```diff
@@ -1,13 +1,14 @@
 {
     "@metadata": {
         "authors": [
             "Kolonahe"
         ]
     },
+    "pywikibot-bot-prefix": "Lopako:",
     "pywikibot-cosmetic-changes": "; n\u0101 ho\u02bbololi helehelena",
     "pywikibot-enter-category-name": "E \u02bbolu\u02bbolu, e kikokiko i ka inoa mahele:",
     "pywikibot-enter-file-links-processing": "Ha\u02bbaliu i ka loulou i ka \u02bbao\u02bbao waihona hea?",
     "pywikibot-enter-finished-browser": "E komi i ke k\u0101ho\u02bbi i ka hana pau \u02bbana o ke p\u014dlamu p\u016bnaewele.",
     "pywikibot-enter-namespace-number": "E \u02bbolu\u02bbolu, e kikokiko i kekahi lewainoa kokoke i k\u0101na helu:",
     "pywikibot-enter-new-text": "E \u02bbolu\u02bbolu, e kikokiko i ke kikokikona hou:",
     "pywikibot-enter-page-processing": "Ha\u02bbaliu ka \u02bbao\u02bbao hea?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/he.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/he.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'בוט:'"}*

```diff
@@ -3,14 +3,15 @@
         "authors": [
             "Amire80",
             "Leonardo Gregianin",
             "Or",
             "YaronSh"
         ]
     },
+    "pywikibot-bot-prefix": "\u05d1\u05d5\u05d8:",
     "pywikibot-cosmetic-changes": "; \u05e9\u05d9\u05e0\u05d5\u05d9\u05d9\u05dd \u05e7\u05d5\u05e1\u05de\u05d8\u05d9\u05d9\u05dd",
     "pywikibot-enter-category-name": "\u05e0\u05d0 \u05dc\u05d4\u05d6\u05d9\u05df \u05d0\u05ea \u05e9\u05dd \u05d4\u05e7\u05d8\u05d2\u05d5\u05e8\u05d9\u05d4:",
     "pywikibot-enter-file-links-processing": "\u05e7\u05d9\u05e9\u05d5\u05e8\u05d9\u05dd \u05dc\u05d0\u05d9\u05d6\u05d4 \u05d3\u05e3 \u05e7\u05d5\u05d1\u05e5 \u05d9\u05e9 \u05dc\u05e2\u05d1\u05d3?",
     "pywikibot-enter-finished-browser": "\u05d9\u05e9 \u05dc\u05dc\u05d7\u05d5\u05e5 Enter \u05db\u05d0\u05e9\u05e8 \u05de\u05e1\u05ea\u05d9\u05d9\u05de\u05ea \u05d4\u05e4\u05e2\u05d5\u05dc\u05d4 \u05d1\u05d3\u05e4\u05d3\u05e4\u05df.",
     "pywikibot-enter-namespace-number": "\u05e0\u05d0 \u05dc\u05d4\u05d6\u05d9\u05df \u05d0\u05ea \u05e9\u05dd \u05de\u05e8\u05d7\u05d1 \u05d4\u05e9\u05dd \u05dc\u05e4\u05d9 \u05d4\u05de\u05e1\u05e4\u05e8 \u05e9\u05dc\u05d5:",
     "pywikibot-enter-new-text": "\u05e0\u05d0 \u05dc\u05d4\u05d6\u05d9\u05df \u05d0\u05ea \u05d4\u05d8\u05e7\u05e1\u05d8 \u05d4\u05d7\u05d3\u05e9:",
     "pywikibot-enter-page-processing": "\u05d0\u05d9\u05d6\u05d4 \u05d3\u05e3 \u05d9\u05e9 \u05dc\u05e2\u05d1\u05d3?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/hi.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/hi.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'pywikibot-bot-prefix'": "'बॉट:'"}*

```diff
@@ -1,14 +1,15 @@
 {
     "@metadata": {
         "authors": [
             "Siddhartha Ghai",
             "\u0938\u0902\u091c\u0940\u0935 \u0915\u0941\u092e\u093e\u0930"
         ]
     },
+    "pywikibot-bot-prefix": "\u092c\u0949\u091f:",
     "pywikibot-cosmetic-changes": "; \u090a\u092a\u0930\u0940 \u092a\u0930\u093f\u0935\u0930\u094d\u0924\u0928",
     "pywikibot-enter-category-name": "\u0915\u0943\u092a\u092f\u093e \u0936\u094d\u0930\u0947\u0923\u0940 \u0915\u093e \u0928\u093e\u092e \u0932\u093f\u0916\u0947\u0902:",
     "pywikibot-enter-file-links-processing": "\u0915\u094c\u0928\u0938\u093e \u092b\u093e\u0907\u0932 \u092a\u0943\u0937\u094d\u0920 \u0938\u0902\u0936\u094b\u0927\u093f\u0924 \u0939\u094b\u0928\u093e \u091a\u093e\u0939\u093f\u090f \u0915\u0940 \u0915\u0921\u093c\u0940 \u091c\u094b\u0921\u093c\u0924\u093e \u0939\u0948?",
     "pywikibot-enter-finished-browser": "\u091c\u092c \u092c\u094d\u0930\u093e\u0909\u091c\u0930 \u092e\u0947\u0902 \u0938\u092e\u093e\u092a\u094d\u0924 \u0939\u094b \u091c\u093e\u092f\u0947 \u0924\u092c \u090f\u0902\u091f\u0930 \u092c\u091f\u0928 \u0926\u092c\u093e\u092f\u0947\u0902\u0964",
     "pywikibot-enter-namespace-number": "\u0915\u0943\u092a\u092f\u093e \u0938\u092e\u094d\u092c\u0902\u0927\u093f\u0924 \u0938\u0902\u0916\u094d\u092f\u093e \u0926\u094d\u0935\u093e\u0930\u093e \u0928\u093e\u092e\u0938\u094d\u0925\u093e\u0928 \u0932\u093f\u0916\u0947\u0902:",
     "pywikibot-enter-new-text": "\u0915\u0943\u092a\u092f\u093e \u0928\u092f\u093e \u092a\u093e\u0920 \u0921\u093e\u0932\u0947\u0902:",
     "pywikibot-enter-page-processing": "\u0915\u094c\u0928 \u0938\u093e \u092a\u0943\u0937\u094d\u0920 \u092a\u094d\u0930\u0915\u094d\u0930\u092e\u0923\u093f\u0924 \u0915\u093f\u092f\u093e \u091c\u093e\u0928\u093e \u091a\u093e\u0939\u093f\u090f?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/hsb.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sh.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4166666666666667%*

 * *Differences: {"'@metadata'": "{'authors': ['Kolega2357']}",*

 * * "'pywikibot-cosmetic-changes'": "'; kozmetičke izmjene'",*

 * * "'pywikibot-enter-category-name'": "'Unesite naziv kategorije:'",*

 * * "'pywikibot-enter-finished-browser'": "'Pritisnite enter kada završite u pregledaču.'",*

 * * "'pywikibot-enter-namespace-number'": "'Unesite imenski prostor pored njegovog broja:'",*

 * * "'pywikibot-enter-new-text'": "'Unesite novi tekst:'",*

 * * "'pywikibot-enter-page-processing'": "'Koja stranica treba da se obradi?'",*

 * * "'pywikibot-enter-xml-file […]*

```diff
@@ -1,14 +1,14 @@
 {
     "@metadata": {
         "authors": [
-            "Michawiki"
+            "Kolega2357"
         ]
     },
-    "pywikibot-cosmetic-changes": "; kosmetiske zm\u011bny",
-    "pywikibot-enter-category-name": "Pro\u0161u zapodaj mjeno kategorije:",
-    "pywikibot-enter-finished-browser": "T\u0142\u00f3\u010d zapodawansku tastu po sk\u00f3n\u010denju wobhladowaka.",
-    "pywikibot-enter-namespace-number": "Pro\u0161u zapodaj \u010dis\u0142o mjenoweho ruma:",
-    "pywikibot-enter-new-text": "Pro\u0161 zapodaj nowy tekst:",
-    "pywikibot-enter-page-processing": "Kotra strona ma so p\u0159ed\u017a\u011b\u0142a\u0107?",
-    "pywikibot-fixes-isbn": "Bo\u0107ik: ISBN so formatuje"
+    "pywikibot-cosmetic-changes": "; kozmeti\u010dke izmjene",
+    "pywikibot-enter-category-name": "Unesite naziv kategorije:",
+    "pywikibot-enter-finished-browser": "Pritisnite enter kada zavr\u0161ite u pregleda\u010du.",
+    "pywikibot-enter-namespace-number": "Unesite imenski prostor pored njegovog broja:",
+    "pywikibot-enter-new-text": "Unesite novi tekst:",
+    "pywikibot-enter-page-processing": "Koja stranica treba da se obradi?",
+    "pywikibot-enter-xml-filename": "Unesite naziv XML ispisa:"
 }
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/hu.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/hu.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8892857142857142%*

 * *Differences: {"'@metadata'": "{'authors': {insert: [(0, 'Bináris')]}}",*

 * * "'pywikibot-bot-prefix'": "'Bot:'",*

 * * "'pywikibot-enter-category-name'": "'Add meg a kategórianevet:'"}*

```diff
@@ -1,18 +1,20 @@
 {
     "@metadata": {
         "authors": [
+            "Bin\u00e1ris",
             "Dani",
             "Dj",
             "R-Joe",
             "Tacsipacsi"
         ]
     },
+    "pywikibot-bot-prefix": "Bot:",
     "pywikibot-cosmetic-changes": "; kozmetikai v\u00e1ltoztat\u00e1sok",
-    "pywikibot-enter-category-name": "Add meg a kateg\u00f3ria nevet:",
+    "pywikibot-enter-category-name": "Add meg a kateg\u00f3rianevet:",
     "pywikibot-enter-file-links-processing": "Melyik f\u00e1jlra mutat\u00f3 hivatkoz\u00e1sokat kell feldolgozni?",
     "pywikibot-enter-finished-browser": "Nyomd meg az Entert, ha v\u00e9gezt\u00e9l a b\u00f6ng\u00e9sz\u0151vel!",
     "pywikibot-enter-namespace-number": "Add meg a n\u00e9vteret a sz\u00e1m\u00e1val:",
     "pywikibot-enter-new-text": "Add meg az \u00faj sz\u00f6veget:",
     "pywikibot-enter-page-processing": "Melyik lapot kell feldolgozni?",
     "pywikibot-enter-xml-filename": "Add meg az XML dump f\u00e1jl nev\u00e9t:",
     "pywikibot-fixes-fckeditor": "Bot: Vizu\u00e1lis szerkeszt\u0151 HTML-j\u00e9nek jav\u00edt\u00e1sa",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ia.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ia.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Robot:'"}*

```diff
@@ -1,13 +1,14 @@
 {
     "@metadata": {
         "authors": [
             "McDutchie"
         ]
     },
+    "pywikibot-bot-prefix": "Robot:",
     "pywikibot-cosmetic-changes": "; cambios cosmetic",
     "pywikibot-enter-category-name": "Per favor entra le nomine del categoria:",
     "pywikibot-enter-file-links-processing": "Le ligamines a qual pagina de file debe esser tractate?",
     "pywikibot-enter-finished-browser": "Preme Enter quando tu ha finite le modification in le navigator.",
     "pywikibot-enter-namespace-number": "Per favor entra le numero de un spatio de nomines:",
     "pywikibot-enter-new-text": "Per favor entra le nove texto:",
     "pywikibot-enter-page-processing": "Qual page debe esser tractate?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/id.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/id.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Bot:'"}*

```diff
@@ -8,14 +8,15 @@
             "IvanLanin",
             "Kenrick95",
             "Rachmat.Wahidi",
             "Rachmat04",
             "Totosunarto"
         ]
     },
+    "pywikibot-bot-prefix": "Bot:",
     "pywikibot-cosmetic-changes": "; perubahan kosmetika",
     "pywikibot-enter-category-name": "Silakan masukkan nama kategori:",
     "pywikibot-enter-file-links-processing": "Pranala ke halaman berkas manakah yang harus diproses?",
     "pywikibot-enter-finished-browser": "Tekan Enter jika telah selesai di peramban web.",
     "pywikibot-enter-namespace-number": "Silakan masukkan ruang nama menurut nomornya:",
     "pywikibot-enter-new-text": "Masukkan teks baru:",
     "pywikibot-enter-page-processing": "Halaman manakah yang harus diproses?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/io.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/io.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Bot:'"}*

```diff
@@ -1,13 +1,14 @@
 {
     "@metadata": {
         "authors": [
             "Joao Xavier"
         ]
     },
+    "pywikibot-bot-prefix": "Bot:",
     "pywikibot-cosmetic-changes": "; modifikuri por plubeligar",
     "pywikibot-enter-category-name": "Voluntez informar la nomo di la kategorio:",
     "pywikibot-enter-file-links-processing": "Quala ligili a qual arkivo mustas traktesar?",
     "pywikibot-enter-finished-browser": "Kliktez ''Enter'' pos finar che vua ret-navigilo.",
     "pywikibot-enter-namespace-number": "Informez ''namespace'' segun olua numero:",
     "pywikibot-enter-new-text": "Voluntez skribar la nova texto:",
     "pywikibot-enter-page-processing": "Quala pagino mustas esar traktata?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/is.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/is.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Vélmenni:'"}*

```diff
@@ -1,14 +1,15 @@
 {
     "@metadata": {
         "authors": [
             "Sn\u00e6var",
             "Sveinn \u00ed Felli"
         ]
     },
+    "pywikibot-bot-prefix": "V\u00e9lmenni:",
     "pywikibot-cosmetic-changes": "; \u00fatlitsbreytingar",
     "pywikibot-enter-category-name": "Vinsamlegast sl\u00e1\u00f0u inn nafn flokksins:",
     "pywikibot-enter-file-links-processing": "Tengla \u00e1 hva\u00f0a skr\u00e1as\u00ed\u00f0u \u00e6tti a\u00f0 vinna me\u00f0?",
     "pywikibot-enter-finished-browser": "\u00ddttu \u00e1 Enter \u00feegar \u00fe\u00fa ert b\u00fainn \u00ed vafranum.",
     "pywikibot-enter-namespace-number": "Vinsamlegast skrifa\u00f0u n\u00famer nafnr\u00fdmisins:",
     "pywikibot-enter-new-text": "Vinsamlegast sl\u00e1\u00f0u inn n\u00fdja textann:",
     "pywikibot-enter-page-processing": "Hva\u00f0a s\u00ed\u00f0u \u00e1 a\u00f0 vinna vi\u00f0?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/it.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/it.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Bot:'"}*

```diff
@@ -3,14 +3,15 @@
         "authors": [
             "Beta16",
             "F. Cosoleto",
             "Gianfranco",
             "Ricordisamoa"
         ]
     },
+    "pywikibot-bot-prefix": "Bot:",
     "pywikibot-cosmetic-changes": "; modifiche estetiche",
     "pywikibot-enter-category-name": "Inserisci il nome della categoria:",
     "pywikibot-enter-file-links-processing": "File per cui devono essere elaborate le pagine che vi puntano",
     "pywikibot-enter-finished-browser": "Premi Invio quando hai terminato nel browser.",
     "pywikibot-enter-namespace-number": "Inserisci il numero di un namespace:",
     "pywikibot-enter-new-text": "Inserisci il nuovo testo:",
     "pywikibot-enter-page-processing": "Quale pagina deve essere elaborata?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ja.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ja.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'pywikibot-bot-prefix'": "'ボットによる:'"}*

```diff
@@ -4,14 +4,15 @@
             "Alex Shih-Han Lin",
             "Fryed-peach",
             "Otokoume",
             "Shirayuki",
             "Weather Top Wizard"
         ]
     },
+    "pywikibot-bot-prefix": "\u30dc\u30c3\u30c8\u306b\u3088\u308b:",
     "pywikibot-cosmetic-changes": "; \u7d30\u90e8\u306e\u7de8\u96c6",
     "pywikibot-enter-category-name": "\u30ab\u30c6\u30b4\u30ea\u540d\u3092\u5165\u529b:",
     "pywikibot-enter-file-links-processing": "\u3069\u306e\u30d5\u30a1\u30a4\u30eb\u30da\u30fc\u30b8\u30d8\u306e\u30ea\u30f3\u30af\u3092\u51e6\u7406\u3057\u307e\u3059\u304b?",
     "pywikibot-enter-finished-browser": "\u7d42\u4e86\u3057\u305f\u3089 Enter \u30ad\u30fc\u3092\u62bc\u3057\u3066\u304f\u3060\u3055\u3044\u3002",
     "pywikibot-enter-namespace-number": "\u540d\u524d\u7a7a\u9593\u306e\u756a\u53f7\u3092\u5165\u529b:",
     "pywikibot-enter-new-text": "\u65b0\u3057\u3044\u30c6\u30ad\u30b9\u30c8\u3092\u5165\u529b:",
     "pywikibot-enter-page-processing": "\u3069\u306e\u30da\u30fc\u30b8\u3092\u51e6\u7406\u3057\u307e\u3059\u304b?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/kab.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/kab.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8888888888888888%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Aṛubut:'"}*

```diff
@@ -1,13 +1,14 @@
 {
     "@metadata": {
         "authors": [
             "K Messaoudi"
         ]
     },
+    "pywikibot-bot-prefix": "A\u1e5bubut:",
     "pywikibot-enter-category-name": "Ttxil sekcem isem n taggayt:",
     "pywikibot-enter-finished-browser": "Sit \u0263ef Kcem mi tfukke\u1e0d deg yiminig.",
     "pywikibot-enter-namespace-number": "Ttxil sekcem tallunt n yisem s um\u1e0dan-is:",
     "pywikibot-enter-new-text": "Ttxil sekcem a\u1e0dris amaynut:",
     "pywikibot-fixes-html": "A\u1e5bubut: Aselket/aseggem n HTML",
     "pywikibot-fixes-isbn": "A\u1e5bubut: Amsal n ISBN",
     "pywikibot-fixes-syntax": "A\u1e5bubut: Ase\u0263ti n tseddast n wiki"
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/kk.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/kk.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Робот:'"}*

```diff
@@ -1,13 +1,14 @@
 {
     "@metadata": {
         "authors": [
             "Arystanbek"
         ]
     },
+    "pywikibot-bot-prefix": "\u0420\u043e\u0431\u043e\u0442:",
     "pywikibot-cosmetic-changes": "; \u0431\u0435\u0437\u0435\u043d\u0434\u0456\u0440\u0443 \u04e9\u0437\u0433\u0435\u0440\u0456\u0441\u0442\u0435\u0440\u0456",
     "pywikibot-enter-category-name": "\u0421\u0430\u043d\u0430\u0442 \u0430\u0442\u0430\u0443\u044b\u043d \u0435\u043d\u0433\u0456\u0437\u0456\u04a3\u0456\u0437:",
     "pywikibot-enter-file-links-processing": "\u0424\u0430\u0439\u043b \u0431\u0435\u0442\u0456 \u0441\u0456\u043b\u0442\u0435\u043c\u0435\u043b\u0435\u0440\u0456\u043d \u04e9\u04a3\u0434\u0435\u0443 \u043a\u0435\u0440\u0435\u043a \u043f\u0435?",
     "pywikibot-enter-finished-browser": "\u0411\u0440\u0430\u0443\u0437\u0435\u0440\u0434\u0435 \u0430\u044f\u049b\u0442\u0430\u0493\u0430\u043d \u043a\u0435\u0437\u0434\u0435 Enter \u043f\u0435\u0440\u043d\u0435\u0441\u0456\u043d \u0431\u0430\u0441\u044b\u04a3\u044b\u0437.",
     "pywikibot-enter-namespace-number": "\u0415\u0441\u0456\u043c \u043a\u0435\u04a3\u0456\u0441\u0442\u0456\u0433\u0456\u043d \u043e\u043d\u044b\u04a3 \u043d\u04e9\u043c\u0435\u0440\u0456 \u0431\u043e\u0439\u044b\u043d\u0448\u0430 \u0435\u043d\u0433\u0456\u0437\u0456\u04a3\u0456\u0437:",
     "pywikibot-enter-new-text": "\u0416\u0430\u04a3\u0430 \u043c\u04d9\u0442\u0456\u043d \u0435\u043d\u0433\u0456\u0437\u0456\u04a3\u0456\u0437:",
     "pywikibot-enter-page-processing": "\u049a\u0430\u043d\u0434\u0430\u0439 \u0431\u0435\u0442 \u04e9\u04a3\u0434\u0435\u0443 \u043a\u0435\u0440\u0435\u043a?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/km.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/km.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/kn.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/kn.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ko.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ko.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'봇:'"}*

```diff
@@ -6,14 +6,15 @@
             "Kwj2772",
             "Priviet",
             "Revi",
             "Ykhwong",
             "\uc544\ub77c"
         ]
     },
+    "pywikibot-bot-prefix": "\ubd07:",
     "pywikibot-cosmetic-changes": "; \uc608\uc058\uac8c \ubc14\uafc8",
     "pywikibot-enter-category-name": "\ubd84\ub958 \uc774\ub984\uc744 \uc785\ub825\ud558\uc138\uc694:",
     "pywikibot-enter-file-links-processing": "\uc5b4\ub5a4 \ud30c\uc77c \ubb38\uc11c\ub85c \uc5f0\uacb0\ub41c \ub9c1\ud06c\ub97c \ucc98\ub9ac\ud558\uc2dc\uaca0\uc2b5\ub2c8\uae4c?",
     "pywikibot-enter-finished-browser": "\ube0c\ub77c\uc6b0\uc800\uc5d0\uc11c \uc791\uc5c5\uc774 \ub05d\ub098\uba74 \uc5d4\ud130 \ud0a4\ub97c \ub204\ub974\uc138\uc694.",
     "pywikibot-enter-namespace-number": "\uc774\ub984\uacf5\uac04 \ubc88\ud638\ub97c \uc785\ub825\ud558\uc138\uc694:",
     "pywikibot-enter-new-text": "\uc0c8 \ud14d\uc2a4\ud2b8\ub97c \uc785\ub825\ud558\uc138\uc694:",
     "pywikibot-enter-page-processing": "\uc5b4\ub5a4 \ubb38\uc11c\ub97c \ucc98\ub9ac\ud558\uc2dc\uaca0\uc2b5\ub2c8\uae4c?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/krc.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/krc.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Бот:'"}*

```diff
@@ -1,13 +1,14 @@
 {
     "@metadata": {
         "authors": [
             "\u041a\u044a\u0430\u0440\u0430\u0447\u0430\u0439\u043b\u044b"
         ]
     },
+    "pywikibot-bot-prefix": "\u0411\u043e\u0442:",
     "pywikibot-cosmetic-changes": "; \u043a\u043e\u0441\u043c\u0435\u0442\u0438\u043a \u0442\u044e\u0440\u043b\u0435\u043d\u0438\u0443\u043b\u0435",
     "pywikibot-enter-category-name": "\u0422\u0438\u043b\u0435\u0439\u0431\u0438\u0437, \u043a\u0430\u0442\u0435\u0433\u043e\u0440\u0438\u044f\u043d\u044b \u0430\u0442\u044b\u043d \u043a\u0438\u0440\u0433\u0438\u0437\u0442\u0438\u0433\u0438\u0437:",
     "pywikibot-enter-file-links-processing": "\u0424\u0430\u0439\u043b\u043d\u044b \u043a\u044a\u0430\u0439\u0441\u044b \u0431\u0435\u0442\u0438\u043d\u0435 \u0434\u0436\u0438\u0431\u0435\u0440\u0438\u0443\u043d\u044e \u0434\u0436\u0430\u0440\u0430\u0448\u0434\u044b\u0440\u044b\u0440\u0433\u044a\u0430 \u043a\u0435\u0440\u0435\u043a\u0434\u0438?",
     "pywikibot-enter-finished-browser": "\u0411\u0440\u0430\u0443\u0437\u0435\u0440\u0434\u0435 \u0431\u0438\u0442\u0441\u0435, Enter \u0442\u0438\u0435\u043a\u0433\u0435 \u0431\u0430\u0441\u044b\u0433\u044a\u044b\u0437.",
     "pywikibot-enter-namespace-number": "\u0422\u0438\u043b\u0435\u0439\u0431\u0438\u0437, \u043d\u043e\u043c\u0435\u0440\u0438\u043d\u0435 \u043a\u0451\u0440\u0435 \u0430\u0442 \u0430\u043b\u0430\u043d\u043d\u044b \u043a\u0438\u0440\u0433\u0438\u0437\u0442\u0438\u0433\u0438\u0437:",
     "pywikibot-enter-new-text": "\u0422\u0438\u043b\u0435\u0439\u0431\u0438\u0437, \u0434\u0436\u0430\u043d\u0433\u044b \u0442\u0435\u043a\u0441\u0442 \u043a\u0438\u0440\u0433\u0438\u0437\u0442\u0438\u0433\u0438\u0437:",
     "pywikibot-enter-page-processing": "\u041a\u044a\u0430\u0439\u0441\u044b \u0431\u0435\u0442 \u0434\u0436\u0430\u0440\u0430\u0448\u0434\u044b\u0440\u044b\u043b\u044b\u0440\u0433\u044a\u0430 \u043a\u0435\u0440\u0435\u043a\u0434\u0438?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ksh.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ksh.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Bot:'"}*

```diff
@@ -1,13 +1,14 @@
 {
     "@metadata": {
         "authors": [
             "Purodha"
         ]
     },
+    "pywikibot-bot-prefix": "Bot:",
     "pywikibot-cosmetic-changes": "; \u00c4nderonge f\u00f6r de Sch\u00f6nheit",
     "pywikibot-enter-category-name": "Jif d\u00e4 Saachjropp iere Nahme en:",
     "pywikibot-enter-file-links-processing": "De Lengks op wat f\u00f6r en Datteisigg sull be\u00e4rbeid w\u00e4\u00e4de?",
     "pywikibot-enter-finished-browser": "Dr\u00f6ck de <i lang=\"en\">Enter</i>-Ta\u00df\u00df, wann de f\u00e4hdesch bess em Brauser.",
     "pywikibot-enter-namespace-number": "Jif de Nommer f\u00f6r dat Apachtemang en:",
     "pywikibot-enter-new-text": "Jif d\u00e4 neue T\u00e4x en:",
     "pywikibot-enter-page-processing": "Wat f\u00f6r en Sigg sulle mer be\u00e4rbeide?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/lb.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/lb.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Bot:'"}*

```diff
@@ -1,14 +1,15 @@
 {
     "@metadata": {
         "authors": [
             "Robby",
             "Soued031"
         ]
     },
+    "pywikibot-bot-prefix": "Bot:",
     "pywikibot-cosmetic-changes": "; kosmetesch \u00c4nnerungen",
     "pywikibot-enter-category-name": "Gitt wgl. den Numm vun der Kategorie an:",
     "pywikibot-enter-file-links-processing": "Linken op wat fir eng Biller-S\u00e4it verschaftt solle ginn?",
     "pywikibot-enter-finished-browser": "Dr\u00e9ckt 'Enter' wann Dir f\u00e4erdeg sidd.",
     "pywikibot-enter-namespace-number": "Gitt wgl. d'Nummer vum Nummraum an:",
     "pywikibot-enter-new-text": "Gitt wgl. den neien Text an:",
     "pywikibot-enter-page-processing": "Watfir eng S\u00e4it soll verschafft ginn?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/lt.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/lt.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9230769230769231%*

 * *Differences: {"'pywikibot-bot-prefix'": "'robotas:'"}*

```diff
@@ -3,14 +3,15 @@
         "authors": [
             "Aswanas",
             "Aurimas Fischer",
             "Hugo.arg",
             "Mantak111"
         ]
     },
+    "pywikibot-bot-prefix": "robotas:",
     "pywikibot-cosmetic-changes": "; smulk\u016bs taisymai",
     "pywikibot-enter-category-name": "\u012eveskite kategorijos pavadinim\u0105:",
     "pywikibot-enter-file-links-processing": "Nurodo, kuris failo puslapis tur\u0117t\u0173 b\u016bti tvarkomas?",
     "pywikibot-enter-finished-browser": "Paspauskite Enter kuomet baigsite nar\u0161ykl\u0117je.",
     "pywikibot-enter-namespace-number": "\u012evestkite vard\u0173 srities numer\u012f:",
     "pywikibot-enter-new-text": "\u012eveskite nauj\u0105 tekst\u0105:",
     "pywikibot-enter-page-processing": "Kuris puslapis tur\u0117t\u0173 b\u016bti tvarkomas?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/lv.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/lv.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Bots:'"}*

```diff
@@ -2,14 +2,15 @@
     "@metadata": {
         "authors": [
             "Karlis",
             "Papuass",
             "Silraks"
         ]
     },
+    "pywikibot-bot-prefix": "Bots:",
     "pywikibot-cosmetic-changes": "; kosm\u0113tisk\u0101s izmai\u0146as",
     "pywikibot-enter-category-name": "L\u016bdzu, ievadiet kategorijas nosaukumu:",
     "pywikibot-enter-file-links-processing": "Saites uz kuru faila lapu b\u016btu j\u0101apstr\u0101d\u0101?",
     "pywikibot-enter-namespace-number": "L\u016bdzu, ievadiet v\u0101rdtelpu p\u0113c t\u0101s numura:",
     "pywikibot-enter-new-text": "L\u016bdzu, ievadiet jaunu tekstu:",
     "pywikibot-enter-page-processing": "Kura lapa b\u016btu j\u0101apstr\u0101d\u0101?",
     "pywikibot-fixes-isbn": "Robots: ISBN format\u0113jums",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/map-bms.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/nds-nl.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.35%*

 * *Differences: {"'@metadata'": "{'authors': ['Servien']}",*

 * * "'pywikibot-bot-prefix'": "'Bot:'",*

 * * "'pywikibot-cosmetic-changes'": "'; kosmetiske wysigingen'",*

 * * "'pywikibot-enter-category-name'": "'Geef de kategorienaam op:'",*

 * * "'pywikibot-enter-file-links-processing'": "'Verwiezingen naor welke bestaandszied mutten "*

 * *                                            "verwarkt wörden?'",*

 * * "'pywikibot-enter-finished-browser'": '\'Drok op "Enter" a\\\'j klaor bin in de webkieker.\'',*

 * * "'pywikibot-enter-namespace-number'": "'Geef n  […]*

```diff
@@ -1,16 +1,21 @@
 {
     "@metadata": {
         "authors": [
-            "StefanusRA"
+            "Servien"
         ]
     },
-    "pywikibot-cosmetic-changes": "; owahan kosmetika",
-    "pywikibot-enter-category-name": "Monggo lebokna jeneng kategori:",
-    "pywikibot-enter-file-links-processing": "Pranala maring kaca berkas endi sing arep deproses?",
-    "pywikibot-enter-finished-browser": "Penet Enter angger wis rampung nang pramban.",
-    "pywikibot-enter-namespace-number": "Monggo lebokna bilikjeneng nanggo nomere:",
-    "pywikibot-enter-new-text": "Monggo lebokna teks anyar:",
-    "pywikibot-enter-page-processing": "Kaca endi sing arep deproses ?",
-    "pywikibot-enter-xml-filename": "Monggo nglebokna jenengberkas dump XML:",
-    "pywikibot-fixes-isbn": "Bot: Mbeneri format ISBN"
+    "pywikibot-bot-prefix": "Bot:",
+    "pywikibot-cosmetic-changes": "; kosmetiske wysigingen",
+    "pywikibot-enter-category-name": "Geef de kategorienaam op:",
+    "pywikibot-enter-file-links-processing": "Verwiezingen naor welke bestaandszied mutten verwarkt w\u00f6rden?",
+    "pywikibot-enter-finished-browser": "Drok op \"Enter\" a'j klaor bin in de webkieker.",
+    "pywikibot-enter-namespace-number": "Geef n naamruumtenummer op:",
+    "pywikibot-enter-new-text": "Geef de nieje tekste op:",
+    "pywikibot-enter-page-processing": "Welke zied mut verwarkt w\u00f6rden?",
+    "pywikibot-enter-xml-filename": "Geef de bestaandsnaam van n XML-dump op:",
+    "pywikibot-fixes-fckeditor": "Bot: HTML van tekstverwarker verbeterd",
+    "pywikibot-fixes-html": "Bot: konversie/ripperasie HTML",
+    "pywikibot-fixes-isbn": "Bot: ISBN upmaked",
+    "pywikibot-fixes-syntax": "Bot: ripperasie wikisyntaxis",
+    "pywikibot-touch": "Pywikibot-nulbewarking"
 }
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/mg.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/mg.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Rôbô:'"}*

```diff
@@ -1,13 +1,14 @@
 {
     "@metadata": {
         "authors": [
             "Jagwar"
         ]
     },
+    "pywikibot-bot-prefix": "R\u00f4b\u00f4:",
     "pywikibot-cosmetic-changes": "; fanovana arak'endrika.",
     "pywikibot-enter-category-name": "Atsofohy ny anaran-tsokajy:",
     "pywikibot-enter-file-links-processing": "Ny rohin-drakitra hovaina?",
     "pywikibot-enter-finished-browser": "Tsindrio \"ENTER\" rehefa tapitra ny fanovana ao amin'ny mpitety tranonkala.",
     "pywikibot-enter-namespace-number": "Atsofohy eto ny laharan'ilay anaran-tsehatra",
     "pywikibot-enter-new-text": "Mampidira lahatsoratra vaovao:",
     "pywikibot-enter-page-processing": "Inona ny pejy hovaina?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/min.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/min.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Bot:'"}*

```diff
@@ -2,14 +2,15 @@
     "@metadata": {
         "authors": [
             "Bennylin",
             "Luthfi94",
             "Naval Scene"
         ]
     },
+    "pywikibot-bot-prefix": "Bot:",
     "pywikibot-cosmetic-changes": "; parubahan kosmetik",
     "pywikibot-enter-category-name": "Masuakkan namo kategori:",
     "pywikibot-enter-file-links-processing": "Pautan ka laman gambar manokah nan ka diproses?",
     "pywikibot-enter-namespace-number": "Masuakkan ruang namo manuruik nomornyo:",
     "pywikibot-enter-new-text": "Masuakkan teks baru:",
     "pywikibot-enter-page-processing": "Laman manokah nan harus diproses?",
     "pywikibot-enter-xml-filename": "Masuakkan namo Berkas sarok XML:",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/mk.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/mk.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Бот:'"}*

```diff
@@ -1,13 +1,14 @@
 {
     "@metadata": {
         "authors": [
             "Bjankuloski06"
         ]
     },
+    "pywikibot-bot-prefix": "\u0411\u043e\u0442:",
     "pywikibot-cosmetic-changes": "; \u043a\u043e\u0437\u043c\u0435\u0442\u0438\u0447\u043a\u0438 \u043f\u0440\u043e\u043c\u0435\u043d\u0438",
     "pywikibot-enter-category-name": "\u0412\u043d\u0435\u0441\u0435\u0442\u0435 \u0433\u043e \u0438\u043c\u0435\u0442\u043e \u043d\u0430 \u043a\u0430\u0442\u0435\u0433\u043e\u0440\u0438\u0458\u0430\u0442\u0430:",
     "pywikibot-enter-file-links-processing": "\u0417\u0430 \u043a\u043e\u0458\u0430 \u043f\u043e\u0434\u0430\u0442\u043e\u0442\u0435\u043a\u0430 \u0434\u0430 \u0433\u0438 \u043e\u0431\u0440\u0430\u0431\u043e\u0442\u0430\u043c \u0432\u0440\u0441\u043a\u0438\u0442\u0435?",
     "pywikibot-enter-finished-browser": "\u0421\u0442\u0438\u0441\u043d\u0435\u0442\u0435 \u043d\u0430 \u201eEnter\u201c \u043a\u043e\u0433\u0430 \u045c\u0435 \u0437\u0430\u0432\u0440\u0448\u0438\u0442\u0435 \u0432\u043e \u043f\u0440\u0435\u043b\u0438\u0441\u0442\u0443\u0432\u0430\u0447\u043e\u0442.",
     "pywikibot-enter-namespace-number": "\u0412\u043d\u0435\u0441\u0435\u0442\u0435 \u0433\u043e \u0438\u043c\u0435\u043d\u0441\u043a\u0438\u043e\u0442 \u043f\u0440\u043e\u0441\u0442\u043e\u0440 \u0441\u043f\u043e\u0440\u0435\u0434 \u043d\u0435\u0433\u043e\u0432\u0438\u043e\u0442 \u0431\u0440\u043e\u0458:",
     "pywikibot-enter-new-text": "\u0412\u043d\u0435\u0441\u0435\u0442\u0435 \u0433\u043e \u043d\u043e\u0432\u0438\u043e\u0442 \u0442\u0435\u043a\u0441\u0442:",
     "pywikibot-enter-page-processing": "\u041a\u043e\u0458\u0430 \u0441\u0442\u0440\u0430\u043d\u0438\u0446\u0430 \u0442\u0440\u0435\u0431\u0430 \u0434\u0430 \u0441\u0435 \u043e\u0431\u0440\u0430\u0431\u043e\u0442\u0438?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ml.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ml.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ms.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ms.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Robot:'"}*

```diff
@@ -1,14 +1,15 @@
 {
     "@metadata": {
         "authors": [
             "Anakmalaysia",
             "Kurniasan"
         ]
     },
+    "pywikibot-bot-prefix": "Robot:",
     "pywikibot-cosmetic-changes": "; perubahan kosmetik",
     "pywikibot-enter-category-name": "Sila masukkan nama kategori:",
     "pywikibot-enter-file-links-processing": "Pautan ke halaman fail yang manakah harus diproses?",
     "pywikibot-enter-finished-browser": "Tekan Enter selepas siap dalam pelayar.",
     "pywikibot-enter-namespace-number": "Sila masukkan ruang nama mengikut nombornya:",
     "pywikibot-enter-new-text": "Sila masukkan teks baru:",
     "pywikibot-enter-page-processing": "Halaman yang manakah harus diproses?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/my.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/my.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'pywikibot-bot-prefix'": "'ဘော့:'"}*

```diff
@@ -1,14 +1,15 @@
 {
     "@metadata": {
         "authors": [
             "Lionslayer",
             "Ninjastrikers"
         ]
     },
+    "pywikibot-bot-prefix": "\u1018\u1031\u102c\u1037:",
     "pywikibot-enter-category-name": "\u1000\u103b\u1031\u1038\u1007\u1030\u1038\u1015\u103c\u102f\u104d \u1000\u100f\u1039\u100d\u1021\u1019\u100a\u103a \u101b\u102d\u102f\u1000\u103a\u1011\u100a\u1037\u103a\u1015\u102b:",
     "pywikibot-enter-finished-browser": "\u1015\u103c\u102e\u1038\u1005\u102e\u1038\u1015\u102b\u1000 \u1018\u101b\u1031\u102c\u1000\u103a\u1007\u102c\u1010\u103d\u1004\u103a Enter \u1000\u102d\u102f \u1014\u103e\u102d\u1015\u103a\u1015\u102b\u104b",
     "pywikibot-enter-namespace-number": "\u1021\u1019\u100a\u103a\u100a\u103d\u103e\u1014\u103a\u1038\u1000\u102d\u102f \u101a\u1004\u103a\u1038\u104f \u1014\u1036\u1015\u102b\u1010\u103a\u1021\u102c\u1038 \u101b\u102d\u102f\u1000\u103a\u1011\u100a\u1037\u103a\u1015\u103c\u102e\u1038 \u1000\u103b\u1031\u1038\u1007\u1030\u1038\u1015\u103c\u102f\u104d \u1011\u100a\u1037\u103a\u101e\u103d\u1004\u103a\u1038\u1015\u102b:",
     "pywikibot-enter-new-text": "\u1005\u102c\u101e\u102c\u1038\u1021\u101e\u1005\u103a\u1000\u102d\u102f \u1000\u103b\u1031\u1038\u1007\u1030\u1038\u1015\u103c\u102f\u104d \u101b\u102d\u102f\u1000\u103a\u1011\u100a\u1037\u103a\u1015\u102b:",
     "pywikibot-enter-page-processing": "\u1019\u100a\u103a\u101e\u100a\u1037\u103a \u1005\u102c\u1019\u103b\u1000\u103a\u1014\u103e\u102c\u1000\u102d\u102f \u101c\u102f\u1015\u103a\u1006\u1031\u102c\u1004\u103a\u1019\u100a\u103a\u1014\u100a\u103a\u1038",
     "pywikibot-enter-xml-filename": "\u1000\u103b\u1031\u1038\u1007\u1030\u1038\u1015\u103c\u102f\u104d XML dump \u1016\u102d\u102f\u1004\u103a\u1021\u1019\u100a\u103a\u1000\u102d\u102f \u1011\u100a\u1037\u103a\u101e\u103d\u1004\u103a\u1038\u1015\u102b:",
     "pywikibot-fixes-html": "\u1018\u1031\u102c\u1037: HTML \u1015\u103c\u1031\u102c\u1004\u103a\u1038\u101c\u1032\u1001\u103c\u1004\u103a\u1038/\u1015\u103c\u1004\u103a\u1006\u1004\u103a\u1001\u103c\u1004\u103a\u1038",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/nan.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/nan.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Bot:'"}*

```diff
@@ -1,14 +1,15 @@
 {
     "@metadata": {
         "authors": [
             "A-l\u00fa-mih",
             "Luuva"
         ]
     },
+    "pywikibot-bot-prefix": "Bot:",
     "pywikibot-cosmetic-changes": "; si\u00f3 h\u0101ng siu-k\u00e1i",
     "pywikibot-enter-category-name": "Chi\u00e1\u207f phah ji\u030dp l\u016bi-pia\u030dt mi\u00e2-h\u014d:",
     "pywikibot-enter-file-links-processing": "Li\u00e2n k\u00f2e t\u00f3 chi\u030dt ki\u0101\u207f t\u00f3ng-\u00e0n \u00ea ia\u030dh-b\u012bn su-i\u00e0u chh\u00f9-l\u00ed?",
     "pywikibot-enter-finished-browser": "Go\u00e2n-s\u00eang \u00ea s\u00ee-ch\u016bn t\u012b li\u00fb-l\u00e1m-kh\u00ec l\u0101i ji\u030dh Enter.",
     "pywikibot-enter-namespace-number": "Chhi\u00e1n chi\u00e0u chi\u030dt-\u00ea mi\u00e2-khong-kan su-ji\u030dp i-\u00ea h\u014d-b\u00e9:",
     "pywikibot-enter-new-text": "Chhi\u00e1\u207f su-ji\u030dp sin b\u00fbn-j\u012b:",
     "pywikibot-enter-page-processing": "T\u00f3 chi\u030dt ia\u030dh s\u012b su-i\u00e0u chh\u00f9-l\u00ed--\u00ea?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/nb.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/nb.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Robot:'"}*

```diff
@@ -2,14 +2,15 @@
     "@metadata": {
         "authors": [
             "Danmichaelo",
             "Jon Harald S\u00f8by",
             "SuperPotato"
         ]
     },
+    "pywikibot-bot-prefix": "Robot:",
     "pywikibot-cosmetic-changes": "; kosmetiske endringer",
     "pywikibot-enter-category-name": "Skriv inn kategorinavnet:",
     "pywikibot-enter-file-links-processing": "Lenker til hvilken bildeside som skal behandles?",
     "pywikibot-enter-finished-browser": "Trykk Enter n\u00e5r du er ferdig i nettleseren.",
     "pywikibot-enter-namespace-number": "Skriv inn et navneromtall:",
     "pywikibot-enter-new-text": "Skriv inn den nye teksten:",
     "pywikibot-enter-page-processing": "Hvilken side skal behandles?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/nds-nl.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/yue.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4166666666666667%*

 * *Differences: {"'@metadata'": "{'authors': ['Hello903hello', 'Shinjiman']}",*

 * * "'pywikibot-bot-prefix'": "'機械人：'",*

 * * "'pywikibot-enter-category-name'": "'請輸入分類名：'",*

 * * "'pywikibot-enter-file-links-processing'": "'有邊啲檔案版嘅拎要處理？'",*

 * * "'pywikibot-enter-finished-browser'": "'喺瀏覽器完成編輯之後撳Enter掣。'",*

 * * "'pywikibot-enter-namespace-number'": "'請輸入空間名嘅冧巴：'",*

 * * "'pywikibot-enter-new-text'": "'請輸入新字：'",*

 * * "'pywikibot-enter-page-processing'": "'應該去處理邊版？'",*

 * * "'pywikibot-enter-xml-filename'": "'請輸入XML傾印嘅檔名：'",*

 * * "'pywikibot-fixes-fckeditor'": "'機 […]*

```diff
@@ -1,20 +1,20 @@
 {
     "@metadata": {
         "authors": [
-            "Servien"
+            "Hello903hello",
+            "Shinjiman"
         ]
     },
-    "pywikibot-cosmetic-changes": "; kosmetiske wysigingen",
-    "pywikibot-enter-category-name": "Geef de kategorienaam op:",
-    "pywikibot-enter-file-links-processing": "Verwiezingen naor welke bestaandszied mutten verwarkt w\u00f6rden?",
-    "pywikibot-enter-finished-browser": "Drok op \"Enter\" a'j klaor bin in de webkieker.",
-    "pywikibot-enter-namespace-number": "Geef n naamruumtenummer op:",
-    "pywikibot-enter-new-text": "Geef de nieje tekste op:",
-    "pywikibot-enter-page-processing": "Welke zied mut verwarkt w\u00f6rden?",
-    "pywikibot-enter-xml-filename": "Geef de bestaandsnaam van n XML-dump op:",
-    "pywikibot-fixes-fckeditor": "Bot: HTML van tekstverwarker verbeterd",
-    "pywikibot-fixes-html": "Bot: konversie/ripperasie HTML",
-    "pywikibot-fixes-isbn": "Bot: ISBN upmaked",
-    "pywikibot-fixes-syntax": "Bot: ripperasie wikisyntaxis",
-    "pywikibot-touch": "Pywikibot-nulbewarking"
+    "pywikibot-bot-prefix": "\u6a5f\u68b0\u4eba\uff1a",
+    "pywikibot-enter-category-name": "\u8acb\u8f38\u5165\u5206\u985e\u540d\uff1a",
+    "pywikibot-enter-file-links-processing": "\u6709\u908a\u5572\u6a94\u6848\u7248\u5605\u62ce\u8981\u8655\u7406\uff1f",
+    "pywikibot-enter-finished-browser": "\u55ba\u700f\u89bd\u5668\u5b8c\u6210\u7de8\u8f2f\u4e4b\u5f8c\u64b3Enter\u63a3\u3002",
+    "pywikibot-enter-namespace-number": "\u8acb\u8f38\u5165\u7a7a\u9593\u540d\u5605\u51a7\u5df4\uff1a",
+    "pywikibot-enter-new-text": "\u8acb\u8f38\u5165\u65b0\u5b57\uff1a",
+    "pywikibot-enter-page-processing": "\u61c9\u8a72\u53bb\u8655\u7406\u908a\u7248\uff1f",
+    "pywikibot-enter-xml-filename": "\u8acb\u8f38\u5165XML\u50be\u5370\u5605\u6a94\u540d\uff1a",
+    "pywikibot-fixes-fckeditor": "\u6a5f\u68b0\u4eba\uff1a\u4fee\u6b63\u8996\u89ba\u7de8\u8f2f\u5668HTML",
+    "pywikibot-fixes-html": "\u6a5f\u68b0\u4eba\uff1a\u8f49\u63db/\u4fee\u6b63HTML",
+    "pywikibot-fixes-syntax": "\u6a5f\u68b0\u4eba\uff1a\u4fee\u6b63wiki\u8a9e\u6cd5",
+    "pywikibot-touch": "Pywikibot touch\u7de8\u8f2f"
 }
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ne.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ne.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9230769230769231%*

 * *Differences: {"'pywikibot-bot-prefix'": "'बोट:'"}*

```diff
@@ -2,14 +2,15 @@
     "@metadata": {
         "authors": [
             "RajeshPandey",
             "\u092a\u0930\u094d\u0935\u0924 \u0938\u0941\u092c\u0947\u0926\u0940",
             "\u0938\u0930\u094b\u091c \u0915\u0941\u092e\u093e\u0930 \u0922\u0915\u093e\u0932"
         ]
     },
+    "pywikibot-bot-prefix": "\u092c\u094b\u091f:",
     "pywikibot-cosmetic-changes": "; \u0915\u0938\u094d\u092e\u0947\u091f\u093f\u0915 \u092a\u0930\u093f\u0935\u0930\u094d\u0924\u0928\u0939\u0930\u0942",
     "pywikibot-enter-category-name": "\u0915\u0943\u092a\u092f\u093e \u0936\u094d\u0930\u0947\u0923\u0940\u0915\u094b \u0928\u093e\u092e \u092a\u094d\u0930\u0935\u093f\u0937\u094d\u0920 \u0917\u0930\u094d\u0928\u0941\u0939\u094b\u0938\u094d :",
     "pywikibot-enter-file-links-processing": "\u092b\u093e\u0907\u0932 \u092a\u0943\u0937\u094d\u0920 \u0938\u092e\u094d\u092a\u093e\u0926\u0928 \u0917\u0930\u094d\u0928\u0941 \u092a\u0930\u094d\u0928\u0947 \u0932\u0915\u094d\u0937\u094d\u092f\u0915\u094b \u0932\u093f\u0919\u094d\u0915 ?",
     "pywikibot-enter-finished-browser": "\u092c\u094d\u0930\u093e\u0909\u091c\u0930\u092e\u093e \u0938\u0915\u093f\u090f\u092a\u091b\u093f \u0907\u0928\u094d\u091f\u0930 \u0925\u093f\u091a\u094d\u0928\u0941\u0939\u094b\u0932\u093e \u0964",
     "pywikibot-enter-namespace-number": "\u0915\u0943\u092a\u092f\u093e \u0928\u093e\u092e\u092a\u0926 \u0938\u0919\u094d\u0916\u094d\u092f\u093e\u0915\u094b \u0930\u0941\u092a\u092e\u093e \u0930\u093e\u0916\u094d\u0928\u0941\u0939\u094b\u0932\u093e :",
     "pywikibot-enter-new-text": "\u0915\u0943\u092a\u092f\u093e \u0928\u092f\u093e\u0901 \u092a\u093e\u0920 \u092a\u094d\u0930\u0935\u093f\u0937\u094d\u0920 \u0917\u0930\u094d\u0928\u0941\u0939\u094b\u0938\u094d :",
     "pywikibot-enter-page-processing": "\u0915\u0941\u0928 \u092a\u0943\u0937\u094d\u0920\u092e\u093e \u0915\u093e\u0930\u094d\u092f \u0917\u0930\u094d\u0928\u0947 \u0939\u094b ?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/new.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/new.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/nl.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sv.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48333333333333334%*

 * *Differences: {"'@metadata'": "{'authors': ['Ainali', 'Anhn', 'Cybjit', 'Jopparn', 'Lokal Profil', 'Mjälten', "*

 * *                "'WikiPhoenix', 'skorpan']}",*

 * * "'pywikibot-bot-prefix'": "'Bot:'",*

 * * "'pywikibot-cosmetic-changes'": "'; kosmetiska ändringar'",*

 * * "'pywikibot-enter-category-name'": "'Ange kategorinamnet:'",*

 * * "'pywikibot-enter-file-links-processing'": "'Länkar till vilken filsida ska behandlas?'",*

 * * "'pywikibot-enter-finished-browser'": "'Tryck på Enter när du är klar i webbläsaren.'",*

 * * "'pywikibot-enter-namespace […]*

```diff
@@ -1,22 +1,28 @@
 {
     "@metadata": {
         "authors": [
-            "McDutchie",
-            "Optilete",
-            "Siebrand"
+            "Ainali",
+            "Anhn",
+            "Cybjit",
+            "Jopparn",
+            "Lokal Profil",
+            "Mj\u00e4lten",
+            "WikiPhoenix",
+            "skorpan"
         ]
     },
-    "pywikibot-cosmetic-changes": "; cosmetische wijzigingen",
-    "pywikibot-enter-category-name": "Geef de categorienaam op:",
-    "pywikibot-enter-file-links-processing": "Koppelingen naar welke bestandspagina verwerken?",
-    "pywikibot-enter-finished-browser": "Druk op \"Enter\" wanneer u klaar bent in de browser.",
-    "pywikibot-enter-namespace-number": "Geef een naamruimtenummer op:",
-    "pywikibot-enter-new-text": "Geef de nieuwe tekst op:",
-    "pywikibot-enter-page-processing": "Welke pagina moet verwerkt worden?",
-    "pywikibot-enter-xml-filename": "Geef de bestandnaam van een XML-dump op:",
-    "pywikibot-fixes-fckeditor": "Robot: HTML van tekstverwerker gecorrigeerd",
-    "pywikibot-fixes-html": "Robot: conversie/reparatie HTML",
-    "pywikibot-fixes-isbn": "Robot: ISBN opgemaakt",
-    "pywikibot-fixes-syntax": "Robot: reparatie wikisyntaxis",
-    "pywikibot-touch": "Pywikibot touch bewerking"
+    "pywikibot-bot-prefix": "Bot:",
+    "pywikibot-cosmetic-changes": "; kosmetiska \u00e4ndringar",
+    "pywikibot-enter-category-name": "Ange kategorinamnet:",
+    "pywikibot-enter-file-links-processing": "L\u00e4nkar till vilken filsida ska behandlas?",
+    "pywikibot-enter-finished-browser": "Tryck p\u00e5 Enter n\u00e4r du \u00e4r klar i webbl\u00e4saren.",
+    "pywikibot-enter-namespace-number": "Ange namnrymden via dess nummer:",
+    "pywikibot-enter-new-text": "Skriv in den nya texten:",
+    "pywikibot-enter-page-processing": "Vilken sida ska behandlas?",
+    "pywikibot-enter-xml-filename": "Ange XML-dumpens filnamn:",
+    "pywikibot-fixes-fckeditor": "Bot: \u00c5tg\u00e4rdar Rich-editor-html",
+    "pywikibot-fixes-html": "Bot: Konverterar/korrigerar HTML",
+    "pywikibot-fixes-isbn": "Bot: Formaterar ISBN",
+    "pywikibot-fixes-syntax": "Bot: Fixar wikisyntax",
+    "pywikibot-touch": "Pywikibot noll-redigering"
 }
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/nqo.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/nqo.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'pywikibot-bot-prefix'": "'ߡߐ߰ߡߐ߮:'"}*

```diff
@@ -1,13 +1,14 @@
 {
     "@metadata": {
         "authors": [
             "Lancine.kounfantoh.fofana"
         ]
     },
+    "pywikibot-bot-prefix": "\u07e1\u07d0\u07f0\u07e1\u07d0\u07ee:",
     "pywikibot-cosmetic-changes": "; \u07e1\u07ca\u07ec\u07de\u07cb\u07f2\u07f0\u07e7\u07ca\u07ec\u07df\u07cc \u07e1\u07dd\u07ca\u07ec\u07df\u07cb\u07f2\u07ec\u07e0\u07cc\u07f2 \u07e0\u07ce\u07ec",
     "pywikibot-enter-category-name": "\u07e6\u07cc\u07df\u07e1\u07ca \u07d5\u07d0\u07ee \u07df\u07ca\u07d8\u07cf\u07f2\u07ec \u07d6\u07ca\u07f0\u07e3\u07cc\u07f2\u07eb:",
     "pywikibot-enter-file-links-processing": "\u07de\u07d0\u07d5\u07d0\u07ee \u07de\u07d0\u07dc\u07cd \u07e2\u07ca\u07d3\u07d0\u07eb \u07d5\u07d0\u07eb \u07e6\u07cb\u07eb \u07db\u07d8\u07cc\u07ec\u07dc\u07cb\u07f2 \u07e1\u07cd\u07f2 \u07e0\u07ca\u07eb",
     "pywikibot-enter-finished-browser": "\u07d8\u07cf\u07f2\u07ec (enter) \u07d8\u07cc\u07ef \u07e3\u07f4\u07cc \u07d3\u07ca\u07f2\u07eb \u07d8\u07ca\u07eb \u07db\u07cf\u07f2\u07ef\u07d3\u07ca\u07df\u07ca\u07f2 \u07e0\u07ca\u07eb.",
     "pywikibot-enter-namespace-number": "\u07d5\u07d0\u07ef \u07de\u07e3\u07cd \u07df\u07ca\u07d8\u07cf\u07f2\u07ec \u07ca\u07ec \u07dd\u07d9\u07cd\u07d5\u07cd \u07df\u07ca\u07eb \u07d6\u07ca\u07f0\u07e3\u07cc\u07f2\u07eb:",
     "pywikibot-enter-new-text": "\u07de\u07df\u07cf\u07dc\u07cd\u07eb \u07de\u07ce\u07d8\u07ca\u07eb \u07df\u07ca\u07d8\u07cf\u07f2\u07ec \u07d6\u07ca\u07f0\u07e3\u07cc\u07f2\u07eb:",
     "pywikibot-enter-page-processing": "\u07de\u07d0\u07dc\u07cd \u07e2\u07ce\u07ec\u07e1\u07ca\u07f2\u07eb \u07e0\u07cb\u07ec \u07e2\u07ca\u07d3\u07d0\u07eb \u07d5\u07d0\u07eb \u07e6\u07cb\u07eb\u061f",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/pl.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/pl.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Robot:'"}*

```diff
@@ -3,14 +3,15 @@
         "authors": [
             "Leszek Krupi\u0144ski",
             "Matma Rex",
             "Sp5uhe",
             "Woytecr"
         ]
     },
+    "pywikibot-bot-prefix": "Robot:",
     "pywikibot-cosmetic-changes": "; zmiany kosmetyczne",
     "pywikibot-enter-category-name": "Wpisz nazw\u0119 kategorii:",
     "pywikibot-enter-file-links-processing": "Linki do strony jakiego pliku maj\u0105 by\u0107 przetworzone?",
     "pywikibot-enter-finished-browser": "Wci\u015bnij Enter, gdy przegl\u0105darka zako\u0144czy prac\u0119.",
     "pywikibot-enter-namespace-number": "Wpisz numer przestrzeni nazw:",
     "pywikibot-enter-new-text": "Wpisz nowy tekst:",
     "pywikibot-enter-page-processing": "Jak\u0105 stron\u0119 przetworzy\u0107?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/pms.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/pms.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9090909090909091%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Trigomiro:'"}*

```diff
@@ -1,14 +1,15 @@
 {
     "@metadata": {
         "authors": [
             "Borich\u00e8t",
             "Dragon\u00f2t"
         ]
     },
+    "pywikibot-bot-prefix": "Trigomiro:",
     "pywikibot-cosmetic-changes": "; cangiament cosm\u00e9tich",
     "pywikibot-enter-category-name": "P\u00ebr pias\u00ec, ch'a anserissa \u00ebl n\u00f2m \u00ebd la categor\u00eca:",
     "pywikibot-enter-file-links-processing": "Liure a la p\u00e0gina d'archivi ch'a ventr\u00eca trat\u00e9?",
     "pywikibot-enter-finished-browser": "Ch'a sgnaca A cap quand a l'ha fin\u00ec ant \u00ebl navigador.",
     "pywikibot-enter-namespace-number": "P\u00ebr pias\u00ec anseriss n\u00eb spassi nominal con s\u00f2 n\u00f9mer:",
     "pywikibot-enter-new-text": "P\u00ebr pias\u00ec, ch'a anserissa \u00ebl test neuv:",
     "pywikibot-enter-page-processing": "Che p\u00e0gina a ventr\u00eca trat\u00e9?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/pt-br.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/pt-br.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Robô:'"}*

```diff
@@ -3,14 +3,15 @@
         "authors": [
             "Eduardo Addad de Oliveira",
             "Eduardoaddad",
             "Giro720",
             555
         ]
     },
+    "pywikibot-bot-prefix": "Rob\u00f4:",
     "pywikibot-cosmetic-changes": "; mudan\u00e7as triviais",
     "pywikibot-enter-category-name": "Insira o nome da categoria:",
     "pywikibot-enter-file-links-processing": "Para qual imagem os links devem ser processados?",
     "pywikibot-enter-finished-browser": "Pressione Enter ao concluir no navegador.",
     "pywikibot-enter-namespace-number": "Insira o n\u00famero de espa\u00e7o nominal:",
     "pywikibot-enter-new-text": "Insira o novo texto:",
     "pywikibot-enter-page-processing": "Qual p\u00e1gina deve ser processada?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/pt.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/pt.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Robô:'"}*

```diff
@@ -4,14 +4,15 @@
             "Alchimista",
             "Hamilton Abreu",
             "Leonardo Gregianin",
             "Malafaya",
             "Vitorvicentevalente"
         ]
     },
+    "pywikibot-bot-prefix": "Rob\u00f4:",
     "pywikibot-cosmetic-changes": "; mudan\u00e7as triviais",
     "pywikibot-enter-category-name": "Por favor, introduza o nome da categoria:",
     "pywikibot-enter-file-links-processing": "Devem ser processadas as hiperliga\u00e7\u00f5es para qual p\u00e1gina de ficheiro?",
     "pywikibot-enter-finished-browser": "Pressione Enter quando terminar no navegador",
     "pywikibot-enter-namespace-number": "Por favor, introduza um espa\u00e7o nominal usando o seu n\u00famero:",
     "pywikibot-enter-new-text": "Por favor, introduza o novo texto:",
     "pywikibot-enter-page-processing": "Que p\u00e1gina deve ser processada?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/qqq.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/qqq.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Summary prefix for bot edits.'"}*

```diff
@@ -6,14 +6,15 @@
             "Fabian Neundorf",
             "Lloffiwr",
             "Macofe",
             "TTMTT",
             "Xqt"
         ]
     },
+    "pywikibot-bot-prefix": "Summary prefix for bot edits.",
     "pywikibot-cosmetic-changes": "Summary message that will be appended to the normal edit summary when cosmetic changes are made on the fly.\n\n\"Cosmetic changes\" here means changes to the appearance of the page only, without any changes to the substance of the page.",
     "pywikibot-enter-category-name": "Message displayed to the bot owner to enter the category name.",
     "pywikibot-enter-file-links-processing": "Question displayed to the bot owner processing links to a given file page.",
     "pywikibot-enter-finished-browser": "Message displayed to the bot owner to press Enter button when browser edits are finished.",
     "pywikibot-enter-namespace-number": "Message displayed to the bot owner to enter a namespace by its number.",
     "pywikibot-enter-new-text": "Message displayed to the bot owner to enter the new text.",
     "pywikibot-enter-page-processing": "Question displayed to the bot owner which page should be processed.",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ro.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ro.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Robot:'"}*

```diff
@@ -1,14 +1,15 @@
 {
     "@metadata": {
         "authors": [
             "Minisarm",
             "Strainu"
         ]
     },
+    "pywikibot-bot-prefix": "Robot:",
     "pywikibot-cosmetic-changes": "; modific\u0103ri cosmetice",
     "pywikibot-enter-category-name": "V\u0103 rug\u0103m s\u0103 introduce\u021bi numele categoriei:",
     "pywikibot-enter-file-links-processing": "Leg\u0103turile c\u0103tre care fi\u0219ier ar trebui procesate?",
     "pywikibot-enter-finished-browser": "Ap\u0103sa\u021bi Enter odat\u0103 ce a\u021bi terminat cu navigatorul.",
     "pywikibot-enter-namespace-number": "V\u0103 rug\u0103m s\u0103 introduce\u021bi un spa\u021biu de nume dup\u0103 num\u0103rul s\u0103u:",
     "pywikibot-enter-new-text": "V\u0103 rug\u0103m s\u0103 introduce\u021bi noul text:",
     "pywikibot-enter-page-processing": "Ce pagin\u0103 ar trebui procesat\u0103?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ru.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ru.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Бот:'"}*

```diff
@@ -7,14 +7,15 @@
             "Movses",
             "Okras",
             "Rubin16",
             "Volkov",
             "\u0410\u043b\u0435\u043a\u0441\u0430\u043d\u0434\u0440 \u0421\u0438\u0433\u0430\u0447\u0451\u0432"
         ]
     },
+    "pywikibot-bot-prefix": "\u0411\u043e\u0442:",
     "pywikibot-cosmetic-changes": "; \u043a\u043e\u0441\u043c\u0435\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0435 \u0438\u0437\u043c\u0435\u043d\u0435\u043d\u0438\u044f",
     "pywikibot-enter-category-name": "\u041f\u043e\u0436\u0430\u043b\u0443\u0439\u0441\u0442\u0430, \u0432\u0432\u0435\u0434\u0438\u0442\u0435 \u043d\u0430\u0437\u0432\u0430\u043d\u0438\u0435 \u043a\u0430\u0442\u0435\u0433\u043e\u0440\u0438\u0438:",
     "pywikibot-enter-file-links-processing": "\u0421\u0441\u044b\u043b\u043a\u0438 \u043d\u0430 \u043a\u0430\u043a\u0443\u044e \u0441\u0442\u0440\u0430\u043d\u0438\u0446\u0443 \u0444\u0430\u0439\u043b\u0430 \u0441\u043b\u0435\u0434\u0443\u0435\u0442 \u043e\u0431\u0440\u0430\u0431\u043e\u0442\u0430\u0442\u044c?",
     "pywikibot-enter-finished-browser": "\u041d\u0430\u0436\u043c\u0438\u0442\u0435 \u043a\u043b\u0430\u0432\u0438\u0448\u0443 Enter, \u043a\u043e\u0433\u0434\u0430 \u0437\u0430\u043a\u043e\u043d\u0447\u0438\u0442\u0435 \u0432\u043d\u043e\u0441\u0438\u0442\u044c \u0438\u0437\u043c\u0435\u043d\u0435\u043d\u0438\u044f \u0432 \u0431\u0440\u0430\u0443\u0437\u0435\u0440\u0435.",
     "pywikibot-enter-namespace-number": "\u041f\u043e\u0436\u0430\u043b\u0443\u0439\u0441\u0442\u0430, \u0432\u0432\u0435\u0434\u0438\u0442\u0435 \u043d\u043e\u043c\u0435\u0440 \u043f\u0440\u043e\u0441\u0442\u0440\u0430\u043d\u0441\u0442\u0432\u0430 \u0438\u043c\u0451\u043d:",
     "pywikibot-enter-new-text": "\u041f\u043e\u0436\u0430\u043b\u0443\u0439\u0441\u0442\u0430, \u0432\u0432\u0435\u0434\u0438\u0442\u0435 \u043d\u043e\u0432\u044b\u0439 \u0442\u0435\u043a\u0441\u0442:",
     "pywikibot-enter-page-processing": "\u041a\u0430\u043a\u0430\u044f \u0441\u0442\u0440\u0430\u043d\u0438\u0446\u0430 \u0434\u043e\u043b\u0436\u043d\u0430 \u043e\u0431\u0440\u0430\u0431\u0430\u0442\u044b\u0432\u0430\u0442\u044c\u0441\u044f?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/sco.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sco.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9090909090909091%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Robot:'"}*

```diff
@@ -1,14 +1,15 @@
 {
     "@metadata": {
         "authors": [
             "Avicennasis",
             "John Reid"
         ]
     },
+    "pywikibot-bot-prefix": "Robot:",
     "pywikibot-cosmetic-changes": "; cosmetic chynges",
     "pywikibot-enter-category-name": "Please enter the category name:",
     "pywikibot-enter-file-links-processing": "Links til whit file page shid be processed?",
     "pywikibot-enter-finished-browser": "Press Enter whan finish't in browser.",
     "pywikibot-enter-namespace-number": "Please enter ae namespace bi its nummer:",
     "pywikibot-enter-new-text": "Please enter the new tex:",
     "pywikibot-enter-page-processing": "Whit page shid be processed?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/sk.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sk.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Bot:'"}*

```diff
@@ -4,14 +4,15 @@
             "Kusavica",
             "Teslaton",
             "Tom\u00e1\u0161Polonec",
             "Wizzard",
             "Yardom78"
         ]
     },
+    "pywikibot-bot-prefix": "Bot:",
     "pywikibot-cosmetic-changes": "; kozmetick\u00e9 zmeny",
     "pywikibot-enter-category-name": "Zadajte n\u00e1zov kateg\u00f3rie:",
     "pywikibot-enter-file-links-processing": "Odkazy na ktor\u00fa str\u00e1nku so s\u00faborom maj\u00fa by\u0165 spracovan\u00e9?",
     "pywikibot-enter-finished-browser": "Po ukon\u010den\u00ed \u010dinnosti v prehliada\u010di stla\u010dte Enter.",
     "pywikibot-enter-namespace-number": "Zadajte \u010d\u00edslo menn\u00e9ho priestoru:",
     "pywikibot-enter-new-text": "Zadajte nov\u00fd text:",
     "pywikibot-enter-page-processing": "Ktor\u00e1 str\u00e1nka m\u00e1 by\u0165 spracovan\u00e1?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/sl.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sl.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Bot:'"}*

```diff
@@ -3,14 +3,15 @@
         "authors": [
             "Dbc334",
             "Eleassar",
             "Irena Plahuta",
             "Mateju"
         ]
     },
+    "pywikibot-bot-prefix": "Bot:",
     "pywikibot-cosmetic-changes": "; oblikovne spremembe",
     "pywikibot-enter-category-name": "Prosimo, vnesite ime kategorije:",
     "pywikibot-enter-file-links-processing": "Povezava do katere strani datoteke naj bo obdelana?",
     "pywikibot-enter-finished-browser": "Ko kon\u010date v brskalniku, pritisnite vna\u0161alko (Enter).",
     "pywikibot-enter-namespace-number": "Prosimo, vnesite \u0161tevilko imenskega prostora.",
     "pywikibot-enter-new-text": "Prosimo, vnesite novo besedilo:",
     "pywikibot-enter-page-processing": "Katera stran naj bo obdelana?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/so.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/so.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9090909090909091%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Bot:'"}*

```diff
@@ -1,13 +1,14 @@
 {
     "@metadata": {
         "authors": [
             "Abshirdheere"
         ]
     },
+    "pywikibot-bot-prefix": "Bot:",
     "pywikibot-cosmetic-changes": "; Badal qurxin ah",
     "pywikibot-enter-category-name": "Fadlan gali magaca qaybta",
     "pywikibot-enter-file-links-processing": "Sawirada lagu uruuriyey bogagga shaqadoodu socoto",
     "pywikibot-enter-finished-browser": "Taabo (Enter) marka uu dhamaado browserka",
     "pywikibot-enter-namespace-number": "Fadlan gali namespace ee nambarkaan:",
     "pywikibot-enter-new-text": "Fadlan gali qoraalka cusub",
     "pywikibot-enter-page-processing": "Boggee ay tahay in laga shaqeeyo",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/sr.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sr.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Бот:'"}*

```diff
@@ -6,14 +6,15 @@
             "Kizule",
             "Milicevic01",
             "Rancher",
             "Sasa Stefanovic",
             "Zoranzoki21"
         ]
     },
+    "pywikibot-bot-prefix": "\u0411\u043e\u0442:",
     "pywikibot-cosmetic-changes": "; \u043a\u043e\u0437\u043c\u0435\u0442\u0438\u0447\u043a\u0435 \u0438\u0437\u043c\u0435\u043d\u0435",
     "pywikibot-enter-category-name": "\u0423\u043d\u0435\u0441\u0438\u0442\u0435 \u0438\u043c\u0435 \u043a\u0430\u0442\u0435\u0433\u043e\u0440\u0438\u0458\u0435:",
     "pywikibot-enter-file-links-processing": "\u0412\u0435\u0437\u0435 \u0434\u043e \u043a\u043e\u0458\u0435 \u0434\u0430\u0442\u043e\u0442\u0435\u043a\u0435 \u0436\u0435\u043b\u0438\u0442\u0435 \u0434\u0430 \u043e\u0431\u0440\u0430\u0434\u0438\u0442\u0435?",
     "pywikibot-enter-finished-browser": "\u041f\u0440\u0438\u0442\u0438\u0441\u043d\u0438\u0442\u0435 Enter \u043a\u0430\u0434\u0430 \u0437\u0430\u0432\u0440\u0448\u0438\u0442\u0435 \u0443\u043d\u043e\u0441 \u0438\u0437\u043c\u0435\u043d\u0430 \u0443 \u043f\u0440\u0435\u0433\u043b\u0435\u0434\u0430\u0447\u0443.",
     "pywikibot-enter-namespace-number": "\u0423\u043d\u0435\u0441\u0438\u0442\u0435 \u0438\u043c\u0435\u043d\u0441\u043a\u0438 \u043f\u0440\u043e\u0441\u0442\u043e\u0440 \u043f\u043e\u0440\u0435\u0434 \u045a\u0435\u0433\u043e\u0432\u043e\u0433 \u0431\u0440\u043e\u0458\u0430:",
     "pywikibot-enter-new-text": "\u0423\u043d\u0435\u0441\u0438\u0442\u0435 \u043d\u043e\u0432\u0438 \u0442\u0435\u043a\u0441\u0442:",
     "pywikibot-enter-page-processing": "\u041a\u043e\u0458\u0443 \u0441\u0442\u0440\u0430\u043d\u0438\u0446\u0443 \u0436\u0435\u043b\u0438\u0442\u0435 \u0434\u0430 \u043e\u0431\u0440\u0430\u0434\u0438\u0442\u0435?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/sv.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/vi.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48333333333333334%*

 * *Differences: {"'@metadata'": "{'authors': ['Minh Nguyen']}",*

 * * "'pywikibot-bot-prefix'": "'Bot:'",*

 * * "'pywikibot-cosmetic-changes'": "'; sửa cách trình bày'",*

 * * "'pywikibot-enter-category-name'": "'Xin vui lòng nhập tên thể loại:'",*

 * * "'pywikibot-enter-file-links-processing'": "'Nên xử lý các liên kết đến trang miêu tả tập tin "*

 * *                                            "nào?'",*

 * * "'pywikibot-enter-finished-browser'": "'Bấm Enter sau khi sửa đổi xong trong trình duyệt.'",*

 * * "'pywikibot-enter-namespace-number'": "'Xin vui lò […]*

```diff
@@ -1,27 +1,21 @@
 {
     "@metadata": {
         "authors": [
-            "Ainali",
-            "Anhn",
-            "Cybjit",
-            "Jopparn",
-            "Lokal Profil",
-            "Mj\u00e4lten",
-            "WikiPhoenix",
-            "skorpan"
+            "Minh Nguyen"
         ]
     },
-    "pywikibot-cosmetic-changes": "; kosmetiska \u00e4ndringar",
-    "pywikibot-enter-category-name": "Ange kategorinamnet:",
-    "pywikibot-enter-file-links-processing": "L\u00e4nkar till vilken filsida ska behandlas?",
-    "pywikibot-enter-finished-browser": "Tryck p\u00e5 Enter n\u00e4r du \u00e4r klar i webbl\u00e4saren.",
-    "pywikibot-enter-namespace-number": "Ange namnrymden via dess nummer:",
-    "pywikibot-enter-new-text": "Skriv in den nya texten:",
-    "pywikibot-enter-page-processing": "Vilken sida ska behandlas?",
-    "pywikibot-enter-xml-filename": "Ange XML-dumpens filnamn:",
-    "pywikibot-fixes-fckeditor": "Bot: \u00c5tg\u00e4rdar Rich-editor-html",
-    "pywikibot-fixes-html": "Bot: Konverterar/korrigerar HTML",
-    "pywikibot-fixes-isbn": "Bot: Formaterar ISBN",
-    "pywikibot-fixes-syntax": "Bot: Fixar wikisyntax",
-    "pywikibot-touch": "Pywikibot noll-redigering"
+    "pywikibot-bot-prefix": "Bot:",
+    "pywikibot-cosmetic-changes": "; s\u1eeda c\u00e1ch tr\u00ecnh b\u00e0y",
+    "pywikibot-enter-category-name": "Xin vui l\u00f2ng nh\u1eadp t\u00ean th\u1ec3 lo\u1ea1i:",
+    "pywikibot-enter-file-links-processing": "N\u00ean x\u1eed l\u00fd c\u00e1c li\u00ean k\u1ebft \u0111\u1ebfn trang mi\u00eau t\u1ea3 t\u1eadp tin n\u00e0o?",
+    "pywikibot-enter-finished-browser": "B\u1ea5m Enter sau khi s\u1eeda \u0111\u1ed5i xong trong tr\u00ecnh duy\u1ec7t.",
+    "pywikibot-enter-namespace-number": "Xin vui l\u00f2ng nh\u1eadp s\u1ed1 kh\u00f4ng gian t\u00ean:",
+    "pywikibot-enter-new-text": "Xin vui l\u00f2ng nh\u1eadp v\u0103n b\u1ea3n m\u1edbi:",
+    "pywikibot-enter-page-processing": "N\u00ean x\u1eed l\u00fd trang n\u00e0o?",
+    "pywikibot-enter-xml-filename": "Xin vui l\u00f2ng nh\u1eadp t\u00ean t\u1eadp tin c\u1ee7a b\u1ea3n sao l\u01b0u XML:",
+    "pywikibot-fixes-fckeditor": "Bot: S\u1eeda m\u00e3 HTML c\u1ee7a tr\u00ecnh so\u1ea1n th\u1ea3o c\u00f3 \u0111\u1ecbnh d\u1ea1ng",
+    "pywikibot-fixes-html": "Bot: Chuy\u1ec3n \u0111\u1ed5i/s\u1eeda HTML",
+    "pywikibot-fixes-isbn": "Bot: \u0110\u1ecbnh d\u1ea1ng ISBN",
+    "pywikibot-fixes-syntax": "Bot: S\u1eeda c\u00fa ph\u00e1p wiki",
+    "pywikibot-touch": "Pywikibot s\u1eeda \u0111\u1ed5i ch\u1ea1m"
 }
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/sw.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sw.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ta.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {"'pywikibot-bot-prefix'": "'தானியங்கி:'"}*

```diff
@@ -1,13 +1,14 @@
 {
     "@metadata": {
         "authors": [
             "Aswn",
             "\u0b9a\u0bc6\u0bb2\u0bcd\u0bb5\u0bbe"
         ]
     },
+    "pywikibot-bot-prefix": "\u0ba4\u0bbe\u0ba9\u0bbf\u0baf\u0b99\u0bcd\u0b95\u0bbf:",
     "pywikibot-cosmetic-changes": "; \u0bae\u0bc7\u0bb2\u0bcb\u0b9f\u0bcd\u0b9f\u0bae\u0bbe\u0ba9 \u0bae\u0bbe\u0bb1\u0bcd\u0bb1\u0b99\u0bcd\u0b95\u0bb3\u0bcd",
     "pywikibot-enter-category-name": "\u0baa\u0b95\u0bc1\u0baa\u0bcd\u0baa\u0bbf\u0ba9\u0bcd \u0baa\u0bc6\u0baf\u0bb0\u0bc8 \u0b87\u0b9f\u0bb5\u0bc1\u0bae\u0bcd:",
     "pywikibot-enter-new-text": "\u0baa\u0bc1\u0ba4\u0bbf\u0baf \u0b89\u0bb0\u0bc8\u0baf\u0bbf\u0ba9\u0bc8 \u0b87\u0b9f\u0bb5\u0bc1\u0bae\u0bcd:",
     "pywikibot-enter-page-processing": "\u0b8e\u0ba8\u0bcd\u0ba4 \u0baa\u0b95\u0bcd\u0b95\u0ba4\u0bcd\u0ba4\u0bbf\u0ba9\u0bc8 \u0b9a\u0bc6\u0baf\u0bb2\u0bbe\u0b95\u0bcd\u0b95\u0baa\u0bcd\u0baa\u0b9f \u0bb5\u0bc7\u0ba3\u0bcd\u0b9f\u0bc1\u0bae\u0bcd?",
     "pywikibot-fixes-isbn": "\u0ba4\u0bbe\u0ba9\u0bbf\u0baf\u0b99\u0bcd\u0b95\u0bbf: ISBN \u0b90 \u0bb5\u0b9f\u0bbf\u0bb5\u0bae\u0bc8\u0ba4\u0bcd\u0ba4\u0bb2\u0bcd"
 }
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/te.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/te.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9090909090909091%*

 * *Differences: {"'pywikibot-bot-prefix'": "'బాటు :'"}*

```diff
@@ -2,14 +2,15 @@
     "@metadata": {
         "authors": [
             "JVRKPRASAD",
             "Veeven",
             "\u0c30\u0c39\u0c4d\u0c2e\u0c3e\u0c28\u0c41\u0c26\u0c4d\u0c26\u0c40\u0c28\u0c4d"
         ]
     },
+    "pywikibot-bot-prefix": "\u0c2c\u0c3e\u0c1f\u0c41 :",
     "pywikibot-cosmetic-changes": "; \u0c2a\u0c48\u0c2a\u0c48 \u0c2e\u0c3e\u0c30\u0c4d\u0c2a\u0c41\u0c32\u0c41",
     "pywikibot-enter-category-name": "\u0c26\u0c2f\u0c1a\u0c47\u0c38\u0c3f \u0c35\u0c30\u0c4d\u0c17\u0c02 \u0c2a\u0c47\u0c30\u0c41 \u0c28\u0c2e\u0c4b\u0c26\u0c41 \u0c1a\u0c47\u0c2f\u0c02\u0c21\u0c3f:",
     "pywikibot-enter-file-links-processing": "\u0c32\u0c3f\u0c02\u0c15\u0c41\u0c32\u0c41 \u0c07\u0c26\u0c3f \u0c0f \u0c2b\u0c48\u0c32\u0c4d \u0c2a\u0c47\u0c1c\u0c40\u0c15\u0c3f \u0c38\u0c02\u0c35\u0c3f\u0c27\u0c3e\u0c28\u0c02 \u0c1a\u0c47\u0c2f\u0c3e\u0c32\u0c3f ?",
     "pywikibot-enter-finished-browser": "\u0c2c\u0c4d\u0c30\u0c4c\u0c1c\u0c30\u0c4d \u0c32\u0c4b \u0c2a\u0c42\u0c30\u0c4d\u0c24\u0c35\u0c17\u0c3e\u0c28\u0c47 \u0c0e\u0c02\u0c1f\u0c30\u0c4d \u0c2a\u0c4d\u0c30\u0c46\u0c38\u0c4d \u0c1a\u0c47\u0c2f\u0c02\u0c21\u0c3f.\n  .",
     "pywikibot-enter-namespace-number": "\u0c12\u0c15 \u0c28\u0c47\u0c2e\u0c4d\u200c\u0c38\u0c4d\u0c2a\u0c47\u0c38\u0c4d \u0c26\u0c3e\u0c28\u0c3f \u0c38\u0c02\u0c16\u0c4d\u0c2f \u0c26\u0c4d\u0c35\u0c3e\u0c30\u0c3e \u0c0e\u0c02\u0c1f\u0c30\u0c4d \u0c1a\u0c47\u0c2f\u0c02\u0c21\u0c3f:\n:",
     "pywikibot-enter-new-text": "\u0c26\u0c2f\u0c1a\u0c47\u0c38\u0c3f \u0c15\u0c4a\u0c24\u0c4d\u0c24 \u0c1f\u0c46\u0c15\u0c4d\u0c38\u0c4d\u0c1f\u0c41 \u0c0e\u0c02\u0c1f\u0c30\u0c4d \u0c1a\u0c46\u0c2f\u0c4d\u0c2f\u0c02\u0c21\u0c3f:",
     "pywikibot-enter-page-processing": "\u0c0f \u0c2a\u0c47\u0c1c\u0c40 \u0c38\u0c02\u0c35\u0c3f\u0c27\u0c3e\u0c28\u0c02 \u0c1a\u0c47\u0c2f\u0c3e\u0c32\u0c3f ?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/th.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/th.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'pywikibot-bot-prefix'": "'บอต:'"}*

```diff
@@ -3,14 +3,15 @@
         "authors": [
             "Aefgh39622",
             "Horus",
             "Nullzero",
             "Octahedron80"
         ]
     },
+    "pywikibot-bot-prefix": "\u0e1a\u0e2d\u0e15:",
     "pywikibot-cosmetic-changes": "; \u0e1b\u0e23\u0e31\u0e1a\u0e41\u0e15\u0e48\u0e07\u0e43\u0e2b\u0e49\u0e2d\u0e48\u0e32\u0e19\u0e07\u0e48\u0e32\u0e22",
     "pywikibot-enter-category-name": "\u0e01\u0e23\u0e38\u0e13\u0e32\u0e43\u0e2a\u0e48\u0e0a\u0e37\u0e48\u0e2d\u0e2b\u0e21\u0e27\u0e14\u0e2b\u0e21\u0e39\u0e48:",
     "pywikibot-enter-file-links-processing": "\u0e25\u0e34\u0e07\u0e01\u0e4c\u0e44\u0e1b\u0e22\u0e31\u0e07\u0e2b\u0e19\u0e49\u0e32\u0e44\u0e1f\u0e25\u0e4c\u0e43\u0e14\u0e04\u0e27\u0e23\u0e08\u0e30\u0e1b\u0e23\u0e30\u0e21\u0e27\u0e25\u0e1c\u0e25?",
     "pywikibot-enter-finished-browser": "\u0e01\u0e14 Enter \u0e40\u0e21\u0e37\u0e48\u0e2d\u0e17\u0e33\u0e07\u0e32\u0e19\u0e43\u0e19\u0e40\u0e1a\u0e23\u0e32\u0e27\u0e4c\u0e40\u0e0b\u0e2d\u0e23\u0e4c\u0e40\u0e23\u0e35\u0e22\u0e1a\u0e23\u0e49\u0e2d\u0e22\u0e41\u0e25\u0e49\u0e27",
     "pywikibot-enter-namespace-number": "\u0e01\u0e23\u0e38\u0e13\u0e32\u0e43\u0e2a\u0e48\u0e2b\u0e21\u0e32\u0e22\u0e40\u0e25\u0e02\u0e02\u0e2d\u0e07\u0e40\u0e19\u0e21\u0e2a\u0e40\u0e1b\u0e0b:",
     "pywikibot-enter-new-text": "\u0e01\u0e23\u0e38\u0e13\u0e32\u0e43\u0e2a\u0e48\u0e02\u0e49\u0e2d\u0e04\u0e27\u0e32\u0e21\u0e43\u0e2b\u0e21\u0e48:",
     "pywikibot-enter-page-processing": "\u0e2b\u0e19\u0e49\u0e32\u0e43\u0e14\u0e04\u0e27\u0e23\u0e08\u0e30\u0e1b\u0e23\u0e30\u0e21\u0e27\u0e25\u0e1c\u0e25?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/tly.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/tly.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9090909090909091%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Робот:'"}*

```diff
@@ -1,13 +1,14 @@
 {
     "@metadata": {
         "authors": [
             "\u0413\u0443\u0441\u0435\u0439\u043d"
         ]
     },
+    "pywikibot-bot-prefix": "\u0420\u043e\u0431\u043e\u0442:",
     "pywikibot-cosmetic-changes": "; \u043a\u043e\u0441\u043c\u0435\u0442\u0438\u043a\u04d9 \u0434\u04d9\u0433\u0438\u0448\u043e\u043d",
     "pywikibot-enter-category-name": "\u0417\u04d9\u04bb\u043c\u04d9\u0442 \u043d\u044b\u0431\u043e, \u0442\u0438\u0441\u043f\u0438\u0440\u0438 \u043d\u043e\u043c \u0434\u04d9\u0493\u0430\u043d\u0434\u04d9\u043d:",
     "pywikibot-enter-file-links-processing": "\u0421\u04d9\u0431\u043e\u043d\u043e\u043d \u0431\u04d9 \u043a\u043e\u043d \u0433\u044b\u043b\u04d9 \u0448\u0438\u043a\u0438\u043b\u043e\u043d \u0441\u04d9\u04bb\u0438\u0444\u04d9 \u0431\u04d9\u043f\u0435 \u0435\u043c\u043e\u043b \u043a\u0430\u0440\u0434\u04d9 \u0431\u044b\u0431\u0443\u043d?",
     "pywikibot-enter-finished-browser": "Enter \u0435\u0433\u04d9\u0442\u04d9\u0434\u044b\u0433\u043c\u04d9 \u0435\u0433\u04d9\u0442\u04d9\u0458\u043e\u043d, \u043a\u0435\u0458\u043d\u04d9 \u043e\u0431\u04d9\u0440\u04d9\u0445\u043d\u0435\u0458\u043e\u043d \u0431\u04d9 \u0431\u0440\u0430\u0443\u0437\u0435\u0440 \u0434\u04d9\u0433\u0438\u0448\u0438\u0458\u043e\u043d \u0434\u04d9\u0493\u0430\u043d\u0434\u0435\u0458.",
     "pywikibot-enter-namespace-number": "\u0417\u04d9\u04bb\u043c\u04d9\u0442 \u043d\u044b\u0431\u043e, \u043d\u043e\u043c\u043e\u043d \u043c\u04d9\u043a\u043e\u043d \u043d\u0443\u043c\u0440\u04d9 \u0434\u04d9\u0493\u0430\u043d\u0434\u04d9\u043d:",
     "pywikibot-enter-new-text": "\u0417\u04d9\u04bb\u043c\u04d9\u0442 \u043d\u044b\u0431\u043e, \u043d\u0443\u0458\u04d9 \u043c\u04d9\u0442\u043d \u0434\u04d9\u0493\u0430\u043d\u0434\u04d9\u043d:",
     "pywikibot-enter-page-processing": "\u041a\u043e\u043d \u0433\u044b\u043b\u04d9 \u0441\u04d9\u04bb\u0438\u0444\u04d9 \u0431\u04d9\u043f\u0435 \u0435\u043c\u043e\u043b \u043a\u0430\u0440\u0434\u04d9 \u0431\u044b\u0431\u0443?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/tr.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/tr.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Bot:'"}*

```diff
@@ -7,14 +7,15 @@
             "Khutuck",
             "McAang",
             "Meelo",
             "Stultiwikia",
             "Vito Genovese"
         ]
     },
+    "pywikibot-bot-prefix": "Bot:",
     "pywikibot-cosmetic-changes": "; kozmetik de\u011fi\u015fiklikler",
     "pywikibot-enter-category-name": "L\u00fctfen kategori ad\u0131n\u0131 girin:",
     "pywikibot-enter-file-links-processing": "Hangi dosya sayfas\u0131n\u0131n ba\u011flant\u0131lar\u0131 i\u015flenmeli?",
     "pywikibot-enter-finished-browser": "Taray\u0131c\u0131da bitti\u011finde Enter tu\u015funa bas\u0131n.",
     "pywikibot-enter-namespace-number": "L\u00fctfen numaras\u0131na g\u00f6re bir ad alan\u0131 girin:",
     "pywikibot-enter-new-text": "L\u00fctfen yeni metni girin:",
     "pywikibot-enter-page-processing": "Hangi sayfa i\u015flenmeli?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/uk.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/uk.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'pywikibot-bot-prefix'": "'Бот:'"}*

```diff
@@ -8,14 +8,15 @@
             "Dmitry Nikitin",
             "Ice bulldog",
             "Movses",
             "\u0410\u0442\u0430",
             "\u0422\u0435\u0441\u0442"
         ]
     },
+    "pywikibot-bot-prefix": "\u0411\u043e\u0442:",
     "pywikibot-cosmetic-changes": "; \u043a\u043e\u0441\u043c\u0435\u0442\u0438\u0447\u043d\u0456 \u0437\u043c\u0456\u043d\u0438",
     "pywikibot-enter-category-name": "\u0412\u0432\u0435\u0434\u0456\u0442\u044c \u043d\u0430\u0437\u0432\u0443 \u043a\u0430\u0442\u0435\u0433\u043e\u0440\u0456\u0457:",
     "pywikibot-enter-file-links-processing": "\u041f\u043e\u0441\u0438\u043b\u0430\u043d\u043d\u044f \u043d\u0430 \u044f\u043a\u0456 \u0444\u0430\u0439\u043b\u0438 \u0441\u043b\u0456\u0434 \u043e\u0431\u0440\u043e\u0431\u0438\u0442\u0438?",
     "pywikibot-enter-finished-browser": "\u041d\u0430\u0442\u0438\u0441\u043d\u0456\u0442\u044c Enter, \u043a\u043e\u043b\u0438 \u0437\u0430\u0432\u0435\u0440\u0448\u0438\u0442\u0435 \u0440\u0435\u0434\u0430\u0433\u0443\u0432\u0430\u043d\u043d\u044f \u0443 \u0431\u0440\u0430\u0443\u0437\u0435\u0440\u0456.",
     "pywikibot-enter-namespace-number": "\u0412\u0432\u0435\u0434\u0456\u0442\u044c \u043d\u043e\u043c\u0435\u0440 \u043f\u0440\u043e\u0441\u0442\u043e\u0440\u0443 \u043d\u0430\u0437\u0432:",
     "pywikibot-enter-new-text": "\u0412\u0432\u0435\u0434\u0456\u0442\u044c \u043d\u043e\u0432\u0438\u0439 \u0442\u0435\u043a\u0441\u0442:",
     "pywikibot-enter-page-processing": "\u042f\u043a\u0456 \u0441\u0442\u043e\u0440\u0456\u043d\u043a\u0438 \u043f\u043e\u0442\u0440\u0456\u0431\u043d\u043e \u043f\u0435\u0440\u0435\u0440\u043e\u0431\u0438\u0442\u0438?",
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/ur.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ur.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/scripts/i18n/pywikibot/yue.json` & `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/zh.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4166666666666667%*

 * *Differences: {"'@metadata'": "{'authors': ['Alex Shih-Han Lin', 'Anakmalaysia', 'Hydra', 'Liuxinyu970226', "*

 * *                "'Qiyue2001', 'VulpesVulpes825', 'Xiplus', 'Yfdyh000']}",*

 * * "'pywikibot-bot-prefix'": "'机器人：'",*

 * * "'pywikibot-cosmetic-changes'": "'；整理源码'",*

 * * "'pywikibot-enter-category-name'": "'请输入分类名称：'",*

 * * "'pywikibot-enter-file-links-processing'": "'哪个文件的链接需要处理？'",*

 * * "'pywikibot-enter-finished-browser'": "'当浏览器编辑结束时，请按回车键。'",*

 * * "'pywikibot-enter-namespace-number'": "'请输入命名空间编号：'",*

 * * "'pywikibot-enter-new-text'": "' […]*

```diff
@@ -1,19 +1,28 @@
 {
     "@metadata": {
         "authors": [
-            "Hello903hello",
-            "Shinjiman"
+            "Alex Shih-Han Lin",
+            "Anakmalaysia",
+            "Hydra",
+            "Liuxinyu970226",
+            "Qiyue2001",
+            "VulpesVulpes825",
+            "Xiplus",
+            "Yfdyh000"
         ]
     },
-    "pywikibot-enter-category-name": "\u8acb\u8f38\u5165\u5206\u985e\u540d\uff1a",
-    "pywikibot-enter-file-links-processing": "\u6709\u908a\u5572\u6a94\u6848\u7248\u5605\u62ce\u8981\u8655\u7406\uff1f",
-    "pywikibot-enter-finished-browser": "\u55ba\u700f\u89bd\u5668\u5b8c\u6210\u7de8\u8f2f\u4e4b\u5f8c\u64b3Enter\u63a3\u3002",
-    "pywikibot-enter-namespace-number": "\u8acb\u8f38\u5165\u7a7a\u9593\u540d\u5605\u51a7\u5df4\uff1a",
-    "pywikibot-enter-new-text": "\u8acb\u8f38\u5165\u65b0\u5b57\uff1a",
-    "pywikibot-enter-page-processing": "\u61c9\u8a72\u53bb\u8655\u7406\u908a\u7248\uff1f",
-    "pywikibot-enter-xml-filename": "\u8acb\u8f38\u5165XML\u50be\u5370\u5605\u6a94\u540d\uff1a",
-    "pywikibot-fixes-fckeditor": "\u6a5f\u68b0\u4eba\uff1a\u4fee\u6b63\u8996\u89ba\u7de8\u8f2f\u5668HTML",
-    "pywikibot-fixes-html": "\u6a5f\u68b0\u4eba\uff1a\u8f49\u63db/\u4fee\u6b63HTML",
-    "pywikibot-fixes-syntax": "\u6a5f\u68b0\u4eba\uff1a\u4fee\u6b63wiki\u8a9e\u6cd5",
-    "pywikibot-touch": "Pywikibot touch\u7de8\u8f2f"
+    "pywikibot-bot-prefix": "\u673a\u5668\u4eba\uff1a",
+    "pywikibot-cosmetic-changes": "\uff1b\u6574\u7406\u6e90\u7801",
+    "pywikibot-enter-category-name": "\u8bf7\u8f93\u5165\u5206\u7c7b\u540d\u79f0\uff1a",
+    "pywikibot-enter-file-links-processing": "\u54ea\u4e2a\u6587\u4ef6\u7684\u94fe\u63a5\u9700\u8981\u5904\u7406\uff1f",
+    "pywikibot-enter-finished-browser": "\u5f53\u6d4f\u89c8\u5668\u7f16\u8f91\u7ed3\u675f\u65f6\uff0c\u8bf7\u6309\u56de\u8f66\u952e\u3002",
+    "pywikibot-enter-namespace-number": "\u8bf7\u8f93\u5165\u547d\u540d\u7a7a\u95f4\u7f16\u53f7\uff1a",
+    "pywikibot-enter-new-text": "\u8bf7\u8f93\u5165\u65b0\u6587\u672c\uff1a",
+    "pywikibot-enter-page-processing": "\u54ea\u4e2a\u9875\u9762\u9700\u8981\u5904\u7406\uff1f",
+    "pywikibot-enter-xml-filename": "\u8bf7\u8f93\u5165XML\u8f6c\u50a8\u7684\u6587\u4ef6\u540d\uff1a",
+    "pywikibot-fixes-fckeditor": "\u673a\u5668\u4eba\uff1a\u4fee\u590d\u5bcc\u7f16\u8f91\u5668html",
+    "pywikibot-fixes-html": "\u673a\u5668\u4eba\uff1a\u8f6c\u6362/\u4fee\u590dHTML",
+    "pywikibot-fixes-isbn": "\u673a\u5668\u4eba\uff1aISBN\u683c\u5f0f\u5316",
+    "pywikibot-fixes-syntax": "\u673a\u5668\u4eba\uff1a\u4fee\u590dwiki\u8bed\u6cd5",
+    "pywikibot-touch": "Pywikibot\u505a\u4e86\u5c0f\u7f16\u8f91"
 }
```

### Comparing `pywikibot-8.0.3/pywikibot/scripts/login.py` & `pywikibot-8.0.4/pywikibot/scripts/login.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/scripts/preload_sites.py` & `pywikibot-8.0.4/pywikibot/scripts/preload_sites.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/scripts/shell.py` & `pywikibot-8.0.4/pywikibot/scripts/shell.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/scripts/version.py` & `pywikibot-8.0.4/pywikibot/scripts/version.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/scripts/wrapper.py` & `pywikibot-8.0.4/pywikibot/scripts/wrapper.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/site/__init__.py` & `pywikibot-8.0.4/pywikibot/site/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/site/_apisite.py` & `pywikibot-8.0.4/pywikibot/site/_apisite.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,19 +114,21 @@
         fam: Union[str, 'pywikibot.family.Family', None] = None,
         user: Optional[str] = None
     ) -> None:
         """Initializer."""
         super().__init__(code, fam, user)
         self._globaluserinfo: Dict[Union[int, str], Any] = {}
         self._interwikimap = _InterwikiMap(self)
-        self._loginstatus = login.LoginStatus.NOT_ATTEMPTED
         self._msgcache: Dict[str, str] = {}
         self._paraminfo = api.ParamInfo(self)
         self._siteinfo = Siteinfo(self)
         self._tokens = TokenWallet(self)
+        self._loginstatus = login.LoginStatus.NOT_ATTEMPTED
+        with suppress(SiteDefinitionError):
+            self.login(cookie_only=True)
 
     def __getstate__(self) -> Dict[str, Any]:
         """Remove TokenWallet before pickling, for security reasons."""
         state = super().__getstate__()
         del state['_tokens']
         del state['_interwikimap']
         return state
@@ -320,27 +322,34 @@
         """Check whether OAuth token is set for this site."""
         auth_token = http.get_authentication(self.base_url(''))
         return auth_token is not None and len(auth_token) == 4
 
     def login(
         self,
         autocreate: bool = False,
-        user: Optional[str] = None
+        user: Optional[str] = None,
+        *,
+        cookie_only: bool = False
     ) -> None:
         """Log the user in if not already logged in.
 
-        .. versionchanged:: 8.0
-           lazy load cookies when logging in.
+        .. versionchanged:: 8.0.0
+           lazy load cookies when logging in. This was dropped in 8.0.4
+        .. versionchanged:: 8.0.4
+           the *cookie_only* parameter was added and cookies are loaded
+           whenever the site is initialized.
 
         .. seealso:: :api:`Login`
 
         :param autocreate: if true, allow auto-creation of the account
             using unified login
         :param user: bot user name. Overrides the username set by
             BaseSite initializer parameter or user config setting
+        :param cookie_only: Only try to login from cookie but do not
+            force to login with username/password settings.
 
         :raises pywikibot.exceptions.NoUsernameError: Username is not
             recognised by the site.
         """
         # TODO: this should include an assert that loginstatus
         #       is not already IN_PROGRESS, however the
         #       login status may be left 'IN_PROGRESS' because
@@ -400,31 +409,30 @@
                              'expect as {right}'
                              .format(site=self,
                                      wrong=self.userinfo['name'],
                                      right=self.username()))
 
             raise NoUsernameError(error_msg)
 
-        login_manager = login.ClientLoginManager(site=self,
-                                                 user=self.username())
-        if login_manager.login(retry=True, autocreate=autocreate):
-            self._username = login_manager.username
-            del self.userinfo  # force reloading
-
-            # load userinfo
-            if self.userinfo['name'] == self.username():
-                self._loginstatus = login.LoginStatus.AS_USER
-                return
-
-            pywikibot.error('{} != {} after {}.login() and successful '
-                            '{}.login()'
-                            .format(self.userinfo['name'],
-                                    self.username(),
-                                    type(self).__name__,
-                                    type(login_manager).__name__))
+        if not cookie_only:
+            login_manager = login.ClientLoginManager(site=self,
+                                                     user=self.username())
+            if login_manager.login(retry=True, autocreate=autocreate):
+                self._username = login_manager.username
+                del self.userinfo  # force reloading
+
+                # load userinfo
+                if self.userinfo['name'] == self.username():
+                    self._loginstatus = login.LoginStatus.AS_USER
+                    return
+
+                pywikibot.error(
+                    f"{self.userinfo['name']} != {self.username()} after "
+                    f'{type(self).__name__}.login() and successful '
+                    f'{type(login_manager).__name__}.login()')
 
         self._loginstatus = login.LoginStatus.NOT_LOGGED_IN  # failure
 
     def _relogin(self) -> None:
         """Force a login sequence without logging out, using the current user.
 
         This is an internal function which is used to re-login when
@@ -534,15 +542,16 @@
             )
             uidata = uirequest.submit()
             assert 'query' in uidata, \
                    "API userinfo response lacks 'query' key"
             assert 'userinfo' in uidata['query'], \
                    "API userinfo response lacks 'userinfo' key"
             self._userinfo = uidata['query']['userinfo']
-            if 'anon' in self._userinfo or not self._userinfo.get('id'):
+            if self._loginstatus != login.LoginStatus.IN_PROGRESS \
+               and ('anon' in self._userinfo or not self._userinfo.get('id')):
                 pywikibot.warning('No user is logged in on site {}'
                                   .format(self))
         return self._userinfo
 
     @userinfo.deleter
     def userinfo(self) -> None:
         """Delete cached userinfo.
```

### Comparing `pywikibot-8.0.3/pywikibot/site/_basesite.py` & `pywikibot-8.0.4/pywikibot/site/_basesite.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/site/_datasite.py` & `pywikibot-8.0.4/pywikibot/site/_datasite.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/site/_decorators.py` & `pywikibot-8.0.4/pywikibot/site/_decorators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/site/_extensions.py` & `pywikibot-8.0.4/pywikibot/site/_extensions.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/site/_generators.py` & `pywikibot-8.0.4/pywikibot/site/_generators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/site/_interwikimap.py` & `pywikibot-8.0.4/pywikibot/site/_interwikimap.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/site/_namespace.py` & `pywikibot-8.0.4/pywikibot/site/_namespace.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/site/_obsoletesites.py` & `pywikibot-8.0.4/pywikibot/site/_obsoletesites.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/site/_siteinfo.py` & `pywikibot-8.0.4/pywikibot/site/_siteinfo.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/site/_tokenwallet.py` & `pywikibot-8.0.4/pywikibot/site/_tokenwallet.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/site/_upload.py` & `pywikibot-8.0.4/pywikibot/site/_upload.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/site_detect.py` & `pywikibot-8.0.4/pywikibot/site_detect.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/specialbots/_unlink.py` & `pywikibot-8.0.4/pywikibot/specialbots/_unlink.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/specialbots/_upload.py` & `pywikibot-8.0.4/pywikibot/specialbots/_upload.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/textlib.py` & `pywikibot-8.0.4/pywikibot/textlib.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/throttle.py` & `pywikibot-8.0.4/pywikibot/throttle.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/time.py` & `pywikibot-8.0.4/pywikibot/time.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/titletranslate.py` & `pywikibot-8.0.4/pywikibot/titletranslate.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/tools/__init__.py` & `pywikibot-8.0.4/pywikibot/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/tools/_deprecate.py` & `pywikibot-8.0.4/pywikibot/tools/_deprecate.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/tools/_logging.py` & `pywikibot-8.0.4/pywikibot/tools/_logging.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/tools/_unidata.py` & `pywikibot-8.0.4/pywikibot/tools/_unidata.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/tools/chars.py` & `pywikibot-8.0.4/pywikibot/tools/chars.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/tools/collections.py` & `pywikibot-8.0.4/pywikibot/tools/collections.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/tools/djvu.py` & `pywikibot-8.0.4/pywikibot/tools/djvu.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/tools/formatter.py` & `pywikibot-8.0.4/pywikibot/tools/formatter.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/tools/itertools.py` & `pywikibot-8.0.4/pywikibot/tools/itertools.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/tools/threading.py` & `pywikibot-8.0.4/pywikibot/tools/threading.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/userinterfaces/__init__.py` & `pywikibot-8.0.4/pywikibot/userinterfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/userinterfaces/_interface_base.py` & `pywikibot-8.0.4/pywikibot/userinterfaces/_interface_base.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/userinterfaces/buffer_interface.py` & `pywikibot-8.0.4/pywikibot/userinterfaces/buffer_interface.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/userinterfaces/gui.py` & `pywikibot-8.0.4/pywikibot/userinterfaces/gui.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/userinterfaces/terminal_interface_base.py` & `pywikibot-8.0.4/pywikibot/userinterfaces/terminal_interface_base.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/userinterfaces/terminal_interface_unix.py` & `pywikibot-8.0.4/pywikibot/userinterfaces/terminal_interface_unix.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/userinterfaces/terminal_interface_win32.py` & `pywikibot-8.0.4/pywikibot/userinterfaces/terminal_interface_win32.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/userinterfaces/transliteration.py` & `pywikibot-8.0.4/pywikibot/userinterfaces/transliteration.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/version.py` & `pywikibot-8.0.4/pywikibot/version.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot/xmlreader.py` & `pywikibot-8.0.4/pywikibot/xmlreader.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.3/pywikibot.egg-info/PKG-INFO` & `pywikibot-8.0.4/pywikibot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywikibot
-Version: 8.0.3
+Version: 8.0.4
 Summary: Python MediaWiki Bot Framework
 Home-page: https://www.mediawiki.org/wiki/Manual:Pywikibot
 Download-URL: https://pywikibot.toolforge.org/
 Maintainer: The Pywikibot team
 Maintainer-email: pywikibot@lists.wikimedia.org
 License: MIT License
 Project-URL: Documentation, https://doc.wikimedia.org/pywikibot/stable/
@@ -257,15 +257,17 @@
 
 Roadmap
 =======
 
 Current release
 ---------------
 
-* Add support for ckb-wiktionary (T332093)
+* L10N Updates
+* Minimal needed mwparserfromhell was decreased to 0.5.2 (T326498, T327600)
+* No longer lazy load password cookies (T271858, T326779, T329132, T330488, T331315)
 
 
 Deprecations
 ------------
 
 * 8.0.0: Timestamp.clone()method is deprecated
   in favour of ``Timestamp.replace()`` method.
```

### Comparing `pywikibot-8.0.3/pywikibot.egg-info/SOURCES.txt` & `pywikibot-8.0.4/pywikibot.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -232,14 +232,15 @@
 pywikibot/scripts/i18n/pywikibot/sr.json
 pywikibot/scripts/i18n/pywikibot/su.json
 pywikibot/scripts/i18n/pywikibot/sv.json
 pywikibot/scripts/i18n/pywikibot/sw.json
 pywikibot/scripts/i18n/pywikibot/szl.json
 pywikibot/scripts/i18n/pywikibot/ta.json
 pywikibot/scripts/i18n/pywikibot/te.json
+pywikibot/scripts/i18n/pywikibot/tg.json
 pywikibot/scripts/i18n/pywikibot/th.json
 pywikibot/scripts/i18n/pywikibot/tk.json
 pywikibot/scripts/i18n/pywikibot/tl.json
 pywikibot/scripts/i18n/pywikibot/tly.json
 pywikibot/scripts/i18n/pywikibot/tr.json
 pywikibot/scripts/i18n/pywikibot/tt.json
 pywikibot/scripts/i18n/pywikibot/uk.json
```

### Comparing `pywikibot-8.0.3/pywikibot.egg-info/requires.txt` & `pywikibot-8.0.4/pywikibot.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-mwparserfromhell>=0.6.3
+mwparserfromhell>=0.5.2
 
 [:python_version < "3.7"]
 requests<2.28.0,>=2.21.0
 setuptools<59.7.0,>=40.8.0
 
 [:python_version >= "3.10"]
 setuptools>=48.0.0
```

### Comparing `pywikibot-8.0.3/setup.py` & `pywikibot-8.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
 extra_deps.update(script_deps)
 extra_deps.update({'scripts': [i for k, v in script_deps.items() for i in v]})
 
 # ------- setup install_requires ------- #
 # packages which are mandatory
 dependencies = [
-    'mwparserfromhell>=0.6.3',
+    'mwparserfromhell>=0.5.2',
     'requests>=2.21.0, <2.28.0; python_version < "3.7"',
     'requests>=2.21.0; python_version>="3.7"',
     # PEP 440
     'setuptools>=48.0.0 ; python_version >= "3.10"',
     'setuptools>=40.8.0 ; python_version >= "3.7" and python_version < "3.10"',
     'setuptools>=40.8.0, <59.7.0 ; python_version < "3.7"',
 ]
```

### Comparing `pywikibot-8.0.3/tests/tests_tests.py` & `pywikibot-8.0.4/tests/tests_tests.py`

 * *Files identical despite different names*

