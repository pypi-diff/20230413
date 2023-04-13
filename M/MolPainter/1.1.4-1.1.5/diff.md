# Comparing `tmp/MolPainter-1.1.4.tar.gz` & `tmp/MolPainter-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MolPainter-1.1.4.tar", last modified: Mon Apr 10 00:20:22 2023, max compression
+gzip compressed data, was "MolPainter-1.1.5.tar", last modified: Thu Apr 13 21:36:14 2023, max compression
```

## Comparing `MolPainter-1.1.4.tar` & `MolPainter-1.1.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 gpantel    (501) staff       (20)        0 2023-04-10 00:20:22.437990 MolPainter-1.1.4/
--rwxr-xr-x   0 gpantel    (501) staff       (20)     1088 2023-03-20 03:43:53.000000 MolPainter-1.1.4/LICENSE
-drwxr-xr-x   0 gpantel    (501) staff       (20)        0 2023-04-10 00:20:22.432264 MolPainter-1.1.4/MolPainter/
--rwxr-xr-x   0 gpantel    (501) staff       (20)    18635 2023-04-09 23:22:03.000000 MolPainter-1.1.4/MolPainter/MolSolvator.py
--rwxr-xr-x   0 gpantel    (501) staff       (20)      149 2023-04-10 00:20:10.000000 MolPainter-1.1.4/MolPainter/__init__.py
--rw-r--r--   0 gpantel    (501) staff       (20)     1288 2023-04-09 23:22:03.000000 MolPainter-1.1.4/MolPainter/about_dialog.py
--rwxr-xr-x   0 gpantel    (501) staff       (20)     5116 2023-03-20 03:43:53.000000 MolPainter-1.1.4/MolPainter/blend_configurator.py
--rwxr-xr-x   0 gpantel    (501) staff       (20)     2915 2023-03-20 03:43:53.000000 MolPainter-1.1.4/MolPainter/cmdbar.py
--rwxr-xr-x   0 gpantel    (501) staff       (20)    22922 2023-03-20 03:43:53.000000 MolPainter-1.1.4/MolPainter/commands.py
--rwxr-xr-x   0 gpantel    (501) staff       (20)     4046 2023-03-20 03:43:53.000000 MolPainter-1.1.4/MolPainter/drawarea.py
--rwxr-xr-x   0 gpantel    (501) staff       (20)    11615 2023-04-09 23:24:07.000000 MolPainter-1.1.4/MolPainter/exporter.py
--rwxr-xr-x   0 gpantel    (501) staff       (20)     2937 2023-03-20 03:43:53.000000 MolPainter-1.1.4/MolPainter/grid_configurator.py
-drwxr-xr-x   0 gpantel    (501) staff       (20)        0 2023-04-10 00:20:22.436681 MolPainter-1.1.4/MolPainter/icons/
--rwxr-xr-x   0 gpantel    (501) staff       (20)     3393 2023-03-20 03:43:53.000000 MolPainter-1.1.4/MolPainter/icons/pencil.png
--rwxr-xr-x   0 gpantel    (501) staff       (20)     3252 2023-03-20 03:43:53.000000 MolPainter-1.1.4/MolPainter/icons/spraycan.png
--rwxr-xr-x   0 gpantel    (501) staff       (20)      694 2023-03-20 03:43:53.000000 MolPainter-1.1.4/MolPainter/icons/square.png
--rwxr-xr-x   0 gpantel    (501) staff       (20)     3405 2023-03-20 03:43:53.000000 MolPainter-1.1.4/MolPainter/icons/zoomin.png
--rwxr-xr-x   0 gpantel    (501) staff       (20)     3395 2023-03-20 03:43:53.000000 MolPainter-1.1.4/MolPainter/icons/zoomout.png
--rwxr-xr-x   0 gpantel    (501) staff       (20)     1985 2023-03-20 03:43:53.000000 MolPainter-1.1.4/MolPainter/layer_configurator.py
--rwxr-xr-x   0 gpantel    (501) staff       (20)    15045 2023-03-20 03:43:53.000000 MolPainter-1.1.4/MolPainter/layer_painter.py
--rwxr-xr-x   0 gpantel    (501) staff       (20)     3474 2023-03-20 03:43:53.000000 MolPainter-1.1.4/MolPainter/molecule_configurator.py
--rwxr-xr-x   0 gpantel    (501) staff       (20)     8057 2023-03-20 03:43:53.000000 MolPainter-1.1.4/MolPainter/molecule_lister.py
--rwxr-xr-x   0 gpantel    (501) staff       (20)     3242 2023-03-20 03:43:53.000000 MolPainter-1.1.4/MolPainter/painter.py
--rwxr-xr-x   0 gpantel    (501) staff       (20)     8507 2023-03-20 03:43:53.000000 MolPainter-1.1.4/MolPainter/proj_saver.py
--rwxr-xr-x   0 gpantel    (501) staff       (20)    10904 2023-03-20 03:43:53.000000 MolPainter-1.1.4/MolPainter/project.py
--rwxr-xr-x   0 gpantel    (501) staff       (20)     3298 2023-03-20 03:43:53.000000 MolPainter-1.1.4/MolPainter/solute_importer.py
--rwxr-xr-x   0 gpantel    (501) staff       (20)     2837 2023-03-20 03:43:53.000000 MolPainter-1.1.4/MolPainter/toolbox.py
-drwxr-xr-x   0 gpantel    (501) staff       (20)        0 2023-04-10 00:20:22.434679 MolPainter-1.1.4/MolPainter.egg-info/
--rw-r--r--   0 gpantel    (501) staff       (20)     4420 2023-04-10 00:20:22.000000 MolPainter-1.1.4/MolPainter.egg-info/PKG-INFO
--rw-r--r--   0 gpantel    (501) staff       (20)      878 2023-04-10 00:20:22.000000 MolPainter-1.1.4/MolPainter.egg-info/SOURCES.txt
--rw-r--r--   0 gpantel    (501) staff       (20)        1 2023-04-10 00:20:22.000000 MolPainter-1.1.4/MolPainter.egg-info/dependency_links.txt
--rw-r--r--   0 gpantel    (501) staff       (20)       97 2023-04-10 00:20:22.000000 MolPainter-1.1.4/MolPainter.egg-info/entry_points.txt
--rw-r--r--   0 gpantel    (501) staff       (20)       28 2023-04-10 00:20:22.000000 MolPainter-1.1.4/MolPainter.egg-info/requires.txt
--rw-r--r--   0 gpantel    (501) staff       (20)       11 2023-04-10 00:20:22.000000 MolPainter-1.1.4/MolPainter.egg-info/top_level.txt
--rw-r--r--   0 gpantel    (501) staff       (20)     4420 2023-04-10 00:20:22.437609 MolPainter-1.1.4/PKG-INFO
--rwxr-xr-x   0 gpantel    (501) staff       (20)     3867 2023-04-10 00:16:44.000000 MolPainter-1.1.4/README.md
--rw-r--r--   0 gpantel    (501) staff       (20)       38 2023-04-10 00:20:22.438128 MolPainter-1.1.4/setup.cfg
--rwxr-xr-x   0 gpantel    (501) staff       (20)      995 2023-03-20 03:43:53.000000 MolPainter-1.1.4/setup.py
-drwxr-xr-x   0 gpantel    (501) staff       (20)        0 2023-04-10 00:20:22.437085 MolPainter-1.1.4/test/
--rw-r--r--   0 gpantel    (501) staff       (20)     3501 2023-04-09 23:24:07.000000 MolPainter-1.1.4/test/test_molpainter.py
+drwxr-xr-x   0 gpantel    (501) staff       (20)        0 2023-04-13 21:36:14.431919 MolPainter-1.1.5/
+-rwxr-xr-x   0 gpantel    (501) staff       (20)     1088 2023-03-20 03:43:53.000000 MolPainter-1.1.5/LICENSE
+drwxr-xr-x   0 gpantel    (501) staff       (20)        0 2023-04-13 21:36:14.420398 MolPainter-1.1.5/MolPainter/
+-rwxr-xr-x   0 gpantel    (501) staff       (20)    18661 2023-04-13 21:35:34.000000 MolPainter-1.1.5/MolPainter/MolSolvator.py
+-rwxr-xr-x   0 gpantel    (501) staff       (20)      149 2023-04-13 21:35:34.000000 MolPainter-1.1.5/MolPainter/__init__.py
+-rw-r--r--   0 gpantel    (501) staff       (20)     1288 2023-04-09 23:22:03.000000 MolPainter-1.1.5/MolPainter/about_dialog.py
+-rwxr-xr-x   0 gpantel    (501) staff       (20)     5116 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/blend_configurator.py
+-rwxr-xr-x   0 gpantel    (501) staff       (20)     2915 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/cmdbar.py
+-rwxr-xr-x   0 gpantel    (501) staff       (20)    22922 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/commands.py
+-rwxr-xr-x   0 gpantel    (501) staff       (20)     4046 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/drawarea.py
+-rwxr-xr-x   0 gpantel    (501) staff       (20)    11615 2023-04-13 21:35:30.000000 MolPainter-1.1.5/MolPainter/exporter.py
+-rwxr-xr-x   0 gpantel    (501) staff       (20)     2937 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/grid_configurator.py
+drwxr-xr-x   0 gpantel    (501) staff       (20)        0 2023-04-13 21:36:14.429607 MolPainter-1.1.5/MolPainter/icons/
+-rwxr-xr-x   0 gpantel    (501) staff       (20)     3393 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/icons/pencil.png
+-rwxr-xr-x   0 gpantel    (501) staff       (20)     3252 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/icons/spraycan.png
+-rwxr-xr-x   0 gpantel    (501) staff       (20)      694 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/icons/square.png
+-rwxr-xr-x   0 gpantel    (501) staff       (20)     3405 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/icons/zoomin.png
+-rwxr-xr-x   0 gpantel    (501) staff       (20)     3395 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/icons/zoomout.png
+-rwxr-xr-x   0 gpantel    (501) staff       (20)     1985 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/layer_configurator.py
+-rwxr-xr-x   0 gpantel    (501) staff       (20)    15045 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/layer_painter.py
+-rwxr-xr-x   0 gpantel    (501) staff       (20)     3474 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/molecule_configurator.py
+-rwxr-xr-x   0 gpantel    (501) staff       (20)     8057 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/molecule_lister.py
+-rwxr-xr-x   0 gpantel    (501) staff       (20)     3242 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/painter.py
+-rwxr-xr-x   0 gpantel    (501) staff       (20)     8507 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/proj_saver.py
+-rwxr-xr-x   0 gpantel    (501) staff       (20)    10904 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/project.py
+-rwxr-xr-x   0 gpantel    (501) staff       (20)     3298 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/solute_importer.py
+-rwxr-xr-x   0 gpantel    (501) staff       (20)     2837 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/toolbox.py
+drwxr-xr-x   0 gpantel    (501) staff       (20)        0 2023-04-13 21:36:14.424360 MolPainter-1.1.5/MolPainter.egg-info/
+-rw-r--r--   0 gpantel    (501) staff       (20)     4619 2023-04-13 21:36:14.000000 MolPainter-1.1.5/MolPainter.egg-info/PKG-INFO
+-rw-r--r--   0 gpantel    (501) staff       (20)      878 2023-04-13 21:36:14.000000 MolPainter-1.1.5/MolPainter.egg-info/SOURCES.txt
+-rw-r--r--   0 gpantel    (501) staff       (20)        1 2023-04-13 21:36:14.000000 MolPainter-1.1.5/MolPainter.egg-info/dependency_links.txt
+-rw-r--r--   0 gpantel    (501) staff       (20)       97 2023-04-13 21:36:14.000000 MolPainter-1.1.5/MolPainter.egg-info/entry_points.txt
+-rw-r--r--   0 gpantel    (501) staff       (20)       28 2023-04-13 21:36:14.000000 MolPainter-1.1.5/MolPainter.egg-info/requires.txt
+-rw-r--r--   0 gpantel    (501) staff       (20)       11 2023-04-13 21:36:14.000000 MolPainter-1.1.5/MolPainter.egg-info/top_level.txt
+-rw-r--r--   0 gpantel    (501) staff       (20)     4619 2023-04-13 21:36:14.431343 MolPainter-1.1.5/PKG-INFO
+-rwxr-xr-x   0 gpantel    (501) staff       (20)     4065 2023-04-13 21:35:34.000000 MolPainter-1.1.5/README.md
+-rw-r--r--   0 gpantel    (501) staff       (20)       38 2023-04-13 21:36:14.432083 MolPainter-1.1.5/setup.cfg
+-rwxr-xr-x   0 gpantel    (501) staff       (20)      995 2023-03-20 03:43:53.000000 MolPainter-1.1.5/setup.py
+drwxr-xr-x   0 gpantel    (501) staff       (20)        0 2023-04-13 21:36:14.430440 MolPainter-1.1.5/test/
+-rw-r--r--   0 gpantel    (501) staff       (20)     3501 2023-04-13 21:35:30.000000 MolPainter-1.1.5/test/test_molpainter.py
```

### Comparing `MolPainter-1.1.4/LICENSE` & `MolPainter-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.4/MolPainter/MolSolvator.py` & `MolPainter-1.1.5/MolPainter/MolSolvator.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,17 @@
     if len(inputs['solvent_molecules']['paths']) != len(inputs['solvent_molecules']['numbers']):
         raise Exception('There should be an equal number of entries for paths and numbers of solent_molecules')
     for i in range(len(inputs['solvent_molecules']['paths'])):
         if os.path.isfile(inputs['solvent_molecules']['paths'][i]) == False:
             raise Exception('The input file %s does not exist'%inputs['solvent_molecules']['paths'][i])
     if 'seed' in inputs['solvent_molecules']:
         seed = inputs['solvent_molecules']['seed']
