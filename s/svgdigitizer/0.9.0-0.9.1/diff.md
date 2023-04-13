# Comparing `tmp/svgdigitizer-0.9.0.tar.gz` & `tmp/svgdigitizer-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svgdigitizer-0.9.0.tar", last modified: Fri Mar 31 17:49:02 2023, max compression
+gzip compressed data, was "svgdigitizer-0.9.1.tar", last modified: Tue Apr  4 18:24:15 2023, max compression
```

## Comparing `svgdigitizer-0.9.0.tar` & `svgdigitizer-0.9.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 17:49:02.248651 svgdigitizer-0.9.0/
--rw-rw-rw-   0        0        0    35823 2022-07-25 09:14:17.000000 svgdigitizer-0.9.0/LICENSE
--rw-rw-rw-   0        0        0     5020 2023-03-31 17:49:02.247649 svgdigitizer-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     4713 2023-03-23 09:38:46.000000 svgdigitizer-0.9.0/README.md
--rw-rw-rw-   0        0        0       42 2023-03-31 17:49:02.248651 svgdigitizer-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0     2121 2023-03-31 17:47:29.000000 svgdigitizer-0.9.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-31 17:49:02.239035 svgdigitizer-0.9.0/svgdigitizer/
--rw-rw-rw-   0        0        0        0 2022-07-25 09:14:17.000000 svgdigitizer-0.9.0/svgdigitizer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-31 17:49:02.244650 svgdigitizer-0.9.0/svgdigitizer/electrochemistry/
--rw-rw-rw-   0        0        0        0 2022-07-25 09:14:17.000000 svgdigitizer-0.9.0/svgdigitizer/electrochemistry/__init__.py
--rw-rw-rw-   0        0        0    16546 2023-03-23 17:05:18.000000 svgdigitizer-0.9.0/svgdigitizer/electrochemistry/cv.py
--rw-rw-rw-   0        0        0    16152 2023-03-31 17:46:35.000000 svgdigitizer-0.9.0/svgdigitizer/entrypoint.py
--rw-rw-rw-   0        0        0     2297 2023-03-23 09:39:01.000000 svgdigitizer-0.9.0/svgdigitizer/exceptions.py
--rw-rw-rw-   0        0        0    17880 2023-03-23 09:39:01.000000 svgdigitizer-0.9.0/svgdigitizer/svg.py
--rw-rw-rw-   0        0        0    61167 2023-03-23 17:05:18.000000 svgdigitizer-0.9.0/svgdigitizer/svgfigure.py
--rw-rw-rw-   0        0        0    80191 2023-03-23 17:05:18.000000 svgdigitizer-0.9.0/svgdigitizer/svgplot.py
-drwxrwxrwx   0        0        0        0 2023-03-31 17:49:02.246649 svgdigitizer-0.9.0/svgdigitizer/test/
--rw-rw-rw-   0        0        0        0 2022-07-25 09:14:17.000000 svgdigitizer-0.9.0/svgdigitizer/test/__init__.py
--rw-rw-rw-   0        0        0     2901 2022-07-25 09:14:17.000000 svgdigitizer-0.9.0/svgdigitizer/test/cli.py
-drwxrwxrwx   0        0        0        0 2023-03-31 17:49:02.243649 svgdigitizer-0.9.0/svgdigitizer.egg-info/
--rw-rw-rw-   0        0        0     5020 2023-03-31 17:49:02.000000 svgdigitizer-0.9.0/svgdigitizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      526 2023-03-31 17:49:02.000000 svgdigitizer-0.9.0/svgdigitizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 17:49:02.000000 svgdigitizer-0.9.0/svgdigitizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-03-31 17:49:02.000000 svgdigitizer-0.9.0/svgdigitizer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      237 2023-03-31 17:49:02.000000 svgdigitizer-0.9.0/svgdigitizer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-03-31 17:49:02.000000 svgdigitizer-0.9.0/svgdigitizer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-04 18:24:15.869823 svgdigitizer-0.9.1/
+-rw-rw-rw-   0        0        0    35823 2022-07-25 09:14:17.000000 svgdigitizer-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0     5020 2023-04-04 18:24:15.869823 svgdigitizer-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4713 2023-04-04 18:23:09.000000 svgdigitizer-0.9.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-04 18:24:15.869823 svgdigitizer-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     2121 2023-04-04 18:24:09.000000 svgdigitizer-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-04 18:24:15.854716 svgdigitizer-0.9.1/svgdigitizer/
+-rw-rw-rw-   0        0        0        0 2022-07-25 09:14:17.000000 svgdigitizer-0.9.1/svgdigitizer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-04 18:24:15.863711 svgdigitizer-0.9.1/svgdigitizer/electrochemistry/
+-rw-rw-rw-   0        0        0        0 2022-07-25 09:14:17.000000 svgdigitizer-0.9.1/svgdigitizer/electrochemistry/__init__.py
+-rw-rw-rw-   0        0        0    16546 2023-03-23 17:05:18.000000 svgdigitizer-0.9.1/svgdigitizer/electrochemistry/cv.py
+-rw-rw-rw-   0        0        0    16351 2023-04-04 18:23:21.000000 svgdigitizer-0.9.1/svgdigitizer/entrypoint.py
+-rw-rw-rw-   0        0        0     2297 2023-03-23 09:39:01.000000 svgdigitizer-0.9.1/svgdigitizer/exceptions.py
+-rw-rw-rw-   0        0        0    17880 2023-03-23 09:39:01.000000 svgdigitizer-0.9.1/svgdigitizer/svg.py
+-rw-rw-rw-   0        0        0    61167 2023-04-03 18:45:26.000000 svgdigitizer-0.9.1/svgdigitizer/svgfigure.py
+-rw-rw-rw-   0        0        0    80191 2023-03-23 17:05:18.000000 svgdigitizer-0.9.1/svgdigitizer/svgplot.py
+drwxrwxrwx   0        0        0        0 2023-04-04 18:24:15.867810 svgdigitizer-0.9.1/svgdigitizer/test/
+-rw-rw-rw-   0        0        0        0 2022-07-25 09:14:17.000000 svgdigitizer-0.9.1/svgdigitizer/test/__init__.py
+-rw-rw-rw-   0        0        0     2901 2022-07-25 09:14:17.000000 svgdigitizer-0.9.1/svgdigitizer/test/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-04 18:24:15.861709 svgdigitizer-0.9.1/svgdigitizer.egg-info/
+-rw-rw-rw-   0        0        0     5020 2023-04-04 18:24:15.000000 svgdigitizer-0.9.1/svgdigitizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      526 2023-04-04 18:24:15.000000 svgdigitizer-0.9.1/svgdigitizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-04 18:24:15.000000 svgdigitizer-0.9.1/svgdigitizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-04 18:24:15.000000 svgdigitizer-0.9.1/svgdigitizer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      237 2023-04-04 18:24:15.000000 svgdigitizer-0.9.1/svgdigitizer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-04 18:24:15.000000 svgdigitizer-0.9.1/svgdigitizer.egg-info/top_level.txt
```

### Comparing `svgdigitizer-0.9.0/LICENSE` & `svgdigitizer-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `svgdigitizer-0.9.0/PKG-INFO` & `svgdigitizer-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svgdigitizer
-Version: 0.9.0
+Version: 0.9.1
 Summary: svgdigitizer is a Python library and command line tool to recover the measured data underlying plots in scientific publications.
 License: GPL 3.0+
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SVGDigitizer — (x,y) Data Points from SVG files
```

