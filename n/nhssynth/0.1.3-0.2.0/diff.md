# Comparing `tmp/nhssynth-0.1.3.tar.gz` & `tmp/nhssynth-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhssynth-0.1.3.tar", max compression
+gzip compressed data, was "nhssynth-0.2.0.tar", max compression
```

## Comparing `nhssynth-0.1.3.tar` & `nhssynth-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,36 @@
--rw-r--r--   0        0        0     1084 2023-02-01 13:23:29.096760 nhssynth-0.1.3/LICENSE
--rw-r--r--   0        0        0     5433 2023-03-23 23:18:59.770745 nhssynth-0.1.3/README.md
--rw-r--r--   0        0        0      937 2023-03-24 18:19:28.165500 nhssynth-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       21 2023-03-21 11:15:21.821516 nhssynth-0.1.3/src/nhssynth/cli/__init__.py
--rw-r--r--   0        0        0     4821 2023-03-24 17:43:01.770932 nhssynth-0.1.3/src/nhssynth/cli/config.py
--rw-r--r--   0        0        0     2923 2023-03-24 17:36:32.373605 nhssynth-0.1.3/src/nhssynth/cli/module_arguments.py
--rw-r--r--   0        0        0     3985 2023-03-24 13:36:30.996293 nhssynth-0.1.3/src/nhssynth/cli/module_setup.py
--rw-r--r--   0        0        0     1786 2023-03-24 17:35:39.873937 nhssynth-0.1.3/src/nhssynth/cli/run.py
--rw-r--r--   0        0        0     2450 2023-03-23 23:10:34.064001 nhssynth-0.1.3/src/nhssynth/modules/README.md
--rw-r--r--   0        0        0        0 2023-03-09 10:01:33.834460 nhssynth-0.1.3/src/nhssynth/modules/__init__.py
--rw-r--r--   0        0        0       20 2023-03-06 16:05:17.363712 nhssynth-0.1.3/src/nhssynth/modules/dataloader/__init__.py
--rw-r--r--   0        0        0     2126 2023-03-23 10:32:55.324292 nhssynth-0.1.3/src/nhssynth/modules/dataloader/io.py
--rw-r--r--   0        0        0     4276 2023-03-24 15:20:03.836219 nhssynth-0.1.3/src/nhssynth/modules/dataloader/metadata.py
--rw-r--r--   0        0        0     1234 2023-03-24 18:14:27.543402 nhssynth-0.1.3/src/nhssynth/modules/dataloader/run.py
--rw-r--r--   0        0        0     4252 2023-03-24 18:14:41.762523 nhssynth-0.1.3/src/nhssynth/modules/dataloader/transformers.py
--rw-r--r--   0        0        0      116 2023-03-23 22:38:49.434395 nhssynth-0.1.3/src/nhssynth/modules/dataloader/utils.py
--rw-r--r--   0        0        0       21 2023-03-07 10:58:04.573024 nhssynth-0.1.3/src/nhssynth/modules/evaluation/__init__.py
--rw-r--r--   0        0        0     3378 2023-03-05 19:45:22.243339 nhssynth-0.1.3/src/nhssynth/modules/evaluation/metrics.py
--rw-r--r--   0        0        0       74 2023-03-05 21:00:46.165508 nhssynth-0.1.3/src/nhssynth/modules/evaluation/run.py
--rw-r--r--   0        0        0    13768 2023-03-03 14:03:40.821108 nhssynth-0.1.3/src/nhssynth/modules/model/DPVAE.py
--rw-r--r--   0        0        0       21 2023-03-07 10:57:59.963528 nhssynth-0.1.3/src/nhssynth/modules/model/__init__.py
--rw-r--r--   0        0        0       82 2023-03-05 21:01:00.847483 nhssynth-0.1.3/src/nhssynth/modules/model/run.py
--rw-r--r--   0        0        0       21 2023-03-07 10:58:07.632275 nhssynth-0.1.3/src/nhssynth/modules/plotting/__init__.py
--rw-r--r--   0        0        0     4654 2023-03-05 19:45:22.243598 nhssynth-0.1.3/src/nhssynth/modules/plotting/plot.py
--rw-r--r--   0        0        0       72 2023-03-05 21:00:32.043935 nhssynth-0.1.3/src/nhssynth/modules/plotting/run.py
--rw-r--r--   0        0        0       21 2023-03-07 10:58:13.024183 nhssynth-0.1.3/src/nhssynth/modules/structure/__init__.py
--rw-r--r--   0        0        0       85 2023-03-07 10:58:26.227434 nhssynth-0.1.3/src/nhssynth/modules/structure/run.py
--rw-r--r--   0        0        0       21 2023-03-24 16:45:18.774121 nhssynth-0.1.3/src/nhssynth/utils/__init__.py
--rw-r--r--   0        0        0       66 2023-03-21 10:59:18.970394 nhssynth-0.1.3/src/nhssynth/utils/constants.py
--rw-r--r--   0        0        0    19406 2023-03-24 15:19:45.781242 nhssynth-0.1.3/src/nhssynth/utils/utils.py
--rw-r--r--   0        0        0     9093 1970-01-01 00:00:00.000000 nhssynth-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-03-31 11:03:40.629205 nhssynth-0.2.0/LICENSE
+-rw-r--r--   0        0        0     6290 2023-04-05 14:58:26.929685 nhssynth-0.2.0/README.md
+-rw-r--r--   0        0        0     1360 2023-04-13 14:44:05.536456 nhssynth-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-03-21 11:15:21.821516 nhssynth-0.2.0/src/nhssynth/cli/__init__.py
+-rw-r--r--   0        0        0     2690 2023-04-12 17:47:54.764686 nhssynth-0.2.0/src/nhssynth/cli/common_arguments.py
+-rw-r--r--   0        0        0     8743 2023-04-13 12:22:56.987449 nhssynth-0.2.0/src/nhssynth/cli/config.py
+-rw-r--r--   0        0        0     7024 2023-04-13 13:06:51.351173 nhssynth-0.2.0/src/nhssynth/cli/module_arguments.py
+-rw-r--r--   0        0        0     6968 2023-04-13 10:55:06.840859 nhssynth-0.2.0/src/nhssynth/cli/module_setup.py
+-rw-r--r--   0        0        0     1409 2023-04-13 13:03:16.862839 nhssynth-0.2.0/src/nhssynth/cli/run.py
+-rw-r--r--   0        0        0       82 2023-04-04 13:59:35.254031 nhssynth-0.2.0/src/nhssynth/common/__init__.py
+-rw-r--r--   0        0        0      292 2023-04-13 15:21:59.569403 nhssynth-0.2.0/src/nhssynth/common/common.py
+-rw-r--r--   0        0        0     3339 2023-04-13 09:38:21.025865 nhssynth-0.2.0/src/nhssynth/common/constants.py
+-rw-r--r--   0        0        0     2078 2023-04-04 13:59:35.254363 nhssynth-0.2.0/src/nhssynth/common/dicts.py
+-rw-r--r--   0        0        0     2953 2023-04-12 15:31:20.079017 nhssynth-0.2.0/src/nhssynth/common/io.py
+-rw-r--r--   0        0        0        0 2023-03-09 10:01:33.834460 nhssynth-0.2.0/src/nhssynth/modules/__init__.py
+-rw-r--r--   0        0        0       20 2023-03-06 16:05:17.363712 nhssynth-0.2.0/src/nhssynth/modules/dataloader/__init__.py
+-rw-r--r--   0        0        0     4082 2023-04-12 15:32:23.986086 nhssynth-0.2.0/src/nhssynth/modules/dataloader/io.py
+-rw-r--r--   0        0        0     5253 2023-04-12 15:46:13.535858 nhssynth-0.2.0/src/nhssynth/modules/dataloader/metadata.py
+-rw-r--r--   0        0        0    20155 2023-04-12 15:46:09.143287 nhssynth-0.2.0/src/nhssynth/modules/dataloader/metatransformer.py
+-rw-r--r--   0        0        0     1596 2023-04-13 12:33:38.185534 nhssynth-0.2.0/src/nhssynth/modules/dataloader/run.py
+-rw-r--r--   0        0        0       21 2023-03-07 10:58:04.573024 nhssynth-0.2.0/src/nhssynth/modules/evaluation/__init__.py
+-rw-r--r--   0        0        0    13625 2023-04-13 15:23:11.578297 nhssynth-0.2.0/src/nhssynth/modules/evaluation/full_report.py
+-rw-r--r--   0        0        0     2644 2023-04-13 10:57:28.285918 nhssynth-0.2.0/src/nhssynth/modules/evaluation/io.py
+-rw-r--r--   0        0        0     3031 2023-04-11 16:04:10.935343 nhssynth-0.2.0/src/nhssynth/modules/evaluation/metrics.py
+-rw-r--r--   0        0        0     1856 2023-04-13 15:24:02.908325 nhssynth-0.2.0/src/nhssynth/modules/evaluation/run.py
+-rw-r--r--   0        0        0     8488 2023-04-13 12:51:55.098685 nhssynth-0.2.0/src/nhssynth/modules/model/DPVAE.py
+-rw-r--r--   0        0        0       21 2023-03-07 10:57:59.963528 nhssynth-0.2.0/src/nhssynth/modules/model/__init__.py
+-rw-r--r--   0        0        0     3092 2023-04-12 15:33:11.172294 nhssynth-0.2.0/src/nhssynth/modules/model/io.py
+-rw-r--r--   0        0        0     3510 2023-04-13 12:45:23.368814 nhssynth-0.2.0/src/nhssynth/modules/model/run.py
+-rw-r--r--   0        0        0       21 2023-03-07 10:58:07.632275 nhssynth-0.2.0/src/nhssynth/modules/plotting/__init__.py
+-rw-r--r--   0        0        0     2611 2023-04-13 11:19:38.014249 nhssynth-0.2.0/src/nhssynth/modules/plotting/io.py
+-rw-r--r--   0        0        0     6510 2023-04-13 12:13:35.989347 nhssynth-0.2.0/src/nhssynth/modules/plotting/plots.py
+-rw-r--r--   0        0        0      727 2023-04-13 12:33:18.866696 nhssynth-0.2.0/src/nhssynth/modules/plotting/run.py
+-rw-r--r--   0        0        0       21 2023-03-07 10:58:13.024183 nhssynth-0.2.0/src/nhssynth/modules/structure/__init__.py
+-rw-r--r--   0        0        0       85 2023-03-07 10:58:26.227434 nhssynth-0.2.0/src/nhssynth/modules/structure/run.py
+-rw-r--r--   0        0        0     7605 1970-01-01 00:00:00.000000 nhssynth-0.2.0/PKG-INFO
```

### Comparing `nhssynth-0.1.3/LICENSE` & `nhssynth-0.2.0/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 NHS England and Improvement
+Copyright (c) 2023 NHS England
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `nhssynth-0.1.3/README.md` & `nhssynth-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,340 +1,394 @@
-00000000: 2320 4e48 5320 5379 6e74 680a 0a3c 6469  # NHS Synth..<di
-00000010: 7620 616c 6967 6e3d 2263 656e 7465 7222  v align="center"
-00000020: 3e0a 0a5b 215b 5079 5049 202d 204c 6174  >..[![PyPI - Lat
-00000030: 6573 7420 5265 6c65 6173 655d 2868 7474  est Release](htt
-00000040: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000050: 2e69 6f2f 7079 7069 2f76 2f6e 6873 7379  .io/pypi/v/nhssy
-00000060: 6e74 683f 7374 796c 653d 666c 6174 2d73  nth?style=flat-s
-00000070: 7175 6172 6529 5d28 6874 7470 733a 2f2f  quare)](https://
-00000080: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
-00000090: 2f6e 6873 7379 6e74 682f 290a 5b21 5b50  /nhssynth/).[![P
-000000a0: 7950 4920 2d20 5768 6565 6c5d 2868 7474  yPI - Wheel](htt
-000000b0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-000000c0: 2e69 6f2f 7079 7069 2f77 6865 656c 2f6e  .io/pypi/wheel/n
-000000d0: 6873 7379 6e74 683f 7374 796c 653d 666c  hssynth?style=fl
-000000e0: 6174 2d73 7175 6172 6529 5d28 6874 7470  at-square)](http
-000000f0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-00000100: 6a65 6374 2f6e 6873 7379 6e74 682f 290a  ject/nhssynth/).
-00000110: 5b21 5b50 7950 4920 2d20 5061 636b 6167  [![PyPI - Packag
-00000120: 6520 5374 6174 7573 5d28 6874 7470 733a  e Status](https:
-00000130: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000140: 2f70 7970 692f 7374 6174 7573 2f6e 6873  /pypi/status/nhs
-00000150: 7379 6e74 683f 7374 796c 653d 666c 6174  synth?style=flat
-00000160: 2d73 7175 6172 6529 5d28 6874 7470 733a  -square)](https:
-00000170: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-00000180: 6374 2f6e 6873 7379 6e74 682f 290a 5b21  ct/nhssynth/).[!
-00000190: 5b50 7950 4920 2d20 5079 7468 6f6e 2056  [PyPI - Python V
-000001a0: 6572 7369 6f6e 5d28 6874 7470 733a 2f2f  ersion](https://
-000001b0: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
-000001c0: 7970 692f 7079 7665 7273 696f 6e73 2f6e  ypi/pyversions/n
-000001d0: 6873 7379 6e74 683f 7374 796c 653d 666c  hssynth?style=fl
-000001e0: 6174 2d73 7175 6172 6529 5d28 6874 7470  at-square)](http
-000001f0: 733a 2f2f 7777 772e 7079 7468 6f6e 2e6f  s://www.python.o
-00000200: 7267 2f64 6f77 6e6c 6f61 6473 2f72 656c  rg/downloads/rel
-00000210: 6561 7365 2f70 7974 686f 6e2d 3331 3030  ease/python-3100
-00000220: 2f29 0a5b 215b 5079 5049 202d 204c 6963  /).[![PyPI - Lic
-00000230: 656e 7365 5d28 6874 7470 733a 2f2f 696d  ense](https://im
-00000240: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
-00000250: 692f 6c2f 6e68 7373 796e 7468 3f73 7479  i/l/nhssynth?sty
-00000260: 6c65 3d66 6c61 742d 7371 7561 7265 295d  le=flat-square)]
-00000270: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000280: 636f 6d2f 6e68 7378 2f6e 6873 7379 6e74  com/nhsx/nhssynt
-00000290: 682f 626c 6f62 2f6d 6169 6e2f 4c49 4345  h/blob/main/LICE
-000002a0: 4e53 4529 0a5b 215b 436f 6465 2073 7479  NSE).[![Code sty
-000002b0: 6c65 3a20 626c 6163 6b5d 2868 7474 7073  le: black](https
-000002c0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-000002d0: 6f2f 6261 6467 652f 636f 6465 2532 3073  o/badge/code%20s
-000002e0: 7479 6c65 2d62 6c61 636b 2d30 3030 3030  tyle-black-00000
-000002f0: 303f 7374 796c 653d 666c 6174 2d73 7175  0?style=flat-squ
-00000300: 6172 6529 5d28 6874 7470 733a 2f2f 6769  are)](https://gi
-00000310: 7468 7562 2e63 6f6d 2f70 7366 2f62 6c61  thub.com/psf/bla
-00000320: 636b 290a 5b21 5b49 6d70 6f72 7473 3a20  ck).[![Imports: 
-00000330: 6973 6f72 745d 2868 7474 7073 3a2f 2f69  isort](https://i
-00000340: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
-00000350: 6467 652f 2532 3069 6d70 6f72 7473 2d69  dge/%20imports-i
-00000360: 736f 7274 2d25 3233 3136 3734 6231 3f73  sort-%231674b1?s
-00000370: 7479 6c65 3d66 6c61 742d 7371 7561 7265  tyle=flat-square
-00000380: 295d 2868 7474 7073 3a2f 2f70 7963 7161  )](https://pycqa
-00000390: 2e67 6974 6875 622e 696f 2f69 736f 7274  .github.io/isort
-000003a0: 2f29 0a0a 3c2f 6469 763e 0a0a 2323 2041  /)..</div>..## A
-000003b0: 626f 7574 2074 6865 2050 726f 6a65 6374  bout the Project
-000003c0: 0a0a 5468 6520 7072 6f6a 6563 7420 6375  ..The project cu
-000003d0: 7272 656e 746c 7920 636f 6e73 6973 7473  rrently consists
-000003e0: 206f 6620 6120 5079 7468 6f6e 2070 6163   of a Python pac
-000003f0: 6b61 6765 2061 6c6f 6e67 7369 6465 2072  kage alongside r
-00000400: 6573 6561 7263 6820 616e 6420 696e 7665  esearch and inve
-00000410: 7374 6967 6174 6976 6520 6d61 7465 7269  stigative materi
-00000420: 616c 7320 636f 7665 7269 6e67 2074 6865  als covering the
-00000430: 2065 6666 6563 7469 7665 6e65 7373 206f   effectiveness o
-00000440: 6620 7468 6520 7061 636b 6167 6520 616e  f the package an
-00000450: 6420 7379 6e74 6865 7469 6320 6461 7461  d synthetic data
-00000460: 206d 6f72 6520 6765 6e65 7261 6c6c 7920   more generally 
-00000470: 7768 656e 2061 7070 6c69 6564 2074 6f20  when applied to 
-00000480: 4e48 5320 7573 6520 6361 7365 732e 0a0a  NHS use cases...
-00000490: 5b50 726f 6a65 6374 2044 6573 6372 6970  [Project Descrip
-000004a0: 7469 6f6e 202d 2053 796e 7468 6574 6963  tion - Synthetic
-000004b0: 2044 6174 6120 4578 706c 6f72 6174 696f   Data Exploratio
-000004c0: 6e3a 2056 6172 6961 7469 6f6e 616c 2041  n: Variational A
-000004d0: 7574 6f65 6e63 6f64 6572 735d 2868 7474  utoencoders](htt
-000004e0: 7073 3a2f 2f6e 6873 782e 6769 7468 7562  ps://nhsx.github
-000004f0: 2e69 6f2f 6e68 7378 2d69 6e74 6572 6e73  .io/nhsx-interns
-00000500: 6869 702d 7072 6f6a 6563 7473 2f73 796e  hip-projects/syn
-00000510: 7468 6574 6963 2d64 6174 612d 6578 706c  thetic-data-expl
-00000520: 6f72 6174 696f 6e2d 7661 652f 290a 0a54  oration-vae/)..T
-00000530: 6865 2063 6f64 6562 6173 6520 6275 696c  he codebase buil
-00000540: 6473 206f 6e20 7072 6576 696f 7573 204e  ds on previous N
-00000550: 4853 5820 416e 616c 7974 6963 7320 556e  HSX Analytics Un
-00000560: 6974 2050 6844 2069 6e74 6572 6e73 6869  it PhD internshi
-00000570: 7073 2063 6f6e 7465 7874 7561 6c69 7369  ps contextualisi
-00000580: 6e67 2061 6e64 2069 6e76 6573 7469 6761  ng and investiga
-00000590: 7469 6e67 2074 6865 2070 6f74 656e 7469  ting the potenti
-000005a0: 616c 2075 7365 206f 6620 5661 7269 6174  al use of Variat
-000005b0: 696f 6e61 6c20 4175 746f 2045 6e63 6f64  ional Auto Encod
-000005c0: 6572 7320 2856 4145 7329 2066 6f72 2073  ers (VAEs) for s
-000005d0: 796e 7468 6574 6963 2064 6174 6120 6765  ynthetic data ge
-000005e0: 6e65 7261 7469 6f6e 2e20 5468 6573 6520  neration. These 
-000005f0: 7765 7265 2075 6e64 6572 7461 6b65 6e20  were undertaken 
-00000600: 6279 2044 6f6d 696e 6963 2044 616e 6b73  by Dominic Danks
-00000610: 2061 6e64 2044 6176 6964 2042 7269 6e64   and David Brind
-00000620: 2e0a 0a5f 2a2a 4e6f 7465 3a2a 2a20 4e6f  ..._**Note:** No
-00000630: 2064 6174 612c 2070 7562 6c69 6320 6f72   data, public or
-00000640: 2070 7269 7661 7465 2061 7265 2073 6861   private are sha
-00000650: 7265 6420 696e 2074 6869 7320 7265 706f  red in this repo
-00000660: 7369 746f 7279 2e5f 0a0a 2323 2047 6574  sitory._..## Get
-00000670: 7469 6e67 2053 7461 7274 6564 0a0a 2323  ting Started..##
-00000680: 2320 5072 6f6a 6563 7420 5374 7563 7475  # Project Stuctu
-00000690: 7265 0a0a 2d20 5468 6520 6d61 696e 2070  re..- The main p
-000006a0: 6163 6b61 6765 2061 6e64 2063 6f64 6562  ackage and codeb
-000006b0: 6173 6520 6973 2066 6f75 6e64 2069 6e20  ase is found in 
-000006c0: 5b60 7372 632f 6e68 7373 796e 7468 605d  [`src/nhssynth`]
-000006d0: 2829 2028 7365 6520 5573 6167 6520 6265  () (see Usage be
-000006e0: 6c6f 7720 666f 7220 6d6f 7265 2069 6e66  low for more inf
-000006f0: 6f72 6d61 7469 6f6e 290a 2d20 4163 636f  ormation).- Acco
-00000700: 6d70 616e 7969 6e67 206d 6174 6572 6961  mpanying materia
-00000710: 6c73 2061 7265 2061 7661 696c 6162 6c65  ls are available
-00000720: 2069 6e20 7468 6520 6064 6f63 7360 2066   in the `docs` f
-00000730: 6f6c 6465 723a 0a20 202d 2041 205b 7265  older:.  - A [re
-00000740: 706f 7274 5d28 646f 6373 2f72 6570 6f72  port](docs/repor
-00000750: 7473 2f72 6570 6f72 742e 7064 6629 2073  ts/report.pdf) s
-00000760: 756d 6d61 7269 7369 6e67 2074 6865 2070  ummarising the p
-00000770: 7265 7669 6f75 7320 6974 6572 6174 696f  revious iteratio
-00000780: 6e20 6f66 2074 6869 7320 7072 6f6a 6563  n of this projec
-00000790: 740a 2020 2d20 4120 5b6d 6f64 656c 2063  t.  - A [model c
-000007a0: 6172 645d 2864 6f63 732f 6d6f 6465 6c5f  ard](docs/model_
-000007b0: 6361 7264 2e6d 6429 2070 726f 7669 6469  card.md) providi
-000007c0: 6e67 206d 6f72 6520 696e 666f 726d 6174  ng more informat
-000007d0: 696f 6e20 6162 6f75 7420 7468 6520 5641  ion about the VA
-000007e0: 4520 7769 7468 2044 6966 6665 7265 6e74  E with Different
-000007f0: 6961 6c20 5072 6976 6163 790a 2d20 4e75  ial Privacy.- Nu
-00000800: 6d65 726f 7573 205b 6578 656d 706c 6172  merous [exemplar
-00000810: 2063 6f6e 6669 6775 7261 7469 6f6e 735d   configurations]
-00000820: 2863 6f6e 6669 6729 2061 7265 2066 6f75  (config) are fou
-00000830: 6e64 2069 6e20 6063 6f6e 6669 6760 0a2d  nd in `config`.-
-00000840: 2045 6d70 7479 2060 6461 7461 6020 616e   Empty `data` an
-00000850: 6420 6065 7870 6572 696d 656e 7473 6020  d `experiments` 
-00000860: 666f 6c64 6572 7320 6172 6520 7072 6f76  folders are prov
-00000870: 6964 6564 3b20 7468 6573 6520 6172 6520  ided; these are 
-00000880: 7468 6520 6465 6661 756c 7420 6c6f 6361  the default loca
-00000890: 7469 6f6e 7320 666f 7220 696e 7075 7473  tions for inputs
-000008a0: 2061 6e64 206f 7574 7075 7473 2077 6865   and outputs whe
-000008b0: 6e20 7275 6e6e 696e 6720 7468 6520 7072  n running the pr
-000008c0: 6f6a 6563 7420 7573 696e 6720 7468 6520  oject using the 
-000008d0: 7072 6f76 6964 6564 205b 6063 6c69 605d  provided [`cli`]
-000008e0: 2873 7263 2f6e 6873 7379 6e74 682f 636c  (src/nhssynth/cl
-000008f0: 692f 2920 6d6f 6475 6c65 0a2d 2050 7265  i/) module.- Pre
-00000900: 2d70 726f 6365 7373 696e 6720 6e6f 7465  -processing note
-00000910: 626f 6f6b 7320 666f 7220 7370 6563 6966  books for specif
-00000920: 6963 2064 6174 6173 6574 7320 7573 6564  ic datasets used
-00000930: 2074 6f20 6173 7365 7373 2074 6865 2061   to assess the a
-00000940: 7070 726f 6163 6820 616e 6420 6f74 6865  pproach and othe
-00000950: 7220 6e6f 6e2d 636f 7265 2063 6f64 6520  r non-core code 
-00000960: 6361 6e20 6265 2066 6f75 6e64 2069 6e20  can be found in 
-00000970: 5b60 6175 7869 6c69 6172 7960 5d28 6175  [`auxiliary`](au
-00000980: 7869 6c69 6172 792f 290a 0a23 2323 2049  xiliary/)..### I
-00000990: 6e73 7461 6c6c 6174 696f 6e0a 0a41 7320  nstallation..As 
-000009a0: 6974 2073 7461 6e64 732c 2077 6520 7265  it stands, we re
-000009b0: 636f 6d6d 656e 6420 7468 6520 666f 6c6c  commend the foll
-000009c0: 6f77 696e 6720 7374 6570 7320 746f 2072  owing steps to r
-000009d0: 6570 726f 6475 6365 206f 7572 2065 7870  eproduce our exp
-000009e0: 6572 696d 656e 7473 2061 6e64 2066 756c  eriments and ful
-000009f0: 6c79 2077 6f72 6b20 7769 7468 2074 6869  ly work with thi
-00000a00: 7320 7072 6f6a 6563 743a 0a0a 312e 2043  s project:..1. C
-00000a10: 6c6f 6e65 2074 6865 2072 6570 6f0a 322e  lone the repo.2.
-00000a20: 2045 6e73 7572 6520 6f6e 6520 6f66 2074   Ensure one of t
-00000a30: 6865 2072 6571 7569 7265 6420 7665 7273  he required vers
-00000a40: 696f 6e73 206f 6620 5079 7468 6f6e 2069  ions of Python i
-00000a50: 7320 696e 7374 616c 6c65 640a 332e 2049  s installed.3. I
-00000a60: 6e73 7461 6c6c 205b 6070 6f65 7472 7960  nstall [`poetry`
-00000a70: 5d28 6874 7470 733a 2f2f 7079 7468 6f6e  ](https://python
-00000a80: 2d70 6f65 7472 792e 6f72 672f 646f 6373  -poetry.org/docs
-00000a90: 2f23 696e 7374 616c 6c61 7469 6f6e 290a  /#installation).
-00000aa0: 342e 2049 6e73 7461 6e74 6961 7465 2061  4. Instantiate a
-00000ab0: 2076 6972 7475 616c 2065 6e76 6972 6f6e   virtual environ
-00000ac0: 6d65 6e74 2c20 652e 672e 2076 6961 2060  ment, e.g. via `
-00000ad0: 7079 7468 6f6e 202d 6d20 7665 6e76 206e  python -m venv n
-00000ae0: 6873 7379 6e74 6860 0a33 2e20 4163 7469  hssynth`.3. Acti
-00000af0: 7661 7465 2074 6865 2076 6972 7475 616c  vate the virtual
-00000b00: 2065 6e76 6972 6f6e 6d65 6e74 2c20 652e   environment, e.
-00000b10: 672e 2076 6961 2060 736f 7572 6365 206e  g. via `source n
-00000b20: 6873 7379 6e74 682f 6269 6e2f 6163 7469  hssynth/bin/acti
-00000b30: 7661 7465 600a 342e 2049 6e73 7461 6c6c  vate`.4. Install
-00000b40: 2070 726f 6a65 6374 2064 6570 656e 6465   project depende
-00000b50: 6e63 6965 7320 7769 7468 2060 706f 6574  ncies with `poet
-00000b60: 7279 2069 6e73 7461 6c6c 6020 286f 7074  ry install` (opt
-00000b70: 696f 6e61 6c6c 7920 696e 7374 616c 6c20  ionally install 
-00000b80: 606a 7570 7974 6572 6020 616e 6420 606e  `jupyter` and `n
-00000b90: 6f74 6562 6f6f 6b60 2074 6f20 776f 726b  otebook` to work
-00000ba0: 2077 6974 6820 736f 6d65 206f 6620 7468   with some of th
-00000bb0: 6520 7072 6570 726f 6365 7373 696e 6720  e preprocessing 
-00000bc0: 6669 6c65 7320 696e 205b 6061 7578 696c  files in [`auxil
-00000bd0: 6961 7279 605d 2861 7578 696c 6961 7279  iary`](auxiliary
-00000be0: 2f29 290a 352e 2049 6e74 6572 6163 7420  /)).5. Interact 
-00000bf0: 7769 7468 2074 6865 2070 6163 6b61 6765  with the package
-00000c00: 2069 6e20 6f6e 6520 6f66 2074 776f 2077   in one of two w
-00000c10: 6179 733a 0a20 2020 202d 2056 6961 2074  ays:.    - Via t
-00000c20: 6865 205b 6063 6c69 605d 2873 7263 2f6e  he [`cli`](src/n
-00000c30: 6873 7379 6e74 682f 636c 692f 2920 6d6f  hssynth/cli/) mo
-00000c40: 6475 6c65 2075 7369 6e67 2060 706f 6574  dule using `poet
-00000c50: 7279 2072 756e 2063 6c69 600a 2020 2020  ry run cli`.    
-00000c60: 2d20 5468 726f 7567 6820 6275 696c 6469  - Through buildi
-00000c70: 6e67 2074 6865 2070 6163 6b61 6765 2077  ng the package w
-00000c80: 6974 6820 6070 6f65 7472 7920 6275 696c  ith `poetry buil
-00000c90: 6460 2061 6e64 2075 7369 6e67 2069 7420  d` and using it 
-00000ca0: 696e 2061 6e20 6578 6973 7469 6e67 2070  in an existing p
-00000cb0: 726f 6a65 6374 2028 6069 6d70 6f72 7420  roject (`import 
-00000cc0: 6e68 7373 796e 7468 6029 2e20 486f 7765  nhssynth`). Howe
-00000cd0: 7665 722c 2069 6620 796f 7520 696e 7465  ver, if you inte
-00000ce0: 6e64 206f 6e20 646f 696e 6720 7468 6520  nd on doing the 
-00000cf0: 6c61 7474 6572 2069 7420 6d61 7920 6265  latter it may be
-00000d00: 2070 7265 6665 7261 626c 6520 746f 2069   preferable to i
-00000d10: 6e73 7465 6164 2066 6f6c 6c6f 7720 7468  nstead follow th
-00000d20: 6520 7365 636f 6e64 2c20 7369 6d70 6c65  e second, simple
-00000d30: 7220 7365 7475 7020 6265 6c6f 772e 0a0a  r setup below...
-00000d40: 466f 7220 6d6f 7265 2073 7461 6e64 6172  For more standar
-00000d50: 6420 7573 6167 6520 6f66 2074 6865 2070  d usage of the p
-00000d60: 6163 6b61 6765 3a0a 0a31 2e20 5275 6e20  ackage:..1. Run 
-00000d70: 6070 6970 2069 6e73 7461 6c6c 206e 6873  `pip install nhs
-00000d80: 7379 6e74 6860 2077 6974 6869 6e20 6120  synth` within a 
-00000d90: 7375 7070 6f72 7465 6420 5079 7468 6f6e  supported Python
-00000da0: 2069 6e73 7461 6c6c 6174 696f 6e0a 322e   installation.2.
-00000db0: 2055 7365 2074 6865 206d 6f64 756c 6573   Use the modules
-00000dc0: 2065 7870 6f72 7465 6420 6279 2074 6865   exported by the
-00000dd0: 2070 6163 6b61 6765 2061 7320 796f 7520   package as you 
-00000de0: 776f 756c 6420 616e 7920 6f74 6865 722e  would any other.
-00000df0: 205f 4e6f 7465 2074 6861 7420 696e 2074   _Note that in t
-00000e00: 6869 7320 7365 7475 7020 796f 7520 7769  his setup you wi
-00000e10: 6c6c 2068 6176 6520 746f 2077 6f72 6b20  ll have to work 
-00000e20: 6d6f 7265 2063 6c6f 7365 6c79 2077 6974  more closely wit
-00000e30: 6820 7468 6520 636f 6e66 6967 7572 6174  h the configurat
-00000e40: 696f 6e20 616e 6420 636f 6465 2074 6f20  ion and code to 
-00000e50: 656e 7375 7265 2079 6f75 2061 7265 2068  ensure you are h
-00000e60: 616e 646c 696e 6720 696e 7075 7473 2061  andling inputs a
-00000e70: 6e64 206f 7574 7075 7473 2066 6f72 2065  nd outputs for e
-00000e80: 6163 6820 6d6f 6475 6c65 2061 7070 726f  ach module appro
-00000e90: 7072 6961 7465 6c79 2e20 5468 6520 636c  priately. The cl
-00000ea0: 6920 6861 6e64 6c65 7320 6120 6c6f 7420  i handles a lot 
-00000eb0: 6f66 2074 6869 7320 636f 6d70 6c65 7869  of this complexi
-00000ec0: 7479 2c20 616e 6420 696e 7465 7261 6374  ty, and interact
-00000ed0: 696e 6720 7769 7468 2074 6865 206d 6f64  ing with the mod
-00000ee0: 756c 6573 2064 6972 6563 746c 7920 6973  ules directly is
-00000ef0: 2063 6f6e 7369 6465 7265 6420 6164 7661   considered adva
-00000f00: 6e63 6564 2075 7361 6765 2e5f 0a0a 2323  nced usage._..##
-00000f10: 2320 5573 6167 650a 0a54 6869 7320 7061  # Usage..This pa
-00000f20: 636b 6167 6520 636f 6d70 7269 7365 7320  ckage comprises 
-00000f30: 6120 7069 7065 6c69 6e65 2074 6861 7420  a pipeline that 
-00000f40: 6973 2072 756e 6e61 626c 6520 7669 6120  is runnable via 
-00000f50: 6070 6f65 7472 7920 7275 6e20 636c 6920  `poetry run cli 
-00000f60: 7069 7065 6c69 6e65 203c 6172 6773 3e60  pipeline <args>`
-00000f70: 206f 7220 6070 6f65 7472 7920 7275 6e20   or `poetry run 
-00000f80: 636c 6920 636f 6e66 6967 203c 636f 6e66  cli config <conf
-00000f90: 6967 2066 696c 6570 6174 683e 602e 2059  ig filepath>`. Y
-00000fa0: 6f75 2063 616e 2072 756e 2074 6865 206d  ou can run the m
-00000fb0: 6f64 756c 6573 2074 6861 7420 6d61 6b65  odules that make
-00000fc0: 2075 7020 7468 6973 2070 6970 656c 696e   up this pipelin
-00000fd0: 6520 696e 6465 7065 6e64 656e 746c 7920  e independently 
-00000fe0: 7669 6120 6070 6f65 7472 7920 7275 6e20  via `poetry run 
-00000ff0: 636c 6920 3c6d 6f64 756c 6520 6e61 6d65  cli <module name
-00001000: 3e60 2e20 546f 2073 6565 2074 6865 206d  >`. To see the m
-00001010: 6f64 756c 6573 2074 6861 7420 6172 6520  odules that are 
-00001020: 6176 6169 6c61 626c 6520 616e 6420 7468  available and th
-00001030: 6569 7220 636f 7272 6573 706f 6e64 696e  eir correspondin
-00001040: 6720 6172 6775 6d65 6e74 7320 616e 6420  g arguments and 
-00001050: 6675 6e63 7469 6f6e 2c20 7275 6e20 6070  function, run `p
-00001060: 6f65 7472 7920 7275 6e20 636c 6920 2d2d  oetry run cli --
-00001070: 6865 6c70 6020 2f20 6070 6f65 7472 7920  help` / `poetry 
-00001080: 7275 6e20 636c 6920 3c6d 6f64 756c 6520  run cli <module 
-00001090: 6e61 6d65 3e20 2d2d 6865 6c70 602e 0a0a  name> --help`...
-000010a0: 5468 6520 6669 6775 7265 2062 656c 6f77  The figure below
-000010b0: 2073 686f 7773 2074 6865 2073 7472 7563   shows the struc
-000010c0: 7475 7265 2061 6e64 2077 6f72 6b66 6c6f  ture and workflo
-000010d0: 7720 6f66 2074 6865 2070 6163 6b61 6765  w of the package
-000010e0: 2061 6e64 2069 7473 206d 6f64 756c 6573   and its modules
-000010f0: 2e0a 0a21 5b5d 2864 6f63 732f 6d6f 6475  ...![](docs/modu
-00001100: 6c65 732e 706e 6729 0a0a 2323 2320 526f  les.png)..### Ro
-00001110: 6164 6d61 700a 0a53 6565 2074 6865 205b  admap..See the [
-00001120: 6f70 656e 2069 7373 7565 735d 2868 7474  open issues](htt
-00001130: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001140: 6e68 7378 2f4e 4853 5379 6e74 682f 6973  nhsx/NHSSynth/is
-00001150: 7375 6573 2920 666f 7220 6120 6c69 7374  sues) for a list
-00001160: 206f 6620 7072 6f70 6f73 6564 2066 6561   of proposed fea
-00001170: 7475 7265 7320 2861 6e64 206b 6e6f 776e  tures (and known
-00001180: 2069 7373 7565 7329 2e0a 0a23 2323 2043   issues)...### C
-00001190: 6f6e 7472 6962 7574 696e 670a 0a43 6f6e  ontributing..Con
-000011a0: 7472 6962 7574 696f 6e73 2061 7265 2077  tributions are w
-000011b0: 6861 7420 6d61 6b65 2074 6865 206f 7065  hat make the ope
-000011c0: 6e20 736f 7572 6365 2063 6f6d 6d75 6e69  n source communi
-000011d0: 7479 2073 7563 6820 616e 2061 6d61 7a69  ty such an amazi
-000011e0: 6e67 2070 6c61 6365 2074 6f20 6c65 6172  ng place to lear
-000011f0: 6e2c 2069 6e73 7069 7265 2c20 616e 6420  n, inspire, and 
-00001200: 6372 6561 7465 2e20 416e 7920 636f 6e74  create. Any cont
-00001210: 7269 6275 7469 6f6e 7320 796f 7520 6d61  ributions you ma
-00001220: 6b65 2061 7265 202a 2a67 7265 6174 6c79  ke are **greatly
-00001230: 2061 7070 7265 6369 6174 6564 2a2a 2e0a   appreciated**..
-00001240: 0a31 2e20 466f 726b 2074 6865 2070 726f  .1. Fork the pro
-00001250: 6a65 6374 0a32 2e20 4372 6561 7465 2079  ject.2. Create y
-00001260: 6f75 7220 6272 616e 6368 2028 6067 6974  our branch (`git
-00001270: 2063 6865 636b 6f75 7420 2d62 203c 796f   checkout -b <yo
-00001280: 7572 7573 6572 6e61 6d65 3e2f 3c66 6561  urusername>/<fea
-00001290: 7475 7265 6e61 6d65 3e60 290a 332e 2043  turename>`).3. C
-000012a0: 6f6d 6d69 7420 796f 7572 2063 6861 6e67  ommit your chang
-000012b0: 6573 2028 6067 6974 2063 6f6d 6d69 7420  es (`git commit 
-000012c0: 2d6d 2027 4164 6420 736f 6d65 2061 6d61  -m 'Add some ama
-000012d0: 7a69 6e67 2066 6561 7475 7265 2760 290a  zing feature'`).
-000012e0: 342e 2050 7573 6820 746f 2074 6865 2062  4. Push to the b
-000012f0: 7261 6e63 6820 2860 6769 7420 7075 7368  ranch (`git push
-00001300: 206f 7269 6769 6e20 3c79 6f75 7275 7365   origin <youruse
-00001310: 726e 616d 653e 2f3c 6665 6174 7572 656e  rname>/<featuren
-00001320: 616d 653e 6029 0a35 2e20 4f70 656e 2061  ame>`).5. Open a
-00001330: 2050 5220 616e 6420 7765 2077 696c 6c20   PR and we will 
-00001340: 7472 7920 746f 2067 6574 2069 7420 6d65  try to get it me
-00001350: 7267 6564 210a 0a5f 5365 6520 5b43 4f4e  rged!.._See [CON
-00001360: 5452 4942 5554 494e 472e 6d64 5d28 2e2f  TRIBUTING.md](./
-00001370: 434f 4e54 5249 4255 5449 4e47 2e6d 6429  CONTRIBUTING.md)
-00001380: 2066 6f72 2064 6574 6169 6c65 6420 6775   for detailed gu
-00001390: 6964 616e 6365 2e5f 0a0a 2323 2320 4c69  idance._..### Li
-000013a0: 6365 6e73 650a 0a44 6973 7472 6962 7574  cense..Distribut
-000013b0: 6564 2075 6e64 6572 2074 6865 204d 4954  ed under the MIT
-000013c0: 204c 6963 656e 7365 2e20 5f53 6565 205b   License. _See [
-000013d0: 4c49 4345 4e53 455d 282e 2f4c 4943 454e  LICENSE](./LICEN
-000013e0: 5345 2920 666f 7220 6d6f 7265 2069 6e66  SE) for more inf
-000013f0: 6f72 6d61 7469 6f6e 2e5f 0a0a 2323 2320  ormation._..### 
-00001400: 436f 6e74 6163 740a 0a54 6f20 6669 6e64  Contact..To find
-00001410: 206f 7574 206d 6f72 6520 6162 6f75 7420   out more about 
-00001420: 7468 6520 5b41 6e61 6c79 7469 6373 2055  the [Analytics U
-00001430: 6e69 745d 2868 7474 7073 3a2f 2f77 7777  nit](https://www
-00001440: 2e6e 6873 782e 6e68 732e 756b 2f6b 6579  .nhsx.nhs.uk/key
-00001450: 2d74 6f6f 6c73 2d61 6e64 2d69 6e66 6f2f  -tools-and-info/
-00001460: 6e68 7378 2d61 6e61 6c79 7469 6373 2d75  nhsx-analytics-u
-00001470: 6e69 742f 2920 7669 7369 7420 6f75 7220  nit/) visit our 
-00001480: 5b70 726f 6a65 6374 2077 6562 7369 7465  [project website
-00001490: 5d28 6874 7470 733a 2f2f 6e68 7378 2e67  ](https://nhsx.g
-000014a0: 6974 6875 622e 696f 2f41 6e61 6c79 7469  ithub.io/Analyti
-000014b0: 6373 556e 6974 2f70 726f 6a65 6374 732e  csUnit/projects.
-000014c0: 6874 6d6c 2920 6f72 2067 6574 2069 6e20  html) or get in 
-000014d0: 746f 7563 6820 6174 205b 616e 616c 7974  touch at [analyt
-000014e0: 6963 732d 756e 6974 406e 6873 782e 6e68  ics-unit@nhsx.nh
-000014f0: 732e 756b 5d28 6d61 696c 746f 3a61 6e61  s.uk](mailto:ana
-00001500: 6c79 7469 6373 2d75 6e69 7440 6e68 7378  lytics-unit@nhsx
-00001510: 2e6e 6873 2e75 6b29 2e0a 0a3c 212d 2d20  .nhs.uk)...<!-- 
-00001520: 2323 2320 4163 6b6e 6f77 6c65 6467 656d  ### Acknowledgem
-00001530: 656e 7473 202d 2d3e 0a                   ents -->.
+00000000: 3c21 2d2d 2050 524f 4a45 4354 2053 4849  <!-- PROJECT SHI
+00000010: 454c 4453 202d 2d3e 0a3c 6469 7620 616c  ELDS -->.<div al
+00000020: 6967 6e3d 2263 656e 7465 7222 3e0a 0a5b  ign="center">..[
+00000030: 215b 5079 5049 202d 204c 6174 6573 7420  ![PyPI - Latest 
+00000040: 5265 6c65 6173 655d 2868 7474 7073 3a2f  Release](https:/
+00000050: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000060: 7079 7069 2f76 2f6e 6873 7379 6e74 683f  pypi/v/nhssynth?
+00000070: 7374 796c 653d 666c 6174 2d73 7175 6172  style=flat-squar
+00000080: 6529 5d28 6874 7470 733a 2f2f 7079 7069  e)](https://pypi
+00000090: 2e6f 7267 2f70 726f 6a65 6374 2f6e 6873  .org/project/nhs
+000000a0: 7379 6e74 682f 290a 5b21 5b50 7950 4920  synth/).[![PyPI 
+000000b0: 2d20 5768 6565 6c5d 2868 7474 7073 3a2f  - Wheel](https:/
+000000c0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+000000d0: 7079 7069 2f77 6865 656c 2f6e 6873 7379  pypi/wheel/nhssy
+000000e0: 6e74 683f 7374 796c 653d 666c 6174 2d73  nth?style=flat-s
+000000f0: 7175 6172 6529 5d28 6874 7470 733a 2f2f  quare)](https://
+00000100: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+00000110: 2f6e 6873 7379 6e74 682f 290a 5b21 5b50  /nhssynth/).[![P
+00000120: 7950 4920 2d20 5061 636b 6167 6520 5374  yPI - Package St
+00000130: 6174 7573 5d28 6874 7470 733a 2f2f 696d  atus](https://im
+00000140: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+00000150: 692f 7374 6174 7573 2f6e 6873 7379 6e74  i/status/nhssynt
+00000160: 683f 7374 796c 653d 666c 6174 2d73 7175  h?style=flat-squ
+00000170: 6172 6529 5d28 6874 7470 733a 2f2f 7079  are)](https://py
+00000180: 7069 2e6f 7267 2f70 726f 6a65 6374 2f6e  pi.org/project/n
+00000190: 6873 7379 6e74 682f 290a 5b21 5b50 7950  hssynth/).[![PyP
+000001a0: 4920 2d20 5079 7468 6f6e 2056 6572 7369  I - Python Versi
+000001b0: 6f6e 5d28 6874 7470 733a 2f2f 696d 672e  on](https://img.
+000001c0: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+000001d0: 7079 7665 7273 696f 6e73 2f6e 6873 7379  pyversions/nhssy
+000001e0: 6e74 683f 7374 796c 653d 666c 6174 2d73  nth?style=flat-s
+000001f0: 7175 6172 6529 5d28 6874 7470 733a 2f2f  quare)](https://
+00000200: 7777 772e 7079 7468 6f6e 2e6f 7267 2f64  www.python.org/d
+00000210: 6f77 6e6c 6f61 6473 2f72 656c 6561 7365  ownloads/release
+00000220: 2f70 7974 686f 6e2d 3331 3030 2f29 0a5b  /python-3100/).[
+00000230: 215b 5079 5049 202d 204c 6963 656e 7365  ![PyPI - License
+00000240: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000250: 6965 6c64 732e 696f 2f70 7970 692f 6c2f  ields.io/pypi/l/
+00000260: 6e68 7373 796e 7468 3f73 7479 6c65 3d66  nhssynth?style=f
+00000270: 6c61 742d 7371 7561 7265 295d 2868 7474  lat-square)](htt
+00000280: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000290: 6e68 7378 2f6e 6873 7379 6e74 682f 626c  nhsx/nhssynth/bl
+000002a0: 6f62 2f6d 6169 6e2f 4c49 4345 4e53 4529  ob/main/LICENSE)
+000002b0: 0a5b 215b 436f 6465 2073 7479 6c65 3a20  .[![Code style: 
+000002c0: 626c 6163 6b5d 2868 7474 7073 3a2f 2f69  black](https://i
+000002d0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
+000002e0: 6467 652f 636f 6465 2532 3073 7479 6c65  dge/code%20style
+000002f0: 2d62 6c61 636b 2d30 3030 3030 303f 7374  -black-000000?st
+00000300: 796c 653d 666c 6174 2d73 7175 6172 6529  yle=flat-square)
+00000310: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000320: 2e63 6f6d 2f70 7366 2f62 6c61 636b 290a  .com/psf/black).
+00000330: 5b21 5b49 6d70 6f72 7473 3a20 6973 6f72  [![Imports: isor
+00000340: 745d 2868 7474 7073 3a2f 2f69 6d67 2e73  t](https://img.s
+00000350: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+00000360: 2532 3069 6d70 6f72 7473 2d69 736f 7274  %20imports-isort
+00000370: 2d25 3233 3136 3734 6231 3f73 7479 6c65  -%231674b1?style
+00000380: 3d66 6c61 742d 7371 7561 7265 295d 2868  =flat-square)](h
+00000390: 7474 7073 3a2f 2f70 7963 7161 2e67 6974  ttps://pycqa.git
+000003a0: 6875 622e 696f 2f69 736f 7274 2f29 0a0a  hub.io/isort/)..
+000003b0: 3c2f 6469 763e 0a0a 0a3c 212d 2d20 5052  </div>...<!-- PR
+000003c0: 4f4a 4543 5420 4c4f 474f 202d 2d3e 0a3c  OJECT LOGO -->.<
+000003d0: 6469 7620 616c 6967 6e3d 2263 656e 7465  div align="cente
+000003e0: 7222 3e0a 2020 3c61 2068 7265 663d 2268  r">.  <a href="h
+000003f0: 7474 7073 3a2f 2f6e 6873 782e 6769 7468  ttps://nhsx.gith
+00000400: 7562 2e69 6f2f 4e48 5353 796e 7468 223e  ub.io/NHSSynth">
+00000410: 0a20 2020 203c 696d 6720 7372 633d 2264  .    <img src="d
+00000420: 6f63 732f 6173 7365 7473 2f4e 4853 2e73  ocs/assets/NHS.s
+00000430: 7667 2220 616c 743d 224c 6f67 6f22 2077  vg" alt="Logo" w
+00000440: 6964 7468 3d22 3230 3022 2068 6569 6768  idth="200" heigh
+00000450: 743d 2231 3030 223e 0a20 203c 2f61 3e0a  t="100">.  </a>.
+00000460: 2020 3c70 2061 6c69 676e 3d22 6365 6e74    <p align="cent
+00000470: 6572 223e 0a20 2020 203c 6120 6872 6566  er">.    <a href
+00000480: 3d22 6874 7470 733a 2f2f 6e68 7378 2e67  ="https://nhsx.g
+00000490: 6974 6875 622e 696f 2f4e 4853 5379 6e74  ithub.io/NHSSynt
+000004a0: 6822 3e3c 7374 726f 6e67 3e45 7870 6c6f  h"><strong>Explo
+000004b0: 7265 2074 6865 2064 6f63 7320 c2bb 3c2f  re the docs ..</
+000004c0: 7374 726f 6e67 3e3c 2f61 3e0a 2020 2020  strong></a>.    
+000004d0: 3c62 7220 2f3e 0a20 2020 203c 6272 202f  <br />.    <br /
+000004e0: 3e0a 2020 3c2f 703e 0a3c 2f64 6976 3e0a  >.  </p>.</div>.
+000004f0: 0a23 204e 4853 2053 796e 7468 0a0a 2323  .# NHS Synth..##
+00000500: 2041 626f 7574 2074 6865 2050 726f 6a65   About the Proje
+00000510: 6374 0a0a 5468 6520 7072 6f6a 6563 7420  ct..The project 
+00000520: 6375 7272 656e 746c 7920 636f 6e73 6973  currently consis
+00000530: 7473 206f 6620 6120 5079 7468 6f6e 2070  ts of a Python p
+00000540: 6163 6b61 6765 2061 6c6f 6e67 7369 6465  ackage alongside
+00000550: 2072 6573 6561 7263 6820 616e 6420 696e   research and in
+00000560: 7665 7374 6967 6174 6976 6520 6d61 7465  vestigative mate
+00000570: 7269 616c 7320 636f 7665 7269 6e67 2074  rials covering t
+00000580: 6865 2065 6666 6563 7469 7665 6e65 7373  he effectiveness
+00000590: 206f 6620 7468 6520 7061 636b 6167 6520   of the package 
+000005a0: 616e 6420 7379 6e74 6865 7469 6320 6461  and synthetic da
+000005b0: 7461 206d 6f72 6520 6765 6e65 7261 6c6c  ta more generall
+000005c0: 7920 7768 656e 2061 7070 6c69 6564 2074  y when applied t
+000005d0: 6f20 4e48 5320 7573 6520 6361 7365 732e  o NHS use cases.
+000005e0: 0a0a 5b50 726f 6a65 6374 2044 6573 6372  ..[Project Descr
+000005f0: 6970 7469 6f6e 202d 2053 796e 7468 6574  iption - Synthet
+00000600: 6963 2044 6174 6120 4578 706c 6f72 6174  ic Data Explorat
+00000610: 696f 6e3a 2056 6172 6961 7469 6f6e 616c  ion: Variational
+00000620: 2041 7574 6f65 6e63 6f64 6572 735d 2868   Autoencoders](h
+00000630: 7474 7073 3a2f 2f6e 6873 782e 6769 7468  ttps://nhsx.gith
+00000640: 7562 2e69 6f2f 6e68 7378 2d69 6e74 6572  ub.io/nhsx-inter
+00000650: 6e73 6869 702d 7072 6f6a 6563 7473 2f73  nship-projects/s
+00000660: 796e 7468 6574 6963 2d64 6174 612d 6578  ynthetic-data-ex
+00000670: 706c 6f72 6174 696f 6e2d 7661 652f 290a  ploration-vae/).
+00000680: 0a54 6865 2063 6f64 6562 6173 6520 6275  .The codebase bu
+00000690: 696c 6473 206f 6e20 7072 6576 696f 7573  ilds on previous
+000006a0: 204e 4853 5820 416e 616c 7974 6963 7320   NHSX Analytics 
+000006b0: 556e 6974 2050 6844 2069 6e74 6572 6e73  Unit PhD interns
+000006c0: 6869 7073 2063 6f6e 7465 7874 7561 6c69  hips contextuali
+000006d0: 7369 6e67 2061 6e64 2069 6e76 6573 7469  sing and investi
+000006e0: 6761 7469 6e67 2074 6865 2070 6f74 656e  gating the poten
+000006f0: 7469 616c 2075 7365 206f 6620 5661 7269  tial use of Vari
+00000700: 6174 696f 6e61 6c20 4175 746f 2045 6e63  ational Auto Enc
+00000710: 6f64 6572 7320 2856 4145 7329 2066 6f72  oders (VAEs) for
+00000720: 2073 796e 7468 6574 6963 2064 6174 6120   synthetic data 
+00000730: 6765 6e65 7261 7469 6f6e 2e20 5468 6573  generation. Thes
+00000740: 6520 7765 7265 2075 6e64 6572 7461 6b65  e were undertake
+00000750: 6e20 6279 2044 6f6d 696e 6963 2044 616e  n by Dominic Dan
+00000760: 6b73 2061 6e64 2044 6176 6964 2042 7269  ks and David Bri
+00000770: 6e64 2e0a 0a5f 2a2a 4e6f 7465 3a2a 2a20  nd..._**Note:** 
+00000780: 4e6f 2064 6174 612c 2070 7562 6c69 6320  No data, public 
+00000790: 6f72 2070 7269 7661 7465 2061 7265 2073  or private are s
+000007a0: 6861 7265 6420 696e 2074 6869 7320 7265  hared in this re
+000007b0: 706f 7369 746f 7279 2e5f 0a0a 2323 2047  pository._..## G
+000007c0: 6574 7469 6e67 2053 7461 7274 6564 0a0a  etting Started..
+000007d0: 2323 2320 5072 6f6a 6563 7420 5374 7275  ### Project Stru
+000007e0: 6374 7572 650a 0a2d 2054 6865 206d 6169  cture..- The mai
+000007f0: 6e20 7061 636b 6167 6520 616e 6420 636f  n package and co
+00000800: 6465 6261 7365 2069 7320 666f 756e 6420  debase is found 
+00000810: 696e 2060 7372 632f 6e68 7373 796e 7468  in `src/nhssynth
+00000820: 6020 2873 6565 2055 7361 6765 2062 656c  ` (see Usage bel
+00000830: 6f77 2066 6f72 206d 6f72 6520 696e 666f  ow for more info
+00000840: 726d 6174 696f 6e29 0a2d 2041 6363 6f6d  rmation).- Accom
+00000850: 7061 6e79 696e 6720 6d61 7465 7269 616c  panying material
+00000860: 7320 6172 6520 6176 6169 6c61 626c 6520  s are available 
+00000870: 696e 2074 6865 2060 646f 6373 6020 666f  in the `docs` fo
+00000880: 6c64 6572 3a0a 2020 2d20 4120 5b72 6570  lder:.  - A [rep
+00000890: 6f72 745d 2872 6570 6f72 7473 2f72 6570  ort](reports/rep
+000008a0: 6f72 742e 7064 6629 2073 756d 6d61 7269  ort.pdf) summari
+000008b0: 7369 6e67 2074 6865 2070 7265 7669 6f75  sing the previou
+000008c0: 7320 6974 6572 6174 696f 6e20 6f66 2074  s iteration of t
+000008d0: 6869 7320 7072 6f6a 6563 740a 2020 2d20  his project.  - 
+000008e0: 4120 5b6d 6f64 656c 2063 6172 645d 286d  A [model card](m
+000008f0: 6f64 656c 5f63 6172 642e 6d64 2920 7072  odel_card.md) pr
+00000900: 6f76 6964 696e 6720 6d6f 7265 2069 6e66  oviding more inf
+00000910: 6f72 6d61 7469 6f6e 2061 626f 7574 2074  ormation about t
+00000920: 6865 2056 4145 2077 6974 6820 4469 6666  he VAE with Diff
+00000930: 6572 656e 7469 616c 2050 7269 7661 6379  erential Privacy
+00000940: 0a2d 204e 756d 6572 6f75 7320 5b65 7865  .- Numerous [exe
+00000950: 6d70 6c61 7220 636f 6e66 6967 7572 6174  mplar configurat
+00000960: 696f 6e73 5d28 2e2e 2f63 6f6e 6669 6729  ions](../config)
+00000970: 2061 7265 2066 6f75 6e64 2069 6e20 6063   are found in `c
+00000980: 6f6e 6669 6760 0a2d 2045 6d70 7479 2060  onfig`.- Empty `
+00000990: 6461 7461 6020 616e 6420 6065 7870 6572  data` and `exper
+000009a0: 696d 656e 7473 6020 666f 6c64 6572 7320  iments` folders 
+000009b0: 6172 6520 7072 6f76 6964 6564 3b20 7468  are provided; th
+000009c0: 6573 6520 6172 6520 7468 6520 6465 6661  ese are the defa
+000009d0: 756c 7420 6c6f 6361 7469 6f6e 7320 666f  ult locations fo
+000009e0: 7220 696e 7075 7473 2061 6e64 206f 7574  r inputs and out
+000009f0: 7075 7473 2077 6865 6e20 7275 6e6e 696e  puts when runnin
+00000a00: 6720 7468 6520 7072 6f6a 6563 7420 7573  g the project us
+00000a10: 696e 6720 7468 6520 7072 6f76 6964 6564  ing the provided
+00000a20: 205b 6063 6c69 605d 282e 2e2f 7372 632f   [`cli`](../src/
+00000a30: 6e68 7373 796e 7468 2f63 6c69 2f29 206d  nhssynth/cli/) m
+00000a40: 6f64 756c 650a 2d20 5072 652d 7072 6f63  odule.- Pre-proc
+00000a50: 6573 7369 6e67 206e 6f74 6562 6f6f 6b73  essing notebooks
+00000a60: 2066 6f72 2073 7065 6369 6669 6320 6461   for specific da
+00000a70: 7461 7365 7473 2075 7365 6420 746f 2061  tasets used to a
+00000a80: 7373 6573 7320 7468 6520 6170 7072 6f61  ssess the approa
+00000a90: 6368 2061 6e64 206f 7468 6572 206e 6f6e  ch and other non
+00000aa0: 2d63 6f72 6520 636f 6465 2063 616e 2062  -core code can b
+00000ab0: 6520 666f 756e 6420 696e 205b 6061 7578  e found in [`aux
+00000ac0: 696c 6961 7279 605d 282e 2e2f 6175 7869  iliary`](../auxi
+00000ad0: 6c69 6172 792f 290a 0a23 2323 2049 6e73  liary/)..### Ins
+00000ae0: 7461 6c6c 6174 696f 6e0a 0a41 7320 6974  tallation..As it
+00000af0: 2073 7461 6e64 732c 2077 6520 7265 636f   stands, we reco
+00000b00: 6d6d 656e 6420 7468 6520 666f 6c6c 6f77  mmend the follow
+00000b10: 696e 6720 7374 6570 7320 746f 2072 6570  ing steps to rep
+00000b20: 726f 6475 6365 206f 7572 2065 7870 6572  roduce our exper
+00000b30: 696d 656e 7473 2061 6e64 2066 756c 6c79  iments and fully
+00000b40: 2077 6f72 6b20 7769 7468 2074 6869 7320   work with this 
+00000b50: 7072 6f6a 6563 743a 0a0a 312e 2043 6c6f  project:..1. Clo
+00000b60: 6e65 2074 6865 2072 6570 6f0a 322e 2045  ne the repo.2. E
+00000b70: 6e73 7572 6520 6f6e 6520 6f66 2074 6865  nsure one of the
+00000b80: 2072 6571 7569 7265 6420 7665 7273 696f   required versio
+00000b90: 6e73 206f 6620 5079 7468 6f6e 2069 7320  ns of Python is 
+00000ba0: 696e 7374 616c 6c65 640a 332e 2049 6e73  installed.3. Ins
+00000bb0: 7461 6c6c 205b 6070 6f65 7472 7960 5d28  tall [`poetry`](
+00000bc0: 6874 7470 733a 2f2f 7079 7468 6f6e 2d70  https://python-p
+00000bd0: 6f65 7472 792e 6f72 672f 646f 6373 2f23  oetry.org/docs/#
+00000be0: 696e 7374 616c 6c61 7469 6f6e 290a 342e  installation).4.
+00000bf0: 2049 6e73 7461 6e74 6961 7465 2061 2076   Instantiate a v
+00000c00: 6972 7475 616c 2065 6e76 6972 6f6e 6d65  irtual environme
+00000c10: 6e74 2c20 652e 672e 2076 6961 2060 7079  nt, e.g. via `py
+00000c20: 7468 6f6e 202d 6d20 7665 6e76 206e 6873  thon -m venv nhs
+00000c30: 7379 6e74 6860 0a33 2e20 4163 7469 7661  synth`.3. Activa
+00000c40: 7465 2074 6865 2076 6972 7475 616c 2065  te the virtual e
+00000c50: 6e76 6972 6f6e 6d65 6e74 2c20 652e 672e  nvironment, e.g.
+00000c60: 2076 6961 2060 736f 7572 6365 206e 6873   via `source nhs
+00000c70: 7379 6e74 682f 6269 6e2f 6163 7469 7661  synth/bin/activa
+00000c80: 7465 600a 342e 2049 6e73 7461 6c6c 2070  te`.4. Install p
+00000c90: 726f 6a65 6374 2064 6570 656e 6465 6e63  roject dependenc
+00000ca0: 6965 7320 7769 7468 2060 706f 6574 7279  ies with `poetry
+00000cb0: 2069 6e73 7461 6c6c 6020 286f 7074 696f   install` (optio
+00000cc0: 6e61 6c6c 7920 696e 7374 616c 6c20 606a  nally install `j
+00000cd0: 7570 7974 6572 6020 616e 6420 606e 6f74  upyter` and `not
+00000ce0: 6562 6f6f 6b60 2074 6f20 776f 726b 2077  ebook` to work w
+00000cf0: 6974 6820 736f 6d65 206f 6620 7468 6520  ith some of the 
+00000d00: 7072 6570 726f 6365 7373 696e 6720 6669  preprocessing fi
+00000d10: 6c65 7320 696e 205b 6061 7578 696c 6961  les in [`auxilia
+00000d20: 7279 605d 2861 7578 696c 6961 7279 2f29  ry`](auxiliary/)
+00000d30: 290a 352e 2049 6e74 6572 6163 7420 7769  ).5. Interact wi
+00000d40: 7468 2074 6865 2070 6163 6b61 6765 2069  th the package i
+00000d50: 6e20 6f6e 6520 6f66 2074 776f 2077 6179  n one of two way
+00000d60: 733a 0a20 2020 202d 2056 6961 2074 6865  s:.    - Via the
+00000d70: 205b 6063 6c69 605d 2873 7263 2f6e 6873   [`cli`](src/nhs
+00000d80: 7379 6e74 682f 636c 692f 2920 6d6f 6475  synth/cli/) modu
+00000d90: 6c65 2075 7369 6e67 2060 706f 6574 7279  le using `poetry
+00000da0: 2072 756e 2063 6c69 600a 2020 2020 2d20   run cli`.    - 
+00000db0: 5468 726f 7567 6820 6275 696c 6469 6e67  Through building
+00000dc0: 2074 6865 2070 6163 6b61 6765 2077 6974   the package wit
+00000dd0: 6820 6070 6f65 7472 7920 6275 696c 6460  h `poetry build`
+00000de0: 2061 6e64 2075 7369 6e67 2069 7420 696e   and using it in
+00000df0: 2061 6e20 6578 6973 7469 6e67 2070 726f   an existing pro
+00000e00: 6a65 6374 2028 6069 6d70 6f72 7420 6e68  ject (`import nh
+00000e10: 7373 796e 7468 6029 2e20 486f 7765 7665  ssynth`). Howeve
+00000e20: 722c 2069 6620 796f 7520 696e 7465 6e64  r, if you intend
+00000e30: 206f 6e20 646f 696e 6720 7468 6520 6c61   on doing the la
+00000e40: 7474 6572 2069 7420 6d61 7920 6265 2070  tter it may be p
+00000e50: 7265 6665 7261 626c 6520 746f 2069 6e73  referable to ins
+00000e60: 7465 6164 2066 6f6c 6c6f 7720 7468 6520  tead follow the 
+00000e70: 7365 636f 6e64 2c20 7369 6d70 6c65 7220  second, simpler 
+00000e80: 7365 7475 7020 6265 6c6f 772e 0a0a 466f  setup below...Fo
+00000e90: 7220 6d6f 7265 2073 7461 6e64 6172 6420  r more standard 
+00000ea0: 7573 6167 6520 6f66 2074 6865 2070 6163  usage of the pac
+00000eb0: 6b61 6765 3a0a 0a31 2e20 5275 6e20 6070  kage:..1. Run `p
+00000ec0: 6970 2069 6e73 7461 6c6c 206e 6873 7379  ip install nhssy
+00000ed0: 6e74 6860 2077 6974 6869 6e20 6120 7375  nth` within a su
+00000ee0: 7070 6f72 7465 6420 5079 7468 6f6e 2069  pported Python i
+00000ef0: 6e73 7461 6c6c 6174 696f 6e0a 322e 2055  nstallation.2. U
+00000f00: 7365 2074 6865 206d 6f64 756c 6573 2065  se the modules e
+00000f10: 7870 6f72 7465 6420 6279 2074 6865 2070  xported by the p
+00000f20: 6163 6b61 6765 2061 7320 796f 7520 776f  ackage as you wo
+00000f30: 756c 6420 616e 7920 6f74 6865 722e 205f  uld any other. _
+00000f40: 4e6f 7465 2074 6861 7420 696e 2074 6869  Note that in thi
+00000f50: 7320 7365 7475 7020 796f 7520 7769 6c6c  s setup you will
+00000f60: 2068 6176 6520 746f 2077 6f72 6b20 6d6f   have to work mo
+00000f70: 7265 2063 6c6f 7365 6c79 2077 6974 6820  re closely with 
+00000f80: 7468 6520 636f 6e66 6967 7572 6174 696f  the configuratio
+00000f90: 6e20 616e 6420 636f 6465 2074 6f20 656e  n and code to en
+00000fa0: 7375 7265 2079 6f75 2061 7265 2068 616e  sure you are han
+00000fb0: 646c 696e 6720 696e 7075 7473 2061 6e64  dling inputs and
+00000fc0: 206f 7574 7075 7473 2066 6f72 2065 6163   outputs for eac
+00000fd0: 6820 6d6f 6475 6c65 2061 7070 726f 7072  h module appropr
+00000fe0: 6961 7465 6c79 2e20 5468 6520 636c 6920  iately. The cli 
+00000ff0: 6861 6e64 6c65 7320 6120 6c6f 7420 6f66  handles a lot of
+00001000: 2074 6869 7320 636f 6d70 6c65 7869 7479   this complexity
+00001010: 2c20 616e 6420 696e 7465 7261 6374 696e  , and interactin
+00001020: 6720 7769 7468 2074 6865 206d 6f64 756c  g with the modul
+00001030: 6573 2064 6972 6563 746c 7920 6973 2063  es directly is c
+00001040: 6f6e 7369 6465 7265 6420 6164 7661 6e63  onsidered advanc
+00001050: 6564 2075 7361 6765 2e5f 0a0a 2323 2320  ed usage._..### 
+00001060: 5573 6167 650a 0a54 6869 7320 7061 636b  Usage..This pack
+00001070: 6167 6520 636f 6d70 7269 7365 7320 6120  age comprises a 
+00001080: 7069 7065 6c69 6e65 2074 6861 7420 6973  pipeline that is
+00001090: 2072 756e 6e61 626c 6520 7669 6120 6070   runnable via `p
+000010a0: 6f65 7472 7920 7275 6e20 636c 6920 7069  oetry run cli pi
+000010b0: 7065 6c69 6e65 203c 6172 6773 3e60 206f  peline <args>` o
+000010c0: 7220 6070 6f65 7472 7920 7275 6e20 636c  r `poetry run cl
+000010d0: 6920 636f 6e66 6967 203c 636f 6e66 6967  i config <config
+000010e0: 2066 696c 6570 6174 683e 602e 2059 6f75   filepath>`. You
+000010f0: 2063 616e 2072 756e 2074 6865 206d 6f64   can run the mod
+00001100: 756c 6573 2074 6861 7420 6d61 6b65 2075  ules that make u
+00001110: 7020 7468 6973 2070 6970 656c 696e 6520  p this pipeline 
+00001120: 696e 6465 7065 6e64 656e 746c 7920 7669  independently vi
+00001130: 6120 6070 6f65 7472 7920 7275 6e20 636c  a `poetry run cl
+00001140: 6920 3c6d 6f64 756c 6520 6e61 6d65 3e60  i <module name>`
+00001150: 2e20 546f 2073 6565 2074 6865 206d 6f64  . To see the mod
+00001160: 756c 6573 2074 6861 7420 6172 6520 6176  ules that are av
+00001170: 6169 6c61 626c 6520 616e 6420 7468 6569  ailable and thei
+00001180: 7220 636f 7272 6573 706f 6e64 696e 6720  r corresponding 
+00001190: 6172 6775 6d65 6e74 7320 616e 6420 6675  arguments and fu
+000011a0: 6e63 7469 6f6e 2c20 7275 6e20 6070 6f65  nction, run `poe
+000011b0: 7472 7920 7275 6e20 636c 6920 2d2d 6865  try run cli --he
+000011c0: 6c70 6020 2f20 6070 6f65 7472 7920 7275  lp` / `poetry ru
+000011d0: 6e20 636c 6920 3c6d 6f64 756c 6520 6e61  n cli <module na
+000011e0: 6d65 3e20 2d2d 6865 6c70 602e 0a0a 5468  me> --help`...Th
+000011f0: 6520 6669 6775 7265 2062 656c 6f77 2073  e figure below s
+00001200: 686f 7773 2074 6865 2073 7472 7563 7475  hows the structu
+00001210: 7265 2061 6e64 2077 6f72 6b66 6c6f 7720  re and workflow 
+00001220: 6f66 2074 6865 2070 6163 6b61 6765 2061  of the package a
+00001230: 6e64 2069 7473 206d 6f64 756c 6573 2e0a  nd its modules..
+00001240: 0a21 5b5d 2864 6f63 732f 6d6f 6475 6c65  .![](docs/module
+00001250: 732e 706e 6729 0a0a 2323 2320 526f 6164  s.png)..### Road
+00001260: 6d61 700a 0a53 6565 2074 6865 205b 6f70  map..See the [op
+00001270: 656e 2069 7373 7565 735d 2868 7474 7073  en issues](https
+00001280: 3a2f 2f67 6974 6875 622e 636f 6d2f 6e68  ://github.com/nh
+00001290: 7378 2f4e 4853 5379 6e74 682f 6973 7375  sx/NHSSynth/issu
+000012a0: 6573 2920 666f 7220 6120 6c69 7374 206f  es) for a list o
+000012b0: 6620 7072 6f70 6f73 6564 2066 6561 7475  f proposed featu
+000012c0: 7265 7320 2861 6e64 206b 6e6f 776e 2069  res (and known i
+000012d0: 7373 7565 7329 2e0a 0a23 2323 2043 6f6e  ssues)...### Con
+000012e0: 7472 6962 7574 696e 670a 0a43 6f6e 7472  tributing..Contr
+000012f0: 6962 7574 696f 6e73 2061 7265 2077 6861  ibutions are wha
+00001300: 7420 6d61 6b65 2074 6865 206f 7065 6e20  t make the open 
+00001310: 736f 7572 6365 2063 6f6d 6d75 6e69 7479  source community
+00001320: 2073 7563 6820 616e 2061 6d61 7a69 6e67   such an amazing
+00001330: 2070 6c61 6365 2074 6f20 6c65 6172 6e2c   place to learn,
+00001340: 2069 6e73 7069 7265 2c20 616e 6420 6372   inspire, and cr
+00001350: 6561 7465 2e20 416e 7920 636f 6e74 7269  eate. Any contri
+00001360: 6275 7469 6f6e 7320 796f 7520 6d61 6b65  butions you make
+00001370: 2061 7265 202a 2a67 7265 6174 6c79 2061   are **greatly a
+00001380: 7070 7265 6369 6174 6564 2a2a 2e0a 0a31  ppreciated**...1
+00001390: 2e20 466f 726b 2074 6865 2070 726f 6a65  . Fork the proje
+000013a0: 6374 0a32 2e20 4372 6561 7465 2079 6f75  ct.2. Create you
+000013b0: 7220 6272 616e 6368 2028 6067 6974 2063  r branch (`git c
+000013c0: 6865 636b 6f75 7420 2d62 203c 796f 7572  heckout -b <your
+000013d0: 7573 6572 6e61 6d65 3e2f 3c66 6561 7475  username>/<featu
+000013e0: 7265 6e61 6d65 3e60 290a 332e 2043 6f6d  rename>`).3. Com
+000013f0: 6d69 7420 796f 7572 2063 6861 6e67 6573  mit your changes
+00001400: 2028 6067 6974 2063 6f6d 6d69 7420 2d6d   (`git commit -m
+00001410: 2027 4164 6420 736f 6d65 2061 6d61 7a69   'Add some amazi
+00001420: 6e67 2066 6561 7475 7265 2760 290a 342e  ng feature'`).4.
+00001430: 2050 7573 6820 746f 2074 6865 2062 7261   Push to the bra
+00001440: 6e63 6820 2860 6769 7420 7075 7368 206f  nch (`git push o
+00001450: 7269 6769 6e20 3c79 6f75 7275 7365 726e  rigin <yourusern
+00001460: 616d 653e 2f3c 6665 6174 7572 656e 616d  ame>/<featurenam
+00001470: 653e 6029 0a35 2e20 4f70 656e 2061 2050  e>`).5. Open a P
+00001480: 5220 616e 6420 7765 2077 696c 6c20 7472  R and we will tr
+00001490: 7920 746f 2067 6574 2069 7420 6d65 7267  y to get it merg
+000014a0: 6564 210a 0a5f 5365 6520 5b43 4f4e 5452  ed!.._See [CONTR
+000014b0: 4942 5554 494e 472e 6d64 5d28 2e2f 434f  IBUTING.md](./CO
+000014c0: 4e54 5249 4255 5449 4e47 2e6d 6429 2066  NTRIBUTING.md) f
+000014d0: 6f72 2064 6574 6169 6c65 6420 6775 6964  or detailed guid
+000014e0: 616e 6365 2e5f 0a0a 5468 616e 6b73 2074  ance._..Thanks t
+000014f0: 6f20 6576 6572 796f 6e65 2074 6861 7420  o everyone that 
+00001500: 6861 7320 636f 6e74 7269 6275 7465 6420  has contributed 
+00001510: 736f 2066 6172 210a 0a3c 6469 7620 616c  so far!..<div al
+00001520: 6967 6e3d 2263 656e 7465 7222 3e0a 3c61  ign="center">.<a
+00001530: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+00001540: 6974 6875 622e 636f 6d2f 6e68 7378 2f6e  ithub.com/nhsx/n
+00001550: 6873 7379 6e74 682f 6772 6170 6873 2f63  hssynth/graphs/c
+00001560: 6f6e 7472 6962 7574 6f72 7322 3e0a 2020  ontributors">.  
+00001570: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00001580: 2f2f 636f 6e74 7269 622e 726f 636b 732f  //contrib.rocks/
+00001590: 696d 6167 653f 7265 706f 3d6e 6873 782f  image?repo=nhsx/
+000015a0: 6e68 7373 796e 7468 2220 2f3e 0a3c 2f61  nhssynth" />.</a
+000015b0: 3e0a 3c2f 6469 763e 0a0a 2323 2320 4c69  >.</div>..### Li
+000015c0: 6365 6e73 650a 0a44 6973 7472 6962 7574  cense..Distribut
+000015d0: 6564 2075 6e64 6572 2074 6865 204d 4954  ed under the MIT
+000015e0: 204c 6963 656e 7365 2e20 5f53 6565 205b   License. _See [
+000015f0: 4c49 4345 4e53 455d 282e 2f4c 4943 454e  LICENSE](./LICEN
+00001600: 5345 2920 666f 7220 6d6f 7265 2069 6e66  SE) for more inf
+00001610: 6f72 6d61 7469 6f6e 2e5f 0a0a 2323 2320  ormation._..### 
+00001620: 436f 6e74 6163 740a 0a54 6869 7320 7072  Contact..This pr
+00001630: 6f6a 6563 7420 6973 2075 6e64 6572 2061  oject is under a
+00001640: 6374 6976 6520 6465 7665 6c6f 706d 656e  ctive developmen
+00001650: 7420 6279 205b 4048 6172 7269 736f 6e57  t by [@HarrisonW
+00001660: 696c 6465 5d28 6874 7470 733a 2f2f 6769  ilde](https://gi
+00001670: 7468 7562 2e63 6f6d 2f48 6172 7269 736f  thub.com/Harriso
+00001680: 6e57 696c 6465 292c 2066 6f72 2061 6e79  nWilde), for any
+00001690: 2071 7565 7374 696f 6e73 206f 7220 7365   questions or se
+000016a0: 6375 7269 7479 2063 6f6e 6365 726e 7320  curity concerns 
+000016b0: 5b63 6f6e 7461 6374 2068 696d 5d28 6d61  [contact him](ma
+000016c0: 696c 746f 3a68 2e77 696c 6465 4077 6172  ilto:h.wilde@war
+000016d0: 7769 636b 2e61 632e 756b 2920 6f72 205b  wick.ac.uk) or [
+000016e0: 7261 6973 6520 616e 2069 7373 7565 5d28  raise an issue](
+000016f0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001700: 6f6d 2f6e 6873 782f 4e48 5353 796e 7468  om/nhsx/NHSSynth
+00001710: 2f69 7373 7565 732f 6e65 772f 6368 6f6f  /issues/new/choo
+00001720: 7365 292e 2041 6c74 6572 6e61 7469 7665  se). Alternative
+00001730: 6c79 2c20 636f 6e74 6163 7420 5b4e 4853  ly, contact [NHS
+00001740: 2045 6e67 6c61 6e64 2054 4441 555d 286d   England TDAU](m
+00001750: 6169 6c74 6f3a 656e 676c 616e 642e 7464  ailto:england.td
+00001760: 6175 406e 6873 2e6e 6574 292e 0a0a 546f  au@nhs.net)...To
+00001770: 2066 696e 6420 6f75 7420 6d6f 7265 2061   find out more a
+00001780: 626f 7574 2074 6865 205b 416e 616c 7974  bout the [Analyt
+00001790: 6963 7320 556e 6974 5d28 6874 7470 733a  ics Unit](https:
+000017a0: 2f2f 7777 772e 6e68 7378 2e6e 6873 2e75  //www.nhsx.nhs.u
+000017b0: 6b2f 6b65 792d 746f 6f6c 732d 616e 642d  k/key-tools-and-
+000017c0: 696e 666f 2f6e 6873 782d 616e 616c 7974  info/nhsx-analyt
+000017d0: 6963 732d 756e 6974 2f29 2076 6973 6974  ics-unit/) visit
+000017e0: 206f 7572 205b 7072 6f6a 6563 7420 7765   our [project we
+000017f0: 6273 6974 655d 2868 7474 7073 3a2f 2f6e  bsite](https://n
+00001800: 6873 782e 6769 7468 7562 2e69 6f2f 416e  hsx.github.io/An
+00001810: 616c 7974 6963 7355 6e69 742f 7072 6f6a  alyticsUnit/proj
+00001820: 6563 7473 2e68 746d 6c29 206f 7220 6765  ects.html) or ge
+00001830: 7420 696e 2074 6f75 6368 2061 7420 5b65  t in touch at [e
+00001840: 6e67 6c61 6e64 2e74 6461 7540 6e68 732e  ngland.tdau@nhs.
+00001850: 6e65 745d 286d 6169 6c74 6f3a 656e 676c  net](mailto:engl
+00001860: 616e 642e 7464 6175 406e 6873 2e6e 6574  and.tdau@nhs.net
+00001870: 292e 0a0a 3c21 2d2d 2023 2323 2041 636b  )...<!-- ### Ack
+00001880: 6e6f 776c 6564 6765 6d65 6e74 7320 2d2d  nowledgements --
+00001890: 3e0a                                     >.
```

### Comparing `nhssynth-0.1.3/pyproject.toml` & `nhssynth-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,49 @@
 [tool.poetry]
 name = "nhssynth"
