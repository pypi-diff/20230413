# Comparing `tmp/Geode_Numerics-2.0.0-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Numerics-3.0.0-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,14 @@
-Zip file size: 2828065 bytes, number of entries: 20
--rw-rw-rw-  2.0 fat      104 b- defN 23-Apr-13 09:01 geode_numerics/__init__.py
--rw-rw-rw-  2.0 fat      207 b- defN 23-Apr-13 09:01 geode_numerics/scalar_function.py
--rw-rw-rw-  2.0 fat      192 b- defN 23-Apr-13 09:01 geode_numerics/surface.py
--rw-rw-rw-  2.0 fat  2269184 b- defN 23-Apr-13 09:02 geode_numerics/bin/Geode-Numerics_frame_field.dll
--rw-rw-rw-  2.0 fat  2150400 b- defN 23-Apr-13 09:02 geode_numerics/bin/Geode-Numerics_scalar_function.dll
--rw-rw-rw-  2.0 fat    60416 b- defN 23-Apr-13 09:02 geode_numerics/bin/Geode-Numerics_surface.dll
--rw-rw-rw-  2.0 fat   317864 b- defN 23-Apr-13 09:02 geode_numerics/bin/concrt140.dll
--rw-rw-rw-  2.0 fat   181760 b- defN 23-Apr-13 09:02 geode_numerics/bin/geode_numerics_py_scalar_function.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   130560 b- defN 23-Apr-13 09:02 geode_numerics/bin/geode_numerics_py_surface.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   566704 b- defN 23-Apr-13 09:02 geode_numerics/bin/msvcp140.dll
--rw-rw-rw-  2.0 fat    23944 b- defN 23-Apr-13 09:02 geode_numerics/bin/msvcp140_1.dll
--rw-rw-rw-  2.0 fat   186800 b- defN 23-Apr-13 09:02 geode_numerics/bin/msvcp140_2.dll
--rw-rw-rw-  2.0 fat    57264 b- defN 23-Apr-13 09:02 geode_numerics/bin/msvcp140_atomic_wait.dll
--rw-rw-rw-  2.0 fat    21424 b- defN 23-Apr-13 09:02 geode_numerics/bin/msvcp140_codecvt_ids.dll
--rw-rw-rw-  2.0 fat    98224 b- defN 23-Apr-13 09:02 geode_numerics/bin/vcruntime140.dll
--rw-rw-rw-  2.0 fat    37256 b- defN 23-Apr-13 09:02 geode_numerics/bin/vcruntime140_1.dll
--rw-rw-rw-  2.0 fat     2285 b- defN 23-Apr-13 09:02 Geode_Numerics-2.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-13 09:02 Geode_Numerics-2.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-Apr-13 09:02 Geode_Numerics-2.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1910 b- defN 23-Apr-13 09:02 Geode_Numerics-2.0.0.dist-info/RECORD
-20 files, 6106613 bytes uncompressed, 2824907 bytes compressed:  53.7%
+Zip file size: 2713165 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      100 b- defN 23-Apr-13 12:57 geode_numerics/__init__.py
+-rw-r--r--  2.0 unx      207 b- defN 23-Apr-13 12:57 geode_numerics/scalar_function.py
+-rw-r--r--  2.0 unx      192 b- defN 23-Apr-13 12:57 geode_numerics/surface.py
+-rwxr-xr-x  2.0 unx   208448 b- defN 23-Apr-13 12:58 geode_numerics/lib64/geode_numerics_py_scalar_function.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   130456 b- defN 23-Apr-13 12:58 geode_numerics/lib64/geode_numerics_py_surface.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx  3167368 b- defN 23-Apr-13 12:58 geode_numerics/lib64/libGeode-Numerics_frame_field.so
+-rwxr-xr-x  2.0 unx  3083248 b- defN 23-Apr-13 12:58 geode_numerics/lib64/libGeode-Numerics_scalar_function.so
+-rwxr-xr-x  2.0 unx    97280 b- defN 23-Apr-13 12:58 geode_numerics/lib64/libGeode-Numerics_surface.so
+-rw-r--r--  2.0 unx     2220 b- defN 23-Apr-13 12:58 Geode_Numerics-3.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      103 b- defN 23-Apr-13 12:58 Geode_Numerics-3.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Apr-13 12:58 Geode_Numerics-3.0.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1196 b- defN 23-Apr-13 12:58 Geode_Numerics-3.0.0.dist-info/RECORD
+12 files, 6690833 bytes uncompressed, 2711109 bytes compressed:  59.5%
```

## zipnote {}

```diff
@@ -3,59 +3,35 @@
 
 Filename: geode_numerics/scalar_function.py
 Comment: 
 
 Filename: geode_numerics/surface.py
 Comment: 
 