### Comparing `svgdigitizer-0.9.0/README.md` & `svgdigitizer-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `svgdigitizer-0.9.0/setup.py` & `svgdigitizer-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  You should have received a copy of the GNU General Public License
 #  along with svgdigitizer. If not, see <https://www.gnu.org/licenses/>.
 # *********************************************************************
 from distutils.core import setup
 
 setup(
     name="svgdigitizer",
-    version="0.9.0",
+    version="0.9.1",
     packages=["svgdigitizer", "svgdigitizer.electrochemistry", "svgdigitizer.test"],
     license="GPL 3.0+",
     description="svgdigitizer is a Python library and command line tool to recover the measured data underlying plots in scientific publications.",
     long_description=open("README.md", encoding="UTF-8").read(),
     long_description_content_type="text/markdown",
     include_package_data=True,
     install_requires=[
```

### Comparing `svgdigitizer-0.9.0/svgdigitizer/electrochemistry/cv.py` & `svgdigitizer-0.9.1/svgdigitizer/electrochemistry/cv.py`

 * *Files identical despite different names*

### Comparing `svgdigitizer-0.9.0/svgdigitizer/entrypoint.py` & `svgdigitizer-0.9.1/svgdigitizer/entrypoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,35 +135,43 @@
         sampling_interval=sampling_interval,
         algorithm="mark-aligned" if skewed else "axis-aligned",
     )
 
 
 def _create_bibliography(svg, metadata):
     r"""
-    Return a bibtex string built from a BIB file and a key provided in `metadata['source']['citation key']`.
+    Return a bibtex string built from a BIB file and a key provided in `metadata['source']['citation key']`,
+    when both requirements are met. Otherwise an empty string is returned.
 
     This is a helper method for :meth:`digitize_cv`.
     """
     from pybtex.database import parse_file
 
-    try:
-        metadata["source"]["citation key"]
-    except KeyError as exc:
-        raise KeyError(
-            "The name of the bibfile must be specified in the metadata in `metadata['source']['citation key']`."
-        ) from exc
+    metadata.setdefault("source", {})
+    metadata["source"].setdefault("citation key", "")
 
-    bibfile = metadata["source"]["citation key"]
+    bibkey = metadata["source"]["citation key"]
+    if not bibkey:
+        logger.warning(
+            'No bibliography key found in metadata["source"]["citation key"]'
+        )
+        return ""
 
     bib_directory = os.path.dirname(svg)
 
-    bibliography = parse_file(
-        f"{os.path.join(bib_directory, bibfile)}.bib", bib_format="bibtex"
-    )
-    return bibliography.entries[bibfile].to_string("bibtex")
+    bibfile = f"{os.path.join(bib_directory, bibkey)}.bib"
+
+    if not os.path.exists(bibfile):
+        logger.warning(
+            f"A citation key with name {bibkey} was provided, but no BIB file was found."
+        )
+        return ""
+
+    bibliography = parse_file(bibfile, bib_format="bibtex")
+    return bibliography.entries[bibkey].to_string("bibtex")
 
 
 @click.command()
 @click.option(
     "--sampling-interval",
     type=float,
     default=None,
@@ -321,15 +329,14 @@
         metadata.setdefault("bibliography", {})
 
         if metadata["bibliography"]:
             logger.warning(
                 "The key with name `bibliography` in the metadata will be overwritten with the new bibliography data."
             )
 
-        # metadata["bibliography"] = _create_bibliography(svg, metadata)
         metadata.update({"bibliography": _create_bibliography(svg, metadata)})
 
     if package:
         package = _create_package(metadata, csvname, outdir)
 
     with open(
         _outfile(svg, suffix=".json", outdir=outdir),
```

### Comparing `svgdigitizer-0.9.0/svgdigitizer/exceptions.py` & `svgdigitizer-0.9.1/svgdigitizer/exceptions.py`

 * *Files identical despite different names*

### Comparing `svgdigitizer-0.9.0/svgdigitizer/svg.py` & `svgdigitizer-0.9.1/svgdigitizer/svg.py`

 * *Files identical despite different names*

### Comparing `svgdigitizer-0.9.0/svgdigitizer/svgfigure.py` & `svgdigitizer-0.9.1/svgdigitizer/svgfigure.py`

 * *Files identical despite different names*

### Comparing `svgdigitizer-0.9.0/svgdigitizer/svgplot.py` & `svgdigitizer-0.9.1/svgdigitizer/svgplot.py`

 * *Files identical despite different names*

### Comparing `svgdigitizer-0.9.0/svgdigitizer/test/cli.py` & `svgdigitizer-0.9.1/svgdigitizer/test/cli.py`

 * *Files identical despite different names*

### Comparing `svgdigitizer-0.9.0/svgdigitizer.egg-info/PKG-INFO` & `svgdigitizer-0.9.1/svgdigitizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svgdigitizer
-Version: 0.9.0
+Version: 0.9.1
 Summary: svgdigitizer is a Python library and command line tool to recover the measured data underlying plots in scientific publications.
 License: GPL 3.0+
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SVGDigitizer — (x,y) Data Points from SVG files
```

### Comparing `svgdigitizer-0.9.0/svgdigitizer.egg-info/SOURCES.txt` & `svgdigitizer-0.9.1/svgdigitizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

