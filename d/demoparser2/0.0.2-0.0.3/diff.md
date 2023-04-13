# Comparing `tmp/demoparser2-0.0.2-cp39-none-win_amd64.whl.zip` & `tmp/demoparser2-0.0.3-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2119965 bytes, number of entries: 5
--rw-r--r--  4.6 unx     2463 b- defN 23-Apr-12 17:34 demoparser2-0.0.2.dist-info/METADATA
--rw-r--r--  4.6 unx       95 b- defN 23-Apr-12 17:34 demoparser2-0.0.2.dist-info/WHEEL
--rw-r--r--  4.6 unx      127 b- defN 23-Apr-12 17:34 demoparser2/__init__.py
--rwxr-xr-x  4.6 unx  7821312 b- defN 23-Apr-12 17:34 demoparser2/demoparser2.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      399 b- defN 23-Apr-12 17:34 demoparser2-0.0.2.dist-info/RECORD
-5 files, 7824396 bytes uncompressed, 2119227 bytes compressed:  72.9%
+Zip file size: 2506211 bytes, number of entries: 5
+-rw-r--r--  4.6 unx     2245 b- defN 23-Apr-13 21:34 demoparser2-0.0.3.dist-info/METADATA
+-rw-r--r--  4.6 unx      128 b- defN 23-Apr-13 21:34 demoparser2-0.0.3.dist-info/WHEEL
+-rw-r--r--  4.6 unx      127 b- defN 23-Apr-13 21:34 demoparser2/__init__.py
+-rwxr-xr-x  4.6 unx  9783784 b- defN 23-Apr-13 21:34 demoparser2/demoparser2.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  4.6 unx      412 b- defN 23-Apr-13 21:34 demoparser2-0.0.3.dist-info/RECORD
+5 files, 9786696 bytes uncompressed, 2505449 bytes compressed:  74.4%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: demoparser2-0.0.2.dist-info/METADATA
+Filename: demoparser2-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: demoparser2-0.0.2.dist-info/WHEEL
+Filename: demoparser2-0.0.3.dist-info/WHEEL
 Comment: 
 
 Filename: demoparser2/__init__.py
 Comment: 
 
-Filename: demoparser2/demoparser2.cp39-win_amd64.pyd
+Filename: demoparser2/demoparser2.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: demoparser2-0.0.2.dist-info/RECORD
+Filename: demoparser2-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `demoparser2-0.0.2.dist-info/METADATA` & `demoparser2-0.0.3.dist-info/METADATA`

 * *Files 23% similar despite different names*

```diff
@@ -1,85 +1,70 @@
 Metadata-Version: 2.1
 Name: demoparser2
-Version: 0.0.2
+Version: 0.0.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: polars
 Requires-Dist: pyarrow
 Requires-Dist: tqdm
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
-# Demo parser for Counter-Strike 2
-
-
-Work in progress so expect some bugs here and there!
-
-## Install
-```pip install demoparser2```
-
-### Usage:
-Game events
-```python
-from demoparser2 import DemoParser
-
-parser = DemoParser("path_to_demo.dem")
-df = parser.parse_events("player_death")
-```
-
-Tick data (entities)
-```python
-from demoparser2 import DemoParser
-
-wanted_props = ["m_vecX", "m_vecY"]
-
-parser = DemoParser("path_to_demo.dem")
-df = parser.parse_ticks(wanted_props)
-```
-
-Both functions return a Pandas Dataframe.
-
-Example output:
-```
-             m_vecX       m_vecY   tick            steamid        name
-0        649.795044   633.648438      0  76512345678912345      person1
-1        526.207642   794.186157      0  76512345678912345      person2
-2        997.494324   583.692871      0  76512345678912345      person3
-3        958.421570   498.485657      0  76512345678912345      person4
-4        624.525696   556.522217      0  76512345678912345      person5
-...             ...          ...    ...                ...         ...
-913215   924.593140   308.131622  30452  76512345678912345      person6
-913216   598.564514   794.186157  30452  76512345678912345      person7
-913217   329.393677   323.219360  30452  76512345678912345      person8
-913218   526.207642    81.611084  30452  76512345678912345      person9
-913219    36.691650   308.887451  30452  76512345678912345      person10
-```
-(steamids and names are made up in this example)
-
-You can also filter ticks:
-```python
-df = parser.parse_ticks(wanted_props, ticks=[x for x in range(29000, 30000)])
-```
-
-
-
-### Progress:
-
-- [x] Game events
-- [x] Server info
-- [x] Sendtables
-- [x] Serverclasses
-- [x] Header
-- [x] Packet entites
-- [ ] String tables
-
-
-
-
-
-## Acknowledgements
-Without Dotabuff's dota 2 parser manta this would not have been possible. Check it out: https://github.com/dotabuff/manta
-
+# Demo parser for Counter-Strike 2
+
+
+Work in progress so expect some bugs here and there!
+
+## Install
+```pip install demoparser2```
+
+### Usage:
+Game events
+```python
+from demoparser2 import DemoParser
+
+parser = DemoParser("path_to_demo.dem")
+df = parser.parse_events("player_death")
+```
+
+Tick data (entities)
+```python
+from demoparser2 import DemoParser
+
+wanted_props = ["m_vecX", "m_vecY"]
+
+parser = DemoParser("path_to_demo.dem")
+df = parser.parse_ticks(wanted_props)
+```
+
+Both functions return a Pandas Dataframe.
+
+Example output:
+```
+             m_vecX       m_vecY   tick            steamid        name
+0        649.795044   633.648438      0  76512345678912345      person1
+1        526.207642   794.186157      0  76512345678912345      person2
+2        997.494324   583.692871      0  76512345678912345      person3
+3        958.421570   498.485657      0  76512345678912345      person4
+4        624.525696   556.522217      0  76512345678912345      person5
+...             ...          ...    ...                ...         ...
+913215   924.593140   308.131622  30452  76512345678912345      person6
+913216   598.564514   794.186157  30452  76512345678912345      person7
+913217   329.393677   323.219360  30452  76512345678912345      person8
+913218   526.207642    81.611084  30452  76512345678912345      person9
+913219    36.691650   308.887451  30452  76512345678912345      person10
+```
+(steamids and names are made up in this example)
+
+You can also filter ticks:
+```python
+df = parser.parse_ticks(wanted_props, ticks=[x for x in range(29000, 30000)])
+```
+
+
+## Acknowledgements
+Without Dotabuff's dota 2 parser manta this would not have been possible. Check it out: https://github.com/dotabuff/manta
+
 The dota 2 demo format is very similar to CS2 demo format with only a few minor changes.
```

