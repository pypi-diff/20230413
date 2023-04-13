# Comparing `tmp/living-figures-0.0.1.tar.gz` & `tmp/living-figures-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "living-figures-0.0.1.tar", last modified: Fri Mar 31 16:35:14 2023, max compression
+gzip compressed data, was "living-figures-0.1.0.tar", last modified: Thu Apr 13 21:35:53 2023, max compression
```

## Comparing `living-figures-0.0.1.tar` & `living-figures-0.1.0.tar`

### file list

```diff
@@ -1,49 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:35:14.446784 living-figures-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-03-31 16:34:16.000000 living-figures-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-31 16:34:16.000000 living-figures-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-03-31 16:35:14.446784 living-figures-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-03-31 16:34:16.000000 living-figures-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-03-31 16:34:16.000000 living-figures-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-31 16:34:16.000000 living-figures-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 16:35:14.446784 living-figures-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-03-31 16:34:16.000000 living-figures-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:35:14.442783 living-figures-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:35:14.442783 living-figures-0.0.1/src/living_figures/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-31 16:34:16.000000 living-figures-0.0.1/src/living_figures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:35:14.442783 living-figures-0.0.1/src/living_figures/bio/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-31 16:34:16.000000 living-figures-0.0.1/src/living_figures/bio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:35:14.446784 living-figures-0.0.1/src/living_figures/bio/fom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 16:34:16.000000 living-figures-0.0.1/src/living_figures/bio/fom/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:35:14.446784 living-figures-0.0.1/src/living_figures/bio/rebase/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 16:34:16.000000 living-figures-0.0.1/src/living_figures/bio/rebase/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:35:14.446784 living-figures-0.0.1/src/living_figures/bio/rebase/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 16:34:16.000000 living-figures-0.0.1/src/living_figures/bio/rebase/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-03-31 16:34:16.000000 living-figures-0.0.1/src/living_figures/bio/rebase/utilities/parse_rebase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-03-31 16:34:16.000000 living-figures-0.0.1/src/living_figures/bio/rebase/utilities/rebase_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:35:14.446784 living-figures-0.0.1/src/living_figures/bio/rebase/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-31 16:34:16.000000 living-figures-0.0.1/src/living_figures/bio/rebase/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21816 2023-03-31 16:34:16.000000 living-figures-0.0.1/src/living_figures/bio/rebase/widgets/panepibrowser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:35:14.446784 living-figures-0.0.1/src/living_figures/bio/volcano/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 16:34:16.000000 living-figures-0.0.1/src/living_figures/bio/volcano/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-03-31 16:34:16.000000 living-figures-0.0.1/src/living_figures/bio/volcano/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-03-31 16:34:16.000000 living-figures-0.0.1/src/living_figures/bio/volcano/make_test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:35:14.446784 living-figures-0.0.1/src/living_figures/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 16:34:16.000000 living-figures-0.0.1/src/living_figures/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-31 16:34:16.000000 living-figures-0.0.1/src/living_figures/helpers/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-31 16:34:16.000000 living-figures-0.0.1/src/living_figures/helpers/sorting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:35:14.442783 living-figures-0.0.1/src/living_figures.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-03-31 16:35:14.000000 living-figures-0.0.1/src/living_figures.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-03-31 16:35:14.000000 living-figures-0.0.1/src/living_figures.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 16:35:14.000000 living-figures-0.0.1/src/living_figures.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-31 16:35:14.000000 living-figures-0.0.1/src/living_figures.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-31 16:35:14.000000 living-figures-0.0.1/src/living_figures.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:35:14.442783 living-figures-0.0.1/src/widget_store/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:35:14.442783 living-figures-0.0.1/src/widget_store/bio/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:35:14.442783 living-figures-0.0.1/src/widget_store/bio/rebase/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:35:14.446784 living-figures-0.0.1/src/widget_store/bio/rebase/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-03-31 16:34:16.000000 living-figures-0.0.1/src/widget_store/bio/rebase/utilities/rebase_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:35:14.446784 living-figures-0.0.1/src/widget_store/bio/rebase/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-31 16:34:16.000000 living-figures-0.0.1/src/widget_store/bio/rebase/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21816 2023-03-31 16:34:16.000000 living-figures-0.0.1/src/widget_store/bio/rebase/widgets/panepibrowser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:35:14.446784 living-figures-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-03-31 16:34:16.000000 living-figures-0.0.1/tests/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:53.633656 living-figures-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-13 21:35:08.000000 living-figures-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 21:35:08.000000 living-figures-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-13 21:35:53.633656 living-figures-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-13 21:35:08.000000 living-figures-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-13 21:35:08.000000 living-figures-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-13 21:35:08.000000 living-figures-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 21:35:53.633656 living-figures-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-13 21:35:08.000000 living-figures-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:53.625656 living-figures-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:53.629656 living-figures-0.1.0/src/living_figures/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 21:35:08.000000 living-figures-0.1.0/src/living_figures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:53.629656 living-figures-0.1.0/src/living_figures/bio/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-13 21:35:08.000000 living-figures-0.1.0/src/living_figures/bio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:53.629656 living-figures-0.1.0/src/living_figures/bio/epigenome/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:08.000000 living-figures-0.1.0/src/living_figures/bio/epigenome/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:53.629656 living-figures-0.1.0/src/living_figures/bio/epigenome/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:08.000000 living-figures-0.1.0/src/living_figures/bio/epigenome/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-04-13 21:35:08.000000 living-figures-0.1.0/src/living_figures/bio/epigenome/utilities/pacbio_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-04-13 21:35:08.000000 living-figures-0.1.0/src/living_figures/bio/epigenome/utilities/parse_rebase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-04-13 21:35:08.000000 living-figures-0.1.0/src/living_figures/bio/epigenome/utilities/rebase_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:53.633656 living-figures-0.1.0/src/living_figures/bio/epigenome/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-13 21:35:08.000000 living-figures-0.1.0/src/living_figures/bio/epigenome/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27526 2023-04-13 21:35:08.000000 living-figures-0.1.0/src/living_figures/bio/epigenome/widgets/panepibrowser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:53.633656 living-figures-0.1.0/src/living_figures/bio/fom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:08.000000 living-figures-0.1.0/src/living_figures/bio/fom/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:53.633656 living-figures-0.1.0/src/living_figures/bio/volcano/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:08.000000 living-figures-0.1.0/src/living_figures/bio/volcano/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-04-13 21:35:08.000000 living-figures-0.1.0/src/living_figures/bio/volcano/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-13 21:35:08.000000 living-figures-0.1.0/src/living_figures/bio/volcano/make_test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:53.633656 living-figures-0.1.0/src/living_figures/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:08.000000 living-figures-0.1.0/src/living_figures/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-13 21:35:08.000000 living-figures-0.1.0/src/living_figures/helpers/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-13 21:35:08.000000 living-figures-0.1.0/src/living_figures/helpers/sorting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:53.629656 living-figures-0.1.0/src/living_figures.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-13 21:35:53.000000 living-figures-0.1.0/src/living_figures.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-13 21:35:53.000000 living-figures-0.1.0/src/living_figures.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 21:35:53.000000 living-figures-0.1.0/src/living_figures.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-13 21:35:53.000000 living-figures-0.1.0/src/living_figures.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-13 21:35:53.000000 living-figures-0.1.0/src/living_figures.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:35:53.633656 living-figures-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-13 21:35:08.000000 living-figures-0.1.0/tests/test_import.py
```

### Comparing `living-figures-0.0.1/LICENSE` & `living-figures-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `living-figures-0.0.1/PKG-INFO` & `living-figures-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: living-figures
-Version: 0.0.1
+Version: 0.1.0
 Summary: Resource of interactive data widgets
 Author-email: Samuel Minot <sminot@fredhutch.org>
 Project-URL: Homepage, https://github.com/FredHutch/widgets-store
 Project-URL: Bug Tracker, https://github.com/FredHutch/widgets-store/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Widget Store
-Collection of useful widgets
+# Living Figures
+Collection of useful interactive data widgets
 
 ## Widgets
 
 The interactive data widgets provided in this repository have been
 created using the [widgets library](https://www.github.com/FredHutch/widgets).
 The idea behind this approach is that the complete set of instructions
 needed to visualize a dataset can be packaged together in a single HTML
@@ -28,15 +28,15 @@
 of [Streamlit](https://streamlit.io/).
 
 ## Using the Store
 
 All of the widgets provided in this store can be installed with:
 
 ```
