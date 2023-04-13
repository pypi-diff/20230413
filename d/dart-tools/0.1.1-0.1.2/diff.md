# Comparing `tmp/dart-tools-0.1.1.tar.gz` & `tmp/dart-tools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dart-tools-0.1.1.tar", last modified: Tue Feb 28 04:27:55 2023, max compression
+gzip compressed data, was "dart-tools-0.1.2.tar", last modified: Thu Apr 13 20:39:45 2023, max compression
```

## Comparing `dart-tools-0.1.1.tar` & `dart-tools-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-02-28 04:27:55.137189 dart-tools-0.1.1/
--rw-r--r--   0 zack       (501) staff       (20)     1061 2023-02-28 02:56:19.000000 dart-tools-0.1.1/LICENSE
--rw-r--r--   0 zack       (501) staff       (20)     3997 2023-02-28 04:27:55.136399 dart-tools-0.1.1/PKG-INFO
--rw-r--r--   0 zack       (501) staff       (20)     1099 2023-02-28 04:24:48.000000 dart-tools-0.1.1/README.md
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-02-28 04:27:55.133294 dart-tools-0.1.1/dart/
--rw-r--r--   0 zack       (501) staff       (20)       64 2023-02-28 04:01:58.000000 dart-tools-0.1.1/dart/__init__.py
--rwxr-xr-x   0 zack       (501) staff       (20)    11058 2023-02-28 04:01:58.000000 dart-tools-0.1.1/dart/dart.py
--rw-r--r--   0 zack       (501) staff       (20)     1709 2023-02-28 02:57:20.000000 dart-tools-0.1.1/dart/order_manager.py
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-02-28 04:27:55.135765 dart-tools-0.1.1/dart_tools.egg-info/
--rw-r--r--   0 zack       (501) staff       (20)     3997 2023-02-28 04:27:55.000000 dart-tools-0.1.1/dart_tools.egg-info/PKG-INFO
--rw-r--r--   0 zack       (501) staff       (20)      290 2023-02-28 04:27:55.000000 dart-tools-0.1.1/dart_tools.egg-info/SOURCES.txt
--rw-r--r--   0 zack       (501) staff       (20)        1 2023-02-28 04:27:55.000000 dart-tools-0.1.1/dart_tools.egg-info/dependency_links.txt
--rw-r--r--   0 zack       (501) staff       (20)       34 2023-02-28 04:27:55.000000 dart-tools-0.1.1/dart_tools.egg-info/entry_points.txt
--rw-r--r--   0 zack       (501) staff       (20)       14 2023-02-28 04:27:55.000000 dart-tools-0.1.1/dart_tools.egg-info/requires.txt
--rw-r--r--   0 zack       (501) staff       (20)        5 2023-02-28 04:27:55.000000 dart-tools-0.1.1/dart_tools.egg-info/top_level.txt
--rw-r--r--   0 zack       (501) staff       (20)     1750 2023-02-28 04:27:23.000000 dart-tools-0.1.1/pyproject.toml
--rw-r--r--   0 zack       (501) staff       (20)       38 2023-02-28 04:27:55.137402 dart-tools-0.1.1/setup.cfg
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-04-13 20:39:45.249085 dart-tools-0.1.2/
+-rw-r--r--   0 zack       (501) staff       (20)     1061 2023-02-28 02:56:19.000000 dart-tools-0.1.2/LICENSE
+-rw-r--r--   0 zack       (501) staff       (20)     4408 2023-04-13 20:39:45.248750 dart-tools-0.1.2/PKG-INFO
+-rw-r--r--   0 zack       (501) staff       (20)     1510 2023-04-03 00:03:57.000000 dart-tools-0.1.2/README.md
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-04-13 20:39:45.245988 dart-tools-0.1.2/dart/
+-rw-r--r--   0 zack       (501) staff       (20)       64 2023-02-28 04:01:58.000000 dart-tools-0.1.2/dart/__init__.py
+-rwxr-xr-x   0 zack       (501) staff       (20)    11087 2023-04-13 20:37:15.000000 dart-tools-0.1.2/dart/dart.py
+-rw-r--r--   0 zack       (501) staff       (20)     1709 2023-02-28 02:57:20.000000 dart-tools-0.1.2/dart/order_manager.py
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-04-13 20:39:45.248256 dart-tools-0.1.2/dart_tools.egg-info/
+-rw-r--r--   0 zack       (501) staff       (20)     4408 2023-04-13 20:39:45.000000 dart-tools-0.1.2/dart_tools.egg-info/PKG-INFO
+-rw-r--r--   0 zack       (501) staff       (20)      290 2023-04-13 20:39:45.000000 dart-tools-0.1.2/dart_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 zack       (501) staff       (20)        1 2023-04-13 20:39:45.000000 dart-tools-0.1.2/dart_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 zack       (501) staff       (20)       34 2023-04-13 20:39:45.000000 dart-tools-0.1.2/dart_tools.egg-info/entry_points.txt
+-rw-r--r--   0 zack       (501) staff       (20)       14 2023-04-13 20:39:45.000000 dart-tools-0.1.2/dart_tools.egg-info/requires.txt
+-rw-r--r--   0 zack       (501) staff       (20)        5 2023-04-13 20:39:45.000000 dart-tools-0.1.2/dart_tools.egg-info/top_level.txt
+-rw-r--r--   0 zack       (501) staff       (20)     1789 2023-04-13 20:34:41.000000 dart-tools-0.1.2/pyproject.toml
+-rw-r--r--   0 zack       (501) staff       (20)       38 2023-04-13 20:39:45.249195 dart-tools-0.1.2/setup.cfg
```

### Comparing `dart-tools-0.1.1/LICENSE` & `dart-tools-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dart-tools-0.1.1/PKG-INFO` & `dart-tools-0.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6461 7274  : 2.1.Name: dart
 00000020: 2d74 6f6f 6c73 0a56 6572 7369 6f6e 3a20  -tools.Version: 
