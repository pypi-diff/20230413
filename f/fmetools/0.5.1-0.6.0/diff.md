# Comparing `tmp/fmetools-0.5.1-py2.py3-none-any.whl.zip` & `tmp/fmetools-0.6.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 32422 bytes, number of entries: 16
--rw-rw-rw-  2.0 fat      375 b- defN 23-Mar-03 23:45 fmetools/__init__.py
+Zip file size: 32690 bytes, number of entries: 16
+-rw-rw-rw-  2.0 fat      375 b- defN 23-Mar-30 22:12 fmetools/__init__.py
 -rw-rw-rw-  2.0 fat     7487 b- defN 23-Feb-18 00:43 fmetools/features.py
 -rw-rw-rw-  2.0 fat     5781 b- defN 23-Mar-03 22:51 fmetools/guiparams.py
 -rw-rw-rw-  2.0 fat    26444 b- defN 23-Feb-18 00:43 fmetools/http.py
 -rw-rw-rw-  2.0 fat     2301 b- defN 23-Feb-18 00:43 fmetools/localize.py
 -rw-rw-rw-  2.0 fat     3346 b- defN 23-Feb-18 00:43 fmetools/logfile.py
--rw-rw-rw-  2.0 fat     7957 b- defN 23-Mar-03 23:10 fmetools/paramparsing.py
+-rw-rw-rw-  2.0 fat     8114 b- defN 23-Mar-30 22:12 fmetools/paramparsing.py
 -rw-rw-rw-  2.0 fat    11898 b- defN 23-Feb-18 00:43 fmetools/parsers.py
--rw-rw-rw-  2.0 fat    19096 b- defN 23-Feb-18 00:43 fmetools/plugins.py
+-rw-rw-rw-  2.0 fat    19364 b- defN 23-Mar-30 22:12 fmetools/plugins.py
 -rw-rw-rw-  2.0 fat     1052 b- defN 23-Feb-18 00:43 fmetools/utils.py
 -rw-rw-rw-  2.0 fat     9675 b- defN 23-Feb-18 00:43 fmetools/webservices.py
--rw-rw-rw-  2.0 fat     1331 b- defN 23-Mar-03 23:45 fmetools-0.5.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3587 b- defN 23-Mar-03 23:45 fmetools-0.5.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Mar-03 23:45 fmetools-0.5.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Mar-03 23:45 fmetools-0.5.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1238 b- defN 23-Mar-03 23:45 fmetools-0.5.1.dist-info/RECORD
-16 files, 101687 bytes uncompressed, 30420 bytes compressed:  70.1%
+-rw-rw-rw-  2.0 fat     1331 b- defN 23-Mar-30 22:13 fmetools-0.6.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3929 b- defN 23-Mar-30 22:13 fmetools-0.6.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Mar-30 22:13 fmetools-0.6.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Mar-30 22:13 fmetools-0.6.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1238 b- defN 23-Mar-30 22:13 fmetools-0.6.0.dist-info/RECORD
+16 files, 102454 bytes uncompressed, 30688 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: fmetools/utils.py
 Comment: 
 
 Filename: fmetools/webservices.py
 Comment: 
 
-Filename: fmetools-0.5.1.dist-info/LICENSE
+Filename: fmetools-0.6.0.dist-info/LICENSE
 Comment: 
 
-Filename: fmetools-0.5.1.dist-info/METADATA
+Filename: fmetools-0.6.0.dist-info/METADATA
 Comment: 
 
-Filename: fmetools-0.5.1.dist-info/WHEEL
+Filename: fmetools-0.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: fmetools-0.5.1.dist-info/top_level.txt
+Filename: fmetools-0.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: fmetools-0.5.1.dist-info/RECORD
+Filename: fmetools-0.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fmetools/__init__.py

```diff
@@ -1,10 +1,10 @@
 # coding: utf-8
 
-__version__ = "0.5.1"
+__version__ = "0.6.0"
 
 import gettext
 import os
 
 # The fmetools python module uses the locale folder fmetools/i18n
 # Any .mo files should be located there as specified in
 # the Python gettext documentation
```

## fmetools/paramparsing.py

