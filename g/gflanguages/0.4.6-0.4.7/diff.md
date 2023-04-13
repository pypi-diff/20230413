# Comparing `tmp/gflanguages-0.4.6.tar.gz` & `tmp/gflanguages-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gflanguages-0.4.6.tar", last modified: Fri Mar 24 10:36:16 2023, max compression
+gzip compressed data, was "gflanguages-0.4.7.tar", last modified: Thu Apr 13 10:01:27 2023, max compression
```

## Comparing `gflanguages-0.4.6.tar` & `gflanguages-0.4.7.tar`

### file list

```diff
@@ -1,2050 +1,2052 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 10:36:16.311072 gflanguages-0.4.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 10:36:15.995069 gflanguages-0.4.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 10:36:15.995069 gflanguages-0.4.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-03-24 10:35:56.000000 gflanguages-0.4.6/.github/workflows/publish-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-03-24 10:35:56.000000 gflanguages-0.4.6/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-24 10:35:56.000000 gflanguages-0.4.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-03-24 10:35:56.000000 gflanguages-0.4.6/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-03-24 10:35:56.000000 gflanguages-0.4.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-24 10:35:56.000000 gflanguages-0.4.6/CONTRIBUTORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10851 2023-03-24 10:35:56.000000 gflanguages-0.4.6/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 10:36:15.995069 gflanguages-0.4.6/Lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 10:36:15.999069 gflanguages-0.4.6/Lib/gflanguages/
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-24 10:36:15.000000 gflanguages-0.4.6/Lib/gflanguages/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 10:36:15.995069 gflanguages-0.4.6/Lib/gflanguages/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 10:36:16.255072 gflanguages-0.4.6/Lib/gflanguages/data/languages/
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/aa_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ab_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/abi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/abq_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/abr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/acd_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ace_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/acf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ach_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/acu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ada_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ade_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/adj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/adl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ady_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ae_Avst.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/aeb_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/aeb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/af_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/agc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/agq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/agr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/aha_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ahl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/aho_Ahom.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ahs_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Armi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Brah.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Chrs.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Egyp.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Elym.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Hatr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Mani.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Narb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Nbat.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Palm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Phli.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Phlp.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Phnx.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Prti.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Samr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Sarb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Sogd.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Sogo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Syrc.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Ugar.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ain_Kana.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ain_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ajg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ak_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/akk_Xsux.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/akp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/akz_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ala_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ale_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/aln_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/alt_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/am_Ethi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/amc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ame_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ami_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/amo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/amr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/an_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/anc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ang_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ank_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ann_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/anp_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/anv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/any_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/aoz_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/apd_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ar_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ar_Syrc.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/arb_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/arc_Armi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/arc_Nbat.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/arc_Palm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/arl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/arn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/aro_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/arp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/arq_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ars_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/art_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/arw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ary_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/arz_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/as_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/asa_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/asg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ast_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/atg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/atj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/auc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/av_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/avk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/avn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/avu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/awa_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/awo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ay_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ayb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/az_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/az_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/az_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/azb_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/azj_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ba_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ba_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bal_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bal_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ban_Bali.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ban_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bap_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bar_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bas_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bav_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bax_Bamu.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bax_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bba_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bbc_Batk.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bbc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bbj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bbp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bci_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bcn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bcq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bcw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bcy_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bdh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/be_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/be_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/beh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bej_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bej_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bem_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ber_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ber_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ber_Tfng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bet_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bew_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bex_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bez_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bfa_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bfd_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bfq_Taml.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bft_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bft_Tibt.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bfy_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bg_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bgc_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bgn_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bgx_Grek.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bhb_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bhi_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bhk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bho_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bho_Kthi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bhy_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bib_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bik_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bim_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bin_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/biv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bjj_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bjn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bjt_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bjv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bkc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bkm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bku_Buhd.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bku_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bkv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bla_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/blo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/blt_Tavt.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bm_Nkoo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bmq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bn_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bn_Newa.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bng_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bnm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bo_Marc.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     9698 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bo_Tibt.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bo_Zanb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/boa_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bom_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bov_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/box_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/boz_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bpy_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bqc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bqi_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bqj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bqp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bqv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/br_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bra_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/brh_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/brh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/brx_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6588 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/brx_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/brx_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bs_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bs_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bsc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bsj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bsp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bsq_Bass.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bsq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bss_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bto_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/btt_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/btv_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bua_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/buc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bud_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bug_Bugi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bug_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bum_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bus_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/buu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bvb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bvi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bwr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bwy_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/byh_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/byn_Ethi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/byn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bys_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/byv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bza_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bze_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bzw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/bzx_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ca_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cab_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cad_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cak_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/car_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cay_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cbi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cbj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cbk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cbr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cbs_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cbt_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cbu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cch_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ccp_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     9670 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ccp_Cakm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cdr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ce_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ceb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cfa_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cfm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cgg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ch_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/chj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/chk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/chm_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/chn_Dupl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/chn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cho_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/chp_Cans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/chp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/chr_Cher.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/chx_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/chy_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cic_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cja_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cja_Cham.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cjk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cjm_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cjm_Cham.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cjs_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cjy_Hans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ckb_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ckl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cko_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ckt_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cky_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cla_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cme_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cmg_Soyo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cnh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cni_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/co_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cof_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/con_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cop_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cop_Copt.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cop_Grek.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cot_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cpf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cps_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cpu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cr_Cans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/crh_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/crh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cri_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/crj_Cans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/crj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/crk_Cans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/crl_Cans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/crl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/crm_Cans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/crs_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cs_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/csa_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/csb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/csk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/csw_Cans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ctd_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ctd_Pauc.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cu_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cu_Glag.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cv_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cwe_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cy_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/cyo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/da_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/daa_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dag_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dak_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dar_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dav_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dbd_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dbq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dcc_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ddn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/de_Dupl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/de_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/de_Runr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/del_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/den_Cans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/den_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dga_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dgh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dgi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dgr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dhi_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dhw_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/did_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/din_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dip_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dje_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dmf_Medf.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dng_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dnj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/doi_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/doi_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/doi_Dogr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/doi_Takr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dop_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dow_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dri_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dsb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dtm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dtp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dts_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dty_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dua_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dug_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dum_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/duu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dv_Thaa.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dwr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dyi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dyo_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dyo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dyu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dyu_Nkoo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dz_Tibt.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/dzg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ebu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ee_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/efi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/egl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/egy_Egyp.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/eka_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ekm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/eky_Kali.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/el_Grek.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ema_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/emk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/en_Brai.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/en_Dsrt.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/en_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/en_Shaw.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/enm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/enn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/eo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/es_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ese_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/esg_Gonm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/esu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/et_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ett_Ital.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ett_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/etu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/etx_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/eu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/eve_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/evn_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/evn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ewo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ext_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/eza_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/fa_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/fan_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/fbl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7222 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ff_Adlm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ff_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ffm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/fi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/fia_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/fil_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/fil_Tglg.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/fit_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/fj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/fkv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/flr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/fmp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/fo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/fod_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/fon_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/fr_Dupl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/fr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/frc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/frm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/fro_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/frp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/frr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/frs_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/fub_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/fuc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/fud_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/fue_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/fuf_Adlm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/fuf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/fuh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/fuq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/fur_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/fuv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/fvr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/fy_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ga_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gaa_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gag_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gag_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gan_Hans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gay_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gba_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gbm_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gby_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gbz_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gcf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gcr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gd_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gde_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gej_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gel_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gem_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gez_Ethi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ggn_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ggn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gil_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/giw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gjk_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gjn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gju_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gju_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gkn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gkp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gld_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/glk_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gmh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gmm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gmv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gmy_Linb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gnd_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gng_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/god_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gof_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/goh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gom_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gon_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gon_Gong.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gon_Gonm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gon_Telu.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gor_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gos_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/got_Goth.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/got_Runr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gqr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/grb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/grc_Cprt.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/grc_Grek.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    18660 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/grc_Linb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/grt_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gsw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gu_Gujr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gub_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/guc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gud_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/guk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gur_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/guu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/guw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gux_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/guz_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gvr_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gwi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gyi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/gyr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ha_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ha_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hag_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hai_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hak_Hans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hak_Hant.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hak_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/haw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/haz_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/he_Hebr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hea_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hi_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hi_Mahj.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hi_Newa.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hia_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hif_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hif_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hig_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hil_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hit_Xsux.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hlt_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hlu_Hluw.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hmd_Hmng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hmd_Plrd.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hmn_Hmng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hmn_Hmnp.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hmn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hms_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hna_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hnd_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hne_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hni_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hnj_Hmng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hnj_Laoo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hnj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hnn_Hano.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hnn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hno_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hns_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ho_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hoc_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hoc_Wara.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hoj_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hop_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hsb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hsn_Hans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ht_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hup_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hus_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/huu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hy_Armn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hyw_Armn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/hz_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ia_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/iba_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ibb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/iby_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ica_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ich_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/id_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/id_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/idd_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/idu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ie_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ife_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ig_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/igb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ige_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ii_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ii_Yiii.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ijj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ijs_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ik_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ikk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ikt_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ikw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ikx_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ilo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/inh_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/inh_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/inh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/io_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/iqw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/iri_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/is_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/it_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/iu_Cans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/iu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/izh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/izr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/izz_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ja_Hira.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    14296 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ja_Jpan.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ja_Kana.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/jab_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/jam_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/jbo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/jbu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/jen_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/jgk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/jgo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/jib_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/jiv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/jmc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/jml_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/jpr_Hebr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/jra_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/jrb_Hebr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/jut_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8740 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/jv_Java.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/jv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ka_Geok.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ka_Geor.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kaa_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kab_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kab_Tfng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kac_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kad_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kai_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kaj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kam_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kao_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kbd_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kbp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kby_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kca_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kcg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kck_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kdc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kde_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kdh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kdl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kdt_Thai.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kea_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kek_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ken_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kez_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kfo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kfr_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kfy_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kge_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kgj_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kgp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kha_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kha_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/khb_Talu.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/khn_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/khq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/khr_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/khr_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/khr_Orya.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kht_Mymr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/khw_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/khw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ki_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kiu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kjg_Laoo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kjg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kjh_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kk_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kk_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kkh_Lana.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kkj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kln_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/km_Khmr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kmb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kmy_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kn_Knda.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/knc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/knf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/knp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ko_Kore.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/koi_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/koi_Perm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kok_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/koo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kos_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kpe_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kpo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kpy_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kqn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kqp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kqs_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kr_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/krc_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kri_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/krj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/krl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/krs_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kru_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ks_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ks_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ksb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ksf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ksh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ksp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ksw_Mymr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ktj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ktu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ku_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ku_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ku_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ku_Yezi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kub_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kuj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kum_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kun_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kus_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kut_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kv_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kv_Perm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kvf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kvr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kvx_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kwi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kxm_Thai.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kxp_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ky_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ky_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ky_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kye_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kyf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kyq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kyu_Kali.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kyw_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kyw_Orya.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/kzr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/la_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lab_Lina.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lad_Hebr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lad_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lag_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lah_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/laj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lam_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/las_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lbe_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lbw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lcp_Thai.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ldb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/led_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lee_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lem_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lep_Lepc.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/les_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lez_Aghb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lez_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lfn_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lfn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lgg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lhm_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/li_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lia_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lif_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lif_Limb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lig_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lij_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lip_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lis_Lisu.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/liv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ljp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lki_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lkt_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lld_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lln_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lmn_Telu.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lmo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lmp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ln_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lns_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lnu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lo_Laoo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lob_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/log_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lok_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lol_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/loq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lor_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lot_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/loz_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lrc_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lt_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ltg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lua_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lue_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lui_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lun_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/luo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lus_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lus_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lut_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/luy_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/luz_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lwl_Thai.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lwo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lzh_Hans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lzh_Hant.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lzh_Phag.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lzz_Geor.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/lzz_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mad_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/maf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mag_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mai_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mai_Newa.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mai_Tirh.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mak_Bugi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mak_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mam_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/man_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/man_Nkoo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mas_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/maw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/maz_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mbo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mbu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mcd_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mcf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mcp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mcu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mda_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mdf_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mdh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mdj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mdr_Bugi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mdr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mdt_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/men_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/men_Mend.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/meq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mer_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mey_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mfa_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mfe_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mfi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mfn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mfo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mfq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mfv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mgc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mgh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mgo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mgp_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mgy_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mhi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mic_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/min_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/min_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/miq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mis_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mis_Hatr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mis_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5199 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mis_Nshu.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mk_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mkl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7976 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ml_Mlym.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mls_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mlt_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mmu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mn_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mn_Mong.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mn_Phag.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mn_Zanb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mnc_Mong.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mnf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mni_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mni_Mtei.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mns_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mnw_Mymr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/moa_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/moe_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/moh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mor_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mos_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mqb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mql_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mr_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mr_Modi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mrd_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mrj_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mro_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mro_Mroo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mrw_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mrw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ms_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ms_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/msc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mt_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mto_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mtr_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mua_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/muh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mui_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mur_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mus_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/muy_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mvy_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mwk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mwl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mwr_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mwv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mww_Hmng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mxc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mxi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mxv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/my_Mymr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/myk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mym_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/myv_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/myx_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/myz_Mand.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mzi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mzk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mzm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mzn_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/mzw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/na_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nan_Hans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nan_Hant.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nan_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nap_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/naq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nat_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/naw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nba_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nch_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ncu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nd_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ndc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ndj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nds_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ndz_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ne_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ne_Newa.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/neb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/new_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/new_Newa.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nfr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ng_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nga_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ngb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ngl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ngp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nhb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nhe_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nhn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nhu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nhw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nia_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nij_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nin_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nio_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/niu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/niy_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/njo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nko_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nku_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nmg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nmz_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nnh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nnp_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nnp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nnp_Wcho.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nnq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nnw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/no_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nod_Lana.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/noe_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nog_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/non_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/non_Runr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/not_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nov_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nqo_Nkoo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nrb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nrf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nsk_Cans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nsk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nso_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nst_Tnsa.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ntm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ntr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nui_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nup_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nus_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nuv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nwb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nxq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ny_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nym_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nyn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nyo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/nzi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/oaa_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/oc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ogc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ohu_Hung.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/oj_Cans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/oj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ojb_Cans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/oki_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/okr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/om_Ethi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/om_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/omn_Lina.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/or_Orya.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/orh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/orv_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/os_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/osa_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/osa_Osge.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/osc_Ital.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/osc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ota_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ote_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/otk_Orkh.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/otn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/owl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ozm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pa_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6289 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pa_Guru.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pag_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pal_Phli.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pal_Phlp.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pam_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pap_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pau_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pbb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pbi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pcd_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pck_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pcm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pdc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pdt_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/peo_Xpeo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pfl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/phn_Phnx.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pi_Brah.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pi_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pi_Sinh.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pi_Thai.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pil_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pip_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pis_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/piu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pka_Brah.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pko_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pms_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/png_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pnt_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pnt_Grek.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pnt_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pon_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pov_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/poy_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ppl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pra_Khar.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/prd_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/prg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pro_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/prq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/prs_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ps_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pt_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/puu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pwo_Mymr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/pym_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/qu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/quc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/qud_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/qug_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/quh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/quy_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/quz_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/qva_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/qvc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/qvh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/qvm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/qvn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/qwh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/qxn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/qxu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rab_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/raj_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rap_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rar_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ray_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rcf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rej_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rej_Rjng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rel_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/res_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rgn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rhg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rhg_Rohg.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ria_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rif_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rif_Tfng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rjs_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rkt_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rmf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rmn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rmo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rmt_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rmu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rng_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ro_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ro_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rob_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rof_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rom_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rom_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rtm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ru_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rub_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rue_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ruf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rug_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rup_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/rwk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ryu_Jpan.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ryu_Kana.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Ahom.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Avst.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Bali.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Batk.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Bhks.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Brah.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Bugi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Buhd.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Cham.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    36822 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Dogr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Gong.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Gonm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Gran.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Hano.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Khar.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Khoj.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Kthi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Lepc.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Limb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Mahj.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Marc.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Modi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Mong.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Mroo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Mtei.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Mult.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Newa.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Olck.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Orya.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Phag.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Ranj.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Rjng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Saur.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Shrd.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Sidd.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Sind.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Sinh.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Sora.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Soyo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Sund.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Sylo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Tagb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Takr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Tirh.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Wara.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Wcho.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Xpeo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Zanb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sad_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/saf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sah_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sam_Hebr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sam_Samr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/saq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sas_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sat_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sat_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sat_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sat_Olck.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sat_Orya.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sav_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/saz_Saur.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sba_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sbp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sck_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/scn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sco_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/scs_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sd_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sd_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sd_Khoj.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sd_Sind.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sdc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sdh_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/se_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/se_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/see_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sef_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/seh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sei_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sel_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ses_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sey_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sga_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sga_Ogam.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sgs_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/she_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/shi_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/shi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/shi_Tfng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/shk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/shn_Mymr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/shp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/shu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/si_Sinh.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sid_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sig_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sil_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sja_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/skr_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/skr_Mult.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sla_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sld_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sli_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/slr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sly_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sma_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/smj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/smn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/smp_Samr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sms_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/snf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/snk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/snn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/snw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/so_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/so_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/so_Osma.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sog_Sogd.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sog_Sogo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sok_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sou_Thai.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/soy_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/spp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sq_Elba.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sr_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/srb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/srb_Sora.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/srn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/srr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/srx_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ss_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ssy_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/st_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/stq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/str_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/su_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/su_Sund.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/suk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/suq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sur_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sus_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sus_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/swb_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/swb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/swc_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/swg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/swv_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sxb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sxn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/sxw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/syc_Syrc.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/syi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/syl_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/syl_Sylo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/syr_Syrc.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/szl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7943 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ta_Taml.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tab_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/taj_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/taj_Tibt.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tal_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tan_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/taq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/taq_Tfng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tbw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tbw_Tagb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tbz_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tca_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tcy_Knda.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tdd_Tale.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tdg_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tdg_Tibt.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tdh_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tdt_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/te_Telu.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ted_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tem_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/teo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ter_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tet_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tfi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tg_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tg_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/th_Thai.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/thf_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/thl_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/thq_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/thr_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ths_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ti_Ethi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tig_Ethi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tik_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tiv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tiw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tjs_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tk_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tk_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tk_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tke_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tkl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tkr_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tkr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tkt_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tlh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tli_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tlj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tly_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tly_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tly_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tmh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tn_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tnr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/to_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tob_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tod_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tog_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/toi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/toj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/top_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/toq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tpi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tpm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tr_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/trp_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tru_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tru_Syrc.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/trv_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/trw_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ts_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tsd_Grek.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tsf_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tsg_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tsi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tsj_Tibt.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tsw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tsz_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tt_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tt_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tt_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ttj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ttr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tts_Thai.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ttt_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ttt_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ttt_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tul_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tum_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tuq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tvd_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tvl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tvu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/twq_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6492 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/txg_Tang.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/txo_Toto.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ty_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tyv_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tzh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tzm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tzm_Tfng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/tzo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ude_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/udm_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/udm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/udu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ug_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ug_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ug_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/uga_Ugar.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/uk_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/uli_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/umb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/unr_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/unr_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/unr_Nagm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/unr_Orya.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/unx_Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/unx_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ur_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ura_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/uth_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/utr_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/uz_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/uz_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/uz_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/vag_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/vai_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/vai_Vaii.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ve_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/vec_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/vep_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/vi_Hani.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/vi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/vic_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/vid_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/vls_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/vmf_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/vmw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/vo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/vot_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/vro_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/vun_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/vut_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/wa_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/wae_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/wal_Ethi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/wal_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/wan_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/war_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/was_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/wbp_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/wbq_Telu.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/wbr_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/wci_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/wib_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/wja_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/wji_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/wls_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/wmw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/wni_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/wo_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/wo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/wob_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/wsg_Gonm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/wtm_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/wuu_Hans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/wwa_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/xal_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/xav_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/xcr_Cari.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/xed_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/xh_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/xlc_Lyci.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/xld_Lydi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/xly_Elym.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/xmf_Geor.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/xmn_Mani.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/xmr_Merc.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/xmr_Mero.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/xna_Narb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/xnr_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/xog_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/xon_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/xpr_Prti.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/xrb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/xsa_Sarb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/xsm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/xsr_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/xum_Ital.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/xum_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/xuo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/xwe_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/yad_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/yal_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/yam_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/yao_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/yap_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/yas_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/yat_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/yav_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/yay_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/yaz_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/yba_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ybb_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ybh_Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/yer_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/yi_Hebr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ykg_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/yko_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/yo_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/yre_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/yrk_Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/yrl_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/yua_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/yue_Hani.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    13480 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/yue_Hans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/yue_Hant.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/za_Hans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/za_Hant.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/za_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/zag_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/zam_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/zap_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/zay_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/zdj_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/zdj_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/zea_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/zen_Tfng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/zgh_Tfng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    15684 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/zh_Hans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)    15600 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/zh_Hant.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/zh_Hebr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/zh_Phag.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ziw_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/zlm_Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/zlm_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/zmi_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/zne_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/zro_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/ztu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/zu_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/zul_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/zun_Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/languages/zza_Latn.textproto
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 10:36:16.291072 gflanguages-0.4.6/Lib/gflanguages/data/regions/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/AC.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/AD.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/AE.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/AF.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/AG.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/AI.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/AL.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/AM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/AO.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/AQ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/AR.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/AS.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/AT.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/AU.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/AW.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/AX.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/AZ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/BA.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/BB.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/BD.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/BE.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/BF.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/BG.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/BH.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/BI.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/BJ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/BL.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/BM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/BN.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/BO.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/BQ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/BR.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/BS.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/BT.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/BV.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/BW.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/BY.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/BZ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/CA.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/CC.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/CD.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/CF.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/CG.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/CH.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/CI.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/CK.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/CL.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/CM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/CN.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/CO.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/CP.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/CR.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/CU.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/CV.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/CW.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/CX.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/CY.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/CZ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/DE.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/DG.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/DJ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/DK.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/DM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/DO.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/DZ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/EA.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/EC.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/EE.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/EG.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/EH.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/ER.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/ES.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/ET.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/FI.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/FJ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/FK.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/FM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/FO.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/FR.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/GA.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/GB.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/GD.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/GE.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/GF.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/GG.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/GH.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/GI.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/GL.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/GM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/GN.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/GP.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/GQ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/GR.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/GS.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/GT.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/GU.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/GW.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/GY.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/HK.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/HM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/HN.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/HR.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/HT.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/HU.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/IC.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/ID.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/IE.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/IL.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/IM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/IN.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/IO.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/IQ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/IR.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/IS.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/IT.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/JE.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/JM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/JO.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/JP.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/KE.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/KG.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/KH.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/KI.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/KM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/KN.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/KP.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/KR.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/KW.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/KY.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/KZ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/LA.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/LB.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/LC.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/LI.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/LK.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/LR.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/LS.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/LT.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/LU.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/LV.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/LY.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/MA.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/MC.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/MD.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/ME.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/MF.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/MG.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/MH.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/MK.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/ML.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/MM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/MN.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/MO.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/MP.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/MQ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/MR.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/MS.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/MT.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/MU.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/MV.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/MW.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/MX.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/MY.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/MZ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/NA.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/NC.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/NE.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/NF.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/NG.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/NI.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/NL.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/NO.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/NP.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/NR.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/NU.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/NZ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/OM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/PA.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/PE.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/PF.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/PG.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/PH.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/PK.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/PL.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/PM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/PN.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/PR.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/PS.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/PT.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/PW.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/PY.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/QA.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/RE.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/RO.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/RS.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/RU.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/RW.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/SA.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/SB.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/SC.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/SD.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/SE.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/SG.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/SH.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/SI.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/SJ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/SK.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/SL.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/SM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/SN.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/SO.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/SR.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/SS.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/ST.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/SV.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/SX.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/SY.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/SZ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/TA.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/TC.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/TD.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/TF.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/TG.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/TH.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/TJ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/TK.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/TL.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/TM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/TN.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/TO.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/TR.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/TT.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/TV.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/TW.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/TZ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/UA.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/UG.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/UM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/US.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/UY.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/UZ.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/VA.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/VC.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/VE.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/VG.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/VI.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/VN.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/VU.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/WF.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/WS.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/XK.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/YE.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/YT.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/ZA.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/ZM.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/regions/ZW.textproto
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 10:36:16.311072 gflanguages-0.4.6/Lib/gflanguages/data/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Adlm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Aghb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Ahom.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Arab.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Aran.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Armi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Armn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Avst.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Bali.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Bamu.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Bass.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Batk.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Beng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Bhks.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Brah.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Brai.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Bugi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Buhd.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Cakm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Cans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Cari.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Cham.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Cher.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Chrs.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Copt.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Cprt.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Cyrl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Deva.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Dogr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Dsrt.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Dupl.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Egyp.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Elba.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Elym.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Ethi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Geok.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Geor.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Glag.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Gong.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Gonm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Goth.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Gran.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Grek.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Gujr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Guru.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Hani.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Hano.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Hans.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Hant.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Hatr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Hebr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Hira.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Hluw.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Hmng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Hmnp.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Hung.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Ital.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Java.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Jpan.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Kali.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Kana.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Khar.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Khmr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Khoj.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Knda.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Kore.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Kthi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Lana.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Laoo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Latn.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Lepc.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Limb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Lina.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Linb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Lisu.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Lyci.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Lydi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Mahj.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Mand.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Mani.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Marc.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Medf.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Mend.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Merc.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Mero.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Mlym.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Modi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Mong.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Mroo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Mtei.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Mult.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Mymr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Nagm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Narb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Nbat.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Newa.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Nkoo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Nshu.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Ogam.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Olck.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Orkh.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Orya.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Osge.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Osma.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Palm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Pauc.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Perm.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Phag.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Phli.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Phlp.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Phnx.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Plrd.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Prti.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Ranj.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Rjng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Rohg.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Runr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Samr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Sarb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Saur.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Shaw.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Shrd.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Sidd.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Sind.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Sinh.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Sogd.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Sogo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Sora.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Soyo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Sund.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Sylo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Syrc.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Tagb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Takr.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Tale.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Talu.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Taml.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Tang.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Tavt.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Telu.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Tfng.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Tglg.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Thaa.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Thai.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Tibt.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Tirh.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Tnsa.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Toto.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Ugar.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Vaii.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Wara.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Wcho.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Xpeo.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Xsux.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Yezi.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Yiii.textproto
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/data/scripts/Zanb.textproto
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/languages_public.proto
--rw-r--r--   0 runner    (1001) docker     (123)    23492 2023-03-24 10:35:56.000000 gflanguages-0.4.6/Lib/gflanguages/languages_public_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 10:36:15.999069 gflanguages-0.4.6/Lib/gflanguages.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-03-24 10:36:15.000000 gflanguages-0.4.6/Lib/gflanguages.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    97650 2023-03-24 10:36:15.000000 gflanguages-0.4.6/Lib/gflanguages.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 10:36:15.000000 gflanguages-0.4.6/Lib/gflanguages.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 10:36:15.000000 gflanguages-0.4.6/Lib/gflanguages.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-24 10:36:15.000000 gflanguages-0.4.6/Lib/gflanguages.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-24 10:36:15.000000 gflanguages-0.4.6/Lib/gflanguages.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-03-24 10:36:16.311072 gflanguages-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-03-24 10:35:56.000000 gflanguages-0.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 10:36:15.995069 gflanguages-0.4.6/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 10:36:15.995069 gflanguages-0.4.6/data/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 10:36:16.311072 gflanguages-0.4.6/data/test/nunito/
--rw-r--r--   0 runner    (1001) docker     (123)   113832 2023-03-24 10:35:56.000000 gflanguages-0.4.6/data/test/nunito/Nunito-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-03-24 10:35:56.000000 gflanguages-0.4.6/data/test/nunito/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 10:35:56.000000 gflanguages-0.4.6/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-24 10:35:56.000000 gflanguages-0.4.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 10:36:16.311072 gflanguages-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-03-24 10:35:56.000000 gflanguages-0.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 10:36:16.311072 gflanguages-0.4.6/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-03-24 10:35:56.000000 gflanguages-0.4.6/snippets/fix-exemplars-duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-03-24 10:35:56.000000 gflanguages-0.4.6/snippets/supported_languages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 10:36:16.311072 gflanguages-0.4.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-03-24 10:35:56.000000 gflanguages-0.4.6/tests/test_data_languages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-03-24 10:35:56.000000 gflanguages-0.4.6/tests/test_dottedcircle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-03-24 10:35:56.000000 gflanguages-0.4.6/tests/test_gflanguages_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-24 10:35:56.000000 gflanguages-0.4.6/tests/test_parsable.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-24 10:35:56.000000 gflanguages-0.4.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:01:27.607752 gflanguages-0.4.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:01:27.283737 gflanguages-0.4.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:01:27.287737 gflanguages-0.4.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-13 10:01:11.000000 gflanguages-0.4.7/.github/workflows/publish-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-13 10:01:11.000000 gflanguages-0.4.7/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-13 10:01:11.000000 gflanguages-0.4.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-13 10:01:11.000000 gflanguages-0.4.7/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-04-13 10:01:11.000000 gflanguages-0.4.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-13 10:01:11.000000 gflanguages-0.4.7/CONTRIBUTORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10851 2023-04-13 10:01:11.000000 gflanguages-0.4.7/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:01:27.283737 gflanguages-0.4.7/Lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:01:27.287737 gflanguages-0.4.7/Lib/gflanguages/
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 10:01:26.000000 gflanguages-0.4.7/Lib/gflanguages/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:01:27.283737 gflanguages-0.4.7/Lib/gflanguages/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:01:27.547749 gflanguages-0.4.7/Lib/gflanguages/data/languages/
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/aa_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ab_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/abi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/abq_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/abr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/acd_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ace_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/acf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ach_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/acu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ada_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ade_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/adj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/adl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ady_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ae_Avst.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/aeb_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/aeb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/af_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/agc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/agq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/agr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/aha_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ahl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/aho_Ahom.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ahs_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Armi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Brah.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Chrs.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Egyp.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Elym.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Hatr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Mani.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Narb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Nbat.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Palm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Phli.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Phlp.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Phnx.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Prti.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Samr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Sarb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Sogd.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Sogo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Syrc.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Ugar.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ain_Kana.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ain_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ajg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ak_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/akk_Xsux.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/akp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/akz_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ala_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ale_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/aln_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/alt_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/am_Ethi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/amc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ame_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ami_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/amo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/amr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/an_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/anc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ang_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ank_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ann_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/anp_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/anv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/any_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/aoz_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/apd_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ar_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ar_Syrc.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/arb_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/arc_Armi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/arc_Nbat.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/arc_Palm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/arl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/arn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/aro_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/arp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/arq_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ars_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/art_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/arw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ary_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/arz_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/as_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/asa_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/asg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ast_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/atg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/atj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/auc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/av_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/avk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/avn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/avu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/awa_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/awo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ay_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ayb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/az_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/az_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/az_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/azb_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/azj_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ba_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ba_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bal_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bal_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ban_Bali.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ban_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bap_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bar_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bas_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bav_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bax_Bamu.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bax_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bba_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bbc_Batk.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bbc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bbj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bbp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bci_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bcn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bcq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bcw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bcy_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bdh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/be_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/be_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/beh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bej_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bej_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bem_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ber_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ber_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ber_Tfng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bet_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bew_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bex_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bez_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bfa_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bfd_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bfq_Taml.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bft_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bft_Tibt.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bfy_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bg_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bgc_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bgn_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bgx_Grek.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bhb_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bhi_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bhk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bho_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bho_Kthi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bhy_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bib_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bik_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bim_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bin_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/biv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bjj_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bjn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bjt_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bjv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bkc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bkm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bku_Buhd.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bku_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bkv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bla_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/blo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/blt_Tavt.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bm_Nkoo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bmq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bn_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bn_Newa.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bng_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bnm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bo_Marc.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     9698 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bo_Tibt.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bo_Zanb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/boa_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bom_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bov_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/box_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/boz_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bpy_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bqc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bqi_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bqj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bqp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bqv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/br_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bra_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/brh_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/brh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/brx_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6588 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/brx_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/brx_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bs_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bs_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bsc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bsj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bsp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bsq_Bass.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bsq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bss_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bto_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/btt_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/btv_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bua_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/buc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bud_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bug_Bugi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bug_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bum_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bus_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/buu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bvb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bvi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bwr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bwy_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/byh_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/byn_Ethi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/byn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bys_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/byv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bza_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bze_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bzw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/bzx_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ca_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cab_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cad_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cak_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/car_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cay_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cbi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cbj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cbk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cbr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cbs_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cbt_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cbu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cch_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ccp_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     9670 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ccp_Cakm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cdr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ce_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ceb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cfa_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cfm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cgg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ch_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/chj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/chk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/chm_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/chn_Dupl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/chn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cho_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/chp_Cans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/chp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/chr_Cher.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/chx_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/chy_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cic_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cja_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cja_Cham.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cjk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cjm_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cjm_Cham.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cjs_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cjy_Hans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ckb_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ckl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cko_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ckt_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cky_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cla_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cme_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cmg_Soyo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cnh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cni_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/co_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cof_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/con_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cop_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cop_Copt.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cop_Grek.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cot_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cpf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cps_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cpu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cr_Cans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/crh_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/crh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cri_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/crj_Cans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/crj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/crk_Cans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/crl_Cans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/crl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/crm_Cans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/crs_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cs_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/csa_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/csb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/csk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/csw_Cans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ctd_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ctd_Pauc.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cu_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cu_Glag.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cv_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cwe_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cy_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/cyo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/da_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/daa_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dag_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dak_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dar_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dav_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dbd_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dbq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dcc_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ddn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/de_Dupl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/de_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/de_Runr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/del_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/den_Cans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/den_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dga_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dgh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dgi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dgr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dhi_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dhw_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/did_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/din_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dip_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dje_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dmf_Medf.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dng_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dnj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/doi_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/doi_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/doi_Dogr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/doi_Takr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dop_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dow_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dri_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dsb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dtm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dtp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dts_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dty_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dua_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dug_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dum_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/duu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dv_Thaa.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dwr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dyi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dyo_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dyo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dyu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dyu_Nkoo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dz_Tibt.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/dzg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ebu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ee_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/efi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/egl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/egy_Egyp.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/eka_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ekm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/eky_Kali.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/el_Grek.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ema_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/emk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/en_Brai.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/en_Dsrt.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/en_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/en_Shaw.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/enm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/enn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/eo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/es_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ese_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/esg_Gonm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/esu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/et_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ett_Ital.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ett_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/etu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/etx_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/eu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/eve_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/evn_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/evn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ewo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ext_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/eza_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/fa_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/fan_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/fbl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7222 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ff_Adlm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ff_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ffm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/fi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/fia_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/fil_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/fil_Tglg.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/fit_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/fj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/fkv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/flr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/fmp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/fo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/fod_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/fon_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/fr_Dupl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/fr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/frc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/frm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/fro_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/frp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/frr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/frs_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/fub_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/fuc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/fud_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/fue_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/fuf_Adlm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/fuf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/fuh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/fuq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/fur_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/fuv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/fvr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/fy_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ga_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gaa_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gag_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gag_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gan_Hans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gay_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gba_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gbm_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gby_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gbz_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gcf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gcr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gd_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gde_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gej_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gel_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gem_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gez_Ethi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ggn_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ggn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gil_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/giw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gjk_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gjn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gju_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gju_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gkn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gkp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gld_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/glk_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gmh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gmm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gmv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gmy_Linb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gnd_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gng_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/god_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gof_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/goh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gom_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gon_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gon_Gong.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gon_Gonm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gon_Telu.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gor_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gos_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/got_Goth.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/got_Runr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gqr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/grb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/grc_Cprt.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/grc_Grek.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)    18660 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/grc_Linb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/grt_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gsw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gu_Gujr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gub_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/guc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gud_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/guk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gur_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/guu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/guw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gux_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/guz_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gvr_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gwi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gyi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/gyr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ha_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ha_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hag_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hai_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hak_Hans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hak_Hant.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hak_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/haw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/haz_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/he_Hebr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hea_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hi_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hi_Mahj.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hi_Newa.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hia_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hif_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hif_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hig_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hil_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hit_Xsux.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hlt_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hlu_Hluw.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hmd_Hmng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hmd_Plrd.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hmn_Hmng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hmn_Hmnp.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hmn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hms_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hna_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hnd_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hne_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hni_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hnj_Hmng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hnj_Laoo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hnj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hnn_Hano.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hnn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hno_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hns_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ho_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hoc_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hoc_Wara.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hoj_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hop_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hsb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hsn_Hans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ht_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hup_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hus_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/huu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hy_Armn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hyw_Armn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/hz_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ia_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/iba_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ibb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/iby_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ica_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ich_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/id_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/id_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/idd_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/idu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ie_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ife_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ig_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/igb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ige_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ii_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ii_Yiii.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ijj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ijs_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ik_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ikk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ikt_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ikw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ikx_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ilo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/inh_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/inh_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/inh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/io_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/iqw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/iri_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/is_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/it_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/iu_Cans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/iu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/izh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/izr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/izz_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ja_Hira.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)    14296 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ja_Jpan.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ja_Kana.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/jab_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/jam_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/jbo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/jbu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/jen_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/jgk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/jgo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/jib_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/jiv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/jmc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/jml_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/jpr_Hebr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/jra_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/jrb_Hebr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/jut_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8740 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/jv_Java.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/jv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ka_Geok.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ka_Geor.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kaa_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kab_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kab_Tfng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kac_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kad_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kai_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kaj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kam_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kao_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kbd_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kbp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kby_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kca_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kcg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kck_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kdc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kde_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kdh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kdl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kdt_Thai.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kea_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kek_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ken_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kez_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kfo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kfr_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kfy_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kge_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kgj_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kgp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kha_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kha_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/khb_Talu.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/khn_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/khq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/khr_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/khr_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/khr_Orya.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kht_Mymr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/khw_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/khw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ki_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kiu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kjg_Laoo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kjg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kjh_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kk_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kk_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kkh_Lana.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kkj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kln_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/km_Khmr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kmb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kmy_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kn_Knda.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/knc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/knf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/knp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ko_Kore.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/koi_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/koi_Perm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kok_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/koo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kos_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kpe_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kpo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kpy_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kqn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kqp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kqs_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kr_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/krc_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kri_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/krj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/krl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/krs_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kru_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ks_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ks_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ksb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ksf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ksh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ksp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ksw_Mymr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ktj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ktu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ku_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ku_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ku_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ku_Yezi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kub_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kuj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kum_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kun_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kus_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kut_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kv_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kv_Perm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kvf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kvr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kvx_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kwi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kxm_Thai.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kxp_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ky_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ky_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ky_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kye_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kyf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kyq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kyu_Kali.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kyw_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kyw_Orya.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/kzr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/la_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lab_Lina.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lad_Hebr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lad_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lag_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lah_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/laj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lam_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/las_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lbe_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lbw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lcp_Thai.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ldb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/led_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lee_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lem_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lep_Lepc.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/les_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lez_Aghb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lez_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lfn_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lfn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lgg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lhm_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/li_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lia_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lif_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lif_Limb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lig_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lij_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lip_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lis_Lisu.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/liv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ljp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lki_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lkt_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lld_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lln_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lmn_Telu.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lmo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lmp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ln_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lns_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lnu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lo_Laoo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lob_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/log_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lok_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lol_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/loq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lor_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lot_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/loz_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lrc_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lt_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ltg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lua_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lue_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lui_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lun_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/luo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lus_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lus_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lut_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/luy_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/luz_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lwl_Thai.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lwo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lzh_Hans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lzh_Hant.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lzh_Phag.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lzz_Geor.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/lzz_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mad_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/maf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mag_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mai_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mai_Newa.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mai_Tirh.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mak_Bugi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mak_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mam_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/man_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/man_Nkoo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mas_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/maw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/maz_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mbo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mbu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mcd_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mcf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mcp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mcu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mda_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mdf_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mdh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mdj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mdr_Bugi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mdr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mdt_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/men_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/men_Mend.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/meq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mer_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mey_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mfa_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mfe_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mfi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mfn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mfo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mfq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mfv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mgc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mgh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mgo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mgp_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mgy_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mhi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mic_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/min_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/min_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/miq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mis_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mis_Hatr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mis_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5199 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mis_Nshu.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mk_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mkl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7976 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ml_Mlym.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mls_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mlt_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mmu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mn_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mn_Mong.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mn_Phag.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mn_Zanb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mnc_Mong.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mnf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mni_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mni_Mtei.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mns_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mnw_Mymr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/moa_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/moe_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/moh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mor_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mos_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mqb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mql_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mr_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mr_Modi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mrd_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mrj_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mro_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mro_Mroo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mrw_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mrw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ms_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ms_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/msc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mt_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mto_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mtr_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mua_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/muh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mui_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mur_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mus_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/muy_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mvy_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mwk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mwl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mwr_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mwv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mww_Hmng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mxc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mxi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mxv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/my_Mymr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/myk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mym_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/myv_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/myx_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/myz_Mand.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mzi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mzk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mzm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mzn_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/mzw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/na_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nan_Hans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nan_Hant.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nan_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nap_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/naq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nat_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/naw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nba_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nch_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ncu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nd_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ndc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ndj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nds_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ndz_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ne_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ne_Newa.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/neb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/new_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/new_Newa.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nfr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ng_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nga_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ngb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ngl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ngp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nhb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nhe_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nhn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nhu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nhw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nia_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nij_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nin_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nio_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/niu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/niy_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/njo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nko_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nku_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nmg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nmz_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nnh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nnp_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nnp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nnp_Wcho.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nnq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nnw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/no_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nod_Lana.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/noe_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nog_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/non_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/non_Runr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/not_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nov_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nqo_Nkoo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nrb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nrf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nsk_Cans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nsk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nso_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nst_Tnsa.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ntm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ntr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nui_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nup_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nus_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nuv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nwb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nxq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ny_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nym_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nyn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nyo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/nzi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/oaa_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/oc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ogc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ohu_Hung.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/oj_Cans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/oj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ojb_Cans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/oki_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/okr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/om_Ethi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/om_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/omn_Lina.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/or_Orya.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/orh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/orv_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/os_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/osa_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/osa_Osge.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/osc_Ital.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/osc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ota_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ote_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/otk_Orkh.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/otn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/owl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ozm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pa_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6289 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pa_Guru.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pag_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pal_Phli.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pal_Phlp.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pam_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pap_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pau_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pbb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pbi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pcd_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pck_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pcm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pdc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pdt_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/peo_Xpeo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pfl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/phn_Phnx.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pi_Brah.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pi_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pi_Sinh.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pi_Thai.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pil_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pip_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pis_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/piu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pka_Brah.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pko_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pms_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/png_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pnt_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pnt_Grek.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pnt_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pon_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pov_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/poy_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ppl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pra_Khar.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/prd_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/prg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pro_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/prq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/prs_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ps_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pt_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/puu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pwo_Mymr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/pym_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/qu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/quc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/qud_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/qug_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/quh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/quy_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/quz_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/qva_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/qvc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/qvh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/qvm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/qvn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/qwh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/qxn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/qxu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rab_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/raj_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rap_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rar_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ray_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rcf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rej_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rej_Rjng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rel_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/res_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rgn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rhg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rhg_Rohg.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ria_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rif_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rif_Tfng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rjs_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rkt_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rmf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rmn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rmo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rmt_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rmu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rng_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ro_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ro_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rob_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rof_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rom_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rom_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rtm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ru_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rub_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rue_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ruf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rug_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rup_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/rwk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ryu_Jpan.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ryu_Kana.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Ahom.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Avst.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Bali.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Batk.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Bhks.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Brah.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Bugi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Buhd.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Cham.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)    36822 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Dogr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Gong.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Gonm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Gran.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Hano.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Khar.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Khoj.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Kthi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Lepc.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Limb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Mahj.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Marc.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Modi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Mong.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Mroo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Mtei.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Mult.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Nand.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Newa.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Olck.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Orya.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Phag.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Ranj.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Rjng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Saur.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Shrd.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Sidd.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Sind.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Sinh.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Sora.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Soyo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Sund.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Sylo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Tagb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Takr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Tirh.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Wara.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Wcho.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Xpeo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Zanb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sad_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/saf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sah_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sam_Hebr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sam_Samr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/saq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sas_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sat_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sat_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sat_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sat_Olck.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sat_Orya.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sav_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/saz_Saur.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sba_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sbp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sck_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/scn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sco_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/scs_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sd_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sd_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sd_Khoj.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sd_Sind.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sdc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sdh_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/se_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/se_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/see_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sef_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/seh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sei_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sel_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ses_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sey_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sga_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sga_Ogam.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sgs_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/she_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/shi_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/shi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/shi_Tfng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/shk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/shn_Mymr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/shp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/shu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/si_Sinh.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sid_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sig_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sil_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sja_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/skr_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/skr_Mult.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sla_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sld_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sli_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/slr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sly_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sma_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/smj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/smn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/smp_Samr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sms_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/snf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/snk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/snn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/snw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/so_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/so_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/so_Osma.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sog_Sogd.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sog_Sogo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sok_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sou_Thai.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/soy_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/spp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sq_Elba.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sr_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/srb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/srb_Sora.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/srn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/srr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/srx_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ss_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ssy_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/st_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/stq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/str_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/su_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/su_Sund.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/suk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/suq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sur_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sus_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sus_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/swb_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/swb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/swc_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/swg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/swv_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sxb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sxn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/sxw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/syc_Syrc.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/syi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/syl_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/syl_Sylo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/syr_Syrc.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/szl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7943 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ta_Taml.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tab_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/taj_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/taj_Tibt.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tal_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tan_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/taq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/taq_Tfng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tbw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tbw_Tagb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tbz_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tca_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tcy_Knda.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tdd_Tale.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tdg_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tdg_Tibt.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tdh_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tdt_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/te_Telu.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ted_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tem_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/teo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ter_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tet_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tfi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tg_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tg_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/th_Thai.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/thf_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/thl_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/thq_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/thr_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ths_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ti_Ethi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tig_Ethi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tik_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tiv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tiw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tjs_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tk_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tk_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tk_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tke_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tkl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tkr_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tkr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tkt_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tlh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tli_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tlj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tly_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tly_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tly_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tmh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tn_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tnr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/to_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tob_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tod_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tog_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/toi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/toj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/top_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/toq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tpi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tpm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tr_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/trp_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tru_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tru_Syrc.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/trv_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/trw_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ts_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tsd_Grek.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tsf_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tsg_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tsi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tsj_Tibt.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tsw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tsz_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tt_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tt_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tt_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ttj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ttr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tts_Thai.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ttt_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ttt_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ttt_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tul_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tum_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tuq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tvd_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tvl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tvu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/twq_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6492 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/txg_Tang.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/txo_Toto.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ty_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tyv_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tzh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tzm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tzm_Tfng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/tzo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ude_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/udm_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/udm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/udu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ug_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ug_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ug_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/uga_Ugar.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/uk_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/uli_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/umb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/unr_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/unr_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/unr_Nagm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/unr_Orya.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/unx_Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/unx_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ur_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ura_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/uth_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/utr_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/uz_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/uz_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/uz_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/vag_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/vai_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/vai_Vaii.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ve_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/vec_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/vep_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/vi_Hani.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/vi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/vic_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/vid_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/vls_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/vmf_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/vmw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/vo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/vot_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/vro_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/vun_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/vut_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/wa_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/wae_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/wal_Ethi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/wal_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/wan_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/war_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/was_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/wbp_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/wbq_Telu.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/wbr_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/wci_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/wib_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/wja_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/wji_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/wls_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/wmw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/wni_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/wo_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/wo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/wob_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/wsg_Gonm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/wtm_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/wuu_Hans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/wwa_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/xal_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/xav_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/xcr_Cari.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/xed_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/xh_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/xlc_Lyci.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/xld_Lydi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/xly_Elym.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/xmf_Geor.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/xmn_Mani.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/xmr_Merc.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/xmr_Mero.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/xna_Narb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/xnr_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/xog_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/xon_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/xpr_Prti.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/xrb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/xsa_Sarb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/xsm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/xsr_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/xum_Ital.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/xum_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/xuo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/xwe_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/yad_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/yal_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/yam_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/yao_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/yap_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/yas_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/yat_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/yav_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/yay_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/yaz_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/yba_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ybb_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ybh_Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/yer_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/yi_Hebr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ykg_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/yko_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/yo_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/yre_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/yrk_Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/yrl_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/yua_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/yue_Hani.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)    13480 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/yue_Hans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/yue_Hant.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/za_Hans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/za_Hant.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/za_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/zag_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/zam_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/zap_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/zay_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/zdj_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/zdj_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/zea_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/zen_Tfng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/zgh_Tfng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)    15684 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/zh_Hans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)    15600 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/zh_Hant.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/zh_Hebr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/zh_Phag.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ziw_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/zlm_Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/zlm_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/zmi_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/zne_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/zro_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/ztu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/zu_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/zul_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/zun_Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/languages/zza_Latn.textproto
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:01:27.583751 gflanguages-0.4.7/Lib/gflanguages/data/regions/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/AC.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/AD.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/AE.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/AF.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/AG.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/AI.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/AL.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/AM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/AO.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/AQ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/AR.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/AS.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/AT.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/AU.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/AW.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/AX.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/AZ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/BA.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/BB.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/BD.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/BE.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/BF.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/BG.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/BH.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/BI.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/BJ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/BL.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/BM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/BN.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/BO.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/BQ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/BR.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/BS.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/BT.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/BV.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/BW.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/BY.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/BZ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/CA.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/CC.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/CD.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/CF.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/CG.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/CH.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/CI.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/CK.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/CL.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/CM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/CN.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/CO.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/CP.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/CR.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/CU.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/CV.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/CW.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/CX.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/CY.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/CZ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/DE.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/DG.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/DJ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/DK.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/DM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/DO.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/DZ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/EA.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/EC.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/EE.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/EG.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/EH.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/ER.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/ES.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/ET.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/FI.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/FJ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/FK.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/FM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/FO.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/FR.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/GA.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/GB.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/GD.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/GE.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/GF.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/GG.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/GH.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/GI.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/GL.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/GM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/GN.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/GP.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/GQ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/GR.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/GS.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/GT.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/GU.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/GW.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/GY.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/HK.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/HM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/HN.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/HR.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/HT.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/HU.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/IC.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/ID.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/IE.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/IL.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/IM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/IN.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/IO.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/IQ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/IR.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/IS.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/IT.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/JE.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/JM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/JO.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/JP.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/KE.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/KG.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/KH.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/KI.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/KM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/KN.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/KP.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/KR.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/KW.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/KY.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/KZ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/LA.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/LB.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/LC.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/LI.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/LK.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/LR.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/LS.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/LT.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/LU.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/LV.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/LY.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/MA.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/MC.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/MD.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/ME.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/MF.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/MG.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/MH.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/MK.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/ML.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/MM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/MN.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/MO.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/MP.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/MQ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/MR.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/MS.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/MT.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/MU.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/MV.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/MW.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/MX.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/MY.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/MZ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/NA.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/NC.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/NE.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/NF.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/NG.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/NI.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/NL.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/NO.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/NP.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/NR.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/NU.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/NZ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/OM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/PA.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/PE.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/PF.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/PG.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/PH.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/PK.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/PL.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/PM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/PN.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/PR.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/PS.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/PT.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/PW.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/PY.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/QA.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/RE.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/RO.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/RS.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/RU.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/RW.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/SA.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/SB.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/SC.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/SD.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/SE.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/SG.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/SH.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/SI.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/SJ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/SK.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/SL.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/SM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/SN.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/SO.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/SR.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/SS.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/ST.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/SV.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/SX.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/SY.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/SZ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/TA.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/TC.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/TD.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/TF.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/TG.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/TH.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/TJ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/TK.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/TL.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/TM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/TN.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/TO.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/TR.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/TT.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/TV.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/TW.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/TZ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/UA.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/UG.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/UM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/US.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/UY.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/UZ.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/VA.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/VC.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/VE.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/VG.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/VI.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/VN.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/VU.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/WF.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/WS.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/XK.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/YE.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/YT.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/ZA.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/ZM.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/regions/ZW.textproto
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:01:27.607752 gflanguages-0.4.7/Lib/gflanguages/data/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Adlm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Aghb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Ahom.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Arab.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Aran.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Armi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Armn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Avst.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Bali.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Bamu.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Bass.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Batk.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Beng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Bhks.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Brah.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Brai.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Bugi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Buhd.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Cakm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Cans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Cari.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Cham.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Cher.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Chrs.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Copt.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Cprt.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Cyrl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Deva.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Dogr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Dsrt.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Dupl.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Egyp.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Elba.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Elym.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Ethi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Geok.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Geor.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Glag.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Gong.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Gonm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Goth.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Gran.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Grek.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Gujr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Guru.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Hani.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Hano.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Hans.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Hant.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Hatr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Hebr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Hira.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Hluw.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Hmng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Hmnp.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Hung.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Ital.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Java.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Jpan.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Kali.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Kana.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Khar.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Khmr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Khoj.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Knda.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Kore.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Kthi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Lana.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Laoo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Latn.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Lepc.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Limb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Lina.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Linb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Lisu.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Lyci.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Lydi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Mahj.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Mand.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Mani.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Marc.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Medf.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Mend.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Merc.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Mero.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Mlym.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Modi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Mong.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Mroo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Mtei.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Mult.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Mymr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Nagm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Nand.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Narb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Nbat.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Newa.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Nkoo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Nshu.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Ogam.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Olck.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Orkh.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Orya.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Osge.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Osma.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Palm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Pauc.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Perm.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Phag.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Phli.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Phlp.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Phnx.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Plrd.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Prti.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Ranj.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Rjng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Rohg.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Runr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Samr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Sarb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Saur.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Shaw.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Shrd.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Sidd.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Sind.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Sinh.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Sogd.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Sogo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Sora.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Soyo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Sund.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Sylo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Syrc.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Tagb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Takr.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Tale.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Talu.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Taml.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Tang.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Tavt.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Telu.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Tfng.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Tglg.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Thaa.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Thai.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Tibt.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Tirh.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Tnsa.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Toto.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Ugar.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Vaii.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Wara.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Wcho.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Xpeo.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Xsux.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Yezi.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Yiii.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/data/scripts/Zanb.textproto
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/languages_public.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    23492 2023-04-13 10:01:11.000000 gflanguages-0.4.7/Lib/gflanguages/languages_public_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:01:27.287737 gflanguages-0.4.7/Lib/gflanguages.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-13 10:01:26.000000 gflanguages-0.4.7/Lib/gflanguages.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    97743 2023-04-13 10:01:27.000000 gflanguages-0.4.7/Lib/gflanguages.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 10:01:26.000000 gflanguages-0.4.7/Lib/gflanguages.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 10:01:26.000000 gflanguages-0.4.7/Lib/gflanguages.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-13 10:01:26.000000 gflanguages-0.4.7/Lib/gflanguages.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 10:01:26.000000 gflanguages-0.4.7/Lib/gflanguages.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-13 10:01:27.607752 gflanguages-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-13 10:01:11.000000 gflanguages-0.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:01:27.287737 gflanguages-0.4.7/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:01:27.287737 gflanguages-0.4.7/data/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:01:27.607752 gflanguages-0.4.7/data/test/nunito/
+-rw-r--r--   0 runner    (1001) docker     (123)   113832 2023-04-13 10:01:11.000000 gflanguages-0.4.7/data/test/nunito/Nunito-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-04-13 10:01:11.000000 gflanguages-0.4.7/data/test/nunito/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 10:01:11.000000 gflanguages-0.4.7/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 10:01:11.000000 gflanguages-0.4.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 10:01:27.607752 gflanguages-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-13 10:01:11.000000 gflanguages-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:01:27.607752 gflanguages-0.4.7/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-13 10:01:11.000000 gflanguages-0.4.7/snippets/fix-exemplars-duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-13 10:01:11.000000 gflanguages-0.4.7/snippets/supported_languages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:01:27.607752 gflanguages-0.4.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-13 10:01:11.000000 gflanguages-0.4.7/tests/test_data_languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-13 10:01:11.000000 gflanguages-0.4.7/tests/test_dottedcircle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-13 10:01:11.000000 gflanguages-0.4.7/tests/test_gflanguages_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-13 10:01:11.000000 gflanguages-0.4.7/tests/test_parsable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-13 10:01:11.000000 gflanguages-0.4.7/tox.ini
```

### Comparing `gflanguages-0.4.6/.github/workflows/publish-release.yml` & `gflanguages-0.4.7/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/.github/workflows/tox.yml` & `gflanguages-0.4.7/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/CHANGELOG.md` & `gflanguages-0.4.7/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 Below are the most important changes from each release.
 
 ## Next release
 