-Filename: geode_numerics/bin/Geode-Numerics_frame_field.dll
+Filename: geode_numerics/lib64/geode_numerics_py_scalar_function.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: geode_numerics/bin/Geode-Numerics_scalar_function.dll
+Filename: geode_numerics/lib64/geode_numerics_py_surface.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: geode_numerics/bin/Geode-Numerics_surface.dll
+Filename: geode_numerics/lib64/libGeode-Numerics_frame_field.so
 Comment: 
 
-Filename: geode_numerics/bin/concrt140.dll
+Filename: geode_numerics/lib64/libGeode-Numerics_scalar_function.so
 Comment: 
 
-Filename: geode_numerics/bin/geode_numerics_py_scalar_function.cp39-win_amd64.pyd
+Filename: geode_numerics/lib64/libGeode-Numerics_surface.so
 Comment: 
 
-Filename: geode_numerics/bin/geode_numerics_py_surface.cp39-win_amd64.pyd
+Filename: Geode_Numerics-3.0.0.dist-info/METADATA
 Comment: 
 
-Filename: geode_numerics/bin/msvcp140.dll
+Filename: Geode_Numerics-3.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: geode_numerics/bin/msvcp140_1.dll
+Filename: Geode_Numerics-3.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: geode_numerics/bin/msvcp140_2.dll
-Comment: 
-
-Filename: geode_numerics/bin/msvcp140_atomic_wait.dll
-Comment: 
-
-Filename: geode_numerics/bin/msvcp140_codecvt_ids.dll
-Comment: 
-
-Filename: geode_numerics/bin/vcruntime140.dll
-Comment: 
-
-Filename: geode_numerics/bin/vcruntime140_1.dll
-Comment: 
-
-Filename: Geode_Numerics-2.0.0.dist-info/METADATA
-Comment: 
-
-Filename: Geode_Numerics-2.0.0.dist-info/WHEEL
-Comment: 
-
-Filename: Geode_Numerics-2.0.0.dist-info/top_level.txt
-Comment: 
-
-Filename: Geode_Numerics-2.0.0.dist-info/RECORD
+Filename: Geode_Numerics-3.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_numerics/__init__.py

 * *Ordering differences only*

```diff
@@ -1,4 +1,4 @@
-## Copyright (c) 2019 - 2023 Geode-solutions
-
-from .surface import *
-from .scalar_function import *
+## Copyright (c) 2019 - 2023 Geode-solutions
+
+from .surface import *
+from .scalar_function import *
```

## geode_numerics/scalar_function.py

```diff
@@ -1,9 +1,9 @@
-#
-# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import geode_common
-
-from .bin.geode_numerics_py_scalar_function import *
-NumericsScalarFunction.initialize()
+#
+# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import geode_common
+
+from .lib64.geode_numerics_py_scalar_function import *
+NumericsScalarFunctionLibrary.initialize()
```

## geode_numerics/surface.py

```diff
@@ -1,9 +1,9 @@
-#
-# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import geode_common
-
-from .bin.geode_numerics_py_surface import *
-NumericsSurface.initialize()
+#
+# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import geode_common
+
+from .lib64.geode_numerics_py_surface import *
+NumericsSurfaceLibrary.initialize()
```