-version = "0.1.3"
+version = "0.2.0"
 description = "Synthetic data generation pipeline leveraging a Differentially Private Variational Auto Encoder assessed using a variety of metrics"
 authors = ["HarrisonWilde <harrisondwilde@outlook.com>"]
+maintainers = ["NHSE TDAU <england.tdau@nhs.net>"]
 license = "MIT"
-readme = ["README.md", "src/nhssynth/modules/README.md"]
+readme = ["README.md"]
 repository = "https://github.com/nhsx/NHSSynth"
 keywords = ["synthetic data", "privacy", "fairness", "machine learning"]
 classifiers = [
     "Development Status :: 3 - Alpha"
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/nhsx/NHSSynth/issues"
+"Docs" = "https://nhsx.github.io/NHSSynth"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.9,<3.11"
 torch = "^1.13.1"
 tqdm = "^4.65.0"
 scikit-learn = "^1.2.1"
 rdt = "^1.3.0"
-opacus = "^1.3.0"
-sdv = "1.0.0b1"
+opacus = "~0.14.0"
+sdv = "^1.0.0"
 pandas = "^1.5.3"
 gower = "^0.1.2"
-matplotlib = "^3.7.1"
+pyyaml = "^6.0"
+setuptools = "^67.6.1"
 
 [tool.poetry.scripts]
 nhssynth = 'nhssynth.cli:run'
 
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+mkdocstrings = {extras = ["python-legacy"], version = "^0.20.0"}
+mkdocs-material = "^9.1.4"
+mkdocs-gen-files = "^0.4.0"
+mkdocs-literate-nav = "^0.6.0"
+mkdocs-section-index = "^0.3.5"
+mkdocs-git-revision-date-localized-plugin = "^1.2.0"
+pymdown-extensions = "^9.10"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nhssynth-0.1.3/src/nhssynth/cli/run.py` & `nhssynth-0.2.0/src/nhssynth/cli/run.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,39 @@
 import argparse
 
-from nhssynth.cli.config import *
-from nhssynth.cli.module_arguments import add_top_level_args
+from nhssynth.cli.config import get_modules_to_run, read_config, write_config
 from nhssynth.cli.module_setup import MODULE_MAP, add_subparser
 
 
-def run():
+def run() -> None:
+    """CLI for preparing, training and evaluating a synthetic data generator."""
 
     parser = argparse.ArgumentParser(
-        prog="SynthVAE", description="CLI for preparing, training and evaluating a synthetic data generator."
+        prog="nhssynth",
+        description="CLI for preparing, training and evaluating a synthetic data generator.",
     )
-    add_top_level_args(parser)
 
     # Below we instantiate one subparser for each module + one for running with a config file and one for
     # doing a full pipeline run with CLI-specified config
     subparsers = parser.add_subparsers()
-
-    # TODO can probably do this better as we dont actually need the `pipeline` or `config` subparsers in this dict
     all_subparsers = {
         name: add_subparser(subparsers, name, option_config) for name, option_config in MODULE_MAP.items()
     }
 
     args = parser.parse_args()
 
     # Use get to return None when no function has been set, i.e. user made no running choice
     executor = vars(args).get("func")
-
-    # If `config` is the specified running choice, we mutate `args` in `read_config`
-    # else we execute according to the user's choice
-    # else we return `--help` if no choice has been passed, i.e. executor is None
-    if not executor:
-        args = read_config(args, parser, all_subparsers)
-    elif executor:
+    if executor:
+        args.modules_to_run = get_modules_to_run(executor)
+        args.module_handover = {}
         executor(args)
+    elif hasattr(args, "input_config"):
+        args = read_config(args, parser, all_subparsers)
     else:
-        parser.parse_args(["--help"])
+        return parser.print_help()
 
     # Whenever either are specified, we want to dump the configuration to allow for this run to be replicated
-    if args.save_config or args.save_config_path:
-        if not args.save_config_path:
-            args.save_config_path = f"experiments/{args.run_name}/config_{args.run_name}.yaml"
+    if args.save_config:
         write_config(args, all_subparsers)
 
-    print("Complete!")
-
-
-if __name__ == "__main__":
-    run()
+    print("Finished!")
```

### Comparing `nhssynth-0.1.3/src/nhssynth/modules/evaluation/metrics.py` & `nhssynth-0.2.0/src/nhssynth/modules/evaluation/metrics.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,130 +1,98 @@
-import numpy as np
-from sdv.evaluation import evaluate
-import gower
-import pandas as pd
+# import gower
+# import numpy as np
+# import pandas as pd
 
-from sdv.metrics.tabular import NumericalMLP, CategoricalSVM
 
-# Distributional metrics - Check distribution differences between synthetic & original dataset as well as how
-# Easy it is to discriminate them i.e. svc detection
-def distribution_metrics(
-    gower_bool,
-    distributional_metrics,
-    data_supp,
-    synthetic_supp,
-    categorical_columns,
-    continuous_columns,
-    saving_filepath="metrics/",
-    pre_proc_method="GMM",
-):
+# # Distributional metrics - Check distribution differences between synthetic & original dataset as well as how
+# # Easy it is to discriminate them i.e. svc detection
+# def distribution_metrics(
+#     args,
+#     data_supp,
+#     synthetic_supp,
+#     categorical_columns,
+# ):
+#     # Define lists to contain the metrics achieved
 
-    # Define lists to contain the metrics achieved
+#     metrics = []
 
-    no_metrics = len(distributional_metrics)
-    metrics = []
+#     # Need these in same column order
 
-    # Need these in same column order
+#     synthetic_supp = synthetic_supp[data_supp.columns]
 
-    synthetic_supp = synthetic_supp[data_supp.columns]
+#     # Now categorical columns need to be converted to objects as SDV infers data
+#     # types from the fields and integers/floats are treated as numerical not categorical
 
-    # Now categorical columns need to be converted to objects as SDV infers data
-    # types from the fields and integers/floats are treated as numerical not categorical
+#     synthetic_supp[categorical_columns] = synthetic_supp[categorical_columns].astype(object)
+#     data_supp[categorical_columns] = data_supp[categorical_columns].astype(object)
 
-    synthetic_supp[categorical_columns] = synthetic_supp[categorical_columns].astype(
-        object
-    )
-    data_supp[categorical_columns] = data_supp[categorical_columns].astype(object)
+#     evals = evaluate(synthetic_supp, data_supp, metrics=distributional_metrics, aggregate=False)
 
-    evals = evaluate(
-        synthetic_supp, data_supp, metrics=distributional_metrics, aggregate=False
-    )
+#     # evals is a pandas dataframe of metrics - if we want to add a gower metric then we can
+#     # save this separately
 
-    # evals is a pandas dataframe of metrics - if we want to add a gower metric then we can
-    # save this separately
+#     metrics = np.array(evals["raw_score"])
 
-    metrics = np.array(evals["raw_score"])
+#     if gower_bool == True:
+#         # Find the gower distance
+#         metrics = np.append(metrics, np.mean(gower.gower_matrix(data_supp, synthetic_supp)))
 
-    if gower_bool == True:
+#         metrics = pd.DataFrame(data=[metrics], columns=(distributional_metrics + ["Gower"]))
 
-        # Find the gower distance
-        metrics = np.append(
-            metrics, np.mean(gower.gower_matrix(data_supp, synthetic_supp))
-        )
+#     else:
+#         metrics = pd.DataFrame(data=[metrics], columns=(distributional_metrics))
 
-        metrics = pd.DataFrame(
-            data=[metrics], columns=(distributional_metrics + ["Gower"])
-        )
+#     # Save these metrics into a pandas dataframe - if the user wants to
 
-    else:
+#     if saving_filepath != None:
+#         metrics.to_csv("{}Metrics_SynthVAE_{}.csv".format(saving_filepath, pre_proc_method))
 
-        metrics = pd.DataFrame(data=[metrics], columns=(distributional_metrics))
+#     return metrics
 
-    # Save these metrics into a pandas dataframe - if the user wants to
 
-    if saving_filepath != None:
+# # Build in some privacy metrics from SDV - TO DO!!!
 
-        metrics.to_csv(
-            "{}Metrics_SynthVAE_{}.csv".format(saving_filepath, pre_proc_method)
-        )
 
-    return metrics
+# def privacy_metrics(
+#     private_variable,
+#     data_supp,
+#     synthetic_supp,
+#     categorical_columns,
+#     continuous_columns,
+# ):
+#     if private_variable in continuous_columns:
+#         continuous_columns = [column for column in continuous_columns if column != private_variable]
 
+#         mlp_priv = NumericalMLP.compute(
+#             data_supp.fillna(0),
+#             synthetic_supp.fillna(0),
+#             key_fields=(continuous_columns),
+#             sensitive_fields=[private_variable],
+#         )
 
-# Build in some privacy metrics from SDV - TO DO!!!
+#         return mlp_priv
 
+#     elif private_variable in categorical_columns:
+#         categorical_columns = [column for column in categorical_columns if column != private_variable]
 
-def privacy_metrics(
-    private_variable,
-    data_supp,
-    synthetic_supp,
-    categorical_columns,
-    continuous_columns,
-    saving_filepath=None,
-    pre_proc_method="GMM",
-):
+#         svm_priv = CategoricalSVM.compute(
+#             data_supp.fillna(0),
+#             synthetic_supp.fillna(0),
+#             key_fields=(categorical_columns),
+#             sensitive_fields=[private_variable],
+#         )
 
-    if private_variable in continuous_columns:
+#         return svm_priv
 
-        continuous_columns = [
-            column for column in continuous_columns if column != private_variable
-        ]
 
-        mlp_priv = NumericalMLP.compute(
-            data_supp.fillna(0),
-            synthetic_supp.fillna(0),
-            key_fields=(continuous_columns),
-            sensitive_fields=[private_variable],
-        )
+# # Build in some fairness metrics (will have to find a library/code these ourselves) - TO DO!!!
 
-        return mlp_priv
 
-    elif private_variable in categorical_columns:
-
-        categorical_columns = [
-            column for column in categorical_columns if column != private_variable
-        ]
-
-        svm_priv = CategoricalSVM.compute(
-            data_supp.fillna(0),
-            synthetic_supp.fillna(0),
-            key_fields=(categorical_columns),
-            sensitive_fields=[private_variable],
-        )
-
-        return svm_priv
-
-
-# Build in some fairness metrics (will have to find a library/code these ourselves) - TO DO!!!
-
-
-def fairness_metrics(
-    user_metrics,
-    data_supp,
-    synthetic_supp,
-    categorical_columns,
-    continuous_columns,
-    saving_filepath=None,
-    pre_proc_method="GMM",
-):
-
-    return None
+# def fairness_metrics(
+#     user_metrics,
+#     data_supp,
+#     synthetic_supp,
+#     categorical_columns,
+#     continuous_columns,
+#     saving_filepath=None,
+# ):
+#     return None
```

### Comparing `nhssynth-0.1.3/src/nhssynth/modules/plotting/plot.py` & `nhssynth-0.2.0/src/nhssynth/modules/plotting/plots.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,155 +1,208 @@
-import argparse
-import numpy as np
-import pandas as pd
-import torch
-
-# For Gower distance
-import gower
-
-# For the SUPPORT dataset
-from pycox.datasets import support
-
-# VAE functions
-from VAE import Decoder, Encoder, VAE
+# import argparse
+# import numpy as np
+# import pandas as pd
+# import torch
 
-from utils import support_pre_proc, reverse_transformers
-
-# Plotting
-import matplotlib
-
-font = {"size": 14}
-matplotlib.rc("font", **font)
 import matplotlib.pyplot as plt
-from mpl_toolkits.axes_grid1 import make_axes_locatable
-
-# For the SUPPORT dataset
-from pycox.datasets import support
-
-# VAE functions
-from VAE import Decoder, Encoder, VAE
-
-parser = argparse.ArgumentParser()
-
-parser.add_argument(
-    "--save_file",
-    required=True,
-    type=str,
-    help="load trained model's state_dict from file",
-)
-
-parser.add_argument(
-    "--pre_proc_method",
-    default="GMM",
-    type=str,
-    help="Choose the pre-processing method that you will apply to the dataset, either GMM or standard",
-)
-
-args = parser.parse_args()
-
-# Import and preprocess the SUPPORT data for ground truth correlations
-data_supp = support.read_df()
-
-# Save the original columns
-
-original_continuous_columns = ["duration"] + [f"x{i}" for i in range(7, 15)]
-original_categorical_columns = ["event"] + [f"x{i}" for i in range(1, 7)]
-
-original_columns = original_categorical_columns + original_continuous_columns
-#%% -------- Data Pre-Processing -------- #
-pre_proc_method = args.pre_proc_method
-
-(
-    x_train,
-    data_supp,
-    reordered_dataframe_columns,
-    continuous_transformers,
-    categorical_transformers,
-    num_categories,
-    num_continuous,
-) = support_pre_proc(data_supp=data_supp, pre_proc_method=pre_proc_method)
-
-
-###############################################################################
-
-# Load saved model - ensure parameters are equivalent to the saved model
-latent_dim = 256
-hidden_dim = 256
-encoder = Encoder(x_train.shape[1], latent_dim, hidden_dim=hidden_dim)
-decoder = Decoder(latent_dim, num_continuous, num_categories=num_categories)
-vae = VAE(encoder, decoder)
-vae.load(args.save_file)
-
-#%% -------- Generate Synthetic Data -------- #
-
-# Generate a synthetic set using trained vae
-
-synthetic_trial = vae.generate(data_supp.shape[0])  # 8873 is size of support
-#%% -------- Inverse Transformation On Synthetic Trial -------- #
+import pandas as pd
+import plotly.graph_objects as go
+import plotly.io as pio
+from sklearn.manifold import TSNE
+
+
+def factorize_all_categoricals(
+    df: pd.DataFrame,
+) -> pd.DataFrame:
+    """Factorize all categorical columns in a dataframe."""
+    for col in df.columns:
+        if df[col].dtype == "object":
+            df[col] = pd.factorize(df[col])[0]
+        elif df[col].dtype == "datetime64[ns]":
+            df[col] = pd.to_numeric(df[col])
+        min_val = df[col].min()
+        max_val = df[col].max()
+        df[col] = (df[col] - min_val) / (max_val - min_val)
+
+    return df
+
+
+def tsne(
+    X_gt: pd.DataFrame,
+    X_syn: pd.DataFrame,
+) -> None:
+    fig, ax = plt.subplots(1, 1, figsize=(12, 10))
+
+    tsne_gt = TSNE(n_components=2, random_state=0, learning_rate="auto", init="pca")
+    proj_gt = pd.DataFrame(tsne_gt.fit_transform(factorize_all_categoricals(X_gt)))
+
+    tsne_syn = TSNE(n_components=2, random_state=0, learning_rate="auto", init="pca")
+    proj_syn = pd.DataFrame(tsne_syn.fit_transform(factorize_all_categoricals(X_syn)))
+
+    fig = go.Figure()
+
+    fig.add_trace(go.Scatter(x=proj_gt[0], y=proj_gt[1], mode="markers", marker=dict(size=10), name="Real data"))
+
+    fig.add_trace(go.Scatter(x=proj_syn[0], y=proj_syn[1], mode="markers", marker=dict(size=10), name="Synthetic data"))
+
+    # Set axis labels and legend
+    fig.update_layout(
+        title="t-SNE plot",
+        xaxis_title="t-SNE 1",
+        yaxis_title="t-SNE 2",
+        legend=dict(x=0, y=1, bgcolor="rgba(255, 255, 255, 0.5)"),
+    )
 
-synthetic_sample = vae.generate(data_supp.shape[0])
+    # Show plot
+    fig.show()
 
-if torch.cuda.is_available():
-    synthetic_sample = pd.DataFrame(
-        synthetic_sample.cpu().detach(), columns=reordered_dataframe_columns
-    )
-else:
-    synthetic_sample = pd.DataFrame(
-        synthetic_sample.detach(), columns=reordered_dataframe_columns
-    )
 
-# Reverse the transformations
+# # For Gower distance
+# import gower
 
-synthetic_supp = reverse_transformers(
-    synthetic_set=synthetic_sample,
-    data_supp_columns=data_supp.columns,
-    cont_transformers=continuous_transformers,
-    cat_transformers=categorical_transformers,
-    pre_proc_method=pre_proc_method,
-)
-
-
-### Create plots
-# Plot 1: Correlation matrix of original data
-plt.figure()
-ax = plt.gca()
-ax.axes.get_xaxis().set_visible(False)
-ax.axes.get_yaxis().set_visible(False)
-im = ax.matshow(data_supp.corr())
-#####
-# Credit: https://stackoverflow.com/questions/18195758/set-matplotlib-colorbar-size-to-match-graph
-divider = make_axes_locatable(ax)
-cax = divider.append_axes("right", size="5%", pad=0.05)
-#####
-plt.colorbar(im, cax=cax)
-plt.savefig("actual_corr_{}.png".format(pre_proc_method), bbox_inches="tight")
-# Plot 2: Correlation matrix of synthetic data
-plt.figure()
-ax = plt.gca()
-ax.axes.get_xaxis().set_visible(False)
-ax.axes.get_yaxis().set_visible(False)
-im = ax.matshow(synthetic_supp.corr())
-#####
-# Credit: https://stackoverflow.com/questions/18195758/set-matplotlib-colorbar-size-to-match-graph
-divider = make_axes_locatable(ax)
-cax = divider.append_axes("right", size="5%", pad=0.05)
-#####
-plt.colorbar(im, cax=cax)
-plt.savefig("sample_corr_{}.png".format(pre_proc_method), bbox_inches="tight")
-# Plot 3: Difference between real and synth correlation matrices + Gower and RMSE values
-plt.figure()
-g = np.mean(gower.gower_matrix(data_supp, synthetic_supp))
-p = np.sqrt(
-    np.mean((data_supp.corr().to_numpy() - synthetic_supp.corr().to_numpy()) ** 2)
-)
-plt.title(f"Gower Distance = {g:.4f}\n Correlation RMSE = {p:.4f}")
-ax = plt.gca()
-ax.axes.get_xaxis().set_visible(False)
-ax.axes.get_yaxis().set_visible(False)
-im = ax.matshow(synthetic_supp.corr() - data_supp.corr())
-#####
-# Credit: https://stackoverflow.com/questions/18195758/set-matplotlib-colorbar-size-to-match-graph
-divider = make_axes_locatable(ax)
-cax = divider.append_axes("right", size="5%", pad=0.05)
-#####
-plt.colorbar(im, cax=cax)
-plt.savefig("diff_corr_{}.png".format(pre_proc_method), bbox_inches="tight")
+# # For the SUPPORT dataset
+# from pycox.datasets import support
+
+# # VAE functions
+# from VAE import Decoder, Encoder, VAE
+
+# from utils import support_pre_proc, reverse_transformers
+
+# # Plotting
+# import matplotlib
+
+# font = {"size": 14}
+# matplotlib.rc("font", **font)
+# import matplotlib.pyplot as plt
+# from mpl_toolkits.axes_grid1 import make_axes_locatable
+
+# # For the SUPPORT dataset
+# from pycox.datasets import support
+
+# # VAE functions
+# from VAE import Decoder, Encoder, VAE
+
+# parser = argparse.ArgumentParser()
+
+# parser.add_argument(
+#     "--save_file",
+#     required=True,
+#     type=str,
+#     help="load trained model's state_dict from file",
+# )
+
+# parser.add_argument(
+#     "--pre_proc_method",
+#     default="GMM",
+#     type=str,
+#     help="Choose the pre-processing method that you will apply to the dataset, either GMM or standard",
+# )
+
+# args = parser.parse_args()
+
+# # Import and preprocess the SUPPORT data for ground truth correlations
+# data_supp = support.read_df()
+
+# # Save the original columns
+
+# original_continuous_columns = ["duration"] + [f"x{i}" for i in range(7, 15)]
+# original_categorical_columns = ["event"] + [f"x{i}" for i in range(1, 7)]
+
+# original_columns = original_categorical_columns + original_continuous_columns
+# #%% -------- Data Pre-Processing -------- #
+# pre_proc_method = args.pre_proc_method
+
+# (
+#     x_train,
+#     data_supp,
+#     reordered_dataframe_columns,
+#     continuous_transformers,
+#     categorical_transformers,
+#     num_categories,
+#     num_continuous,
+# ) = support_pre_proc(data_supp=data_supp, pre_proc_method=pre_proc_method)
+
+
+# ###############################################################################
+
+# # Load saved model - ensure parameters are equivalent to the saved model
+# latent_dim = 256
+# hidden_dim = 256
+# encoder = Encoder(x_train.shape[1], latent_dim, hidden_dim=hidden_dim)
+# decoder = Decoder(latent_dim, num_continuous, num_categories=num_categories)
+# vae = VAE(encoder, decoder)
+# vae.load(args.save_file)
+
+# #%% -------- Generate Synthetic Data -------- #
+
+# # Generate a synthetic set using trained vae
+
+# synthetic_trial = vae.generate(data_supp.shape[0])  # 8873 is size of support
+# #%% -------- Inverse Transformation On Synthetic Trial -------- #
+
+# synthetic_sample = vae.generate(data_supp.shape[0])
+
+# if torch.cuda.is_available():
+#     synthetic_sample = pd.DataFrame(
+#         synthetic_sample.cpu().detach(), columns=reordered_dataframe_columns
+#     )
+# else:
+#     synthetic_sample = pd.DataFrame(
+#         synthetic_sample.detach(), columns=reordered_dataframe_columns
+#     )
+
+# # Reverse the transformations
+
+# synthetic_supp = reverse_transformers(
+#     synthetic_set=synthetic_sample,
+#     data_supp_columns=data_supp.columns,
+#     cont_transformers=continuous_transformers,
+#     cat_transformers=categorical_transformers,
+#     pre_proc_method=pre_proc_method,
+# )
+
+
+# ### Create plots
+# # Plot 1: Correlation matrix of original data
+# plt.figure()
+# ax = plt.gca()
+# ax.axes.get_xaxis().set_visible(False)
+# ax.axes.get_yaxis().set_visible(False)
+# im = ax.matshow(data_supp.corr())
+# #####
+# # Credit: https://stackoverflow.com/questions/18195758/set-matplotlib-colorbar-size-to-match-graph
+# divider = make_axes_locatable(ax)
+# cax = divider.append_axes("right", size="5%", pad=0.05)
+# #####
+# plt.colorbar(im, cax=cax)
+# plt.savefig("actual_corr_{}.png".format(pre_proc_method), bbox_inches="tight")
+# # Plot 2: Correlation matrix of synthetic data
+# plt.figure()
+# ax = plt.gca()
+# ax.axes.get_xaxis().set_visible(False)
+# ax.axes.get_yaxis().set_visible(False)
+# im = ax.matshow(synthetic_supp.corr())
+# #####
+# # Credit: https://stackoverflow.com/questions/18195758/set-matplotlib-colorbar-size-to-match-graph
+# divider = make_axes_locatable(ax)
+# cax = divider.append_axes("right", size="5%", pad=0.05)
+# #####
+# plt.colorbar(im, cax=cax)
+# plt.savefig("sample_corr_{}.png".format(pre_proc_method), bbox_inches="tight")
+# # Plot 3: Difference between real and synth correlation matrices + Gower and RMSE values
+# plt.figure()
+# g = np.mean(gower.gower_matrix(data_supp, synthetic_supp))
+# p = np.sqrt(
+#     np.mean((data_supp.corr().to_numpy() - synthetic_supp.corr().to_numpy()) ** 2)
+# )
+# plt.title(f"Gower Distance = {g:.4f}\n Correlation RMSE = {p:.4f}")
+# ax = plt.gca()
+# ax.axes.get_xaxis().set_visible(False)
+# ax.axes.get_yaxis().set_visible(False)
+# im = ax.matshow(synthetic_supp.corr() - data_supp.corr())
+# #####
+# # Credit: https://stackoverflow.com/questions/18195758/set-matplotlib-colorbar-size-to-match-graph
+# divider = make_axes_locatable(ax)
+# cax = divider.append_axes("right", size="5%", pad=0.05)
+# #####
+# plt.colorbar(im, cax=cax)
+# plt.savefig("diff_corr_{}.png".format(pre_proc_method), bbox_inches="tight")
```

