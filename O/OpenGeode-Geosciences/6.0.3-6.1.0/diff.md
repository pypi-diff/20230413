# Comparing `tmp/OpenGeode_Geosciences-6.0.3-cp39-cp39-win_amd64.whl.zip` & `tmp/OpenGeode_Geosciences-6.1.0-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4562 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat       76 b- defN 23-Apr-04 14:23 opengeode_geosciences/__init__.py
--rw-rw-rw-  2.0 fat     1243 b- defN 23-Apr-04 14:23 opengeode_geosciences/geosciences.py
--rw-rw-rw-  2.0 fat       96 b- defN 23-Apr-04 14:25 opengeode_geosciences/opengeode_geosciences.py
--rw-rw-rw-  2.0 fat     1242 b- defN 23-Apr-04 14:25 opengeode_geosciences/opengeode_geosciences_geosciences.py
--rw-rw-rw-  2.0 fat     3183 b- defN 23-Apr-04 14:25 OpenGeode_Geosciences-6.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-04 14:25 OpenGeode_Geosciences-6.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       22 b- defN 23-Apr-04 14:25 OpenGeode_Geosciences-6.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      752 b- defN 23-Apr-04 14:25 OpenGeode_Geosciences-6.0.3.dist-info/RECORD
-8 files, 6714 bytes uncompressed, 3218 bytes compressed:  52.1%
+Zip file size: 435020 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       73 b- defN 23-Apr-13 07:13 opengeode_geosciences/__init__.py
+-rw-r--r--  2.0 unx     1224 b- defN 23-Apr-13 07:13 opengeode_geosciences/geosciences.py
+-rwxr-xr-x  2.0 unx  1863696 b- defN 23-Apr-13 07:13 opengeode_geosciences/lib64/libOpenGeode-Geosciences_geosciences.so
+-rwxr-xr-x  2.0 unx   483904 b- defN 23-Apr-13 07:13 opengeode_geosciences/lib64/opengeode_geosciences_py_geosciences.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx     3138 b- defN 23-Apr-13 07:13 OpenGeode_Geosciences-6.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      103 b- defN 23-Apr-13 07:13 OpenGeode_Geosciences-6.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       22 b- defN 23-Apr-13 07:13 OpenGeode_Geosciences-6.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      817 b- defN 23-Apr-13 07:13 OpenGeode_Geosciences-6.1.0.dist-info/RECORD
+8 files, 2352977 bytes uncompressed, 433560 bytes compressed:  81.6%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: opengeode_geosciences/__init__.py
 Comment: 
 
 Filename: opengeode_geosciences/geosciences.py
 Comment: 
 
-Filename: opengeode_geosciences/opengeode_geosciences.py
+Filename: opengeode_geosciences/lib64/libOpenGeode-Geosciences_geosciences.so
 Comment: 
 
-Filename: opengeode_geosciences/opengeode_geosciences_geosciences.py
+Filename: opengeode_geosciences/lib64/opengeode_geosciences_py_geosciences.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: OpenGeode_Geosciences-6.0.3.dist-info/METADATA
+Filename: OpenGeode_Geosciences-6.1.0.dist-info/METADATA
 Comment: 
 
-Filename: OpenGeode_Geosciences-6.0.3.dist-info/WHEEL
+Filename: OpenGeode_Geosciences-6.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: OpenGeode_Geosciences-6.0.3.dist-info/top_level.txt
+Filename: OpenGeode_Geosciences-6.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: OpenGeode_Geosciences-6.0.3.dist-info/RECORD
+Filename: OpenGeode_Geosciences-6.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## opengeode_geosciences/__init__.py

 * *Ordering differences only*

```diff
@@ -1,3 +1,3 @@
-## Copyright (c) 2019 - 2023 Geode-solutions
-
-from .geosciences import *
+## Copyright (c) 2019 - 2023 Geode-solutions
+
+from .geosciences import *
```

## opengeode_geosciences/geosciences.py

```diff
@@ -1,25 +1,25 @@
-# Copyright (c) 2019 - 2023 Geode-solutions
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in
-# all copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
-import opengeode
-
-from .opengeode_geosciences_py_geosciences import *
-
-OpenGeodeGeosciencesGeosciences.initialize()
+# Copyright (c) 2019 - 2023 Geode-solutions
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+import opengeode
+
+from .lib64.opengeode_geosciences_py_geosciences import *
+
+OpenGeodeGeosciencesGeosciences.initialize()
```