-    
+    else:
+        seed = None
+
     # 1) Define lattice_width and lattice_height coming from the canvas
     lattice_width = inputs['solute_lattice']['width'] # e.g. 32 angstroms
     lattice_height = inputs['solute_lattice']['height'] # e.g. 16 angstroms
     lattice_spacing = inputs['solute_lattice']['spacing'] # e.g. 8 angstroms
     
     # 2) Define solvent lattice spacing
     solvent_lattice_spacing = inputs['solvent_lattice']['spacing']# e.g. 5 angstroms
```

### Comparing `MolPainter-1.1.4/MolPainter/about_dialog.py` & `MolPainter-1.1.5/MolPainter/about_dialog.py`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.4/MolPainter/blend_configurator.py` & `MolPainter-1.1.5/MolPainter/blend_configurator.py`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.4/MolPainter/cmdbar.py` & `MolPainter-1.1.5/MolPainter/cmdbar.py`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.4/MolPainter/commands.py` & `MolPainter-1.1.5/MolPainter/commands.py`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.4/MolPainter/drawarea.py` & `MolPainter-1.1.5/MolPainter/drawarea.py`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.4/MolPainter/exporter.py` & `MolPainter-1.1.5/MolPainter/exporter.py`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.4/MolPainter/grid_configurator.py` & `MolPainter-1.1.5/MolPainter/grid_configurator.py`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.4/MolPainter/icons/pencil.png` & `MolPainter-1.1.5/MolPainter/icons/pencil.png`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.4/MolPainter/icons/spraycan.png` & `MolPainter-1.1.5/MolPainter/icons/spraycan.png`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.4/MolPainter/icons/square.png` & `MolPainter-1.1.5/MolPainter/icons/square.png`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.4/MolPainter/icons/zoomin.png` & `MolPainter-1.1.5/MolPainter/icons/zoomin.png`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.4/MolPainter/icons/zoomout.png` & `MolPainter-1.1.5/MolPainter/icons/zoomout.png`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.4/MolPainter/layer_configurator.py` & `MolPainter-1.1.5/MolPainter/layer_configurator.py`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.4/MolPainter/layer_painter.py` & `MolPainter-1.1.5/MolPainter/layer_painter.py`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.4/MolPainter/molecule_configurator.py` & `MolPainter-1.1.5/MolPainter/molecule_configurator.py`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.4/MolPainter/molecule_lister.py` & `MolPainter-1.1.5/MolPainter/molecule_lister.py`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.4/MolPainter/painter.py` & `MolPainter-1.1.5/MolPainter/painter.py`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.4/MolPainter/proj_saver.py` & `MolPainter-1.1.5/MolPainter/proj_saver.py`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.4/MolPainter/project.py` & `MolPainter-1.1.5/MolPainter/project.py`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.4/MolPainter/solute_importer.py` & `MolPainter-1.1.5/MolPainter/solute_importer.py`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.4/MolPainter/toolbox.py` & `MolPainter-1.1.5/MolPainter/toolbox.py`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.4/MolPainter.egg-info/PKG-INFO` & `MolPainter-1.1.5/MolPainter.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MolPainter
-Version: 1.1.4
+Version: 1.1.5
 Summary: Tool for drawing complex planar molecular systems of arbitrary composition and molecule placement
 Home-page: https://github.com/gpantel/MolPainter
 Author: George Pantelopulos, Aaron Liberatore
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
@@ -82,7 +82,11 @@
 The new *Insert Solutes* button has the following fields
 
 * **Path** path to a PDB file of the solute you want to add. There can only be one solute in the system at a time!
 * **Buffer space (Å)** the length of the buffer added to obstruct more cells neighboring coordinates of the solute.
 * **Center solute at z (Å)** centers the (x,y,z) coordinates of the solute to the center of the MolPainter grid at a particular plane in the z-dimension.
 * **Expand grid to fit solute** expands the MolPainter grid to fit the (x,y,z) coordinates of the solute system. If the solute system has negative coordinates, these coordinates will still lay outside of the MolPainter canvases!
 
+### Let us promote your work using MolPainter!
+
+* Please reach out to us and let us know about the cool work you've done!
+* We would like to promote interesting systems constructed using MolPainter.
```

