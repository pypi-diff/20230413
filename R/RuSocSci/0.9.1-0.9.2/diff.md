# Comparing `tmp/RuSocSci-0.9.1-py2.py3-none-any.whl.zip` & `tmp/RuSocSci-0.9.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,12 @@
-Zip file size: 26272 bytes, number of entries: 11
--rwxr-xr-x  2.0 unx      423 b- defN 23-Apr-11 11:57 rusocsci/__init__.py
+Zip file size: 23563 bytes, number of entries: 10
+-rwxr-xr-x  2.0 unx      423 b- defN 23-Apr-13 11:57 rusocsci/__init__.py
 -rwxr-xr-x  2.0 unx     8373 b- defN 19-Jul-05 08:08 rusocsci/buttonbox.py
--rwxr-xr-x  2.0 unx     6802 b- defN 18-Sep-14 07:47 rusocsci/buttonbox2.py
 -rwxr-xr-x  2.0 unx     3935 b- defN 19-Jul-05 08:32 rusocsci/extended.py
 -rwxr-xr-x  2.0 unx     2491 b- defN 19-Jul-04 09:34 rusocsci/joystick.py
--rwxr-xr-x  2.0 unx     9630 b- defN 22-Jun-20 10:59 rusocsci/utils.py
--rwxr-xr-x  2.0 unx    35147 b- defN 23-Apr-11 12:02 RuSocSci-0.9.1.dist-info/LICENSE
--rwxr-xr-x  2.0 unx      934 b- defN 23-Apr-11 12:02 RuSocSci-0.9.1.dist-info/METADATA
--rwxr-xr-x  2.0 unx      110 b- defN 23-Apr-11 12:02 RuSocSci-0.9.1.dist-info/WHEEL
--rwxr-xr-x  2.0 unx        9 b- defN 23-Apr-11 12:02 RuSocSci-0.9.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      852 b- defN 23-Apr-11 12:02 RuSocSci-0.9.1.dist-info/RECORD
-11 files, 68706 bytes uncompressed, 24846 bytes compressed:  63.8%
+-rwxr-xr-x  2.0 unx     9630 b- defN 22-Jun-20 10:54 rusocsci/utils.py
+-rwxr-xr-x  2.0 unx    35147 b- defN 23-Apr-13 11:57 RuSocSci-0.9.2.dist-info/LICENSE
+-rwxr-xr-x  2.0 unx      934 b- defN 23-Apr-13 11:57 RuSocSci-0.9.2.dist-info/METADATA
+-rwxr-xr-x  2.0 unx      110 b- defN 23-Apr-13 11:57 RuSocSci-0.9.2.dist-info/WHEEL
+-rwxr-xr-x  2.0 unx        9 b- defN 23-Apr-13 11:57 RuSocSci-0.9.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      773 b- defN 23-Apr-13 11:57 RuSocSci-0.9.2.dist-info/RECORD
+10 files, 61825 bytes uncompressed, 22257 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -1,34 +1,31 @@
 Filename: rusocsci/__init__.py
 Comment: 
 
 Filename: rusocsci/buttonbox.py
 Comment: 
 
-Filename: rusocsci/buttonbox2.py
-Comment: 
-
 Filename: rusocsci/extended.py
 Comment: 
 
 Filename: rusocsci/joystick.py
 Comment: 
 
 Filename: rusocsci/utils.py
 Comment: 
 
-Filename: RuSocSci-0.9.1.dist-info/LICENSE
+Filename: RuSocSci-0.9.2.dist-info/LICENSE
 Comment: 
 
-Filename: RuSocSci-0.9.1.dist-info/METADATA
+Filename: RuSocSci-0.9.2.dist-info/METADATA
 Comment: 
 
-Filename: RuSocSci-0.9.1.dist-info/WHEEL
+Filename: RuSocSci-0.9.2.dist-info/WHEEL
 Comment: 
 
-Filename: RuSocSci-0.9.1.dist-info/top_level.txt
+Filename: RuSocSci-0.9.2.dist-info/top_level.txt
 Comment: 
 
