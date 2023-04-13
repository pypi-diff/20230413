# Comparing `tmp/espeak_phonemizer_windows-1.0.3.tar.gz` & `tmp/espeak_phonemizer_windows-1.0.3.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "espeak_phonemizer_windows-1.0.3.tar", max compression
+gzip compressed data, was "espeak_phonemizer_windows-1.0.3.post0.tar", max compression
```

## Comparing `espeak_phonemizer_windows-1.0.3.tar` & `espeak_phonemizer_windows-1.0.3.post0.tar`

### file list

```diff
@@ -1,366 +1,366 @@
--rw-r--r--   0        0        0     5829 2023-04-08 15:04:00.113685 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/__init__.py
--rw-r--r--   0        0        0     3981 2021-10-11 19:47:08.000000 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/__main__.py
--rw-r--r--   0        0        0   121473 2023-04-08 01:38:59.471480 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/af_dict
--rw-r--r--   0        0        0    63878 2023-04-08 01:38:59.471480 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/am_dict
--rw-r--r--   0        0        0     6691 2023-04-08 01:38:59.471480 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/an_dict
--rw-r--r--   0        0        0   478165 2023-04-08 01:38:59.481860 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ar_dict
--rw-r--r--   0        0        0     5005 2023-04-08 01:38:59.481860 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/as_dict
--rw-r--r--   0        0        0    43773 2023-04-08 01:38:59.481860 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/az_dict
--rw-r--r--   0        0        0     2098 2023-04-08 01:38:59.481860 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ba_dict
--rw-r--r--   0        0        0     2652 2023-04-08 01:38:59.481860 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/be_dict
--rw-r--r--   0        0        0    87051 2023-04-08 01:38:59.481860 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/bg_dict
--rw-r--r--   0        0        0    89979 2023-04-08 01:38:59.481860 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/bn_dict
--rw-r--r--   0        0        0     5226 2023-04-08 01:38:59.481860 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/bpy_dict
--rw-r--r--   0        0        0    47068 2023-04-08 01:38:59.481860 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/bs_dict
--rw-r--r--   0        0        0    45566 2023-04-08 01:38:59.481860 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ca_dict
--rw-r--r--   0        0        0     2859 2023-04-08 01:38:59.481860 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/chr_dict
--rw-r--r--   0        0        0  1566335 2023-04-08 01:38:59.491809 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/cmn_dict
--rw-r--r--   0        0        0    49645 2023-04-08 01:38:59.491809 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/cs_dict
--rw-r--r--   0        0        0     1344 2023-04-08 01:38:59.491809 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/cv_dict
--rw-r--r--   0        0        0    43130 2023-04-08 01:38:59.491809 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/cy_dict
--rw-r--r--   0        0        0   245287 2023-04-08 01:38:59.497384 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/da_dict
--rw-r--r--   0        0        0    68276 2023-04-08 01:38:59.497384 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/de_dict
--rw-r--r--   0        0        0    72841 2023-04-08 01:38:59.497384 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/el_dict
--rw-r--r--   0        0        0   166944 2023-04-08 01:38:59.501927 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/en_dict
--rw-r--r--   0        0        0     4666 2023-04-08 01:38:59.501927 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/eo_dict
--rw-r--r--   0        0        0    49252 2023-04-08 01:38:59.501927 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/es_dict
--rw-r--r--   0        0        0    44263 2023-04-08 01:38:59.501927 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/et_dict
--rw-r--r--   0        0        0    48841 2023-04-08 01:38:59.501927 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/eu_dict
--rw-r--r--   0        0        0   292423 2023-04-08 01:38:59.501927 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/fa_dict
--rw-r--r--   0        0        0    43928 2023-04-08 01:38:59.501927 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/fi_dict
--rw-r--r--   0        0        0    63727 2023-04-08 01:38:59.501927 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/fr_dict
--rw-r--r--   0        0        0    52673 2023-04-08 01:38:59.501927 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ga_dict
--rw-r--r--   0        0        0    49121 2023-04-08 01:38:59.501927 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/gd_dict
--rw-r--r--   0        0        0     3248 2023-04-08 01:38:59.501927 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/gn_dict
--rw-r--r--   0        0        0     3433 2023-04-08 01:38:59.501927 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/grc_dict
--rw-r--r--   0        0        0    82480 2023-04-08 01:38:59.501927 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/gu_dict
--rw-r--r--   0        0        0     3335 2023-04-08 01:38:59.501927 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/hak_dict
--rw-r--r--   0        0        0     2443 2023-04-08 01:38:59.501927 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/haw_dict
--rw-r--r--   0        0        0     6963 2023-04-08 01:38:59.501927 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/he_dict
--rw-r--r--   0        0        0    92143 2023-04-08 01:38:59.511715 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/hi_dict
--rw-r--r--   0        0        0    49388 2023-04-08 01:38:59.511715 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/hr_dict
--rw-r--r--   0        0        0     1803 2023-04-08 01:38:59.511715 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ht_dict
--rw-r--r--   0        0        0   153785 2023-04-08 01:38:59.513327 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/hu_dict
--rw-r--r--   0        0        0    62263 2023-04-08 01:38:59.513327 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/hy_dict
--rw-r--r--   0        0        0   331275 2023-04-08 01:38:59.513327 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ia_dict
--rw-r--r--   0        0        0    43458 2023-04-08 01:38:59.513327 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/id_dict
--rw-r--r--   0        0        0     2040 2023-04-08 01:38:59.513327 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/intonations
--rw-r--r--   0        0        0     2165 2023-04-08 01:38:59.513327 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/io_dict
--rw-r--r--   0        0        0    44354 2023-04-08 01:38:59.521446 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/is_dict
--rw-r--r--   0        0        0   152889 2023-04-08 01:38:59.521697 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/it_dict
--rw-r--r--   0        0        0    47652 2023-04-08 01:38:59.521697 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ja_dict
--rw-r--r--   0        0        0     2243 2023-04-08 01:38:59.521697 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/jbo_dict
--rw-r--r--   0        0        0    87775 2023-04-08 01:38:59.521697 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ka_dict
--rw-r--r--   0        0        0     1859 2023-04-08 01:38:59.521697 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/kk_dict
--rw-r--r--   0        0        0     2838 2023-04-08 01:38:59.521697 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/kl_dict
--rw-r--r--   0        0        0    87828 2023-04-08 01:38:59.521697 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/kn_dict
--rw-r--r--   0        0        0    47523 2023-04-08 01:38:59.521697 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ko_dict
--rw-r--r--   0        0        0     6394 2023-04-08 01:38:59.521697 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/kok_dict
--rw-r--r--   0        0        0     2265 2023-04-08 01:38:59.521697 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ku_dict
--rw-r--r--   0        0        0    64977 2023-04-08 01:38:59.521697 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ky_dict
--rw-r--r--   0        0        0     3806 2023-04-08 01:38:59.521697 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/la_dict
--rw-r--r--   0        0        0      119 2023-04-08 01:38:59.521697 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/aav/vi
--rw-r--r--   0        0        0      152 2023-04-08 01:38:59.521697 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/aav/vi-VN-x-central
--rw-r--r--   0        0        0      151 2023-04-08 01:38:59.521697 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/aav/vi-VN-x-south
--rw-r--r--   0        0        0       45 2023-04-08 01:38:59.521697 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/art/eo
--rw-r--r--   0        0        0       31 2023-04-08 01:38:59.529526 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/art/ia
--rw-r--r--   0        0        0       55 2023-04-08 01:38:59.529526 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/art/io
--rw-r--r--   0        0        0       73 2023-04-08 01:38:59.529526 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/art/jbo
--rw-r--r--   0        0        0      135 2023-04-08 01:38:59.529526 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/art/lfn
--rw-r--r--   0        0        0       61 2023-04-08 01:38:59.529526 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/art/piqd
--rw-r--r--   0        0        0      147 2023-04-08 01:38:59.529526 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/art/py
--rw-r--r--   0        0        0       63 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/art/qdb
--rw-r--r--   0        0        0      177 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/art/qya
--rw-r--r--   0        0        0      179 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/art/sjn
--rw-r--r--   0        0        0      120 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/azc/nci
--rw-r--r--   0        0        0       30 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/bat/lt
--rw-r--r--   0        0        0      324 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/bat/ltg
--rw-r--r--   0        0        0      238 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/bat/lv
--rw-r--r--   0        0        0       45 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/bnt/sw
--rw-r--r--   0        0        0       46 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/bnt/tn
--rw-r--r--   0        0        0      127 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/ccs/ka
--rw-r--r--   0        0        0       41 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/cel/cy
--rw-r--r--   0        0        0       70 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/cel/ga
--rw-r--r--   0        0        0       55 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/cel/gd
--rw-r--r--   0        0        0       43 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/cus/om
--rw-r--r--   0        0        0       60 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/dra/kn
--rw-r--r--   0        0        0       62 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/dra/ml
--rw-r--r--   0        0        0       56 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/dra/ta
--rw-r--r--   0        0        0       77 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/dra/te
--rw-r--r--   0        0        0       33 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/esx/kl
--rw-r--r--   0        0        0       59 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/eu
--rw-r--r--   0        0        0       47 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/gmq/da
--rw-r--r--   0        0        0       29 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/gmq/is
--rw-r--r--   0        0        0       94 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/gmq/nb
--rw-r--r--   0        0        0       27 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/gmq/sv
--rw-r--r--   0        0        0      131 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/gmw/af
--rw-r--r--   0        0        0       45 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/gmw/de
--rw-r--r--   0        0        0      148 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/gmw/en
--rw-r--r--   0        0        0      355 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/gmw/en-029
--rw-r--r--   0        0        0      312 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/gmw/en-GB-scotland
--rw-r--r--   0        0        0      252 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/gmw/en-GB-x-gbclan
--rw-r--r--   0        0        0      200 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/gmw/en-GB-x-gbcwmd
--rw-r--r--   0        0        0      264 2023-04-08 01:38:59.541669 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/gmw/en-GB-x-rp
--rw-r--r--   0        0        0      272 2023-04-08 01:38:59.541669 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/gmw/en-US
--rw-r--r--   0        0        0      285 2023-04-08 01:38:59.541669 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/gmw/en-US-nyc
--rw-r--r--   0        0        0       33 2023-04-08 01:38:59.541669 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/gmw/lb
--rw-r--r--   0        0        0       25 2023-04-08 01:38:59.541669 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/gmw/nl
--rw-r--r--   0        0        0       25 2023-04-08 01:38:59.541669 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/grk/el
--rw-r--r--   0        0        0      105 2023-04-08 01:38:59.541669 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/grk/grc
--rw-r--r--   0        0        0       46 2023-04-08 01:38:59.541669 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/inc/as
--rw-r--r--   0        0        0       27 2023-04-08 01:38:59.541669 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/inc/bn
--rw-r--r--   0        0        0       41 2023-04-08 01:38:59.541669 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/inc/bpy
--rw-r--r--   0        0        0       46 2023-04-08 01:38:59.541669 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/inc/gu
--rw-r--r--   0        0        0       25 2023-04-08 01:38:59.541669 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/inc/hi
--rw-r--r--   0        0        0       28 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/inc/kok
--rw-r--r--   0        0        0       45 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/inc/mr
--rw-r--r--   0        0        0       41 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/inc/ne
--rw-r--r--   0        0        0       43 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/inc/or
--rw-r--r--   0        0        0       27 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/inc/pa
--rw-r--r--   0        0        0       69 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/inc/sd
--rw-r--r--   0        0        0       61 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/inc/si
--rw-r--r--   0        0        0      101 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/inc/ur
--rw-r--r--   0        0        0       64 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/ine/hy
--rw-r--r--   0        0        0      389 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/ine/hyw
--rw-r--r--   0        0        0      108 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/ine/sq
--rw-r--r--   0        0        0       94 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/ira/fa
--rw-r--r--   0        0        0      277 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/ira/fa-Latn
--rw-r--r--   0        0        0       45 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/ira/ku
--rw-r--r--   0        0        0      596 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/iro/chr
--rw-r--r--   0        0        0      309 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/itc/la
--rw-r--r--   0        0        0       57 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/jpx/ja
--rw-r--r--   0        0        0       56 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/ko
--rw-r--r--   0        0        0       45 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/map/haw
--rw-r--r--   0        0        0      191 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/miz/mto
--rw-r--r--   0        0        0      216 2023-04-08 01:38:59.551434 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/myn/quc
--rw-r--r--   0        0        0      141 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/poz/id
--rw-r--r--   0        0        0      388 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/poz/mi
--rw-r--r--   0        0        0      444 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/poz/ms
--rw-r--r--   0        0        0       93 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/qu
--rw-r--r--   0        0        0       29 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/roa/an
--rw-r--r--   0        0        0       27 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/roa/ca
--rw-r--r--   0        0        0       67 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/roa/es
--rw-r--r--   0        0        0      178 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/roa/es-419
--rw-r--r--   0        0        0       85 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/roa/fr
--rw-r--r--   0        0        0       92 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/roa/fr-BE
--rw-r--r--   0        0        0       92 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/roa/fr-CH
--rw-r--r--   0        0        0      148 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/roa/ht
--rw-r--r--   0        0        0      116 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/roa/it
--rw-r--r--   0        0        0       69 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/roa/pap
--rw-r--r--   0        0        0      102 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/roa/pt
--rw-r--r--   0        0        0      116 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/roa/pt-BR
--rw-r--r--   0        0        0       28 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/roa/ro
--rw-r--r--   0        0        0       51 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/sai/gn
--rw-r--r--   0        0        0       45 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/sem/am
--rw-r--r--   0        0        0       55 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/sem/ar
--rw-r--r--   0        0        0       44 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/sem/he
--rw-r--r--   0        0        0       45 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/sem/mt
--rw-r--r--   0        0        0      722 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/sit/cmn
--rw-r--r--   0        0        0      172 2023-04-08 01:38:59.558921 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/sit/cmn-Latn-pinyin
--rw-r--r--   0        0        0      134 2023-04-08 01:38:59.559233 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/sit/hak
--rw-r--r--   0        0        0       59 2023-04-08 01:38:59.559233 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/sit/my
--rw-r--r--   0        0        0      207 2023-04-08 01:38:59.559233 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/sit/yue
--rw-r--r--   0        0        0      226 2023-04-08 01:38:59.559233 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/sit/yue-Latn-jyutping
--rw-r--r--   0        0        0       96 2023-04-08 01:38:59.559233 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/tai/shn
--rw-r--r--   0        0        0       40 2023-04-08 01:38:59.559233 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/tai/th
--rw-r--r--   0        0        0       49 2023-04-08 01:38:59.559233 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/trk/az
--rw-r--r--   0        0        0       27 2023-04-08 01:38:59.561358 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/trk/ba
--rw-r--r--   0        0        0       43 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/trk/cv
--rw-r--r--   0        0        0       44 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/trk/kk
--rw-r--r--   0        0        0       47 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/trk/ky
--rw-r--r--   0        0        0       42 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/trk/nog
--rw-r--r--   0        0        0       27 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/trk/tk
--rw-r--r--   0        0        0       27 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/trk/tr
--rw-r--r--   0        0        0       25 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/trk/tt
--rw-r--r--   0        0        0       26 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/trk/ug
--rw-r--r--   0        0        0       43 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/trk/uz
--rw-r--r--   0        0        0      247 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/urj/et
--rw-r--r--   0        0        0      248 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/urj/fi
--rw-r--r--   0        0        0       80 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/urj/hu
--rw-r--r--   0        0        0       49 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/urj/smj
--rw-r--r--   0        0        0       56 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/zle/be
--rw-r--r--   0        0        0       61 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/zle/ru
--rw-r--r--   0        0        0       97 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/zle/ru-cl
--rw-r--r--   0        0        0      296 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/zle/ru-LV
--rw-r--r--   0        0        0      103 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/zle/uk
--rw-r--r--   0        0        0      116 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/zls/bg
--rw-r--r--   0        0        0      244 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/zls/bs
--rw-r--r--   0        0        0      277 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/zls/hr
--rw-r--r--   0        0        0       30 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/zls/mk
--rw-r--r--   0        0        0       47 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/zls/sl
--rw-r--r--   0        0        0      263 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/zls/sr
--rw-r--r--   0        0        0       25 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/zlw/cs
--rw-r--r--   0        0        0       42 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/zlw/pl
--rw-r--r--   0        0        0       26 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/zlw/sk
--rw-r--r--   0        0        0   687931 2023-04-08 01:38:59.571544 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lb_dict
--rw-r--r--   0        0        0     2793 2023-04-08 01:38:59.571544 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lfn_dict
--rw-r--r--   0        0        0    49890 2023-04-08 01:38:59.571544 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lt_dict
--rw-r--r--   0        0        0    66337 2023-04-08 01:38:59.571544 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lv_dict
--rw-r--r--   0        0        0     1346 2023-04-08 01:38:59.577442 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/mi_dict
--rw-r--r--   0        0        0    63859 2023-04-08 01:38:59.577442 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/mk_dict
--rw-r--r--   0        0        0    92345 2023-04-08 01:38:59.577442 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ml_dict
--rw-r--r--   0        0        0    87391 2023-04-08 01:38:59.581649 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/mr_dict
--rw-r--r--   0        0        0    53541 2023-04-08 01:38:59.581649 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ms_dict
--rw-r--r--   0        0        0     4384 2023-04-08 01:38:59.581649 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/mt_dict
--rw-r--r--   0        0        0     3960 2023-04-08 01:38:59.581649 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/mto_dict
--rw-r--r--   0        0        0    95948 2023-04-08 01:38:59.581649 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/my_dict
--rw-r--r--   0        0        0     1534 2023-04-08 01:38:59.581649 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/nci_dict
--rw-r--r--   0        0        0    95377 2023-04-08 01:38:59.581649 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ne_dict
--rw-r--r--   0        0        0    65979 2023-04-08 01:38:59.581649 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/nl_dict
--rw-r--r--   0        0        0     4178 2023-04-08 01:38:59.581649 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/no_dict
--rw-r--r--   0        0        0     3294 2023-04-08 01:38:59.581649 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/nog_dict
--rw-r--r--   0        0        0     2302 2023-04-08 01:38:59.581649 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/om_dict
--rw-r--r--   0        0        0    89246 2023-04-08 01:38:59.581649 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/or_dict
--rw-r--r--   0        0        0    79953 2023-04-08 01:38:59.581649 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/pa_dict
--rw-r--r--   0        0        0     2128 2023-04-08 01:38:59.581649 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/pap_dict
--rw-r--r--   0        0        0   550424 2023-04-08 01:38:59.591647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/phondata
--rw-r--r--   0        0        0    22808 2023-04-08 01:38:59.593249 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/phondata-manifest
--rw-r--r--   0        0        0    39074 2023-04-08 01:38:59.593249 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/phonindex
--rw-r--r--   0        0        0    55796 2023-04-08 01:38:59.593249 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/phontab
--rw-r--r--   0        0        0     1710 2023-04-08 01:38:59.593249 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/piqd_dict
--rw-r--r--   0        0        0    76730 2023-04-08 01:38:59.593249 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/pl_dict
--rw-r--r--   0        0        0    67817 2023-04-08 01:38:59.593249 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/pt_dict
--rw-r--r--   0        0        0     2409 2023-04-08 01:38:59.593249 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/py_dict
--rw-r--r--   0        0        0     3028 2023-04-08 01:38:59.593249 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/qdb_dict
--rw-r--r--   0        0        0     1919 2023-04-08 01:38:59.593249 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/qu_dict
--rw-r--r--   0        0        0     1450 2023-04-08 01:38:59.593249 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/quc_dict
--rw-r--r--   0        0        0     1939 2023-04-08 01:38:59.593249 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/qya_dict
--rw-r--r--   0        0        0    68538 2023-04-08 01:38:59.593249 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ro_dict
--rw-r--r--   0        0        0  8532392 2023-04-08 01:38:59.661255 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ru_dict
--rw-r--r--   0        0        0    59928 2023-04-08 01:38:59.671132 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/sd_dict
--rw-r--r--   0        0        0    88172 2023-04-08 01:38:59.671132 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/shn_dict
--rw-r--r--   0        0        0    85384 2023-04-08 01:38:59.673664 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/si_dict
--rw-r--r--   0        0        0     1783 2023-04-08 01:38:59.673664 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/sjn_dict
--rw-r--r--   0        0        0    50002 2023-04-08 01:38:59.673664 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/sk_dict
--rw-r--r--   0        0        0    45047 2023-04-08 01:38:59.673664 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/sl_dict
--rw-r--r--   0        0        0    35095 2023-04-08 01:38:59.673664 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/smj_dict
--rw-r--r--   0        0        0    45003 2023-04-08 01:38:59.673664 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/sq_dict
--rw-r--r--   0        0        0    46832 2023-04-08 01:38:59.681384 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/sr_dict
--rw-r--r--   0        0        0    47836 2023-04-08 01:38:59.681384 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/sv_dict
--rw-r--r--   0        0        0    47804 2023-04-08 01:38:59.681384 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/sw_dict
--rw-r--r--   0        0        0   209553 2023-04-08 01:38:59.681384 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ta_dict
--rw-r--r--   0        0        0    94837 2023-04-08 01:38:59.681384 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/te_dict
--rw-r--r--   0        0        0     2301 2023-04-08 01:38:59.681384 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/th_dict
--rw-r--r--   0        0        0    20868 2023-04-08 01:38:59.681384 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/tk_dict
--rw-r--r--   0        0        0     3072 2023-04-08 01:38:59.681384 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/tn_dict
--rw-r--r--   0        0        0    46793 2023-04-08 01:38:59.689682 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/tr_dict
--rw-r--r--   0        0        0     2121 2023-04-08 01:38:59.689682 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/tt_dict
--rw-r--r--   0        0        0     2070 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ug_dict
--rw-r--r--   0        0        0     3492 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/uk_dict
--rw-r--r--   0        0        0   133556 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ur_dict
--rw-r--r--   0        0        0     2540 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/uz_dict
--rw-r--r--   0        0        0    52608 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/vi_dict
--rw-r--r--   0        0        0       81 2023-04-08 01:38:59.701664 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/adam
--rw-r--r--   0        0        0      138 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Alex
--rw-r--r--   0        0        0      474 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Alicia
--rw-r--r--   0        0        0      376 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Andrea
--rw-r--r--   0        0        0      320 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Andy
--rw-r--r--   0        0        0      518 2023-04-08 01:38:59.701664 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/anika
--rw-r--r--   0        0        0      538 2023-04-08 01:38:59.701664 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/anikaRobot
--rw-r--r--   0        0        0      315 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Annie
--rw-r--r--   0        0        0      317 2023-04-08 01:38:59.701664 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/announcer
--rw-r--r--   0        0        0      402 2023-04-08 01:38:59.701664 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/antonio
--rw-r--r--   0        0        0      361 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/AnxiousAndy
--rw-r--r--   0        0        0      358 2023-04-08 01:38:59.701664 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/aunty
--rw-r--r--   0        0        0      360 2023-04-08 01:38:59.701664 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/belinda
--rw-r--r--   0        0        0      212 2023-04-08 01:38:59.701664 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/benjamin
--rw-r--r--   0        0        0      224 2023-04-08 01:38:59.701664 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/boris
--rw-r--r--   0        0        0       62 2023-04-08 01:38:59.701664 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/caleb
--rw-r--r--   0        0        0      104 2023-04-08 01:38:59.701664 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/croak
--rw-r--r--   0        0        0      120 2023-04-08 01:38:59.701664 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/david
--rw-r--r--   0        0        0     3858 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Demonic
--rw-r--r--   0        0        0      305 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Denis
--rw-r--r--   0        0        0      401 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Diogo
--rw-r--r--   0        0        0      303 2023-04-08 01:38:59.701664 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/ed
--rw-r--r--   0        0        0      161 2023-04-08 01:38:59.705804 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/edward
--rw-r--r--   0        0        0      162 2023-04-08 01:38:59.705804 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/edward2
--rw-r--r--   0        0        0      342 2023-04-08 01:38:59.705804 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/f1
--rw-r--r--   0        0        0      378 2023-04-08 01:38:59.705804 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/f2
--rw-r--r--   0        0        0      397 2023-04-08 01:38:59.705804 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/f3
--rw-r--r--   0        0        0      368 2023-04-08 01:38:59.705804 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/f4
--rw-r--r--   0        0        0      455 2023-04-08 01:38:59.705804 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/f5
--rw-r--r--   0        0        0      156 2023-04-08 01:38:59.705804 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/fast
--rw-r--r--   0        0        0      281 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Gene
--rw-r--r--   0        0        0      283 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Gene2
--rw-r--r--   0        0        0      279 2023-04-08 01:38:59.705804 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/grandma
--rw-r--r--   0        0        0      270 2023-04-08 01:38:59.705804 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/grandpa
--rw-r--r--   0        0        0      270 2023-04-08 01:38:59.705804 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/gustave
--rw-r--r--   0        0        0      403 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Henrique
--rw-r--r--   0        0        0      400 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Hugo
--rw-r--r--   0        0        0     3168 2023-04-08 01:38:59.705804 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/ian
--rw-r--r--   0        0        0      274 2023-04-08 01:38:59.711418 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/iven
--rw-r--r--   0        0        0      293 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/iven2
--rw-r--r--   0        0        0      275 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/iven3
--rw-r--r--   0        0        0      274 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/iven4
--rw-r--r--   0        0        0      267 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Jacky
--rw-r--r--   0        0        0     3186 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/john
--rw-r--r--   0        0        0      361 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/kaukovalta
--rw-r--r--   0        0        0       42 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/klatt
--rw-r--r--   0        0        0       42 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/klatt2
--rw-r--r--   0        0        0       43 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/klatt3
--rw-r--r--   0        0        0       43 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/klatt4
--rw-r--r--   0        0        0       43 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/klatt5
--rw-r--r--   0        0        0       43 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/klatt6
--rw-r--r--   0        0        0      338 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Lee
--rw-r--r--   0        0        0      370 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/linda
--rw-r--r--   0        0        0      355 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/m1
--rw-r--r--   0        0        0      279 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/m2
--rw-r--r--   0        0        0      317 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/m3
--rw-r--r--   0        0        0      307 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/m4
--rw-r--r--   0        0        0      277 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/m5
--rw-r--r--   0        0        0      201 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/m6
--rw-r--r--   0        0        0      271 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/m7
--rw-r--r--   0        0        0      300 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/m8
--rw-r--r--   0        0        0      268 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/marcelo
--rw-r--r--   0        0        0      467 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Marco
--rw-r--r--   0        0        0      270 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Mario
--rw-r--r--   0        0        0      225 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/max
--rw-r--r--   0        0        0      270 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Michael
--rw-r--r--   0        0        0      404 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/michel
--rw-r--r--   0        0        0      404 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/miguel
--rw-r--r--   0        0        0      119 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Mike
--rw-r--r--   0        0        0      200 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/mike2
--rw-r--r--   0        0        0     3193 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Mr serious
--rw-r--r--   0        0        0      296 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Nguyen
--rw-r--r--   0        0        0     3189 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/norbert
--rw-r--r--   0        0        0     3194 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/pablo
--rw-r--r--   0        0        0      300 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/paul
--rw-r--r--   0        0        0      375 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/pedro
--rw-r--r--   0        0        0      354 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/quincy
--rw-r--r--   0        0        0      217 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Reed
--rw-r--r--   0        0        0      249 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/RicishayMax
--rw-r--r--   0        0        0      460 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/RicishayMax2
--rw-r--r--   0        0        0      460 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/RicishayMax3
--rw-r--r--   0        0        0      265 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/rob
--rw-r--r--   0        0        0      274 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/robert
--rw-r--r--   0        0        0      477 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/robosoft
--rw-r--r--   0        0        0      480 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/robosoft2
--rw-r--r--   0        0        0      481 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/robosoft3
--rw-r--r--   0        0        0      472 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/robosoft4
--rw-r--r--   0        0        0      470 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/robosoft5
--rw-r--r--   0        0        0      302 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/robosoft6
--rw-r--r--   0        0        0      435 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/robosoft7
--rw-r--r--   0        0        0      259 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/robosoft8
--rw-r--r--   0        0        0      555 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/sandro
--rw-r--r--   0        0        0      297 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/shelby
--rw-r--r--   0        0        0      385 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/steph
--rw-r--r--   0        0        0      388 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/steph2
--rw-r--r--   0        0        0      399 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/steph3
--rw-r--r--   0        0        0      420 2023-04-08 01:38:59.701379 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Storm
--rw-r--r--   0        0        0      383 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/travis
--rw-r--r--   0        0        0     3189 2023-04-08 01:38:59.701664 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Tweaky
--rw-r--r--   0        0        0      417 2023-04-08 01:38:59.701664 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/UniRobot
--rw-r--r--   0        0        0      268 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/victor
--rw-r--r--   0        0        0      199 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/whisper
--rw-r--r--   0        0        0      416 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/whisperf
--rw-r--r--   0        0        0      275 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/zac
--rw-r--r--   0        0        0   563571 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/yue_dict
--rw-r--r--   0        0        0   526336 2023-04-08 01:38:59.731771 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-x64.dll
--rw-r--r--   0        0        0   378880 2023-04-08 01:38:59.731771 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-x86.dll
--rw-r--r--   0        0        0        0 2021-10-11 19:47:08.000000 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/py.typed
--rw-r--r--   0        0        0        7 2023-04-08 14:57:30.982438 espeak_phonemizer_windows-1.0.3/espeak_phonemizer/VERSION
--rw-r--r--   0        0        0    35147 2021-10-11 19:47:08.000000 espeak_phonemizer_windows-1.0.3/LICENSE
--rw-r--r--   0        0        0      845 2023-04-08 15:07:36.563328 espeak_phonemizer_windows-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1486 2023-02-24 17:02:27.801498 espeak_phonemizer_windows-1.0.3/README.md
--rw-r--r--   0        0        0     4431 1970-01-01 00:00:00.000000 espeak_phonemizer_windows-1.0.3/setup.py
--rw-r--r--   0        0        0     2481 1970-01-01 00:00:00.000000 espeak_phonemizer_windows-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     5266 2023-04-12 22:12:45.682291 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/__init__.py
+-rw-r--r--   0        0        0     3981 2021-10-11 19:47:08.000000 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/__main__.py
+-rw-r--r--   0        0        0   121473 2023-04-08 01:38:59.471480 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/af_dict
+-rw-r--r--   0        0        0    63878 2023-04-08 01:38:59.471480 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/am_dict
+-rw-r--r--   0        0        0     6691 2023-04-08 01:38:59.471480 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/an_dict
+-rw-r--r--   0        0        0   478165 2023-04-08 01:38:59.481860 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ar_dict
+-rw-r--r--   0        0        0     5005 2023-04-08 01:38:59.481860 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/as_dict
+-rw-r--r--   0        0        0    43773 2023-04-08 01:38:59.481860 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/az_dict
+-rw-r--r--   0        0        0     2098 2023-04-08 01:38:59.481860 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ba_dict
+-rw-r--r--   0        0        0     2652 2023-04-08 01:38:59.481860 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/be_dict
+-rw-r--r--   0        0        0    87051 2023-04-08 01:38:59.481860 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/bg_dict
+-rw-r--r--   0        0        0    89979 2023-04-08 01:38:59.481860 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/bn_dict
+-rw-r--r--   0        0        0     5226 2023-04-08 01:38:59.481860 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/bpy_dict
+-rw-r--r--   0        0        0    47068 2023-04-08 01:38:59.481860 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/bs_dict
+-rw-r--r--   0        0        0    45566 2023-04-08 01:38:59.481860 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ca_dict
+-rw-r--r--   0        0        0     2859 2023-04-08 01:38:59.481860 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/chr_dict
+-rw-r--r--   0        0        0  1566335 2023-04-08 01:38:59.491809 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/cmn_dict
+-rw-r--r--   0        0        0    49645 2023-04-08 01:38:59.491809 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/cs_dict
+-rw-r--r--   0        0        0     1344 2023-04-08 01:38:59.491809 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/cv_dict
+-rw-r--r--   0        0        0    43130 2023-04-08 01:38:59.491809 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/cy_dict
+-rw-r--r--   0        0        0   245287 2023-04-08 01:38:59.497384 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/da_dict
+-rw-r--r--   0        0        0    68276 2023-04-08 01:38:59.497384 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/de_dict
+-rw-r--r--   0        0        0    72841 2023-04-08 01:38:59.497384 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/el_dict
+-rw-r--r--   0        0        0   166944 2023-04-08 01:38:59.501927 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/en_dict
+-rw-r--r--   0        0        0     4666 2023-04-08 01:38:59.501927 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/eo_dict
+-rw-r--r--   0        0        0    49252 2023-04-08 01:38:59.501927 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/es_dict
+-rw-r--r--   0        0        0    44263 2023-04-08 01:38:59.501927 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/et_dict
+-rw-r--r--   0        0        0    48841 2023-04-08 01:38:59.501927 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/eu_dict
+-rw-r--r--   0        0        0   292423 2023-04-08 01:38:59.501927 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/fa_dict
+-rw-r--r--   0        0        0    43928 2023-04-08 01:38:59.501927 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/fi_dict
+-rw-r--r--   0        0        0    63727 2023-04-08 01:38:59.501927 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/fr_dict
+-rw-r--r--   0        0        0    52673 2023-04-08 01:38:59.501927 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ga_dict
+-rw-r--r--   0        0        0    49121 2023-04-08 01:38:59.501927 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/gd_dict
+-rw-r--r--   0        0        0     3248 2023-04-08 01:38:59.501927 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/gn_dict
+-rw-r--r--   0        0        0     3433 2023-04-08 01:38:59.501927 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/grc_dict
+-rw-r--r--   0        0        0    82480 2023-04-08 01:38:59.501927 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/gu_dict
+-rw-r--r--   0        0        0     3335 2023-04-08 01:38:59.501927 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/hak_dict
+-rw-r--r--   0        0        0     2443 2023-04-08 01:38:59.501927 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/haw_dict
+-rw-r--r--   0        0        0     6963 2023-04-08 01:38:59.501927 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/he_dict
+-rw-r--r--   0        0        0    92143 2023-04-08 01:38:59.511715 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/hi_dict
+-rw-r--r--   0        0        0    49388 2023-04-08 01:38:59.511715 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/hr_dict
+-rw-r--r--   0        0        0     1803 2023-04-08 01:38:59.511715 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ht_dict
+-rw-r--r--   0        0        0   153785 2023-04-08 01:38:59.513327 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/hu_dict
+-rw-r--r--   0        0        0    62263 2023-04-08 01:38:59.513327 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/hy_dict
+-rw-r--r--   0        0        0   331275 2023-04-08 01:38:59.513327 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ia_dict
+-rw-r--r--   0        0        0    43458 2023-04-08 01:38:59.513327 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/id_dict
+-rw-r--r--   0        0        0     2040 2023-04-08 01:38:59.513327 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/intonations
+-rw-r--r--   0        0        0     2165 2023-04-08 01:38:59.513327 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/io_dict
+-rw-r--r--   0        0        0    44354 2023-04-08 01:38:59.521446 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/is_dict
+-rw-r--r--   0        0        0   152889 2023-04-08 01:38:59.521697 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/it_dict
+-rw-r--r--   0        0        0    47652 2023-04-08 01:38:59.521697 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ja_dict
+-rw-r--r--   0        0        0     2243 2023-04-08 01:38:59.521697 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/jbo_dict
+-rw-r--r--   0        0        0    87775 2023-04-08 01:38:59.521697 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ka_dict
+-rw-r--r--   0        0        0     1859 2023-04-08 01:38:59.521697 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/kk_dict
+-rw-r--r--   0        0        0     2838 2023-04-08 01:38:59.521697 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/kl_dict
+-rw-r--r--   0        0        0    87828 2023-04-08 01:38:59.521697 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/kn_dict
+-rw-r--r--   0        0        0    47523 2023-04-08 01:38:59.521697 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ko_dict
+-rw-r--r--   0        0        0     6394 2023-04-08 01:38:59.521697 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/kok_dict
+-rw-r--r--   0        0        0     2265 2023-04-08 01:38:59.521697 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ku_dict
+-rw-r--r--   0        0        0    64977 2023-04-08 01:38:59.521697 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ky_dict
+-rw-r--r--   0        0        0     3806 2023-04-08 01:38:59.521697 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/la_dict
+-rw-r--r--   0        0        0      119 2023-04-08 01:38:59.521697 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/aav/vi
+-rw-r--r--   0        0        0      152 2023-04-08 01:38:59.521697 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/aav/vi-VN-x-central
+-rw-r--r--   0        0        0      151 2023-04-08 01:38:59.521697 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/aav/vi-VN-x-south
+-rw-r--r--   0        0        0       45 2023-04-08 01:38:59.521697 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/art/eo
+-rw-r--r--   0        0        0       31 2023-04-08 01:38:59.529526 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/art/ia
+-rw-r--r--   0        0        0       55 2023-04-08 01:38:59.529526 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/art/io
+-rw-r--r--   0        0        0       73 2023-04-08 01:38:59.529526 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/art/jbo
+-rw-r--r--   0        0        0      135 2023-04-08 01:38:59.529526 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/art/lfn
+-rw-r--r--   0        0        0       61 2023-04-08 01:38:59.529526 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/art/piqd
+-rw-r--r--   0        0        0      147 2023-04-08 01:38:59.529526 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/art/py
+-rw-r--r--   0        0        0       63 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/art/qdb
+-rw-r--r--   0        0        0      177 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/art/qya
+-rw-r--r--   0        0        0      179 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/art/sjn
+-rw-r--r--   0        0        0      120 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/azc/nci
+-rw-r--r--   0        0        0       30 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/bat/lt
+-rw-r--r--   0        0        0      324 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/bat/ltg
+-rw-r--r--   0        0        0      238 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/bat/lv
+-rw-r--r--   0        0        0       45 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/bnt/sw
+-rw-r--r--   0        0        0       46 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/bnt/tn
+-rw-r--r--   0        0        0      127 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/ccs/ka
+-rw-r--r--   0        0        0       41 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/cel/cy
+-rw-r--r--   0        0        0       70 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/cel/ga
+-rw-r--r--   0        0        0       55 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/cel/gd
+-rw-r--r--   0        0        0       43 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/cus/om
+-rw-r--r--   0        0        0       60 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/dra/kn
+-rw-r--r--   0        0        0       62 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/dra/ml
+-rw-r--r--   0        0        0       56 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/dra/ta
+-rw-r--r--   0        0        0       77 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/dra/te
+-rw-r--r--   0        0        0       33 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/esx/kl
+-rw-r--r--   0        0        0       59 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/eu
+-rw-r--r--   0        0        0       47 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/gmq/da
+-rw-r--r--   0        0        0       29 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/gmq/is
+-rw-r--r--   0        0        0       94 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/gmq/nb
+-rw-r--r--   0        0        0       27 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/gmq/sv
+-rw-r--r--   0        0        0      131 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/gmw/af
+-rw-r--r--   0        0        0       45 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/gmw/de
+-rw-r--r--   0        0        0      148 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/gmw/en
+-rw-r--r--   0        0        0      355 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/gmw/en-029
+-rw-r--r--   0        0        0      312 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/gmw/en-GB-scotland
+-rw-r--r--   0        0        0      252 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/gmw/en-GB-x-gbclan
+-rw-r--r--   0        0        0      200 2023-04-08 01:38:59.531149 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/gmw/en-GB-x-gbcwmd
+-rw-r--r--   0        0        0      264 2023-04-08 01:38:59.541669 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/gmw/en-GB-x-rp
+-rw-r--r--   0        0        0      272 2023-04-08 01:38:59.541669 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/gmw/en-US
+-rw-r--r--   0        0        0      285 2023-04-08 01:38:59.541669 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/gmw/en-US-nyc
+-rw-r--r--   0        0        0       33 2023-04-08 01:38:59.541669 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/gmw/lb
+-rw-r--r--   0        0        0       25 2023-04-08 01:38:59.541669 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/gmw/nl
+-rw-r--r--   0        0        0       25 2023-04-08 01:38:59.541669 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/grk/el
+-rw-r--r--   0        0        0      105 2023-04-08 01:38:59.541669 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/grk/grc
+-rw-r--r--   0        0        0       46 2023-04-08 01:38:59.541669 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/inc/as
+-rw-r--r--   0        0        0       27 2023-04-08 01:38:59.541669 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/inc/bn
+-rw-r--r--   0        0        0       41 2023-04-08 01:38:59.541669 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/inc/bpy
+-rw-r--r--   0        0        0       46 2023-04-08 01:38:59.541669 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/inc/gu
+-rw-r--r--   0        0        0       25 2023-04-08 01:38:59.541669 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/inc/hi
+-rw-r--r--   0        0        0       28 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/inc/kok
+-rw-r--r--   0        0        0       45 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/inc/mr
+-rw-r--r--   0        0        0       41 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/inc/ne
+-rw-r--r--   0        0        0       43 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/inc/or
+-rw-r--r--   0        0        0       27 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/inc/pa
+-rw-r--r--   0        0        0       69 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/inc/sd
+-rw-r--r--   0        0        0       61 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/inc/si
+-rw-r--r--   0        0        0      101 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/inc/ur
+-rw-r--r--   0        0        0       64 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/ine/hy
+-rw-r--r--   0        0        0      389 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/ine/hyw
+-rw-r--r--   0        0        0      108 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/ine/sq
+-rw-r--r--   0        0        0       94 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/ira/fa
+-rw-r--r--   0        0        0      277 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/ira/fa-Latn
+-rw-r--r--   0        0        0       45 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/ira/ku
+-rw-r--r--   0        0        0      596 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/iro/chr
+-rw-r--r--   0        0        0      309 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/itc/la
+-rw-r--r--   0        0        0       57 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/jpx/ja
+-rw-r--r--   0        0        0       56 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/ko
+-rw-r--r--   0        0        0       45 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/map/haw
+-rw-r--r--   0        0        0      191 2023-04-08 01:38:59.545307 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/miz/mto
+-rw-r--r--   0        0        0      216 2023-04-08 01:38:59.551434 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/myn/quc
+-rw-r--r--   0        0        0      141 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/poz/id
+-rw-r--r--   0        0        0      388 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/poz/mi
+-rw-r--r--   0        0        0      444 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/poz/ms
+-rw-r--r--   0        0        0       93 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/qu
+-rw-r--r--   0        0        0       29 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/roa/an
+-rw-r--r--   0        0        0       27 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/roa/ca
+-rw-r--r--   0        0        0       67 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/roa/es
+-rw-r--r--   0        0        0      178 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/roa/es-419
+-rw-r--r--   0        0        0       85 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/roa/fr
+-rw-r--r--   0        0        0       92 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/roa/fr-BE
+-rw-r--r--   0        0        0       92 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/roa/fr-CH
+-rw-r--r--   0        0        0      148 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/roa/ht
+-rw-r--r--   0        0        0      116 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/roa/it
+-rw-r--r--   0        0        0       69 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/roa/pap
+-rw-r--r--   0        0        0      102 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/roa/pt
+-rw-r--r--   0        0        0      116 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/roa/pt-BR
+-rw-r--r--   0        0        0       28 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/roa/ro
+-rw-r--r--   0        0        0       51 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/sai/gn
+-rw-r--r--   0        0        0       45 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/sem/am
+-rw-r--r--   0        0        0       55 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/sem/ar
+-rw-r--r--   0        0        0       44 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/sem/he
+-rw-r--r--   0        0        0       45 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/sem/mt
+-rw-r--r--   0        0        0      722 2023-04-08 01:38:59.551847 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/sit/cmn
+-rw-r--r--   0        0        0      172 2023-04-08 01:38:59.558921 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/sit/cmn-Latn-pinyin
+-rw-r--r--   0        0        0      134 2023-04-08 01:38:59.559233 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/sit/hak
+-rw-r--r--   0        0        0       59 2023-04-08 01:38:59.559233 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/sit/my
+-rw-r--r--   0        0        0      207 2023-04-08 01:38:59.559233 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/sit/yue
+-rw-r--r--   0        0        0      226 2023-04-08 01:38:59.559233 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/sit/yue-Latn-jyutping
+-rw-r--r--   0        0        0       96 2023-04-08 01:38:59.559233 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/tai/shn
+-rw-r--r--   0        0        0       40 2023-04-08 01:38:59.559233 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/tai/th
+-rw-r--r--   0        0        0       49 2023-04-08 01:38:59.559233 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/trk/az
+-rw-r--r--   0        0        0       27 2023-04-08 01:38:59.561358 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/trk/ba
+-rw-r--r--   0        0        0       43 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/trk/cv
+-rw-r--r--   0        0        0       44 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/trk/kk
+-rw-r--r--   0        0        0       47 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/trk/ky
+-rw-r--r--   0        0        0       42 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/trk/nog
+-rw-r--r--   0        0        0       27 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/trk/tk
+-rw-r--r--   0        0        0       27 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/trk/tr
+-rw-r--r--   0        0        0       25 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/trk/tt
+-rw-r--r--   0        0        0       26 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/trk/ug
+-rw-r--r--   0        0        0       43 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/trk/uz
+-rw-r--r--   0        0        0      247 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/urj/et
+-rw-r--r--   0        0        0      248 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/urj/fi
+-rw-r--r--   0        0        0       80 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/urj/hu
+-rw-r--r--   0        0        0       49 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/urj/smj
+-rw-r--r--   0        0        0       56 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/zle/be
+-rw-r--r--   0        0        0       61 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/zle/ru
+-rw-r--r--   0        0        0       97 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/zle/ru-cl
+-rw-r--r--   0        0        0      296 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/zle/ru-LV
+-rw-r--r--   0        0        0      103 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/zle/uk
+-rw-r--r--   0        0        0      116 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/zls/bg
+-rw-r--r--   0        0        0      244 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/zls/bs
+-rw-r--r--   0        0        0      277 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/zls/hr
+-rw-r--r--   0        0        0       30 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/zls/mk
+-rw-r--r--   0        0        0       47 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/zls/sl
+-rw-r--r--   0        0        0      263 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/zls/sr
+-rw-r--r--   0        0        0       25 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/zlw/cs
+-rw-r--r--   0        0        0       42 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/zlw/pl
+-rw-r--r--   0        0        0       26 2023-04-08 01:38:59.561584 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/zlw/sk
+-rw-r--r--   0        0        0   687931 2023-04-08 01:38:59.571544 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lb_dict
+-rw-r--r--   0        0        0     2793 2023-04-08 01:38:59.571544 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lfn_dict
+-rw-r--r--   0        0        0    49890 2023-04-08 01:38:59.571544 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lt_dict
+-rw-r--r--   0        0        0    66337 2023-04-08 01:38:59.571544 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lv_dict
+-rw-r--r--   0        0        0     1346 2023-04-08 01:38:59.577442 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/mi_dict
+-rw-r--r--   0        0        0    63859 2023-04-08 01:38:59.577442 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/mk_dict
+-rw-r--r--   0        0        0    92345 2023-04-08 01:38:59.577442 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ml_dict
+-rw-r--r--   0        0        0    87391 2023-04-08 01:38:59.581649 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/mr_dict
+-rw-r--r--   0        0        0    53541 2023-04-08 01:38:59.581649 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ms_dict
+-rw-r--r--   0        0        0     4384 2023-04-08 01:38:59.581649 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/mt_dict
+-rw-r--r--   0        0        0     3960 2023-04-08 01:38:59.581649 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/mto_dict
+-rw-r--r--   0        0        0    95948 2023-04-08 01:38:59.581649 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/my_dict
+-rw-r--r--   0        0        0     1534 2023-04-08 01:38:59.581649 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/nci_dict
+-rw-r--r--   0        0        0    95377 2023-04-08 01:38:59.581649 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ne_dict
+-rw-r--r--   0        0        0    65979 2023-04-08 01:38:59.581649 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/nl_dict
+-rw-r--r--   0        0        0     4178 2023-04-08 01:38:59.581649 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/no_dict
+-rw-r--r--   0        0        0     3294 2023-04-08 01:38:59.581649 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/nog_dict
+-rw-r--r--   0        0        0     2302 2023-04-08 01:38:59.581649 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/om_dict
+-rw-r--r--   0        0        0    89246 2023-04-08 01:38:59.581649 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/or_dict
+-rw-r--r--   0        0        0    79953 2023-04-08 01:38:59.581649 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/pa_dict
+-rw-r--r--   0        0        0     2128 2023-04-08 01:38:59.581649 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/pap_dict
+-rw-r--r--   0        0        0   550424 2023-04-08 01:38:59.591647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/phondata
+-rw-r--r--   0        0        0    22808 2023-04-08 01:38:59.593249 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/phondata-manifest
+-rw-r--r--   0        0        0    39074 2023-04-08 01:38:59.593249 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/phonindex
+-rw-r--r--   0        0        0    55796 2023-04-08 01:38:59.593249 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/phontab
+-rw-r--r--   0        0        0     1710 2023-04-08 01:38:59.593249 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/piqd_dict
+-rw-r--r--   0        0        0    76730 2023-04-08 01:38:59.593249 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/pl_dict
+-rw-r--r--   0        0        0    67817 2023-04-08 01:38:59.593249 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/pt_dict
+-rw-r--r--   0        0        0     2409 2023-04-08 01:38:59.593249 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/py_dict
+-rw-r--r--   0        0        0     3028 2023-04-08 01:38:59.593249 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/qdb_dict
+-rw-r--r--   0        0        0     1919 2023-04-08 01:38:59.593249 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/qu_dict
+-rw-r--r--   0        0        0     1450 2023-04-08 01:38:59.593249 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/quc_dict
+-rw-r--r--   0        0        0     1939 2023-04-08 01:38:59.593249 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/qya_dict
+-rw-r--r--   0        0        0    68538 2023-04-08 01:38:59.593249 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ro_dict
+-rw-r--r--   0        0        0  8532392 2023-04-08 01:38:59.661255 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ru_dict
+-rw-r--r--   0        0        0    59928 2023-04-08 01:38:59.671132 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/sd_dict
+-rw-r--r--   0        0        0    88172 2023-04-08 01:38:59.671132 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/shn_dict
+-rw-r--r--   0        0        0    85384 2023-04-08 01:38:59.673664 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/si_dict
+-rw-r--r--   0        0        0     1783 2023-04-08 01:38:59.673664 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/sjn_dict
+-rw-r--r--   0        0        0    50002 2023-04-08 01:38:59.673664 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/sk_dict
+-rw-r--r--   0        0        0    45047 2023-04-08 01:38:59.673664 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/sl_dict
+-rw-r--r--   0        0        0    35095 2023-04-08 01:38:59.673664 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/smj_dict
+-rw-r--r--   0        0        0    45003 2023-04-08 01:38:59.673664 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/sq_dict
+-rw-r--r--   0        0        0    46832 2023-04-08 01:38:59.681384 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/sr_dict
+-rw-r--r--   0        0        0    47836 2023-04-08 01:38:59.681384 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/sv_dict
+-rw-r--r--   0        0        0    47804 2023-04-08 01:38:59.681384 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/sw_dict
+-rw-r--r--   0        0        0   209553 2023-04-08 01:38:59.681384 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ta_dict
+-rw-r--r--   0        0        0    94837 2023-04-08 01:38:59.681384 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/te_dict
+-rw-r--r--   0        0        0     2301 2023-04-08 01:38:59.681384 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/th_dict
+-rw-r--r--   0        0        0    20868 2023-04-08 01:38:59.681384 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/tk_dict
+-rw-r--r--   0        0        0     3072 2023-04-08 01:38:59.681384 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/tn_dict
+-rw-r--r--   0        0        0    46793 2023-04-08 01:38:59.689682 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/tr_dict
+-rw-r--r--   0        0        0     2121 2023-04-08 01:38:59.689682 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/tt_dict
+-rw-r--r--   0        0        0     2070 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ug_dict
+-rw-r--r--   0        0        0     3492 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/uk_dict
+-rw-r--r--   0        0        0   133556 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ur_dict
+-rw-r--r--   0        0        0     2540 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/uz_dict
+-rw-r--r--   0        0        0    52608 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/vi_dict
+-rw-r--r--   0        0        0       81 2023-04-08 01:38:59.701664 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/adam
+-rw-r--r--   0        0        0      138 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Alex
+-rw-r--r--   0        0        0      474 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Alicia
+-rw-r--r--   0        0        0      376 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Andrea
+-rw-r--r--   0        0        0      320 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Andy
+-rw-r--r--   0        0        0      518 2023-04-08 01:38:59.701664 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/anika
+-rw-r--r--   0        0        0      538 2023-04-08 01:38:59.701664 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/anikaRobot
+-rw-r--r--   0        0        0      315 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Annie
+-rw-r--r--   0        0        0      317 2023-04-08 01:38:59.701664 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/announcer
+-rw-r--r--   0        0        0      402 2023-04-08 01:38:59.701664 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/antonio
+-rw-r--r--   0        0        0      361 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/AnxiousAndy
+-rw-r--r--   0        0        0      358 2023-04-08 01:38:59.701664 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/aunty
+-rw-r--r--   0        0        0      360 2023-04-08 01:38:59.701664 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/belinda
+-rw-r--r--   0        0        0      212 2023-04-08 01:38:59.701664 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/benjamin
+-rw-r--r--   0        0        0      224 2023-04-08 01:38:59.701664 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/boris
+-rw-r--r--   0        0        0       62 2023-04-08 01:38:59.701664 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/caleb
+-rw-r--r--   0        0        0      104 2023-04-08 01:38:59.701664 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/croak
+-rw-r--r--   0        0        0      120 2023-04-08 01:38:59.701664 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/david
+-rw-r--r--   0        0        0     3858 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Demonic
+-rw-r--r--   0        0        0      305 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Denis
+-rw-r--r--   0        0        0      401 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Diogo
+-rw-r--r--   0        0        0      303 2023-04-08 01:38:59.701664 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/ed
+-rw-r--r--   0        0        0      161 2023-04-08 01:38:59.705804 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/edward
+-rw-r--r--   0        0        0      162 2023-04-08 01:38:59.705804 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/edward2
+-rw-r--r--   0        0        0      342 2023-04-08 01:38:59.705804 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/f1
+-rw-r--r--   0        0        0      378 2023-04-08 01:38:59.705804 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/f2
+-rw-r--r--   0        0        0      397 2023-04-08 01:38:59.705804 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/f3
+-rw-r--r--   0        0        0      368 2023-04-08 01:38:59.705804 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/f4
+-rw-r--r--   0        0        0      455 2023-04-08 01:38:59.705804 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/f5
+-rw-r--r--   0        0        0      156 2023-04-08 01:38:59.705804 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/fast
+-rw-r--r--   0        0        0      281 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Gene
+-rw-r--r--   0        0        0      283 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Gene2
+-rw-r--r--   0        0        0      279 2023-04-08 01:38:59.705804 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/grandma
+-rw-r--r--   0        0        0      270 2023-04-08 01:38:59.705804 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/grandpa
+-rw-r--r--   0        0        0      270 2023-04-08 01:38:59.705804 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/gustave
+-rw-r--r--   0        0        0      403 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Henrique
+-rw-r--r--   0        0        0      400 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Hugo
+-rw-r--r--   0        0        0     3168 2023-04-08 01:38:59.705804 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/ian
+-rw-r--r--   0        0        0      274 2023-04-08 01:38:59.711418 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/iven
+-rw-r--r--   0        0        0      293 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/iven2
+-rw-r--r--   0        0        0      275 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/iven3
+-rw-r--r--   0        0        0      274 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/iven4
+-rw-r--r--   0        0        0      267 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Jacky
+-rw-r--r--   0        0        0     3186 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/john
+-rw-r--r--   0        0        0      361 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/kaukovalta
+-rw-r--r--   0        0        0       42 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/klatt
+-rw-r--r--   0        0        0       42 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/klatt2
+-rw-r--r--   0        0        0       43 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/klatt3
+-rw-r--r--   0        0        0       43 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/klatt4
+-rw-r--r--   0        0        0       43 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/klatt5
+-rw-r--r--   0        0        0       43 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/klatt6
+-rw-r--r--   0        0        0      338 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Lee
+-rw-r--r--   0        0        0      370 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/linda
+-rw-r--r--   0        0        0      355 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/m1
+-rw-r--r--   0        0        0      279 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/m2
+-rw-r--r--   0        0        0      317 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/m3
+-rw-r--r--   0        0        0      307 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/m4
+-rw-r--r--   0        0        0      277 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/m5
+-rw-r--r--   0        0        0      201 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/m6
+-rw-r--r--   0        0        0      271 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/m7
+-rw-r--r--   0        0        0      300 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/m8
+-rw-r--r--   0        0        0      268 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/marcelo
+-rw-r--r--   0        0        0      467 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Marco
+-rw-r--r--   0        0        0      270 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Mario
+-rw-r--r--   0        0        0      225 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/max
+-rw-r--r--   0        0        0      270 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Michael
+-rw-r--r--   0        0        0      404 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/michel
+-rw-r--r--   0        0        0      404 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/miguel
+-rw-r--r--   0        0        0      119 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Mike
+-rw-r--r--   0        0        0      200 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/mike2
+-rw-r--r--   0        0        0     3193 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Mr serious
+-rw-r--r--   0        0        0      296 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Nguyen
+-rw-r--r--   0        0        0     3189 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/norbert
+-rw-r--r--   0        0        0     3194 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/pablo
+-rw-r--r--   0        0        0      300 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/paul
+-rw-r--r--   0        0        0      375 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/pedro
+-rw-r--r--   0        0        0      354 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/quincy
+-rw-r--r--   0        0        0      217 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Reed
+-rw-r--r--   0        0        0      249 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/RicishayMax
+-rw-r--r--   0        0        0      460 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/RicishayMax2
+-rw-r--r--   0        0        0      460 2023-04-08 01:38:59.691286 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/RicishayMax3
+-rw-r--r--   0        0        0      265 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/rob
+-rw-r--r--   0        0        0      274 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/robert
+-rw-r--r--   0        0        0      477 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/robosoft
+-rw-r--r--   0        0        0      480 2023-04-08 01:38:59.711647 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/robosoft2
+-rw-r--r--   0        0        0      481 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/robosoft3
+-rw-r--r--   0        0        0      472 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/robosoft4
+-rw-r--r--   0        0        0      470 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/robosoft5
+-rw-r--r--   0        0        0      302 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/robosoft6
+-rw-r--r--   0        0        0      435 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/robosoft7
+-rw-r--r--   0        0        0      259 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/robosoft8
+-rw-r--r--   0        0        0      555 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/sandro
+-rw-r--r--   0        0        0      297 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/shelby
+-rw-r--r--   0        0        0      385 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/steph
+-rw-r--r--   0        0        0      388 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/steph2
+-rw-r--r--   0        0        0      399 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/steph3
+-rw-r--r--   0        0        0      420 2023-04-08 01:38:59.701379 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Storm
+-rw-r--r--   0        0        0      383 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/travis
+-rw-r--r--   0        0        0     3189 2023-04-08 01:38:59.701664 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Tweaky
+-rw-r--r--   0        0        0      417 2023-04-08 01:38:59.701664 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/UniRobot
+-rw-r--r--   0        0        0      268 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/victor
+-rw-r--r--   0        0        0      199 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/whisper
+-rw-r--r--   0        0        0      416 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/whisperf
+-rw-r--r--   0        0        0      275 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/zac
+-rw-r--r--   0        0        0   563571 2023-04-08 01:38:59.721491 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/yue_dict
+-rw-r--r--   0        0        0   526336 2023-04-08 01:38:59.731771 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-x64.dll
+-rw-r--r--   0        0        0   378880 2023-04-08 01:38:59.731771 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-x86.dll
+-rw-r--r--   0        0        0        0 2021-10-11 19:47:08.000000 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/py.typed
+-rw-r--r--   0        0        0        7 2023-04-08 14:57:30.982438 espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/VERSION
+-rw-r--r--   0        0        0    35147 2021-10-11 19:47:08.000000 espeak_phonemizer_windows-1.0.3.post0/LICENSE
+-rw-r--r--   0        0        0      851 2023-04-13 10:14:20.354487 espeak_phonemizer_windows-1.0.3.post0/pyproject.toml
+-rw-r--r--   0        0        0     1486 2023-02-24 17:02:27.801498 espeak_phonemizer_windows-1.0.3.post0/README.md
+-rw-r--r--   0        0        0     4437 1970-01-01 00:00:00.000000 espeak_phonemizer_windows-1.0.3.post0/setup.py
+-rw-r--r--   0        0        0     2487 1970-01-01 00:00:00.000000 espeak_phonemizer_windows-1.0.3.post0/PKG-INFO
```

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/__init__.py` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -127,23 +127,7 @@
         if phoneme_separator:
             phonemes_str = re.sub(
                 "[" + re.escape(phoneme_separator) + "]+",
                 phoneme_separator,
                 phonemes_str,
             )
         return phonemes_str