+## 0.4.7
+- #70 Add Nandinagari
+
 ## 0.4.6 (2023-Mar-24)
 - #52 Addition of exemplar character sets for Latin-based African Lang
 uages
 - #53 Adding caps letters to Latin-based African languages that have gflang profiles
 - #67 Add kana sample text
 
 ## 0.4.5 (2023-Mars-22)
```

### Comparing `gflanguages-0.4.6/CONTRIBUTORS.txt` & `gflanguages-0.4.7/CONTRIBUTORS.txt`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/LICENSE.txt` & `gflanguages-0.4.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/__init__.py` & `gflanguages-0.4.7/Lib/gflanguages/__init__.py`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/aa_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/aa_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ab_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ab_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ace_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ace_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/acf_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/acf_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/acu_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/acu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ada_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ada_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/adl_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/adl_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ady_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ady_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/af_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/af_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/agq_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/agq_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/agr_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/agr_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Armi.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Armi.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Brah.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Brah.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Chrs.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Chrs.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Egyp.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Egyp.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Elym.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Elym.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Hatr.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Hatr.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Mani.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Mani.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Narb.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Narb.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Nbat.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Nbat.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Palm.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Palm.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Phli.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Phli.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Phlp.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Phlp.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Phnx.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Phnx.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Prti.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Prti.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Samr.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Samr.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Sarb.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Sarb.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Sogd.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Sogd.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Sogo.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Sogo.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Syrc.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Syrc.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/aii_Ugar.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/aii_Ugar.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ajg_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ajg_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ak_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ak_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/akk_Xsux.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/akk_Xsux.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ale_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ale_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/aln_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/aln_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/alt_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/alt_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/am_Ethi.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/am_Ethi.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/amc_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/amc_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ame_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ame_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ami_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ami_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/amr_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/amr_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/an_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/an_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ang_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ang_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ar_Arab.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ar_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/arb_Arab.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/arb_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/arc_Armi.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/arc_Armi.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/arc_Nbat.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/arc_Nbat.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/arc_Palm.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/arc_Palm.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/arl_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/arl_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/arn_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/arn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/arp_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/arp_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/art_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/art_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/arz_Arab.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/arz_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/as_Beng.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/as_Beng.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ast_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ast_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/auc_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/auc_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/awa_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/awa_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ay_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ay_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/az_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/az_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/az_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/az_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/azb_Arab.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/azb_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/azj_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/azj_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ba_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ba_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ba_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ba_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ban_Bali.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ban_Bali.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ban_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ban_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/bap_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/bap_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/bas_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/bas_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/bax_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/bax_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/bba_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/bba_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/bci_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/bci_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/be_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/be_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/be_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/be_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/bem_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/bem_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/bew_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/bew_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/bfa_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/bfa_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/bg_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/bg_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/bho_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/bho_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/bi_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/bi_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/bik_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/bik_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/bin_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/bin_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/bjj_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/bjj_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/blt_Tavt.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/blt_Tavt.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/bm_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/bm_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/bn_Beng.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/bn_Beng.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/bo_Tibt.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/bo_Tibt.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/boa_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/boa_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/bpy_Beng.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/bpy_Beng.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/br_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/br_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/brh_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/brh_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/brx_Beng.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/brx_Beng.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/brx_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/brx_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/brx_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/brx_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/bs_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/bs_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/bs_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/bs_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/bsq_Bass.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/bsq_Bass.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/bua_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/bua_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/buc_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/buc_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/bug_Bugi.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/bug_Bugi.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/bug_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/bug_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/bum_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/bum_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/bvi_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/bvi_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/bwy_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/bwy_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/byh_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/byh_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ca_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ca_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/cab_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/cab_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/cak_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/cak_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/cbi_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/cbi_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/cbk_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/cbk_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/cbr_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/cbr_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/cbs_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/cbs_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/cbt_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/cbt_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/cbu_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/cbu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ccp_Beng.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ccp_Beng.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ccp_Cakm.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ccp_Cakm.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ce_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ce_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ceb_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ceb_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/cfm_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/cfm_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ch_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ch_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/chj_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/chj_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/chk_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/chk_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/chr_Cher.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/chr_Cher.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/chx_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/chx_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/cic_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/cic_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/cjk_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/cjk_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/cjs_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/cjs_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/cjy_Hans.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/cjy_Hans.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ckb_Arab.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ckb_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/cnh_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/cnh_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/cni_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/cni_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/co_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/co_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/cof_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/cof_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/con_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/con_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/cop_Copt.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/cop_Copt.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/cot_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/cot_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/cpu_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/cpu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/crh_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/crh_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/cri_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/cri_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/crs_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/crs_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/cs_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/cs_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/csa_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/csa_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/csb_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/csb_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/csw_Cans.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/csw_Cans.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ctd_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ctd_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/cu_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/cu_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/cu_Glag.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/cu_Glag.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/cv_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/cv_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/cy_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/cy_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/cyo_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/cyo_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/da_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/da_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/dag_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/dag_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ddn_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ddn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/de_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/de_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/dga_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/dga_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/dhi_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/dhi_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/dhw_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/dhw_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/dip_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/dip_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/dmf_Medf.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/dmf_Medf.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/doi_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/doi_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/dsb_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/dsb_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/dtp_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/dtp_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/dty_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/dty_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/duu_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/duu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/dv_Thaa.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/dv_Thaa.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/dyo_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/dyo_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/dyu_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/dyu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/dz_Tibt.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/dz_Tibt.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ee_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ee_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/egy_Egyp.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/egy_Egyp.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/el_Grek.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/el_Grek.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/emk_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/emk_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/en_Brai.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/en_Brai.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/en_Dsrt.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/en_Dsrt.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/en_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/en_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/en_Shaw.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/en_Shaw.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/eo_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/eo_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/es_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/es_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ese_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ese_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/et_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/et_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ett_Ital.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ett_Ital.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/eu_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/eu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/eve_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/eve_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/evn_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/evn_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ewo_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ewo_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ext_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ext_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/fa_Arab.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/fa_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ff_Adlm.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ff_Adlm.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ff_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ff_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/fi_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/fi_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/fil_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/fil_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/fil_Tglg.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/fil_Tglg.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/fj_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/fj_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/fkv_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/fkv_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/fo_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/fo_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/fon_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/fon_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/fr_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/fr_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/fro_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/fro_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/frp_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/frp_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/frr_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/frr_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/fuc_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/fuc_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/fuf_Adlm.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/fuf_Adlm.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/fuf_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/fuf_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/fur_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/fur_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/fuv_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/fuv_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/fvr_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/fvr_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/fy_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/fy_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ga_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ga_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/gaa_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/gaa_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/gag_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/gag_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/gag_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/gag_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/gan_Hans.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/gan_Hans.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/gbz_Arab.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/gbz_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/gcf_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/gcf_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/gcr_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/gcr_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/gd_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/gd_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/gem_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/gem_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/gez_Ethi.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/gez_Ethi.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/giw_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/giw_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/gjn_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/gjn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/gju_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/gju_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/gkp_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/gkp_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/gl_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/gl_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/gld_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/gld_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/gmh_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/gmh_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/gmy_Linb.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/gmy_Linb.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/gn_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/gn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/goh_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/goh_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/gom_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/gom_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/got_Goth.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/got_Goth.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/got_Runr.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/got_Runr.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/grc_Cprt.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/grc_Cprt.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/grc_Grek.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/grc_Grek.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/grc_Linb.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/grc_Linb.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/gsw_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/gsw_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/gu_Gujr.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/gu_Gujr.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/guc_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/guc_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/guu_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/guu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/gv_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/gv_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/gyr_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/gyr_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ha_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ha_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/hak_Hans.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/hak_Hans.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/haw_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/haw_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/he_Hebr.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/he_Hebr.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/hea_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/hea_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/hi_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/hi_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/hil_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/hil_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/hit_Xsux.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/hit_Xsux.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/hlt_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/hlt_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/hlu_Hluw.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/hlu_Hluw.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/hmd_Plrd.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/hmd_Plrd.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/hmn_Hmng.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/hmn_Hmng.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/hmn_Hmnp.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/hmn_Hmnp.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/hmn_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/hmn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/hms_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/hms_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/hna_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/hna_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/hne_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/hne_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/hni_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/hni_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/hnj_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/hnj_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/hns_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/hns_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/hoc_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/hoc_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/hr_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/hr_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/hsb_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/hsb_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/hsn_Hans.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/hsn_Hans.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ht_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ht_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/hu_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/hu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/hus_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/hus_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/huu_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/huu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/hy_Armn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/hy_Armn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/hyw_Armn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/hyw_Armn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ia_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ia_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ibb_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ibb_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/id_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/id_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/idu_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/idu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ie_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ie_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ig_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ig_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ii_Yiii.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ii_Yiii.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ijs_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ijs_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ilo_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ilo_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/io_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/io_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/is_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/is_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/it_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/it_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/iu_Cans.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/iu_Cans.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ja_Hira.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ja_Hira.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ja_Jpan.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ja_Jpan.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ja_Kana.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ja_Kana.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/jbo_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/jbo_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/jgo_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/jgo_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/jiv_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/jiv_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/jra_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/jra_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/jv_Java.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/jv_Java.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/jv_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/jv_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ka_Geok.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ka_Geok.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ka_Geor.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ka_Geor.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/kaa_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/kaa_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/kab_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/kab_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/kab_Tfng.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/kab_Tfng.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/kbd_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/kbd_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/kbp_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/kbp_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/kde_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/kde_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/kdh_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/kdh_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/kea_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/kea_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/kek_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/kek_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/kg_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/kg_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/kgj_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/kgj_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/kha_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/kha_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/khb_Talu.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/khb_Talu.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/khr_Beng.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/khr_Beng.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/khr_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/khr_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/khr_Orya.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/khr_Orya.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/khw_Arab.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/khw_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/khw_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/khw_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/kjh_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/kjh_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/kk_Arab.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/kk_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/kk_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/kk_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/kk_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/kk_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/kkh_Lana.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/kkh_Lana.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/kkj_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/kkj_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/kl_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/kl_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/km_Khmr.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/km_Khmr.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/kmb_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/kmb_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/kn_Knda.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/kn_Knda.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/knc_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/knc_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ko_Kore.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ko_Kore.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/koi_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/koi_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/kok_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/kok_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/koo_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/koo_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/kqn_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/kqn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/kqs_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/kqs_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/kr_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/kr_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/krc_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/krc_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/kri_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/kri_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/krl_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/krl_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/kru_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/kru_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ks_Arab.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ks_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ksh_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ksh_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ksw_Mymr.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ksw_Mymr.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ktu_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ktu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ku_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ku_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ku_Yezi.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ku_Yezi.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/kw_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/kw_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/kwi_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/kwi_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ky_Arab.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ky_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ky_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ky_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/kyu_Kali.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/kyu_Kali.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/kyw_Beng.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/kyw_Beng.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/kyw_Orya.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/kyw_Orya.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/la_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/la_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/lad_Hebr.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/lad_Hebr.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/lad_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/lad_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/lah_Arab.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/lah_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/lb_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/lb_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/lfn_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/lfn_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/lfn_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/lfn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/lg_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/lg_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/lhm_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/lhm_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/lia_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/lia_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/lif_Limb.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/lif_Limb.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/lij_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/lij_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/lis_Lisu.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/lis_Lisu.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/liv_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/liv_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ljp_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ljp_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/lkt_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/lkt_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/lld_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/lld_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/lmo_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/lmo_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ln_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ln_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/lns_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/lns_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/lo_Laoo.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/lo_Laoo.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/lob_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/lob_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/lot_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/lot_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/loz_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/loz_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/lrc_Arab.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/lrc_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/lt_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/lt_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/lu_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/lu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/lua_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/lua_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/lue_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/lue_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/lun_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/lun_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/lus_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/lus_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/lut_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/lut_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/lv_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/lv_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mad_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mad_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mag_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mag_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mai_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mai_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mam_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mam_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/man_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/man_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mas_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mas_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/maz_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/maz_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mcd_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mcd_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mcf_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mcf_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/men_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/men_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/men_Mend.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/men_Mend.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mfe_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mfe_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mfq_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mfq_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mg_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mg_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mgo_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mgo_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mh_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mh_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mi_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mi_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mic_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mic_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/min_Arab.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/min_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/min_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/min_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/miq_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/miq_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mis_Arab.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mis_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mis_Hatr.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mis_Hatr.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mis_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mis_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mis_Nshu.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mis_Nshu.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mk_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mk_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ml_Mlym.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ml_Mlym.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mn_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mn_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mn_Mong.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mn_Mong.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mni_Beng.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mni_Beng.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mni_Mtei.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mni_Mtei.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mnw_Mymr.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mnw_Mymr.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mor_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mor_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mos_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mos_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mr_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mr_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mr_Modi.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mr_Modi.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mrw_Arab.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mrw_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mrw_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mrw_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ms_Arab.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ms_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mt_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mt_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mto_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mto_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mui_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mui_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mus_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mus_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mxi_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mxi_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mxv_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mxv_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/my_Mymr.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/my_Mymr.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/myz_Mand.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/myz_Mand.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/mzi_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/mzi_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/nan_Hans.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/nan_Hans.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/nan_Hant.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/nan_Hant.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/nap_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/nap_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/nb_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/nb_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/nba_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/nba_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/nds_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/nds_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ne_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ne_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/new_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/new_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/new_Newa.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/new_Newa.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ng_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ng_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/nhn_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/nhn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/nio_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/nio_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/niu_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/niu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/njo_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/njo_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/nku_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/nku_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/nl_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/nl_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/nmg_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/nmg_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/nn_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/nn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/nnh_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/nnh_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/nnp_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/nnp_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/nnp_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/nnp_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/nnp_Wcho.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/nnp_Wcho.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/non_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/non_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/non_Runr.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/non_Runr.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/not_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/not_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/nqo_Nkoo.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/nqo_Nkoo.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/nr_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/nr_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/nrf_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/nrf_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/nso_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/nso_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/nst_Tnsa.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/nst_Tnsa.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/nus_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/nus_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/nv_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/nv_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ny_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ny_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/nym_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/nym_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/nyn_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/nyn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/nzi_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/nzi_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/oaa_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/oaa_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/oc_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/oc_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ohu_Hung.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ohu_Hung.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ojb_Cans.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ojb_Cans.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/oki_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/oki_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/om_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/om_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/or_Orya.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/or_Orya.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/orh_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/orh_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/orv_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/orv_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/os_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/os_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/osa_Osge.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/osa_Osge.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/osc_Ital.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/osc_Ital.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ota_Arab.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ota_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ote_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ote_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/otk_Orkh.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/otk_Orkh.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/otn_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/otn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/owl_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/owl_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/pa_Guru.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/pa_Guru.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/pal_Phli.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/pal_Phli.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/pam_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/pam_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/pap_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/pap_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/pau_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/pau_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/pbb_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/pbb_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/pcd_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/pcd_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/pck_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/pck_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/pcm_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/pcm_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/phn_Phnx.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/phn_Phnx.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/pis_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/pis_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/piu_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/piu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/pl_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/pl_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/pms_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/pms_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/pon_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/pon_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/pov_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/pov_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ppl_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ppl_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/pro_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/pro_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/prq_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/prq_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ps_Arab.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ps_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/pt_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/pt_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/pwo_Mymr.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/pwo_Mymr.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/qu_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/qu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/quc_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/quc_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/qud_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/qud_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/qug_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/qug_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/quh_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/quh_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/quy_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/quy_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/quz_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/quz_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/qva_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/qva_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/qvc_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/qvc_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/qvh_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/qvh_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/qvm_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/qvm_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/qvn_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/qvn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/qwh_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/qwh_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/qxn_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/qxn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/qxu_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/qxu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/rab_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/rab_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/rar_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/rar_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ray_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ray_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/rcf_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/rcf_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/rej_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/rej_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/rej_Rjng.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/rej_Rjng.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/rgn_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/rgn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/rhg_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/rhg_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/rhg_Rohg.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/rhg_Rohg.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/rkt_Beng.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/rkt_Beng.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/rm_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/rm_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/rmn_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/rmn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/rn_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/rn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ro_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ro_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ro_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ro_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ru_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ru_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/rue_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/rue_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/rup_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/rup_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/rw_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/rw_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Ahom.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Ahom.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Avst.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Avst.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Bali.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Bali.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Batk.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Batk.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Bhks.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Bhks.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Brah.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Brah.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Bugi.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Bugi.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Buhd.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Buhd.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Cham.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Cham.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Dogr.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Dogr.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Gong.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Gong.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Gonm.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Gonm.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Gran.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Gran.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Hano.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Hano.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Khar.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Khar.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Khoj.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Khoj.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Kthi.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Kthi.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Lepc.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Lepc.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Limb.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Limb.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Mahj.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Mahj.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Marc.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Marc.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Modi.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Modi.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Mong.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Mong.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Mroo.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Mroo.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Mtei.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Mtei.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Mult.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Mult.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Newa.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Newa.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Olck.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Olck.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Orya.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Orya.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Phag.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Phag.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Ranj.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Ranj.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Rjng.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Rjng.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Saur.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Saur.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Shrd.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Shrd.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Sidd.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Sidd.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Sind.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Sind.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Sinh.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Sinh.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Sora.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Sora.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Soyo.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Soyo.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Sund.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Sund.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Sylo.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Sylo.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Tagb.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Tagb.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Takr.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Takr.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Tirh.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Tirh.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Wara.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Wara.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Wcho.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Wcho.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Xpeo.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Xpeo.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sa_Zanb.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sa_Zanb.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sah_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sah_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sas_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sas_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sat_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sat_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sc_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sc_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/scn_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/scn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sco_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sco_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sd_Arab.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sd_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sd_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sd_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/se_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/se_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sey_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sey_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sg_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sg_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sga_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sga_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sga_Ogam.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sga_Ogam.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/shi_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/shi_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/shk_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/shk_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/shn_Mymr.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/shn_Mymr.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/shp_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/shp_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/si_Sinh.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/si_Sinh.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sja_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sja_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sk_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sk_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/skr_Arab.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/skr_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sl_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sl_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sla_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sla_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/slr_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/slr_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sm_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sm_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/smn_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/smn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/smp_Samr.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/smp_Samr.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sn_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/snk_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/snk_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/snn_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/snn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/so_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/so_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/so_Osma.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/so_Osma.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sq_Elba.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sq_Elba.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sq_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sq_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sr_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sr_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sr_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sr_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/srn_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/srn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/srr_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/srr_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ss_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ss_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/st_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/st_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/stq_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/stq_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/str_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/str_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/su_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/su_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/su_Sund.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/su_Sund.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/suk_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/suk_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sus_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sus_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sv_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sv_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/sw_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/sw_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/swb_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/swb_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/syc_Syrc.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/syc_Syrc.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/syl_Beng.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/syl_Beng.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/syl_Sylo.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/syl_Sylo.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/szl_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/szl_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ta_Taml.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ta_Taml.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/taj_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/taj_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/taj_Tibt.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/taj_Tibt.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/taq_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/taq_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/taq_Tfng.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/taq_Tfng.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/tbw_Tagb.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/tbw_Tagb.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/tbz_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/tbz_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/tca_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/tca_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/tdd_Tale.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/tdd_Tale.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/tdt_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/tdt_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/te_Telu.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/te_Telu.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/tem_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/tem_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/tet_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/tet_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/tg_Arab.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/tg_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/tg_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/tg_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/tg_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/tg_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/th_Thai.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/th_Thai.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/thf_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/thf_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ths_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ths_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ti_Ethi.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ti_Ethi.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/tiv_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/tiv_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/tiw_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/tiw_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/tjs_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/tjs_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/tk_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/tk_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/tk_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/tk_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/tly_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/tly_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/tn_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/tn_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/to_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/to_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/tob_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/tob_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/toi_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/toi_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/toj_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/toj_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/top_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/top_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/tpi_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/tpi_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/tr_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/tr_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/trp_Beng.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/trp_Beng.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/tru_Syrc.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/tru_Syrc.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ts_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ts_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/tsz_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/tsz_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/tt_Arab.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/tt_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/tt_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/tt_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/tt_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/tt_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/tvl_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/tvl_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/txg_Tang.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/txg_Tang.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/txo_Toto.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/txo_Toto.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ty_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ty_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/tyv_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/tyv_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/tzh_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/tzh_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/tzm_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/tzm_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/tzo_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/tzo_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/udu_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/udu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ug_Arab.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ug_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ug_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ug_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ug_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ug_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/uga_Ugar.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/uga_Ugar.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/uk_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/uk_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/umb_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/umb_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/unr_Beng.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/unr_Beng.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/unr_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/unr_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/unr_Nagm.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/unr_Nagm.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/unr_Orya.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/unr_Orya.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/unx_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/unx_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ur_Arab.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ur_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ura_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ura_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/uz_Arab.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/uz_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/uz_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/uz_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/uz_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/uz_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/vai_Vaii.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/vai_Vaii.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ve_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ve_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/vec_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/vec_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/vep_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/vep_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/vi_Hani.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/vi_Hani.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/vi_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/vi_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/vmw_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/vmw_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/vo_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/vo_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/vro_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/vro_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/wa_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/wa_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/wae_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/wae_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/war_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/war_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/wo_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/wo_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/wuu_Hans.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/wuu_Hans.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/wwa_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/wwa_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/xcr_Cari.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/xcr_Cari.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/xh_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/xh_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/xlc_Lyci.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/xlc_Lyci.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/xld_Lydi.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/xld_Lydi.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/xly_Elym.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/xly_Elym.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/xmn_Mani.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/xmn_Mani.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/xna_Narb.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/xna_Narb.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/xnr_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/xnr_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/xpr_Prti.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/xpr_Prti.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/xsa_Sarb.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/xsa_Sarb.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/xsm_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/xsm_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/xsr_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/xsr_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/yad_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/yad_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/yao_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/yao_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/yap_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/yap_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/yav_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/yav_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ybh_Deva.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ybh_Deva.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/yi_Hebr.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/yi_Hebr.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ykg_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ykg_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/yo_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/yo_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/yrk_Cyrl.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/yrk_Cyrl.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/yua_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/yua_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/yue_Hani.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/yue_Hani.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/yue_Hans.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/yue_Hans.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/yue_Hant.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/yue_Hant.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/za_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/za_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/zam_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/zam_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/zdj_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/zdj_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/zgh_Tfng.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/zgh_Tfng.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/zh_Hans.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/zh_Hans.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/zh_Hant.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/zh_Hant.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/zh_Hebr.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/zh_Hebr.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/zlm_Arab.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/zlm_Arab.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/zlm_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/zlm_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/zro_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/zro_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/ztu_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/ztu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/zu_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/zu_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/data/languages/zza_Latn.textproto` & `gflanguages-0.4.7/Lib/gflanguages/data/languages/zza_Latn.textproto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/languages_public.proto` & `gflanguages-0.4.7/Lib/gflanguages/languages_public.proto`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages/languages_public_pb2.py` & `gflanguages-0.4.7/Lib/gflanguages/languages_public_pb2.py`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/Lib/gflanguages.egg-info/PKG-INFO` & `gflanguages-0.4.7/Lib/gflanguages.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gflanguages
-Version: 0.4.6
+Version: 0.4.7
 Summary: A python API for evaluating language support in the Google Fonts collection.
 Home-page: https://github.com/googlefonts/lang/
 Author: Dave Crossland, Felipe Sanches, Marc Foley, Roderick Sheeter
 Author-email: dave@lab6.com
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Fonts
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `gflanguages-0.4.6/Lib/gflanguages.egg-info/SOURCES.txt` & `gflanguages-0.4.7/Lib/gflanguages.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1216,14 +1216,15 @@
 Lib/gflanguages/data/languages/sa_Mahj.textproto
 Lib/gflanguages/data/languages/sa_Marc.textproto
 Lib/gflanguages/data/languages/sa_Modi.textproto
 Lib/gflanguages/data/languages/sa_Mong.textproto
 Lib/gflanguages/data/languages/sa_Mroo.textproto
 Lib/gflanguages/data/languages/sa_Mtei.textproto
 Lib/gflanguages/data/languages/sa_Mult.textproto
+Lib/gflanguages/data/languages/sa_Nand.textproto
 Lib/gflanguages/data/languages/sa_Newa.textproto
 Lib/gflanguages/data/languages/sa_Olck.textproto
 Lib/gflanguages/data/languages/sa_Orya.textproto
 Lib/gflanguages/data/languages/sa_Phag.textproto
 Lib/gflanguages/data/languages/sa_Ranj.textproto
 Lib/gflanguages/data/languages/sa_Rjng.textproto
 Lib/gflanguages/data/languages/sa_Saur.textproto
@@ -1955,14 +1956,15 @@
 Lib/gflanguages/data/scripts/Modi.textproto
 Lib/gflanguages/data/scripts/Mong.textproto
 Lib/gflanguages/data/scripts/Mroo.textproto
 Lib/gflanguages/data/scripts/Mtei.textproto
 Lib/gflanguages/data/scripts/Mult.textproto
 Lib/gflanguages/data/scripts/Mymr.textproto
 Lib/gflanguages/data/scripts/Nagm.textproto
+Lib/gflanguages/data/scripts/Nand.textproto
 Lib/gflanguages/data/scripts/Narb.textproto
 Lib/gflanguages/data/scripts/Nbat.textproto
 Lib/gflanguages/data/scripts/Newa.textproto
 Lib/gflanguages/data/scripts/Nkoo.textproto
 Lib/gflanguages/data/scripts/Nshu.textproto
 Lib/gflanguages/data/scripts/Ogam.textproto
 Lib/gflanguages/data/scripts/Olck.textproto
```