## Comparing `Geode_Numerics-2.0.0.dist-info/METADATA` & `Geode_Numerics-3.0.0.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,41 @@
-Metadata-Version: 2.1
-Name: Geode-Numerics
-Version: 2.0.0
-Summary: Numerical algorithm module
-Home-page: https://github.com/Geode-solutions/Geode-Numerics
-Author: Geode-solutions
-Author-email: contact@geode-solutions.com
-License: Proprietary
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-Requires-Dist: geode-common (==24.*,>=24.0.5)
-Requires-Dist: opengeode-core (==13.*,>=13.4.15)
-
-<h1 align="center">Geode-Numerics<sup><i>by Geode-solutions</i></sup></h1>
-<h3 align="center">Numerics OpenGeode module</h3>
-
-<p align="center">
-  <img src="https://github.com/Geode-solutions/Geode-Numerics_private/workflows/CI/badge.svg" alt="Build Status">
-  <img src="https://github.com/Geode-solutions/Geode-Numerics_private/workflows/CD/badge.svg" alt="Deploy Status">
-  <img src="https://codecov.io/gh/Geode-solutions/Geode-Numerics_private/branch/master/graph/badge.svg" alt="Coverage Status">
-  <img src="https://img.shields.io/github/release/Geode-solutions/Geode-Numerics_private.svg" alt="Version">
-</p>
-
-<p align="center">
-  <img src="https://img.shields.io/static/v1?label=Windows&logo=windows&logoColor=white&message=support&color=success" alt="Windows support">
-  <img src="https://img.shields.io/static/v1?label=Ubuntu&logo=Ubuntu&logoColor=white&message=support&color=success" alt="Ubuntu support">
-  <img src="https://img.shields.io/static/v1?label=Red%20Hat&logo=Red-Hat&logoColor=white&message=support&color=success" alt="Red Hat support">
-  <img src="https://img.shields.io/static/v1?label=macOS&logo=apple&logoColor=white&message=support&color=success" alt="macOS support">
-</p>
-
-<p align="center">
-  <img src="https://img.shields.io/badge/C%2B%2B-11-blue.svg" alt="Language">
-  <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License">
-  <img src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg" alt="Semantic-release">
-  <a href="https://opengeode-slack-invite.herokuapp.com">
-    <img src="https://opengeode-slack-invite.herokuapp.com/badge.svg" alt="Slack invite">
-  </a>
-  <a href="https://doi.org/10.5281/zenodo.3610370">
-    <img src="https://zenodo.org/badge/DOI/10.5281/zenodo.3610370.svg" alt="DOI">
-  </a>
-
-Copyright (c) 2019 - 2023, Geode-solutions
-
-
+Metadata-Version: 2.1
+Name: Geode-Numerics
+Version: 3.0.0
+Summary: Numerical algorithm module
+Home-page: https://github.com/Geode-solutions/Geode-Numerics
+Author: Geode-solutions
+Author-email: contact@geode-solutions.com
+License: Proprietary
+Description-Content-Type: text/markdown
+Requires-Dist: geode-common (==25.*,>=25.0.0)
+Requires-Dist: opengeode-core (==14.*,>=14.0.0)
+
+<h1 align="center">Geode-Numerics<sup><i>by Geode-solutions</i></sup></h1>
+<h3 align="center">Numerics OpenGeode module</h3>
+
+<p align="center">
+  <img src="https://github.com/Geode-solutions/Geode-Numerics_private/workflows/CI/badge.svg" alt="Build Status">
+  <img src="https://github.com/Geode-solutions/Geode-Numerics_private/workflows/CD/badge.svg" alt="Deploy Status">
+  <img src="https://codecov.io/gh/Geode-solutions/Geode-Numerics_private/branch/master/graph/badge.svg" alt="Coverage Status">
+  <img src="https://img.shields.io/github/release/Geode-solutions/Geode-Numerics_private.svg" alt="Version">
+</p>
+
+<p align="center">
+  <img src="https://img.shields.io/static/v1?label=Windows&logo=windows&logoColor=white&message=support&color=success" alt="Windows support">
+  <img src="https://img.shields.io/static/v1?label=Ubuntu&logo=Ubuntu&logoColor=white&message=support&color=success" alt="Ubuntu support">
+  <img src="https://img.shields.io/static/v1?label=Red%20Hat&logo=Red-Hat&logoColor=white&message=support&color=success" alt="Red Hat support">
+  <img src="https://img.shields.io/static/v1?label=macOS&logo=apple&logoColor=white&message=support&color=success" alt="macOS support">
+</p>
+
+<p align="center">
+  <img src="https://img.shields.io/badge/C%2B%2B-11-blue.svg" alt="Language">
+  <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License">
+  <img src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg" alt="Semantic-release">
+  <a href="https://opengeode-slack-invite.herokuapp.com">
+    <img src="https://opengeode-slack-invite.herokuapp.com/badge.svg" alt="Slack invite">
+  </a>
+  <a href="https://doi.org/10.5281/zenodo.3610370">
+    <img src="https://zenodo.org/badge/DOI/10.5281/zenodo.3610370.svg" alt="DOI">
+  </a>
+
+Copyright (c) 2019 - 2023, Geode-solutions
```

### html2text {}

```diff
@@ -1,12 +1,11 @@
-Metadata-Version: 2.1 Name: Geode-Numerics Version: 2.0.0 Summary: Numerical
+Metadata-Version: 2.1 Name: Geode-Numerics Version: 3.0.0 Summary: Numerical
 algorithm module Home-page: https://github.com/Geode-solutions/Geode-Numerics
 Author: Geode-solutions Author-email: contact@geode-solutions.com License:
-Proprietary Platform: UNKNOWN Description-Content-Type: text/markdown Requires-
-Dist: geode-common (==24.*,>=24.0.5) Requires-Dist: opengeode-core
-(==13.*,>=13.4.15)
+Proprietary Description-Content-Type: text/markdown Requires-Dist: geode-common
+(==25.*,>=25.0.0) Requires-Dist: opengeode-core (==14.*,>=14.0.0)
                 ****** Geode-Numericsby Geode-solutions ******
                       **** Numerics OpenGeode module ****
           [Build Status] [Deploy Status] [Coverage Status] [Version]
      [Windows support] [Ubuntu support] [Red Hat support] [macOS support]
 [Language] [License] [Semantic-release] [Slack_invite] [DOI] Copyright (c) 2019
                            - 2023, Geode-solutions
```

## Comparing `Geode_Numerics-2.0.0.dist-info/RECORD` & `Geode_Numerics-3.0.0.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,12 @@
-geode_numerics/__init__.py,sha256=Gci8zlJMKSi7fA96eH5f7TUEJ7lz2jQAGc-cUNuSTqU,104
-geode_numerics/scalar_function.py,sha256=27ems4Kk_Cpy70C0TGhDLI4ROAc4gaEN0hzMg-8r9dI,207
-geode_numerics/surface.py,sha256=AUqBLBwapmiZ7gv8YCM1LKm3JsTLL1WU_TjBVh8Tru4,192
-geode_numerics/bin/Geode-Numerics_frame_field.dll,sha256=UQ1zPi_N4bJCekihhJOAkjXOeclzw3S7-_UZ0_Ur6yI,2269184
-geode_numerics/bin/Geode-Numerics_scalar_function.dll,sha256=e-9HVYbULhsQn1XMWeOY1YzHJqUOdZAEs2VoF3j11KY,2150400
-geode_numerics/bin/Geode-Numerics_surface.dll,sha256=dQPHw5xx_8I2jGjAvPHvBJlNRLwZ6QZC7mgFMgNASq8,60416
-geode_numerics/bin/concrt140.dll,sha256=VzIpoH84q50vwuGluY6SQ7mzkQAyMYDIOtfdr5ju5Go,317864
-geode_numerics/bin/geode_numerics_py_scalar_function.cp39-win_amd64.pyd,sha256=d1xmdYZ0U_tPfF3OAzWOFU43NXWnfqw-rZNrz9kutEI,181760
-geode_numerics/bin/geode_numerics_py_surface.cp39-win_amd64.pyd,sha256=Gkw-KddAvzcg4LBKddP1M5a1NngY_3q18VTTwxG7b6I,130560
-geode_numerics/bin/msvcp140.dll,sha256=n-5vNlR9b26nygM4ZVVV26a7D3mLxgM00puU0VR9pNo,566704
-geode_numerics/bin/msvcp140_1.dll,sha256=hzGpPlGcJZXJ_UiebZrAfpZESMDaHI7p7lAKeYlIJhc,23944
-geode_numerics/bin/msvcp140_2.dll,sha256=Nmr44HHwBNpdlagypGsuiCGo4ClDQKk_fJXPSMRBBn4,186800
-geode_numerics/bin/msvcp140_atomic_wait.dll,sha256=xhoocR-Mbpv9SHnPX1OwE9ZTutrTCKvj6IfGlLIj1vA,57264
-geode_numerics/bin/msvcp140_codecvt_ids.dll,sha256=m0X9BpvQB22Kv-t8PDCh9cX8jnEkAXhTqT2DGjRsPSE,21424
-geode_numerics/bin/vcruntime140.dll,sha256=nStA8DlcxdG01eoXuElwwplx1EjDcQRnbbV3WG1K0bE,98224
-geode_numerics/bin/vcruntime140_1.dll,sha256=NASKuqBw7ME7MYzqMUJfTKPt0TPTUDGKxlJZ5gWMizI,37256
-Geode_Numerics-2.0.0.dist-info/METADATA,sha256=2ROb29Q-btZ7XQtiWbizkvM3hjLs8cP-7g68BUfYy3w,2285
-Geode_Numerics-2.0.0.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-Geode_Numerics-2.0.0.dist-info/top_level.txt,sha256=btImDcRfDC3xFt4EkvH1wXfhk4t1qY8t71xeEbMo-qk,15
-Geode_Numerics-2.0.0.dist-info/RECORD,,
+geode_numerics/__init__.py,sha256=3EtxJT9ddldsaNE94oAdYASutM9BY_te64OtXiL1rVc,100
+geode_numerics/scalar_function.py,sha256=Bq-wj-txSO3oSEiAZPpDI3XYU-dudxjSrj_S0hPnF1Q,207
+geode_numerics/surface.py,sha256=S-muREDcs8u0ADae1jtx64-w0PfcQ8vbNgobQs0SuRM,192
+geode_numerics/lib64/geode_numerics_py_scalar_function.cpython-39-x86_64-linux-gnu.so,sha256=fytO4fppxh6-JOijN-QajvrglFRMQErYFDZ26g5lweY,208448
+geode_numerics/lib64/geode_numerics_py_surface.cpython-39-x86_64-linux-gnu.so,sha256=nDA_5cj7LRRHbbpSHb-w7hJAsgeq8ul4rgSMgalsoek,130456
+geode_numerics/lib64/libGeode-Numerics_frame_field.so,sha256=PBEU5yxXvyN-t6JEOWFDnKBgcrJhH8ZpHj10nCUFVkA,3167368
+geode_numerics/lib64/libGeode-Numerics_scalar_function.so,sha256=u5EE9_pjNExh0fYNSPt0wTSqJj25J16bhLIHpp5DqbQ,3083248
+geode_numerics/lib64/libGeode-Numerics_surface.so,sha256=iKVC5cAWBVOcR_WBB6up9SlCdQ-ILvrg778S2JJM-dA,97280
+Geode_Numerics-3.0.0.dist-info/METADATA,sha256=kutpyQzU3pPyrt2OWBxvVGsylWI8x91UwzGWnNCDrQc,2220
+Geode_Numerics-3.0.0.dist-info/WHEEL,sha256=3oXbtF4vYwmQyf0LQIagKtl0VO3gP86556qKiLb0bDc,103
+Geode_Numerics-3.0.0.dist-info/top_level.txt,sha256=btImDcRfDC3xFt4EkvH1wXfhk4t1qY8t71xeEbMo-qk,15
+Geode_Numerics-3.0.0.dist-info/RECORD,,
```

