# Comparing `tmp/vizelec-0.1.1.tar.gz` & `tmp/vizelec-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vizelec-0.1.1.tar", max compression
+gzip compressed data, was "vizelec-0.1.2.tar", max compression
```

## Comparing `vizelec-0.1.1.tar` & `vizelec-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      891 2023-04-13 09:16:53.485708 vizelec-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1294 2023-04-13 09:14:39.715711 vizelec-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-03-16 11:27:13.722130 vizelec-0.1.1/vizelec/__init__.py
--rw-r--r--   0        0        0      221 2023-04-13 09:14:03.795136 vizelec-0.1.1/vizelec/main.py
--rw-r--r--   0        0        0      796 2023-04-13 09:10:17.425371 vizelec-0.1.1/vizelec/pinout.py
--rw-r--r--   0        0        0     3290 2023-04-13 09:09:59.406444 vizelec-0.1.1/vizelec/spice.py
--rw-r--r--   0        0        0     1945 1970-01-01 00:00:00.000000 vizelec-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      891 2023-04-13 10:00:37.299258 vizelec-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1294 2023-04-13 09:14:39.715711 vizelec-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-03-16 11:27:13.722130 vizelec-0.1.2/vizelec/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-13 09:14:03.795136 vizelec-0.1.2/vizelec/main.py
+-rw-r--r--   0        0        0      845 2023-04-13 09:59:17.879101 vizelec-0.1.2/vizelec/pinout.py
+-rw-r--r--   0        0        0     3290 2023-04-13 09:09:59.406444 vizelec-0.1.2/vizelec/spice.py
+-rw-r--r--   0        0        0     1895 1970-01-01 00:00:00.000000 vizelec-0.1.2/PKG-INFO
```

### Comparing `vizelec-0.1.1/pyproject.toml` & `vizelec-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vizelec"
-version = "0.1.1"
+version = "0.1.2"
 description = "Generate drawing and graph of schematic from various files."
 authors = ["Patarimi <38954040+Patarimi@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 
 [tool.poetry.scripts]
@@ -14,15 +14,15 @@
 doc         = "typer vizelec.main utils docs --name vizelec --output README.md"
 show-update = "poetry show -l -o"
 publish     = "poetry publish --build --username __token__ --password $PYPI_TOKEN"
 increment   = ""
 release     = ["doc", "publish"]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 schemdraw = "^0.16"
 typer = "^0.7.0"
 networkx = "^3.0"
 matplotlib = "^3.7.1"
 
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `vizelec-0.1.1/README.md` & `vizelec-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `vizelec-0.1.1/vizelec/pinout.py` & `vizelec-0.1.2/vizelec/pinout.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 map_pin = {"W": "left", "E": "right", "S": "bott", "N": "top"}
 
 
 @app.command("show")
 def show_pin_order(conf_file: str):
     pin_list = read_conf(conf_file)
-    pins = (elm.IcPin(name=name, side=side) for name, side in pin_list)
+    pins = (elm.IcPin(name=name, side=side, rotation=0 if side in ("left", "right") else 90) for name, side in pin_list)
     schem = sd.Drawing()
     schem += elm.Ic(pins=pins)
     schem.draw()
     return
 
 
 def read_conf(conf_file: str):
```

### Comparing `vizelec-0.1.1/vizelec/spice.py` & `vizelec-0.1.2/vizelec/spice.py`

 * *Files identical despite different names*

### Comparing `vizelec-0.1.1/PKG-INFO` & `vizelec-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: vizelec
-Version: 0.1.1
+Version: 0.1.2
 Summary: Generate drawing and graph of schematic from various files.
 License: MIT
 Author: Patarimi
 Author-email: 38954040+Patarimi@users.noreply.github.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: networkx (>=3.0,<4.0)
 Requires-Dist: schemdraw (>=0.16,<0.17)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
```