### Comparing `gflanguages-0.4.6/PKG-INFO` & `gflanguages-0.4.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gflanguages
-Version: 0.4.6
+Version: 0.4.7
 Summary: A python API for evaluating language support in the Google Fonts collection.
 Home-page: https://github.com/googlefonts/lang/
 Author: Dave Crossland, Felipe Sanches, Marc Foley, Roderick Sheeter
 Author-email: dave@lab6.com
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Fonts
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `gflanguages-0.4.6/README.md` & `gflanguages-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/data/test/nunito/Nunito-Regular.ttf` & `gflanguages-0.4.7/data/test/nunito/Nunito-Regular.ttf`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/data/test/nunito/OFL.txt` & `gflanguages-0.4.7/data/test/nunito/OFL.txt`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/setup.py` & `gflanguages-0.4.7/setup.py`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/snippets/fix-exemplars-duplicates.py` & `gflanguages-0.4.7/snippets/fix-exemplars-duplicates.py`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/snippets/supported_languages.py` & `gflanguages-0.4.7/snippets/supported_languages.py`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/tests/test_data_languages.py` & `gflanguages-0.4.7/tests/test_data_languages.py`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/tests/test_dottedcircle.py` & `gflanguages-0.4.7/tests/test_dottedcircle.py`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/tests/test_gflanguages_api.py` & `gflanguages-0.4.7/tests/test_gflanguages_api.py`

 * *Files identical despite different names*

### Comparing `gflanguages-0.4.6/tests/test_parsable.py` & `gflanguages-0.4.7/tests/test_parsable.py`

 * *Files identical despite different names*