-00000030: 302e 312e 310a 5375 6d6d 6172 793a 2054  0.1.1.Summary: T
+00000030: 302e 312e 320a 5375 6d6d 6172 793a 2054  0.1.2.Summary: T
 00000040: 6865 2044 6172 7420 434c 4920 616e 6420  he Dart CLI and 
 00000050: 5079 7468 6f6e 204c 6962 7261 7279 0a41  Python Library.A
 00000060: 7574 686f 722d 656d 6169 6c3a 2044 6172  uthor-email: Dar
 00000070: 7420 536f 6674 7761 7265 2054 6561 6d20  t Software Team 
 00000080: 3c73 6f66 7477 6172 6540 6974 7364 6172  <software@itsdar
 00000090: 742e 636f 6d3e 0a4c 6963 656e 7365 3a20  t.com>.License: 
 000000a0: 4d49 5420 4c69 6365 6e73 650a 2020 2020  MIT License.    
@@ -175,76 +175,102 @@
 00000ae0: 4c69 6272 6172 6965 7320 3a3a 2050 7974  Libraries :: Pyt
 00000af0: 686f 6e20 4d6f 6475 6c65 730a 5265 7175  hon Modules.Requ
 00000b00: 6972 6573 2d50 7974 686f 6e3a 203e 3d33  ires-Python: >=3
 00000b10: 2e37 0a44 6573 6372 6970 7469 6f6e 2d43  .7.Description-C
 00000b20: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
 00000b30: 742f 6d61 726b 646f 776e 0a4c 6963 656e  t/markdown.Licen
 00000b40: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
