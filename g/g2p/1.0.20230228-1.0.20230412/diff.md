# Comparing `tmp/g2p-1.0.20230228.tar.gz` & `tmp/g2p-1.0.20230412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g2p-1.0.20230228.tar", last modified: Tue Feb 28 22:34:00 2023, max compression
+gzip compressed data, was "g2p-1.0.20230412.tar", last modified: Wed Apr 12 22:08:22 2023, max compression
```

## Comparing `g2p-1.0.20230228.tar` & `g2p-1.0.20230412.tar`

### file list

```diff
@@ -1,422 +1,430 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.519989 g2p-1.0.20230228/
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-02-28 22:33:45.000000 g2p-1.0.20230228/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-02-28 22:33:45.000000 g2p-1.0.20230228/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15114 2023-02-28 22:34:00.519989 g2p-1.0.20230228/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14629 2023-02-28 22:33:45.000000 g2p-1.0.20230228/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.479989 g2p-1.0.20230228/g2p/
--rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    27352 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.479989 g2p-1.0.20230228/g2p/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)    21063 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/create_fallback_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/create_ipa_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.479989 g2p-1.0.20230228/g2p/mappings/langs/
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.479989 g2p-1.0.20230228/g2p/mappings/langs/alq/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/alq/alq_to_ipa.csv
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/alq/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.483989 g2p-1.0.20230228/g2p/mappings/langs/atj/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/atj/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/atj/atj_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/atj/atj_to_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/atj/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.483989 g2p-1.0.20230228/g2p/mappings/langs/ckt/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/ckt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/ckt/ckt_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/ckt/ckt_to_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/ckt/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.483989 g2p-1.0.20230228/g2p/mappings/langs/clc/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/clc/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/clc/doulos.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.483989 g2p-1.0.20230228/g2p/mappings/langs/crg/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/crg/abbreviations.csv
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/crg/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/crg/crg-dv-to-crg-ipa.csv
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/crg/crg-tmd-to-crg-ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.483989 g2p-1.0.20230228/g2p/mappings/langs/crj/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/crj/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/crj/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/crj/crj_equiv.json
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/crj/crj_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/crj/crj_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.483989 g2p-1.0.20230228/g2p/mappings/langs/crk/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/crk/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/crk/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/crk/crk-no-symbols_to_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/crk/crk_to_crk-no-symbols.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.483989 g2p-1.0.20230228/g2p/mappings/langs/crl/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/crl/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/crl/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/crl/crl_equiv.json
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/crl/crl_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/crl/crl_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.483989 g2p-1.0.20230228/g2p/mappings/langs/crm/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/crm/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/crm/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12358 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/crm/crm_equiv.json
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/crm/crm_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/crm/crm_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.483989 g2p-1.0.20230228/g2p/mappings/langs/crx/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/crx/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/crx/stella_orth_to_syllabics.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/crx/stella_syllabics_to_orth.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.487989 g2p-1.0.20230228/g2p/mappings/langs/csw/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/csw/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/csw/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10982 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/csw/csw_equiv.json
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/csw/csw_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/csw/csw_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.487989 g2p-1.0.20230228/g2p/mappings/langs/ctp/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/ctp/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/ctp/ctp_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/ctp/ctp_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.487989 g2p-1.0.20230228/g2p/mappings/langs/dan/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/dan/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/dan/dan_abbs.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/dan/dan_to_dummy.json
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/dan/dan_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.491989 g2p-1.0.20230228/g2p/mappings/langs/eng/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/eng/cmu_sphinx.metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)  3231441 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/eng/cmudict_SPHINX_40.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/eng/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/eng/dummy_to_arpabet.json
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/eng/eng_inventory.json
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/eng/eng_ipa_to_arpabet.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.491989 g2p-1.0.20230228/g2p/mappings/langs/fin/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/fin/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/fin/fin_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.491989 g2p-1.0.20230228/g2p/mappings/langs/font-encodings/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/font-encodings/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/font-encodings/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/font-encodings/fn_unicode.csv
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/font-encodings/hei_doulos.csv
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/font-encodings/hei_times.csv
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/font-encodings/nav_times.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.491989 g2p-1.0.20230228/g2p/mappings/langs/fra/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/fra/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/fra/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/fra/fra_abbs.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/fra/fra_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.495989 g2p-1.0.20230228/g2p/mappings/langs/generated/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/alq-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/atj-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/crg-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/crk-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/dan-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/fin-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/fra-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/gla-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/gwi-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/haa-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/ikt-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/ikt-ipa_to_hamming-eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/iku-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/iku-ipa_to_hamming-eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)    10603 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/iku-sro-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/lml-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/mic-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/moe-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/moh-equiv_to_dummy.json
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/moh-equiv_to_hamming_dummy.json
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/moh-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/moh-ipa_to_hamming-eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/oji-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/oka-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/see-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/str-equiv_to_dummy.json
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/str-equiv_to_hamming_dummy.json
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/str-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/str-ipa_to_hamming-eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)    13035 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/tau-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/tce-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/tli-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/ttm-ipa_to_eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/und-ascii_to_dummy.json
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/und-ascii_to_hamming_dummy.json
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/und-ipa_to_hamming-eng-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/generated/win-ipa_to_eng-ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.495989 g2p-1.0.20230228/g2p/mappings/langs/git/
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/git/APA.csv
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/git/Ortho_variables.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/git/Orthography.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/git/Orthography_Deterministic.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/git/RAPA.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/git/RAPA_Deterministic.csv
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/git/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/git/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/git/equiv.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/git/git_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/git/git_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.495989 g2p-1.0.20230228/g2p/mappings/langs/gla/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/gla/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/gla/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/gla/gla_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.495989 g2p-1.0.20230228/g2p/mappings/langs/gwi/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/gwi/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/gwi/gwi_equiv.json
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/gwi/gwi_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.495989 g2p-1.0.20230228/g2p/mappings/langs/haa/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/haa/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/haa/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/haa/haa_abbs.csv
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/haa/haa_equiv.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/haa/haa_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.499989 g2p-1.0.20230228/g2p/mappings/langs/ikt/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/ikt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/ikt/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/ikt/ikt_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.499989 g2p-1.0.20230228/g2p/mappings/langs/iku/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/iku/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/iku/iku_equiv_to_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/iku/iku_sro_to_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/iku/iku_to_iku_equiv.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.499989 g2p-1.0.20230228/g2p/mappings/langs/kkz/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/kkz/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/kkz/kkz_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/kkz/kkz_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.499989 g2p-1.0.20230228/g2p/mappings/langs/kwk/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/kwk/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/kwk/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/kwk/kwk_boas_to_umista.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/kwk/kwk_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/kwk/kwk_napa_to_ipa.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/kwk/kwk_napa_to_xsampa.json
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/kwk/kwk_umista_to_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/kwk/kwk_xsampa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/kwk/napa_equiv_ubc.csv
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/kwk/napa_equiv_uvic.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/kwk/umista_equiv.csv
--rw-r--r--   0 runner    (1001) docker     (123)   308837 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/langs.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.499989 g2p-1.0.20230228/g2p/mappings/langs/lml/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/lml/abbreviations.csv
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/lml/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/lml/lml_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.499989 g2p-1.0.20230228/g2p/mappings/langs/mic/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/mic/abbreviations.csv
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/mic/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/mic/mic_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.499989 g2p-1.0.20230228/g2p/mappings/langs/moe/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/moe/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/moe/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/moe/moe_abbs.csv
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/moe/moe_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.499989 g2p-1.0.20230228/g2p/mappings/langs/moh/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/moh/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/moh/abbreviations.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/moh/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/moh/moh_equiv.json
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/moh/moh_to_festival.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/moh/moh_to_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/network.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.503989 g2p-1.0.20230228/g2p/mappings/langs/norm/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/norm/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/norm/panphon_preprocessor.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/norm/tone-map.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.503989 g2p-1.0.20230228/g2p/mappings/langs/oji/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/oji/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/oji/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/oji/oji_syllabics_to_orth.csv
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/oji/oji_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.503989 g2p-1.0.20230228/g2p/mappings/langs/oka/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/oka/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/oka/oka_equiv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/oka/oka_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.503989 g2p-1.0.20230228/g2p/mappings/langs/see/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/see/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/see/see_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.503989 g2p-1.0.20230228/g2p/mappings/langs/srs/
--rwxr-xr-x   0 runner    (1001) docker     (123)      535 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/srs/config.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     2109 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/srs/srs_ipa_to_eng_ipa.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     6083 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/srs/srs_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.503989 g2p-1.0.20230228/g2p/mappings/langs/str/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/str/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/str/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/str/str_equiv.json
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/str/str_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.503989 g2p-1.0.20230228/g2p/mappings/langs/tau/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/tau/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/tau/tau_equiv.json
--rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/tau/tau_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.503989 g2p-1.0.20230228/g2p/mappings/langs/tce/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/tce/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/tce/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/tce/tce_equiv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/tce/tce_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.503989 g2p-1.0.20230228/g2p/mappings/langs/tgx/
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/tgx/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/tgx/tgx_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/tgx/tgx_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.503989 g2p-1.0.20230228/g2p/mappings/langs/tli/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/tli/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/tli/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/tli/tli_equiv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/tli/tli_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.503989 g2p-1.0.20230228/g2p/mappings/langs/ttm/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/ttm/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/ttm/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/ttm/ttm_equiv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/ttm/ttm_to_ipa.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.503989 g2p-1.0.20230228/g2p/mappings/langs/und/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/und/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/und/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/und/und_ipa_to_eng_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/und/und_to_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.507989 g2p-1.0.20230228/g2p/mappings/langs/win/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/win/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/win/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/win/hoocak_alphabet.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/langs/win/win_to_ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20794 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/mappings/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.507989 g2p-1.0.20230228/g2p/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/static/blockly_main.js
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/static/blocks.js
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)    21998 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/static/custom.js
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/static/echart_custom.js
--rw-r--r--   0 runner    (1001) docker     (123)    16633 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/static/languages-network.json
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/static/normalize.css
--rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/static/skeleton.css
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/static/swagger.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.507989 g2p-1.0.20230228/g2p/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/templates/docs.html
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.507989 g2p-1.0.20230228/g2p/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.507989 g2p-1.0.20230228/g2p/tests/public/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.511989 g2p-1.0.20230228/g2p/tests/public/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/crg.psv
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/crj.psv
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/crk.psv
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/crl.psv
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/crm.psv
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/csw.psv
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/ctp.csv
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/eng.csv
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/fin.psv
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/fn_unicode.psv
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/fra.psv
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/fra_panagrams.txt
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/fra_panagrams_NFD.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/fra_simple.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/git.psv
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/gwi.psv
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/haa.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/ikt.psv
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/iku-sro.psv
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/iku.psv
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/kwk.psv
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/lml.psv
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/mic.psv
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/moe.psv
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/moh.psv
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/oji-syl.psv
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/oji.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/oka.csv
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/srs.psv
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/str.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/str_un_human_rights.txt
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/tau.psv
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/tce.csv
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/tli.csv
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/ttm.csv
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/data/win.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/git_to_ipa.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.515989 g2p-1.0.20230228/g2p/tests/public/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/abbreviation_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/abbreviation_mapping.csv
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/abbreviations.csv
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/abbreviations.json
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/abbreviations.psv
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/abbreviations.substring.csv
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/abbreviations.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.475989 g2p-1.0.20230228/g2p/tests/public/mappings/bad_langs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.519989 g2p-1.0.20230228/g2p/tests/public/mappings/bad_langs/lang1/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/bad_langs/lang1/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/bad_langs/lang1/minimal.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.475989 g2p-1.0.20230228/g2p/tests/public/mappings/bad_langs2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.519989 g2p-1.0.20230228/g2p/tests/public/mappings/bad_langs2/lang1/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/bad_langs2/lang1/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/bad_langs2/lang1/minimal.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.519989 g2p-1.0.20230228/g2p/tests/public/mappings/case-feed/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/case-feed/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/case-feed/cf-in-lc-to-cf-out-uc.csv
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/case-feed/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/case-feed/empty.csv
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/compose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/compose1-2.csv
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/compose2-3.csv
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/deletion.csv
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/deletion.json
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/deletion_config_csv.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/deletion_config_json.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/g2p_studio.csv
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/g2p_studio2.csv
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/gen-map-1.csv
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/gen-map-2.csv
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/gen-map-3a.csv
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/gen-map-3b.csv
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/gen-map_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/gm1-ipa_to_gm2-ipa.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      121 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/gm2-ipa_to_gm3-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/gm3-ipa_to_gm2-ipa.json
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/malformed_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/minimal.csv
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/minimal.json
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/minimal.psv
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/minimal.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/minimal.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/minimal_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/minimal_configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/no_escape.csv
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/null.csv
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/null_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/rule-ordering.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/test_to_ipa.csv
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/tokenize_punct.csv
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/mappings/tokenize_punct_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/public/sample_response.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     4582 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/run.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4663 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/test_api_resources.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5034 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/test_check_ipa_arpabet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15944 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/test_cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5880 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/test_create_mapping.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1480 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/test_doctor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1612 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/test_doctor_expensive.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3178 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/test_fallback.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17859 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/test_indices.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1974 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/test_langs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12916 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/test_mappings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1110 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/test_network.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8943 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/test_studio.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3967 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/test_tokenize_and_map.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5521 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/test_tokenizer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5502 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/test_transducer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2203 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/test_unidecode_transducer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10070 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/test_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9835 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/test_z_local_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/tests/time_panphon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.519989 g2p-1.0.20230228/g2p/transducer/
--rw-r--r--   0 runner    (1001) docker     (123)    35909 2023-02-28 22:33:45.000000 g2p-1.0.20230228/g2p/transducer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:34:00.479989 g2p-1.0.20230228/g2p.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15114 2023-02-28 22:34:00.000000 g2p-1.0.20230228/g2p.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13781 2023-02-28 22:34:00.000000 g2p-1.0.20230228/g2p.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 22:34:00.000000 g2p-1.0.20230228/g2p.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-28 22:34:00.000000 g2p-1.0.20230228/g2p.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 22:34:00.000000 g2p-1.0.20230228/g2p.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-02-28 22:34:00.000000 g2p-1.0.20230228/g2p.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-28 22:34:00.000000 g2p-1.0.20230228/g2p.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-02-28 22:34:00.519989 g2p-1.0.20230228/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-02-28 22:33:45.000000 g2p-1.0.20230228/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.338273 g2p-1.0.20230412/
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-12 22:08:04.000000 g2p-1.0.20230412/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-12 22:08:04.000000 g2p-1.0.20230412/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15096 2023-04-12 22:08:22.338273 g2p-1.0.20230412/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14611 2023-04-12 22:08:04.000000 g2p-1.0.20230412/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.246272 g2p-1.0.20230412/g2p/
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27745 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.246272 g2p-1.0.20230412/g2p/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)    22040 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/create_fallback_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/create_ipa_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.258272 g2p-1.0.20230412/g2p/mappings/langs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.262272 g2p-1.0.20230412/g2p/mappings/langs/alq/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/alq/alq_to_ipa.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/alq/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.262272 g2p-1.0.20230412/g2p/mappings/langs/atj/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/atj/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/atj/atj_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/atj/atj_to_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/atj/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.262272 g2p-1.0.20230412/g2p/mappings/langs/ckt/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/ckt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/ckt/ckt_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/ckt/ckt_to_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/ckt/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.262272 g2p-1.0.20230412/g2p/mappings/langs/clc/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/clc/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/clc/doulos.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.266272 g2p-1.0.20230412/g2p/mappings/langs/crg/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crg/abbreviations.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crg/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crg/crg-dv-to-crg-ipa.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crg/crg-tmd-to-crg-ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.266272 g2p-1.0.20230412/g2p/mappings/langs/crj/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crj/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crj/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crj/crj_equiv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crj/crj_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crj/crj_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.266272 g2p-1.0.20230412/g2p/mappings/langs/crk/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crk/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crk/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crk/crk-no-symbols_to_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crk/crk_to_crk-no-symbols.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.266272 g2p-1.0.20230412/g2p/mappings/langs/crl/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crl/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crl/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crl/crl_equiv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crl/crl_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crl/crl_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.270272 g2p-1.0.20230412/g2p/mappings/langs/crm/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crm/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crm/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12358 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crm/crm_equiv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crm/crm_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crm/crm_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.270272 g2p-1.0.20230412/g2p/mappings/langs/crx/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crx/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crx/stella_orth_to_syllabics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/crx/stella_syllabics_to_orth.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.270272 g2p-1.0.20230412/g2p/mappings/langs/csw/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/csw/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/csw/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10982 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/csw/csw_equiv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/csw/csw_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/csw/csw_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.270272 g2p-1.0.20230412/g2p/mappings/langs/ctp/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/ctp/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/ctp/ctp_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/ctp/ctp_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.270272 g2p-1.0.20230412/g2p/mappings/langs/dan/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/dan/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/dan/dan_abbs.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/dan/dan_to_dummy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/dan/dan_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.278272 g2p-1.0.20230412/g2p/mappings/langs/eng/
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/eng/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)  4215929 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/eng/cmudict.ipa.aligned.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/eng/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/eng/dummy_to_arpabet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/eng/eng_arpabet_to_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/eng/eng_inventory.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/eng/eng_ipa_to_arpabet.json
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/eng/make_alignments.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/eng/make_ipa_cmudict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/eng/reverse_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.278272 g2p-1.0.20230412/g2p/mappings/langs/fin/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/fin/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/fin/fin_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.282272 g2p-1.0.20230412/g2p/mappings/langs/font-encodings/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/font-encodings/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/font-encodings/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/font-encodings/fn_unicode.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/font-encodings/hei_doulos.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/font-encodings/hei_times.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/font-encodings/nav_times.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.282272 g2p-1.0.20230412/g2p/mappings/langs/fra/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/fra/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/fra/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/fra/fra_abbs.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/fra/fra_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.290272 g2p-1.0.20230412/g2p/mappings/langs/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/alq-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/atj-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/crg-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/crk-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/dan-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/fin-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/fra-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/gla-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/gwi-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/haa-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/ikt-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/ikt-ipa_to_hamming-eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/iku-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/iku-ipa_to_hamming-eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10603 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/iku-sro-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/lml-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/mic-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/moe-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/moh-equiv_to_dummy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/moh-equiv_to_hamming_dummy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/moh-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/moh-ipa_to_hamming-eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/oji-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/oka-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/see-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/str-equiv_to_dummy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/str-equiv_to_hamming_dummy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/str-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/str-ipa_to_hamming-eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13035 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/tau-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/tce-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/tli-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/ttm-ipa_to_eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/und-ascii_to_dummy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/und-ascii_to_hamming_dummy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/und-ipa_to_hamming-eng-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/generated/win-ipa_to_eng-ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.290272 g2p-1.0.20230412/g2p/mappings/langs/git/
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/git/APA.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/git/Ortho_variables.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/git/Orthography.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/git/Orthography_Deterministic.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/git/RAPA.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/git/RAPA_Deterministic.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/git/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/git/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/git/equiv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/git/git_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/git/git_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.290272 g2p-1.0.20230412/g2p/mappings/langs/gla/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/gla/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/gla/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/gla/gla_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.294272 g2p-1.0.20230412/g2p/mappings/langs/gwi/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/gwi/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/gwi/gwi_equiv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/gwi/gwi_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.294272 g2p-1.0.20230412/g2p/mappings/langs/haa/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/haa/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/haa/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/haa/haa_abbs.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/haa/haa_equiv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/haa/haa_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.294272 g2p-1.0.20230412/g2p/mappings/langs/ikt/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/ikt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/ikt/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/ikt/ikt_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.294272 g2p-1.0.20230412/g2p/mappings/langs/iku/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/iku/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/iku/iku_equiv_to_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/iku/iku_sro_to_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/iku/iku_to_iku_equiv.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.294272 g2p-1.0.20230412/g2p/mappings/langs/kkz/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/kkz/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/kkz/kkz_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/kkz/kkz_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.298272 g2p-1.0.20230412/g2p/mappings/langs/kwk/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/kwk/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/kwk/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/kwk/kwk_boas_to_umista.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/kwk/kwk_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/kwk/kwk_napa_to_ipa.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/kwk/kwk_napa_to_xsampa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/kwk/kwk_umista_to_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/kwk/kwk_xsampa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/kwk/napa_equiv_ubc.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/kwk/napa_equiv_uvic.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/kwk/umista_equiv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  7050749 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/langs.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.298272 g2p-1.0.20230412/g2p/mappings/langs/lml/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/lml/abbreviations.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/lml/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/lml/lml_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.298272 g2p-1.0.20230412/g2p/mappings/langs/mic/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/mic/abbreviations.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/mic/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/mic/mic_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.298272 g2p-1.0.20230412/g2p/mappings/langs/moe/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/moe/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/moe/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/moe/moe_abbs.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/moe/moe_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.302272 g2p-1.0.20230412/g2p/mappings/langs/moh/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/moh/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/moh/abbreviations.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/moh/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/moh/moh_equiv.json
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/moh/moh_to_festival.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/moh/moh_to_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/network.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.302272 g2p-1.0.20230412/g2p/mappings/langs/norm/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/norm/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/norm/panphon_preprocessor.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/norm/tone-map.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.302272 g2p-1.0.20230412/g2p/mappings/langs/oji/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/oji/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/oji/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/oji/oji_syllabics_to_orth.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/oji/oji_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.302272 g2p-1.0.20230412/g2p/mappings/langs/oka/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/oka/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/oka/oka_equiv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/oka/oka_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.302272 g2p-1.0.20230412/g2p/mappings/langs/see/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/see/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/see/see_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.306272 g2p-1.0.20230412/g2p/mappings/langs/srs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      535 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/srs/config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2109 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/srs/srs_ipa_to_eng_ipa.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6083 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/srs/srs_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.306272 g2p-1.0.20230412/g2p/mappings/langs/str/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/str/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/str/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/str/str_equiv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/str/str_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.306272 g2p-1.0.20230412/g2p/mappings/langs/tau/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/tau/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/tau/tau_equiv.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/tau/tau_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.306272 g2p-1.0.20230412/g2p/mappings/langs/tce/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/tce/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/tce/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/tce/tce_equiv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/tce/tce_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.306272 g2p-1.0.20230412/g2p/mappings/langs/tgx/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/tgx/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/tgx/tgx_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/tgx/tgx_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.306272 g2p-1.0.20230412/g2p/mappings/langs/tli/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/tli/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/tli/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/tli/tli_equiv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/tli/tli_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.310272 g2p-1.0.20230412/g2p/mappings/langs/ttm/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/ttm/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/ttm/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/ttm/ttm_equiv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/ttm/ttm_to_ipa.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.310272 g2p-1.0.20230412/g2p/mappings/langs/und/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/und/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/und/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/und/und_ipa_to_eng_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/und/und_to_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.310272 g2p-1.0.20230412/g2p/mappings/langs/win/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/win/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/win/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/win/hoocak_alphabet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/langs/win/win_to_ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23309 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/mappings/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.310272 g2p-1.0.20230412/g2p/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/static/blockly_main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/static/blocks.js
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    23193 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/static/custom.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/static/echart_custom.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15645 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/static/languages-network.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/static/normalize.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/static/skeleton.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/static/swagger.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.314272 g2p-1.0.20230412/g2p/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/templates/docs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.318272 g2p-1.0.20230412/g2p/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.318272 g2p-1.0.20230412/g2p/tests/public/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.326273 g2p-1.0.20230412/g2p/tests/public/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/crg.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/crj.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/crk.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/crl.psv
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/crm.psv
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/csw.psv
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/ctp.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/eng.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/fin.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/fn_unicode.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/fra.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/fra_panagrams.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/fra_panagrams_NFD.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/fra_simple.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/git.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/gwi.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/haa.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/ikt.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/iku-sro.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/iku.psv
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/kwk.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/lml.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/mic.psv
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/moe.psv
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/moh.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/oji-syl.psv
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/oji.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/oka.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/srs.psv
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/str.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/str_un_human_rights.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/tau.psv
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/tce.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/tli.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/ttm.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/data/win.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/git_to_ipa.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.334273 g2p-1.0.20230412/g2p/tests/public/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/abbreviation_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/abbreviation_mapping.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/abbreviations.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/abbreviations.json
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/abbreviations.psv
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/abbreviations.substring.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/abbreviations.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.242272 g2p-1.0.20230412/g2p/tests/public/mappings/bad_langs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.334273 g2p-1.0.20230412/g2p/tests/public/mappings/bad_langs/lang1/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/bad_langs/lang1/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/bad_langs/lang1/minimal.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.242272 g2p-1.0.20230412/g2p/tests/public/mappings/bad_langs2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.334273 g2p-1.0.20230412/g2p/tests/public/mappings/bad_langs2/lang1/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/bad_langs2/lang1/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/bad_langs2/lang1/minimal.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/bad_lexicon_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.338273 g2p-1.0.20230412/g2p/tests/public/mappings/case-feed/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/case-feed/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/case-feed/cf-in-lc-to-cf-out-uc.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/case-feed/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/case-feed/empty.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/compose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/compose1-2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/compose2-3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/deletion.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/deletion.json
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/deletion_config_csv.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/deletion_config_json.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/g2p_studio.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/g2p_studio2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/gen-map-1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/gen-map-2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/gen-map-3a.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/gen-map-3b.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/gen-map_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/gm1-ipa_to_gm2-ipa.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      121 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/gm2-ipa_to_gm3-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/gm3-ipa_to_gm2-ipa.json
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/hello.aligned.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/lexicon_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/malformed_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/minimal.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/minimal.json
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/minimal.psv
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/minimal.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/minimal.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/minimal_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/minimal_configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/no_escape.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/null.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/null_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/rule-ordering.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/test_to_ipa.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/tokenize_punct.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/mappings/tokenize_punct_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/public/sample_response.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4682 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4900 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_api_resources.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5237 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_check_ipa_arpabet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16189 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6249 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_create_mapping.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1480 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_doctor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1858 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_doctor_expensive.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3214 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_fallback.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23149 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_indices.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1991 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_langs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_lexicon_transducer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13478 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_mappings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1299 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_network.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10273 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_studio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5937 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_tokenize_and_map.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5723 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_tokenizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11446 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_transducer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2501 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_unidecode_transducer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10254 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9835 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/test_z_local_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/tests/time_panphon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.338273 g2p-1.0.20230412/g2p/transducer/
+-rw-r--r--   0 runner    (1001) docker     (123)    49089 2023-04-12 22:08:04.000000 g2p-1.0.20230412/g2p/transducer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:08:22.246272 g2p-1.0.20230412/g2p.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15096 2023-04-12 22:08:22.000000 g2p-1.0.20230412/g2p.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14116 2023-04-12 22:08:22.000000 g2p-1.0.20230412/g2p.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 22:08:22.000000 g2p-1.0.20230412/g2p.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-12 22:08:22.000000 g2p-1.0.20230412/g2p.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 22:08:21.000000 g2p-1.0.20230412/g2p.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-12 22:08:22.000000 g2p-1.0.20230412/g2p.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 22:08:22.000000 g2p-1.0.20230412/g2p.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-12 22:08:22.338273 g2p-1.0.20230412/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-12 22:08:04.000000 g2p-1.0.20230412/setup.py
```

### Comparing `g2p-1.0.20230228/LICENSE` & `g2p-1.0.20230412/LICENSE`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/PKG-INFO` & `g2p-1.0.20230412/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g2p
-Version: 1.0.20230228
+Version: 1.0.20230412
 Summary: Module for creating context-aware, rule-based G2P mappings that preserve indices
 Home-page: https://github.com/roedoejet/g2p
 Author: Aidan Pine
 Author-email: hello@aidanpine.ca
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 # Gᵢ2Pᵢ
 
 [![codecov](https://codecov.io/gh/roedoejet/g2p/branch/main/graph/badge.svg)](https://codecov.io/gh/roedoejet/g2p)
 [![Documentation Status](https://readthedocs.org/projects/g2p/badge/?version=latest)](https://g2p.readthedocs.io/en/latest/?badge=latest)
 [![Build Status](https://github.com/roedoejet/g2p/actions/workflows/tests.yml/badge.svg)](https://github.com/roedoejet/g2p/actions)
 [![PyPI package](https://img.shields.io/pypi/v/g2p.svg)](https://pypi.org/project/g2p/)
 [![license](https://img.shields.io/badge/Licence-MIT-green)](LICENSE)
-[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/roedoejet/g2p)
+[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg)](https://github.com/roedoejet/g2p)
 
 > Grapheme-to-Phoneme transformations that preserve input and output indices!
 
 This library is for handling arbitrary conversions between input and output segments while preserving indices.
 
 ![indices](https://raw.githubusercontent.com/roedoejet/g2p/main/g2p/static/assets/bonjour.png)
```