```diff
@@ -58,48 +58,49 @@
         :raises ValueError: If FME cannot find the specified transformer.
         """
         # If the given name is foo.bar.baz, then first try using foo.bar as
         # the fmePackageName argument, for better performance.
         # Fully-qualified package name is still required.
         # FMETransformer will also take the fully-qualified name without
         # the fmePackageName argument, but it's slower.
-        resolve = [(transformer_name, None)]
+        resolve = [(transformer_name, "")]
         name_parts = transformer_name.split(".", maxsplit=2)
         if len(name_parts) == 3:
             resolve.insert(0, (transformer_name, ".".join(name_parts[:2])))
+        if version is None:
+            version = -1
 
-        for name, pkg in resolve:
+        for i, value in enumerate(resolve):
+            name, pkg = value
             try:
-                self.xformer = FMETransformer(
-                    name, fmePackageName=pkg, transformerVersion=version
-                )
-                self.transformer_name = name
-                self.transformer_fpkg = pkg
-            except FMEException:
+                # FMETransformer was added in b23224.
+                # Before b23264, it accepted but ignored kwargs. (FMEENGINE-77074)
+                # For max compatibility, don't use kwargs here.
+                self.xformer = FMETransformer(name, pkg, version)
+            except FMEException as ex:
+                if i == len(resolve) - 1:
+                    raise ValueError(f"Could not resolve {transformer_name}") from ex
                 continue
-            if self.xformer:
-                break
-        try:
-            self.xformer
-        except AttributeError as e:
-            raise ValueError(f"Could not resolve {transformer_name}") from e
+            self.transformer_name = name
+            self.transformer_fpkg = pkg
+            break
 
     def change_version(self, version: Optional[int] = None):
         """
         Change to a different version of the transformer definition.
         This clears state, so serialized parameter values need to be set again
         before their parsed values can be retrieved.
 
         :param version: Transformer version to load.
             If not provided, then the latest version is loaded.
         """
+        if version is None:
+            version = -1
         self.xformer = FMETransformer(
-            self.transformer_name,
-            fmePackageName=self.transformer_fpkg,
-            transformerVersion=version,
+            self.transformer_name, self.transformer_fpkg, version
         )
 
     def is_required(self, name) -> bool:
         """
         :param name: Parameter name.
         :returns: True if the parameter is required according to the
             transformer definition.
```

## fmetools/plugins.py

```diff
@@ -2,19 +2,21 @@
 
 """
 FME PluginBuilder subclasses that provide improved functionality.
 """
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
+import warnings
+
 from fmeobjects import FMEFeature
 from pluginbuilder import FMEReader, FMEWriter
 
 from .logfile import get_configured_logger
-from .parsers import OpenParameters, MappingFile
+from .parsers import MappingFile, OpenParameters
 
 
 class FMESimplifiedReader(FMEReader):
     """Base class for Python-based FME reader implementations.
 
     :ivar str _type_name: The name used in the following contexts:
 
@@ -304,15 +306,15 @@
     def __enter__(self):
         return self
 
     def __exit__(self, *args):
         self.close()
 
 
-class FMETransformer(object):
+class FMEBaseTransformer(object):
     """
     Base class that represents the interface expected by the FME
     infrastructure for Python-based FME transformer implementations.
 
     For testing purposes, this class can be used as a context manager.
     """
 
@@ -419,15 +421,23 @@
         :type support_type: int
         :returns: True if the passed in support type is supported.
         :rtype: bool
         """
         return False
 
 
-class FMEEnhancedTransformer(FMETransformer):
+class FMETransformer(FMEBaseTransformer):
+    def __init__(self):
+        super(FMEBaseTransformer, self).__init__()
+        warnings.warn(
+            "Avoid confusion with fmeobjects.FMETransformer", DeprecationWarning
+        )
+
+
+class FMEEnhancedTransformer(FMEBaseTransformer):
     """
     Recommended base class for transformer implementations.
 
     This class adds methods to introduce more granularity to the transformer lifecycle.
 
     :meth:`input` is broken down to these methods for implementations to overwrite:
        - :meth:`pre_input`
```

## Comparing `fmetools-0.5.1.dist-info/LICENSE` & `fmetools-0.6.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fmetools-0.5.1.dist-info/METADATA` & `fmetools-0.6.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmetools
-Version: 0.5.1
+Version: 0.6.0
 Summary: Tools for extending Safe Software's FME using Python.
 Home-page: https://github.com/safesoftware/fmetools
 Author: Safe Software Inc.
 License: BSD
 Keywords: FME fmeobjects
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -49,14 +49,22 @@
 2. Install dev requirements using `pip install -r requirements.txt`
 3. Do a dev install using `pip install --editable .`
 4. Run tests using `pytest`
 5. Build wheel using `python -m build --wheel`
 
 # fmetools changes
 