-Filename: RuSocSci-0.9.1.dist-info/RECORD
+Filename: RuSocSci-0.9.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rusocsci/__init__.py

```diff
@@ -1,12 +1,12 @@
 # Copyright (C) 2013-2022 Wilbert van Ham, Radboud University Nijmegen
 # Distributed under the terms of the GNU General Public License (GPL).
 
 #version info for RuSocSci
-__version__='0.9.1'
+__version__='0.9.2'
 __license__='GNU GPLv3 (or more recent equivalent)'
 __author__='Wilbert van Ham'
 __author_email__='wilbert.vanham@ru.nl'
 __maintainer_email__='wilbert.vanham@ru.nl'
 __url__='https://www.socsci.ru.nl/wilberth/python/rusocsci.html'
```

## Comparing `RuSocSci-0.9.1.dist-info/LICENSE` & `RuSocSci-0.9.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `RuSocSci-0.9.1.dist-info/METADATA` & `RuSocSci-0.9.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RuSocSci
-Version: 0.9.1
+Version: 0.9.2
 Summary: Support package for Radboud University Nijmegen, Faculty of Social Sciences hardware, with PsychoPy-like API.
 Home-page: https://www.socsci.ru.nl/wilberth/python/rusocsci.html
 Author: Wilbert van Ham
 Author-email: w.vanham@socsci.ru.nl
 License: GPLv3+
 Keywords: hardware
 Platform: UNKNOWN
```

## Comparing `RuSocSci-0.9.1.dist-info/RECORD` & `RuSocSci-0.9.2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-rusocsci/__init__.py,sha256=dc7hIujZJZ-X9h4y8SU7sZlSo0RhIytUfdRhnYJodjo,423
+rusocsci/__init__.py,sha256=ziKe6GgycgGA2dIp2JApnX0MALEwkCDrVCPxijVRwg0,423
 rusocsci/buttonbox.py,sha256=SNkApy4G-SC3vhfMvsQYS9IZTXOEXEh0FOvmhkzFwNs,8373
-rusocsci/buttonbox2.py,sha256=APJjgshiwhJIc-dhEFNwsN1DCozv5ycwzbo5Bh-3DXc,6802
 rusocsci/extended.py,sha256=n-0Ne0ayVeOmnsXUsYY12tT-91cfVt3lEM5QAVLlI_U,3935
 rusocsci/joystick.py,sha256=snTMgCOcPAUyb8bl-x6sZ5X8r5ifZKcO5k_tLzpw2t0,2491
 rusocsci/utils.py,sha256=e9UoWMSy4XNqOfK1wrf1rh9pk0anGrMP_12aIUxngE8,9630
-RuSocSci-0.9.1.dist-info/LICENSE,sha256=jOtLnuWt7d5Hsx6XXB2QxzrSe2sWWh3NgMfFRetluQM,35147
-RuSocSci-0.9.1.dist-info/METADATA,sha256=7fo1dVKvD0_rFOBNKSY4uDQNEfJMcU0i1eQcimrWioE,934
-RuSocSci-0.9.1.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-RuSocSci-0.9.1.dist-info/top_level.txt,sha256=bB8ODObfJoZvAt61cOq0gTlEJu4FWQMpjUa4KQhTbzg,9
-RuSocSci-0.9.1.dist-info/RECORD,,
+RuSocSci-0.9.2.dist-info/LICENSE,sha256=jOtLnuWt7d5Hsx6XXB2QxzrSe2sWWh3NgMfFRetluQM,35147
+RuSocSci-0.9.2.dist-info/METADATA,sha256=wLW_mh-efn-2P4BOu8kU4g8Qn5v4YFwom9nT4-f5jmM,934
+RuSocSci-0.9.2.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+RuSocSci-0.9.2.dist-info/top_level.txt,sha256=bB8ODObfJoZvAt61cOq0gTlEJu4FWQMpjUa4KQhTbzg,9
+RuSocSci-0.9.2.dist-info/RECORD,,
```