-
-    @staticmethod
-    def _call_espeakng(args, popen_kwargs=None):
-        popen_kwargs = popen_kwargs or {}
-        args = [os.fspath(ESPEAK_NG_EXE), *args]
-        startupinfo = subprocess.STARTUPINFO()
-        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
-        ret = subprocess.run(
-            " ".join(args),
-            capture_output=True,
-            creationflags=subprocess.CREATE_NO_WINDOW,
-            startupinfo=startupinfo,
-            **popen_kwargs,
-        )
-        ret.check_returncode()
-        return ret.stdout
```

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/__main__.py` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/__main__.py`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/af_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/af_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/am_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/am_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/an_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/an_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ar_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ar_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/as_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/as_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/az_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/az_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ba_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ba_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/be_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/be_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/bg_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/bg_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/bn_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/bn_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/bpy_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/bpy_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/bs_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/bs_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ca_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ca_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/chr_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/chr_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/cmn_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/cmn_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/cs_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/cs_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/cv_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/cv_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/cy_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/cy_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/da_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/da_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/de_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/de_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/el_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/el_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/en_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/en_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/eo_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/eo_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/es_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/es_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/et_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/et_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/eu_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/eu_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/fa_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/fa_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/fi_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/fi_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/fr_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/fr_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ga_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ga_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/gd_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/gd_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/gn_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/gn_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/grc_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/grc_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/gu_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/gu_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/hak_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/hak_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/haw_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/haw_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/he_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/he_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/hi_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/hi_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/hr_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/hr_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ht_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ht_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/hu_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/hu_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/hy_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/hy_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ia_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ia_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/id_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/id_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/intonations` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/intonations`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/io_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/io_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/is_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/is_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/it_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/it_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ja_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ja_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/jbo_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/jbo_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ka_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ka_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/kk_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/kk_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/kl_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/kl_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/kn_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/kn_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ko_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ko_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/kok_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/kok_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ku_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ku_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ky_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ky_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/la_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/la_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/iro/chr` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/iro/chr`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/sit/cmn` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lang/sit/cmn`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lb_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lb_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lfn_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lfn_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lt_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lt_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/lv_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/lv_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/mi_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/mi_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/mk_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/mk_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ml_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ml_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/mr_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/mr_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ms_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ms_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/mt_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/mt_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/mto_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/mto_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/my_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/my_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/nci_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/nci_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ne_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ne_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/nl_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/nl_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/no_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/no_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/nog_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/nog_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/om_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/om_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/or_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/or_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/pa_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/pa_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/pap_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/pap_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/phondata` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/phondata`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/phondata-manifest` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/phondata-manifest`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/phonindex` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/phonindex`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/phontab` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/phontab`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/piqd_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/piqd_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/pl_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/pl_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/pt_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/pt_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/py_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/py_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/qdb_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/qdb_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/qu_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/qu_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/quc_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/quc_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/qya_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/qya_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ro_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ro_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ru_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ru_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/sd_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/sd_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/shn_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/shn_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/si_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/si_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/sjn_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/sjn_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/sk_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/sk_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/sl_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/sl_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/smj_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/smj_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/sq_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/sq_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/sr_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/sr_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/sv_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/sv_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/sw_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/sw_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ta_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ta_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/te_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/te_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/th_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/th_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/tk_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/tk_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/tn_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/tn_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/tr_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/tr_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/tt_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/tt_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ug_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ug_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/uk_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/uk_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/ur_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/ur_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/uz_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/uz_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/vi_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/vi_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/anika` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/anika`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/anikaRobot` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/anikaRobot`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Demonic` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Demonic`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/ian` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/ian`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/john` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/john`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Mr serious` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Mr serious`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/norbert` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/norbert`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/pablo` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/pablo`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/sandro` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/sandro`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Tweaky` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/voices/!v/Tweaky`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-data/yue_dict` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-data/yue_dict`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-x64.dll` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-x64.dll`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/espeak_phonemizer/espeak-ng/espeak-ng-x86.dll` & `espeak_phonemizer_windows-1.0.3.post0/espeak_phonemizer/espeak-ng/espeak-ng-x86.dll`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/LICENSE` & `espeak_phonemizer_windows-1.0.3.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/pyproject.toml` & `espeak_phonemizer_windows-1.0.3.post0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "espeak-phonemizer-windows"
-version = "1.0.3"
+version = "1.0.3.post0"
 description = "Uses espeak-ng to transform text into IPA phonemes."
 authors = ["mush42 <ibnomer2011@hotmail.com>"]
 license = "GNU GENERAL PUBLIC LICENSE"
 readme = "README.md"
 packages = [{include = "espeak_phonemizer"}]
 repository = "https://github.com/mush42/espeak-phonemizer-windows"
 keywords = ["espeak", "phonemes", "ipa", "nlp"]