-pip install widget-store
+pip install living-figures
 ```
 
 Once installed, you can load your data into one of these widgets
 and save an interactive HTML file with:
 
 ```#!/usr/bin/env python
 from living_figures.bio import Volcano
```

### Comparing `living-figures-0.0.1/README.md` & `living-figures-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Widget Store
-Collection of useful widgets
+# Living Figures
+Collection of useful interactive data widgets
 
 ## Widgets
 
 The interactive data widgets provided in this repository have been
 created using the [widgets library](https://www.github.com/FredHutch/widgets).
 The idea behind this approach is that the complete set of instructions
 needed to visualize a dataset can be packaged together in a single HTML
@@ -14,15 +14,15 @@
 of [Streamlit](https://streamlit.io/).
 
 ## Using the Store
 
 All of the widgets provided in this store can be installed with:
 
 ```
-pip install widget-store
+pip install living-figures
 ```
 
 Once installed, you can load your data into one of these widgets
 and save an interactive HTML file with:
 
 ```#!/usr/bin/env python
 from living_figures.bio import Volcano
```

### Comparing `living-figures-0.0.1/pyproject.toml` & `living-figures-0.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "living-figures"
-version = "0.0.1"
+dynamic = ["version"]
 authors = [
   { name="Samuel Minot", email="sminot@fredhutch.org" },
 ]
 description = "Resource of interactive data widgets"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `living-figures-0.0.1/src/living_figures/bio/rebase/utilities/parse_rebase.py` & `living-figures-0.1.0/src/living_figures/bio/epigenome/utilities/parse_rebase.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.0.1/src/living_figures/bio/rebase/utilities/rebase_file.py` & `living-figures-0.1.0/src/living_figures/bio/epigenome/utilities/rebase_file.py`

 * *Files 12% similar despite different names*

```diff
@@ -72,32 +72,64 @@
         """Parse any tabular data files uploaded by the user."""
 
         # Read in each of the files and add them to
         # the existing data
         for file in files:
 
             if file is not None:
-                genome_name = file.name
 
-                for suffix in [".txt"]:
-                    if genome_name.endswith(suffix):
-                        genome_name = genome_name[:-len(suffix)]
-
-                # Try to read the file
-                try:
-                    enzymes = parse_rebase(file)
-                    pass
-                except Exception as e:
-                    self.main_container.warning(
-                        f"Could not read file ({file})\n{str(e)}"
-                    )
-
-                # Add it to the table, overwriting
-                # any other data for the same genome
-                self.add_genome_data(enzymes, genome_name)
+                # If the user uploaded a CSV
+                if file.name.endswith('.csv'):
+
+                    # Read the CSV
+                    self.parse_csv(file)
+
+                # Otherwise
+                else:
+
+                    # Parse the REBASE txt file
+                    self.parse_txt(file)
+
+    def parse_csv(self, file):
+
+        # Read the CSV file
+        df = pd.read_csv(file)
+
+        # Make sure that there is a 'genome' column
+        msg = 'Expected the uploaded CSV to have a "genome" column'
+        assert 'genome' in df.columns.values, msg
+
+        # Iterate over each genome
+        for genome_name, enzymes in df.groupby("genome"):
+
+            # Add it to the table, overwriting
+            # any other data for the same genome
+            self.add_genome_data(enzymes, genome_name)
+
+    def parse_txt(self, file):
+
+        # Get the genome name for this particular file
+        genome_name = file.name
+
+        for suffix in [".txt"]:
+            if genome_name.endswith(suffix):
+                genome_name = genome_name[:-len(suffix)]
+
+        # Try to read the file
+        try:
+            enzymes = parse_rebase(file)
+            pass
+        except Exception as e:
+            self.main_container.warning(
+                f"Could not read file ({file})\n{str(e)}"
+            )
+
+        # Add it to the table, overwriting
+        # any other data for the same genome
+        self.add_genome_data(enzymes, genome_name)
 
     def add_genome_data(self, enzymes: pd.DataFrame, genome_name: str):
 
         # If the existing table does not have any data
         if self.get_value().shape[0] == 0:
 
             # Just add the data
```

### Comparing `living-figures-0.0.1/src/living_figures/bio/rebase/widgets/panepibrowser.py` & `living-figures-0.1.0/src/living_figures/bio/epigenome/widgets/panepibrowser.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,128 +2,203 @@
 
 from typing import Tuple
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 import widgets.streamlit as wist
-from living_figures.bio.rebase.utilities.rebase_file import StREBASE
+from living_figures.bio.epigenome.utilities.pacbio_file import StPBMotif
 from living_figures.helpers.scaling import convert_text_to_scalar
 from living_figures.helpers.sorting import sort_table
+import streamlit as st
+
+st.set_page_config(layout="wide")
 
 
 class PanEpiGenomeBrowser(wist.StreamlitWidget):
     """
     Visualize the epigenetic information from a collection of
-    genomes, with input files provided in REBASE format.
+    genomes, with input files provided in PacBio motifs.csv format.
     """
 
+    layout = 'wide'
+
+    extra_imports = [
+        "from typing import Tuple, Union",
+        "import pandas as pd",
+        "import plotly.express as px",
+        "import plotly.graph_objects as go",
+        "from plotly.subplots import make_subplots",
+        "from living_figures.bio.epigenome.utilities.pacbio_file import StPBMotif", # noqa
+        "from living_figures.helpers.scaling import convert_text_to_scalar",
+        "from living_figures.helpers.sorting import sort_table",
+        "from widgets.base.helpers import encode_dataframe_string",
+        "from widgets.base.helpers import parse_dataframe_string"
+    ]
+
+    requirements = ["living_figures", "scipy"]
+    pyodide_requirements = ["scipy"]
+
     children = [
-        StREBASE(
-            id="rebase"
-        ),
-        wist.StDataFrame(
-            id="genomes_annot",
-            label="Genome Annotations"
-        ),
-        wist.StDownloadDataFrame(
-            target="genomes_annot",
-            label="Download Genome Annotations"
-        ),
-        wist.StDataFrame(
-            id="motifs_annot",
-            label="Motif Annotations"
-        ),
-        wist.StDownloadDataFrame(
-            target="motifs_annot",
-            label="Download Motif Annotations"
-        ),
-        wist.StMultiSelect(
-            id='hidden_genomes',
-            label="Hide Genomes"
-        ),
-        wist.StMultiSelect(
-            id='hidden_motifs',
-            label="Hide Motifs"
-        ),
-        wist.StSelectString(
-            id='genome_axis',
-            label="Show Genomes On",
-            options=["Rows", "Columns"],
-            value="Rows"
-        ),
-        wist.StSelectString(
-            id='sort_genomes_by',
-            label="Sort Genomes By",
-            options=["Motif Presence/Absence", "Genome Annotations"],
-            value="Motif Presence/Absence"
-        ),
-        wist.StSelectString(
-            id='sort_motifs_by',
-            label="Sort Motifs By",
-            options=["Genome Presence/Absence", "Motif Annotations"],
-            value="Genome Presence/Absence"
-        ),
-        wist.StMultiSelect(
-            id="annot_genomes_by",
-            label="Annotate Genomes By"
-        ),
-        wist.StMultiSelect(
-            id="annot_motifs_by",
-            label="Annotate Motifs By"
-        ),
-        wist.StSelectString(
-            id="heatmap_cpal",
-            label="Heatmap Color Palette",
-            options=px.colors.named_colorscales(),
-            value="blues"
-        ),
-        wist.StSelectString(
-            id="annot_cpal",
-            label="Annotation Color Palette",
-            options=px.colors.named_colorscales(),
-            value="bluered"
-        ),
-        wist.StInteger(
-            label="Figure Width",
-            id="figure_width",
-            min_value=100,
-            max_value=1200,
-            step=1,
-            value=600
+        wist.StResource(
+            id='plotting'
         ),
-        wist.StInteger(
-            label="Figure Height",
-            id="figure_height",
-            min_value=100,
-            max_value=1200,
-            step=1,
-            value=600
-        ),
-        wist.StInteger(
-            id="min_fraction",
-            label="Minimum Percentage per Motif",
-            min_value=0,
-            max_value=100,
-            value=25,
-            step=1,
-            help="Only show motifs present at this minimum threshold"
+        wist.StExpander(
+            id='files',
+            label="Input Files",
+            expanded=True,
+            children=[
+                StPBMotif(
+                    id="pacbio"
+                ),
+                wist.StDownloadDataFrame(
+                    target="pacbio",
+                    label="Download PacBio Motif Data"
+                ),
+                wist.StDataFrame(
+                    id="genomes_annot",
+                    label="Genome Annotations"
+                ),
+                wist.StDownloadDataFrame(
+                    target="genomes_annot",
+                    label="Download Genome Annotations"
+                ),
+                wist.StDataFrame(
+                    id="motifs_annot",
+                    label="Motif Annotations"
+                ),
+                wist.StDownloadDataFrame(
+                    target="motifs_annot",
+                    label="Download Motif Annotations"
+                )
+            ]
         ),
-        wist.StInteger(
-            id="min_prevalence",
-            label="Minimum Number of Genomes per Motif",
-            min_value=1,
-            value=1,
-            step=1,
-            help="Only show motifs which are present in sufficient genomes"
+        wist.StColumns(
+            children=[
+                wist.StExpander(
+                    id="contents",
+                    expanded=False,
+                    children=[
+                        wist.StString(
+                            id='title'
+                        ),
+                        wist.StTextArea(
+                            id='description'
+                        ),
+                        wist.StMultiSelect(
+                            id='hidden_genomes',
+                            label="Hide Genomes"
+                        ),
+                        wist.StMultiSelect(
+                            id='hidden_motifs',
+                            label="Hide Motifs"
+                        ),
+                        wist.StFloat(
+                            id="min_fraction",
+                            label="Minimum Fraction per Motif",
+                            min_value=0.,
+                            max_value=1.0,
+                            value=0.25,
+                            step=0.01,
+                            help="Only show motifs present at this minimum threshold" # noqa
+                        ),
+                        wist.StInteger(
+                            id="min_prevalence",
+                            label="Minimum Number of Genomes per Motif",
+                            min_value=1,
+                            value=1,
+                            step=1,
+                            help="Only show motifs which are present in sufficient genomes" # noqa
+                        )
+                    ],
+                    sidebar=False
+                ),
+                wist.StExpander(
+                    id="annotations",
+                    expanded=False,
+                    children=[
+                        wist.StMultiSelect(
+                            id="label_genomes_by",
+                            label="Label Genomes By"
+                        ),
+                        wist.StMultiSelect(
+                            id="annot_genomes_by",
+                            label="Annotate Genomes By"
+                        ),
+                        wist.StMultiSelect(
+                            id="annot_motifs_by",
+                            label="Annotate Motifs By"
+                        ),
+                        wist.StSelectString(
+                            id='sort_genomes_by',
+                            label="Sort Genomes By",
+                            options=["Motif Presence/Absence", "Genome Annotations"], # noqa
+                            value="Motif Presence/Absence"
+                        ),
+                        wist.StSelectString(
+                            id='sort_motifs_by',
+                            label="Sort Motifs By",
+                            options=["Genome Presence/Absence", "Motif Annotations"], # noqa
+                            value="Genome Presence/Absence"
+                        ),
+                        wist.StSelectString(
+                            id='genome_axis',
+                            label="Show Genomes On",
+                            options=["Rows", "Columns"],
+                            value="Rows"
+                        )
+                    ],
+                    sidebar=False
+                ),
+                wist.StExpander(
+                    id="formatting",
+                    expanded=False,
+                    children=[
+                        wist.StSelectString(
+                            id="heatmap_cpal",
+                            label="Heatmap Color Palette",
+                            options=px.colors.named_colorscales(),
+                            value="blues"
+                        ),
+                        wist.StSelectString(
+                            id="annot_cpal",
+                            label="Annotation Color Palette",
+                            options=px.colors.named_colorscales(),
+                            value="bluered"
+                        ),
+                        wist.StFloat(
+                            id="genome_annot_width",
+                            label="Genome Annotation Width",
+                            value=0.05,
+                            min=0.
+                        ),
+                        wist.StFloat(
+                            id="enzyme_annot_width",
+                            label="Enzyme Annotation Width",
+                            value=0.05,
+                            min=0.
+                        ),
+                        wist.StInteger(
+                            label="Figure Height",
+                            id="figure_height",
+                            min_value=100,
+                            max_value=1200,
+                            step=1,
+                            value=600
+                        )
+                    ],
+                    sidebar=False
+                )
+            ],
+            sidebar=False
         )
     ]
 
     def get_df_vals(self, df_name, cname):
-        df = self.get([df_name])
+        df = self.get(["files", df_name])
         if df.shape[0] > 0:
             return df[
                 cname
             ].dropna(
             ).drop_duplicates(
             ).tolist()
         else:
@@ -132,38 +207,44 @@
     def update_selector_options(self, df_name, cname, selector):
         """Keep the Hide Genomes selector in sync."""
 
         # Get the list of genomes from the specified table
         all_options = self.get_df_vals(df_name, cname)
 
         # Get the list of options in the specified input
-        avail_options = self.get([selector], attr="options")
+        avail_options = self.get(
+            ["columns", "contents", selector],
+            attr="options"
+        )
 
         # If they are not the same
         if set(avail_options) != set(all_options):
 
             # Update the menu item
-            self.set([selector], attr="options", value=all_options)
+            self.set(
+                ["columns", "contents", selector],
+                attr="options", value=all_options
+            )
 
-    def update_table(self, table, rebase_cname):
+    def update_table(self, table, pacbio_cname):
         """
         Update the specified table, making sure that it contains
         a row with an 'id' value for each of the unique values
-        in the specifed column in the REBASE table.
+        in the specifed column in the PacBio table.
         """
 
-        # Get the list of values from the specified column in the REBASE table
-        all_options = self.get_df_vals("rebase", rebase_cname)
+        # Get the list of values from the specified column in the PacBio table
+        all_options = self.get_df_vals("pacbio", pacbio_cname)
 
         # If there are no options, stop
         if len(all_options) == 0:
             return
 
         # Get the target table which may be updated
-        df = self.get([table])
+        df = self.get(["files", table])
 
         # If the table is empty
         if df.shape[0] == 0:
 
             # Set up a new table
             df = pd.DataFrame(dict(id=all_options))
 
@@ -187,85 +268,89 @@
             # Otherwise, add in new rows
             df = pd.concat([
                 df,
                 pd.DataFrame(dict(id=missing_options))
             ])
 
         # Update the modified table
-        self.set(path=[table], value=df)
+        self.set(path=["files", table], value=df)
 
         # Also update the download button
-        self._get_child(f"download_{table}").run_self()
+        self._get_child("files", f"download_{table}").run_self()
 
     def run_self(self):
 
         # Update the metadata tables, if needed
         self.update_table("genomes_annot", "genome")
-        self.update_table("motifs_annot", "enz_name")
+        self.update_table("motifs_annot", "motif_id")
 
         # Update the hidden_genomes selector
-        self.update_selector_options("rebase", "genome", "hidden_genomes")
-        self.update_selector_options("rebase", "enz_name", "hidden_motifs")
+        self.update_selector_options("pacbio", "genome", "hidden_genomes")
+        self.update_selector_options("pacbio", "motif_id", "hidden_motifs")
 
         # Update the annotation selectors
         self.update_annotation_selectors()
 
         # Make the plot
         self.plot_heatmap()
 
         # Give the user the option to clone this widget
-        self.clone_button()
+        self.clone_button(sidebar=False)
 
     def update_annotation_selectors(self):
 
-        genomes_annot = self.get(["genomes_annot"])
+        genomes_annot = self.get(["files", "genomes_annot"])
         if genomes_annot.shape[0] == 0:
             genomes_annot = pd.DataFrame(dict(id=[]))
         else:
             msg = "Must provide 'id' column in genome annotations"
             assert 'id' in genomes_annot.columns.values, msg
 
             genomes_annot = genomes_annot.set_index('id')
 
         for df, input_elem in [
             (self.join_motif_annots(), "annot_motifs_by"),
-            (genomes_annot, "annot_genomes_by")
+            (genomes_annot, "annot_genomes_by"),
+            (genomes_annot, "label_genomes_by")
         ]:
             self.set(
-                path=[input_elem],
+                path=["columns", "annotations", input_elem],
                 attr="options",
                 value=df.columns.values
             )
 
     def plot_heatmap(self):
 
         # Get the wide-form tables for plotting
         value_df, text_df = self.prep_heatmap_data()
 
         if value_df is None:
             return
 
-        # Add the motif annotations from the REBASE files
+        # Add the motif annotations from the PacBio files
         # to the user-provided motif annotations
         motif_annot = self.join_motif_annots()
 
         # Get the genome annotations
-        genomes_annot = self.get(["genomes_annot"]).set_index('id')
+        genomes_annot = self.get(["files", "genomes_annot"]).set_index('id')
+
+        # Get the annotation parameters
+        annot_params = self._get_child("columns", "annotations").all_values()
 
         # If the user wants to sort the enzymes by an annotation
-        if self.get(["sort_motifs_by"]) == "Motif Annotations":
+        if annot_params["sort_motifs_by"] == "Motif Annotations":
 
             msg = "Must specify motif annotations for sorting"
-            assert len(self.get(["annot_motifs_by"])) > 0, msg
+            assert len(annot_params["annot_motifs_by"]) > 0, msg
 
             # Sort the annotation table
             enzyme_annot_df = motif_annot.reindex(
-                columns=self.get(["annot_motifs_by"])
+                columns=annot_params["annot_motifs_by"]
             ).sort_values(
-                by=self.get(["annot_motifs_by"])
+                by=annot_params["annot_motifs_by"]
             )
 
             # Only keep the motifs which are detected in >=1 genome
             enzyme_annot_df = enzyme_annot_df.reindex(
                 index=[
                     i for i in enzyme_annot_df.index.values
                     if i in value_df.columns.values
@@ -279,29 +364,29 @@
             text_df = text_df.reindex(
                 columns=enzyme_annot_df.index.values
             )
 
         # Otherwise, the annotations should match the order of the genomes
         else:
             enzyme_annot_df = motif_annot.reindex(
-                columns=self.get(["annot_motifs_by"]) if len(self.get(["annot_motifs_by"])) > 0 else ['none'], # noqa
+                columns=annot_params["annot_motifs_by"] if len(annot_params["annot_motifs_by"]) > 0 else ['none'], # noqa
                 index=value_df.columns.values
             )
 
         # If the user wants to sort the genomes by an annotation
-        if self.get(["sort_genomes_by"]) == "Genome Annotations":
+        if annot_params["sort_genomes_by"] == "Genome Annotations":
 
             msg = "Must specify genome annotations for sorting"
-            assert len(self.get(["annot_genomes_by"])) > 0, msg
+            assert len(annot_params["annot_genomes_by"]) > 0, msg
 
             # Sort the genome annotation table
             genomes_annot_df = genomes_annot.reindex(
-                columns=self.get(["annot_genomes_by"])
+                columns=annot_params["annot_genomes_by"]
             ).sort_values(
-                by=self.get(["annot_genomes_by"])
+                by=annot_params["annot_genomes_by"]
             )
 
             # Only keep the genomes which have >=1 motif detected
             genomes_annot_df = genomes_annot_df.reindex(
                 index=[
                     i for i in genomes_annot_df.index.values
                     if i in value_df.index.values
@@ -315,52 +400,73 @@
             text_df = text_df.reindex(
                 index=genomes_annot_df.index.values
             )
 
         # Otherwise, the annotations should match the order of the genomes
         else:
             genomes_annot_df = genomes_annot.reindex(
-                columns=self.get(["annot_genomes_by"]) if len(self.get(["annot_genomes_by"])) > 0 else ['none'], # noqa
+                columns=annot_params["annot_genomes_by"] if len(annot_params["annot_genomes_by"]) > 0 else ['none'], # noqa
                 index=value_df.index.values
             )
 
+        # If the option was selected to relabel genomes
+        if len(annot_params["label_genomes_by"]) > 0:
+
+            genome_name_map = {}
+            for genome_ix, genome_r in genomes_annot.reindex(
+                columns=annot_params["label_genomes_by"]
+            ).iterrows():
+
+                genome_name_map[
+                    genome_ix
+                ] = f"{' '.join(map(str, genome_r.values))} ({genome_ix})"
+
+            value_df = value_df.rename(index=genome_name_map.get)
+            text_df = text_df.rename(index=genome_name_map.get)
+            genomes_annot_df = genomes_annot_df.rename(
+                index=genome_name_map.get
+            )
+
         # For the colors, convert all values to numeric and scale to 0-1
         enzyme_marginal_z = enzyme_annot_df.apply(
             convert_text_to_scalar
         )
         genome_marginal_z = genomes_annot_df.apply(
             convert_text_to_scalar
         )
 
+        # Get the formatting parameters
+        formatting = self._get_child("columns", "formatting").all_values()
+
         # Set the fraction of the plot used for the marginal annotation
         # depending on the number of those annotations
         enzyme_annot_frac = min(
             0.5,
-            0.02 + (0.05 * float(len(self.get(["annot_motifs_by"]))))
+            0.02 + (formatting["enzyme_annot_width"] * float(len(annot_params["annot_motifs_by"]))) # noqa
         )
         genomes_annot_frac = min(
             0.5,
-            0.02 + (0.05 * float(len(self.get(["annot_genomes_by"]))))
+            0.02 + (formatting["genome_annot_width"] * float(len(annot_params["annot_genomes_by"]))) # noqa
         )
 
         # If the genomes are being displayed on the horizontal axis
-        if self.get(['genome_axis']) == "Columns":
+        if annot_params['genome_axis'] == "Columns":
 
             # Transpose the DataFrames with genome/motif values
             value_df = value_df.T
             text_df = text_df.T
 
             # The enzyme marginal annotation will be on the rows
-            row_marginal_x = self.get(["annot_motifs_by"])
+            row_marginal_x = annot_params["annot_motifs_by"]
             row_marginal_y = value_df.index.values
             row_marginal_z = enzyme_marginal_z.values
             row_marginal_text = enzyme_annot_df.values
 
             # The genome marginal annotation will be on the columns
-            col_marginal_y = self.get(["annot_genomes_by"])
+            col_marginal_y = annot_params["annot_genomes_by"]
             col_marginal_x = value_df.columns.values
             col_marginal_z = genome_marginal_z.T.values
             col_marginal_text = genomes_annot_df.T.values
 
             # Compute the data for the genome-marginal barplot
             genome_bar_x = value_df.columns.values
             genome_bar_y = (value_df > 0).sum(axis=0)
@@ -391,26 +497,26 @@
             motif_bar_nrows = 2
             motif_bar_ncols = 3
 
         # Otherwise
         else:
 
             # The genomes must be displayed on the vertical axis
-            assert self.get(['genome_axis']) == "Rows"
+            assert annot_params['genome_axis'] == "Rows"
 
             # The genome/motif data does not need to be transposed
 
             # The enzyme marginal annotation will be on the columns
             col_marginal_x = value_df.columns.values
-            col_marginal_y = self.get(["annot_motifs_by"])
+            col_marginal_y = annot_params["annot_motifs_by"]
             col_marginal_z = enzyme_marginal_z.T.values
             col_marginal_text = enzyme_annot_df.T.values
 
             # The genome marginal annotation will be on the rows
-            row_marginal_x = self.get(["annot_genomes_by"])
+            row_marginal_x = annot_params["annot_genomes_by"]
             row_marginal_y = value_df.index.values
             row_marginal_z = genome_marginal_z.values
             row_marginal_text = genomes_annot_df.values
 
             # Compute the data for the marginal barplot
             genome_bar_x = (value_df > 0).sum(axis=1)
             genome_bar_y = value_df.index.values
@@ -460,45 +566,45 @@
 
         # Add the heatmap to the plot
         fig.append_trace(
             go.Heatmap(
                 x=value_df.columns.values,
                 y=value_df.index.values,
                 z=value_df.values,
-                colorscale=self.get(["heatmap_cpal"]),
+                colorscale=formatting["heatmap_cpal"],
                 text=text_df.values,
                 hoverinfo="text",
                 colorbar_title="Percent<br>Detection<br>of Motif"
             ),
             row=2,
             col=2
         )
 
         # Add the marginal annotation on the rows
         fig.append_trace(
             go.Heatmap(
                 x=row_marginal_x,
                 y=row_marginal_y,
                 z=row_marginal_z,
-                colorscale=self.get(["annot_cpal"]),
+                colorscale=formatting["annot_cpal"],
                 text=row_marginal_text,
                 hoverinfo="text",
                 showscale=False,
             ),
             row=2,
             col=1
         )
 
         # Add the marginal annotation on the columns
         fig.append_trace(
             go.Heatmap(
                 x=col_marginal_x,
                 y=col_marginal_y,
                 z=col_marginal_z,
-                colorscale=self.get(["annot_cpal"]),
+                colorscale=formatting["annot_cpal"],
                 text=col_marginal_text,
                 hoverinfo="text",
                 showscale=False
             ),
             row=1,
             col=2
         )
@@ -529,30 +635,45 @@
             ),
             row=motif_bar_nrows,
             col=motif_bar_ncols
         )
 
         # Set up the size of the figure
         fig.update_layout(
-            height=self.get(['figure_height']),
-            width=self.get(['figure_width']),
+            height=formatting['figure_height'],
             paper_bgcolor='rgba(0,0,0,0)',
             plot_bgcolor='rgba(0,0,0,0)'
         )
 
-        # Return the figure
-        self.main_container.plotly_chart(fig)
+        # Display the figure in the 'plotting' container
+        plot_area = self._get_child('plotting').main_container
+
+        # If there is a title
+        title = self.get(["columns", "contents", "title"])
+        if title is not None and len(title) > 0 and title != "None":
+            plot_area.write(f"### {title}")
+
+        # Show the chart
+        plot_area.plotly_chart(
+            fig,
+            use_container_width=True
+        )
+
+        # If there is a description
+        description = self.get(["columns", "contents", "description"])
+        if description is not None:
+            plot_area.write(description)
 
     def join_motif_annots(self) -> pd.DataFrame:
         """
         Join the user-provided motif annotations to the set
         of automatically generated annotations.
         """
 
-        user_annots = self.get(["motifs_annot"])
+        user_annots = self.get(["files", "motifs_annot"])
         if user_annots.shape[0] == 0:
             user_annots = pd.DataFrame(dict(id=[]))
         else:
             msg = "Must provide 'id' column in motif annotations"
             assert 'id' in user_annots.columns.values, msg
             user_annots = user_annots.set_index('id')
 
@@ -561,65 +682,57 @@
             self.get_motif_annots(),
             how='outer',
             left_index=True,
             right_index=True
         )
 
     def get_motif_annots(self) -> pd.DataFrame:
-        """Get the motif annotations from the REBASE files."""
+        """Get the motif annotations from the PacBio files."""
 
-        rebase = self.get(["rebase"])
+        pacbio = self.get(["files", "pacbio"])
 
-        df = pd.DataFrame({
-            cname: rebase.groupby(
-                'enz_name'
-            ).head(
-                1
-            ).set_index(
-                'enz_name'
-            )[cname]
-            for cname in [
-                "enz_type",
-                "sub_type",
-                "meth_base",
-                "meth_type",
-                "comp_meth_base",
-                "rec_seq",
-                "type_label"
-            ]
-            if cname in rebase.columns.values
-        })
+        if pacbio.shape[0] == 0:
 
-        if 'rec_seq' in df.columns.values:
-            df = df.assign(
-                motif_length=lambda d: d.rec_seq.apply(len)
-            )
+            return pd.DataFrame()
 
-        return df
+        return pacbio.groupby(
+            'motif_id'
+        ).head(
+            1
+        ).set_index(
+            'motif_id'
+        ).reindex(
+            columns=[
+                "motifString",
+                "centerPos",
+                "modificationType",
+                "motif_length"
+            ]
+        )
 
     def prep_heatmap_data(self) -> Tuple[pd.DataFrame, pd.DataFrame]:
 
         user_inputs = self.all_values(flatten=True)
 
-        if user_inputs["rebase"].shape[0] == 0:
+        if user_inputs["pacbio"].shape[0] == 0:
             self.main_container.info(
-                "Please add REBASE information to get started"
+                "Please add PacBio epigenetic motif information to get started"
             )
             return None, None
 
         # MAKE A WIDE TABLE
-        value_df = user_inputs["rebase"].pivot_table(
+        value_df = user_inputs["pacbio"].pivot_table(
             index="genome",
-            columns="enz_name",
-            values="percent_detected"
+            columns="motif_id",
+            values="fraction"
         ).fillna(0)
 
-        text_df = user_inputs["rebase"].pivot(
+        text_df = user_inputs["pacbio"].pivot(
             index="genome",
-            columns="enz_name",
+            columns="motif_id",
             values="text"
         ).fillna("")
 
         # MASK ANY SELECTED ROWS/COLUMNS
         if len(user_inputs['hidden_motifs']) > 0:
             value_df = value_df.drop(
                 columns=user_inputs['hidden_motifs']
@@ -655,14 +768,20 @@
 
             # If no motifs are left
             if value_df.shape[0] == 0:
                 msg = f"No motifs are found in >= {min_prev} genomes"
                 self.main_container.warning(msg)
                 return None, None
 
+        # If there is only one genome or one motif
+        if value_df.shape[0] < 2 or value_df.shape[1] < 2:
+            msg = "Please provide information for multiple genomes"
+            self.main_container.warning(msg)
+            return None, None
+
         # SORT THE ROWS/COLUMNS
         value_df = sort_table(value_df)
 
         # REALIGN TEXT TABLE TO MATCH VALUES
         text_df = text_df.reindex(
             index=value_df.index.values,
             columns=value_df.columns.values
```

### Comparing `living-figures-0.0.1/src/living_figures/bio/volcano/app.py` & `living-figures-0.1.0/src/living_figures/bio/volcano/app.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.0.1/src/living_figures/bio/volcano/make_test_data.py` & `living-figures-0.1.0/src/living_figures/bio/volcano/make_test_data.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.0.1/src/living_figures/helpers/sorting.py` & `living-figures-0.1.0/src/living_figures/helpers/sorting.py`

 * *Files identical despite different names*

### Comparing `living-figures-0.0.1/src/living_figures.egg-info/PKG-INFO` & `living-figures-0.1.0/src/living_figures.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: living-figures
-Version: 0.0.1
+Version: 0.1.0
 Summary: Resource of interactive data widgets
 Author-email: Samuel Minot <sminot@fredhutch.org>
 Project-URL: Homepage, https://github.com/FredHutch/widgets-store
 Project-URL: Bug Tracker, https://github.com/FredHutch/widgets-store/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Widget Store
-Collection of useful widgets
+# Living Figures
+Collection of useful interactive data widgets
 
 ## Widgets
 
 The interactive data widgets provided in this repository have been
 created using the [widgets library](https://www.github.com/FredHutch/widgets).
 The idea behind this approach is that the complete set of instructions
 needed to visualize a dataset can be packaged together in a single HTML
@@ -28,15 +28,15 @@
 of [Streamlit](https://streamlit.io/).
 
 ## Using the Store
 
 All of the widgets provided in this store can be installed with:
 
 ```
-pip install widget-store
+pip install living-figures
 ```
 
 Once installed, you can load your data into one of these widgets
 and save an interactive HTML file with:
 
 ```#!/usr/bin/env python
 from living_figures.bio import Volcano
```

### Comparing `living-figures-0.0.1/src/widget_store/bio/rebase/utilities/rebase_file.py` & `living-figures-0.1.0/src/living_figures/bio/epigenome/utilities/pacbio_file.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 """
-Utilities needed for processing REBASE data.
+Utilities needed for processing PacBio epigenetic motif data.
 """
 
 from typing import Union
 from widgets.base.helpers import parse_dataframe_string
 from widgets.base.helpers import encode_dataframe_string
 import pandas as pd
 from widgets.streamlit.resource.files.base import StFile
-from living_figures.bio.rebase.utilities.parse_rebase import parse_rebase
 
 
-class StREBASE(StFile):
-    """Process epigenetic data from REBASE format."""
+class StPBMotif(StFile):
+    """Process epigenetic data from PacBio motifs.csv format."""
 
     value = pd.DataFrame()
 
     def __init__(
         self,
-        id="rebase",
+        id="pacbio_motif",
         value=None,
-        label="REBASE Files",
+        label="PacBio Motifs",
         help: Union[str, None] = None,
         disabled: bool = False,
         label_visibility: str = "visible",
         sidebar=True,
         show_uploader=True,
         **kwargs
     ):
@@ -43,15 +42,15 @@
                             (equivalent to label=""). If "collapsed", both
                             the label and the space are removed.
                             Default is "visible"
             sidebar (bool): Set up UI in the sidebar vs. the main container
             show_uploader:  Show / hide the uploader element
 
         Returns:
-            StREBASE:       The instantiated resource object.
+            StPBMotif:       The instantiated resource object.
         """
 
         # Parse the provided value, converting from a gzip-compressed
         # string if necessary
         value = parse_dataframe_string(value)
 
         # Set up the resource attributes
@@ -72,55 +71,143 @@
         """Parse any tabular data files uploaded by the user."""
 
         # Read in each of the files and add them to
         # the existing data
         for file in files:
 
             if file is not None:
-                genome_name = file.name
 
-                for suffix in [".txt"]:
-                    if genome_name.endswith(suffix):
-                        genome_name = genome_name[:-len(suffix)]
-
-                # Try to read the file
-                try:
-                    enzymes = parse_rebase(file)
-                    pass
-                except Exception as e:
-                    self.main_container.warning(
-                        f"Could not read file ({file})\n{str(e)}"
-                    )
-
-                # Add it to the table, overwriting
-                # any other data for the same genome
-                self.add_genome_data(enzymes, genome_name)
+                # If the user uploaded a CSV
+                if file.name.endswith('.csv'):
 
-    def add_genome_data(self, enzymes: pd.DataFrame, genome_name: str):
+                    # Read the CSV
+                    self.parse_csv(file)
+
+    def parse_csv(self, file):
+
+        # Read the CSV file
+        motifs = pd.read_csv(file)
+
+        # Make sure that the expected columns are present
+        expected_cnames = [
+            "motifString",
+            "centerPos",
+            "modificationType",
+            "fraction",
+            "nDetected",
+            "nGenome",
+            "groupTag",
+            "partnerMotifString",
+            "meanScore",
+            "meanIpdRatio",
+            "meanCoverage",
+            "objectiveScore"
+        ]
+
+        missing_cnames = [
+            cname
+            for cname in expected_cnames
+            if cname not in motifs.columns.values
+        ]
+
+        # If any of those columns are missing
+        if len(missing_cnames) > 0:
+            # Warn the user
+            self.main_container.warning(
+                f"Did not find expected columns - {', '.join(missing_cnames)}"
+            )
+            # Take no further action
+            return
+
+        # Add a unique ID for the motif + position + modification
+        # Also add the motif length
+        motifs = motifs.assign(
+            text=motifs.apply(
+                self.format_motif_text,
+                axis=1
+            ),
+            motif_id=motifs.apply(
+                lambda r: f"{r['motifString']}-{r['centerPos']}-{r['modificationType']}", # noqa
+                axis=1
+            ),
+            motif_length=motifs['motifString'].apply(len)
+        )
+
+        # If there is a 'genome' column already present, then this CSV must
+        # have been downloaded from a previous iteration of the browser
+        if 'genome' in motifs.columns.values:
+
+            # Add each of the individual genomes
+            for genome_name, genome_motifs in motifs.groupby('genome'):
+                self.add_genome_data(genome_motifs, genome_name)
+
+        # If no 'genome' column is present, it must be from a single genome
+        else:
+
+            # Get the genome name from the file name
+            genome_name = file.name
+
+            # Strip off the standard suffix
+            for suffix in [".csv", "motifs", "."]:
+                if genome_name.endswith(suffix):
+                    genome_name = genome_name[:-len(suffix)]
+
+            # If there is nothing left
+            if len(genome_name) == 0:
+                # Assign a null value
+                genome_name = None
+
+            # Add it to the table, overwriting
+            # any other data for the same genome
+            self.add_genome_data(motifs, genome_name)
+
+    def format_motif_text(self, r):
+        """Format the hovertext field."""
+
+        return "<br>".join([
+            f"{k}: {v}" for k, v in r.items()
+        ])
+
+    def add_genome_data(
+        self,
+        motifs: pd.DataFrame,
+        genome_name: Union[str, None]
+    ):
+
+        # If the genome_name is null
+        if genome_name is None:
+
+            # Pick a new genome name following the pattern "Unnamed N"
+            genome_name_ix = self.get_value().reindex(
+                columns=['genome']
+            ).dropna(
+            ).drop_duplicates(
+            ).shape[0] + 1
+            genome_name = f"Unnamed {genome_name_ix}"
 
         # If the existing table does not have any data
         if self.get_value().shape[0] == 0:
 
             # Just add the data
-            self.set_value(enzymes.assign(genome=genome_name))
+            self.set_value(motifs.assign(genome=genome_name))
 
         # If the existing table does indeed have data
         else:
 
             # Make sure that there is a 'genome' column
             self.sanity_check_data()
 
             # Add the new data, removing any other
             # data from the same genome
             self.set_value(
                 pd.concat([
                     self.get_value().query(
                         f"genome != '{genome_name}'"
                     ),
-                    enzymes.assign(genome=genome_name)
+                    motifs.assign(genome=genome_name)
                 ])
             )
 
     def sanity_check_data(self):
         """Run some sanity checks on the data table."""
 
         df = self.get_value()
```

### Comparing `living-figures-0.0.1/tests/test_import.py` & `living-figures-0.1.0/tests/test_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from living_figures.bio.volcano.app import Volcano # noqa
-from living_figures.bio.rebase.widgets import PanEpiGenomeBrowser # noqa
+from living_figures.bio.epigenome.widgets import PanEpiGenomeBrowser # noqa
 import unittest
 
 
 class TestInit(unittest.TestCase):
 
     def test_init_volcano(self):
```