+## 0.6.0
+
+* Rename `fmetools.plugins.FMETransformer` to `FMEBaseTransformer`
+  to avoid potential confusion with `fmeobjects.FMETransformer`.
+  Instantiating `fmetools.plugins.FMETransformer` now emits a warning,
+  and will be removed in a future release.
+* `fmetools.paramparsing.TransformerParameterParser`: Support FME >= b23264.
+
 ## 0.5.1
 
 * Add `fmetools.paramparsing.TransformerParameterParser`: a class for parsing
   internal attribute values from transformer parameters. Requires FME 2023.
 * Require Python 3.7+.
 
 ## 0.4.4
```

## Comparing `fmetools-0.5.1.dist-info/RECORD` & `fmetools-0.6.0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-fmetools/__init__.py,sha256=_Blhh-WpTtNBAly2YLFnqas8A3IaeKpVnB8Yyc7Dmco,375
+fmetools/__init__.py,sha256=5GCjMkj2bycvBNFPTMaD2FfImM6r7Vokga6gZ4h-PGo,375
 fmetools/features.py,sha256=89PIQYToz2v6-knEDJeG5YnWeQAngitdxnUgSpcuIDI,7487
 fmetools/guiparams.py,sha256=WXwNf7p6yVXmwkb3eafZoa5KwBHCmhvOwb35AuqSqm8,5781
 fmetools/http.py,sha256=D76lCuu4feAvCES701ukq0UfkFVW88cwfJmduSbhtFc,26444
 fmetools/localize.py,sha256=h91dCHEfO39Yo9RlUw6Jdu3hI4xa6YxE6B8c8Zs68F8,2301
 fmetools/logfile.py,sha256=q2vapWcdYSvVYL86fAoYNBp2l70V34tDlaLpnPQa-6E,3346
-fmetools/paramparsing.py,sha256=X5NIvRODU-jK081sDg6fqQmAosIhrahGlq2CZFurmIg,7957
+fmetools/paramparsing.py,sha256=t-2rnJ20HJFM2BZ1Ej-OB1RMHtprtxWSVfoL6Kq-EJ0,8114
 fmetools/parsers.py,sha256=E99AGZMvnHuIgo_bddcMi46iys4DwxsGvgOkQ1V4y2g,11898
-fmetools/plugins.py,sha256=r2L2-niOHLTDAyyIWmvtbRxZc10y_xxfACLU_7x5MJE,19096
+fmetools/plugins.py,sha256=0HCm_gR9IVARdiQEZXx2stFF2_2Ma5fmNyJprchrGUg,19364
 fmetools/utils.py,sha256=rxz0nZpkhq6VsBsuHn-N86VZF2TQvBpbR76UJ711IKM,1052
 fmetools/webservices.py,sha256=isrY_nhzWynfYgwYUvl1sLUdPpfGC-krBSpvsb_cJMg,9675
-fmetools-0.5.1.dist-info/LICENSE,sha256=PpNszLe8BmZ0HzNTnHzzxHOea-5xsg9a3sdH21tebA4,1331
-fmetools-0.5.1.dist-info/METADATA,sha256=53ibX0HlGNPsx7OZcD7W2EAgUEucieDInofHBmGyaMs,3587
-fmetools-0.5.1.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-fmetools-0.5.1.dist-info/top_level.txt,sha256=JjCaZBooRHcq4es3xJzII3r6MGB3nbsSaaADot83UKU,9
-fmetools-0.5.1.dist-info/RECORD,,
+fmetools-0.6.0.dist-info/LICENSE,sha256=PpNszLe8BmZ0HzNTnHzzxHOea-5xsg9a3sdH21tebA4,1331
+fmetools-0.6.0.dist-info/METADATA,sha256=C72Dcy7yCWXK_eEvcLskxvuHhNPzWn43vf4PXhbXjiE,3929
+fmetools-0.6.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+fmetools-0.6.0.dist-info/top_level.txt,sha256=JjCaZBooRHcq4es3xJzII3r6MGB3nbsSaaADot83UKU,9
+fmetools-0.6.0.dist-info/RECORD,,
```