### Comparing `g2p-1.0.20230228/README.md` & `g2p-1.0.20230412/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Gᵢ2Pᵢ
 
 [![codecov](https://codecov.io/gh/roedoejet/g2p/branch/main/graph/badge.svg)](https://codecov.io/gh/roedoejet/g2p)
 [![Documentation Status](https://readthedocs.org/projects/g2p/badge/?version=latest)](https://g2p.readthedocs.io/en/latest/?badge=latest)
 [![Build Status](https://github.com/roedoejet/g2p/actions/workflows/tests.yml/badge.svg)](https://github.com/roedoejet/g2p/actions)
 [![PyPI package](https://img.shields.io/pypi/v/g2p.svg)](https://pypi.org/project/g2p/)
 [![license](https://img.shields.io/badge/Licence-MIT-green)](LICENSE)
-[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/roedoejet/g2p)
+[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg)](https://github.com/roedoejet/g2p)
 
 > Grapheme-to-Phoneme transformations that preserve input and output indices!
 
 This library is for handling arbitrary conversions between input and output segments while preserving indices.
 
 ![indices](https://raw.githubusercontent.com/roedoejet/g2p/main/g2p/static/assets/bonjour.png)
```

### Comparing `g2p-1.0.20230228/g2p/__init__.py` & `g2p-1.0.20230412/g2p/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,55 +13,66 @@
     from g2p import make_tokenizer
     tokenizer = make_tokenizer(lang)
     list_of_tokens = tokenizer.tokenize_text(input_text)
 
 """
 import io
 import sys
+from typing import Dict, Optional, Tuple, Union
 
 from networkx import shortest_path
 from networkx.exception import NetworkXNoPath
 
 from g2p.exceptions import InvalidLanguageCode, NoPath
 from g2p.log import LOGGER
 from g2p.mappings import Mapping
 from g2p.mappings.langs import LANGS_NETWORK
 from g2p.mappings.tokenizer import make_tokenizer
 from g2p.transducer import CompositeTransducer, TokenizingTransducer, Transducer
 
-if sys.stdout.encoding != "utf8" and hasattr(sys.stdout, "buffer"):
-    sys.stdout = io.TextIOWrapper(sys.stdout.buffer, encoding="utf8")
-
-if sys.stderr.encoding != "utf8" and hasattr(sys.stderr, "buffer"):
-    sys.stderr = io.TextIOWrapper(sys.stderr.buffer, encoding="utf8")
+if "pytest" not in sys.modules:
+    if sys.stdout.encoding != "utf8" and hasattr(sys.stdout, "buffer"):
+        sys.stdout = io.TextIOWrapper(sys.stdout.buffer, encoding="utf8")
+    if sys.stderr.encoding != "utf8" and hasattr(sys.stderr, "buffer"):
+        sys.stderr = io.TextIOWrapper(sys.stderr.buffer, encoding="utf8")
 
 if sys.version_info < (3, 6):
     sys.exit(
         f"Python 3.6 or more recent is required. You are using {sys.version}.\n"
         "Please use a newer version of Python."
     )
 
 
-_g2p_cache = {}
+_g2p_cache: Dict[
+    Tuple[str, str, Optional[str]],
+    Union[Transducer, CompositeTransducer, TokenizingTransducer],
+] = {}
 
 
-def make_g2p(in_lang: str, out_lang: str, tok_lang=None):
+def make_g2p(in_lang: str, out_lang: str, tok_lang: Optional[str] = None):
     """Make a g2p Transducer for mapping text from in_lang to out_lang via the
     shortest path between them.
 
+    In general you should also add `tok_lang` to specify the language
+    for tokenization (probably the same as `in_lang`), because
+    transducers are not guaranteed to deal with whitespace,
+    punctuation, etc, properly.
+
     Args:
         in_lang (str): input language code
         out_lang (str): output language code
+        tok_lang (Optional[str]): language for tokenization
 
     Returns:
-        Transducer from in_lang to out_lang
+        Transducer from in_lang to out_lang, optionally with a tokenizer.
 
     Raises:
         InvalidLanguageCode: if in_lang or out_lang don't exist
         NoPath: if there is path between in_lang and out_lang
+
     """
     if (in_lang, out_lang, tok_lang) in _g2p_cache:
         return _g2p_cache[(in_lang, out_lang, tok_lang)]
 
     # Check in_lang is a node in network
     if in_lang not in LANGS_NETWORK.nodes:
         LOGGER.error(f"No lang called '{in_lang}'. Please try again.")
@@ -93,14 +104,15 @@
         mapping = Mapping(in_lang=lang1, out_lang=lang2)
         LOGGER.debug(
             f"Adding mapping between {lang1} and {lang2} to composite transducer."
         )
         mappings_needed.append(mapping)
 
     # Either construct a Transducer or Composite Transducer
+    transducer: Union[Transducer, CompositeTransducer, TokenizingTransducer]
     if len(mappings_needed) == 1:
         transducer = Transducer(mappings_needed[0])
     else:
         transducer = CompositeTransducer([Transducer(x) for x in mappings_needed])
 
     # If tokenization was requested, return a TokenizingTransducer
     if tok_lang:
```

### Comparing `g2p-1.0.20230228/g2p/api.py` & `g2p-1.0.20230412/g2p/api.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/app.py` & `g2p-1.0.20230412/g2p/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 """
 
 Views and config to the g2p Studio web app
 
 """
-import json
-import os
 from typing import Union
 
 from flask import Flask, render_template
 from flask_cors import CORS
 from flask_socketio import SocketIO, emit
-from networkx.algorithms.dag import ancestors, descendants
+from networkx import shortest_path
 
 from g2p import make_g2p
 from g2p.api import g2p_api
-from g2p.log import LOGGER
 from g2p.mappings import Mapping
 from g2p.mappings.langs import LANGS_NETWORK
 from g2p.mappings.utils import expand_abbreviations_format, flatten_abbreviations_format
-from g2p.static import __file__ as static_file
 from g2p.transducer import (
     CompositeTransducer,
     CompositeTransductionGraph,
     Transducer,
     TransductionGraph,
 )
 
@@ -52,45 +48,14 @@
         "#000"
         if 1 - (int(R, 16) * 0.299 + int(G, 16) * 0.587 + int(B, 16) * 0.114) / 255
         < 0.5
         else "#fff"
     )
 
 
-def network_to_echart(write_to_file: bool = False, layout: bool = False):
-    nodes = []
-    no_nodes = len(LANGS_NETWORK.nodes)
-    for node in LANGS_NETWORK.nodes:
-        lang_name = node.split("-")[0]
-        no_ancestors = len(ancestors(LANGS_NETWORK, node))
-        no_descendants = len(descendants(LANGS_NETWORK, node))
-        size = min(
-            20,
-            max(
-                2, ((no_ancestors / no_nodes) * 100 + (no_descendants / no_nodes) * 100)
-            ),
-        )
-        node = {"name": node, "symbolSize": size, "id": node, "category": lang_name}
-        nodes.append(node)
-    nodes.sort(key=lambda x: x["name"])
-    edges = []
-    for edge in LANGS_NETWORK.edges:
-        edges.append({"source": edge[0], "target": edge[1]})
-    if write_to_file:
-        with open(
-            os.path.join(os.path.dirname(static_file), "languages-network.json"),
-            "w",
-            encoding="utf-8",
-            newline="\n",
-        ) as f:
-            f.write(json.dumps({"nodes": nodes, "edges": edges}) + "\n")
-        LOGGER.info("Wrote network nodes and edges to static file.")
-    return nodes, edges
-
-
 def return_echart_data(tg: Union[CompositeTransductionGraph, TransductionGraph]):
     x = 100
     diff = 200
     nodes = []
     edges = []
     index_offset = 0
     colour = "#222222"
@@ -148,31 +113,14 @@
             }
             for i, x in enumerate(tier.output_string)
         ]
         nodes += outputs
     return nodes, edges
 
 
-def return_empty_mappings(n=DEFAULT_N):
-    """Return 'n' * empty mappings"""
-    y = 0
-    mappings = []
-    while y < n:
-        mappings.append(
-            {"in": "", "out": "", "context_before": "", "context_after": ""}
-        )
-        y += 1
-    return mappings
-
-
-def return_descendant_nodes(node: str):
-    """Return possible outputs for a given input"""
-    return [x for x in descendants(LANGS_NETWORK, node)]
-
-
 @APP.route("/")
 def home():
     """Return homepage of g2p studio"""
     return render_template("index.html")
 
 
 @APP.route("/docs")
@@ -190,14 +138,17 @@
         mappings_obj = Mapping(
             mapping["mapping"],
             abbreviations=flatten_abbreviations_format(mapping["abbreviations"]),
             **mapping["kwargs"],
         )
         transducer = Transducer(mappings_obj)
         transducers.append(transducer)
+    if len(transducers) == 0:
+        emit("conversion response", {"output_string": message["data"]["input_string"]})
+        return
     transducer = CompositeTransducer(transducers)
     if message["data"]["index"]:
         tg = transducer(message["data"]["input_string"])
         data, links = return_echart_data(tg)
         emit(
             "conversion response",
             {
@@ -211,34 +162,68 @@
         emit("conversion response", {"output_string": output_string})
 
 
 @SOCKETIO.on("table event", namespace="/table")
 def change_table(message):
     """Change the lookup table"""
     if message["in_lang"] == "custom" or message["out_lang"] == "custom":
-        mappings = Mapping(return_empty_mappings())
-    else:
-        transducer = make_g2p(message["in_lang"], message["out_lang"])
-    if isinstance(transducer, Transducer):
-        mappings = [transducer.mapping]
-    elif isinstance(transducer, CompositeTransducer):
-        mappings = [x.mapping for x in transducer._transducers]
+        # These are only used to generate JSON to send to the client,
+        # so it's safe to create a list of references to the same thing.
+        mappings = [
+            {"in": "", "out": "", "context_before": "", "context_after": ""}
+        ] * DEFAULT_N
+        abbs = [[""] * 6] * DEFAULT_N
+        kwargs = {
+            "language_name": "Custom",
+            "display_name": "Custom",
+            "in_lang": "custom",
+            "out_lang": "custom",
+            "include": False,
+            "type": "mapping",
+            "case_sensitive": True,
+            "norm_form": "NFC",
+            "escape_special": False,
+            "prevent_feeding": False,
+            "reverse": False,
+            "rule_ordering": "as-written",
+            "out_delimiter": "",
+        }
+        emit(
+            "table response",
+            [
+                {
+                    "mappings": mappings,
+                    "abbs": abbs,
+                    "kwargs": kwargs,
+                }
+            ],
+        )
     else:
-        pass
-    emit(
-        "table response",
-        [
-            {
-                "mappings": x.plain_mapping(),
-                "abbs": expand_abbreviations_format(x.abbreviations),
-                "kwargs": x.kwargs,
-            }
-            for x in mappings
-        ],
-    )
+        # Do not create a composite transducer just to decompose it,
+        # because it is the individual ones which are cached by g2p
+        path = shortest_path(LANGS_NETWORK, message["in_lang"], message["out_lang"])
+        if len(path) == 1:
+            transducer = make_g2p(message["in_lang"], message["out_lang"])
+            mappings = [transducer.mapping]
+        else:
+            mappings = []
+            for lang1, lang2 in zip(path[:-1], path[1:]):
+                transducer = make_g2p(lang1, lang2)
+                mappings.append(transducer.mapping)
+        emit(
+            "table response",
+            [
+                {
+                    "mappings": x.plain_mapping(),
+                    "abbs": expand_abbreviations_format(x.abbreviations),
+                    "kwargs": x.kwargs,
+                }
+                for x in mappings
+            ],
+        )
 
 
 @SOCKETIO.on("connect", namespace="/connect")
 def test_connect():
     """Let client know disconnected"""
     emit("connection response", {"data": "Connected"})
```

### Comparing `g2p-1.0.20230228/g2p/cli.py` & `g2p-1.0.20230412/g2p/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import yaml
 from flask.cli import FlaskGroup
 from networkx import has_path
 
 from g2p import make_g2p
 from g2p._version import VERSION
 from g2p.api import update_docs
-from g2p.app import APP, network_to_echart
+from g2p.app import APP
 from g2p.exceptions import InvalidLanguageCode, MappingMissing, NoPath
 from g2p.log import LOGGER
 from g2p.mappings import Mapping
 from g2p.mappings.create_fallback_mapping import (
     DUMMY_INVENTORY,
     align_to_dummy_fallback,
 )
@@ -31,16 +31,21 @@
 from g2p.mappings.langs import (
     LANGS_DIR,
     LANGS_NETWORK,
     LANGS_PKL_NAME,
     MAPPINGS_AVAILABLE,
     NETWORK_PKL_NAME,
 )
-from g2p.mappings.langs.utils import cache_langs, check_ipa_known_segs
+from g2p.mappings.langs.utils import (
+    cache_langs,
+    check_ipa_known_segs,
+    network_to_echart,
+)
 from g2p.mappings.utils import is_ipa, is_xsampa, load_mapping_from_path, normalize
+from g2p.static import __file__ as static_file
 from g2p.transducer import Transducer
 
 PRINTER = pprint.PrettyPrinter(indent=4)
 
 
 def create_app():
     """Return the flask app for g2p"""
@@ -420,14 +425,21 @@
             new_mapping.mapping_to_file(out_dir)
         else:
             new_mapping.config_to_file()
             new_mapping.mapping_to_file()
 
 
 @click.option(
+    "--substring-alignments",
+    "-a",
+    default=False,
+    is_flag=True,
+    help="Show the minimal monotonic substring alignments.",
+)
+@click.option(
     "--pretty-edges",
     "-e",
     default=False,
     is_flag=True,
     help="Show the traduction graph in a pretty, plain-text format.",
 )
 @click.option(
@@ -480,14 +492,15 @@
     path,
     tok,
     check,
     debugger,
     pretty_edges,
     tok_lang,
     config,
+    substring_alignments,
 ):
     """Convert INPUT_TEXT through g2p mapping(s) from IN_LANG to OUT_LANG.
 
     Visit http://g2p-studio.herokuapp.com/api/v1/langs for a list of languages.
 
     There must be a path from IN_LANG to OUT_LANG, possibly via some intermediates.
     For example, mapping from fra to eng-arpabet will successively apply
@@ -547,14 +560,16 @@
         transducer = make_g2p(in_lang, out_lang, tok_lang=tok_lang)
     elif path:
         transducer = Transducer(Mapping(path))
     tg = transducer(input_text)
     if check:
         transducer.check(tg, display_warnings=True)
     outputs = [tg.output_string]
+    if substring_alignments:
+        outputs += [tg.substring_alignments()]
     if pretty_edges:
         outputs += [tg.pretty_edges()]
     if debugger:
         outputs += [tg.edges, tg.debugger]
     if len(outputs) > 1:
         click.echo(pprint.pformat(outputs, indent=4))
     else:
@@ -644,15 +659,17 @@
         langs_path = os.path.join(in_dir, LANGS_PKL_NAME)
         network_path = os.path.join(in_dir, NETWORK_PKL_NAME)
     else:
         langs_path = os.path.join(out_dir, LANGS_PKL_NAME)
         network_path = os.path.join(out_dir, NETWORK_PKL_NAME)
     cache_langs(dir_path=in_dir, langs_path=langs_path, network_path=network_path)
     update_docs()
-    network_to_echart(write_to_file=True)
+    network_to_echart(
+        outfile=os.path.join(os.path.dirname(static_file), "languages-network.json")
+    )
 
 
 @click.argument("path", type=click.Path(exists=True, file_okay=True, dir_okay=False))
 @click.argument("lang")
 @cli.command(
     context_settings=CONTEXT_SETTINGS,
     short_help="Scan a document for unknown characters.",
```

### Comparing `g2p-1.0.20230228/g2p/exceptions.py` & `g2p-1.0.20230412/g2p/exceptions.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/__init__.py` & `g2p-1.0.20230412/g2p/mappings/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     escape_special_characters,
     expand_abbreviations,
     find_mapping,
     is_dummy,
     is_ipa,
     is_xsampa,
     load_abbreviations_from_file,
+    load_alignments_from_file,
     load_from_file,
     load_mapping_from_path,
     normalize,
     validate,
 )
 
 GEN_DIR = os.path.join(os.path.dirname(LANGS_FILE), "generated")
@@ -77,28 +78,36 @@
         input are applied first. Sorting the rules like this prevents shorter rules
         from taking part in feeding relations
         (previously this was accomplished with ``as_is=False``).
 
     @param prevent_feeding: bool = False
         Converts each rule into an intermediary form
 
+    @param type: str = None
+        Type of mapping, either "mapping" (rules), "unidecode" (magical Unicode guessing) or
+        "lexicon" (lookup in an aligned lexicon).
+
+    @param alignments: str = None
+        A string specifying a file from which to load alignments when type = "lexicon".
+
     """
 
     def __init__(  # noqa: C901
         self,
         mapping=None,
         abbreviations: Union[str, DefaultDict[str, List[str]]] = None,
         **kwargs,
     ):
         # should these just be explicit instead of kwargs...
         # yes, they should
         self.allowable_kwargs = [
             "language_name",
             "display_name",
             "mapping",
+            "alignments",
             "in_lang",
             "out_lang",
             "out_delimiter",
             "as_is",
             "case_sensitive",
             "rule_ordering",
             "escape_special",
@@ -130,14 +139,20 @@
                 )
                 self.process_loaded_config(loaded_config)
             elif "id" in self.kwargs:
                 loaded_config = self.find_mapping_by_id(self.kwargs["id"])
                 self.process_loaded_config(loaded_config)
             elif self.kwargs.get("type", "") == "unidecode":
                 self.mapping = []
+            elif self.kwargs.get("type", "") == "lexicon":
+                self.mapping = []
+                if "alignments" in self.kwargs:
+                    self.alignments = load_alignments_from_file(
+                        self.kwargs["alignments"], self.kwargs["out_delimiter"]
+                    )
             else:
                 raise exceptions.MalformedLookup()
         if (
             self.abbreviations
             and self.mapping
             and "match_pattern" not in self.mapping[0]
         ):
@@ -221,14 +236,17 @@
 
     def process_loaded_config(self, config):
         """For a mapping loaded from a file, take the keyword arguments and supply them to the
         Mapping, and get any abbreviations data.
         """
         if config.get("type", "") == "unidecode":
             self.mapping = []
+        elif config.get("type", "") == "lexicon":
+            self.mapping = []
+            self.alignments = config["alignment_data"]
         else:
             self.mapping = config["mapping_data"]
             self.abbreviations = config.get("abbreviations_data", None)
         mapping_kwargs = OrderedDict(
             {k: v for k, v in config.items() if k in self.allowable_kwargs}
         )
         # Merge kwargs, but prioritize kwargs that initialized the Mapping
@@ -383,25 +401,32 @@
             inp = create_fixed_width_lookbehind(before) + input_match
             if after:
                 inp += f"(?={after})"
             if not self.kwargs["case_sensitive"]:
                 rule_regex = re.compile(inp, re.I)
             else:
                 rule_regex = re.compile(inp)
-        except:
+        except re.error as e:
             in_lang = self.kwargs.get("in_lang", "und")
             out_lang = self.kwargs.get("out_lang", "und")
             LOGGER.error(
-                f"Your regex in mapping between {in_lang} and {out_lang} is malformed. \
-                    Do you have un-escaped regex characters in your input {inp}, contexts {before}, {after}?"
-            )
-            raise Exception(
-                f"Your regex in mapping between {in_lang} and {out_lang} is malformed. \
-                    Do you have un-escaped regex characters in your input {inp}, contexts {before}, {after}?"
+                "Your regex in mapping between %s and %s is malformed.  "
+                "Do you have un-escaped regex characters in your input %s, contexts %s, %s?  "
+                "Error is: %s",
+                in_lang,
+                out_lang,
+                inp,
+                before,
+                after,
+                e.msg,
             )
+            raise exceptions.MalformedMapping(
+                f"Your regex in mapping between {in_lang} and {out_lang} is malformed.  "
+                f"Do you have un-escaped regex characters in your input {inp}, contexts {before}, {after}?"
+            ) from e
         return rule_regex
 
     def reverse_mappings(self, mapping):
         """Reverse the mapping"""
         for io in mapping:
             io["in"], io["out"] = io["out"], io["in"]
             del io["context_before"]
```

### Comparing `g2p-1.0.20230228/g2p/mappings/create_fallback_mapping.py` & `g2p-1.0.20230412/g2p/mappings/create_fallback_mapping.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,34 +6,37 @@
 from g2p.mappings.create_ipa_mapping import align_inventories
 from g2p.mappings.utils import is_ipa, unicode_escape
 
 DUMMY_INVENTORY = ["ɑ", "i", "u", "t", "s", "n"]
 
 
 def align_to_dummy_fallback(
-    mapping: Mapping, io: str = "in", distance: str = "weighted_feature_edit_distance"
+    mapping: Mapping,
+    io: str = "in",
+    distance: str = "weighted_feature_edit_distance",
+    quiet=False,
 ):
     """Create a mapping from mapping's output inventory to a minimalist dummy inventory"""
     config = {"in_lang": mapping.kwargs[f"{io}_lang"], "out_lang": "dummy"}
     default_char = "t"
     if is_ipa(mapping.kwargs[f"{io}_lang"]):
         mapping = align_inventories(
-            mapping.inventory(io), DUMMY_INVENTORY, distance=distance
+            mapping.inventory(io), DUMMY_INVENTORY, distance=distance, quiet=quiet
         )
     else:
         und_g2p = make_g2p("und", "und-ipa")
         mapping = [
             {
                 "in": unicode_escape(x),
                 "out": und_g2p(unidecode(x).lower()).output_string,
             }
             for x in mapping.inventory(io)
         ]
         dummy_list = align_inventories(
-            [x["out"] for x in mapping], DUMMY_INVENTORY, distance=distance
+            [x["out"] for x in mapping], DUMMY_INVENTORY, distance=distance, quiet=quiet
         )
         dummy_dict = {}
         for x in dummy_list:
             if x["in"]:
                 dummy_dict[x["in"]] = x["out"]
 
         for x in mapping:
```

### Comparing `g2p-1.0.20230228/g2p/mappings/create_ipa_mapping.py` & `g2p-1.0.20230412/g2p/mappings/create_ipa_mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,15 @@
     return distance_method
 
 
 def create_multi_mapping(
     src_mappings: List[Tuple[Mapping, str]],
     tgt_mappings: List[Tuple[Mapping, str]],
     distance: str = "weighted_feature_edit_distance",
+    quiet=False,
 ) -> Mapping:
     """Create a mapping for a set of source mappings to a set of target mappings
 
     Each src/tgt mappings is a (mapping: Mapping, in_or_out: str) pair specifying
     the mapping to use and whether its input ("in") or output ("out") inventory
     should be used to create the new mapping.
 
@@ -147,15 +148,17 @@
         if not is_ipa(name):
             LOGGER.warning(
                 "Unsupported orthography of tgt inventory: %s; must be IPA", name
             )
         tgt_inventory.extend(mapping.inventory(io))
     tgt_inventory = deduplicate(tgt_inventory)
 
-    mapping = align_inventories(src_inventory, tgt_inventory, distance=distance)
+    mapping = align_inventories(
+        src_inventory, tgt_inventory, distance=distance, quiet=quiet
+    )
 
     config = {
         "in_lang": compact_ipa_names(map_1_names),
         "out_lang": compact_ipa_names(map_2_names),
         "language_name": "IPA",
         "rule_ordering": "apply-longest-first",
         "mapping": mapping,
@@ -171,14 +174,15 @@
 
 def create_mapping(
     mapping_1: Mapping,
     mapping_2: Mapping,
     mapping_1_io: str = "out",
     mapping_2_io: str = "in",
     distance: str = "weighted_feature_edit_distance",
+    quiet=False,
 ) -> Mapping:
     """Create a mapping from mapping_1's output inventory to mapping_2's input inventory"""
 
     map_1_name = mapping_1.kwargs[f"{mapping_1_io}_lang"]
     map_2_name = mapping_2.kwargs[f"{mapping_2_io}_lang"]
     if not is_ipa(map_1_name) and not is_xsampa(map_1_name):
         LOGGER.warning(
@@ -193,14 +197,15 @@
     l1_is_xsampa, l2_is_xsampa = is_xsampa(map_1_name), is_xsampa(map_2_name)
     mapping = align_inventories(
         mapping_1.inventory(mapping_1_io),
         mapping_2.inventory(mapping_2_io),
         l1_is_xsampa,
         l2_is_xsampa,
         distance=distance,
+        quiet=quiet,
     )
 
     # Initialize mapping with input language parameters (as_is,
     # case_sensitive, prevent_feeding, etc)
     config = mapping_1.kwargs.copy()
     # Fix up names, etc.
     if "authors" in config:
@@ -225,14 +230,15 @@
 
 def align_inventories(
     inventory_l1,
     inventory_l2,
     l1_is_xsampa=False,
     l2_is_xsampa=False,
     distance="weighted_feature_edit_distance",
+    quiet=False,
 ):
     """Align inventories by finding a good sequence in inventory_l2 for each
     character in inventory_l1"""
 
     # find_good_match() is a function inside align_inventories() because it
     # lets us initialize dst and ps_pseqs globally once, yielding a roughly 8x
     # speed inprovements over the previous version of the code.
@@ -289,17 +295,20 @@
                 inventory_l2[best_output],
             )
             good_match.append(inventory_l2[best_output])
             i += len(best_input)  # greedy!
         return "".join(good_match)
 
     mapping = []
-    pbar = tqdm(total=100)
+    if not quiet:
+        pbar = tqdm(total=100)
     step = 1 / len(inventory_l1) * 100
     for i1, p1 in enumerate(process_characters(inventory_l1, l1_is_xsampa)):
         # we enumerate the strings because we want to save the original string
         # (e.g., 'kʷ') to the mapping, not the processed one (e.g. 'kw')
         good_match = find_good_match(p1, inventory_l2)
         mapping.append({"in": inventory_l1[i1], "out": good_match})
-        pbar.update(step)
-    pbar.close()
+        if not quiet:
+            pbar.update(step)
+    if not quiet:
+        pbar.close()
     return mapping
```

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/__init__.py` & `g2p-1.0.20230412/g2p/mappings/langs/__init__.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/atj/atj_ipa_to_eng_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/atj/atj_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/atj/atj_to_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/atj/atj_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/ckt/ckt_ipa_to_eng_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/ckt/ckt_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/ckt/ckt_to_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/ckt/ckt_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/crg/config.yaml` & `g2p-1.0.20230412/g2p/mappings/langs/crg/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/crj/config.yaml` & `g2p-1.0.20230412/g2p/mappings/langs/crj/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/crj/crj_equiv.json` & `g2p-1.0.20230412/g2p/mappings/langs/crj/crj_equiv.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/crj/crj_ipa_to_eng_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/crj/crj_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/crj/crj_to_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/crj/crj_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/crk/config.yaml` & `g2p-1.0.20230412/g2p/mappings/langs/crk/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/crk/crk-no-symbols_to_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/crk/crk-no-symbols_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/crl/README.md` & `g2p-1.0.20230412/g2p/mappings/langs/crl/README.md`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/crl/config.yaml` & `g2p-1.0.20230412/g2p/mappings/langs/crl/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/crl/crl_equiv.json` & `g2p-1.0.20230412/g2p/mappings/langs/crl/crl_equiv.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/crl/crl_ipa_to_eng_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/crl/crl_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/crl/crl_to_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/crl/crl_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/crm/config.yaml` & `g2p-1.0.20230412/g2p/mappings/langs/crm/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/crm/crm_equiv.json` & `g2p-1.0.20230412/g2p/mappings/langs/crm/crm_equiv.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/crm/crm_ipa_to_eng_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/crm/crm_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/crm/crm_to_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/crm/crm_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/crx/stella_orth_to_syllabics.csv` & `g2p-1.0.20230412/g2p/mappings/langs/crx/stella_orth_to_syllabics.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/crx/stella_syllabics_to_orth.csv` & `g2p-1.0.20230412/g2p/mappings/langs/crx/stella_syllabics_to_orth.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/csw/config.yaml` & `g2p-1.0.20230412/g2p/mappings/langs/csw/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/csw/csw_equiv.json` & `g2p-1.0.20230412/g2p/mappings/langs/csw/csw_equiv.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/csw/csw_ipa_to_eng_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/csw/csw_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/csw/csw_to_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/csw/csw_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/ctp/config.yaml` & `g2p-1.0.20230412/g2p/mappings/langs/ctp/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/ctp/ctp_ipa_to_eng_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/ctp/ctp_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/ctp/ctp_to_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/ctp/ctp_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/dan/dan_to_dummy.json` & `g2p-1.0.20230412/g2p/mappings/langs/dan/dan_to_dummy.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/eng/config.yaml` & `g2p-1.0.20230412/g2p/mappings/langs/eng/config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -41,9 +41,17 @@
     type: mapping
     norm_form: "NFC"
     authors:
       - Patrick Littell
     mapping: eng_ipa_to_arpabet.json
     rule_ordering: apply-longest-first
     <<: *shared
-    # TODO: Need lexicon mapping
-
+  - display_name: English to IPA
+    type: lexicon
+    alignments: cmudict.ipa.aligned.txt
+    in_lang: eng
+    out_lang: eng-ipa
+    case_sensitive: false
+    norm_form: "NFC"
+    authors:
+      - David Huggins-Daines
+    <<: *shared
```

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/eng/eng_ipa_to_arpabet.json` & `g2p-1.0.20230412/g2p/mappings/langs/eng/eng_ipa_to_arpabet.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/font-encodings/README.md` & `g2p-1.0.20230412/g2p/mappings/langs/font-encodings/README.md`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/font-encodings/config.yaml` & `g2p-1.0.20230412/g2p/mappings/langs/font-encodings/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/font-encodings/fn_unicode.csv` & `g2p-1.0.20230412/g2p/mappings/langs/font-encodings/fn_unicode.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/fra/README.txt` & `g2p-1.0.20230412/g2p/mappings/langs/fra/README.txt`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/fra/fra_to_ipa.csv` & `g2p-1.0.20230412/g2p/mappings/langs/fra/fra_to_ipa.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/atj-ipa_to_eng-ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/atj-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/config.yaml` & `g2p-1.0.20230412/g2p/mappings/langs/generated/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/crg-ipa_to_eng-ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/crg-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/crk-ipa_to_eng-ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/crk-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/dan-ipa_to_eng-ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/dan-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/fin-ipa_to_eng-ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/fin-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/fra-ipa_to_eng-ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/fra-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/gla-ipa_to_eng-ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/gla-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/gwi-ipa_to_eng-ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/gwi-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/haa-ipa_to_eng-ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/haa-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/ikt-ipa_to_eng-ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/ikt-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/ikt-ipa_to_hamming-eng-ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/ikt-ipa_to_hamming-eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/iku-ipa_to_eng-ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/iku-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/iku-ipa_to_hamming-eng-ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/iku-ipa_to_hamming-eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/iku-sro-ipa_to_eng-ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/iku-sro-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/mic-ipa_to_eng-ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/mic-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/moe-ipa_to_eng-ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/moe-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/moh-equiv_to_dummy.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/moh-equiv_to_dummy.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/moh-equiv_to_hamming_dummy.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/moh-equiv_to_hamming_dummy.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/moh-ipa_to_eng-ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/moh-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/moh-ipa_to_hamming-eng-ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/moh-ipa_to_hamming-eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/oji-ipa_to_eng-ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/oji-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/oka-ipa_to_eng-ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/oka-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/str-equiv_to_dummy.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/str-equiv_to_dummy.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/str-equiv_to_hamming_dummy.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/str-equiv_to_hamming_dummy.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/str-ipa_to_eng-ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/str-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/str-ipa_to_hamming-eng-ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/str-ipa_to_hamming-eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/tau-ipa_to_eng-ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/tau-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/tce-ipa_to_eng-ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/tce-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/tli-ipa_to_eng-ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/tli-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/ttm-ipa_to_eng-ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/ttm-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/und-ascii_to_dummy.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/und-ascii_to_dummy.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/und-ascii_to_hamming_dummy.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/und-ascii_to_hamming_dummy.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/und-ipa_to_hamming-eng-ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/und-ipa_to_hamming-eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/generated/win-ipa_to_eng-ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/generated/win-ipa_to_eng-ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/git/APA.csv` & `g2p-1.0.20230412/g2p/mappings/langs/git/APA.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/git/Orthography.csv` & `g2p-1.0.20230412/g2p/mappings/langs/git/Orthography.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/git/Orthography_Deterministic.csv` & `g2p-1.0.20230412/g2p/mappings/langs/git/Orthography_Deterministic.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/git/RAPA.csv` & `g2p-1.0.20230412/g2p/mappings/langs/git/RAPA.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/git/RAPA_Deterministic.csv` & `g2p-1.0.20230412/g2p/mappings/langs/git/RAPA_Deterministic.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/git/config.yaml` & `g2p-1.0.20230412/g2p/mappings/langs/git/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/git/git_ipa_to_eng_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/git/git_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/git/git_to_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/git/git_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/gla/gla_to_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/gla/gla_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/gwi/config.yaml` & `g2p-1.0.20230412/g2p/mappings/langs/gwi/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/gwi/gwi_to_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/gwi/gwi_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/haa/config.yaml` & `g2p-1.0.20230412/g2p/mappings/langs/haa/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/haa/haa_abbs.csv` & `g2p-1.0.20230412/g2p/mappings/langs/haa/haa_abbs.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/haa/haa_to_ipa.csv` & `g2p-1.0.20230412/g2p/mappings/langs/haa/haa_to_ipa.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/ikt/ikt_to_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/ikt/ikt_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/iku/config.yaml` & `g2p-1.0.20230412/g2p/mappings/langs/iku/config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     in_lang: iku
     out_lang: iku-equiv
     type: mapping
     rule_ordering: apply-longest-first
     authors:
       - Patrick Littell
     mapping: iku_to_iku_equiv.json
-    <<: *shared
+    language_name: Inuktitut Syllabics
   - display_name: Inuktitut to IPA
     in_lang: iku-equiv
     out_lang: iku-ipa
     type: mapping
     rule_ordering: apply-longest-first
     authors:
       - Patrick Littell
@@ -25,8 +25,8 @@
     type: mapping
     case_sensitive: false
     norm_form: NFD
     rule_ordering: apply-longest-first
     authors:
       - Patrick Littell
     mapping: iku_sro_to_ipa.json
-    <<: *shared
+    language_name: Inuktitut Romanized
```

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/iku/iku_equiv_to_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/iku/iku_equiv_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/iku/iku_sro_to_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/iku/iku_sro_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/iku/iku_to_iku_equiv.json` & `g2p-1.0.20230412/g2p/mappings/langs/iku/iku_to_iku_equiv.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/kkz/config.yaml` & `g2p-1.0.20230412/g2p/mappings/langs/kkz/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/kkz/kkz_ipa_to_eng_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/kkz/kkz_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/kkz/kkz_to_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/kkz/kkz_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/kwk/config.yaml` & `g2p-1.0.20230412/g2p/mappings/langs/kwk/config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     mapping: kwk_napa_to_ipa.csv
     in_lang: kwk-napa
     out_lang: kwk-ipa
     rule_ordering: apply-longest-first
     authors:
       - Patrick Littell
       - Fineen Davis
-    <<: *shared
+    language_name: Kwak'wala (NAPA orthography)
   - display_name: Kwak'wala (U'mista) to IPA
     mapping: kwk_umista_to_ipa.json
     in_lang: kwk-umista
     out_lang: kwk-ipa
     rule_ordering: apply-longest-first
     authors:
       - Patrick Littell
@@ -29,15 +29,15 @@
   - display_name: Kwak'wala (U'mista) Equivalencies
     mapping: umista_equiv.csv
     in_lang: kwk-umista
     out_lang: kwk-umista-con
     rule_ordering: apply-longest-first
     authors:
       - Fineen Davis
-    <<: *shared
+    language_name: Kwak'wala (U'mista orthography)
   - display_name: Kwak'wala (NAPA) Equivalencies
     mapping: napa_equiv_ubc.csv
     in_lang: kwk-napa-ubc
     out_lang: kwk-napa-ubc-con
     rule_ordering: apply-longest-first
     authors:
       - Fineen Davis
@@ -54,8 +54,11 @@
     mapping: kwk_boas_to_umista.csv
     in_lang: kwk-boas
     out_lang: kwk-umista
     rule_ordering: apply-longest-first
     prevent_feeding: true
     authors:
       - Fineen Davis
-    <<: *shared
+      - Olivia Chen
+      - Daisy Rosenblum
+      - Dante cerron
+    language_name: Kwak'wala (Boas orthography)
```

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/kwk/kwk_ipa_to_eng_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/kwk/kwk_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/kwk/kwk_napa_to_xsampa.json` & `g2p-1.0.20230412/g2p/mappings/langs/kwk/kwk_napa_to_xsampa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/kwk/kwk_umista_to_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/kwk/kwk_umista_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/kwk/kwk_xsampa_to_eng_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/kwk/kwk_xsampa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/kwk/napa_equiv_ubc.csv` & `g2p-1.0.20230412/g2p/mappings/langs/kwk/napa_equiv_ubc.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/kwk/napa_equiv_uvic.csv` & `g2p-1.0.20230412/g2p/mappings/langs/kwk/napa_equiv_uvic.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/kwk/umista_equiv.csv` & `g2p-1.0.20230412/g2p/mappings/langs/kwk/umista_equiv.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/mic/mic_to_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/mic/mic_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/moe/moe_to_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/moe/moe_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/moh/config.yaml` & `g2p-1.0.20230412/g2p/mappings/langs/moh/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/moh/moh_to_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/und/und_ipa_to_eng_ipa.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.33152173913043476%*

 * *Differences: {'0': "{'out': 'ɑ'}",*

 * * '1': "{'in': 'b', 'out': 'b'}",*

 * * '10': "{'in': 'm', 'out': 'm', delete: ['context_after']}",*

 * * '12': "{'in': 'o', 'out': 'oː'}",*

 * * '13': "{'in': 'p', 'out': 'p'}",*

 * * '14': "{'in': 'q', 'out': 'k'}",*

 * * '15': "{'in': 'r', 'out': 'ɾ', delete: ['context_after']}",*

 * * '16': "{'in': 's', 'out': 's', delete: ['prevent_feeding']}",*

 * * '17': "{'in': 't', 'out': 't'}",*

 * * '18': "{'in': 't͡s', 'out': 'ts'}",*

 * * '19': "{'in': 'u', 'out': 'u'}",*

 * * '2': "{'in': 'd', 'out': 'd'}",*

 * * '20': "{'in': 'v', 'out': 'v'} […]*

```diff
@@ -1,201 +1,114 @@
 [
     {
-        "context_after": "VOWEL",
-        "in": "ti",
-        "out": "d\u0361\u0292"
-    },
-    {
-        "context_after": "VOWEL",
-        "in": "tshi",
-        "out": "t\u0361\u0283"
-    },
-    {
-        "context_after": "VOWEL",
-        "in": "hsi",
-        "out": "\u0283"
-    },
-    {
-        "in": "tsy",
-        "out": "d\u0361\u0292"
-    },
-    {
-        "context_after": "VOWEL",
-        "in": "t",
-        "out": "d"
-    },
-    {
-        "context_after": "VOWEL",
-        "in": "k",
-        "out": "\u0261"
-    },
-    {
-        "context_after": "VOWEL",
-        "in": "kw",
-        "out": "\u0261\u02b7"
-    },
-    {
-        "in": "\u00e1:",
-        "out": "\u00e1\u02d0",
-        "prevent_feeding": true
-    },
-    {
-        "in": "\u00e0:",
-        "out": "\u00e0\u02d0"
-    },
-    {
-        "in": "a:",
-        "out": "a\u02d0"
-    },
-    {
-        "in": "\u00e1",
-        "out": "\u00e1"
-    },
-    {
         "in": "a",
-        "out": "a"
-    },
-    {
-        "in": "\u00e8n:",
-        "out": "\u028c\u0303\u0300\u02d0"
-    },
-    {
-        "in": "e\u0301n:",
-        "out": "\u028c\u0303\u0301\u02d0"
-    },
-    {
-        "context_after": "CONSONANT|\\s|$",
-        "in": "e\u0301n",
-        "out": "\u028c\u0303\u0301"
-    },
-    {
-        "context_after": "CONSONANT|\\s|$",
-        "in": "en:",
-        "out": "\u028c\u0303\u02d0"
-    },
-    {
-        "context_after": "CONSONANT|\\s|$",
-        "in": "en",
-        "out": "\u028c\u0303"
+        "out": "\u0251"
     },
     {
-        "in": "\u00e8:",
-        "out": "\u00e8\u02d0"
+        "in": "b",
+        "out": "b"
     },
     {
-        "in": "\u00e9:",
-        "out": "\u00e9\u02d0",
-        "prevent_feeding": true
-    },
-    {
-        "in": "\u00e9",
-        "out": "\u00e9"
+        "in": "d",
+        "out": "d"
     },
     {
         "in": "e",
-        "out": "e"
-    },
-    {
-        "in": "i:",
-        "out": "i\u02d0"
+        "out": "e\u02d0"
     },
     {
-        "in": "\u00ed:",
-        "out": "\u00ed\u02d0",
-        "prevent_feeding": true
-    },
-    {
-        "in": "\u00ed",
-        "out": "\u00ed"
+        "in": "f",
+        "out": "f"
     },
     {
-        "in": "\u00ec:",
-        "out": "\u00ec\u02d0"
+        "in": "h",
+        "out": "h"
     },
     {
         "in": "i",
         "out": "i"
     },
     {
+        "in": "j",
+        "out": "j"
+    },
+    {
         "in": "k",
         "out": "k"
     },
     {
-        "in": "kw",
-        "out": "k\u02b7"
+        "in": "l",
+        "out": "l"
     },
     {
-        "context_after": "\\s|$",
-        "in": "kw",
-        "out": "k\u02b0\u02b7"
+        "in": "m",
+        "out": "m"
     },
     {
         "in": "n",
         "out": "n"
     },
     {
-        "in": "\u00f3n:",
-        "out": "\u0169\u0301\u02d0"
+        "in": "o",
+        "out": "o\u02d0"
     },
     {
-        "in": "\u00f2n:",
-        "out": "\u0169\u0300\u02d0"
+        "in": "p",
+        "out": "p"
     },
     {
-        "in": "\u00f3n",
-        "out": "\u0169\u0301"
+        "in": "q",
+        "out": "k"
     },
     {
-        "context_after": "CONSONANT|\\s|$",
-        "in": "on",
-        "out": "\u0169"
+        "in": "r",
+        "out": "\u027e"
     },
     {
-        "in": "\u00f3:",
-        "out": "\u00f3\u02d0",
-        "prevent_feeding": true
+        "in": "s",
+        "out": "s"
     },
     {
-        "in": "\u00f2:",
-        "out": "\u00f2\u02d0"
+        "in": "t",
+        "out": "t"
     },
     {
-        "in": "\u00f3",
-        "out": "\u00f3"
+        "in": "t\u0361s",
+        "out": "ts"
     },
     {
-        "in": "o",
-        "out": "o"
+        "in": "u",
+        "out": "u"
     },
     {
-        "in": "r",
-        "out": "r"
+        "in": "v",
+        "out": "v"
     },
     {
-        "in": "h",
-        "out": "h"
+        "in": "w",
+        "out": "w"
     },
     {
-        "in": "t",
-        "out": "t"
+        "in": "x",
+        "out": "k"
     },
     {
-        "in": "s",
-        "out": "s"
+        "in": "z",
+        "out": "z"
     },
     {
-        "in": "w",
-        "out": "w"
+        "in": "\u0259",
+        "out": "\u0259"
     },
     {
-        "in": "wh",
-        "out": "f"
+        "in": "\u0261",
+        "out": "\u0261"
     },
     {
-        "in": "y",
-        "out": "j"
+        "in": "\u0292",
+        "out": "\u0292"
     },
     {
-        "in": "'",
+        "in": "\u0294",
         "out": "\u0294"
     }
 ]
```

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/network.pkl` & `g2p-1.0.20230412/g2p/mappings/langs/network.pkl`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8004 95c3 1500 0000 0000 008c 186e 6574  .............net
+00000000: 8004 95f0 1500 0000 0000 008c 186e 6574  .............net
 00000010: 776f 726b 782e 636c 6173 7365 732e 6469  workx.classes.di
 00000020: 6772 6170 6894 8c07 4469 4772 6170 6894  graph...DiGraph.
 00000030: 9394 2981 947d 9428 8c17 6772 6170 685f  ..)..}.(..graph_
 00000040: 6174 7472 5f64 6963 745f 6661 6374 6f72  attr_dict_factor
 00000050: 7994 8c08 6275 696c 7469 6e73 948c 0464  y...builtins...d
 00000060: 6963 7494 9394 8c11 6e6f 6465 5f64 6963  ict.....node_dic
 00000070: 745f 6661 6374 6f72 7994 6808 8c16 6e6f  t_factory.h...no
@@ -42,308 +42,311 @@
 00000290: 6265 7494 7d94 8c0d 6861 6d6d 696e 672d  bet.}...hamming-
 000002a0: 6475 6d6d 7994 7d94 8c19 6861 6d6d 696e  dummy.}...hammin
 000002b0: 672d 6475 6d6d 792d 656e 672d 6172 7061  g-dummy-eng-arpa
 000002c0: 6265 7494 7d94 8c0b 656e 672d 6172 7061  bet.}...eng-arpa
 000002d0: 6265 7494 7d94 8c0f 6861 6d6d 696e 672d  bet.}...hamming-
 000002e0: 656e 672d 6970 6194 7d94 8c13 6861 6d6d  eng-ipa.}...hamm
 000002f0: 696e 672d 656e 672d 6172 7061 6265 7494  ing-eng-arpabet.
-00000300: 7d94 8c03 6669 6e94 7d94 8c07 6669 6e2d  }...fin.}...fin-
-00000310: 6970 6194 7d94 8c0a 6865 692d 646f 756c  ipa.}...hei-doul
-00000320: 6f73 947d 948c 0368 6569 947d 948c 0e68  os.}...hei.}...h
-00000330: 6569 2d74 696d 6573 2d66 6f6e 7494 7d94  ei-times-font.}.
-00000340: 8c0e 6e61 762d 7469 6d65 732d 666f 6e74  ..nav-times-font
-00000350: 947d 948c 036e 6176 947d 948c 0f66 6e2d  .}...nav.}...fn-
-00000360: 756e 6963 6f64 652d 666f 6e74 947d 948c  unicode-font.}..
-00000370: 0a66 6e2d 756e 6963 6f64 6594 7d94 8c03  .fn-unicode.}...
-00000380: 6672 6194 7d94 8c07 6672 612d 6970 6194  fra.}...fra-ipa.
-00000390: 7d94 8c07 7374 722d 6970 6194 7d94 8c07  }...str-ipa.}...
-000003a0: 7365 652d 6970 6194 7d94 8c07 6c6d 6c2d  see-ipa.}...lml-
-000003b0: 6970 6194 7d94 8c07 6f6a 692d 6970 6194  ipa.}...oji-ipa.
-000003c0: 7d94 8c07 676c 612d 6970 6194 7d94 8c07  }...gla-ipa.}...
-000003d0: 7463 652d 6970 6194 7d94 8c07 746c 692d  tce-ipa.}...tli-
-000003e0: 6970 6194 7d94 8c07 6777 692d 6970 6194  ipa.}...gwi-ipa.
-000003f0: 7d94 8c07 6d69 632d 6970 6194 7d94 8c07  }...mic-ipa.}...
-00000400: 696b 752d 6970 6194 7d94 8c07 696b 742d  iku-ipa.}...ikt-
-00000410: 6970 6194 7d94 8c0b 696b 752d 7372 6f2d  ipa.}...iku-sro-
-00000420: 6970 6194 7d94 8c07 6861 612d 6970 6194  ipa.}...haa-ipa.
-00000430: 7d94 8c07 7474 6d2d 6970 6194 7d94 8c07  }...ttm-ipa.}...
-00000440: 7461 752d 6970 6194 7d94 8c07 6d6f 682d  tau-ipa.}...moh-
-00000450: 6970 6194 7d94 8c09 6d6f 682d 6571 7569  ipa.}...moh-equi
-00000460: 7694 7d94 8c09 7374 722d 6571 7569 7694  v.}...str-equiv.
-00000470: 7d94 8c09 756e 642d 6173 6369 6994 7d94  }...und-ascii.}.
-00000480: 8c07 756e 642d 6970 6194 7d94 8c07 6d6f  ..und-ipa.}...mo
-00000490: 652d 6970 6194 7d94 8c07 7769 6e2d 6970  e-ipa.}...win-ip
-000004a0: 6194 7d94 8c07 6f6b 612d 6970 6194 7d94  a.}...oka-ipa.}.
-000004b0: 8c03 6769 7494 7d94 8c07 6769 742d 6970  ..git.}...git-ip
-000004c0: 6194 7d94 8c07 6769 742d 6170 6194 7d94  a.}...git-apa.}.
-000004d0: 8c09 6769 742d 6571 7569 7694 7d94 8c03  ..git-equiv.}...
-000004e0: 676c 6194 7d94 8c03 6777 6994 7d94 8c09  gla.}...gwi.}...
-000004f0: 6777 692d 6571 7569 7694 7d94 8c03 6861  gwi-equiv.}...ha
-00000500: 6194 7d94 8c09 6861 612d 6571 7569 7694  a.}...haa-equiv.
-00000510: 7d94 8c03 696b 7494 7d94 8c03 696b 7594  }...ikt.}...iku.
-00000520: 7d94 8c09 696b 752d 6571 7569 7694 7d94  }...iku-equiv.}.
-00000530: 8c07 696b 752d 7372 6f94 7d94 8c03 6b6b  ..iku-sro.}...kk
-00000540: 7a94 7d94 8c07 6b6b 7a2d 6970 6194 7d94  z.}...kkz-ipa.}.
-00000550: 8c07 6b77 6b2d 6970 6194 7d94 8c08 6b77  ..kwk-ipa.}...kw
-00000560: 6b2d 6e61 7061 947d 948c 0a6b 776b 2d75  k-napa.}...kwk-u
-00000570: 6d69 7374 6194 7d94 8c0e 6b77 6b2d 756d  mista.}...kwk-um
-00000580: 6973 7461 2d63 6f6e 947d 948c 0c6b 776b  ista-con.}...kwk
-00000590: 2d6e 6170 612d 7562 6394 7d94 8c10 6b77  -napa-ubc.}...kw
-000005a0: 6b2d 6e61 7061 2d75 6263 2d63 6f6e 947d  k-napa-ubc-con.}
-000005b0: 948c 0d6b 776b 2d6e 6170 612d 7576 6963  ...kwk-napa-uvic
-000005c0: 947d 948c 116b 776b 2d6e 6170 612d 7576  .}...kwk-napa-uv
-000005d0: 6963 2d63 6f6e 947d 948c 086b 776b 2d62  ic-con.}...kwk-b
-000005e0: 6f61 7394 7d94 8c03 6c6d 6c94 7d94 8c03  oas.}...lml.}...
-000005f0: 6d69 6394 7d94 8c03 6d6f 6594 7d94 8c03  mic.}...moe.}...
-00000600: 6d6f 6894 7d94 8c0c 6d6f 682d 6665 7374  moh.}...moh-fest
-00000610: 6976 616c 947d 948c 0369 7061 947d 948c  ival.}...ipa.}..
-00000620: 036f 6a69 947d 948c 076f 6a69 2d73 796c  .oji.}...oji-syl
-00000630: 947d 948c 096f 6b61 2d65 7175 6976 947d  .}...oka-equiv.}
-00000640: 948c 036f 6b61 947d 948c 0373 6565 947d  ...oka.}...see.}
-00000650: 948c 0373 7273 947d 948c 0773 7273 2d69  ...srs.}...srs-i
-00000660: 7061 947d 948c 0373 7472 947d 948c 0374  pa.}...str.}...t
-00000670: 6175 947d 948c 0974 6175 2d65 7175 6976  au.}...tau-equiv
-00000680: 947d 948c 0374 6365 947d 948c 0974 6365  .}...tce.}...tce
-00000690: 2d65 7175 6976 947d 948c 0374 6778 947d  -equiv.}...tgx.}
-000006a0: 948c 0774 6778 2d69 7061 947d 948c 0374  ...tgx-ipa.}...t
-000006b0: 6c69 947d 948c 0974 6c69 2d65 7175 6976  li.}...tli-equiv
-000006c0: 947d 948c 0374 746d 947d 948c 0974 746d  .}...ttm.}...ttm
-000006d0: 2d65 7175 6976 947d 948c 0375 6e64 947d  -equiv.}...und.}
-000006e0: 948c 0377 696e 947d 9475 8c04 5f61 646a  ...win.}.u.._adj
-000006f0: 947d 9428 6812 7d94 6814 7d94 7368 147d  .}.(h.}.h.}.sh.}
-00000700: 948c 0765 6e67 2d69 7061 947d 9473 6816  ...eng-ipa.}.sh.
-00000710: 7d94 6818 7d94 7368 187d 9468 1a7d 9473  }.h.}.sh.}.h.}.s
-00000720: 681a 7d94 685c 7d94 7368 1c7d 9468 1e7d  h.}.h\}.sh.}.h.}
-00000730: 9473 681e 7d94 8c07 656e 672d 6970 6194  .sh.}...eng-ipa.
-00000740: 7d94 7368 207d 9468 227d 9473 6822 7d94  }.sh }.h"}.sh"}.
-00000750: 6824 7d94 6826 7d94 7368 267d 948c 0765  h$}.h&}.sh&}...e
-00000760: 6e67 2d69 7061 947d 9473 6828 7d94 8c07  ng-ipa.}.sh(}...
-00000770: 6372 672d 6970 6194 7d94 7368 2a7d 9468  crg-ipa.}.sh*}.h
-00000780: 2c7d 9473 682c 7d94 682e 7d94 7368 2e7d  ,}.sh,}.h.}.sh.}
-00000790: 948c 0765 6e67 2d69 7061 947d 9473 6830  ...eng-ipa.}.sh0
-000007a0: 7d94 6832 7d94 7368 327d 948c 0765 6e67  }.h2}.sh2}...eng
-000007b0: 2d69 7061 947d 9473 6834 7d94 8c0e 6372  -ipa.}.sh4}...cr
-000007c0: 6b2d 6e6f 2d73 796d 626f 6c73 947d 9473  k-no-symbols.}.s
-000007d0: 6836 7d94 6838 7d94 7368 387d 9468 3a7d  h6}.h8}.sh8}.h:}
-000007e0: 9473 683a 7d94 8c07 656e 672d 6970 6194  .sh:}...eng-ipa.
-000007f0: 7d94 7368 3c7d 9468 3e7d 9473 683e 7d94  }.sh<}.h>}.sh>}.
-00000800: 6840 7d94 7368 407d 948c 0765 6e67 2d69  h@}.sh@}...eng-i
-00000810: 7061 947d 9473 6842 7d94 6844 7d94 7368  pa.}.shB}.hD}.sh
-00000820: 447d 948c 0763 7278 2d73 726f 947d 9473  D}...crx-sro.}.s
-00000830: 6846 7d94 6848 7d94 7368 487d 9468 4a7d  hF}.hH}.shH}.hJ}
-00000840: 9473 684a 7d94 8c07 656e 672d 6970 6194  .shJ}...eng-ipa.
-00000850: 7d94 7368 4c7d 9468 4e7d 9473 684e 7d94  }.shL}.hN}.shN}.
-00000860: 8c07 656e 672d 6970 6194 7d94 7368 507d  ..eng-ipa.}.shP}
-00000870: 9468 527d 9473 6852 7d94 8c07 656e 672d  .hR}.shR}...eng-
-00000880: 6970 6194 7d94 7368 547d 9468 567d 9473  ipa.}.shT}.hV}.s
-00000890: 6856 7d94 6858 7d94 685a 7d94 7368 5a7d  hV}.hX}.hZ}.shZ}
-000008a0: 9468 5c7d 9468 5e7d 9468 607d 9473 6860  .h\}.h^}.h`}.sh`
-000008b0: 7d94 6862 7d94 6864 7d94 7368 647d 948c  }.hb}.hd}.shd}..
-000008c0: 0765 6e67 2d69 7061 947d 9473 6866 7d94  .eng-ipa.}.shf}.
-000008d0: 6868 7d94 7368 687d 9468 6a7d 948c 0368  hh}.shh}.hj}...h
-000008e0: 6569 947d 9473 686c 7d94 686e 7d94 7368  ei.}.shl}.hn}.sh
-000008f0: 6e7d 9468 707d 9468 727d 9473 6872 7d94  n}.hp}.hr}.shr}.
-00000900: 6874 7d94 6876 7d94 7368 767d 948c 0765  ht}.hv}.shv}...e
-00000910: 6e67 2d69 7061 947d 9473 6878 7d94 288c  ng-ipa.}.shx}.(.
-00000920: 0765 6e67 2d69 7061 947d 948c 0f68 616d  .eng-ipa.}...ham
-00000930: 6d69 6e67 2d65 6e67 2d69 7061 947d 9475  ming-eng-ipa.}.u
-00000940: 687a 7d94 8c07 656e 672d 6970 6194 7d94  hz}...eng-ipa.}.
-00000950: 7368 7c7d 948c 0765 6e67 2d69 7061 947d  sh|}...eng-ipa.}
-00000960: 9473 687e 7d94 8c07 656e 672d 6970 6194  .sh~}...eng-ipa.
-00000970: 7d94 7368 807d 948c 0765 6e67 2d69 7061  }.sh.}...eng-ipa
-00000980: 947d 9473 6882 7d94 8c07 656e 672d 6970  .}.sh.}...eng-ip
-00000990: 6194 7d94 7368 847d 948c 0765 6e67 2d69  a.}.sh.}...eng-i
-000009a0: 7061 947d 9473 6886 7d94 8c07 656e 672d  pa.}.sh.}...eng-
-000009b0: 6970 6194 7d94 7368 887d 948c 0765 6e67  ipa.}.sh.}...eng
-000009c0: 2d69 7061 947d 9473 688a 7d94 288c 0765  -ipa.}.sh.}.(..e
-000009d0: 6e67 2d69 7061 947d 948c 0f68 616d 6d69  ng-ipa.}...hammi
-000009e0: 6e67 2d65 6e67 2d69 7061 947d 9475 688c  ng-eng-ipa.}.uh.
-000009f0: 7d94 288c 0765 6e67 2d69 7061 947d 948c  }.(..eng-ipa.}..
-00000a00: 0f68 616d 6d69 6e67 2d65 6e67 2d69 7061  .hamming-eng-ipa
-00000a10: 947d 9475 688e 7d94 8c07 656e 672d 6970  .}.uh.}...eng-ip
-00000a20: 6194 7d94 7368 907d 948c 0765 6e67 2d69  a.}.sh.}...eng-i
-00000a30: 7061 947d 9473 6892 7d94 8c07 656e 672d  pa.}.sh.}...eng-
-00000a40: 6970 6194 7d94 7368 947d 948c 0765 6e67  ipa.}.sh.}...eng
-00000a50: 2d69 7061 947d 9473 6896 7d94 288c 0765  -ipa.}.sh.}.(..e
-00000a60: 6e67 2d69 7061 947d 948c 0f68 616d 6d69  ng-ipa.}...hammi
-00000a70: 6e67 2d65 6e67 2d69 7061 947d 9468 dc7d  ng-eng-ipa.}.h.}
-00000a80: 9468 de7d 9475 6898 7d94 288c 0564 756d  .h.}.uh.}.(..dum
-00000a90: 6d79 947d 948c 0d68 616d 6d69 6e67 2d64  my.}...hamming-d
-00000aa0: 756d 6d79 947d 948c 076d 6f68 2d69 7061  ummy.}...moh-ipa
-00000ab0: 947d 9475 689a 7d94 288c 0564 756d 6d79  .}.uh.}.(..dummy
-00000ac0: 947d 948c 0d68 616d 6d69 6e67 2d64 756d  .}...hamming-dum
-00000ad0: 6d79 947d 948c 0773 7472 2d69 7061 947d  my.}...str-ipa.}
-00000ae0: 9475 689c 7d94 288c 0564 756d 6d79 947d  .uh.}.(..dummy.}
-00000af0: 948c 0d68 616d 6d69 6e67 2d64 756d 6d79  ...hamming-dummy
-00000b00: 947d 948c 0775 6e64 2d69 7061 947d 9475  .}...und-ipa.}.u
-00000b10: 689e 7d94 288c 0f68 616d 6d69 6e67 2d65  h.}.(..hamming-e
-00000b20: 6e67 2d69 7061 947d 948c 0765 6e67 2d69  ng-ipa.}...eng-i
-00000b30: 7061 947d 9475 68a0 7d94 8c07 656e 672d  pa.}.uh.}...eng-
-00000b40: 6970 6194 7d94 7368 a27d 948c 0765 6e67  ipa.}.sh.}...eng
-00000b50: 2d69 7061 947d 9473 68a4 7d94 8c07 656e  -ipa.}.sh.}...en
-00000b60: 672d 6970 6194 7d94 7368 a67d 9428 68a8  g-ipa.}.sh.}.(h.
-00000b70: 7d94 68aa 7d94 68ac 7d94 7568 a87d 948c  }.h.}.h.}.uh.}..
-00000b80: 0765 6e67 2d69 7061 947d 9473 68aa 7d94  .eng-ipa.}.sh.}.
-00000b90: 68ac 7d94 68ae 7d94 8c07 676c 612d 6970  h.}.h.}...gla-ip
-00000ba0: 6194 7d94 7368 b07d 9468 b27d 9473 68b2  a.}.sh.}.h.}.sh.
-00000bb0: 7d94 8c07 6777 692d 6970 6194 7d94 7368  }...gwi-ipa.}.sh
-00000bc0: b47d 9468 b67d 9473 68b6 7d94 8c07 6861  .}.h.}.sh.}...ha
-00000bd0: 612d 6970 6194 7d94 7368 b87d 948c 0769  a-ipa.}.sh.}...i
-00000be0: 6b74 2d69 7061 947d 9473 68ba 7d94 68bc  kt-ipa.}.sh.}.h.
-00000bf0: 7d94 7368 bc7d 948c 0769 6b75 2d69 7061  }.sh.}...iku-ipa
-00000c00: 947d 9473 68be 7d94 8c0b 696b 752d 7372  .}.sh.}...iku-sr
-00000c10: 6f2d 6970 6194 7d94 7368 c07d 9468 c27d  o-ipa.}.sh.}.h.}
-00000c20: 9473 68c2 7d94 8c07 656e 672d 6970 6194  .sh.}...eng-ipa.
-00000c30: 7d94 7368 c47d 948c 0765 6e67 2d69 7061  }.sh.}...eng-ipa
-00000c40: 947d 9473 68c6 7d94 8c07 6b77 6b2d 6970  .}.sh.}...kwk-ip
-00000c50: 6194 7d94 7368 c87d 9428 8c07 6b77 6b2d  a.}.sh.}.(..kwk-
-00000c60: 6970 6194 7d94 68ca 7d94 7568 ca7d 9468  ipa.}.h.}.uh.}.h
-00000c70: cc7d 9468 ce7d 9473 68ce 7d94 68d0 7d94  .}.h.}.sh.}.h.}.
-00000c80: 68d2 7d94 7368 d27d 9468 d47d 948c 0a6b  h.}.sh.}.h.}...k
-00000c90: 776b 2d75 6d69 7374 6194 7d94 7368 d67d  wk-umista.}.sh.}
-00000ca0: 948c 076c 6d6c 2d69 7061 947d 9473 68d8  ...lml-ipa.}.sh.
-00000cb0: 7d94 8c07 6d69 632d 6970 6194 7d94 7368  }...mic-ipa.}.sh
-00000cc0: da7d 948c 076d 6f65 2d69 7061 947d 9473  .}...moe-ipa.}.s
-00000cd0: 68dc 7d94 8c09 6d6f 682d 6571 7569 7694  h.}...moh-equiv.
-00000ce0: 7d94 7368 de7d 948c 076d 6f68 2d69 7061  }.sh.}...moh-ipa
-00000cf0: 947d 9473 68e0 7d94 8c03 6970 6194 7d94  .}.sh.}...ipa.}.
-00000d00: 7368 e27d 948c 076f 6a69 2d69 7061 947d  sh.}...oji-ipa.}
-00000d10: 9473 68e4 7d94 8c03 6f6a 6994 7d94 7368  .sh.}...oji.}.sh
-00000d20: e67d 948c 076f 6b61 2d69 7061 947d 9473  .}...oka-ipa.}.s
-00000d30: 68e8 7d94 8c09 6f6b 612d 6571 7569 7694  h.}...oka-equiv.
-00000d40: 7d94 7368 ea7d 948c 0773 6565 2d69 7061  }.sh.}...see-ipa
-00000d50: 947d 9473 68ec 7d94 68ee 7d94 7368 ee7d  .}.sh.}.h.}.sh.}
-00000d60: 948c 0765 6e67 2d69 7061 947d 9473 68f0  ...eng-ipa.}.sh.
-00000d70: 7d94 8c09 7374 722d 6571 7569 7694 7d94  }...str-equiv.}.
-00000d80: 7368 f27d 9468 f47d 9473 68f4 7d94 8c07  sh.}.h.}.sh.}...
-00000d90: 7461 752d 6970 6194 7d94 7368 f67d 9468  tau-ipa.}.sh.}.h
-00000da0: f87d 9473 68f8 7d94 8c07 7463 652d 6970  .}.sh.}...tce-ip
-00000db0: 6194 7d94 7368 fa7d 9468 fc7d 9473 68fc  a.}.sh.}.h.}.sh.
-00000dc0: 7d94 8c07 656e 672d 6970 6194 7d94 7368  }...eng-ipa.}.sh
-00000dd0: fe7d 946a 0001 0000 7d94 736a 0001 0000  .}.j....}.sj....
-00000de0: 7d94 8c07 746c 692d 6970 6194 7d94 736a  }...tli-ipa.}.sj
-00000df0: 0201 0000 7d94 6a04 0100 007d 9473 6a04  ....}.j....}.sj.
-00000e00: 0100 007d 948c 0774 746d 2d69 7061 947d  ...}...ttm-ipa.}
-00000e10: 9473 6a06 0100 007d 948c 0975 6e64 2d61  .sj....}...und-a
-00000e20: 7363 6969 947d 9473 6a08 0100 007d 948c  scii.}.sj....}..
-00000e30: 0777 696e 2d69 7061 947d 9473 758c 055f  .win-ipa.}.su.._
-00000e40: 7072 6564 947d 9428 6812 7d94 6814 7d94  pred.}.(h.}.h.}.
-00000e50: 6812 6a0d 0100 0073 6816 7d94 6818 7d94  h.j....sh.}.h.}.
-00000e60: 6816 6a12 0100 0073 681a 7d94 288c 0761  h.j....sh.}.(..a
-00000e70: 746a 2d69 7061 946a 1401 0000 8c07 636b  tj-ipa.j......ck
-00000e80: 742d 6970 6194 6a1b 0100 008c 0763 726a  t-ipa.j......crj
-00000e90: 2d69 7061 946a 2d01 0000 8c07 6372 6c2d  -ipa.j-.....crl-
-00000ea0: 6970 6194 6a3c 0100 008c 0763 726d 2d69  ipa.j<.....crm-i
-00000eb0: 7061 946a 4301 0000 8c07 6373 772d 6970  pa.jC.....csw-ip
-00000ec0: 6194 6a4f 0100 008c 0763 7470 2d69 7061  a.jO.....ctp-ipa
-00000ed0: 946a 5401 0000 8c07 6461 6e2d 6970 6194  .jT.....dan-ipa.
-00000ee0: 6a59 0100 008c 0766 7261 2d69 7061 946a  jY.....fra-ipa.j
-00000ef0: 7901 0000 6878 6a7c 0100 008c 0761 6c71  y...hxj|.....alq
-00000f00: 2d69 7061 946a 1001 0000 687a 6a81 0100  -ipa.j....hzj...
-00000f10: 0068 7c6a 8401 0000 687e 6a87 0100 0068  .h|j....h~j....h
-00000f20: 806a 8a01 0000 8c07 6372 6b2d 6970 6194  .j......crk-ipa.
-00000f30: 6a32 0100 0068 826a 8d01 0000 8c07 6372  j2...h.j......cr
-00000f40: 672d 6970 6194 6a23 0100 0068 846a 9001  g-ipa.j#...h.j..
-00000f50: 0000 6886 6a93 0100 0068 886a 9601 0000  ..h.j....h.j....
-00000f60: 688a 6a99 0100 0068 8c6a 9e01 0000 688e  h.j....h.j....h.
-00000f70: 6aa3 0100 0068 906a a601 0000 6892 6aa9  j....h.j....h.j.
-00000f80: 0100 0068 946a ac01 0000 6896 6aaf 0100  ...h.j....h.j...
-00000f90: 0068 a06a d001 0000 68a2 6ad3 0100 008c  .h.j....h.j.....
-00000fa0: 0766 696e 2d69 7061 946a 6801 0000 68a4  .fin-ipa.jh...h.
-00000fb0: 6ad6 0100 008c 0767 6974 2d69 7061 946a  j......git-ipa.j
-00000fc0: dd01 0000 8c07 6b6b 7a2d 6970 6194 6afc  ......kkz-ipa.j.
-00000fd0: 0100 0068 c46a ff01 0000 8c07 7372 732d  ...h.j......srs-
-00000fe0: 6970 6194 6a36 0200 008c 0774 6778 2d69  ipa.j6.....tgx-i
-00000ff0: 7061 946a 4802 0000 8c07 756e 642d 6970  pa.jH.....und-ip
-00001000: 6194 6acd 0100 0075 681c 7d94 681e 7d94  a.j....uh.}.h.}.
-00001010: 681c 6a18 0100 0073 6820 7d94 6822 7d94  h.j....sh }.h"}.
-00001020: 6820 6a1d 0100 0073 6824 7d94 6826 7d94  h j....sh$}.h&}.
-00001030: 2868 246a 2001 0000 6828 6a26 0100 0075  (h$j ...h(j&...u
-00001040: 6828 7d94 682a 7d94 682c 7d94 682a 6a28  h(}.h*}.h,}.h*j(
-00001050: 0100 0073 682e 7d94 8c09 6372 6a2d 6571  ...sh.}...crj-eq
-00001060: 7569 7694 6a2a 0100 0073 6830 7d94 6834  uiv.j*...sh0}.h4
-00001070: 6a35 0100 0073 6832 7d94 6830 6a2f 0100  j5...sh2}.h0j/..
-00001080: 0073 6834 7d94 6836 7d94 6838 7d94 6836  .sh4}.h6}.h8}.h6
-00001090: 6a37 0100 0073 683a 7d94 8c09 6372 6c2d  j7...sh:}...crl-
-000010a0: 6571 7569 7694 6a39 0100 0073 683c 7d94  equiv.j9...sh<}.
-000010b0: 683e 7d94 683c 6a3e 0100 0073 6840 7d94  h>}.h<j>...sh@}.
-000010c0: 8c09 6372 6d2d 6571 7569 7694 6a40 0100  ..crm-equiv.j@..
-000010d0: 0073 6842 7d94 8c07 6372 782d 7379 6c94  .shB}...crx-syl.
-000010e0: 6a48 0100 0073 6844 7d94 6842 6a45 0100  jH...shD}.hBjE..
-000010f0: 0073 6846 7d94 6848 7d94 6846 6a4a 0100  .shF}.hH}.hFjJ..
-00001100: 0073 684a 7d94 8c09 6373 772d 6571 7569  .shJ}...csw-equi
-00001110: 7694 6a4c 0100 0073 684c 7d94 684e 7d94  v.jL...shL}.hN}.
-00001120: 684c 6a51 0100 0073 6850 7d94 6852 7d94  hLjQ...shP}.hR}.
-00001130: 6850 6a56 0100 0073 6854 7d94 2868 986a  hPjV...shT}.(h.j
-00001140: b601 0000 689a 6abd 0100 0068 9c6a c401  ....h.j....h.j..
-00001150: 0000 7568 567d 9468 546a 5b01 0000 7368  ..uhV}.hTj[...sh
-00001160: 587d 9428 8c09 6d6f 682d 6571 7569 7694  X}.(..moh-equiv.
-00001170: 6ab8 0100 008c 0973 7472 2d65 7175 6976  j......str-equiv
-00001180: 946a bf01 0000 8c09 756e 642d 6173 6369  .j......und-asci
-00001190: 6994 6ac6 0100 0075 685a 7d94 6858 6a5e  i.j....uhZ}.hXj^
-000011a0: 0100 0073 685c 7d94 8c07 656e 672d 6970  ...sh\}...eng-ip
-000011b0: 6194 6a16 0100 0073 685e 7d94 288c 0773  a.j....sh^}.(..s
-000011c0: 7472 2d69 7061 946a 7e01 0000 8c07 6d6f  tr-ipa.j~.....mo
-000011d0: 682d 6970 6194 6ab1 0100 008c 0769 6b75  h-ipa.j......iku
-000011e0: 2d69 7061 946a 9b01 0000 689e 6acb 0100  -ipa.j....h.j...
-000011f0: 008c 0769 6b74 2d69 7061 946a a001 0000  ...ikt-ipa.j....
-00001200: 7568 607d 9468 5e6a 6201 0000 7368 627d  uh`}.h^jb...shb}
-00001210: 9468 647d 9468 626a 6501 0000 7368 667d  .hd}.hbje...shf}
-00001220: 9468 687d 9428 6866 6a6a 0100 0068 6a6a  .hh}.(hfjj...hjj
-00001230: 6e01 0000 7568 6a7d 9468 6c7d 9468 6e7d  n...uhj}.hl}.hn}
-00001240: 9468 6c6a 7001 0000 7368 707d 9468 727d  .hljp...shp}.hr}
-00001250: 9468 706a 7301 0000 7368 747d 9468 767d  .hpjs...sht}.hv}
-00001260: 9468 746a 7601 0000 7368 787d 948c 0973  .htjv...shx}...s
-00001270: 7472 2d65 7175 6976 946a c101 0000 7368  tr-equiv.j....sh
-00001280: 7a7d 9468 ea6a 3102 0000 7368 7c7d 9468  z}.h.j1...sh|}.h
-00001290: d66a 1302 0000 7368 7e7d 9468 e26a 2502  .j....sh~}.h.j%.
-000012a0: 0000 7368 807d 9468 ae6a e201 0000 7368  ..sh.}.h.j....sh
-000012b0: 827d 948c 0974 6365 2d65 7175 6976 946a  .}...tce-equiv.j
-000012c0: 4302 0000 7368 847d 948c 0974 6c69 2d65  C...sh.}...tli-e
-000012d0: 7175 6976 946a 4d02 0000 7368 867d 948c  quiv.jM...sh.}..
-000012e0: 0967 7769 2d65 7175 6976 946a e701 0000  .gwi-equiv.j....
-000012f0: 7368 887d 9468 d86a 1602 0000 7368 8a7d  sh.}.h.j....sh.}
-00001300: 948c 0969 6b75 2d65 7175 6976 946a f401  ...iku-equiv.j..
-00001310: 0000 7368 8c7d 9468 b86a ef01 0000 7368  ..sh.}.h.j....sh
-00001320: 8e7d 9468 be6a f701 0000 7368 907d 948c  .}.h.j....sh.}..
-00001330: 0968 6161 2d65 7175 6976 946a ec01 0000  .haa-equiv.j....
-00001340: 7368 927d 948c 0974 746d 2d65 7175 6976  sh.}...ttm-equiv
-00001350: 946a 5202 0000 7368 947d 948c 0974 6175  .jR...sh.}...tau
-00001360: 2d65 7175 6976 946a 3e02 0000 7368 967d  -equiv.j>...sh.}
-00001370: 9428 8c09 6d6f 682d 6571 7569 7694 6aba  .(..moh-equiv.j.
-00001380: 0100 008c 0c6d 6f68 2d66 6573 7469 7661  .....moh-festiva
-00001390: 6c94 6a1f 0200 0075 6898 7d94 8c03 6d6f  l.j....uh.}...mo
-000013a0: 6894 6a1c 0200 0073 689a 7d94 68f0 6a39  h.j....sh.}.h.j9
-000013b0: 0200 0073 689c 7d94 6a06 0100 006a 5502  ...sh.}.j....jU.
-000013c0: 0000 7368 9e7d 948c 0975 6e64 2d61 7363  ..sh.}...und-asc
-000013d0: 6969 946a c801 0000 7368 a07d 9468 da6a  ii.j....sh.}.h.j
-000013e0: 1902 0000 7368 a27d 946a 0801 0000 6a58  ....sh.}.j....jX
-000013f0: 0200 0073 68a4 7d94 68e6 6a2b 0200 0073  ...sh.}.h.j+...s
-00001400: 68a6 7d94 68a8 7d94 68a6 6ad8 0100 0073  h.}.h.}.h.j....s
-00001410: 68aa 7d94 8c03 6769 7494 6ad9 0100 0073  h.}...git.j....s
-00001420: 68ac 7d94 8c03 6769 7494 6ada 0100 0073  h.}...git.j....s
-00001430: 68ae 7d94 68b0 7d94 68b2 7d94 68b0 6ae4  h.}.h.}.h.}.h.j.
-00001440: 0100 0073 68b4 7d94 68b6 7d94 68b4 6ae9  ...sh.}.h.}.h.j.
-00001450: 0100 0073 68b8 7d94 68ba 7d94 68bc 7d94  ...sh.}.h.}.h.}.
-00001460: 68ba 6af1 0100 0073 68be 7d94 68c0 7d94  h.j....sh.}.h.}.
-00001470: 68c2 7d94 68c0 6af9 0100 0073 68c4 7d94  h.}.h.j....sh.}.
-00001480: 2868 c66a 0202 0000 68c8 6a05 0200 0075  (h.j....h.j....u
-00001490: 68c6 7d94 68c8 7d94 68d4 6a10 0200 0073  h.}.h.}.h.j....s
-000014a0: 68ca 7d94 8c0a 6b77 6b2d 756d 6973 7461  h.}...kwk-umista
-000014b0: 946a 0602 0000 7368 cc7d 9468 ce7d 9468  .j....sh.}.h.}.h
-000014c0: cc6a 0902 0000 7368 d07d 9468 d27d 9468  .j....sh.}.h.}.h
-000014d0: d06a 0c02 0000 7368 d47d 9468 d67d 9468  .j....sh.}.h.}.h
-000014e0: d87d 9468 da7d 9468 dc7d 948c 076d 6f68  .}.h.}.h.}...moh
-000014f0: 2d69 7061 946a b201 0000 7368 de7d 948c  -ipa.j....sh.}..
-00001500: 076d 6f68 2d69 7061 946a b301 0000 7368  .moh-ipa.j....sh
-00001510: e07d 9468 e06a 2202 0000 7368 e27d 9468  .}.h.j"...sh.}.h
-00001520: e46a 2802 0000 7368 e47d 9468 e67d 9468  .j(...sh.}.h.}.h
-00001530: e86a 2e02 0000 7368 e87d 9468 ea7d 9468  .j....sh.}.h.}.h
-00001540: ec7d 9468 ee7d 9468 ec6a 3302 0000 7368  .}.h.}.h.j3...sh
-00001550: f07d 9468 f27d 9468 f47d 9468 f26a 3b02  .}.h.}.h.}.h.j;.
-00001560: 0000 7368 f67d 9468 f87d 9468 f66a 4002  ..sh.}.h.}.h.j@.
-00001570: 0000 7368 fa7d 9468 fc7d 9468 fa6a 4502  ..sh.}.h.}.h.jE.
-00001580: 0000 7368 fe7d 946a 0001 0000 7d94 68fe  ..sh.}.j....}.h.
-00001590: 6a4a 0200 0073 6a02 0100 007d 946a 0401  jJ...sj....}.j..
-000015a0: 0000 7d94 6a02 0100 006a 4f02 0000 736a  ..}.j....jO...sj
-000015b0: 0601 0000 7d94 6a08 0100 007d 9475 8c05  ....}.j....}.u..
-000015c0: 5f73 7563 6394 6a0b 0100 0075 622e       _succ.j....ub.
+00000300: 7d94 8c03 656e 6794 7d94 8c03 6669 6e94  }...eng.}...fin.
+00000310: 7d94 8c07 6669 6e2d 6970 6194 7d94 8c0a  }...fin-ipa.}...
+00000320: 6865 692d 646f 756c 6f73 947d 948c 0368  hei-doulos.}...h
+00000330: 6569 947d 948c 0e68 6569 2d74 696d 6573  ei.}...hei-times
+00000340: 2d66 6f6e 7494 7d94 8c0e 6e61 762d 7469  -font.}...nav-ti
+00000350: 6d65 732d 666f 6e74 947d 948c 036e 6176  mes-font.}...nav
+00000360: 947d 948c 0f66 6e2d 756e 6963 6f64 652d  .}...fn-unicode-
+00000370: 666f 6e74 947d 948c 0a66 6e2d 756e 6963  font.}...fn-unic
+00000380: 6f64 6594 7d94 8c03 6672 6194 7d94 8c07  ode.}...fra.}...
+00000390: 6672 612d 6970 6194 7d94 8c07 7374 722d  fra-ipa.}...str-
+000003a0: 6970 6194 7d94 8c07 7365 652d 6970 6194  ipa.}...see-ipa.
+000003b0: 7d94 8c07 6c6d 6c2d 6970 6194 7d94 8c07  }...lml-ipa.}...
+000003c0: 6f6a 692d 6970 6194 7d94 8c07 676c 612d  oji-ipa.}...gla-
+000003d0: 6970 6194 7d94 8c07 7463 652d 6970 6194  ipa.}...tce-ipa.
+000003e0: 7d94 8c07 746c 692d 6970 6194 7d94 8c07  }...tli-ipa.}...
+000003f0: 6777 692d 6970 6194 7d94 8c07 6d69 632d  gwi-ipa.}...mic-
+00000400: 6970 6194 7d94 8c07 696b 752d 6970 6194  ipa.}...iku-ipa.
+00000410: 7d94 8c07 696b 742d 6970 6194 7d94 8c0b  }...ikt-ipa.}...
+00000420: 696b 752d 7372 6f2d 6970 6194 7d94 8c07  iku-sro-ipa.}...
+00000430: 6861 612d 6970 6194 7d94 8c07 7474 6d2d  haa-ipa.}...ttm-
+00000440: 6970 6194 7d94 8c07 7461 752d 6970 6194  ipa.}...tau-ipa.
+00000450: 7d94 8c07 6d6f 682d 6970 6194 7d94 8c09  }...moh-ipa.}...
+00000460: 6d6f 682d 6571 7569 7694 7d94 8c09 7374  moh-equiv.}...st
+00000470: 722d 6571 7569 7694 7d94 8c09 756e 642d  r-equiv.}...und-
+00000480: 6173 6369 6994 7d94 8c07 756e 642d 6970  ascii.}...und-ip
+00000490: 6194 7d94 8c07 6d6f 652d 6970 6194 7d94  a.}...moe-ipa.}.
+000004a0: 8c07 7769 6e2d 6970 6194 7d94 8c07 6f6b  ..win-ipa.}...ok
+000004b0: 612d 6970 6194 7d94 8c03 6769 7494 7d94  a-ipa.}...git.}.
+000004c0: 8c07 6769 742d 6970 6194 7d94 8c07 6769  ..git-ipa.}...gi
+000004d0: 742d 6170 6194 7d94 8c09 6769 742d 6571  t-apa.}...git-eq
+000004e0: 7569 7694 7d94 8c03 676c 6194 7d94 8c03  uiv.}...gla.}...
+000004f0: 6777 6994 7d94 8c09 6777 692d 6571 7569  gwi.}...gwi-equi
+00000500: 7694 7d94 8c03 6861 6194 7d94 8c09 6861  v.}...haa.}...ha
+00000510: 612d 6571 7569 7694 7d94 8c03 696b 7494  a-equiv.}...ikt.
+00000520: 7d94 8c03 696b 7594 7d94 8c09 696b 752d  }...iku.}...iku-
+00000530: 6571 7569 7694 7d94 8c07 696b 752d 7372  equiv.}...iku-sr
+00000540: 6f94 7d94 8c03 6b6b 7a94 7d94 8c07 6b6b  o.}...kkz.}...kk
+00000550: 7a2d 6970 6194 7d94 8c07 6b77 6b2d 6970  z-ipa.}...kwk-ip
+00000560: 6194 7d94 8c08 6b77 6b2d 6e61 7061 947d  a.}...kwk-napa.}
+00000570: 948c 0a6b 776b 2d75 6d69 7374 6194 7d94  ...kwk-umista.}.
+00000580: 8c0e 6b77 6b2d 756d 6973 7461 2d63 6f6e  ..kwk-umista-con
+00000590: 947d 948c 0c6b 776b 2d6e 6170 612d 7562  .}...kwk-napa-ub
+000005a0: 6394 7d94 8c10 6b77 6b2d 6e61 7061 2d75  c.}...kwk-napa-u
+000005b0: 6263 2d63 6f6e 947d 948c 0d6b 776b 2d6e  bc-con.}...kwk-n
+000005c0: 6170 612d 7576 6963 947d 948c 116b 776b  apa-uvic.}...kwk
+000005d0: 2d6e 6170 612d 7576 6963 2d63 6f6e 947d  -napa-uvic-con.}
+000005e0: 948c 086b 776b 2d62 6f61 7394 7d94 8c03  ...kwk-boas.}...
+000005f0: 6c6d 6c94 7d94 8c03 6d69 6394 7d94 8c03  lml.}...mic.}...
+00000600: 6d6f 6594 7d94 8c03 6d6f 6894 7d94 8c0c  moe.}...moh.}...
+00000610: 6d6f 682d 6665 7374 6976 616c 947d 948c  moh-festival.}..
+00000620: 0369 7061 947d 948c 036f 6a69 947d 948c  .ipa.}...oji.}..
+00000630: 076f 6a69 2d73 796c 947d 948c 096f 6b61  .oji-syl.}...oka
+00000640: 2d65 7175 6976 947d 948c 036f 6b61 947d  -equiv.}...oka.}
+00000650: 948c 0373 6565 947d 948c 0373 7273 947d  ...see.}...srs.}
+00000660: 948c 0773 7273 2d69 7061 947d 948c 0373  ...srs-ipa.}...s
+00000670: 7472 947d 948c 0374 6175 947d 948c 0974  tr.}...tau.}...t
+00000680: 6175 2d65 7175 6976 947d 948c 0374 6365  au-equiv.}...tce
+00000690: 947d 948c 0974 6365 2d65 7175 6976 947d  .}...tce-equiv.}
+000006a0: 948c 0374 6778 947d 948c 0774 6778 2d69  ...tgx.}...tgx-i
+000006b0: 7061 947d 948c 0374 6c69 947d 948c 0974  pa.}...tli.}...t
+000006c0: 6c69 2d65 7175 6976 947d 948c 0374 746d  li-equiv.}...ttm
+000006d0: 947d 948c 0974 746d 2d65 7175 6976 947d  .}...ttm-equiv.}
+000006e0: 948c 0375 6e64 947d 948c 0377 696e 947d  ...und.}...win.}
+000006f0: 9475 8c04 5f61 646a 947d 9428 6812 7d94  .u.._adj.}.(h.}.
+00000700: 6814 7d94 7368 147d 948c 0765 6e67 2d69  h.}.sh.}...eng-i
+00000710: 7061 947d 9473 6816 7d94 6818 7d94 7368  pa.}.sh.}.h.}.sh
+00000720: 187d 9468 1a7d 9473 681a 7d94 685c 7d94  .}.h.}.sh.}.h\}.
+00000730: 7368 1c7d 9468 1e7d 9473 681e 7d94 8c07  sh.}.h.}.sh.}...
+00000740: 656e 672d 6970 6194 7d94 7368 207d 9468  eng-ipa.}.sh }.h
+00000750: 227d 9473 6822 7d94 6824 7d94 6826 7d94  "}.sh"}.h$}.h&}.
+00000760: 7368 267d 948c 0765 6e67 2d69 7061 947d  sh&}...eng-ipa.}
+00000770: 9473 6828 7d94 8c07 6372 672d 6970 6194  .sh(}...crg-ipa.
+00000780: 7d94 7368 2a7d 9468 2c7d 9473 682c 7d94  }.sh*}.h,}.sh,}.
+00000790: 682e 7d94 7368 2e7d 948c 0765 6e67 2d69  h.}.sh.}...eng-i
+000007a0: 7061 947d 9473 6830 7d94 6832 7d94 7368  pa.}.sh0}.h2}.sh
+000007b0: 327d 948c 0765 6e67 2d69 7061 947d 9473  2}...eng-ipa.}.s
+000007c0: 6834 7d94 8c0e 6372 6b2d 6e6f 2d73 796d  h4}...crk-no-sym
+000007d0: 626f 6c73 947d 9473 6836 7d94 6838 7d94  bols.}.sh6}.h8}.
+000007e0: 7368 387d 9468 3a7d 9473 683a 7d94 8c07  sh8}.h:}.sh:}...
+000007f0: 656e 672d 6970 6194 7d94 7368 3c7d 9468  eng-ipa.}.sh<}.h
+00000800: 3e7d 9473 683e 7d94 6840 7d94 7368 407d  >}.sh>}.h@}.sh@}
+00000810: 948c 0765 6e67 2d69 7061 947d 9473 6842  ...eng-ipa.}.shB
+00000820: 7d94 6844 7d94 7368 447d 948c 0763 7278  }.hD}.shD}...crx
+00000830: 2d73 726f 947d 9473 6846 7d94 6848 7d94  -sro.}.shF}.hH}.
+00000840: 7368 487d 9468 4a7d 9473 684a 7d94 8c07  shH}.hJ}.shJ}...
+00000850: 656e 672d 6970 6194 7d94 7368 4c7d 9468  eng-ipa.}.shL}.h
+00000860: 4e7d 9473 684e 7d94 8c07 656e 672d 6970  N}.shN}...eng-ip
+00000870: 6194 7d94 7368 507d 9468 527d 9473 6852  a.}.shP}.hR}.shR
+00000880: 7d94 8c07 656e 672d 6970 6194 7d94 7368  }...eng-ipa.}.sh
+00000890: 547d 9468 567d 9473 6856 7d94 6858 7d94  T}.hV}.shV}.hX}.
+000008a0: 685a 7d94 7368 5a7d 9468 5c7d 9468 5e7d  hZ}.shZ}.h\}.h^}
+000008b0: 9468 607d 9473 6860 7d94 6862 7d94 8c07  .h`}.sh`}.hb}...
+000008c0: 656e 672d 6970 6194 7d94 7368 647d 9468  eng-ipa.}.shd}.h
+000008d0: 667d 9473 6866 7d94 8c07 656e 672d 6970  f}.shf}...eng-ip
+000008e0: 6194 7d94 7368 687d 9468 6a7d 9473 686a  a.}.shh}.hj}.shj
+000008f0: 7d94 686c 7d94 8c03 6865 6994 7d94 7368  }.hl}...hei.}.sh
+00000900: 6e7d 9468 707d 9473 6870 7d94 6872 7d94  n}.hp}.shp}.hr}.
+00000910: 6874 7d94 7368 747d 9468 767d 9468 787d  ht}.sht}.hv}.hx}
+00000920: 9473 6878 7d94 8c07 656e 672d 6970 6194  .shx}...eng-ipa.
+00000930: 7d94 7368 7a7d 9428 8c07 656e 672d 6970  }.shz}.(..eng-ip
+00000940: 6194 7d94 8c0f 6861 6d6d 696e 672d 656e  a.}...hamming-en
+00000950: 672d 6970 6194 7d94 7568 7c7d 948c 0765  g-ipa.}.uh|}...e
+00000960: 6e67 2d69 7061 947d 9473 687e 7d94 8c07  ng-ipa.}.sh~}...
+00000970: 656e 672d 6970 6194 7d94 7368 807d 948c  eng-ipa.}.sh.}..
+00000980: 0765 6e67 2d69 7061 947d 9473 6882 7d94  .eng-ipa.}.sh.}.
+00000990: 8c07 656e 672d 6970 6194 7d94 7368 847d  ..eng-ipa.}.sh.}
+000009a0: 948c 0765 6e67 2d69 7061 947d 9473 6886  ...eng-ipa.}.sh.
+000009b0: 7d94 8c07 656e 672d 6970 6194 7d94 7368  }...eng-ipa.}.sh
+000009c0: 887d 948c 0765 6e67 2d69 7061 947d 9473  .}...eng-ipa.}.s
+000009d0: 688a 7d94 8c07 656e 672d 6970 6194 7d94  h.}...eng-ipa.}.
+000009e0: 7368 8c7d 9428 8c07 656e 672d 6970 6194  sh.}.(..eng-ipa.
+000009f0: 7d94 8c0f 6861 6d6d 696e 672d 656e 672d  }...hamming-eng-
+00000a00: 6970 6194 7d94 7568 8e7d 9428 8c07 656e  ipa.}.uh.}.(..en
+00000a10: 672d 6970 6194 7d94 8c0f 6861 6d6d 696e  g-ipa.}...hammin
+00000a20: 672d 656e 672d 6970 6194 7d94 7568 907d  g-eng-ipa.}.uh.}
+00000a30: 948c 0765 6e67 2d69 7061 947d 9473 6892  ...eng-ipa.}.sh.
+00000a40: 7d94 8c07 656e 672d 6970 6194 7d94 7368  }...eng-ipa.}.sh
+00000a50: 947d 948c 0765 6e67 2d69 7061 947d 9473  .}...eng-ipa.}.s
+00000a60: 6896 7d94 8c07 656e 672d 6970 6194 7d94  h.}...eng-ipa.}.
+00000a70: 7368 987d 9428 8c07 656e 672d 6970 6194  sh.}.(..eng-ipa.
+00000a80: 7d94 8c0f 6861 6d6d 696e 672d 656e 672d  }...hamming-eng-
+00000a90: 6970 6194 7d94 68de 7d94 68e0 7d94 7568  ipa.}.h.}.h.}.uh
+00000aa0: 9a7d 9428 8c05 6475 6d6d 7994 7d94 8c0d  .}.(..dummy.}...
+00000ab0: 6861 6d6d 696e 672d 6475 6d6d 7994 7d94  hamming-dummy.}.
+00000ac0: 8c07 6d6f 682d 6970 6194 7d94 7568 9c7d  ..moh-ipa.}.uh.}
+00000ad0: 9428 8c05 6475 6d6d 7994 7d94 8c0d 6861  .(..dummy.}...ha
+00000ae0: 6d6d 696e 672d 6475 6d6d 7994 7d94 8c07  mming-dummy.}...
+00000af0: 7374 722d 6970 6194 7d94 7568 9e7d 9428  str-ipa.}.uh.}.(
+00000b00: 8c05 6475 6d6d 7994 7d94 8c0d 6861 6d6d  ..dummy.}...hamm
+00000b10: 696e 672d 6475 6d6d 7994 7d94 8c07 756e  ing-dummy.}...un
+00000b20: 642d 6970 6194 7d94 7568 a07d 9428 8c0f  d-ipa.}.uh.}.(..
+00000b30: 6861 6d6d 696e 672d 656e 672d 6970 6194  hamming-eng-ipa.
+00000b40: 7d94 8c07 656e 672d 6970 6194 7d94 7568  }...eng-ipa.}.uh
+00000b50: a27d 948c 0765 6e67 2d69 7061 947d 9473  .}...eng-ipa.}.s
+00000b60: 68a4 7d94 8c07 656e 672d 6970 6194 7d94  h.}...eng-ipa.}.
+00000b70: 7368 a67d 948c 0765 6e67 2d69 7061 947d  sh.}...eng-ipa.}
+00000b80: 9473 68a8 7d94 2868 aa7d 9468 ac7d 9468  .sh.}.(h.}.h.}.h
+00000b90: ae7d 9475 68aa 7d94 8c07 656e 672d 6970  .}.uh.}...eng-ip
+00000ba0: 6194 7d94 7368 ac7d 9468 ae7d 9468 b07d  a.}.sh.}.h.}.h.}
+00000bb0: 948c 0767 6c61 2d69 7061 947d 9473 68b2  ...gla-ipa.}.sh.
+00000bc0: 7d94 68b4 7d94 7368 b47d 948c 0767 7769  }.h.}.sh.}...gwi
+00000bd0: 2d69 7061 947d 9473 68b6 7d94 68b8 7d94  -ipa.}.sh.}.h.}.
+00000be0: 7368 b87d 948c 0768 6161 2d69 7061 947d  sh.}...haa-ipa.}
+00000bf0: 9473 68ba 7d94 8c07 696b 742d 6970 6194  .sh.}...ikt-ipa.
+00000c00: 7d94 7368 bc7d 9468 be7d 9473 68be 7d94  }.sh.}.h.}.sh.}.
+00000c10: 8c07 696b 752d 6970 6194 7d94 7368 c07d  ..iku-ipa.}.sh.}
+00000c20: 948c 0b69 6b75 2d73 726f 2d69 7061 947d  ...iku-sro-ipa.}
+00000c30: 9473 68c2 7d94 68c4 7d94 7368 c47d 948c  .sh.}.h.}.sh.}..
+00000c40: 0765 6e67 2d69 7061 947d 9473 68c6 7d94  .eng-ipa.}.sh.}.
+00000c50: 8c07 656e 672d 6970 6194 7d94 7368 c87d  ..eng-ipa.}.sh.}
+00000c60: 948c 076b 776b 2d69 7061 947d 9473 68ca  ...kwk-ipa.}.sh.
+00000c70: 7d94 288c 076b 776b 2d69 7061 947d 9468  }.(..kwk-ipa.}.h
+00000c80: cc7d 9475 68cc 7d94 68ce 7d94 68d0 7d94  .}.uh.}.h.}.h.}.
+00000c90: 7368 d07d 9468 d27d 9468 d47d 9473 68d4  sh.}.h.}.h.}.sh.
+00000ca0: 7d94 68d6 7d94 8c0a 6b77 6b2d 756d 6973  }.h.}...kwk-umis
+00000cb0: 7461 947d 9473 68d8 7d94 8c07 6c6d 6c2d  ta.}.sh.}...lml-
+00000cc0: 6970 6194 7d94 7368 da7d 948c 076d 6963  ipa.}.sh.}...mic
+00000cd0: 2d69 7061 947d 9473 68dc 7d94 8c07 6d6f  -ipa.}.sh.}...mo
+00000ce0: 652d 6970 6194 7d94 7368 de7d 948c 096d  e-ipa.}.sh.}...m
+00000cf0: 6f68 2d65 7175 6976 947d 9473 68e0 7d94  oh-equiv.}.sh.}.
+00000d00: 8c07 6d6f 682d 6970 6194 7d94 7368 e27d  ..moh-ipa.}.sh.}
+00000d10: 948c 0369 7061 947d 9473 68e4 7d94 8c07  ...ipa.}.sh.}...
+00000d20: 6f6a 692d 6970 6194 7d94 7368 e67d 948c  oji-ipa.}.sh.}..
+00000d30: 036f 6a69 947d 9473 68e8 7d94 8c07 6f6b  .oji.}.sh.}...ok
+00000d40: 612d 6970 6194 7d94 7368 ea7d 948c 096f  a-ipa.}.sh.}...o
+00000d50: 6b61 2d65 7175 6976 947d 9473 68ec 7d94  ka-equiv.}.sh.}.
+00000d60: 8c07 7365 652d 6970 6194 7d94 7368 ee7d  ..see-ipa.}.sh.}
+00000d70: 9468 f07d 9473 68f0 7d94 8c07 656e 672d  .h.}.sh.}...eng-
+00000d80: 6970 6194 7d94 7368 f27d 948c 0973 7472  ipa.}.sh.}...str
+00000d90: 2d65 7175 6976 947d 9473 68f4 7d94 68f6  -equiv.}.sh.}.h.
+00000da0: 7d94 7368 f67d 948c 0774 6175 2d69 7061  }.sh.}...tau-ipa
+00000db0: 947d 9473 68f8 7d94 68fa 7d94 7368 fa7d  .}.sh.}.h.}.sh.}
+00000dc0: 948c 0774 6365 2d69 7061 947d 9473 68fc  ...tce-ipa.}.sh.
+00000dd0: 7d94 68fe 7d94 7368 fe7d 948c 0765 6e67  }.h.}.sh.}...eng
+00000de0: 2d69 7061 947d 9473 6a00 0100 007d 946a  -ipa.}.sj....}.j
+00000df0: 0201 0000 7d94 736a 0201 0000 7d94 8c07  ....}.sj....}...
+00000e00: 746c 692d 6970 6194 7d94 736a 0401 0000  tli-ipa.}.sj....
+00000e10: 7d94 6a06 0100 007d 9473 6a06 0100 007d  }.j....}.sj....}
+00000e20: 948c 0774 746d 2d69 7061 947d 9473 6a08  ...ttm-ipa.}.sj.
+00000e30: 0100 007d 948c 0975 6e64 2d61 7363 6969  ...}...und-ascii
+00000e40: 947d 9473 6a0a 0100 007d 948c 0777 696e  .}.sj....}...win
+00000e50: 2d69 7061 947d 9473 758c 055f 7072 6564  -ipa.}.su.._pred
+00000e60: 947d 9428 6812 7d94 6814 7d94 6812 6a0f  .}.(h.}.h.}.h.j.
+00000e70: 0100 0073 6816 7d94 6818 7d94 6816 6a14  ...sh.}.h.}.h.j.
+00000e80: 0100 0073 681a 7d94 288c 0761 746a 2d69  ...sh.}.(..atj-i
+00000e90: 7061 946a 1601 0000 8c07 636b 742d 6970  pa.j......ckt-ip
+00000ea0: 6194 6a1d 0100 008c 0763 726a 2d69 7061  a.j......crj-ipa
+00000eb0: 946a 2f01 0000 8c07 6372 6c2d 6970 6194  .j/.....crl-ipa.
+00000ec0: 6a3e 0100 008c 0763 726d 2d69 7061 946a  j>.....crm-ipa.j
+00000ed0: 4501 0000 8c07 6373 772d 6970 6194 6a51  E.....csw-ipa.jQ
+00000ee0: 0100 008c 0763 7470 2d69 7061 946a 5601  .....ctp-ipa.jV.
+00000ef0: 0000 6862 6a68 0100 008c 0764 616e 2d69  ..hbjh.....dan-i
+00000f00: 7061 946a 5b01 0000 8c07 6672 612d 6970  pa.j[.....fra-ip
+00000f10: 6194 6a7e 0100 0068 7a6a 8101 0000 8c07  a.j~...hzj......
+00000f20: 616c 712d 6970 6194 6a12 0100 0068 7c6a  alq-ipa.j....h|j
+00000f30: 8601 0000 687e 6a89 0100 0068 806a 8c01  ....h~j....h.j..
+00000f40: 0000 6882 6a8f 0100 008c 0763 726b 2d69  ..h.j......crk-i
+00000f50: 7061 946a 3401 0000 6884 6a92 0100 008c  pa.j4...h.j.....
+00000f60: 0763 7267 2d69 7061 946a 2501 0000 6886  .crg-ipa.j%...h.
+00000f70: 6a95 0100 0068 886a 9801 0000 688a 6a9b  j....h.j....h.j.
+00000f80: 0100 0068 8c6a 9e01 0000 688e 6aa3 0100  ...h.j....h.j...
+00000f90: 0068 906a a801 0000 6892 6aab 0100 0068  .h.j....h.j....h
+00000fa0: 946a ae01 0000 6896 6ab1 0100 0068 986a  .j....h.j....h.j
+00000fb0: b401 0000 68a2 6ad5 0100 0068 a46a d801  ....h.j....h.j..
+00000fc0: 0000 8c07 6669 6e2d 6970 6194 6a6d 0100  ....fin-ipa.jm..
+00000fd0: 0068 a66a db01 0000 8c07 6769 742d 6970  .h.j......git-ip
+00000fe0: 6194 6ae2 0100 008c 076b 6b7a 2d69 7061  a.j......kkz-ipa
+00000ff0: 946a 0102 0000 68c6 6a04 0200 008c 0773  .j....h.j......s
+00001000: 7273 2d69 7061 946a 3b02 0000 8c07 7467  rs-ipa.j;.....tg
+00001010: 782d 6970 6194 6a4d 0200 008c 0775 6e64  x-ipa.jM.....und
+00001020: 2d69 7061 946a d201 0000 7568 1c7d 9468  -ipa.j....uh.}.h
+00001030: 1e7d 9468 1c6a 1a01 0000 7368 207d 9468  .}.h.j....sh }.h
+00001040: 227d 9468 206a 1f01 0000 7368 247d 9468  "}.h j....sh$}.h
+00001050: 267d 9428 6824 6a22 0100 0068 286a 2801  &}.(h$j"...h(j(.
+00001060: 0000 7568 287d 9468 2a7d 9468 2c7d 9468  ..uh(}.h*}.h,}.h
+00001070: 2a6a 2a01 0000 7368 2e7d 948c 0963 726a  *j*...sh.}...crj
+00001080: 2d65 7175 6976 946a 2c01 0000 7368 307d  -equiv.j,...sh0}
+00001090: 9468 346a 3701 0000 7368 327d 9468 306a  .h4j7...sh2}.h0j
+000010a0: 3101 0000 7368 347d 9468 367d 9468 387d  1...sh4}.h6}.h8}
+000010b0: 9468 366a 3901 0000 7368 3a7d 948c 0963  .h6j9...sh:}...c
+000010c0: 726c 2d65 7175 6976 946a 3b01 0000 7368  rl-equiv.j;...sh
+000010d0: 3c7d 9468 3e7d 9468 3c6a 4001 0000 7368  <}.h>}.h<j@...sh
+000010e0: 407d 948c 0963 726d 2d65 7175 6976 946a  @}...crm-equiv.j
+000010f0: 4201 0000 7368 427d 948c 0763 7278 2d73  B...shB}...crx-s
+00001100: 796c 946a 4a01 0000 7368 447d 9468 426a  yl.jJ...shD}.hBj
+00001110: 4701 0000 7368 467d 9468 487d 9468 466a  G...shF}.hH}.hFj
+00001120: 4c01 0000 7368 4a7d 948c 0963 7377 2d65  L...shJ}...csw-e
+00001130: 7175 6976 946a 4e01 0000 7368 4c7d 9468  quiv.jN...shL}.h
+00001140: 4e7d 9468 4c6a 5301 0000 7368 507d 9468  N}.hLjS...shP}.h
+00001150: 527d 9468 506a 5801 0000 7368 547d 9428  R}.hPjX...shT}.(
+00001160: 689a 6abb 0100 0068 9c6a c201 0000 689e  h.j....h.j....h.
+00001170: 6ac9 0100 0075 6856 7d94 6854 6a5d 0100  j....uhV}.hTj]..
+00001180: 0073 6858 7d94 288c 096d 6f68 2d65 7175  .shX}.(..moh-equ
+00001190: 6976 946a bd01 0000 8c09 7374 722d 6571  iv.j......str-eq
+000011a0: 7569 7694 6ac4 0100 008c 0975 6e64 2d61  uiv.j......und-a
+000011b0: 7363 6969 946a cb01 0000 7568 5a7d 9468  scii.j....uhZ}.h
+000011c0: 586a 6001 0000 7368 5c7d 948c 0765 6e67  Xj`...sh\}...eng
+000011d0: 2d69 7061 946a 1801 0000 7368 5e7d 9428  -ipa.j....sh^}.(
+000011e0: 8c07 7374 722d 6970 6194 6a83 0100 008c  ..str-ipa.j.....
+000011f0: 076d 6f68 2d69 7061 946a b601 0000 8c07  .moh-ipa.j......
+00001200: 696b 752d 6970 6194 6aa0 0100 0068 a06a  iku-ipa.j....h.j
+00001210: d001 0000 8c07 696b 742d 6970 6194 6aa5  ......ikt-ipa.j.
+00001220: 0100 0075 6860 7d94 685e 6a64 0100 0073  ...uh`}.h^jd...s
+00001230: 6862 7d94 6864 7d94 6866 7d94 6864 6a6a  hb}.hd}.hf}.hdjj
+00001240: 0100 0073 6868 7d94 686a 7d94 2868 686a  ...shh}.hj}.(hhj
+00001250: 6f01 0000 686c 6a73 0100 0075 686c 7d94  o...hljs...uhl}.
+00001260: 686e 7d94 6870 7d94 686e 6a75 0100 0073  hn}.hp}.hnju...s
+00001270: 6872 7d94 6874 7d94 6872 6a78 0100 0073  hr}.ht}.hrjx...s
+00001280: 6876 7d94 6878 7d94 6876 6a7b 0100 0073  hv}.hx}.hvj{...s
+00001290: 687a 7d94 8c09 7374 722d 6571 7569 7694  hz}...str-equiv.
+000012a0: 6ac6 0100 0073 687c 7d94 68ec 6a36 0200  j....sh|}.h.j6..
+000012b0: 0073 687e 7d94 68d8 6a18 0200 0073 6880  .sh~}.h.j....sh.
+000012c0: 7d94 68e4 6a2a 0200 0073 6882 7d94 68b0  }.h.j*...sh.}.h.
+000012d0: 6ae7 0100 0073 6884 7d94 8c09 7463 652d  j....sh.}...tce-
+000012e0: 6571 7569 7694 6a48 0200 0073 6886 7d94  equiv.jH...sh.}.
+000012f0: 8c09 746c 692d 6571 7569 7694 6a52 0200  ..tli-equiv.jR..
+00001300: 0073 6888 7d94 8c09 6777 692d 6571 7569  .sh.}...gwi-equi
+00001310: 7694 6aec 0100 0073 688a 7d94 68da 6a1b  v.j....sh.}.h.j.
+00001320: 0200 0073 688c 7d94 8c09 696b 752d 6571  ...sh.}...iku-eq
+00001330: 7569 7694 6af9 0100 0073 688e 7d94 68ba  uiv.j....sh.}.h.
+00001340: 6af4 0100 0073 6890 7d94 68c0 6afc 0100  j....sh.}.h.j...
+00001350: 0073 6892 7d94 8c09 6861 612d 6571 7569  .sh.}...haa-equi
+00001360: 7694 6af1 0100 0073 6894 7d94 8c09 7474  v.j....sh.}...tt
+00001370: 6d2d 6571 7569 7694 6a57 0200 0073 6896  m-equiv.jW...sh.
+00001380: 7d94 8c09 7461 752d 6571 7569 7694 6a43  }...tau-equiv.jC
+00001390: 0200 0073 6898 7d94 288c 096d 6f68 2d65  ...sh.}.(..moh-e
+000013a0: 7175 6976 946a bf01 0000 8c0c 6d6f 682d  quiv.j......moh-
+000013b0: 6665 7374 6976 616c 946a 2402 0000 7568  festival.j$...uh
+000013c0: 9a7d 948c 036d 6f68 946a 2102 0000 7368  .}...moh.j!...sh
+000013d0: 9c7d 9468 f26a 3e02 0000 7368 9e7d 946a  .}.h.j>...sh.}.j
+000013e0: 0801 0000 6a5a 0200 0073 68a0 7d94 8c09  ....jZ...sh.}...
+000013f0: 756e 642d 6173 6369 6994 6acd 0100 0073  und-ascii.j....s
+00001400: 68a2 7d94 68dc 6a1e 0200 0073 68a4 7d94  h.}.h.j....sh.}.
+00001410: 6a0a 0100 006a 5d02 0000 7368 a67d 9468  j....j]...sh.}.h
+00001420: e86a 3002 0000 7368 a87d 9468 aa7d 9468  .j0...sh.}.h.}.h
+00001430: a86a dd01 0000 7368 ac7d 948c 0367 6974  .j....sh.}...git
+00001440: 946a de01 0000 7368 ae7d 948c 0367 6974  .j....sh.}...git
+00001450: 946a df01 0000 7368 b07d 9468 b27d 9468  .j....sh.}.h.}.h
+00001460: b47d 9468 b26a e901 0000 7368 b67d 9468  .}.h.j....sh.}.h
+00001470: b87d 9468 b66a ee01 0000 7368 ba7d 9468  .}.h.j....sh.}.h
+00001480: bc7d 9468 be7d 9468 bc6a f601 0000 7368  .}.h.}.h.j....sh
+00001490: c07d 9468 c27d 9468 c47d 9468 c26a fe01  .}.h.}.h.}.h.j..
+000014a0: 0000 7368 c67d 9428 68c8 6a07 0200 0068  ..sh.}.(h.j....h
+000014b0: ca6a 0a02 0000 7568 c87d 9468 ca7d 9468  .j....uh.}.h.}.h
+000014c0: d66a 1502 0000 7368 cc7d 948c 0a6b 776b  .j....sh.}...kwk
+000014d0: 2d75 6d69 7374 6194 6a0b 0200 0073 68ce  -umista.j....sh.
+000014e0: 7d94 68d0 7d94 68ce 6a0e 0200 0073 68d2  }.h.}.h.j....sh.
+000014f0: 7d94 68d4 7d94 68d2 6a11 0200 0073 68d6  }.h.}.h.j....sh.
+00001500: 7d94 68d8 7d94 68da 7d94 68dc 7d94 68de  }.h.}.h.}.h.}.h.
+00001510: 7d94 8c07 6d6f 682d 6970 6194 6ab7 0100  }...moh-ipa.j...
+00001520: 0073 68e0 7d94 8c07 6d6f 682d 6970 6194  .sh.}...moh-ipa.
+00001530: 6ab8 0100 0073 68e2 7d94 68e2 6a27 0200  j....sh.}.h.j'..
+00001540: 0073 68e4 7d94 68e6 6a2d 0200 0073 68e6  .sh.}.h.j-...sh.
+00001550: 7d94 68e8 7d94 68ea 6a33 0200 0073 68ea  }.h.}.h.j3...sh.
+00001560: 7d94 68ec 7d94 68ee 7d94 68f0 7d94 68ee  }.h.}.h.}.h.}.h.
+00001570: 6a38 0200 0073 68f2 7d94 68f4 7d94 68f6  j8...sh.}.h.}.h.
+00001580: 7d94 68f4 6a40 0200 0073 68f8 7d94 68fa  }.h.j@...sh.}.h.
+00001590: 7d94 68f8 6a45 0200 0073 68fc 7d94 68fe  }.h.jE...sh.}.h.
+000015a0: 7d94 68fc 6a4a 0200 0073 6a00 0100 007d  }.h.jJ...sj....}
+000015b0: 946a 0201 0000 7d94 6a00 0100 006a 4f02  .j....}.j....jO.
+000015c0: 0000 736a 0401 0000 7d94 6a06 0100 007d  ..sj....}.j....}
+000015d0: 946a 0401 0000 6a54 0200 0073 6a08 0100  .j....jT...sj...
+000015e0: 007d 946a 0a01 0000 7d94 758c 055f 7375  .}.j....}.u.._su
+000015f0: 6363 946a 0d01 0000 7562 2e              cc.j....ub.
```

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/norm/tone-map.txt` & `g2p-1.0.20230412/g2p/mappings/langs/norm/tone-map.txt`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/oji/config.yaml` & `g2p-1.0.20230412/g2p/mappings/langs/oji/config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -20,8 +20,8 @@
       - Shankhalika Srikanth
     type: mapping
     mapping: oji_syllabics_to_orth.csv
     prevent_feeding: true
     rule_ordering: as-written
     case_sensitive: false
     norm_form: NFC
-    <<: *shared
+    language_name: Ojibwe Syllabics
```

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/oji/oji_syllabics_to_orth.csv` & `g2p-1.0.20230412/g2p/mappings/langs/oji/oji_syllabics_to_orth.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/srs/config.yaml` & `g2p-1.0.20230412/g2p/mappings/langs/srs/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/srs/srs_ipa_to_eng_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/srs/srs_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/srs/srs_to_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/srs/srs_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/str/config.yaml` & `g2p-1.0.20230412/g2p/mappings/langs/str/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/str/str_equiv.json` & `g2p-1.0.20230412/g2p/mappings/langs/str/str_equiv.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/str/str_to_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/str/str_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/tau/config.yml` & `g2p-1.0.20230412/g2p/mappings/langs/tau/config.yml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/tau/tau_to_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/tau/tau_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/tce/config.yaml` & `g2p-1.0.20230412/g2p/mappings/langs/tce/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/tce/tce_to_ipa.csv` & `g2p-1.0.20230412/g2p/mappings/langs/tce/tce_to_ipa.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/tgx/config.yml` & `g2p-1.0.20230412/g2p/mappings/langs/tgx/config.yml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/tgx/tgx_ipa_to_eng_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/tgx/tgx_ipa_to_eng_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/tgx/tgx_to_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/tgx/tgx_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/tli/config.yaml` & `g2p-1.0.20230412/g2p/mappings/langs/tli/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/tli/tli_to_ipa.csv` & `g2p-1.0.20230412/g2p/mappings/langs/tli/tli_to_ipa.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/ttm/config.yaml` & `g2p-1.0.20230412/g2p/mappings/langs/ttm/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/und/config.yaml` & `g2p-1.0.20230412/g2p/mappings/langs/und/config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     mapping: und_ipa_to_eng_ipa.json
     in_lang: und-ipa
     out_lang: hamming-eng-ipa
     rule_ordering: apply-longest-first
     authors:
       - Patrick Littell
     <<: *shared
-  - display_name: Undertermined Unicode to ASCII
+  - display_name: Undetermined Unicode to ASCII
     type: unidecode
     norm: NFD
     in_lang: und
     out_lang: und-ascii
     authors:
       - Eric Joanis
     <<: *shared
```

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/und/und_ipa_to_eng_ipa.json` & `g2p-1.0.20230412/g2p/tests/public/git_to_ipa.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('type', 'mapping'), ('authors', ['Aidan Pine']), ('created', "*

 * *            "'2019-06-23'), ('last_modified', '2019-06-23'), ('in_metadata', "*

 * *            "OrderedDict([('display_name', 'Gitksan'), ('display', True), ('lang', 'git'), "*

 * *            "('format', 'custom'), ('delimiter', ''), ('case_insensitive', True)])), "*

 * *            "('out_metadata', OrderedDict([('lang', 'git-ipa'), ('format', 'ipa'), ('delimiter', "*

 * *            "'')])), ('map', [OrderedDict([('in', 'a'), ('out',  […]*

```diff
@@ -1,114 +1,160 @@
-[
-    {
-        "in": "a",
-        "out": "\u0251"
+{
+    "authors": [
+        "Aidan Pine"
+    ],
+    "comments": [],
+    "created": "2019-06-23",
+    "in_metadata": {
+        "case_insensitive": true,
+        "delimiter": "",
+        "display": true,
+        "display_name": "Gitksan",
+        "format": "custom",
+        "lang": "git"
+    },
+    "last_modified": "2019-06-23",
+    "map": [
+        {
+            "in": "a",
+            "out": "\u00e6"
+        },
+        {
+            "in": "aa",
+            "out": "a\u02d0"
+        },
+        {
+            "in": "ee",
+            "out": "e\u02d0"
+        },
+        {
+            "in": "p",
+            "out": "b"
+        },
+        {
+            "in": "t",
+            "out": "d"
+        },
+        {
+            "in": "kw",
+            "out": "k\u02b7"
+        },
+        {
+            "in": "s",
+            "out": "s"
+        },
+        {
+            "in": "k",
+            "out": "k"
+        },
+        {
+            "in": "g",
+            "out": "\u025f"
+        },
+        {
+            "in": "gy",
+            "out": "\u025f"
+        },
+        {
+            "in": "gw",
+            "out": "\u0261\u02b7"
+        },
+        {
+            "in": "d",
+            "out": "d"
+        },
+        {
+            "in": "b",
+            "out": "b"
+        },
+        {
+            "in": "l",
+            "out": "l"
+        },
+        {
+            "in": "r",
+            "out": "l"
+        },
+        {
+            "in": "m",
+            "out": "m"
+        },
+        {
+            "in": "n",
+            "out": "n"
+        },
+        {
+            "in": "x",
+            "out": "x"
+        },
+        {
+            "in": "w",
+            "out": "w"
+        },
+        {
+            "in": "o",
+            "out": "\u0254"
+        },
+        {
+            "in": "oo",
+            "out": "o\u02d0"
+        },
+        {
+            "in": "u",
+            "out": "u"
+        },
+        {
+            "in": "'",
+            "out": "\u0294"
+        },
+        {
+            "in": "y",
+            "out": "j"
+        },
+        {
+            "in": "k\u0332",
+            "out": "q"
+        },
+        {
+            "in": "ts",
+            "out": "t\u0361s"
+        },
+        {
+            "in": "g\u0332",
+            "out": "\u0281"
+        },
+        {
+            "in": "hl",
+            "out": "\u026c"
+        },
+        {
+            "in": "j",
+            "out": "d\u0361\u0292"
+        },
+        {
+            "in": "x\u0332",
+            "out": "\u03c7"
+        },
+        {
+            "in": "xw",
+            "out": "x\u02b7"
+        },
+        {
+            "in": "e",
+            "out": "i"
+        },
+        {
+            "in": "uu",
+            "out": "u\u02d0"
+        },
+        {
+            "in": "ii",
+            "out": "i\u02d0"
+        }
+    ],
+    "out_metadata": {
+        "delimiter": "",
+        "format": "ipa",
+        "lang": "git-ipa"
     },
-    {
-        "in": "b",
-        "out": "b"
-    },
-    {
-        "in": "d",
-        "out": "d"
-    },
-    {
-        "in": "e",
-        "out": "e\u02d0"
-    },
-    {
-        "in": "f",
-        "out": "f"
-    },
-    {
-        "in": "h",
-        "out": "h"
-    },
-    {
-        "in": "i",
-        "out": "i"
-    },
-    {
-        "in": "j",
-        "out": "j"
-    },
-    {
-        "in": "k",
-        "out": "k"
-    },
-    {
-        "in": "l",
-        "out": "l"
-    },
-    {
-        "in": "m",
-        "out": "m"
-    },
-    {
-        "in": "n",
-        "out": "n"
-    },
-    {
-        "in": "o",
-        "out": "o\u02d0"
-    },
-    {
-        "in": "p",
-        "out": "p"
-    },
-    {
-        "in": "q",
-        "out": "k"
-    },
-    {
-        "in": "r",
-        "out": "\u027e"
-    },
-    {
-        "in": "s",
-        "out": "s"
-    },
-    {
-        "in": "t",
-        "out": "t"
-    },
-    {
-        "in": "t\u0361s",
-        "out": "ts"
-    },
-    {
-        "in": "u",
-        "out": "u"
-    },
-    {
-        "in": "v",
-        "out": "v"
-    },
-    {
-        "in": "w",
-        "out": "w"
-    },
-    {
-        "in": "x",
-        "out": "k"
-    },
-    {
-        "in": "z",
-        "out": "z"
-    },
-    {
-        "in": "\u0259",
-        "out": "\u0259"
-    },
-    {
-        "in": "\u0261",
-        "out": "\u0261"
-    },
-    {
-        "in": "\u0292",
-        "out": "\u0292"
-    },
-    {
-        "in": "\u0294",
-        "out": "\u0294"
-    }
-]
+    "type": "mapping"
+}
```

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/und/und_to_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/und/und_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/utils.py` & `g2p-1.0.20230412/g2p/mappings/langs/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """
 
 Utilities used by other classes
 
 """
 
+import json
 import pickle
 from pathlib import Path
 
 import yaml
 from networkx import DiGraph, write_gpickle
+from networkx.algorithms.dag import ancestors, descendants
 
 from g2p.exceptions import MalformedMapping
 from g2p.log import LOGGER
 from g2p.mappings import Mapping
 from g2p.mappings.langs import (
     LANGS_DIR,
+    LANGS_NETWORK,
     LANGS_NWORK_PATH,
     LANGS_PKL,
     MAPPINGS_AVAILABLE,
 )
 from g2p.mappings.utils import is_ipa, load_mapping_from_path
 
 # panphon.distance.Distance() takes a long time to initialize, so...
@@ -51,15 +54,15 @@
         mappings_to_check = [x["out_lang"] for x in MAPPINGS_AVAILABLE]
     found_error = False
     for mapping in [
         x for x in MAPPINGS_AVAILABLE if x["out_lang"] in mappings_to_check
     ]:
         if is_ipa(mapping["out_lang"]):
             reverse = mapping.get("reverse", False)
-            for rule in mapping["mapping_data"]:
+            for rule in mapping.get("mapping_data", ()):
                 output = rule["in"] if reverse else rule["out"]
                 if not is_panphon(output):
                     LOGGER.warning(
                         f"Output '{rule['out']}' in rule {rule} in mapping between {mapping['in_lang']} "
                         f"and {mapping['out_lang']} is not recognized as valid IPA by panphon."
                     )
                     found_error = True
@@ -184,7 +187,38 @@
     with open(network_path, "wb") as f:
         write_gpickle(lang_network, f, protocol=4)
 
     with open(langs_path, "wb") as f:
         pickle.dump(langs, f, protocol=4)
 
     return langs
+
+
+def network_to_echart(outfile: str = None, layout: bool = False):
+    nodes = []
+    no_nodes = len(LANGS_NETWORK.nodes)
+    for node in LANGS_NETWORK.nodes:
+        lang_name = node.split("-")[0]
+        no_ancestors = len(ancestors(LANGS_NETWORK, node))
+        no_descendants = len(descendants(LANGS_NETWORK, node))
+        size = min(
+            20,
+            max(
+                2, ((no_ancestors / no_nodes) * 100 + (no_descendants / no_nodes) * 100)
+            ),
+        )
+        node = {"name": node, "symbolSize": size, "id": node, "category": lang_name}
+        nodes.append(node)
+    nodes.sort(key=lambda x: x["name"])
+    edges = []
+    for edge in LANGS_NETWORK.edges:
+        edges.append({"source": edge[0], "target": edge[1]})
+    if outfile:
+        with open(
+            outfile,
+            "w",
+            encoding="utf-8",
+            newline="\n",
+        ) as f:
+            f.write(json.dumps({"nodes": nodes, "edges": edges}) + "\n")
+        LOGGER.info("Wrote network nodes and edges to static file.")
+    return nodes, edges
```

### Comparing `g2p-1.0.20230228/g2p/mappings/langs/win/win_to_ipa.json` & `g2p-1.0.20230412/g2p/mappings/langs/win/win_to_ipa.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/tokenizer.py` & `g2p-1.0.20230412/g2p/mappings/tokenizer.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/mappings/utils.py` & `g2p-1.0.20230412/g2p/mappings/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import csv
 import json
 import os
 import unicodedata as ud
 from collections import defaultdict
 from copy import deepcopy
 from pathlib import Path
-from typing import Dict, List, Tuple
+from typing import Dict, List, Tuple, TypeVar, Union
 
 import regex as re
 import yaml
 
 from g2p import exceptions
 from g2p.log import LOGGER
 from g2p.mappings import langs
@@ -88,17 +88,23 @@
                 inp,
                 normalized,
                 norm_form,
             )
         return normalized
 
 
+# compose_indices is generic because we would like to propagate the
+# type of its second input, in the case where we *know* there will not
+# be None (NFC and NFD conversions)
+IntOrOptionalInt = TypeVar("IntOrOptionalInt", bound=Union[int, None])
+
+
 def compose_indices(
-    indices1: List[Tuple[int, int]], indices2: List[Tuple[int, int]]
-) -> List[Tuple[int, int]]:
+    indices1: List[Tuple[int, int]], indices2: List[Tuple[int, IntOrOptionalInt]]
+) -> List[Tuple[int, IntOrOptionalInt]]:
     """Compose indices1 + indices2 into direct arcs from the inputs of indices1
     to the outputs of indices 2.
 
     E.g., [(0,1), (1,4)] composed with [(0,0), (1,2), (1,3), (4,2)] is
     [(0,2), (0,3), (1,2)]
     """
     # for O(1) lookup of arcs leaving indices2
@@ -303,15 +309,15 @@
     else:
         raise exceptions.IncorrectFileType(
             f"File {path} is not a valid mapping filetype."
         )
     return validate(mapping, path)
 
 
-def load_mapping_from_path(path_to_mapping_config, index=0):
+def load_mapping_from_path(path_to_mapping_config, index=0):  # noqa: C901
     """Loads a mapping from a path, if there is more than one mapping, then it loads based on the int
     provided to the 'index' argument. Default is 0.
     """
     path = Path(path_to_mapping_config)
     # If path leads to actual mapping config
     if path.exists() and (path.suffix.endswith("yml") or path.suffix.endswith("yaml")):
         # safe load it
@@ -352,14 +358,25 @@
             except (OSError, exceptions.IncorrectFileType) as e:
                 raise exceptions.MalformedMapping(
                     f"Cannot load mapping data file specified in {path}: {e}"
                 ) from e
         elif mapping.get("type", "") == "unidecode":
             # This mapping is not implemented as a regular mapping, but as custom software
             pass
+        elif mapping.get("type", "") == "lexicon":
+            # This mapping has a file of alignments
+            try:
+                mapping["alignment_data"] = load_alignments_from_file(
+                    os.path.join(path.parent, mapping["alignments"]),
+                    mapping.get("out_delimiter", ""),
+                )
+            except OSError as e:
+                raise exceptions.MalformedMapping(
+                    f"Cannot load alignment data file specified in {path}: {e}"
+                ) from e
         else:
             # Is "mapping" key missing?
             raise exceptions.MalformedMapping(
                 'Key "mapping:" missing from a mapping in {}.'.format(path)
             )
         # load any abbreviations
         if "abbreviations" in mapping:
@@ -378,15 +395,19 @@
 
 def find_mapping(in_lang: str, out_lang: str) -> list:
     """Given an input and output, find a mapping to get between them."""
     for mapping in langs.MAPPINGS_AVAILABLE:
         map_in_lang = mapping.get("in_lang", "")
         map_out_lang = mapping.get("out_lang", "")
         if map_in_lang == in_lang and map_out_lang == out_lang:
-            return deepcopy(mapping)
+            if mapping.get("type") == "lexicon":
+                # do *not* deep copy this, because alignments are big!
+                return mapping.copy()
+            else:
+                return deepcopy(mapping)
     raise exceptions.MappingMissing(in_lang, out_lang)
 
 
 def validate(mapping, path):
     try:
         for io in mapping:
             if "context_before" not in io:
@@ -442,14 +463,48 @@
     else:
         raise exceptions.IncorrectFileType(
             f"Sorry, abbreviations must be stored as CSV/TSV/PSV files. You provided the following: {path}"
         )
     return abbs
 
 
+def load_alignments_from_file(path, delimiter="") -> Dict[str, Tuple]:
+    """Load alignments in Phonetisaurus default format.
+
+    Returns a mapping of input words to output alignments used to
+    create a lexicon mapping.  These are of the form (length,
+    outputs, length, outputs, ...) - that is, a sequence of pairs
+    specifying how much of the input to consume and what it maps
+    to.  This particular format is used to avoid redundancy with
+    the keys in the dictionary.
+    """
+    LOGGER.info("Loading alignments from %s", path)
+    alignments = {}
+    with open(path, encoding="utf8") as f:
+        for spam in f:
+            spam = spam.strip()
+            if not spam:
+                continue
+            chars = ""
+            mappings: List[Union[int, str]] = []
+            for mapping in spam.split():
+                idx = mapping.rindex("}")
+                # Note that we care about *character* indices, so we join them together
+                in_seq = "".join(tok for tok in mapping[:idx].split("|") if tok != "_")
+                out_seq = delimiter.join(
+                    tok for tok in mapping[idx + 1 :].split("|") if tok != "_"
+                )
+                chars += in_seq
+                # To save space, make the mappings flat and only store
+                # the number of input characters rather than the characters themselves
+                mappings.extend((len(in_seq), out_seq))
+            alignments["".join(chars)] = tuple(mappings)
+    return alignments
+
+
 def is_ipa(lang: str) -> bool:
     pattern = re.compile("[-_]?ipa$")
     return bool(re.search(pattern, lang))
 
 
 def is_xsampa(lang: str) -> bool:
     pattern = re.compile("[-_]?x(-?)sampa$")
```

### Comparing `g2p-1.0.20230228/g2p/static/blockly_main.js` & `g2p-1.0.20230412/g2p/static/blockly_main.js`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/static/blocks.js` & `g2p-1.0.20230412/g2p/static/blocks.js`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/static/custom.css` & `g2p-1.0.20230412/g2p/static/custom.css`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/static/custom.js` & `g2p-1.0.20230412/g2p/static/custom.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -67,14 +67,16 @@
     let escape_special = '';
     let reverse = '';
     let active = '';
     let out_delimiter = '';
     let prevent_feeding = '';
     let norm_form = 'NFC';
     let type = 'mapping';
+    let in_lang = '';
+    let out_lang = '';
     if (index === 0) {
         active = 'active'
     }
     if ('include' in data && data['include']) {
         include = 'checked'
     }
     if (data['rule_ordering'] === 'as-written') {
@@ -100,14 +102,19 @@
     }
     if (data['norm_form']) {
         norm_form = data['norm_form']
     }
     if (data['type']) {
         type = data['type']
     }
+    // For lexicon mappings, we can only use the built-in mapping
+    if (type == ['lexicon']) {
+        in_lang = data['in_lang']
+        out_lang = data['out_lang']
+    }
     let settings_template = `
     <div class='${active} settings'>
         <form>
             <fieldset>
                 <div></div>
                 <div>
                     <input ${include} class='include' id='include-${index}' type='checkbox' name='include' value='include'>
@@ -143,14 +150,16 @@
                     <input id='norm_form-${index}' type='text' name='norm_form' value='${norm_form}' maxlength='4' minlength='3'>
                 </div>
                 <div>
                     <label for='out_delimiter'>Output Delimiter</label>
                     <input id='out_delimiter-${index}' type='text' name='out_delimiter' value='${out_delimiter}' placeholder='delimiter' maxlength='1'>
                 </div>
                 <input id='type-${index}' type='hidden' name='type' value='${type}' maxlength='20' minlength='0'>
+                <input id='in_lang-${index}' type='hidden' name='in_lang' value='${in_lang}' maxlength='20' minlength='0'>
+                <input id='out_lang-${index}' type='hidden' name='out_lang' value='${out_lang}' maxlength='20' minlength='0'>
             </fieldset>
         </form>
     </div>`
     $('#settings-container').append(settings_template)
     document.getElementById(`include-${index}`).addEventListener('click', function(event) {
         const include = event.target.checked
         setKwargs(index, {
@@ -356,16 +365,20 @@
 getIncludedMappings = function() {
     let indices = getIncludedIndices()
     let mappings = []
     if (TABLES.length === indices.length && ABBS.length === indices.length) {
 
         for (index of indices) {
             mapping = {}
+            let kwargs = getKwargs(index)
+            if (kwargs["type"] == "lexicon")
+                mapping['mapping'] = null;
+            else
+                mapping['mapping'] = TABLES[index].getSourceData().filter(v => v.in)
             // Extract only non-empty rules and abbreviations for processing
-            mapping['mapping'] = TABLES[index].getSourceData().filter(v => v.in)
             mapping['abbreviations'] = ABBS[index].getData().filter(v => v[0])
             mapping['kwargs'] = getKwargs(index)
             mappings.push(mapping)
         }
     }
     return mappings
 }
@@ -376,25 +389,35 @@
     const escape_special = document.getElementById(`escape_special-${index}`).checked
     const reverse = document.getElementById(`reverse-${index}`).checked
     const include = document.getElementById(`include-${index}`).checked
     const out_delimiter = document.getElementById(`out_delimiter-${index}`).value
     const prevent_feeding = document.getElementById(`prevent_feeding-${index}`).checked
     const norm_form = document.getElementById(`norm_form-${index}`).value
     const type = document.getElementById(`type-${index}`).value
-    return {
-        rule_ordering,
-        case_sensitive,
-        escape_special,
-        reverse,
-        include,
-        out_delimiter,
-        norm_form,
-        prevent_feeding,
-        type
-    }
+    if (type === "lexicon") {
+        const in_lang = document.getElementById(`in_lang-${index}`).value
+        const out_lang = document.getElementById(`out_lang-${index}`).value
+        // Lexicon G2P cannot be customized (FIXME: likewise for unidecode actually)
+        return {
+            type,
+            in_lang,
+            out_lang
+        }
+    } else
+        return {
+            rule_ordering,
+            case_sensitive,
+            escape_special,
+            reverse,
+            include,
+            out_delimiter,
+            norm_form,
+            prevent_feeding,
+            type
+        }
 }
 
 var setKwargs = function(index, kwargs) {
     if ('rule_ordering' in kwargs) {
         $(`#rule_ordering-${index}`).val(kwargs['rule_ordering'])
     }
     if ('case_sensitive' in kwargs) {
@@ -417,14 +440,20 @@
     }
     if ('norm_form' in kwargs) {
         document.getElementById(`norm_form-${index}`).value = kwargs['norm_form']
     }
     if ('type' in kwargs) {
         document.getElementById(`type-${index}`).value = kwargs['type']
     }
+    if ('in_lang' in kwargs) {
+        document.getElementById(`in_lang-${index}`).value = kwargs['in_lang']
+    }
+    if ('out_lang' in kwargs) {
+        document.getElementById(`out_lang-${index}`).value = kwargs['out_lang']
+    }
     convert()
 }
 
 var conversionSocket = io.connect('//' + document.domain + ':' + location.port + '/convert');
 var connectionSocket = io.connect('//' + document.domain + ':' + location.port + '/connect');
 var tableSocket = io.connect('//' + document.domain + ':' + location.port + '/table');
```

### Comparing `g2p-1.0.20230228/g2p/static/echart_custom.js` & `g2p-1.0.20230412/g2p/static/echart_custom.js`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/static/languages-network.json` & `g2p-1.0.20230412/g2p/static/languages-network.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9702968750000001%*

 * *Differences: {"'edges'": "{insert: [(35, OrderedDict([('source', 'eng'), ('target', 'eng-ipa')]))]}",*

 * * "'nodes'": "{0: {'symbolSize': 2.4}, 1: {'symbolSize': 2.4000000000000004}, 2: {'symbolSize': "*

 * *            "2.4}, 3: {'symbolSize': 2.4000000000000004}, 4: {'symbolSize': 2.4}, 5: "*

 * *            "{'symbolSize': 2.4000000000000004}, 8: {'symbolSize': 2.4}, 9: {'symbolSize': 3.2}, "*

 * *            "10: {'symbolSize': 2.4}, 11: {'symbolSize': 3.2}, 12: {'symbolSize': 3.2}, 13: "*

 * *            "{'symbolSize': 3.2}, 14: {'symbol […]*

```diff
@@ -137,14 +137,18 @@
             "target": "hamming-dummy-eng-arpabet"
         },
         {
             "source": "hamming-eng-ipa",
             "target": "hamming-eng-arpabet"
         },
         {
+            "source": "eng",
+            "target": "eng-ipa"
+        },
+        {
             "source": "fin",
             "target": "fin-ipa"
         },
         {
             "source": "fin-ipa",
             "target": "eng-ipa"
         },
@@ -510,45 +514,45 @@
         }
     ],
     "nodes": [
         {
             "category": "alq",
             "id": "alq",
             "name": "alq",
-            "symbolSize": 2.4193548387096775
+            "symbolSize": 2.4
         },
         {
             "category": "alq",
             "id": "alq-ipa",
             "name": "alq-ipa",
-            "symbolSize": 2.419354838709677
+            "symbolSize": 2.4000000000000004
         },
         {
             "category": "atj",
             "id": "atj",
             "name": "atj",
-            "symbolSize": 2.4193548387096775
+            "symbolSize": 2.4
         },
         {
             "category": "atj",
             "id": "atj-ipa",
             "name": "atj-ipa",
-            "symbolSize": 2.419354838709677
+            "symbolSize": 2.4000000000000004
         },
         {
             "category": "ckt",
             "id": "ckt",
             "name": "ckt",
-            "symbolSize": 2.4193548387096775
+            "symbolSize": 2.4
         },
         {
             "category": "ckt",
             "id": "ckt-ipa",
             "name": "ckt-ipa",
-            "symbolSize": 2.419354838709677
+            "symbolSize": 2.4000000000000004
         },
         {
             "category": "clc",
             "id": "clc",
             "name": "clc",
             "symbolSize": 2
         },
@@ -558,99 +562,99 @@
             "name": "clc-doulos",
             "symbolSize": 2
         },
         {
             "category": "crg",
             "id": "crg-dv",
             "name": "crg-dv",
-            "symbolSize": 2.4193548387096775
+            "symbolSize": 2.4
         },
         {
             "category": "crg",
             "id": "crg-ipa",
             "name": "crg-ipa",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "crg",
             "id": "crg-tmd",
             "name": "crg-tmd",
-            "symbolSize": 2.4193548387096775
+            "symbolSize": 2.4
         },
         {
             "category": "crj",
             "id": "crj",
             "name": "crj",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "crj",
             "id": "crj-equiv",
             "name": "crj-equiv",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "crj",
             "id": "crj-ipa",
             "name": "crj-ipa",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "crk",
             "id": "crk",
             "name": "crk",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "crk",
             "id": "crk-ipa",
             "name": "crk-ipa",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "crk",
             "id": "crk-no-symbols",
             "name": "crk-no-symbols",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "crl",
             "id": "crl",
             "name": "crl",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "crl",
             "id": "crl-equiv",
             "name": "crl-equiv",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "crl",
             "id": "crl-ipa",
             "name": "crl-ipa",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "crm",
             "id": "crm",
             "name": "crm",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "crm",
             "id": "crm-equiv",
             "name": "crm-equiv",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "crm",
             "id": "crm-ipa",
             "name": "crm-ipa",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "crx",
             "id": "crx-sro",
             "name": "crx-sro",
             "symbolSize": 2
         },
@@ -660,63 +664,69 @@
             "name": "crx-syl",
             "symbolSize": 2
         },
         {
             "category": "csw",
             "id": "csw",
             "name": "csw",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "csw",
             "id": "csw-equiv",
             "name": "csw-equiv",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "csw",
             "id": "csw-ipa",
             "name": "csw-ipa",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "ctp",
             "id": "ctp",
             "name": "ctp",
-            "symbolSize": 2.4193548387096775
+            "symbolSize": 2.4
         },
         {
             "category": "ctp",
             "id": "ctp-ipa",
             "name": "ctp-ipa",
-            "symbolSize": 2.419354838709677
+            "symbolSize": 2.4000000000000004
         },
         {
             "category": "dan",
             "id": "dan",
             "name": "dan",
-            "symbolSize": 2.4193548387096775
+            "symbolSize": 2.4
         },
         {
             "category": "dan",
             "id": "dan-ipa",
             "name": "dan-ipa",
-            "symbolSize": 2.419354838709677
+            "symbolSize": 2.4000000000000004
         },
         {
             "category": "dummy",
             "id": "dummy",
             "name": "dummy",
-            "symbolSize": 7.258064516129032
+            "symbolSize": 7.2
         },
         {
             "category": "dummy",
             "id": "dummy-eng-arpabet",
             "name": "dummy-eng-arpabet",
-            "symbolSize": 7.258064516129033
+            "symbolSize": 7.199999999999999
+        },
+        {
+            "category": "eng",
+            "id": "eng",
+            "name": "eng",
+            "symbolSize": 2
         },
         {
             "category": "eng",
             "id": "eng-arpabet",
             "name": "eng-arpabet",
             "symbolSize": 20
         },
@@ -726,21 +736,21 @@
             "name": "eng-ipa",
             "symbolSize": 20
         },
         {
             "category": "fin",
             "id": "fin",
             "name": "fin",
-            "symbolSize": 2.4193548387096775
+            "symbolSize": 2.4
         },
         {
             "category": "fin",
             "id": "fin-ipa",
             "name": "fin-ipa",
-            "symbolSize": 2.419354838709677
+            "symbolSize": 2.4000000000000004
         },
         {
             "category": "fn",
             "id": "fn-unicode",
             "name": "fn-unicode",
             "symbolSize": 2
         },
@@ -750,27 +760,27 @@
             "name": "fn-unicode-font",
             "symbolSize": 2
         },
         {
             "category": "fra",
             "id": "fra",
             "name": "fra",
-            "symbolSize": 2.4193548387096775
+            "symbolSize": 2.4
         },
         {
             "category": "fra",
             "id": "fra-ipa",
             "name": "fra-ipa",
-            "symbolSize": 2.419354838709677
+            "symbolSize": 2.4000000000000004
         },
         {
             "category": "git",
             "id": "git",
             "name": "git",
-            "symbolSize": 4.032258064516129
+            "symbolSize": 4.0
         },
         {
             "category": "git",
             "id": "git-apa",
             "name": "git-apa",
             "symbolSize": 2
         },
@@ -780,87 +790,87 @@
             "name": "git-equiv",
             "symbolSize": 2
         },
         {
             "category": "git",
             "id": "git-ipa",
             "name": "git-ipa",
-            "symbolSize": 2.419354838709677
+            "symbolSize": 2.4000000000000004
         },
         {
             "category": "gla",
             "id": "gla",
             "name": "gla",
-            "symbolSize": 2.4193548387096775
+            "symbolSize": 2.4
         },
         {
             "category": "gla",
             "id": "gla-ipa",
             "name": "gla-ipa",
-            "symbolSize": 2.419354838709677
+            "symbolSize": 2.4000000000000004
         },
         {
             "category": "gwi",
             "id": "gwi",
             "name": "gwi",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "gwi",
             "id": "gwi-equiv",
             "name": "gwi-equiv",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "gwi",
             "id": "gwi-ipa",
             "name": "gwi-ipa",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "haa",
             "id": "haa",
             "name": "haa",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "haa",
             "id": "haa-equiv",
             "name": "haa-equiv",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "haa",
             "id": "haa-ipa",
             "name": "haa-ipa",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "hamming",
             "id": "hamming-dummy",
             "name": "hamming-dummy",
-            "symbolSize": 7.258064516129032
+            "symbolSize": 7.2
         },
         {
             "category": "hamming",
             "id": "hamming-dummy-eng-arpabet",
             "name": "hamming-dummy-eng-arpabet",
-            "symbolSize": 7.258064516129033
+            "symbolSize": 7.199999999999999
         },
         {
             "category": "hamming",
             "id": "hamming-eng-arpabet",
             "name": "hamming-eng-arpabet",
-            "symbolSize": 12.903225806451612
+            "symbolSize": 12.8
         },
         {
             "category": "hamming",
             "id": "hamming-eng-ipa",
             "name": "hamming-eng-ipa",
-            "symbolSize": 12.903225806451614
+            "symbolSize": 12.8
         },
         {
             "category": "hei",
             "id": "hei",
             "name": "hei",
             "symbolSize": 2
         },
@@ -876,87 +886,87 @@
             "name": "hei-times-font",
             "symbolSize": 2
         },
         {
             "category": "ikt",
             "id": "ikt",
             "name": "ikt",
-            "symbolSize": 4.032258064516129
+            "symbolSize": 4.0
         },
         {
             "category": "ikt",
             "id": "ikt-ipa",
             "name": "ikt-ipa",
-            "symbolSize": 4.032258064516129
+            "symbolSize": 4.0
         },
         {
             "category": "iku",
             "id": "iku",
             "name": "iku",
-            "symbolSize": 4.838709677419355
+            "symbolSize": 4.8
         },
         {
             "category": "iku",
             "id": "iku-equiv",
             "name": "iku-equiv",
-            "symbolSize": 4.838709677419355
+            "symbolSize": 4.8
         },
         {
             "category": "iku",
             "id": "iku-ipa",
             "name": "iku-ipa",
-            "symbolSize": 4.838709677419354
+            "symbolSize": 4.800000000000001
         },
         {
             "category": "iku",
             "id": "iku-sro",
             "name": "iku-sro",
-            "symbolSize": 2.4193548387096775
+            "symbolSize": 2.4
         },
         {
             "category": "iku",
             "id": "iku-sro-ipa",
             "name": "iku-sro-ipa",
-            "symbolSize": 2.419354838709677
+            "symbolSize": 2.4000000000000004
         },
         {
             "category": "ipa",
             "id": "ipa",
             "name": "ipa",
             "symbolSize": 2
         },
         {
             "category": "kkz",
             "id": "kkz",
             "name": "kkz",
-            "symbolSize": 2.4193548387096775
+            "symbolSize": 2.4
         },
         {
             "category": "kkz",
             "id": "kkz-ipa",
             "name": "kkz-ipa",
-            "symbolSize": 2.419354838709677
+            "symbolSize": 2.4000000000000004
         },
         {
             "category": "kwk",
             "id": "kwk-boas",
             "name": "kwk-boas",
-            "symbolSize": 4.032258064516129
+            "symbolSize": 4.0
         },
         {
             "category": "kwk",
             "id": "kwk-ipa",
             "name": "kwk-ipa",
-            "symbolSize": 4.032258064516129
+            "symbolSize": 4.0
         },
         {
             "category": "kwk",
             "id": "kwk-napa",
             "name": "kwk-napa",
-            "symbolSize": 2.4193548387096775
+            "symbolSize": 2.4
         },
         {
             "category": "kwk",
             "id": "kwk-napa-ubc",
             "name": "kwk-napa-ubc",
             "symbolSize": 2
         },
@@ -978,81 +988,81 @@
             "name": "kwk-napa-uvic-con",
             "symbolSize": 2
         },
         {
             "category": "kwk",
             "id": "kwk-umista",
             "name": "kwk-umista",
-            "symbolSize": 4.032258064516129
+            "symbolSize": 4.0
         },
         {
             "category": "kwk",
             "id": "kwk-umista-con",
             "name": "kwk-umista-con",
             "symbolSize": 2
         },
         {
             "category": "lml",
             "id": "lml",
             "name": "lml",
-            "symbolSize": 2.4193548387096775
+            "symbolSize": 2.4
         },
         {
             "category": "lml",
             "id": "lml-ipa",
             "name": "lml-ipa",
-            "symbolSize": 2.419354838709677
+            "symbolSize": 2.4000000000000004
         },
         {
             "category": "mic",
             "id": "mic",
             "name": "mic",
-            "symbolSize": 2.4193548387096775
+            "symbolSize": 2.4
         },
         {
             "category": "mic",
             "id": "mic-ipa",
             "name": "mic-ipa",
-            "symbolSize": 2.419354838709677
+            "symbolSize": 2.4000000000000004
         },
         {
             "category": "moe",
             "id": "moe",
             "name": "moe",
-            "symbolSize": 2.4193548387096775
+            "symbolSize": 2.4
         },
         {
             "category": "moe",
             "id": "moe-ipa",
             "name": "moe-ipa",
-            "symbolSize": 2.419354838709677
+            "symbolSize": 2.4000000000000004
         },
         {
             "category": "moh",
             "id": "moh",
             "name": "moh",
-            "symbolSize": 11.290322580645162
+            "symbolSize": 11.2
         },
         {
             "category": "moh",
             "id": "moh-equiv",
             "name": "moh-equiv",
-            "symbolSize": 11.290322580645162
+            "symbolSize": 11.2
         },
         {
             "category": "moh",
             "id": "moh-festival",
             "name": "moh-festival",
-            "symbolSize": 11.290322580645162
+            "symbolSize": 11.2
         },
         {
             "category": "moh",
             "id": "moh-ipa",
             "name": "moh-ipa",
-            "symbolSize": 11.290322580645162
+            "symbolSize": 11.2
         },
         {
             "category": "nav",
             "id": "nav",
             "name": "nav",
             "symbolSize": 2
         },
@@ -1062,197 +1072,197 @@
             "name": "nav-times-font",
             "symbolSize": 2
         },
         {
             "category": "oji",
             "id": "oji",
             "name": "oji",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "oji",
             "id": "oji-ipa",
             "name": "oji-ipa",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "oji",
             "id": "oji-syl",
             "name": "oji-syl",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "oka",
             "id": "oka",
             "name": "oka",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "oka",
             "id": "oka-equiv",
             "name": "oka-equiv",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "oka",
             "id": "oka-ipa",
             "name": "oka-ipa",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "see",
             "id": "see",
             "name": "see",
-            "symbolSize": 2.4193548387096775
+            "symbolSize": 2.4
         },
         {
             "category": "see",
             "id": "see-ipa",
             "name": "see-ipa",
-            "symbolSize": 2.419354838709677
+            "symbolSize": 2.4000000000000004
         },
         {
             "category": "srs",
             "id": "srs",
             "name": "srs",
-            "symbolSize": 2.4193548387096775
+            "symbolSize": 2.4
         },
         {
             "category": "srs",
             "id": "srs-ipa",
             "name": "srs-ipa",
-            "symbolSize": 2.419354838709677
+            "symbolSize": 2.4000000000000004
         },
         {
             "category": "str",
             "id": "str",
             "name": "str",
-            "symbolSize": 8.064516129032258
+            "symbolSize": 8.0
         },
         {
             "category": "str",
             "id": "str-equiv",
             "name": "str-equiv",
-            "symbolSize": 8.064516129032258
+            "symbolSize": 7.999999999999999
         },
         {
             "category": "str",
             "id": "str-ipa",
             "name": "str-ipa",
-            "symbolSize": 4.838709677419354
+            "symbolSize": 4.800000000000001
         },
         {
             "category": "tau",
             "id": "tau",
             "name": "tau",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "tau",
             "id": "tau-equiv",
             "name": "tau-equiv",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "tau",
             "id": "tau-ipa",
             "name": "tau-ipa",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "tce",
             "id": "tce",
             "name": "tce",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "tce",
             "id": "tce-equiv",
             "name": "tce-equiv",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "tce",
             "id": "tce-ipa",
             "name": "tce-ipa",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "tgx",
             "id": "tgx",
             "name": "tgx",
-            "symbolSize": 2.4193548387096775
+            "symbolSize": 2.4
         },
         {
             "category": "tgx",
             "id": "tgx-ipa",
             "name": "tgx-ipa",
-            "symbolSize": 2.419354838709677
+            "symbolSize": 2.4000000000000004
         },
         {
             "category": "tli",
             "id": "tli",
             "name": "tli",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "tli",
             "id": "tli-equiv",
             "name": "tli-equiv",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "tli",
             "id": "tli-ipa",
             "name": "tli-ipa",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "ttm",
             "id": "ttm",
             "name": "ttm",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "ttm",
             "id": "ttm-equiv",
             "name": "ttm-equiv",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "ttm",
             "id": "ttm-ipa",
             "name": "ttm-ipa",
-            "symbolSize": 3.225806451612903
+            "symbolSize": 3.2
         },
         {
             "category": "und",
             "id": "und",
             "name": "und",
-            "symbolSize": 8.064516129032258
+            "symbolSize": 8.0
         },
         {
             "category": "und",
             "id": "und-ascii",
             "name": "und-ascii",
-            "symbolSize": 8.064516129032258
+            "symbolSize": 7.999999999999999
         },
         {
             "category": "und",
             "id": "und-ipa",
             "name": "und-ipa",
-            "symbolSize": 4.838709677419354
+            "symbolSize": 4.800000000000001
         },
         {
             "category": "win",
             "id": "win",
             "name": "win",
-            "symbolSize": 2.4193548387096775
+            "symbolSize": 2.4
         },
         {
             "category": "win",
             "id": "win-ipa",
             "name": "win-ipa",
-            "symbolSize": 2.419354838709677
+            "symbolSize": 2.4000000000000004
         }
     ]
 }
```

### Comparing `g2p-1.0.20230228/g2p/static/normalize.css` & `g2p-1.0.20230412/g2p/static/normalize.css`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/static/skeleton.css` & `g2p-1.0.20230412/g2p/static/skeleton.css`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/static/swagger.json` & `g2p-1.0.20230412/g2p/static/swagger.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999583333333333%*

 * *Differences: {"'components'": "{'schemas': {'Langs': {'enum': {insert: [(34, 'eng')]}}}}"}*

```diff
@@ -33,14 +33,15 @@
                     "csw-ipa",
                     "ctp",
                     "ctp-ipa",
                     "dan",
                     "dan-ipa",
                     "dummy",
                     "dummy-eng-arpabet",
+                    "eng",
                     "eng-arpabet",
                     "eng-ipa",
                     "fin",
                     "fin-ipa",
                     "fn-unicode",
                     "fn-unicode-font",
                     "fra",
```

### Comparing `g2p-1.0.20230228/g2p/templates/docs.html` & `g2p-1.0.20230412/g2p/templates/docs.html`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/templates/index.html` & `g2p-1.0.20230412/g2p/templates/index.html`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/tests/public/data/__init__.py` & `g2p-1.0.20230412/g2p/tests/public/data/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 Each line in the test file consists of SOURCE,TARGET,INPUT,OUTPUT
 """
 
 import csv
 import os
 from glob import glob
+from typing import List
 
 from g2p.log import LOGGER
 
 """Directory where the public test data is located"""
 DATA_DIR = os.path.dirname(__file__)
 
 """Cached for langs data, so we don't have to reload it multiple times"""
 loaded_langs_to_test = None
 
 
-def load_public_test_data():
+def load_public_test_data() -> List[List[str]]:
     """Load public/data/*.?sv for test data in various languages
 
-    Returns: List[List[in_lang, out_lang, in_text, out_text]]
+    Returns: List[List[in_lang, out_lang, in_text, out_text, filename:lineno]]
     """
     global loaded_langs_to_test
     if loaded_langs_to_test is not None:
         return loaded_langs_to_test
 
     langs_to_test = []
     for fn in sorted(glob(os.path.join(DATA_DIR, "*.*sv"))):
@@ -53,11 +54,12 @@
                     continue
                 elif len(row) < 4:
                     LOGGER.warning(
                         f"Row in {fn} containing values {row} does not have the right values."
                         f"Please check your data."
                     )
                 else:
+                    row.append(f"{fn}:{i+1}")
                     langs_to_test.append(row)
 
     loaded_langs_to_test = langs_to_test
     return langs_to_test
```

### Comparing `g2p-1.0.20230228/g2p/tests/public/data/crl.psv` & `g2p-1.0.20230412/g2p/tests/public/data/crl.psv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/tests/public/data/fin.psv` & `g2p-1.0.20230412/g2p/tests/public/data/fin.psv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/tests/public/data/fra.psv` & `g2p-1.0.20230412/g2p/tests/public/data/fra.psv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/tests/public/data/fra_panagrams.txt` & `g2p-1.0.20230412/g2p/tests/public/data/fra_panagrams.txt`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/tests/public/data/fra_panagrams_NFD.txt` & `g2p-1.0.20230412/g2p/tests/public/data/fra_panagrams_NFD.txt`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/tests/public/data/gwi.psv` & `g2p-1.0.20230412/g2p/tests/public/data/gwi.psv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/tests/public/data/haa.csv` & `g2p-1.0.20230412/g2p/tests/public/data/haa.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/tests/public/data/ikt.psv` & `g2p-1.0.20230412/g2p/tests/public/data/ikt.psv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/tests/public/data/iku-sro.psv` & `g2p-1.0.20230412/g2p/tests/public/data/iku-sro.psv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/tests/public/data/mic.psv` & `g2p-1.0.20230412/g2p/tests/public/data/mic.psv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/tests/public/data/moh.psv` & `g2p-1.0.20230412/g2p/tests/public/data/moh.psv`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 moh|moh-ipa|tshiateiakorí:wake|t͡ʃadeiaɡoríːwaɡe|palatalization test and high tone i #2
 moh|moh-ipa|wahonwarihótahsien|wahũwarihódaʃʌ̃|palatalization test and stressed o #3
 moh|moh-ipa|ioteri'wahséhton|ioderiʔwahséhdũ|voicing test and stressed e #1
 moh|moh-ipa|Wahshakawénhahse|wahshaɡawʌ̃́hahse|voicing test and stressed e #2
 moh|moh-ipa|watkwenhrá:rons|watɡʷʌ̃hráːrũs|voicing test and high tone a #3
 moh|moh-ipa|Sáhtkawh|sáhtɡaf
 moh|moh-ipa|kèn:reks|ɡʌ̃̀ːreks
+moh|moh-ipa|Borakén Makhró Aprám|boraɡʌ̃́ makhró aprám|borrowed foreign words
+moh|moh-ipa|aonsákken'|aũsákɡʌ̃ʔ
 moh|moh-festival|ronwahnonterátie's|roNwahnoNdera1dze7s|palatalization test and stresssed a #1
 moh|moh-festival|tshiateiakorí:wake|chadeiagori1Lwage|palatalization test and high tone i #2
 moh|moh-festival|wahonwarihótahsien|wahoNwariho1daxheN|palatalization test and stressed o #3
 moh|moh-festival|ioteri'wahséhton|ioderi7wahse1hdoN|voicing test and stressed e #1
 moh|moh-festival|Wahshakawénhahse|wahshagaweN1hahse|voicing test and stressed e #2
 moh|moh-festival|watkwenhrá:rons|watgWeNhra1LroNs|voicing test and high tone a #3
 moh|moh-festival|Sáhtkawh|sa1htgaf
@@ -33,10 +35,10 @@
 moh-festival|moh|watgWeNhra1LroNs|watkwenhrá:rons|voicing test and high tone a #3
 moh-festival|moh|sa1htgaf|sáhtkawh
 moh-festival|moh|geN2Lreks|kèn:reks
 moh|moh-equiv|ohna'kènke|ohna'kèn:ke|low tone vowels must be long
 moh|moh-equiv|wahrènehste|wahrè:nehste
 moh-ipa|moh|ohnaʔɡʌ̃̀ːɡe|ohna'kèn:ke|low tone vowels must be long
 moh-ipa|moh|wahrèːnehsde|wahrè:nehste|low tone vowels must be long
-moh|eng-arpabet|satetshén'en|S AE D EH T S HH AH N HH AH N 
+moh|eng-arpabet|satetshén'en|S AE D EH T S HH AH N HH AH N
 moh|eng-ipa|ó:ni|oːni
-moh|moh-equiv|iahontòkten|iahontò:kten
+moh|moh-equiv|iahontòkten|iahontò:kten
```

### Comparing `g2p-1.0.20230228/g2p/tests/public/data/oji-syl.psv` & `g2p-1.0.20230412/g2p/tests/public/data/oji-syl.psv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/tests/public/data/oka.csv` & `g2p-1.0.20230412/g2p/tests/public/data/oka.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/tests/public/data/tau.psv` & `g2p-1.0.20230412/g2p/tests/public/data/tau.psv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/tests/public/data/tli.csv` & `g2p-1.0.20230412/g2p/tests/public/data/tli.csv`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/tests/public/mappings/case-feed/README.md` & `g2p-1.0.20230412/g2p/tests/public/mappings/case-feed/README.md`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/tests/public/mappings/case-feed/config.yaml` & `g2p-1.0.20230412/g2p/tests/public/mappings/case-feed/config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/tests/public/mappings/gen-map_config.yaml` & `g2p-1.0.20230412/g2p/tests/public/mappings/gen-map_config.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/tests/public/mappings/minimal.xlsx` & `g2p-1.0.20230412/g2p/tests/public/mappings/minimal.xlsx`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/tests/public/mappings/minimal_configs.yaml` & `g2p-1.0.20230412/g2p/tests/public/mappings/minimal_configs.yaml`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/tests/public/sample_response.json` & `g2p-1.0.20230412/g2p/tests/public/sample_response.json`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/tests/run.py` & `g2p-1.0.20230412/g2p/tests/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,37 +16,37 @@
 # Unit tests
 from g2p.log import LOGGER
 from g2p.tests.test_api_resources import ResourceIntegrationTest
 from g2p.tests.test_check_ipa_arpabet import CheckIpaArpabetTest
 from g2p.tests.test_cli import CliTest
 from g2p.tests.test_create_mapping import MappingCreationTest
 from g2p.tests.test_doctor import DoctorTest
+from g2p.tests.test_doctor_expensive import ExpensiveDoctorTest
 from g2p.tests.test_fallback import FallbackTest
 from g2p.tests.test_indices import IndicesTest
 from g2p.tests.test_langs import LangTest
+from g2p.tests.test_lexicon_transducer import LexiconTransducerTest
 from g2p.tests.test_mappings import MappingTest
 from g2p.tests.test_network import NetworkTest
 from g2p.tests.test_tokenize_and_map import TokenizeAndMapTest
 from g2p.tests.test_tokenizer import TokenizerTest
 from g2p.tests.test_transducer import TransducerTest
 from g2p.tests.test_unidecode_transducer import UnidecodeTransducerTest
 from g2p.tests.test_utils import UtilsTest
 from g2p.tests.test_z_local_config import LocalConfigTest
 
-# Deliberately left out:
-# from g2p.tests.test_doctor_expensive import ExpensiveDoctorTest
-
 LOADER = TestLoader()
 
 TRANSDUCER_TESTS = [
     LOADER.loadTestsFromTestCase(test)
     for test in [
         IndicesTest,
         TransducerTest,
         UnidecodeTransducerTest,
+        LexiconTransducerTest,
     ]
 ]
 
 MAPPINGS_TESTS = [
     LOADER.loadTestsFromTestCase(test)
     for test in [
         FallbackTest,
@@ -69,14 +69,15 @@
 
 INTEGRATION_TESTS = [
     LOADER.loadTestsFromTestCase(test)
     for test in [
         CliTest,
         ResourceIntegrationTest,
         DoctorTest,
+        ExpensiveDoctorTest,
     ]
 ]
 
 # LocalConfigTest has to get run last, to avoid interactions with other test
 # cases, since it has side effects on the global database
 LAST_DEV_TEST = [
     LOADER.loadTestsFromTestCase(test)
```

### Comparing `g2p-1.0.20230228/g2p/tests/test_api_resources.py` & `g2p-1.0.20230412/g2p/tests/test_api_resources.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,28 +60,28 @@
         Ensure all routes return 200
         """
         for rt in self.routes_no_args:
             try:
                 r = self.client().get(rt)
                 self.assertEqual(r.status_code, 200)
                 LOGGER.debug("Route " + rt + " returned " + str(r.status_code))
-            except:
+            except Exception:
                 LOGGER.error("Couldn't connect. Is flask running?")
 
     def test_response_code_with_args(self):
         """
         Ensure all args return 200
         """
         for ep in self.routes_only_args:
             for node in LANGS_NETWORK.nodes:
                 rt = re.sub(self.arg_match, node, ep)
                 try:
                     r = self.client().get(rt)
                     self.assertEqual(r.status_code, 200)
-                except:
+                except Exception:
                     LOGGER.error("Couldn't connect. Is flask running?")
             LOGGER.debug(
                 "Successfully tested "
                 + str(len(LANGS_NETWORK.nodes))
                 + " node resources at route "
                 + ep
                 + " ."
@@ -123,21 +123,26 @@
         minimal_response = self.client().get(
             self.conversion_route, query_string=minimal_params
         )
         data["debugger"] = False
         data["index"] = False
         self.assertEqual(minimal_response.status_code, 200)
         self.assertEqual(minimal_response.get_json(), data)
-        bad_response = self.client().get(self.conversion_route, query_string=bad_params)
-        same_response = self.client().get(
-            self.conversion_route, query_string=same_params
-        )
+        with self.assertLogs(LOGGER, level="ERROR"):
+            bad_response = self.client().get(
+                self.conversion_route, query_string=bad_params
+            )
+        with self.assertLogs(LOGGER, level="ERROR"):
+            same_response = self.client().get(
+                self.conversion_route, query_string=same_params
+            )
         self.assertEqual(bad_response.status_code, 400)
         self.assertEqual(same_response.status_code, 400)
-        missing_response = self.client().get(
-            self.conversion_route, query_string=missing_params
-        )
+        with self.assertLogs(LOGGER, level="ERROR"):
+            missing_response = self.client().get(
+                self.conversion_route, query_string=missing_params
+            )
         self.assertEqual(missing_response.status_code, 404)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `g2p-1.0.20230228/g2p/tests/test_check_ipa_arpabet.py` & `g2p-1.0.20230412/g2p/tests/test_check_ipa_arpabet.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 class CheckIpaArpabetTest(TestCase):
     def test_is_IPA(self):
         self.assertTrue(utils.is_panphon("ijŋeːʒoːɡd͡ʒ"))  # All panphon chars
         self.assertTrue(utils.is_panphon("ij ij"))  # tokenizes on spaces
         # ASCII g is not ipa/panphon use ɡ (\u0261)
         # self.assertFalse(utils.is_panphon("ga"))  - tolerated because of panphon preprocessor!
         # ASCII : is not ipa/panphon, use ː (\u02D0)
-        self.assertFalse(utils.is_panphon("ge:", display_warnings=True))
+        with self.assertLogs(LOGGER, level="WARNING"):
+            self.assertFalse(utils.is_panphon("ge:", display_warnings=True))
 
     def test_is_arpabet(self):
         arpabet_string = "S AH S IY  EH  AO N  T EH"
         non_arpabet_string = "sometext"
         self.assertTrue(utils.is_arpabet(arpabet_string))
         self.assertFalse(utils.is_arpabet(non_arpabet_string))
 
@@ -31,15 +32,16 @@
         self.assertTrue(transducer.check(transducer("ɡɑŋi")))
         self.assertFalse(transducer.check(transducer("ñ")))
 
     def test_check_ipa(self):
         transducer = make_g2p("fra", "fra-ipa")
         self.assertTrue(transducer.check(transducer("ceci")))
         self.assertFalse(transducer.check(transducer("ñ")))
-        self.assertFalse(transducer.check(transducer("ñ"), display_warnings=True))
+        with self.assertLogs(LOGGER, level="WARNING"):
+            self.assertFalse(transducer.check(transducer("ñ"), display_warnings=True))
         self.assertTrue(transducer.check(transducer("ceci est un test été à")))
 
         transducer = make_g2p("fra-ipa", "eng-ipa")
         self.assertFalse(transducer.check(transducer("ñ")))
 
     def test_is_ipa_with_panphon_preprocessor(self):
         # panphon doesn't like these directly, but our panphon proprocessor "patches" them
@@ -68,20 +70,21 @@
         self.assertFalse(transducer.check(transducer("ñ oǹ")))
         self.assertTrue(
             transducer.check(transducer("ceci, cela; c'est tokenizé: alors c'est bon!"))
         )
         self.assertFalse(
             transducer.check(transducer("mais... c'est ñoñ, si du texte ne passe pas!"))
         )
-        self.assertFalse(
-            transducer.check(
-                transducer("mais... c'est ñoñ, si du texte ne passe pas!"),
-                display_warnings=True,
+        with self.assertLogs(LOGGER, level="WARNING"):
+            self.assertFalse(
+                transducer.check(
+                    transducer("mais... c'est ñoñ, si du texte ne passe pas!"),
+                    display_warnings=True,
+                )
             )
-        )
 
     def test_shallow_check(self):
         transducer = make_g2p("win", "eng-arpabet", tok_lang="win")
         # This is False, but should be True! It's False because the mapping outputs :
         # instead of ː
         # EJJ 2022-06-16 With #100 fixed, this check is no longer failing.
         # self.assertFalse(transducer.check(transducer("uu")))
@@ -98,17 +101,17 @@
             "sh'oo Jign maasee' do'eent'aa shyyyh"
         ).output_string
         self.assertTrue(utils.is_panphon(eng_ipa))
         eng_arpabet = make_g2p("tau", "eng-arpabet", tok_lang="tau")(
             "sh'oo Jign maasee' do'eent'aa shyyyh"
         ).output_string
         self.assertTrue(utils.is_arpabet(eng_arpabet))
-        LOGGER.warning(
-            f"tau-ipa {tau_ipa}\neng-ipa {eng_ipa}\n eng-arpabet {eng_arpabet}"
-        )
+        # LOGGER.warning(
+        #     f"tau-ipa {tau_ipa}\neng-ipa {eng_ipa}\n eng-arpabet {eng_arpabet}"
+        # )
         self.assertTrue(
             transducer.check(transducer("sh'oo Jign maasee' do'eent'aa shyyyh"))
         )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `g2p-1.0.20230228/g2p/tests/test_cli.py` & `g2p-1.0.20230412/g2p/tests/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         for tok_option in [["--tok", "--check"], ["--no-tok"]]:
             for test in langs_to_test:
                 output_string = self.runner.invoke(
                     convert, [*tok_option, test[2], test[0], test[1]]
                 ).stdout.strip()
                 if output_string != test[3].strip():
                     LOGGER.warning(
-                        f"test_cli.py: {test[0]}->{test[1]} mapping error: '{test[2]}' "
+                        f"test_cli.py for {test[-1]}: {test[0]}->{test[1]} mapping error: '{test[2]}' "
                         f"should map to '{test[3]}', got '{output_string}' (with {tok_option})."
                     )
                     if error_count == 0:
                         first_failed_test = test + [tok_option]
                     error_count += 1
 
         if error_count > 0:
@@ -190,20 +190,26 @@
             self.assertIn(low, returned_set)
         mapped_upper = "ABCDEHIJKLMNOPQSTUVWXYZ"
         for u in mapped_upper:
             self.assertNotIn(u, returned_set)
         mapped_lower = "s"
         self.assertNotIn(mapped_lower, returned_set)
 
+    def test_convert_option_a(self):
+        result = self.runner.invoke(convert, "-a hello eng eng-arpabet")
+        self.assertIn(
+            "[('h', 'HH '), ('e', 'AH '), ('ll', 'L '), ('o', 'OW ')]", result.stdout
+        )
+
     def test_convert_option_e(self):
         result = self.runner.invoke(convert, "-e est fra eng-arpabet")
         for s in [
-            "[['e', 'ɛ'], ['s', 'ɛ'], ['t', 'ɛ']]",
-            "[['ɛ', 'ɛ']]",
-            "[['ɛ', 'E'], ['ɛ', 'H'], ['ɛ', ' ']]",
+            "[('e', 'ɛ'), ('s', 'ɛ'), ('t', 'ɛ')]",
+            "[('ɛ', 'ɛ')]",
+            "[('ɛ', 'E'), ('ɛ', 'H'), ('ɛ', ' ')]",
         ]:
             self.assertIn(s, result.stdout)
 
     def test_convert_option_d(self):
         result = self.runner.invoke(convert, "-d est fra eng-arpabet")
         for s in ["'input': 'est'", "'output': 'ɛ'", "'input': 'ɛ'", "'output': 'EH '"]:
             self.assertIn(s, result.stdout)
```

### Comparing `g2p-1.0.20230228/g2p/tests/test_create_mapping.py` & `g2p-1.0.20230412/g2p/tests/test_create_mapping.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
 Test all Mappings
 """
 
 from unittest import TestCase, main
 
+from g2p.log import LOGGER
 from g2p.mappings import Mapping
 from g2p.mappings.create_ipa_mapping import (
     DISTANCE_METRICS,
     create_mapping,
     create_multi_mapping,
 )
 from g2p.transducer import Transducer
@@ -37,111 +38,119 @@
     def test_unigram_mappings(self):
         src_mappings = [
             {"in": "ᐃ", "out": "i"},
             {"in": "ᐅ", "out": "u"},
             {"in": "ᐊ", "out": "a"},
         ]
         src_mapping = Mapping(src_mappings, in_lang="crj", out_lang="crj-ipa")
-        mapping = create_mapping(src_mapping, self.target_mapping)
+        mapping = create_mapping(src_mapping, self.target_mapping, quiet=True)
         transducer = Transducer(mapping)
         self.assertEqual(transducer("a").output_string, "ɑ")
         self.assertEqual(transducer("i").output_string, "i")
         self.assertEqual(transducer("u").output_string, "u")
 
     def test_bigram_mappings(self):
         src_mappings = [
             {"in": "ᐱ", "out": "pi"},
             {"in": "ᑎ", "out": "ti"},
             {"in": "ᑭ", "out": "ki"},
         ]
         src_mapping = Mapping(src_mappings, in_lang="crj", out_lang="crj-ipa")
-        mapping = create_mapping(src_mapping, self.target_mapping)
+        mapping = create_mapping(src_mapping, self.target_mapping, quiet=True)
         transducer = Transducer(mapping)
         self.assertEqual(transducer("pi").output_string, "pi")
         self.assertEqual(transducer("ti").output_string, "ti")
         self.assertEqual(transducer("ki").output_string, "ki")
 
     def test_trigram_mappings(self):
         src_mappings = [
             {"in": "ᒋ", "out": "t͡ʃi"},
             {"in": "ᒍ", "out": "t͡ʃu"},
             {"in": "ᒐ", "out": "t͡ʃa"},
         ]
         src_mapping = Mapping(src_mappings, in_lang="crj", out_lang="crj-ipa")
-        mapping = create_mapping(src_mapping, self.target_mapping)
+        mapping = create_mapping(src_mapping, self.target_mapping, quiet=True)
         transducer = Transducer(mapping)
         self.assertEqual(transducer("t͡ʃi").output_string, "tʃi")
         self.assertEqual(transducer("t͡ʃu").output_string, "tʃu")
         self.assertEqual(transducer("t͡ʃa").output_string, "tʃɑ")
 
     def test_long_mappings(self):
         src_mappings = [
             {"in": "ᐧᐯ", "out": "pʷeː"},
             {"in": "ᐧᑌ", "out": "tʷeː"},
             {"in": "ᐧᑫ", "out": "kʷeː"},
         ]
         src_mapping = Mapping(src_mappings, in_lang="crj", out_lang="crj-ipa")
-        mapping = create_mapping(src_mapping, self.target_mapping)
+        mapping = create_mapping(src_mapping, self.target_mapping, quiet=True)
         transducer = Transducer(mapping)
         self.assertEqual(transducer("pʷeː").output_string, "pweː")
         self.assertEqual(transducer("tʷeː").output_string, "tweː")
         self.assertEqual(transducer("kʷeː").output_string, "kweː")
 
     def test_distance_errors(self):
         src_mappings = [{"in": "ᐃ", "out": "i"}]
         src_mapping = Mapping(src_mappings, in_lang="crj", out_lang="crj-ipa")
         # Exercise looking up distances in the known list
         with self.assertRaises(ValueError):
             _ = create_mapping(
-                src_mapping, self.target_mapping, distance="not_a_distance"
+                src_mapping, self.target_mapping, distance="not_a_distance", quiet=True
             )
         with self.assertRaises(ValueError):
             _ = create_multi_mapping(
                 [(src_mapping, "out")],
                 [(self.target_mapping, "in")],
                 distance="not_a_distance",
+                quiet=True,
             )
         # White box testing: monkey-patch an invalid distance to validate the
         # second way we make sure distances are supported
         DISTANCE_METRICS.append("not_a_real_distance")
-        with self.assertRaises(ValueError):
+        with self.assertRaises(ValueError), self.assertLogs(LOGGER, level="ERROR"):
             _ = create_mapping(
-                src_mapping, self.target_mapping, distance="not_a_real_distance"
+                src_mapping,
+                self.target_mapping,
+                distance="not_a_real_distance",
+                quiet=True,
             )
-        with self.assertRaises(ValueError):
+        with self.assertRaises(ValueError), self.assertLogs(LOGGER, level="ERROR"):
             _ = create_multi_mapping(
                 [(src_mapping, "out")],
                 [(self.target_mapping, "in")],
                 distance="not_a_real_distance",
+                quiet=True,
             )
         DISTANCE_METRICS.pop()
 
     def test_distances(self):
         # These mapppings are chosen to create different generated mappings
         # from the various distances.
         src_mappings = [
             {"in": "ᐧᐯ", "out": "pʷeː"},
             {"in": "ᒋ", "out": "t͡ʃi"},
             {"in": "ᕃ", "out": "ʁaj"},
         ]
         src_mapping = Mapping(src_mappings, in_lang="crj", out_lang="crj-ipa")
-        mapping = create_mapping(src_mapping, self.target_mapping)
+        mapping = create_mapping(src_mapping, self.target_mapping, quiet=True)
         # print("mapping", mapping, list(mapping), "distance", "default")
         self.assertTrue(isinstance(mapping, Mapping))
         set_of_mappings = {tuple(m["out"] for m in mapping)}
         for distance in DISTANCE_METRICS:
             mapping = create_mapping(
-                src_mapping, self.target_mapping, distance=distance
+                src_mapping, self.target_mapping, distance=distance, quiet=True
             )
             # print("mapping", mapping, list(mapping), "distance", distance)
             self.assertTrue(isinstance(mapping, Mapping))
             set_of_mappings.add(tuple(m["out"] for m in mapping))
 
             mapping = create_multi_mapping(
-                [(src_mapping, "out")], [(self.target_mapping, "in")], distance=distance
+                [(src_mapping, "out")],
+                [(self.target_mapping, "in")],
+                distance=distance,
+                quiet=True,
             )
             self.assertTrue(isinstance(mapping, Mapping))
             set_of_mappings.add(tuple(m["out"] for m in mapping))
         self.assertGreater(len(set_of_mappings), 3)
 
 
 if __name__ == "__main__":
```

### Comparing `g2p-1.0.20230228/g2p/tests/test_doctor.py` & `g2p-1.0.20230412/g2p/tests/test_doctor.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/tests/test_doctor_expensive.py` & `g2p-1.0.20230412/g2p/tests/test_doctor_expensive.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,20 +20,24 @@
 
     # Migrated here from test_cli.py
     def test_doctor_cli(self):
         # TODO: assert something more useful here...
         # This test simulates calling "g2p doctor" on the command line with no arguments,
         # which runs doctor on all mappings.
         runner = APP.test_cli_runner()
-        result = runner.invoke(doctor)
+        with self.assertLogs(LOGGER, level="WARNING") as cm:
+            result = runner.invoke(doctor)
         self.assertEqual(result.exit_code, 0)
-        self.assertGreaterEqual(len(result.stdout), 10000)
+        self.assertGreaterEqual(len(cm.output), 100)
 
     # Migrated here from test_doctor.py
-    def test_ipa_known_segs_all(self):
+    # And skip this test, because test_doctor_cli() indirectly does the
+    # expensive call to check_ipa_know_segs already so there is no value in
+    # doing it a second time here.
+    def not_test_ipa_known_segs_all(self):
         # This test simulates the innards of having called "g2p doctor" on the command
         # line with no arguments, again running the innards of doctor on all mappings.
         with self.assertLogs(LOGGER, level="WARNING") as cm:
             check_ipa_known_segs()
         self.assertGreaterEqual(len(cm.output), 20)
```

### Comparing `g2p-1.0.20230228/g2p/tests/test_fallback.py` & `g2p-1.0.20230412/g2p/tests/test_fallback.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,42 +51,42 @@
                 {"in": "i", "out": "ɑ̃"},
                 {"in": "b", "out": "β"},
                 {"in": "g", "out": "ɡ"},
             ],
             in_lang="test",
             out_lang="test-ipa",
         )
-        test_in = align_to_dummy_fallback(mapping)
+        test_in = align_to_dummy_fallback(mapping, quiet=True)
         self.assertEqual(
             test_in.mapping,
             [
                 rule("a", "ɑ", "", "", "a"),
                 rule("e", "i", "", "", "e"),
                 rule("i", "i", "", "", "i"),
                 rule("b", "t", "", "", "b"),
                 rule("g", "t", "", "", "g"),
                 rule("g", "t", "", "", "g"),
                 rule("i", "i", "", "", "i"),
             ],
         )
 
-        test_out = align_to_dummy_fallback(mapping, "out")
+        test_out = align_to_dummy_fallback(mapping, "out", quiet=True)
         self.assertEqual(
             test_out.mapping,
             [
                 rule("æ", "ɑi", "", "", "æ"),
                 rule("ɐ", "ɑ", "", "", "ɐ"),
                 rule("ɑ̃", "ɑ", "", "", "ɑ̃"),
                 rule("β", "t", "", "", "β"),
                 rule("ɡ", "t", "", "", "ɡ"),
                 rule("g", "t", "", "", "g"),
                 rule("ةُ", "ɑu", "", "", "ةُ"),
             ],
         )
-        test_ipa = align_to_dummy_fallback(ipa_mapping, "out")
+        test_ipa = align_to_dummy_fallback(ipa_mapping, "out", quiet=True)
         self.assertEqual(
             test_ipa.mapping,
             [
                 rule("æ", "ɑ", "", "", "æ"),
                 rule("ɐ", "ɑ", "", "", "ɐ"),
                 rule("ɑ̃", "ɑ", "", "", "ɑ̃"),
                 rule("β", "s", "", "", "β"),
```

### Comparing `g2p-1.0.20230228/g2p/tests/test_indices.py` & `g2p-1.0.20230412/g2p/tests/test_indices.py`

 * *Files 19% similar despite different names*

```diff
@@ -161,14 +161,19 @@
         a
         0
 
         [ ((0, 'a'), (0, 'a')),
           ((1, 'b'), (0, '')),
           ((1, 'c'), (0, '')) ]
 
+    Test case # 11
+        # Sort of an insertion test (empty inputs are not allowed)
+
+    Test case # 12
+        # Verify that empty inputs are not allowed
     """
 
     def __init__(self, *args):
         # Let's use __init__() to set all these up just once at class creation
         # time, instead of setUp() which repeatedly does it for each test case
         super().__init__(*args)
         self.test_mapping_one = Mapping([{"in": "t", "out": "p", "context_after": "e"}])
@@ -276,23 +281,29 @@
         self.trans_feeding_2 = Transducer(self.test_feeding_mapping_2)
 
     def test_feeding(self):
         """Test feeding"""
         transducer_1 = self.trans_feeding_1("ab")
         self.assertEqual(transducer_1.output_string, "cd")
         self.assertEqual(transducer_1.edges, [(0, 0), (0, 1), (1, 0), (1, 1)])
+        # because of "crossed" indices, we get one single monotonic alignment
+        self.assertEqual(transducer_1.substring_alignments(), [("ab", "cd")])
         transducer_2 = self.trans_feeding_2("a")
         self.assertEqual(transducer_2.output_string, "b")
         self.assertEqual(transducer_2.edges, [(0, 0)])
+        self.assertEqual(transducer_2.substring_alignments(), [("a", "b")])
 
     def test_issue_157(self):
         """Test explicit problem from Issue 157"""
         transducer = self.trans_157("abcmn")
         self.assertEqual(transducer.output_string, "deNM")
         self.assertEqual(transducer.edges, [(0, 0), (1, 1), (2, 1), (3, 3), (4, 2)])
+        self.assertEqual(
+            transducer.substring_alignments(), [("a", "d"), ("bc", "e"), ("mn", "NM")]
+        )
 
     def test_issue_173(self):
         """Test explicit problems from Issue 173"""
         transducer_1 = self.trans_173_1("xyzmndef")
         transducer_2 = self.trans_173_2("xyzmndef")
         transducer_3 = self.trans_173_3("abc")
         transducer_4 = self.trans_173_4("abc")
@@ -301,19 +312,39 @@
         self.assertEqual(transducer_3.output_string, "XY")
         self.assertEqual(transducer_4.output_string, "xyz")
         self.assertEqual(
             transducer_1.edges,
             [(0, 1), (1, 0), (2, 0), (3, 2), (4, 3), (5, 4), (6, 5), (7, 6)],
         )
         self.assertEqual(
+            transducer_1.substring_alignments(),
+            [("xyz", "ab"), ("m", "m"), ("n", "n"), ("d", "d"), ("e", "e"), ("f", "f")],
+        )
+        self.assertEqual(
             transducer_2.edges,
             [(0, 0), (1, 1), (2, 1), (3, 2), (4, 3), (5, 4), (6, 5), (7, 6)],
         )
+        self.assertEqual(
+            transducer_2.substring_alignments(),
+            [
+                ("x", "a"),
+                ("yz", "b"),
+                ("m", "m"),
+                ("n", "n"),
+                ("d", "d"),
+                ("e", "e"),
+                ("f", "f"),
+            ],
+        )
         self.assertEqual(transducer_3.edges, [(0, 0), (1, 0), (2, 1)])
+        self.assertEqual(transducer_3.substring_alignments(), [("ab", "X"), ("c", "Y")])
         self.assertEqual(transducer_4.edges, [(0, 0), (0, 1), (1, 2), (2, 2)])
+        self.assertEqual(
+            transducer_4.substring_alignments(), [("a", "xy"), ("bc", "z")]
+        )
 
     def test_explicit_equal(self):
         """Test synonymous syntax for explicit indices"""
         explicit_1 = self.trans_explicit_equal_1("ab")
         explicit_2 = self.trans_explicit_equal_2("ab")
         explicit_3 = self.trans_explicit_equal_4("ab")
         implicit = self.trans_explicit_equal_3("ab")
@@ -342,99 +373,187 @@
         transducer_lite = self.trans_wacky_lite("abcc")
         transducer_lite_extra = self.trans_wacky_lite("abcca")
         self.assertEqual(transducer_lite.output_string, "ccccc")
         self.assertEqual(transducer_lite_extra.output_string, "ccccca")
         self.assertEqual(
             transducer_lite.edges, [(0, 4), (1, 0), (2, 1), (2, 2), (3, 3)]
         )
+        self.assertEqual(transducer_lite.substring_alignments(), [("abcc", "ccccc")])
         self.assertEqual(
             transducer_lite_extra.edges,
             [(0, 4), (1, 0), (2, 1), (2, 2), (3, 3), (4, 5)],
         )
+        self.assertEqual(
+            transducer_lite_extra.substring_alignments(),
+            [("abcc", "ccccc"), ("a", "a")],
+        )
         transducer_no_i = self.trans_wacky("\U0001f600\U0001f603\U0001f604\U0001f604")
         self.assertEqual(
             transducer_no_i.output_string,
             "\U0001f604\U0001f604\U0001f604\U0001f604\U0001f604",
         )
         transducer = self.trans_wacky("\U0001f600\U0001f603\U0001f604\U0001f604")
         self.assertEqual(
             transducer.output_string,
             "\U0001f604\U0001f604\U0001f604\U0001f604\U0001f604",
         )
         self.assertEqual(transducer.edges, [(0, 4), (1, 0), (2, 1), (2, 2), (3, 3)])
+        self.assertEqual(
+            transducer.substring_alignments(),
+            [
+                (
+                    "\U0001f600\U0001f603\U0001f604\U0001f604",
+                    "\U0001f604\U0001f604\U0001f604\U0001f604\U0001f604",
+                )
+            ],
+        )
 
     def test_circum(self):
         """Test circumfixing"""
         transducer = self.trans_circum("ac")
         self.assertEqual(transducer.output_string, "cac")
         self.assertEqual(transducer.edges, [(0, 1), (1, 0), (1, 2)])
+        self.assertEqual(transducer.substring_alignments(), [("ac", "cac")])
 
     def test_case_one(self):
         """Test case one"""
         transducer = self.trans_one("test")
         self.assertEqual(transducer.output_string, "pest")
         self.assertEqual(transducer.edges, [(0, 0), (1, 1), (2, 2), (3, 3)])
+        self.assertEqual(
+            transducer.substring_alignments(),
+            [("t", "p"), ("e", "e"), ("s", "s"), ("t", "t")],
+        )
+        transducer = self.trans_one("")
+        self.assertEqual(transducer.output_string, "")
+        self.assertEqual(transducer.edges, [])
+        self.assertEqual(transducer.substring_alignments(), [])
 
     def test_case_two(self):
         transducer = self.trans_two("test")
         self.assertEqual(transducer.output_string, "tst")
         self.assertEqual(transducer.edges, [(0, 0), (1, 0), (2, 1), (3, 2)])
+        self.assertEqual(
+            transducer.substring_alignments(), [("te", "t"), ("s", "s"), ("t", "t")]
+        )
 
     def test_case_three(self):
         transducer = self.trans_three("test")
         self.assertEqual(transducer.output_string, "chest")
         self.assertEqual(transducer.edges, [(0, 0), (0, 1), (1, 2), (2, 3), (3, 4)])
+        self.assertEqual(
+            transducer.substring_alignments(),
+            [("t", "ch"), ("e", "e"), ("s", "s"), ("t", "t")],
+        )
 
     def test_case_four(self):
         transducer = self.trans_four("test")
         self.assertEqual(transducer.output_string, "pst")
         self.assertEqual(transducer.edges, [(0, 0), (1, 0), (2, 1), (3, 2)])
+        self.assertEqual(
+            transducer.substring_alignments(), [("te", "p"), ("s", "s"), ("t", "t")]
+        )
 
     def test_case_six(self):
         transducer = self.trans_six("test")
         self.assertEqual(transducer.output_string, "tset")
         self.assertEqual(transducer.edges, [(0, 0), (1, 2), (2, 1), (3, 3)])
+        self.assertEqual(
+            transducer.substring_alignments(), [("t", "t"), ("es", "se"), ("t", "t")]
+        )
 
     def test_case_long_six(self):
         transducer = self.trans_six("esesse")
         self.assertEqual(transducer.output_string, "sesese")
+        # Ensure that *minimal* monotonic segments are output
+        self.assertEqual(
+            transducer.substring_alignments(),
+            [("es", "se"), ("es", "se"), ("s", "s"), ("e", "e")],
+        )
 
     def test_case_seven(self):
         transducer_as_written = self.test_seven_as_written("test")
         self.assertEqual(transducer_as_written.output_string, "test")
         self.assertEqual(transducer_as_written.edges, [(0, 0), (1, 1), (2, 2), (3, 3)])
+        self.assertEqual(
+            transducer_as_written.substring_alignments(),
+            [("t", "t"), ("e", "e"), ("s", "s"), ("t", "t")],
+        )
         transducer = self.trans_seven("test")
         self.assertEqual(transducer.output_string, "tesht")
         self.assertEqual(transducer.edges, [(0, 0), (1, 1), (2, 2), (2, 3), (3, 4)])
+        self.assertEqual(
+            transducer.substring_alignments(),
+            [("t", "t"), ("e", "e"), ("s", "sh"), ("t", "t")],
+        )
 
     def test_case_eight(self):
         transducer = self.trans_eight("test")
         self.assertEqual(transducer.output_string, "chess")
         self.assertEqual(transducer.edges, [(0, 0), (1, 1), (1, 2), (2, 3), (3, 4)])
+        self.assertEqual(
+            transducer.substring_alignments(),
+            [("t", "c"), ("e", "he"), ("s", "s"), ("t", "s")],
+        )
 
     def test_case_nine(self):
         transducer = self.trans_nine("aa")
         self.assertEqual(transducer.output_string, "")
         self.assertEqual(transducer.edges, [(0, None), (1, None)])
+        # Support deletions in substring_alignments
+        self.assertEqual(transducer.substring_alignments(), [("aa", "")])
+        transducer = self.trans_nine("aabbaab")
+        self.assertEqual(transducer.output_string, "bbb")
+        self.assertEqual(
+            transducer.edges,
+            [(0, 0), (1, 0), (2, 0), (3, 1), (4, 1), (5, 1), (6, 2)],
+        )
+        # Support deletions in substring_alignments.  NOTE: these
+        # alignments are quite bogus due to the ad-hoc treatment of
+        # deletions by rule-based mappings
+        self.assertEqual(
+            transducer.substring_alignments(),
+            [("aab", "b"), ("baa", "b"), ("b", "b")],
+        )
 
     def test_case_ten(self):
         transducer = self.trans_ten("abc")
         self.assertEqual(transducer.output_string, "a")
         self.assertEqual(transducer.edges, [(0, 0), (1, 0), (2, 0)])
+        self.assertEqual(transducer.substring_alignments(), [("abc", "a")])
 
     def test_case_eleven(self):
         transducer = self.trans_eleven("a")
         self.assertEqual(transducer.output_string, "aaaa")
         self.assertEqual(transducer.edges, [(0, 0), (0, 1), (0, 2), (0, 3)])
+        self.assertEqual(transducer.substring_alignments(), [("a", "aaaa")])
+
+    def test_case_twelve(self):
+        # Empty inputs are not allowed (should it actually throw an exception?)
+        with self.assertLogs() as cm:
+            self.test_mapping_twelve = Mapping(
+                [{"in": "", "out": "aa", "context_before": "b"}]
+            )
+            self.trans_twelve = Transducer(self.test_mapping_twelve)
+            transducer = self.trans_twelve("b")
+        self.assertIn(
+            "disallowed",
+            cm.output[0],
+            "it should warn that empty inputs are disallowed",
+        )
+        self.assertEqual(transducer.output_string, "b")
 
     def test_case_acdc(self):
         transducer = Transducer(Mapping([{"in": "a{1}c{2}", "out": "c{2}a{1}c{2}"}]))
         tg = transducer("acdc")
         self.assertEqual(tg.output_string, "cacdc")
         self.assertEqual(tg.edges, [(0, 1), (1, 0), (1, 2), (2, 3), (3, 4)])
+        self.assertEqual(
+            tg.substring_alignments(), [("ac", "cac"), ("d", "d"), ("c", "c")]
+        )
 
     def test_case_acac(self):
         transducer = Transducer(Mapping([{"in": "ab{1}c{2}", "out": "ab{2}"}]))
         transducer_default = Transducer(
             Mapping([{"in": "ab", "out": ""}, {"in": "c", "out": "ab"}])
         )
         tg = transducer("abcabc")
@@ -448,14 +567,15 @@
                 (2, 1),
                 (3, 1),
                 (4, 1),
                 (5, 2),
                 (5, 3),
             ],
         )
+        self.assertEqual(tg.substring_alignments(), [("abcab", "ab"), ("c", "ab")])
         tg_default = transducer_default("abcabc")
         self.assertEqual(tg_default.output_string, "abab")
         self.assertEqual(
             tg_default.edges,
             [
                 (0, 0),
                 (1, 0),
@@ -463,14 +583,17 @@
                 (2, 1),
                 (3, 1),
                 (4, 1),
                 (5, 2),
                 (5, 3),
             ],
         )
+        self.assertEqual(
+            tg_default.substring_alignments(), [("abcab", "ab"), ("c", "ab")]
+        )
 
     def test_arpabet(self):
         transducer = Transducer(
             Mapping([{"in": "ĩ", "out": "IY N"}], norm_form="NFC", out_delimiter=" ")
         )
         transducer_nfd = Transducer(
             Mapping([{"in": "ĩ", "out": "IY N"}], norm_form="NFD", out_delimiter=" ")
@@ -490,14 +613,15 @@
                 (1, 5),
                 (1, 6),
                 (1, 7),
                 (1, 8),
                 (1, 9),
             ],
         )
+        self.assertEqual(tg.substring_alignments(), [("ĩ", "IY N "), ("ĩ", "IY N ")])
         self.assertEqual(
             tg_nfd.edges,
             [
                 (0, 0),
                 (1, 1),
                 (1, 2),
                 (1, 3),
@@ -505,11 +629,15 @@
                 (2, 5),
                 (3, 6),
                 (3, 7),
                 (3, 8),
                 (3, 9),
             ],
         )
+        self.assertEqual(
+            tg_nfd.substring_alignments(),
+            [("i", "I"), ("̃", "Y N "), ("i", "I"), ("̃", "Y N ")],
+        )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `g2p-1.0.20230228/g2p/tests/test_langs.py` & `g2p-1.0.20230412/g2p/tests/test_langs.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
         # Then we call assertEqual on the first failed case, to make unittest register the failure.
         error_count = 0
         for test in langs_to_test:
             transducer = make_g2p(test[0], test[1])
             output_string = transducer(test[2]).output_string.strip()
             if output_string != test[3].strip():
                 LOGGER.warning(
-                    "test_langs.py: mapping error: {} from {} to {} should be {}, got {}".format(
-                        test[2], test[0], test[1], test[3], output_string
+                    "test_langs.py: mapping error for {}: {} from {} to {} should be {}, got {}".format(
+                        test[-1], test[2], test[0], test[1], test[3], output_string
                     )
                 )
                 if error_count == 0:
                     first_failed_test = test
                 error_count += 1
 
         if error_count > 0:
```

### Comparing `g2p-1.0.20230228/g2p/tests/test_mappings.py` & `g2p-1.0.20230412/g2p/tests/test_mappings.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import unicodedata as ud
 from contextlib import redirect_stderr
 from tempfile import NamedTemporaryFile
 from typing import List
 from unittest import TestCase, main
 
 from g2p import exceptions
+from g2p.log import LOGGER
 from g2p.mappings import Mapping
 from g2p.tests.public import __file__ as public_data
 from g2p.transducer import Transducer
 
 
 def rules_from_strings(*mapping: str) -> List[dict]:
     """Quick pseudo constructor for unit testing of mappings"""
@@ -239,24 +240,32 @@
         self.assertEqual(mapping.kwargs["rule_ordering"], "apply-longest-first")
         self.assertFalse(mapping.kwargs["case_sensitive"])
         self.assertTrue(mapping.kwargs["escape_special"])
         self.assertEqual(mapping.kwargs["norm_form"], "NFD")
         self.assertTrue(mapping.kwargs["reverse"])
 
     def test_null_input(self):
-        mapping = Mapping([{"in": "", "out": "a"}])
+        with self.assertLogs(LOGGER, level="WARNING"):
+            mapping = Mapping([{"in": "", "out": "a"}])
         self.assertFalse(mapping())
 
     def test_no_escape(self):
         mapping = Mapping(
             os.path.join(os.path.dirname(public_data), "mappings", "no_escape.csv")
         )
         transducer = Transducer(mapping)
         self.assertEqual(transducer("?").output_string, "ʔ")
 
+    def test_invalid_regex(self):
+        rules = [{"in": "fo(o", "out": "bar"}]
+        with self.assertLogs(LOGGER, level="ERROR"):
+            with self.assertRaises(exceptions.MalformedMapping) as cm:
+                _ = Mapping(rules)
+        self.assertIn("regex", cm.exception.message)
+
     def test_invalid_rules_json(self):
         rules = [{"in": "a"}, {"out": "c"}]
         self.assertRaises(exceptions.MalformedMapping, Mapping, rules)
 
     def test_invalid_rules_csv(self):
         tf = NamedTemporaryFile(
             prefix="test_invalid_rules_", mode="w", suffix=".csv", delete=False
@@ -278,24 +287,25 @@
     def test_extend_and_deduplicate(self):
         mapping1 = Mapping(rules_from_strings("a:b", "c:d", "g:h"))
         mapping2 = Mapping(rules_from_strings("a:x", "c:d", "e:f"))
         extend_ref = Mapping(
             rules_from_strings("a:b", "c:d", "g:h", "a:x", "c:d", "e:f")
         )
         mapping1.extend(mapping2)
-        self.assertEquals(mapping1.mapping, extend_ref.mapping)
+        self.assertEqual(mapping1.mapping, extend_ref.mapping)
         dedup_ref = Mapping(rules_from_strings("a:b", "c:d", "g:h", "a:x", "e:f"))
         mapping1.deduplicate()
-        self.assertEquals(mapping1.mapping, dedup_ref.mapping)
+        self.assertEqual(mapping1.mapping, dedup_ref.mapping)
 
     def test_g2p_studio_csv(self):
         # Ensure that a single CSV file from Studio works properly
-        mapping = Mapping(
-            os.path.join(os.path.dirname(public_data), "mappings", "g2p_studio.csv")
-        )
+        with self.assertLogs(LOGGER, level="WARNING"):  # silence "" input warnings
+            mapping = Mapping(
+                os.path.join(os.path.dirname(public_data), "mappings", "g2p_studio.csv")
+            )
         transducer = Transducer(mapping)
         self.assertEqual(
             transducer("Jouni haluaa juoda kahvia").output_string,
             "Jouni hɑluɑː juodɑ kɑhviɑ",
         )
         # Concatenate them (this is not a good idea) and make sure it works anyway
         tf = NamedTemporaryFile(
@@ -314,15 +324,16 @@
         tf.write("\n")
         with open(
             os.path.join(os.path.dirname(public_data), "mappings", "g2p_studio2.csv"),
             encoding="utf8",
         ) as fh:
             tf.write(fh.read())
         tf.close()
-        mapping = Mapping(tf.name)
+        with self.assertLogs(LOGGER, level="WARNING"):  # silence "" input warnings
+            mapping = Mapping(tf.name)
         transducer = Transducer(mapping)
         self.assertEqual(
             transducer("tee on herkullista").output_string, "teː on herkullistɑ"
         )
         os.unlink(tf.name)
```

### Comparing `g2p-1.0.20230228/g2p/tests/test_network.py` & `g2p-1.0.20230412/g2p/tests/test_network.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 #!/usr/bin/env python
 
 from unittest import TestCase, main
 
 from g2p import make_g2p
 from g2p.exceptions import InvalidLanguageCode, NoPath
+from g2p.log import LOGGER
 from g2p.transducer import CompositeTransducer, Transducer
 
 
 class NetworkTest(TestCase):
     """Basic Test for available networks"""
 
     def setUp(self):
         pass
 
     def test_not_found(self):
         with self.assertRaises(InvalidLanguageCode):
-            make_g2p("foo", "eng-ipa")
+            with self.assertLogs(LOGGER, level="ERROR"):
+                make_g2p("foo", "eng-ipa")
         with self.assertRaises(InvalidLanguageCode):
-            make_g2p("git", "bar")
+            with self.assertLogs(LOGGER, level="ERROR"):
+                make_g2p("git", "bar")
 
     def test_no_path(self):
-        with self.assertRaises(NoPath):
+        with self.assertRaises(NoPath), self.assertLogs(LOGGER, level="ERROR"):
             make_g2p("hei", "git")
 
     def test_valid_composite(self):
         transducer = make_g2p("atj", "eng-ipa")
         self.assertTrue(isinstance(transducer, CompositeTransducer))
         self.assertEqual("niɡiɡw", transducer("nikikw").output_string)
```

### Comparing `g2p-1.0.20230228/g2p/tests/test_studio.py` & `g2p-1.0.20230412/g2p/tests/test_studio.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,26 +39,52 @@
     def test_socket_connection(self):
         self.assertTrue(self.socketio_test_client.is_connected())
 
     async def test_sanity(self):
         async with async_playwright() as p:
             browser = await p.chromium.launch(channel="chrome", headless=True)
             page = await browser.new_page()
+            await page.goto(f"http://localhost:{self.port}/docs")
+            await page.wait_for_timeout(1000)
             await page.goto(f"http://localhost:{self.port}")
             await page.wait_for_timeout(1000)
             input_el = page.locator("#input")
             output_el = page.locator("#output")
             await page.type("#input", "hello world")
             await page.wait_for_timeout(1000)
             input_text = await input_el.input_value()
             output_text = await output_el.input_value()
             self.assertEqual(input_text, output_text)
             self.assertEqual(input_text, "hello world")
             await input_el.fill("")
             await output_el.fill("")
+            await page.type("#input", "hello world")
+            await page.wait_for_timeout(1000)
+            radio_el = page.locator("#animated-radio")
+            await radio_el.click()
+            await page.wait_for_timeout(1000)
+
+    async def test_switch_langs(self):
+        async with async_playwright() as p:
+            browser = await p.chromium.launch(channel="chrome", headless=True)
+            page = await browser.new_page()
+            await page.goto(f"http://localhost:{self.port}")
+            await page.wait_for_timeout(1000)
+            in_lang_selector = page.locator("#input-langselect")
+            # Switch to a language
+            await in_lang_selector.select_option(value="alq")
+            await page.wait_for_timeout(1000)
+            settings_title = await page.text_content("#link-0")
+            self.assertEqual(settings_title, "Algonquin to IPA")
+            # Switch back to custom
+            await in_lang_selector.select_option(value="Custom")
+            await page.wait_for_timeout(1000)
+            settings_title = await page.text_content("#link-0")
+            self.assertEqual(settings_title, "Custom")
+            # FIXME: Test that the table works somewhere, somehow
 
     async def test_langs(self):
 
         langs_to_test = load_public_test_data()
         error_count = 0
 
         # The current g2p-studio app leaks memory, so that if we try to run all the test
```

### Comparing `g2p-1.0.20230228/g2p/tests/test_tokenize_and_map.py` & `g2p-1.0.20230412/g2p/tests/test_tokenize_and_map.py`

 * *Files 22% similar despite different names*

```diff
@@ -34,14 +34,17 @@
             tokenizer, transducer, self.contextualize("sq")
         )
         self.assertEqual(string_ipa, self.contextualize(word_ipa))
 
     def test_tokenizing_transducer(self):
         ref_word_ipa = g2p.make_g2p("mic", "mic-ipa")("sq").output_string
         transducer = g2p.make_g2p("mic", "mic-ipa", tok_lang="mic")
+        self.assertEqual(transducer.transducer.in_lang, transducer.in_lang)
+        self.assertEqual(transducer.transducer.out_lang, transducer.out_lang)
+        self.assertEqual(transducer.transducer, transducer.transducers[0])
         word_ipa = transducer("sq").output_string
         self.assertEqual(word_ipa, ref_word_ipa)
         string_ipa = transducer(self.contextualize("sq")).output_string
         self.assertEqual(string_ipa, self.contextualize(ref_word_ipa))
 
     def test_tokenizing_transducer_chain(self):
         transducer = g2p.make_g2p("fra", "eng-arpabet", tok_lang="fra")
@@ -53,47 +56,100 @@
     def test_tokenizing_transducer_debugger(self):
         transducer = g2p.make_g2p("fra", "fra-ipa", tok_lang="fra")
         debugger = transducer("ceci est un test.").debugger
         self.assertEqual(len(debugger), 4)
 
     def test_tokenizing_transducer_edges(self):
         transducer = g2p.make_g2p("fra", "fra-ipa", tok_lang="fra")
-        edges = transducer("est est").edges
+        tg = transducer("est est")
         # est -> ɛ, so edges are (0, 0), (1, 0), (2, 0) for each "est", plus the
         # space to the space, and the second set of edges being offset
         ref_edges = [(0, 0), (1, 0), (2, 0), (3, 1), (4, 2), (5, 2), (6, 2)]
-        self.assertEqual(edges, ref_edges)
+        self.assertEqual(tg.edges, ref_edges)
+        ref_alignments = [("est", "ɛ"), (" ", " "), ("est", "ɛ")]
+        self.assertEqual(tg.substring_alignments(), ref_alignments)
 
     def test_tokenizing_transducer_edges2(self):
         ref_edges = g2p.make_g2p("fra", "fra-ipa")("ça ça").edges
         edges = g2p.make_g2p("fra", "fra-ipa", tok_lang="fra")("ça ça").edges
         self.assertEqual(edges, ref_edges)
 
     def test_tokenizing_transducer_edge_chain(self):
         transducer = g2p.make_g2p("fra", "eng-arpabet", tok_lang="fra")
-        edges = transducer("est est").edges
+        # .edges on a transducer is always a single array with the
+        # end-to-end mapping, for a composed transducer we can access
+        # the individual tiers with .tiers
         ref_edges = [
+            # "est est" -> "EH  EH "
+            # est -> EH
+            (0, 0),
+            (0, 1),
+            (0, 2),
+            (1, 0),
+            (1, 1),
+            (1, 2),
+            (2, 0),
+            (2, 1),
+            (2, 2),
+            # space -> space
+            (3, 3),
+            # est -> EH
+            (4, 4),
+            (4, 5),
+            (4, 6),
+            (5, 4),
+            (5, 5),
+            (5, 6),
+            (6, 4),
+            (6, 5),
+            (6, 6),
+        ]
+        tg = transducer("est est")
+        self.assertEqual(tg.alignments(), ref_edges)
+        ref_alignments = [("est", "EH "), (" ", " "), ("est", "EH ")]
+        self.assertEqual(tg.substring_alignments(), ref_alignments)
+
+        tier_edges = [x.edges for x in tg.tiers]
+        ref_tier_edges = [
             # "est est" -> "ɛ ɛ"
             [(0, 0), (1, 0), (2, 0), (3, 1), (4, 2), (5, 2), (6, 2)],
             # "ɛ ɛ" -> "ɛ ɛ"
             [(0, 0), (1, 1), (2, 2)],
             # "ɛ ɛ" -> "EH  EH "
             [(0, 0), (0, 1), (0, 2), (1, 3), (2, 4), (2, 5), (2, 6)],
         ]
-        self.assertEqual(edges, ref_edges)
+        self.assertEqual(tier_edges, ref_tier_edges)
+        tier_alignments = [x.substring_alignments() for x in tg.tiers]
+        ref_tier_alignments = [
+            [("est", "ɛ"), (" ", " "), ("est", "ɛ")],
+            [("ɛ", "ɛ"), (" ", " "), ("ɛ", "ɛ")],
+            [("ɛ", "EH "), (" ", " "), ("ɛ", "EH ")],
+        ]
+        self.assertEqual(tier_alignments, ref_tier_alignments)
 
     def test_tokenizing_transducer_edge_spaces(self):
         transducer = g2p.make_g2p("fra", "eng-arpabet", tok_lang="fra")
-        edges = transducer("  a, ").edges
         ref_edges = [
+            # "  a, " -> "  AA , "
+            (0, 0),
+            (1, 1),
+            (2, 2),
+            (2, 3),
+            (2, 4),
+            (3, 5),
+            (4, 6),
+        ]
+        self.assertEqual(transducer("  a, ").alignments(), ref_edges)
+        tier_edges = [x.edges for x in transducer("  a, ").tiers]
+        ref_tier_edges = [
             # "  a, " -> "  a, "
             [(0, 0), (1, 1), (2, 2), (3, 3), (4, 4)],
             # "  a, " -> "  ɑ, "
             [(0, 0), (1, 1), (2, 2), (3, 3), (4, 4)],
             # "  ɑ, " -> "  AA , "
             [(0, 0), (1, 1), (2, 2), (2, 3), (2, 4), (3, 5), (4, 6)],
         ]
-        self.assertEqual(edges, ref_edges)
+        self.assertEqual(tier_edges, ref_tier_edges)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `g2p-1.0.20230228/g2p/tests/test_tokenizer.py` & `g2p-1.0.20230412/g2p/tests/test_tokenizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,22 +73,24 @@
         self.assertEqual(len(tokens), 1)
         self.assertTrue(tokens[0]["is_word"])
         self.assertEqual(tokens[0]["text"], "ts'nj")
 
     def test_tokenize_tce_equiv(self):
         input = "ts'e ts`e ts‘e ts’"
         self.assertEqual(len(tok.make_tokenizer("fra").tokenize_text(input)), 14)
-        tce_tokens = tok.make_tokenizer("tce").tokenize_text(input)
+        # tce_tokens = tok.make_tokenizer("tce").tokenize_text(input)
         # LOGGER.warning([x["text"] for x in tce_tokens])
         self.assertEqual(len(tok.make_tokenizer("tce").tokenize_text(input)), 7)
 
     def test_tokenizer_identity_tce(self):
         self.assertNotEqual(tok.make_tokenizer("eng"), tok.make_tokenizer("fra"))
         self.assertNotEqual(tok.make_tokenizer("eng"), tok.make_tokenizer("tce"))
-        self.assertEqual(tok.make_tokenizer("eng"), tok.make_tokenizer())
+        self.assertEqual(tok.make_tokenizer("tce"), tok.make_tokenizer("tce"))
+        self.assertNotEqual(tok.make_tokenizer("tce"), tok.make_tokenizer())
+        self.assertEqual(tok.make_tokenizer("foo"), tok.make_tokenizer())
 
     def test_tokenize_kwk(self):
         """kwk is easier than tce: we just need to use kwk-umista -> kwk-ipa, but that's not
         implemented yet.
         Now works - issue #46 fixed this.
         """
         self.assertEqual(
@@ -109,17 +111,18 @@
 
     def test_tokenize_not_ipa_implicit(self):
         tokenizer = tok.make_tokenizer("fn-unicode-font")
         self.assertNotEqual(tokenizer, tok.make_tokenizer())
 
     def test_tokenize_lang_does_not_exit(self):
         self.assertEqual(tok.make_tokenizer("not_a_language"), tok.make_tokenizer())
-        self.assertEqual(
-            tok.make_tokenizer("fra", "not_a_language"), tok.make_tokenizer()
-        )
+        with self.assertLogs():
+            self.assertEqual(
+                tok.make_tokenizer("fra", "not_a_language"), tok.make_tokenizer()
+            )
 
     def test_make_tokenizer_error(self):
         with self.assertRaises(ValueError):
             _ = tok.make_tokenizer("fra", "eng-arpabet", ["fra-ipa", "eng-ipa"])
 
     def test_deprecated_warning(self):
         with self.assertLogs(LOGGER, level="WARNING") as cm:
```

### Comparing `g2p-1.0.20230228/g2p/tests/test_unidecode_transducer.py` & `g2p-1.0.20230412/g2p/tests/test_unidecode_transducer.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,16 +45,25 @@
         transducer = make_g2p("und", "eng-arpabet")
         tg = transducer("السلام عليكم")
         self.assertEqual(tg.output_string, "L S L M  L Y K M ")
 
     def test_unidecode_arabic_presentation_to_arpabet(self):
         transducer = make_g2p("und", "eng-arpabet")
         tg = transducer("ﺷﻜﺮﺍﹰ")
-        self.assertEqual(tg.output_string, "S HH K D  AA N ")
+        self.assertEqual(tg.output_string, "S HH K D AA N ")
 
     def test_unidecode_kanji_to_arpabet(self):
         transducer = make_g2p("und", "eng-arpabet")
         tg = transducer("日本語")
-        self.assertEqual(tg.output_string, "D IY  B EY N  Y UW  ")
+        self.assertEqual(tg.output_string, "D IY B EY N Y UW ")
+
+    def test_unidecode_hanzi_to_arpabet(self):
+        transducer = make_g2p("und", "eng-arpabet")
+        tg = transducer("你们好!你们说汉语马?")
+        self.assertEqual(
+            tg.output_string,
+            "N IY M EY N HH AA OW N IY M EY N S HH UW OW Y IY Y UW M AA HH ",
+        )
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `g2p-1.0.20230228/g2p/tests/test_utils.py` & `g2p-1.0.20230412/g2p/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import os
 from collections import defaultdict
 from unittest import TestCase, main
 
 import yaml
 
 from g2p.exceptions import IncorrectFileType, MalformedMapping, RecursionError
+from g2p.log import LOGGER
 from g2p.mappings import Mapping, utils
 from g2p.tests.public import PUBLIC_DIR
 
 
 class UtilsTest(TestCase):
     def setUp(self):
         pass
@@ -107,15 +108,15 @@
         self.assertEqual(minimal["mapping_data"], json["mapping_data"])
         self.assertEqual(minimal["mapping_data"], xlsx["mapping_data"])
 
     def test_validate(self):
         pass
 
     def test_escape_special(self):
-        self.assertEqual(utils.escape_special_characters({"in": "?"}), {"in": "\?"})
+        self.assertEqual(utils.escape_special_characters({"in": "?"}), {"in": "\\?"})
 
     def test_load_abbs(self):
         with self.assertRaises(IncorrectFileType):
             utils.load_abbreviations_from_file(
                 os.path.join(PUBLIC_DIR, "mappings", "abbreviations.json")
             )
         for abb in ["abbreviations.csv", "abbreviations.tsv", "abbreviations.psv"]:
@@ -130,18 +131,22 @@
             "in_lang": "test",
             "out_lang": "test-out",
             "rule_ordering": "apply-longest-first",
         }
         # config = utils.generate_config('test', 'test-out', 'Test', 'TestOut')
         config["mapping"] = [{"in": "a", "out": "b"}]
         mapping = Mapping(**config)
-        mapping.config_to_file(os.path.join(PUBLIC_DIR, "mappings", "test_config.yaml"))
-        mapping.config_to_file(
-            os.path.join(PUBLIC_DIR, "mappings", "generated_add.yaml")
-        )
+        with self.assertLogs(LOGGER, level="WARNING"):
+            mapping.config_to_file(
+                os.path.join(PUBLIC_DIR, "mappings", "test_config.yaml")
+            )
+        with self.assertLogs(LOGGER, level="WARNING"):
+            mapping.config_to_file(
+                os.path.join(PUBLIC_DIR, "mappings", "generated_add.yaml")
+            )
         mapping.mapping_to_file(os.path.join(PUBLIC_DIR, "mappings"))
         test_config = utils.load_mapping_from_path(
             os.path.join(PUBLIC_DIR, "mappings", "test_config.yaml")
         )
         test_config_added = utils.load_mapping_from_path(
             os.path.join(PUBLIC_DIR, "mappings", "generated_add.yaml")
         )
```

### Comparing `g2p-1.0.20230228/g2p/tests/test_z_local_config.py` & `g2p-1.0.20230412/g2p/tests/test_z_local_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,21 +216,21 @@
         result = self.runner.invoke(
             convert,
             [normalize("é", "NFD"), "c1", "c3", "--config", config_path, "-d", "-e"],
         )
         self.assertEqual(result.exit_code, 0)
         self.assertIn("[[(0, 0), (1, 0)], [(0, 0), (0, 1)]]", result.output)
         self.assertIn(
-            "[[['e', 'ò'], ['́', 'ò']], [['ò', 'u'], ['ò', '̀']]]", result.output
+            "[[('e', 'ò'), ('́', 'ò')], [('ò', 'u'), ('ò', '̀')]]", result.output
         )
 
         result = self.runner.invoke(
             convert,
             [normalize("é", "NFC"), "c1", "c3", "--config", config_path, "-d", "-e"],
         )
         self.assertEqual(result.exit_code, 0)
         self.assertIn("[[(0, 0)], [(0, 0), (0, 1)]]", result.output)
-        self.assertIn("[[['é', 'ò']], [['ò', 'u'], ['ò', '̀']]]", result.output)
+        self.assertIn("[[('é', 'ò')], [('ò', 'u'), ('ò', '̀')]]", result.output)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `g2p-1.0.20230228/g2p/tests/time_panphon.py` & `g2p-1.0.20230412/g2p/tests/time_panphon.py`

 * *Files identical despite different names*

### Comparing `g2p-1.0.20230228/g2p/transducer/__init__.py` & `g2p-1.0.20230412/g2p/transducer/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 """
 This module contains the Transducer and CompositeTransducer classes
 which are responsible for performing transductions in the g2p library.
 """
 
 import copy
 import re
-from collections import defaultdict
-from typing import Dict, List
 import unicodedata
+from collections import OrderedDict, defaultdict
+from typing import Dict, List, Optional, Set, Tuple, Union
 
 import text_unidecode
 
 from g2p.log import LOGGER
 from g2p.mappings import Mapping
 from g2p.mappings.langs.utils import is_arpabet, is_panphon
 from g2p.mappings.tokenizer import DefaultTokenizer
@@ -38,126 +38,338 @@
 # The first item (int) in a change is the index of where the change occurs, and
 # the second item (int) is the change offset
 # Example:
 # an insertion of length 1 at index 0 followed by a deletion of length one at index 2
 # [[0,1],[2,-1]]
 ChangeLog = List[List[int]]
 
-UNIDECODE_SPECIALS = ["@", "?", "'", ",", ":", " "]
+UNIDECODE_SPECIALS = ["@", "?", "'", ",", ":"]
+
+
+def normalize_edges(
+    edges: List[Tuple[int, Optional[int]]]
+) -> List[Tuple[int, Optional[int]]]:
+    """Normalize and sort a list of edges.
+
+    Specifically, this:
+
+    - Removes any non-deletion edges with the same input index as a deletion
+    - Resolves all deletions to map the outputs to the previous index if possible,
+      the following index if possible, or otherwise None (in practice this means
+      that None only occurs if the output is empty)
+    - Sorts edges based on the input and suppresses duplicates
+    """
+    to_remove: Set[int] = set()
+    for i, edge in enumerate(edges):
+        if edge[1] is None:
+            for j, other_edge in enumerate(edges):
+                if other_edge != edge and other_edge[0] == edge[0]:
+                    to_remove.add(j)
+    edges = [edge for i, edge in enumerate(edges) if i not in to_remove]
+    # sort based on inputs
+    edges.sort(key=lambda x: x[0])
+    for i, edge in enumerate(edges):
+        if edge[1] is None:
+            # if previous exists, use that, otherwise use following, otherwise None
+            previous = [x for x in edges[:i] if x[1] is not None]
+            # Note: if len(edges) == 1, edges[1:] is empty, not an IndexError
+            following = [x for x in edges[i + 1 :] if x[1] is not None]
+            if previous:
+                edges[i] = (edge[0], previous[-1][1])
+            elif following:
+                edges[i] = (edge[0], following[0][1])
+    # uniquify preserving order
+    return list(OrderedDict.fromkeys((i, j) for i, j in edges))
 
-def sanitize_unidecode_output(s: str) -> bool:
-    return "".join(c if c.isalpha() or c in UNIDECODE_SPECIALS else "" for c in s)
 
 class TransductionGraph:
     """This is the object returned after performing a transduction using a Transducer.
 
     Each TransductionGraph must be initialized with an input string.
     """
 
     def __init__(self, input_string: str):
         # Plain strings
         self._input_string = input_string
         self._output_string = input_string
         # Nodes
-        self._input_nodes = [[i, x] for i, x in enumerate(input_string)]
-        self._output_nodes = [[i, x] for i, x in enumerate(input_string)]
+        self._input_nodes: List[Tuple[int, str]] = list(enumerate(input_string))
+        self._output_nodes: List[Tuple[int, str]] = list(enumerate(input_string))
         # Edges
-        self._edges = [[i, i] for i, x in enumerate(input_string)]
+        self._edges: List[Tuple[int, Optional[int]]] = [
+            (i, i) for i in range(len(input_string))
+        ]
         # Debugger
         self._debugger = []  # type: ignore
 
     def __str__(self):
         return self._output_string
 
     @property
-    def input_string(self):
-        """str: The input string that initialized the TransductionGraph."""
+    def input_string(self) -> str:
+        """The input string that initialized the TransductionGraph."""
         return self._input_string
 
     @input_string.setter
     def input_string(self, value):
         # Only modify this if you're also adjusting the edges at the same time!
         self._input_string = value
-        self._input_nodes = [[i, x] for i, x in enumerate(value)]
+        self._input_nodes = list(enumerate(value))
 
     @property
-    def output_string(self):
+    def output_string(self) -> str:
         """str: The output string."""
         return self._output_string
 
     @output_string.setter
     def output_string(self, value):
         self._output_string = value
-        self._output_nodes = [[i, x] for i, x in enumerate(value)]
+        self._output_nodes = list(enumerate(value))
 
     @property
-    def input_nodes(self):
-        """List[List[int, str]]: A list of nodes (index and character string) corresponding to the input"""
+    def input_nodes(self) -> List[Tuple[int, str]]:
+        """List of nodes (index and character string) corresponding to the input"""
         return self._input_nodes
 
     @input_nodes.setter
     def input_nodes(self, value):
         raise ValueError(
             f"Sorry, you tried to change the input nodes to {value} but they cannot be changed."
         )
 
     @property
-    def output_nodes(self):
-        """List[List[int, str]]: A list of nodes (index and character string) corresponding to the output"""
+    def output_nodes(self) -> List[Tuple[int, str]]:
+        """List of nodes (index and character string) corresponding to the output"""
         return self._output_nodes
 
     @output_nodes.setter
     def output_nodes(self, value):
         raise ValueError(
             f"Sorry, you tried to change the output nodes to {value} but they cannot be changed directly. Change output_string instead."
         )
 
     @property
-    def edges(self):
-        """List[List[int, int]]: A list of edges (input node index, output node index) corresponding to the indices of the transformation"""
+    def edges(self) -> List:
+        """List[Tuple[int, Optional[int]]] of edges for the transformation.
+
+        Note that currently this is *not* the same between
+        TransductionGraph and CompositeTransductionGraph.
+        """
         return self._edges
 
     @edges.setter
     def edges(self, value):
         self._edges = value
 
     @property
-    def debugger(self):
-        """List[dict]: A list of lists of rules applied during the transformation. Useful for debugging."""
+    def debugger(self) -> List[list]:
+        """List[List[dict]]: A list of lists of rules applied during the
+        transformation. Useful for debugging.
+
+        Note that currently this is *not* the same between TransductionGraph
+        and CompositeTransductionGraph.
+
+        """
         return self._debugger
 
     @debugger.setter
     def debugger(self, value):
         self._debugger = value
 
     @property
-    def tiers(self):
-        """List[TransductionGraph]: A list of TransductionGraph objects for each tier in the graph"""
-        return self
+    def tiers(self) -> List["TransductionGraph"]:  # noqa: F821
+        """A list of TransductionGraph objects for each tier in the graph
+        (there is one tier)."""
+        return [self]
 
     @tiers.setter
     def tiers(self, value):
         raise ValueError(
             f"Sorry, you tried to change the tiers to {value} but they cannot be changed"
         )
 
     def pretty_edges(self):
-        edges = copy.deepcopy(self._edges)
+        """List[Tuple[str, str]] of edges resolved to the string nodes.
+
+        Note that this currently *not* the same output between
+        TransductionGraph and ComposedTransductionGraph.
+        """
+        edges = self._edges[:]
         edges.sort(key=lambda x: x[0])
-        for i, edge in enumerate(edges):
+        out_edges = []
+        for edge in edges:
+            assert edge[0] is not None  # Empty inputs are not allowed
             if edge[1] is None:
-                edges[i] = [self._input_nodes[edge[0]][1], None]
+                out_edges.append((self._input_nodes[edge[0]][1], None))
             else:
-                edges[i] = [
-                    self._input_nodes[edge[0]][1],
-                    self._output_nodes[edge[1]][1],
-                ]
-        return edges
+                out_edges.append(
+                    (
+                        self._input_nodes[edge[0]][1],
+                        self._output_nodes[edge[1]][1],
+                    )
+                )
+        return out_edges
 
-    def as_dict(self):
+    def alignments(self) -> List[Tuple[int, Optional[int]]]:
+        """Alignments (input node index, output node index) for the full
+        (possibly composed) transduction.
+
+        Insertions are not allowed in rules, but deletions are.  In
+        most cases they will *not* be represented as `None` in the
+        output node index, except in the case where there is a
+        deletion and the output string is empty.
+
+        Nonetheless code must be robust to the possibility of `None`
+        occurring as the output of an alignment.
+
+        Note that this method *is* compatible between TransductionGraph
+        and CompositeTransductionGraph.
+
+        """
+        return self._edges
+
+    def substring_alignments(self) -> List[Tuple[str, str]]:  # noqa: C901
+        """Alignments of input to output substrings for this graph.
+
+        As opposed to `pretty_edges`, this method will return the
+        one-to-many or many-to-one alignments produced by a
+        conversion.  It is also the same between TransductionGraph and
+        CompositeTransductionGraph.  For example, assuming this input
+        and output with these edges::
+
+            ABCDEFF
+            aabbcdef
+            [(0, 0), (0, 1), (1, 2), (1, 3), (2, 4), (3, 5),
+             (4, 6), (5, 7), (6, 7)]
+
+        it should return::
+
+            [('A', 'aa'), ('B', 'bb'), ('C', c'), ('D', 'd'),
+             ('E', 'e'), ('FF', 'f')]
+
+        In the case of reorderings, the substrings returned correspond
+        to the minimal *monotonic* alignments, that is, the minimal
+        subsequences which preserve ordering between the input and
+        output.  So, for example given these edges::
+
+            ABCDEF
+            abefcd
+            [(0, 0), (1, 1), (2, 4), (3, 5), (4, 2), (5, 3)]
+
+        it should return::
+
+            [('A', 'a'), ('B', 'b'), ('CDEF', 'efcd')]
+
+        This means, that in the case of truly radical reorderings,
+        there is no "alignment" per se.  This is highly unlikely to
+        occur, given the constrained nature of g2p rules.
+
+        Note that in the case of multi-character outputs such as in
+        ARPABET, the output substrings *do not necessarily* correspond
+        to tokens, and spaces are treated as any other character in
+        the alignment (thus, alignments of (' ', ' ') are possible).
+        If you wish to reconstruct the input it is your resonsibility
+        to collect all the alignments corresponding to an output token
+        (this should not be too hard to do).
+
+        """
+        alignments = self.alignments()
+
+        def find_monotonic_segments(alignments):
+            segments = []
+            # Sort according to input and output (None is not allowed on input)
+            isort = sorted(
+                alignments, key=lambda x: (x[0], x[0]) if x[1] is None else x
+            )
+            osort = sorted(
+                alignments, key=lambda x: (x[0], x[0]) if x[1] is None else (x[1], x[0])
+            )
+            # print("isort:", isort)
+            # print("osort:", osort)
+            # Use -1 as flag value because None has a meaning in alignments
+            istart = ostart = iend = oend = -1
+            for iedge, oedge in zip(isort, osort):
+                # Create a new segment if the sorting orders agree, or
+                # if the subsequent alignments cannot overlap with the
+                # current segment
+                non_overlapping = (
+                    -1 not in (iend, oend) and iedge[0] > iend and oedge[0] > oend
+                )
+                if iedge == oedge or non_overlapping:
+                    # Output an existing segment if we have one
+                    if iend != -1:
+                        segments.append((istart, iend, ostart, oend))
+                        istart = ostart = iend = oend = -1
+                    # And if we have entered an agreement region output that
+                    if iedge == oedge:
+                        ipos, opos = iedge
+                        segments.append((ipos, ipos, opos, opos))
+                        istart = ostart = iend = oend = -1
+                        continue
+                if istart == -1:  # Start a new segment
+                    # Smallest input index (by definition)
+                    istart = iedge[0]
+                    # Smallest output index (by definition)
+                    ostart = oedge[1]
+                    # These are updated below
+                    iend = oedge[0]
+                    oend = iedge[1]
+                else:  # Expand an existing segment
+                    assert oedge[0] is not None
+                    assert iedge[1] is not None
+                    iend = max(iend, oedge[0])
+                    oend = max(oend, iedge[1])
+            if istart != -1:
+                assert iend != -1
+            # Output a final segment if one exists
+            if iend != -1:
+                segments.append((istart, iend, ostart, oend))
+            return segments
+
+        # Construct areas of agreement
+        segments = find_monotonic_segments(alignments)
+        # print("segments:", segments)
+
+        def merge_overlapping_segments(segments):
+            if len(segments) <= 1:
+                return segments
+            istart, iend, ostart, oend = segments[0]
+            output = []
+            for seg in segments[1:]:
+                # If *start* points are outside current segment, start a new one
+                if None in (seg[2], oend):  # handle only None in outputs
+                    output_outside = not (None, None) == (seg[2], oend)
+                else:
+                    output_outside = seg[2] > oend
+                if seg[0] > iend and output_outside:
+                    output.append((istart, iend, ostart, oend))
+                    istart, iend, ostart, oend = seg
+                else:
+                    # Update endpoints to include this segment
+                    iend = seg[1]
+                    oend = seg[3]
+            output.append((istart, iend, ostart, oend))
+            return output
+
+        # Merge overlapping segments
+        segments = merge_overlapping_segments(segments)
+        # print("merged:", segments)
+        # Output string alignments
+        substrings = []
+        for istart, iend, ostart, oend in segments:
+            istr = self._input_string[istart : iend + 1]
+            if ostart is None:
+                assert oend is None
+                ostr = ""
+            else:
+                ostr = self._output_string[ostart : oend + 1]
+            substrings.append((istr, ostr))
+        return substrings
+
+    def as_dict(self) -> dict:
         return {
             "edges": self._edges,
             "input": self._input_string,
             "output": self._output_string,
             "input_nodes": self._input_nodes,
             "output_nodes": self._output_nodes,
         }
@@ -173,19 +385,22 @@
         out_offset = len(self._output_nodes)
         # append input and output strings
         self._input_string += tg._input_string
         self._output_string += tg._output_string
         # append nodes
         self._input_nodes += [(i + in_offset, x) for (i, x) in tg._input_nodes]
         self._output_nodes += [(i + out_offset, x) for (i, x) in tg._output_nodes]
-        # append edges
-        self._edges += [
-            (i + in_offset, None if j is None else j + out_offset)
-            for (i, j) in tg._edges
-        ]
+        # append edges and normalize
+        self._edges = normalize_edges(
+            self._edges
+            + [
+                (i + in_offset, None if j is None else j + out_offset)
+                for i, j in tg.edges
+            ]
+        )
         # append debuggers
         self._debugger += tg._debugger
 
     def __iadd__(self, tg):
         self.append(tg)
         return self
 
@@ -237,19 +452,34 @@
         """
         if string:
             intermediate_ord = ord(string[0])
             return intermediate_ord - 983040
         else:
             return -1
 
-    def resolve_intermediate_chars(self, output_string):
+    @property
+    def in_lang(self) -> str:
+        """Input language node name"""
+        return self.mapping.kwargs.get("in_lang", "und")
+
+    @property
+    def out_lang(self) -> str:
+        """Output language node name"""
+        return self.mapping.kwargs.get("out_lang", "und")
+
+    @property
+    def transducers(self) -> List["Transducer"]:  # noqa: F821
+        """Sequence of underlying Transducer objects"""
+        return [self]
+
+    def resolve_intermediate_chars(self, output_string) -> str:
         """Go through all chars and resolve any intermediate characters from the Private Supplementary Use Area
         to their mapped equivalents.
         """
-        indices_seen = defaultdict(int)
+        indices_seen: Dict[int, int] = defaultdict(int)
         for i, char in enumerate(output_string):
             intermediate_index = self._pua_to_index(char)
             # if not Private Supplementary Use character
             if intermediate_index < 0:
                 continue
             output_char_index = indices_seen[intermediate_index]
             try:
@@ -267,15 +497,15 @@
                     + output_string[i + 1 :]
                 )
             indices_seen[intermediate_index] += 1
         return output_string
 
     def get_match_groups(
         self, tg, start_end, io, diff_from_input, out_string, output_start
-    ):
+    ) -> Tuple[dict, dict]:
         """Take the inputs to explicit indices matching and create groups of
             Input and Output matches that are grouped by their explicit indices.
 
             For example, applying a rule that is defined: a{1}b{2} → b{2}a{1} on the input "ab"
             will return inputs, outputs where:
 
             inputs = {'1': [{'index': 0, 'string': 'a'}], '2': [{'index': 1, 'string': 'b'}] }
@@ -299,15 +529,15 @@
         """
         input_char_matches = [
             x.group() for x in self._char_match_pattern.finditer(io["in"])
         ]
         input_match_indices = [
             x.group() for x in self._index_match_pattern.finditer(io["in"])
         ]
-        inputs = {}
+        inputs: Dict[str, List[dict]] = {}
         index = 0
 
         input_start = (
             start_end[0] - diff_from_input[self.get_input_from_output(tg, start_end[0])]
         )
 
         for i, m in enumerate(input_match_indices):
@@ -319,15 +549,15 @@
                 index += 1
         output_char_matches = [
             x.group() for x in self._char_match_pattern.finditer(out_string)
         ]
         output_match_indices = [
             x.group() for x in self._index_match_pattern.finditer(out_string)
         ]
-        outputs = {}
+        outputs: Dict[str, List[dict]] = {}
         index = 0
         for i, m in enumerate(output_match_indices):
             for char in output_char_matches[i]:
                 if m in outputs:
                     outputs[m].append({"index": index + output_start, "string": char})
                 else:
                     outputs[m] = [{"index": index + output_start, "string": char}]
@@ -349,17 +579,17 @@
         # update indices
         for k, edge in enumerate(tg.edges):
             if (
                 edge[1] is not None
                 and (ahh == 0 or tg.edges[k - 1][1] is None)
                 and edge[1] == index_to_delete
             ):
-                tg.edges[k][1] = None
+                tg.edges[k] = (edge[0], None)
             elif edge[1] is not None and edge[1] >= index_to_delete:
-                tg.edges[k][1] -= 1
+                tg.edges[k] = (edge[0], edge[1] - 1)
 
     def insert_character(self, tg, character_to_insert, index_to_insert_character):
         """Insert character at `index_to_insert_character` in TransductionGraph output
 
         Args:
             tg (TransductionGraph): the current Transduction Graph
             character_to_insert (str): the character to insert
@@ -369,15 +599,15 @@
         tg.output_string = (
             tg.output_string[:index_to_insert_character]
             + character_to_insert
             + tg.output_string[index_to_insert_character:]
         )
         for j, edge in enumerate(tg.edges):
             if edge[1] is not None and edge[1] >= index_to_insert_character:
-                tg.edges[j][1] += 1
+                tg.edges[j] = (edge[0], edge[1] + 1)
 
     def change_character(self, tg, character, index_to_change):
         """Change character at `index_to_change` in TransductionGraph output to `character`
 
         Args:
             tg (TransductionGraph): the current Transduction Graph
             character (str): the character to change to
@@ -453,15 +683,17 @@
                     if output_matches:
                         tg.edges = [x for x in tg.edges if x[1] != index_to_delete]
                         tg.edges.append([input_matches[i]["index"], None])
 
     def get_input_from_output(self, tg, output_node):
         return max(x[0] for x in tg.edges if x[1] == output_node)
 
-    def get_longest_and_shortest(self, in_string_or_matches, out_string_or_matches):
+    def get_longest_and_shortest(
+        self, in_string_or_matches, out_string_or_matches
+    ) -> Tuple[str, Union[str, list], Union[str, list]]:
         """Given two strings or match lists determine the longest and shortest. If
            the input is longer than the output, the process is to delete,
            if the output is longer than the input, the process is to insert.
            If the input and output are the same length, the process is basic.
 
         Args:
             in_string_or_matches (str|List): input string
@@ -511,31 +743,38 @@
             #  - decrement edges following the deleted character
             elif process == "delete":
                 # Nodes
                 index_to_delete = output_index - deleted
                 self.delete_character(tg, index_to_delete, i)
                 deleted += 1
 
-    def apply_unidecode(self, to_convert: str):
+    def apply_unidecode(self, to_convert: str) -> TransductionGraph:
         to_convert = unicode_escape(to_convert)
         saved_to_convert = to_convert
         if self.norm_form:
             to_convert, norm_indices = normalize_with_indices(
                 to_convert, self.norm_form
             )
         else:
             norm_indices = None
         tg = TransductionGraph(to_convert)
 
         # Conversion is done character by character using unidecode
-        converted = [
-            text_unidecode.unidecode(unicodedata.normalize("NFKC", c))
-            for c in to_convert
-        ]
-        converted = [sanitize_unidecode_output(c) for c in converted]
+        # We retain spaces in the input, but spaces from unidecode are removed
+        converted = []
+        for in_char in to_convert:
+            unidecode_str = text_unidecode.unidecode(
+                unicodedata.normalize("NFKC", in_char)
+            )
+            cc = [
+                c
+                for c in unidecode_str
+                if c.isalpha() or c in UNIDECODE_SPECIALS or in_char.isspace()
+            ]
+            converted.append("".join(cc))
         tg.output_string = "".join(converted)
 
         # Edges are calculated to follow the conversion step by step
         if not tg.output_string:
             # Some inputs get completely deleted by unidecode, in which case there are no
             # valid edges to output.
             tg.edges = []
@@ -554,17 +793,64 @@
                 tg.edges = compose_indices(norm_indices, edges)
                 tg.input_string = saved_to_convert
             else:
                 tg.edges = edges
 
         return tg
 
+    def apply_lexicon(self, to_convert: str):
+        tg = TransductionGraph(to_convert)
+        if not self.case_sensitive:
+            to_convert = to_convert.lower()
+        alignment = self.mapping.alignments.get(to_convert, ())
+        if not alignment:
+            tg.edges = []
+            tg.output_string = ""
+        else:
+            tg.output_string = ""
+            edges: List[Tuple[int, int]] = []
+            in_pos = 0
+            out_pos = 0
+            # Mappings are flattened to save space
+            for idx in range(0, len(alignment), 2):
+                (n_inputs, outtxt) = alignment[idx : idx + 2]
+                for i in range(n_inputs):
+                    for j in range(len(outtxt)):
+                        edges.append((in_pos + i, out_pos + j))
+                    if len(outtxt) == 0:
+                        # Attach deletions to the previous output if
+                        # possible, otherwise the next output.  This
+                        # will be modified to None below if the output
+                        # string is empty.
+                        edges.append((in_pos + i, max(0, out_pos - 1)))
+                if n_inputs == 0:
+                    # Attach insertions to the previous input
+                    for j in range(len(outtxt)):
+                        edges.append((in_pos, out_pos + j))
+                in_pos += n_inputs
+                if len(outtxt) != 0:
+                    out_pos += len(outtxt) + len(self.out_delimiter)
+                    # Be bug-compatible with mappings and add an extra delimiter
+                    tg.output_string += outtxt + self.out_delimiter
+            # Fix up bogus indices here
+            out_len = len(tg.output_string)
+            tg.edges = []
+            for in_pos, out_pos in edges:
+                assert in_pos is not None
+                if out_pos >= out_len:
+                    tg.edges.append((in_pos, None if out_len == 0 else out_len - 1))
+                else:
+                    tg.edges.append((in_pos, out_pos))
+        return tg
+
     def apply_rules(self, to_convert: str):  # noqa: C901
         if self.mapping.kwargs.get("type", "") == "unidecode":
             return self.apply_unidecode(to_convert)
+        elif self.mapping.kwargs.get("type", "") == "lexicon":
+            return self.apply_lexicon(to_convert)
 
         # perform any normalization
         to_convert = unicode_escape(to_convert)
         saved_to_convert = to_convert
         if not self.case_sensitive:
             to_convert = to_convert.lower()
         if self.norm_form:
@@ -660,53 +946,28 @@
                     diff_from_output[n] += diff
                 for n in range(input_index, len(diff_from_input)):
                     diff_from_input[n] += diff
 
         if intermediate_forms:
             tg.output_string = self.resolve_intermediate_chars(tg.output_string)
 
-        # fix None
-        to_remove = []  # type: ignore
-        for i, edge in enumerate(tg.edges):
-            if edge[1] is None:
-                to_remove.extend(
-                    i
-                    for other_edge in tg.edges
-                    if other_edge != edge and other_edge[0] == edge[0]
-                )
-
-        for i in set(to_remove):
-            del tg.edges[i]
-        # sort based on inputs
-        tg.edges.sort(key=lambda x: x[0])
-        for i, edge in enumerate(tg.edges):
-            if edge[1] is None:
-                # if previous exists, use that, otherwise use following, otherwise None
-                previous = [x for x in tg.edges[:i] if x[1] is not None]
-                try:
-                    following = [x for x in tg.edges[i + 1 :] if x[1] is not None]
-                except IndexError:
-                    following = None
-                if previous:
-                    edge[1] = previous[-1][1]
-                elif following:
-                    edge[1] = following[0][1]
-        tg.edges = list(dict.fromkeys([tuple(x) for x in tg.edges]))
+        # sort and fix None
+        tg.edges = normalize_edges(tg.edges)
         if norm_indices is not None:
             tg.edges = compose_indices(norm_indices, tg.edges)
             tg.input_string = saved_to_convert
         return tg
 
     def check(
         self,
         tg: TransductionGraph,
         shallow=False,
         display_warnings=False,
         original_input=None,
-    ):
+    ) -> bool:
         out_lang = self.mapping.kwargs["out_lang"]
         if "eng-arpabet" in out_lang:
             if is_arpabet(tg.output_string):
                 return True
             if display_warnings:
                 display_input = original_input or tg.input_string
                 LOGGER.warning(
@@ -745,40 +1006,81 @@
         self._edges = [x.edges for x in tg_list]
         # Debugger
         self._debugger = [x.debugger for x in tg_list]
         # Tiers
         self._tiers = tg_list
 
     @property
-    def tiers(self):
-        """List[TransductionGraph]: A list of TransductionGraph objects for each tier in the CompositeTransducer"""
+    def tiers(self) -> List[TransductionGraph]:
+        """A list of TransductionGraph objects for each tier in the CompositeTransducer"""
         return self._tiers
 
     @tiers.setter
     def tiers(self, value):
         raise ValueError(
             f"Sorry, you tried to change the tiers to {value} but they cannot be changed"
         )
 
+    @property
+    def edges(self) -> List:
+        """List[List[Tuple[int, Optional[int]]]] of edges for each tier in the
+        transformation.
+
+        Note that this is unfortunately *not* the same between
+        TransductionGraph and ComposedTransductionGraph.
+        """
+        return self._edges
+
+    @edges.setter
+    def edges(self, value):
+        raise ValueError(
+            f"Sorry, you tried to change the edges to {value} but they cannot be changed"
+        )
+
+    @property
+    def debugger(self) -> List[list]:
+        """List[List[List[dict]]]: A list of lists of lists of rules applied
+        during the transformation. Useful for debugging.  Note that
+        this is not the same between TransductionGraph and
+        CompositeTransductionGraph.
+
+        """
+        return self._debugger
+
+    @debugger.setter
+    def debugger(self, value):
+        raise ValueError(
+            f"Sorry, you tried to change the debugger to {value} but they cannot be changed"
+        )
+
     def pretty_edges(self):
+        """List[List[Tuple[str, str]]] of edges for each tier, expressed as
+        strings.
+
+        Note that this is unfortunately *not* the same output between
+        TransductionGraph and ComposedTransductionGraph.
+
+        """
         pretty_edges = []
-        for tier_i, edges in enumerate(self._edges):
-            edges = copy.deepcopy(edges)
-            edges.sort(key=lambda x: x[0])
-            for i, edge in enumerate(edges):
-                if edge[1] is None:
-                    edges[i] = [self.tiers[tier_i].input_nodes[edge[0]][1], None]
-                else:
-                    edges[i] = [
-                        self.tiers[tier_i].input_nodes[edge[0]][1],
-                        self.tiers[tier_i].output_nodes[edge[1]][1],
-                    ]
-            pretty_edges.append(edges)
+        for tier in self._tiers:
+            pretty_edges.append(tier.pretty_edges())
         return pretty_edges
 
+    def alignments(self) -> List[Tuple[int, Optional[int]]]:
+        """Return list of alignments (input node index, output node index) for
+        the full transduction.
+
+        Note that this *is* the same between TransductionGraph and
+        CompositeTransductionGraph.
+        """
+        composed = self.tiers[0].edges
+        for tier in self.tiers[1:]:
+            composed = compose_indices(composed, tier.edges)
+        return composed
+
     def as_dict(self):
         return {
             "edges": self._edges,
             "input": self._input_string,
             "output": self._output_string,
             "input_nodes": self._input_nodes,
             "output_nodes": self._output_nodes,
@@ -817,14 +1119,29 @@
 
     def __repr__(self):
         return f"{self.__class__} between {self._transducers[0].mapping.kwargs.get('in_lang', 'und')} and {self._transducers[-1].mapping.kwargs.get('out_lang', 'und')}"
 
     def __call__(self, to_convert: str):
         return self.apply_rules(to_convert)
 
+    @property
+    def transducers(self):
+        """Sequence of underlying Transducer objects"""
+        return self._transducers
+
+    @property
+    def in_lang(self):
+        """Input language node name"""
+        return self._transducers[0].in_lang
+
+    @property
+    def out_lang(self):
+        """Output language node name"""
+        return self._transducers[-1].out_lang
+
     def apply_rules(self, to_convert: str):
         tg_list = []
         for transducer in self._transducers:
             tg = transducer(to_convert)
             tg_list.append(tg)
             to_convert = tg.output_string
         return CompositeTransductionGraph(tg_list)
@@ -854,20 +1171,27 @@
                         return False
             return result
 
 
 class TokenizingTransducer:
     """This class combines tokenization and transduction.
 
+    This is particularly useful for lexicon mappings, which cannot
+    handle more than a single word at a time.
+
     Attributes:
-        transducer (Transducer): A Tranducer object for the mapping part
+        transducer (Transducer): A Transducer object for the mapping part
         tokenizer (DefaultTokenizer): A Tokenizer object to split the string before mapping
     """
 
-    def __init__(self, transducer: Transducer, tokenizer: DefaultTokenizer):
+    def __init__(
+        self,
+        transducer: Union[Transducer, CompositeTransducer],
+        tokenizer: DefaultTokenizer,
+    ):
         self._transducer = transducer
         self._tokenizer = tokenizer
 
     def __call__(self, to_convert: str):
         # perform normalization before tokenizing, since it can change tokenization
         if self._transducer.norm_form:
             to_convert = normalize(to_convert, self._transducer.norm_form)
@@ -882,14 +1206,34 @@
                 word_tg = self._transducer(token["text"])
                 tg += word_tg
             else:
                 non_word_tg = TransductionGraph(token["text"])
                 tg += non_word_tg
         return tg
 
+    @property
+    def transducer(self):
+        """Underlying Transducer object"""
+        return self._transducer
+
+    @property
+    def transducers(self) -> List[Transducer]:
+        """Sequence of underlying Transducer objects"""
+        return self._transducer.transducers
+
+    @property
+    def in_lang(self) -> str:
+        """Input language node name"""
+        return self._transducer.in_lang
+
+    @property
+    def out_lang(self) -> str:
+        """Output language node name"""
+        return self._transducer.out_lang
+
     def check(self, tg: TransductionGraph, shallow=False, display_warnings=False):
         # The obvious implementation fails, because we need to check only the words, not
         # the text between the words!
         # return self._transducer.check(tg) # <- complains about characters between words
 
         # So, sadly, we redo the work of transduction so we can check the words only, step
         # by step. I don't like this solution, but I don't see how to get around it.
```

### Comparing `g2p-1.0.20230228/g2p.egg-info/PKG-INFO` & `g2p-1.0.20230412/g2p.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g2p
-Version: 1.0.20230228
+Version: 1.0.20230412
 Summary: Module for creating context-aware, rule-based G2P mappings that preserve indices
 Home-page: https://github.com/roedoejet/g2p
 Author: Aidan Pine
 Author-email: hello@aidanpine.ca
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 # Gᵢ2Pᵢ
 
 [![codecov](https://codecov.io/gh/roedoejet/g2p/branch/main/graph/badge.svg)](https://codecov.io/gh/roedoejet/g2p)
 [![Documentation Status](https://readthedocs.org/projects/g2p/badge/?version=latest)](https://g2p.readthedocs.io/en/latest/?badge=latest)
 [![Build Status](https://github.com/roedoejet/g2p/actions/workflows/tests.yml/badge.svg)](https://github.com/roedoejet/g2p/actions)
 [![PyPI package](https://img.shields.io/pypi/v/g2p.svg)](https://pypi.org/project/g2p/)
 [![license](https://img.shields.io/badge/Licence-MIT-green)](LICENSE)
-[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/roedoejet/g2p)
+[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg)](https://github.com/roedoejet/g2p)
 
 > Grapheme-to-Phoneme transformations that preserve input and output indices!
 
 This library is for handling arbitrary conversions between input and output segments while preserving indices.
 
 ![indices](https://raw.githubusercontent.com/roedoejet/g2p/main/g2p/static/assets/bonjour.png)
```

### Comparing `g2p-1.0.20230228/g2p.egg-info/SOURCES.txt` & `g2p-1.0.20230412/g2p.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -72,20 +72,24 @@
 g2p/mappings/langs/ctp/config.yaml
 g2p/mappings/langs/ctp/ctp_ipa_to_eng_ipa.json
 g2p/mappings/langs/ctp/ctp_to_ipa.json
 g2p/mappings/langs/dan/config.yaml
 g2p/mappings/langs/dan/dan_abbs.csv
 g2p/mappings/langs/dan/dan_to_dummy.json
 g2p/mappings/langs/dan/dan_to_ipa.csv
-g2p/mappings/langs/eng/cmu_sphinx.metadata.json
-g2p/mappings/langs/eng/cmudict_SPHINX_40.txt
+g2p/mappings/langs/eng/README.md
+g2p/mappings/langs/eng/cmudict.ipa.aligned.txt
 g2p/mappings/langs/eng/config.yaml
 g2p/mappings/langs/eng/dummy_to_arpabet.json
+g2p/mappings/langs/eng/eng_arpabet_to_ipa.json
 g2p/mappings/langs/eng/eng_inventory.json
 g2p/mappings/langs/eng/eng_ipa_to_arpabet.json
+g2p/mappings/langs/eng/make_alignments.sh
+g2p/mappings/langs/eng/make_ipa_cmudict.py
+g2p/mappings/langs/eng/reverse_json.py
 g2p/mappings/langs/fin/config.yaml
 g2p/mappings/langs/fin/fin_to_ipa.csv
 g2p/mappings/langs/font-encodings/README.md
 g2p/mappings/langs/font-encodings/config.yaml
 g2p/mappings/langs/font-encodings/fn_unicode.csv
 g2p/mappings/langs/font-encodings/hei_doulos.csv
 g2p/mappings/langs/font-encodings/hei_times.csv
@@ -255,14 +259,15 @@
 g2p/tests/test_cli.py
 g2p/tests/test_create_mapping.py
 g2p/tests/test_doctor.py
 g2p/tests/test_doctor_expensive.py
 g2p/tests/test_fallback.py
 g2p/tests/test_indices.py
 g2p/tests/test_langs.py
+g2p/tests/test_lexicon_transducer.py
 g2p/tests/test_mappings.py
 g2p/tests/test_network.py
 g2p/tests/test_studio.py
 g2p/tests/test_tokenize_and_map.py
 g2p/tests/test_tokenizer.py
 g2p/tests/test_transducer.py
 g2p/tests/test_unidecode_transducer.py
@@ -313,14 +318,15 @@
 g2p/tests/public/mappings/abbreviation_config.yaml
 g2p/tests/public/mappings/abbreviation_mapping.csv
 g2p/tests/public/mappings/abbreviations.csv
 g2p/tests/public/mappings/abbreviations.json
 g2p/tests/public/mappings/abbreviations.psv
 g2p/tests/public/mappings/abbreviations.substring.csv
 g2p/tests/public/mappings/abbreviations.tsv
+g2p/tests/public/mappings/bad_lexicon_config.yaml
 g2p/tests/public/mappings/compose.yaml
 g2p/tests/public/mappings/compose1-2.csv
 g2p/tests/public/mappings/compose2-3.csv
 g2p/tests/public/mappings/deletion.csv
 g2p/tests/public/mappings/deletion.json
 g2p/tests/public/mappings/deletion_config_csv.yaml
 g2p/tests/public/mappings/deletion_config_json.yaml
@@ -330,14 +336,16 @@
 g2p/tests/public/mappings/gen-map-2.csv
 g2p/tests/public/mappings/gen-map-3a.csv
 g2p/tests/public/mappings/gen-map-3b.csv
 g2p/tests/public/mappings/gen-map_config.yaml
 g2p/tests/public/mappings/gm1-ipa_to_gm2-ipa.json
 g2p/tests/public/mappings/gm2-ipa_to_gm3-ipa.json
 g2p/tests/public/mappings/gm3-ipa_to_gm2-ipa.json
+g2p/tests/public/mappings/hello.aligned.txt
+g2p/tests/public/mappings/lexicon_config.yaml
 g2p/tests/public/mappings/malformed_config.yaml
 g2p/tests/public/mappings/minimal.csv
 g2p/tests/public/mappings/minimal.json
 g2p/tests/public/mappings/minimal.psv
 g2p/tests/public/mappings/minimal.tsv
 g2p/tests/public/mappings/minimal.xlsx
 g2p/tests/public/mappings/minimal_config.yaml
```

### Comparing `g2p-1.0.20230228/setup.py` & `g2p-1.0.20230412/setup.py`

 * *Files identical despite different names*