-00000b50: 0a0a 2320 6461 7274 2d74 6f6f 6c73 0a0a  ..# dart-tools..
-00000b60: 5b44 6172 745d 2868 7474 7073 3a2f 2f69  [Dart](https://i
-00000b70: 7473 6461 7274 2e63 6f6d 3f6e 723d 3129  tsdart.com?nr=1)
-00000b80: 2069 7320 5072 6f6a 6563 7420 4d61 6e61   is Project Mana
-00000b90: 6765 6d65 6e74 206f 6e20 4175 746f 7069  gement on Autopi
-00000ba0: 6c6f 742e 0a0a 5468 6973 2069 7320 7468  lot...This is th
-00000bb0: 6520 4461 7274 2043 4c49 2061 6e64 2050  e Dart CLI and P
-00000bc0: 7974 686f 6e20 4c69 6272 6172 792e 2049  ython Library. I
-00000bd0: 7420 656e 6162 6c65 7320 6469 7265 6374  t enables direct
-00000be0: 2069 6e74 6572 6174 696f 6e20 7769 7468   interation with
-00000bf0: 2044 6172 7420 7468 726f 7567 6820 6120   Dart through a 
-00000c00: 7465 726d 696e 616c 2043 4c49 206f 7220  terminal CLI or 
-00000c10: 7468 726f 7567 6820 5079 7468 6f6e 2e0a  through Python..
-00000c20: 0a0a 2323 2053 6574 7570 0a0a 496e 2074  ..## Setup..In t
-00000c30: 6865 2074 6572 6d69 6e61 6c2c 2069 6e73  he terminal, ins
-00000c40: 7461 6c6c 2077 6974 680a 6060 6062 6173  tall with.```bas
-00000c50: 680a 7069 7020 696e 7374 616c 6c20 6461  h.pip install da
-00000c60: 7274 2d74 6f6f 6c73 0a60 6060 0a0a 5468  rt-tools.```..Th
-00000c70: 656e 2c20 6c6f 6769 6e20 7769 7468 0a60  en, login with.`
-00000c80: 6060 6261 7368 0a64 6172 7420 6c6f 6769  ``bash.dart logi
-00000c90: 6e0a 6060 600a 0a0a 2323 2055 7361 6765  n.```...## Usage
-00000ca0: 0a0a 2323 2320 4173 2061 2043 4c49 0a0a  ..### As a CLI..
-00000cb0: 496e 2074 6865 2074 6572 6d69 6e61 6c2c  In the terminal,
-00000cc0: 2073 6565 2074 6865 2068 656c 7020 6d65   see the help me
-00000cd0: 7373 6167 6520 7769 7468 0a60 6060 6261  ssage with.```ba
-00000ce0: 7368 0a64 6172 7420 2d2d 6865 6c70 0a60  sh.dart --help.`
-00000cf0: 6060 0a0a 4372 6561 7465 2061 2074 6173  ``..Create a tas
-00000d00: 6b20 7769 7468 0a60 6060 6261 7368 0a64  k with.```bash.d
-00000d10: 6172 7420 6372 6561 7465 7461 736b 2022  art createtask "
-00000d20: 6e65 7720 7461 736b 220a 6060 600a 0a42  new task".```..B
-00000d30: 6567 696e 2077 6f72 6b20 6f6e 2061 2074  egin work on a t
-00000d40: 6173 6b20 7769 7468 0a60 6060 6261 7368  ask with.```bash
-00000d50: 0a64 6172 7420 6265 6769 6e74 6173 6b0a  .dart begintask.
-00000d60: 6060 600a 0a23 2323 2041 7320 6120 5079  ```..### As a Py
-00000d70: 7468 6f6e 204c 6962 7261 7279 0a0a 496e  thon Library..In
-00000d80: 2050 7974 686f 6e2c 2072 756e 0a60 6060   Python, run.```
-00000d90: 7079 7468 6f6e 0a66 726f 6d20 6461 7274  python.from dart
-00000da0: 2069 6d70 6f72 7420 6c6f 6769 6e2c 2063   import login, c
-00000db0: 7265 6174 655f 7461 736b 2c20 6265 6769  reate_task, begi
-00000dc0: 6e5f 7461 736b 0a0a 2320 6f6e 6c79 206e  n_task..# only n
-00000dd0: 6565 6465 6420 6f6e 6520 7469 6d65 0a6c  eeded one time.l
-00000de0: 6f67 696e 2829 0a0a 6372 6561 7465 5f74  ogin()..create_t
-00000df0: 6173 6b28 226e 6577 2074 6173 6b22 290a  ask("new task").
-00000e00: 0a62 6567 696e 5f74 6173 6b28 290a 6060  .begin_task().``
-00000e10: 600a 0a23 2320 4865 6c70 2061 6e64 2052  `..## Help and R
-00000e20: 6573 6f75 7263 6573 0a0a 2d20 5b48 6f6d  esources..- [Hom
-00000e30: 6570 6167 655d 2868 7474 7073 3a2f 2f77  epage](https://w
-00000e40: 7777 2e69 7473 6461 7274 2e63 6f6d 2f3f  ww.itsdart.com/?
-00000e50: 6e72 3d31 290a 2d20 5b57 6562 2041 7070  nr=1).- [Web App
-00000e60: 5d28 6874 7470 733a 2f2f 6170 702e 6974  ](https://app.it
-00000e70: 7364 6172 742e 636f 6d2f 290a 2d20 5b48  sdart.com/).- [H
-00000e80: 656c 7020 4365 6e74 6572 5d28 6874 7470  elp Center](http
-00000e90: 733a 2f2f 6974 732d 6461 7274 2e6e 6f74  s://its-dart.not
-00000ea0: 696f 6e2e 7369 7465 2f44 6172 742d 4865  ion.site/Dart-He
-00000eb0: 6c70 2d43 656e 7465 722d 3832 3036 6132  lp-Center-8206a2
-00000ec0: 6161 3239 3536 3439 3666 3839 3838 6237  aa2956496f8988b7
-00000ed0: 6233 3263 6463 6432 3035 290a 2d20 5b42  b32cdcd205).- [B
-00000ee0: 7567 7320 616e 6420 4665 6174 7572 6573  ugs and Features
-00000ef0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000f00: 2e63 6f6d 2f69 7473 2d64 6172 742f 6461  .com/its-dart/da
-00000f10: 7274 2d74 6f6f 6c73 2f69 7373 7565 7329  rt-tools/issues)
-00000f20: 0a2d 205b 4c69 6272 6172 7920 536f 7572  .- [Library Sour
-00000f30: 6365 5d28 6874 7470 733a 2f2f 6769 7468  ce](https://gith
-00000f40: 7562 2e63 6f6d 2f69 7473 2d64 6172 742f  ub.com/its-dart/
-00000f50: 6461 7274 2d74 6f6f 6c73 2f29 0a2d 2045  dart-tools/).- E
-00000f60: 6d61 696c 2075 7320 6174 205b 7375 7070  mail us at [supp
-00000f70: 6f72 7440 6974 7364 6172 742e 636f 6d5d  ort@itsdart.com]
-00000f80: 286d 6169 6c74 6f3a 7375 7070 6f72 7440  (mailto:support@
-00000f90: 6974 7364 6172 742e 636f 6d29 0a         itsdart.com).
+00000b50: 0a0a 3c64 6976 2061 6c69 676e 3d22 6365  ..<div align="ce
+00000b60: 6e74 6572 223e 0a20 203c 6831 3e44 6172  nter">.  <h1>Dar
+00000b70: 7420 546f 6f6c 733c 2f68 313e 0a20 203c  t Tools</h1>.  <
+00000b80: 703e 0a20 2020 203c 6120 6872 6566 3d22  p>.    <a href="
+00000b90: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00000ba0: 2f70 726f 6a65 6374 2f64 6172 742d 746f  /project/dart-to
+00000bb0: 6f6c 7322 3e3c 696d 6720 7372 633d 2268  ols"><img src="h
+00000bc0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000bd0: 6473 2e69 6f2f 7079 7069 2f76 2f64 6172  ds.io/pypi/v/dar
+00000be0: 742d 746f 6f6c 732e 7376 6722 2061 6c74  t-tools.svg" alt
+00000bf0: 3d22 5079 5049 223e 3c2f 613e 0a20 2020  ="PyPI"></a>.   
+00000c00: 203c 6120 6872 6566 3d22 746f 782e 696e   <a href="tox.in
+00000c10: 6922 3e3c 696d 6720 7372 633d 2268 7474  i"><img src="htt
+00000c20: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000c30: 2e69 6f2f 7079 7069 2f70 7976 6572 7369  .io/pypi/pyversi
+00000c40: 6f6e 732f 6461 7274 2d74 6f6f 6c73 2220  ons/dart-tools" 
+00000c50: 616c 743d 2253 7570 706f 7274 6564 2050  alt="Supported P
+00000c60: 7974 686f 6e20 5665 7273 696f 6e73 223e  ython Versions">
+00000c70: 3c2f 613e 0a20 2020 203c 6120 6872 6566  </a>.    <a href
+00000c80: 3d22 4c49 4345 4e53 4522 3e3c 696d 6720  ="LICENSE"><img 
+00000c90: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+00000ca0: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
+00000cb0: 7562 2f6c 6963 656e 7365 2f69 7473 2d64  ub/license/its-d
+00000cc0: 6172 742f 6461 7274 2d74 6f6f 6c73 2220  art/dart-tools" 
+00000cd0: 616c 743d 224c 6963 656e 7365 223e 3c2f  alt="License"></
+00000ce0: 613e 0a20 203c 2f70 3e0a 3c2f 6469 763e  a>.  </p>.</div>
+00000cf0: 0a0a 5b44 6172 745d 2868 7474 7073 3a2f  ..[Dart](https:/
+00000d00: 2f69 7473 6461 7274 2e63 6f6d 3f6e 723d  /itsdart.com?nr=
+00000d10: 3129 2069 7320 5072 6f6a 6563 7420 4d61  1) is Project Ma
+00000d20: 6e61 6765 6d65 6e74 206f 6e20 4175 746f  nagement on Auto
+00000d30: 7069 6c6f 742e 0a0a 6064 6172 742d 746f  pilot...`dart-to
+00000d40: 6f6c 7360 2069 7320 7468 6520 4461 7274  ols` is the Dart
+00000d50: 2043 4c49 2061 6e64 2050 7974 686f 6e20   CLI and Python 
+00000d60: 4c69 6272 6172 792e 2049 7420 656e 6162  Library. It enab
+00000d70: 6c65 7320 6469 7265 6374 2069 6e74 6567  les direct integ
+00000d80: 7261 7469 6f6e 2077 6974 6820 4461 7274  ration with Dart
+00000d90: 2074 6872 6f75 6768 2061 2074 6572 6d69   through a termi
+00000da0: 6e61 6c20 434c 4920 6f72 2074 6872 6f75  nal CLI or throu
+00000db0: 6768 2050 7974 686f 6e2e 0a0a 0a23 2320  gh Python....## 
+00000dc0: 5365 7475 700a 0a49 6e20 7468 6520 7465  Setup..In the te
+00000dd0: 726d 696e 616c 2c20 696e 7374 616c 6c20  rminal, install 
+00000de0: 7769 7468 0a60 6060 6261 7368 0a70 6970  with.```bash.pip
+00000df0: 2069 6e73 7461 6c6c 2064 6172 742d 746f   install dart-to
+00000e00: 6f6c 730a 6060 600a 0a54 6865 6e2c 206c  ols.```..Then, l
+00000e10: 6f67 696e 2077 6974 680a 6060 6062 6173  ogin with.```bas
+00000e20: 680a 6461 7274 206c 6f67 696e 0a60 6060  h.dart login.```
+00000e30: 0a0a 0a23 2320 5573 6167 650a 0a23 2323  ...## Usage..###
+00000e40: 2041 7320 6120 434c 490a 0a49 6e20 7468   As a CLI..In th
+00000e50: 6520 7465 726d 696e 616c 2c20 7365 6520  e terminal, see 
+00000e60: 7468 6520 6865 6c70 206d 6573 7361 6765  the help message
+00000e70: 2077 6974 680a 6060 6062 6173 680a 6461   with.```bash.da
+00000e80: 7274 202d 2d68 656c 700a 6060 600a 0a43  rt --help.```..C
+00000e90: 7265 6174 6520 6120 7461 736b 2077 6974  reate a task wit
+00000ea0: 680a 6060 6062 6173 680a 6461 7274 2063  h.```bash.dart c
+00000eb0: 7265 6174 6574 6173 6b20 226e 6577 2074  reatetask "new t
+00000ec0: 6173 6b22 0a60 6060 0a0a 4265 6769 6e20  ask".```..Begin 
+00000ed0: 776f 726b 206f 6e20 6120 7461 736b 2077  work on a task w
+00000ee0: 6974 680a 6060 6062 6173 680a 6461 7274  ith.```bash.dart
+00000ef0: 2062 6567 696e 7461 736b 0a60 6060 0a0a   begintask.```..
+00000f00: 2323 2320 4173 2061 2050 7974 686f 6e20  ### As a Python 
+00000f10: 4c69 6272 6172 790a 0a49 6e20 5079 7468  Library..In Pyth
+00000f20: 6f6e 2c20 7275 6e0a 6060 6070 7974 686f  on, run.```pytho
+00000f30: 6e0a 6672 6f6d 2064 6172 7420 696d 706f  n.from dart impo
+00000f40: 7274 206c 6f67 696e 2c20 6372 6561 7465  rt login, create
+00000f50: 5f74 6173 6b2c 2062 6567 696e 5f74 6173  _task, begin_tas
+00000f60: 6b0a 0a23 206f 6e6c 7920 6e65 6564 6564  k..# only needed
+00000f70: 206f 6e65 2074 696d 650a 6c6f 6769 6e28   one time.login(
+00000f80: 290a 0a63 7265 6174 655f 7461 736b 2822  )..create_task("
+00000f90: 6e65 7720 7461 736b 2229 0a0a 6265 6769  new task")..begi
+00000fa0: 6e5f 7461 736b 2829 0a60 6060 0a0a 2323  n_task().```..##
+00000fb0: 2048 656c 7020 616e 6420 5265 736f 7572   Help and Resour
+00000fc0: 6365 730a 0a2d 205b 486f 6d65 7061 6765  ces..- [Homepage
+00000fd0: 5d28 6874 7470 733a 2f2f 7777 772e 6974  ](https://www.it
+00000fe0: 7364 6172 742e 636f 6d2f 3f6e 723d 3129  sdart.com/?nr=1)
+00000ff0: 0a2d 205b 5765 6220 4170 705d 2868 7474  .- [Web App](htt
+00001000: 7073 3a2f 2f61 7070 2e69 7473 6461 7274  ps://app.itsdart
+00001010: 2e63 6f6d 2f29 0a2d 205b 4865 6c70 2043  .com/).- [Help C
+00001020: 656e 7465 725d 2868 7474 7073 3a2f 2f69  enter](https://i
+00001030: 7473 2d64 6172 742e 6e6f 7469 6f6e 2e73  ts-dart.notion.s
+00001040: 6974 652f 4461 7274 2d48 656c 702d 4365  ite/Dart-Help-Ce
+00001050: 6e74 6572 2d38 3230 3661 3261 6132 3935  nter-8206a2aa295
+00001060: 3634 3936 6638 3938 3862 3762 3332 6364  6496f8988b7b32cd
+00001070: 6364 3230 3529 0a2d 205b 4275 6773 2061  cd205).- [Bugs a
+00001080: 6e64 2046 6561 7475 7265 735d 2868 7474  nd Features](htt
+00001090: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000010a0: 6974 732d 6461 7274 2f64 6172 742d 746f  its-dart/dart-to
+000010b0: 6f6c 732f 6973 7375 6573 290a 2d20 5b4c  ols/issues).- [L
+000010c0: 6962 7261 7279 2053 6f75 7263 655d 2868  ibrary Source](h
+000010d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000010e0: 6d2f 6974 732d 6461 7274 2f64 6172 742d  m/its-dart/dart-
+000010f0: 746f 6f6c 732f 290a 2d20 456d 6169 6c20  tools/).- Email 
+00001100: 7573 2061 7420 5b73 7570 706f 7274 4069  us at [support@i
+00001110: 7473 6461 7274 2e63 6f6d 5d28 6d61 696c  tsdart.com](mail
+00001120: 746f 3a73 7570 706f 7274 4069 7473 6461  to:support@itsda
+00001130: 7274 2e63 6f6d 290a                      rt.com).
```

### Comparing `dart-tools-0.1.1/dart/dart.py` & `dart-tools-0.1.2/dart/dart.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,16 +269,17 @@
         e["duid"]
         for e in user_bundle["statuses"]
         if e["kind"] not in _TERM_STATUS_KINDS
     }
     filtered_tasks = [
         e
         for e in user_bundle["tasks"]
-        if user_email in e["assigneeEmails"]
+        if not e["inTrash"]
         and e["dartboardDuid"] == active_duid
+        and user_email in e["assigneeEmails"]
         and e["statusDuid"] in unterm_status_duids
         and e["drafterEmail"] is None
     ]
     filtered_tasks.sort(key=lambda e: e["order"])
 
     chosen_task = filtered_tasks[
         pick(
```

### Comparing `dart-tools-0.1.1/dart/order_manager.py` & `dart-tools-0.1.2/dart/order_manager.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.1.1/dart_tools.egg-info/PKG-INFO` & `dart-tools-0.1.2/dart_tools.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6461 7274  : 2.1.Name: dart
 00000020: 2d74 6f6f 6c73 0a56 6572 7369 6f6e 3a20  -tools.Version: 
-00000030: 302e 312e 310a 5375 6d6d 6172 793a 2054  0.1.1.Summary: T
+00000030: 302e 312e 320a 5375 6d6d 6172 793a 2054  0.1.2.Summary: T
 00000040: 6865 2044 6172 7420 434c 4920 616e 6420  he Dart CLI and 
 00000050: 5079 7468 6f6e 204c 6962 7261 7279 0a41  Python Library.A
 00000060: 7574 686f 722d 656d 6169 6c3a 2044 6172  uthor-email: Dar
 00000070: 7420 536f 6674 7761 7265 2054 6561 6d20  t Software Team 
 00000080: 3c73 6f66 7477 6172 6540 6974 7364 6172  <software@itsdar
 00000090: 742e 636f 6d3e 0a4c 6963 656e 7365 3a20  t.com>.License: 
 000000a0: 4d49 5420 4c69 6365 6e73 650a 2020 2020  MIT License.    
@@ -175,76 +175,102 @@
 00000ae0: 4c69 6272 6172 6965 7320 3a3a 2050 7974  Libraries :: Pyt
 00000af0: 686f 6e20 4d6f 6475 6c65 730a 5265 7175  hon Modules.Requ
 00000b00: 6972 6573 2d50 7974 686f 6e3a 203e 3d33  ires-Python: >=3
 00000b10: 2e37 0a44 6573 6372 6970 7469 6f6e 2d43  .7.Description-C
 00000b20: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
 00000b30: 742f 6d61 726b 646f 776e 0a4c 6963 656e  t/markdown.Licen
 00000b40: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
-00000b50: 0a0a 2320 6461 7274 2d74 6f6f 6c73 0a0a  ..# dart-tools..
-00000b60: 5b44 6172 745d 2868 7474 7073 3a2f 2f69  [Dart](https://i
-00000b70: 7473 6461 7274 2e63 6f6d 3f6e 723d 3129  tsdart.com?nr=1)
-00000b80: 2069 7320 5072 6f6a 6563 7420 4d61 6e61   is Project Mana
-00000b90: 6765 6d65 6e74 206f 6e20 4175 746f 7069  gement on Autopi
-00000ba0: 6c6f 742e 0a0a 5468 6973 2069 7320 7468  lot...This is th
-00000bb0: 6520 4461 7274 2043 4c49 2061 6e64 2050  e Dart CLI and P
-00000bc0: 7974 686f 6e20 4c69 6272 6172 792e 2049  ython Library. I
-00000bd0: 7420 656e 6162 6c65 7320 6469 7265 6374  t enables direct
-00000be0: 2069 6e74 6572 6174 696f 6e20 7769 7468   interation with
-00000bf0: 2044 6172 7420 7468 726f 7567 6820 6120   Dart through a 
-00000c00: 7465 726d 696e 616c 2043 4c49 206f 7220  terminal CLI or 
-00000c10: 7468 726f 7567 6820 5079 7468 6f6e 2e0a  through Python..
-00000c20: 0a0a 2323 2053 6574 7570 0a0a 496e 2074  ..## Setup..In t
-00000c30: 6865 2074 6572 6d69 6e61 6c2c 2069 6e73  he terminal, ins
-00000c40: 7461 6c6c 2077 6974 680a 6060 6062 6173  tall with.```bas
-00000c50: 680a 7069 7020 696e 7374 616c 6c20 6461  h.pip install da
-00000c60: 7274 2d74 6f6f 6c73 0a60 6060 0a0a 5468  rt-tools.```..Th
-00000c70: 656e 2c20 6c6f 6769 6e20 7769 7468 0a60  en, login with.`
-00000c80: 6060 6261 7368 0a64 6172 7420 6c6f 6769  ``bash.dart logi
-00000c90: 6e0a 6060 600a 0a0a 2323 2055 7361 6765  n.```...## Usage
-00000ca0: 0a0a 2323 2320 4173 2061 2043 4c49 0a0a  ..### As a CLI..
-00000cb0: 496e 2074 6865 2074 6572 6d69 6e61 6c2c  In the terminal,
-00000cc0: 2073 6565 2074 6865 2068 656c 7020 6d65   see the help me
-00000cd0: 7373 6167 6520 7769 7468 0a60 6060 6261  ssage with.```ba
-00000ce0: 7368 0a64 6172 7420 2d2d 6865 6c70 0a60  sh.dart --help.`
-00000cf0: 6060 0a0a 4372 6561 7465 2061 2074 6173  ``..Create a tas
-00000d00: 6b20 7769 7468 0a60 6060 6261 7368 0a64  k with.```bash.d
-00000d10: 6172 7420 6372 6561 7465 7461 736b 2022  art createtask "
-00000d20: 6e65 7720 7461 736b 220a 6060 600a 0a42  new task".```..B
-00000d30: 6567 696e 2077 6f72 6b20 6f6e 2061 2074  egin work on a t
-00000d40: 6173 6b20 7769 7468 0a60 6060 6261 7368  ask with.```bash
-00000d50: 0a64 6172 7420 6265 6769 6e74 6173 6b0a  .dart begintask.
-00000d60: 6060 600a 0a23 2323 2041 7320 6120 5079  ```..### As a Py
-00000d70: 7468 6f6e 204c 6962 7261 7279 0a0a 496e  thon Library..In
-00000d80: 2050 7974 686f 6e2c 2072 756e 0a60 6060   Python, run.```
-00000d90: 7079 7468 6f6e 0a66 726f 6d20 6461 7274  python.from dart
-00000da0: 2069 6d70 6f72 7420 6c6f 6769 6e2c 2063   import login, c
-00000db0: 7265 6174 655f 7461 736b 2c20 6265 6769  reate_task, begi
-00000dc0: 6e5f 7461 736b 0a0a 2320 6f6e 6c79 206e  n_task..# only n
-00000dd0: 6565 6465 6420 6f6e 6520 7469 6d65 0a6c  eeded one time.l
-00000de0: 6f67 696e 2829 0a0a 6372 6561 7465 5f74  ogin()..create_t
-00000df0: 6173 6b28 226e 6577 2074 6173 6b22 290a  ask("new task").
-00000e00: 0a62 6567 696e 5f74 6173 6b28 290a 6060  .begin_task().``
-00000e10: 600a 0a23 2320 4865 6c70 2061 6e64 2052  `..## Help and R
-00000e20: 6573 6f75 7263 6573 0a0a 2d20 5b48 6f6d  esources..- [Hom
-00000e30: 6570 6167 655d 2868 7474 7073 3a2f 2f77  epage](https://w
-00000e40: 7777 2e69 7473 6461 7274 2e63 6f6d 2f3f  ww.itsdart.com/?
-00000e50: 6e72 3d31 290a 2d20 5b57 6562 2041 7070  nr=1).- [Web App
-00000e60: 5d28 6874 7470 733a 2f2f 6170 702e 6974  ](https://app.it
-00000e70: 7364 6172 742e 636f 6d2f 290a 2d20 5b48  sdart.com/).- [H
-00000e80: 656c 7020 4365 6e74 6572 5d28 6874 7470  elp Center](http
-00000e90: 733a 2f2f 6974 732d 6461 7274 2e6e 6f74  s://its-dart.not
-00000ea0: 696f 6e2e 7369 7465 2f44 6172 742d 4865  ion.site/Dart-He
-00000eb0: 6c70 2d43 656e 7465 722d 3832 3036 6132  lp-Center-8206a2
-00000ec0: 6161 3239 3536 3439 3666 3839 3838 6237  aa2956496f8988b7
-00000ed0: 6233 3263 6463 6432 3035 290a 2d20 5b42  b32cdcd205).- [B
-00000ee0: 7567 7320 616e 6420 4665 6174 7572 6573  ugs and Features
-00000ef0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000f00: 2e63 6f6d 2f69 7473 2d64 6172 742f 6461  .com/its-dart/da
-00000f10: 7274 2d74 6f6f 6c73 2f69 7373 7565 7329  rt-tools/issues)
-00000f20: 0a2d 205b 4c69 6272 6172 7920 536f 7572  .- [Library Sour
-00000f30: 6365 5d28 6874 7470 733a 2f2f 6769 7468  ce](https://gith
-00000f40: 7562 2e63 6f6d 2f69 7473 2d64 6172 742f  ub.com/its-dart/
-00000f50: 6461 7274 2d74 6f6f 6c73 2f29 0a2d 2045  dart-tools/).- E
-00000f60: 6d61 696c 2075 7320 6174 205b 7375 7070  mail us at [supp
-00000f70: 6f72 7440 6974 7364 6172 742e 636f 6d5d  ort@itsdart.com]
-00000f80: 286d 6169 6c74 6f3a 7375 7070 6f72 7440  (mailto:support@
-00000f90: 6974 7364 6172 742e 636f 6d29 0a         itsdart.com).
+00000b50: 0a0a 3c64 6976 2061 6c69 676e 3d22 6365  ..<div align="ce
+00000b60: 6e74 6572 223e 0a20 203c 6831 3e44 6172  nter">.  <h1>Dar
+00000b70: 7420 546f 6f6c 733c 2f68 313e 0a20 203c  t Tools</h1>.  <
+00000b80: 703e 0a20 2020 203c 6120 6872 6566 3d22  p>.    <a href="
+00000b90: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00000ba0: 2f70 726f 6a65 6374 2f64 6172 742d 746f  /project/dart-to
+00000bb0: 6f6c 7322 3e3c 696d 6720 7372 633d 2268  ols"><img src="h
+00000bc0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000bd0: 6473 2e69 6f2f 7079 7069 2f76 2f64 6172  ds.io/pypi/v/dar
+00000be0: 742d 746f 6f6c 732e 7376 6722 2061 6c74  t-tools.svg" alt
+00000bf0: 3d22 5079 5049 223e 3c2f 613e 0a20 2020  ="PyPI"></a>.   
+00000c00: 203c 6120 6872 6566 3d22 746f 782e 696e   <a href="tox.in
+00000c10: 6922 3e3c 696d 6720 7372 633d 2268 7474  i"><img src="htt
+00000c20: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000c30: 2e69 6f2f 7079 7069 2f70 7976 6572 7369  .io/pypi/pyversi
+00000c40: 6f6e 732f 6461 7274 2d74 6f6f 6c73 2220  ons/dart-tools" 
+00000c50: 616c 743d 2253 7570 706f 7274 6564 2050  alt="Supported P
+00000c60: 7974 686f 6e20 5665 7273 696f 6e73 223e  ython Versions">
+00000c70: 3c2f 613e 0a20 2020 203c 6120 6872 6566  </a>.    <a href
+00000c80: 3d22 4c49 4345 4e53 4522 3e3c 696d 6720  ="LICENSE"><img 
+00000c90: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+00000ca0: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
+00000cb0: 7562 2f6c 6963 656e 7365 2f69 7473 2d64  ub/license/its-d
+00000cc0: 6172 742f 6461 7274 2d74 6f6f 6c73 2220  art/dart-tools" 
+00000cd0: 616c 743d 224c 6963 656e 7365 223e 3c2f  alt="License"></
+00000ce0: 613e 0a20 203c 2f70 3e0a 3c2f 6469 763e  a>.  </p>.</div>
+00000cf0: 0a0a 5b44 6172 745d 2868 7474 7073 3a2f  ..[Dart](https:/
+00000d00: 2f69 7473 6461 7274 2e63 6f6d 3f6e 723d  /itsdart.com?nr=
+00000d10: 3129 2069 7320 5072 6f6a 6563 7420 4d61  1) is Project Ma
+00000d20: 6e61 6765 6d65 6e74 206f 6e20 4175 746f  nagement on Auto
+00000d30: 7069 6c6f 742e 0a0a 6064 6172 742d 746f  pilot...`dart-to
+00000d40: 6f6c 7360 2069 7320 7468 6520 4461 7274  ols` is the Dart
+00000d50: 2043 4c49 2061 6e64 2050 7974 686f 6e20   CLI and Python 
+00000d60: 4c69 6272 6172 792e 2049 7420 656e 6162  Library. It enab
+00000d70: 6c65 7320 6469 7265 6374 2069 6e74 6567  les direct integ
+00000d80: 7261 7469 6f6e 2077 6974 6820 4461 7274  ration with Dart
+00000d90: 2074 6872 6f75 6768 2061 2074 6572 6d69   through a termi
+00000da0: 6e61 6c20 434c 4920 6f72 2074 6872 6f75  nal CLI or throu
+00000db0: 6768 2050 7974 686f 6e2e 0a0a 0a23 2320  gh Python....## 
+00000dc0: 5365 7475 700a 0a49 6e20 7468 6520 7465  Setup..In the te
+00000dd0: 726d 696e 616c 2c20 696e 7374 616c 6c20  rminal, install 
+00000de0: 7769 7468 0a60 6060 6261 7368 0a70 6970  with.```bash.pip
+00000df0: 2069 6e73 7461 6c6c 2064 6172 742d 746f   install dart-to
+00000e00: 6f6c 730a 6060 600a 0a54 6865 6e2c 206c  ols.```..Then, l
+00000e10: 6f67 696e 2077 6974 680a 6060 6062 6173  ogin with.```bas
+00000e20: 680a 6461 7274 206c 6f67 696e 0a60 6060  h.dart login.```
+00000e30: 0a0a 0a23 2320 5573 6167 650a 0a23 2323  ...## Usage..###
+00000e40: 2041 7320 6120 434c 490a 0a49 6e20 7468   As a CLI..In th
+00000e50: 6520 7465 726d 696e 616c 2c20 7365 6520  e terminal, see 
+00000e60: 7468 6520 6865 6c70 206d 6573 7361 6765  the help message
+00000e70: 2077 6974 680a 6060 6062 6173 680a 6461   with.```bash.da
+00000e80: 7274 202d 2d68 656c 700a 6060 600a 0a43  rt --help.```..C
+00000e90: 7265 6174 6520 6120 7461 736b 2077 6974  reate a task wit
+00000ea0: 680a 6060 6062 6173 680a 6461 7274 2063  h.```bash.dart c
+00000eb0: 7265 6174 6574 6173 6b20 226e 6577 2074  reatetask "new t
+00000ec0: 6173 6b22 0a60 6060 0a0a 4265 6769 6e20  ask".```..Begin 
+00000ed0: 776f 726b 206f 6e20 6120 7461 736b 2077  work on a task w
+00000ee0: 6974 680a 6060 6062 6173 680a 6461 7274  ith.```bash.dart
+00000ef0: 2062 6567 696e 7461 736b 0a60 6060 0a0a   begintask.```..
+00000f00: 2323 2320 4173 2061 2050 7974 686f 6e20  ### As a Python 
+00000f10: 4c69 6272 6172 790a 0a49 6e20 5079 7468  Library..In Pyth
+00000f20: 6f6e 2c20 7275 6e0a 6060 6070 7974 686f  on, run.```pytho
+00000f30: 6e0a 6672 6f6d 2064 6172 7420 696d 706f  n.from dart impo
+00000f40: 7274 206c 6f67 696e 2c20 6372 6561 7465  rt login, create
+00000f50: 5f74 6173 6b2c 2062 6567 696e 5f74 6173  _task, begin_tas
+00000f60: 6b0a 0a23 206f 6e6c 7920 6e65 6564 6564  k..# only needed
+00000f70: 206f 6e65 2074 696d 650a 6c6f 6769 6e28   one time.login(
+00000f80: 290a 0a63 7265 6174 655f 7461 736b 2822  )..create_task("
+00000f90: 6e65 7720 7461 736b 2229 0a0a 6265 6769  new task")..begi
+00000fa0: 6e5f 7461 736b 2829 0a60 6060 0a0a 2323  n_task().```..##
+00000fb0: 2048 656c 7020 616e 6420 5265 736f 7572   Help and Resour
+00000fc0: 6365 730a 0a2d 205b 486f 6d65 7061 6765  ces..- [Homepage
+00000fd0: 5d28 6874 7470 733a 2f2f 7777 772e 6974  ](https://www.it
+00000fe0: 7364 6172 742e 636f 6d2f 3f6e 723d 3129  sdart.com/?nr=1)
+00000ff0: 0a2d 205b 5765 6220 4170 705d 2868 7474  .- [Web App](htt
+00001000: 7073 3a2f 2f61 7070 2e69 7473 6461 7274  ps://app.itsdart
+00001010: 2e63 6f6d 2f29 0a2d 205b 4865 6c70 2043  .com/).- [Help C
+00001020: 656e 7465 725d 2868 7474 7073 3a2f 2f69  enter](https://i
+00001030: 7473 2d64 6172 742e 6e6f 7469 6f6e 2e73  ts-dart.notion.s
+00001040: 6974 652f 4461 7274 2d48 656c 702d 4365  ite/Dart-Help-Ce
+00001050: 6e74 6572 2d38 3230 3661 3261 6132 3935  nter-8206a2aa295
+00001060: 3634 3936 6638 3938 3862 3762 3332 6364  6496f8988b7b32cd
+00001070: 6364 3230 3529 0a2d 205b 4275 6773 2061  cd205).- [Bugs a
+00001080: 6e64 2046 6561 7475 7265 735d 2868 7474  nd Features](htt
+00001090: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000010a0: 6974 732d 6461 7274 2f64 6172 742d 746f  its-dart/dart-to
+000010b0: 6f6c 732f 6973 7375 6573 290a 2d20 5b4c  ols/issues).- [L
+000010c0: 6962 7261 7279 2053 6f75 7263 655d 2868  ibrary Source](h
+000010d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000010e0: 6d2f 6974 732d 6461 7274 2f64 6172 742d  m/its-dart/dart-
+000010f0: 746f 6f6c 732f 290a 2d20 456d 6169 6c20  tools/).- Email 
+00001100: 7573 2061 7420 5b73 7570 706f 7274 4069  us at [support@i
+00001110: 7473 6461 7274 2e63 6f6d 5d28 6d61 696c  tsdart.com](mail
+00001120: 746f 3a73 7570 706f 7274 4069 7473 6461  to:support@itsda
+00001130: 7274 2e63 6f6d 290a                      rt.com).
```

### Comparing `dart-tools-0.1.1/pyproject.toml` & `dart-tools-0.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dart-tools"
-version = "0.1.1"
+version = "0.1.2"
 description = "The Dart CLI and Python Library"
 readme = "README.md"
 requires-python = ">=3.7"
 
 license = {file = "LICENSE"}
 keywords = ["dart", "cli", "projectmanagement", "taskmanagement"]
 authors = [
@@ -47,7 +47,10 @@
 
 [project.scripts]
 dart = "dart:cli"
 
 [build-system]
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
+
+[tool.setuptools]
+packages = ["dart"]
```