```

### Comparing `espeak_phonemizer_windows-1.0.3/README.md` & `espeak_phonemizer_windows-1.0.3.post0/README.md`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer_windows-1.0.3/setup.py` & `espeak_phonemizer_windows-1.0.3.post0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
                        'espeak-ng/espeak-ng-data/lang/zle/*',
                        'espeak-ng/espeak-ng-data/lang/zls/*',
                        'espeak-ng/espeak-ng-data/lang/zlw/*',
                        'espeak-ng/espeak-ng-data/voices/!v/*']}
 
 setup_kwargs = {
     'name': 'espeak-phonemizer-windows',
-    'version': '1.0.3',
+    'version': '1.0.3.post0',
     'description': 'Uses espeak-ng to transform text into IPA phonemes.',
     'long_description': "# eSpeak Phonemizer Windows\n\n\nUses [espeak-ng](https://github.com/espeak-ng/espeak-ng) to transform text into [IPA](https://en.wikipedia.org/wiki/International_Phonetic_Alphabet) phonemes.\n\nThis is a fork of [espeak-phonemizer](https://github.com/rhasspy/espeak-phonemizer) that adds support for Windows.\n\n## Installation\n\n```sh\npip install espeak_phonemizer_windows\n```\n\nIf installation was successful, you should be able to run:\n\n```sh\nespeak-phonemizer --version\n```\n\n## Basic Phonemization\n\nSimply pass your text into the standard input of `espeak-phonemizer`:\n\n```sh\necho 'This is a test.' | espeak-phonemizer -v en-us\nðɪs ɪz ɐ tˈɛst\n```\n\n### Separators\n\nPhoneme and word separators can be changed:\n\n```sh\necho 'This is a test.' | espeak-phonemizer -v en-us -p '_' -w '#'\nð_ɪ_s#ɪ_z#ɐ#t_ˈɛ_s_t\n```\n\n### Punctuation and Stress\n\nSome punctuation can be kept (.,;:!?) in the output:\n\n```sh\necho 'This: is, a, test.' | espeak-phonemizer -v en-us --keep-punctuation\nðˈɪs: ˈɪz, ˈeɪ, tˈɛst.\n```\n\nStress markers can also be dropped:\n\n```sh\necho 'This is a test.' | espeak-phonemizer -v en-us --no-stress\nðɪs ɪz ɐ tɛst\n```\n\n### Delimited Input\n\nThe `--csv` flag enables delimited input with fields separated by a '|' (change with `--csv-delimiter`):\n\n```sh\necho 's1|This is a test.' | espeak-phonemizer -v en-us --csv\ns1|This is a test.|ðɪs ɪz ɐ tˈɛst\n```\n\nPhonemes are added as a final column, allowing you to pass arbitrary metadata through to the output.\n\n",
     'author': 'mush42',
     'author_email': 'ibnomer2011@hotmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mush42/espeak-phonemizer-windows',
```

### Comparing `espeak_phonemizer_windows-1.0.3/PKG-INFO` & `espeak_phonemizer_windows-1.0.3.post0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: espeak-phonemizer-windows
-Version: 1.0.3
+Version: 1.0.3.post0
 Summary: Uses espeak-ng to transform text into IPA phonemes.
 Home-page: https://github.com/mush42/espeak-phonemizer-windows
 License: GNU GENERAL PUBLIC LICENSE
 Keywords: espeak,phonemes,ipa,nlp
 Author: mush42
 Author-email: ibnomer2011@hotmail.com
 Requires-Python: >=3.8,<4.0
```