## Comparing `OpenGeode_Geosciences-6.0.3.dist-info/METADATA` & `OpenGeode_Geosciences-6.1.0.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,74 +1,72 @@
-Metadata-Version: 2.1
-Name: OpenGeode-Geosciences
-Version: 6.0.3
-Summary: OpenGeode module for Geosciences
-Home-page: https://github.com/Geode-solutions/OpenGeode-Geosciences
-Author: Geode-solutions
-Author-email: contact@geode-solutions.com
-License: MIT
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
-<h1 align="center">OpenGeode-Geosciences<sup><i>by Geode-solutions</i></sup></h1>
-<h3 align="center">OpenGeode module for Geosciences</h3>
-
-<p align="center">
-  <img src="https://github.com/Geode-solutions/OpenGeode-Geosciences/workflows/CI/badge.svg" alt="Build Status">
-  <img src="https://github.com/Geode-solutions/OpenGeode-Geosciences/workflows/CD/badge.svg" alt="Deploy Status">
-  <img src="https://codecov.io/gh/Geode-solutions/OpenGeode-Geosciences/branch/master/graph/badge.svg" alt="Coverage Status">
-  <img src="https://img.shields.io/github/release/Geode-solutions/OpenGeode-Geosciences.svg" alt="Version">
-  <img src="https://img.shields.io/pypi/v/opengeode-geosciences" alt="PyPI" >
-</p>
-
-<p align="center">
-  <img src="https://img.shields.io/static/v1?label=Windows&logo=windows&logoColor=white&message=support&color=success" alt="Windows support">
-  <img src="https://img.shields.io/static/v1?label=Ubuntu&logo=Ubuntu&logoColor=white&message=support&color=success" alt="Ubuntu support">
-  <img src="https://img.shields.io/static/v1?label=Red%20Hat&logo=Red-Hat&logoColor=white&message=support&color=success" alt="Red Hat support">
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
-</p>
-
----
-
-## Introduction
-
-OpenGeode-Geosciences is a module of [OpenGeode] provides data structures for geological models and geological objects.
-
-[OpenGeode]: https://github.com/Geode-solutions/OpenGeode
-
-
-## Documentation
-
-To check out our live documentation, visit [docs.geode-solutions.com](https://docs.geode-solutions.com).
-
-Installing OpenGeode-Geosciences is done:
- * either, by compiling the C++ source.
- * or, by using pip command ```pip install OpenGeode-Geosciences``` and add ```import opengeode_geosciences``` in your Python script.
-
-
-## Questions
-For questions and support please use the official [slack](https://opengeode-slack-invite.herokuapp.com) and go to the channel #geosciences. The issue list of this repo is exclusively for bug reports and feature requests. 
-
-
-## Changelog
-
-Detailed changes for each release are documented in the [release notes](https://github.com/Geode-solutions/OpenGeode-Geosciences/releases).
-
-
-## License
-
-[MIT](https://opensource.org/licenses/MIT)
-
-Copyright (c) 2019 - 2023, Geode-solutions
-
-
+Metadata-Version: 2.1
+Name: OpenGeode-Geosciences
+Version: 6.1.0
+Summary: OpenGeode module for Geosciences
+Home-page: https://github.com/Geode-solutions/OpenGeode-Geosciences
+Author: Geode-solutions
+Author-email: contact@geode-solutions.com
+License: MIT
+Description-Content-Type: text/markdown
+Requires-Dist: opengeode-core (==13.*,>=13.4.15)
+
+<h1 align="center">OpenGeode-Geosciences<sup><i>by Geode-solutions</i></sup></h1>
+<h3 align="center">OpenGeode module for Geosciences</h3>
+
+<p align="center">
+  <img src="https://github.com/Geode-solutions/OpenGeode-Geosciences/workflows/CI/badge.svg" alt="Build Status">
+  <img src="https://github.com/Geode-solutions/OpenGeode-Geosciences/workflows/CD/badge.svg" alt="Deploy Status">
+  <img src="https://codecov.io/gh/Geode-solutions/OpenGeode-Geosciences/branch/master/graph/badge.svg" alt="Coverage Status">
+  <img src="https://img.shields.io/github/release/Geode-solutions/OpenGeode-Geosciences.svg" alt="Version">
+  <img src="https://img.shields.io/pypi/v/opengeode-geosciences" alt="PyPI" >
+</p>
+
+<p align="center">
+  <img src="https://img.shields.io/static/v1?label=Windows&logo=windows&logoColor=white&message=support&color=success" alt="Windows support">
+  <img src="https://img.shields.io/static/v1?label=Ubuntu&logo=Ubuntu&logoColor=white&message=support&color=success" alt="Ubuntu support">
+  <img src="https://img.shields.io/static/v1?label=Red%20Hat&logo=Red-Hat&logoColor=white&message=support&color=success" alt="Red Hat support">
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
+</p>
+
+---
+
+## Introduction
+
+OpenGeode-Geosciences is a module of [OpenGeode] provides data structures for geological models and geological objects.
+
+[OpenGeode]: https://github.com/Geode-solutions/OpenGeode
+
+
+## Documentation
+
+To check out our live documentation, visit [docs.geode-solutions.com](https://docs.geode-solutions.com).
+
+Installing OpenGeode-Geosciences is done:
+ * either, by compiling the C++ source.
+ * or, by using pip command ```pip install OpenGeode-Geosciences``` and add ```import opengeode_geosciences``` in your Python script.
+
+
+## Questions
+For questions and support please use the official [slack](https://opengeode-slack-invite.herokuapp.com) and go to the channel #geosciences. The issue list of this repo is exclusively for bug reports and feature requests. 
+
+
+## Changelog
+
+Detailed changes for each release are documented in the [release notes](https://github.com/Geode-solutions/OpenGeode-Geosciences/releases).
+
+
+## License
+
+[MIT](https://opensource.org/licenses/MIT)
+
+Copyright (c) 2019 - 2023, Geode-solutions
```

### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: OpenGeode-Geosciences Version: 6.0.3 Summary:
+Metadata-Version: 2.1 Name: OpenGeode-Geosciences Version: 6.1.0 Summary:
 OpenGeode module for Geosciences Home-page: https://github.com/Geode-solutions/
 OpenGeode-Geosciences Author: Geode-solutions Author-email: contact@geode-
-solutions.com License: MIT Platform: UNKNOWN Description-Content-Type: text/
-markdown
+solutions.com License: MIT Description-Content-Type: text/markdown Requires-
+Dist: opengeode-core (==13.*,>=13.4.15)
              ****** OpenGeode-Geosciencesby Geode-solutions ******
                   **** OpenGeode module for Geosciences ****
        [Build Status] [Deploy Status] [Coverage Status] [Version] [PyPI]
              [Windows support] [Ubuntu support] [Red Hat support]
          [Language] [License] [Semantic-release] [Slack_invite] [DOI]
 --- ## Introduction OpenGeode-Geosciences is a module of [OpenGeode] provides
 data structures for geological models and geological objects. [OpenGeode]:
```

## Comparing `OpenGeode_Geosciences-6.0.3.dist-info/RECORD` & `OpenGeode_Geosciences-6.1.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-opengeode_geosciences/__init__.py,sha256=3gfi2_ujUn4X-L5usd1bmg_nN2fa3eELZmWPrURzUKA,76
-opengeode_geosciences/geosciences.py,sha256=wEhuNK86vYBlUrHJmy-jUiEIvpcT3fHACs2Czej0woQ,1243
-opengeode_geosciences/opengeode_geosciences.py,sha256=9F8WfPRS1BKmAZSI7E8wxFGjVAGvZlNgF2fFob-2hjo,96
-opengeode_geosciences/opengeode_geosciences_geosciences.py,sha256=JcJJfMtD2aj_jdsfKd5bOE2woa1WQYNL-qM3kXfuhgQ,1242
-OpenGeode_Geosciences-6.0.3.dist-info/METADATA,sha256=FwfZB07kUaBj44DNNB6-C6oINIdhPHqP36ZCb9iT8qw,3183
-OpenGeode_Geosciences-6.0.3.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-OpenGeode_Geosciences-6.0.3.dist-info/top_level.txt,sha256=eFBaUchohZc70xqscdwdB_yif7gMPIL5JXdcDqoHasU,22
-OpenGeode_Geosciences-6.0.3.dist-info/RECORD,,
+opengeode_geosciences/__init__.py,sha256=onsTNKTic8V09z-uK2srd8sWWdju5AnB-axE1rTwwBA,73
+opengeode_geosciences/geosciences.py,sha256=omzZkQuC779C40a-l_Z_RoKMTXxcBBrdlxfLmH9aNjE,1224
+opengeode_geosciences/lib64/libOpenGeode-Geosciences_geosciences.so,sha256=y7Zmx0xhwYxvom0tCEGzs3CfD9QF00WYn7OFj1ubfEY,1863696
+opengeode_geosciences/lib64/opengeode_geosciences_py_geosciences.cpython-39-x86_64-linux-gnu.so,sha256=7I4O8i5Sy2o6qraPQICf0s_whFURmtS7-MEB29PiH04,483904
+OpenGeode_Geosciences-6.1.0.dist-info/METADATA,sha256=IEiHn_naFOPgWsys1JfgmzKvNSinWCQYC3FhbC_UOSU,3138
+OpenGeode_Geosciences-6.1.0.dist-info/WHEEL,sha256=3oXbtF4vYwmQyf0LQIagKtl0VO3gP86556qKiLb0bDc,103
+OpenGeode_Geosciences-6.1.0.dist-info/top_level.txt,sha256=eFBaUchohZc70xqscdwdB_yif7gMPIL5JXdcDqoHasU,22
+OpenGeode_Geosciences-6.1.0.dist-info/RECORD,,
```