### Comparing `MolPainter-1.1.4/MolPainter.egg-info/SOURCES.txt` & `MolPainter-1.1.5/MolPainter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.4/PKG-INFO` & `MolPainter-1.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MolPainter
-Version: 1.1.4
+Version: 1.1.5
 Summary: Tool for drawing complex planar molecular systems of arbitrary composition and molecule placement
 Home-page: https://github.com/gpantel/MolPainter
 Author: George Pantelopulos, Aaron Liberatore
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
@@ -82,7 +82,11 @@
 The new *Insert Solutes* button has the following fields
 
 * **Path** path to a PDB file of the solute you want to add. There can only be one solute in the system at a time!
 * **Buffer space (Å)** the length of the buffer added to obstruct more cells neighboring coordinates of the solute.
 * **Center solute at z (Å)** centers the (x,y,z) coordinates of the solute to the center of the MolPainter grid at a particular plane in the z-dimension.
 * **Expand grid to fit solute** expands the MolPainter grid to fit the (x,y,z) coordinates of the solute system. If the solute system has negative coordinates, these coordinates will still lay outside of the MolPainter canvases!
 
+### Let us promote your work using MolPainter!
+
+* Please reach out to us and let us know about the cool work you've done!
+* We would like to promote interesting systems constructed using MolPainter.
```

### Comparing `MolPainter-1.1.4/README.md` & `MolPainter-1.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -68,7 +68,11 @@
 The new *Insert Solutes* button has the following fields
 
 * **Path** path to a PDB file of the solute you want to add. There can only be one solute in the system at a time!
 * **Buffer space (Å)** the length of the buffer added to obstruct more cells neighboring coordinates of the solute.
 * **Center solute at z (Å)** centers the (x,y,z) coordinates of the solute to the center of the MolPainter grid at a particular plane in the z-dimension.
 * **Expand grid to fit solute** expands the MolPainter grid to fit the (x,y,z) coordinates of the solute system. If the solute system has negative coordinates, these coordinates will still lay outside of the MolPainter canvases!
 
+### Let us promote your work using MolPainter!
+
+* Please reach out to us and let us know about the cool work you've done!
+* We would like to promote interesting systems constructed using MolPainter.
```

### Comparing `MolPainter-1.1.4/setup.py` & `MolPainter-1.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.4/test/test_molpainter.py` & `MolPainter-1.1.5/test/test_molpainter.py`

 * *Files identical despite different names*

