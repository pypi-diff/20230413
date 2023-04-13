# Comparing `tmp/navicat_marc-0.1.8.tar.gz` & `tmp/navicat_marc-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "navicat_marc-0.1.8.tar", last modified: Fri Mar 31 18:46:15 2023, max compression
+gzip compressed data, was "navicat_marc-0.1.9.tar", last modified: Wed Apr  5 14:58:12 2023, max compression
```

## Comparing `navicat_marc-0.1.8.tar` & `navicat_marc-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:46:15.367967 navicat_marc-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-31 18:45:50.000000 navicat_marc-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-03-31 18:46:15.367967 navicat_marc-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-03-31 18:45:50.000000 navicat_marc-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:46:15.367967 navicat_marc-0.1.8/navicat_marc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 18:45:50.000000 navicat_marc-0.1.8/navicat_marc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-31 18:45:50.000000 navicat_marc-0.1.8/navicat_marc/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12103 2023-03-31 18:45:50.000000 navicat_marc-0.1.8/navicat_marc/clustering.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4044 2023-03-31 18:45:50.000000 navicat_marc-0.1.8/navicat_marc/da.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2245 2023-03-31 18:45:50.000000 navicat_marc-0.1.8/navicat_marc/distatis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      746 2023-03-31 18:45:50.000000 navicat_marc-0.1.8/navicat_marc/erel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      233 2023-03-31 18:45:50.000000 navicat_marc-0.1.8/navicat_marc/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16630 2023-03-31 18:45:50.000000 navicat_marc-0.1.8/navicat_marc/helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9135 2023-03-31 18:45:50.000000 navicat_marc-0.1.8/navicat_marc/marc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24198 2023-03-31 18:45:50.000000 navicat_marc-0.1.8/navicat_marc/molecule.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11289 2023-03-31 18:45:50.000000 navicat_marc-0.1.8/navicat_marc/rmsd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      569 2023-03-31 18:45:50.000000 navicat_marc-0.1.8/navicat_marc/test_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:46:15.367967 navicat_marc-0.1.8/navicat_marc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-03-31 18:46:15.000000 navicat_marc-0.1.8/navicat_marc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-03-31 18:46:15.000000 navicat_marc-0.1.8/navicat_marc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 18:46:15.000000 navicat_marc-0.1.8/navicat_marc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-31 18:46:15.000000 navicat_marc-0.1.8/navicat_marc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-31 18:46:15.000000 navicat_marc-0.1.8/navicat_marc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-31 18:46:15.000000 navicat_marc-0.1.8/navicat_marc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-31 18:45:50.000000 navicat_marc-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 18:46:15.367967 navicat_marc-0.1.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-03-31 18:45:50.000000 navicat_marc-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:58:12.834032 navicat_marc-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-05 14:57:40.000000 navicat_marc-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-04-05 14:58:12.834032 navicat_marc-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-04-05 14:57:40.000000 navicat_marc-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:58:12.830032 navicat_marc-0.1.9/navicat_marc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 14:57:40.000000 navicat_marc-0.1.9/navicat_marc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-05 14:57:40.000000 navicat_marc-0.1.9/navicat_marc/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12173 2023-04-05 14:57:40.000000 navicat_marc-0.1.9/navicat_marc/clustering.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4044 2023-04-05 14:57:40.000000 navicat_marc-0.1.9/navicat_marc/da.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2245 2023-04-05 14:57:40.000000 navicat_marc-0.1.9/navicat_marc/distatis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      746 2023-04-05 14:57:40.000000 navicat_marc-0.1.9/navicat_marc/erel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      233 2023-04-05 14:57:40.000000 navicat_marc-0.1.9/navicat_marc/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16630 2023-04-05 14:57:40.000000 navicat_marc-0.1.9/navicat_marc/helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9135 2023-04-05 14:57:40.000000 navicat_marc-0.1.9/navicat_marc/marc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24749 2023-04-05 14:57:40.000000 navicat_marc-0.1.9/navicat_marc/molecule.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11289 2023-04-05 14:57:40.000000 navicat_marc-0.1.9/navicat_marc/rmsd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      569 2023-04-05 14:57:40.000000 navicat_marc-0.1.9/navicat_marc/test_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:58:12.834032 navicat_marc-0.1.9/navicat_marc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-04-05 14:58:12.000000 navicat_marc-0.1.9/navicat_marc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-05 14:58:12.000000 navicat_marc-0.1.9/navicat_marc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 14:58:12.000000 navicat_marc-0.1.9/navicat_marc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-05 14:58:12.000000 navicat_marc-0.1.9/navicat_marc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-05 14:58:12.000000 navicat_marc-0.1.9/navicat_marc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-05 14:58:12.000000 navicat_marc-0.1.9/navicat_marc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-05 14:57:40.000000 navicat_marc-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 14:58:12.834032 navicat_marc-0.1.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-04-05 14:57:40.000000 navicat_marc-0.1.9/setup.py
```

### Comparing `navicat_marc-0.1.8/LICENSE` & `navicat_marc-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `navicat_marc-0.1.8/PKG-INFO` & `navicat_marc-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: navicat_marc
-Version: 0.1.8
+Version: 0.1.9
 Summary: Modular Analysis of Representative Conformers
 Home-page: https://github.com/lcmd-epfl/marc/
 Author: rlaplaza, lcmd-epfl
 Author-email: "R. Laplaza" <rlaplaza@duck.com>
 Keywords: compchem
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `navicat_marc-0.1.8/README.md` & `navicat_marc-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `navicat_marc-0.1.8/navicat_marc/clustering.py` & `navicat_marc-0.1.9/navicat_marc/clustering.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,24 +121,25 @@
             s=30,
             edgecolors="black",
             zorder=2,
             c=cmb[i][1],
             marker="X",
             label=f"{names[index]}",
         )
+    plt.savefig("tsne_plot.png", bbox_inches="tight")
     box = ax.get_position()
     ax.set_position([box.x0, box.y0 + box.height * 0.1, box.width, box.height * 0.9])
     ax.legend(
         loc="upper center",
         bbox_to_anchor=(0.5, -0.05),
         fancybox=True,
         shadow=True,
-        ncol=len(clusters),
+        ncol=min(len(clusters), 10),
     )
-    plt.savefig("tsne_plot.png", bbox_inches="tight")
+    plt.savefig("tsne_plot_legend.png", bbox_inches="tight")
     plt.close()
 
 
 def kmeans_clustering(n_clusters, m: np.ndarray, rank=5, verb=0):
     mds = MDS(
         dissimilarity="precomputed",
         n_components=rank,
```

### Comparing `navicat_marc-0.1.8/navicat_marc/da.py` & `navicat_marc-0.1.9/navicat_marc/da.py`

 * *Files identical despite different names*

### Comparing `navicat_marc-0.1.8/navicat_marc/distatis.py` & `navicat_marc-0.1.9/navicat_marc/distatis.py`

 * *Files identical despite different names*

### Comparing `navicat_marc-0.1.8/navicat_marc/erel.py` & `navicat_marc-0.1.9/navicat_marc/erel.py`

 * *Files identical despite different names*

### Comparing `navicat_marc-0.1.8/navicat_marc/helpers.py` & `navicat_marc-0.1.9/navicat_marc/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
     mbuilder = argparse.ArgumentParser(
         prog="navicat_marc",
         description="Analyse conformer ensembles to find the most representative structures.",
         epilog="Remember to cite the marc paper or repository - \n if they have a DOI by now\n - and enjoy!",
     )
     mbuilder.add_argument(
-        "-version", "--version", action="version", version="%(prog)s 0.1.8"
+        "-version", "--version", action="version", version="%(prog)s 0.1.9"
     )
     mbuilder.add_argument(
         "-i",
         "--i",
         "-input",
         dest="input",
         nargs="+",
```

### Comparing `navicat_marc-0.1.8/navicat_marc/marc.py` & `navicat_marc-0.1.9/navicat_marc/marc.py`

 * *Files identical despite different names*

### Comparing `navicat_marc-0.1.8/navicat_marc/molecule.py` & `navicat_marc-0.1.9/navicat_marc/molecule.py`

 * *Files 2% similar despite different names*

```diff
@@ -449,14 +449,15 @@
         lines=None,
         radii=None,
         scale_factor=1.10,
         noh=True,
     ):
         self.scale_factor = scale_factor
         self.radii = radii
+        self.name = name
         if filename is not None:
             self.name = splitext(filename)[0]
             self.from_file(filename, noh)
         elif lines is not None:
             self.from_lines(lines, noh)
             self.name = name
         else:
@@ -483,14 +484,15 @@
             raise InputError(
                 f"Could not obtain the number of atoms in the .xyz file {filename} from first line. Please check format."
             )
 
         # The title line may contain an energy
         title = f.readline().strip()
         energy = None
+        posname = None
         if "energy:" in title and energy is None:
             try:
                 etitle = title.split(":")[1].split(" ")[1].rstrip()
                 energy = float(etitle) * ha_to_kcalmol
             except ValueError:
                 energy = None
             except AttributeError:
@@ -499,14 +501,18 @@
             try:
                 etitle = title.split("Eopt")[-1].rstrip()
                 energy = float(etitle) * ha_to_kcalmol
             except ValueError:
                 energy = None
             except AttributeError:
                 energy = None
+            try:
+                posname = title.split(" ")[0].split("/")[-1].split(".")[-1].rstrip()
+            except Exception:
+                pass
         if energy is None:
             try:
                 energy = float(title) * ha_to_kcalmol
             except ValueError:
                 energy = None
             except AttributeError:
                 energy = None
@@ -543,14 +549,16 @@
         if noh:
             self.atoms = atoms[np.where(atoms > 1)]
             self.coordinates = V[np.where(atoms > 1)]
         else:
             self.atoms = atoms
             self.coordinates = V
         self.energy = energy
+        if self.name is None and self.name != posname:
+            self.name = posname
         if self.radii is None and self.atoms is not None:
             self.set_radii()
         self.set_am()
         self.set_graph()
 
     def from_lines(self, lines, noh=True):
         V = list()
@@ -565,14 +573,15 @@
             raise InputError(
                 f"Could not obtain the number of atoms in the .xyz file line {lines[0]}. Please check format."
             )
 
         # The title line may contain an energy
         title = next(lines_iter).strip()
         energy = None
+        posname = None
         if "energy:" in title and energy is None:
             try:
                 etitle = title.split(":")[1].split(" ")[1].rstrip()
                 energy = float(etitle) * ha_to_kcalmol
             except ValueError:
                 energy = None
             except AttributeError:
@@ -581,14 +590,18 @@
             try:
                 etitle = title.split("Eopt")[-1].rstrip()
                 energy = float(etitle) * ha_to_kcalmol
             except ValueError:
                 energy = None
             except AttributeError:
                 energy = None
+            try:
+                posname = title.split(" ")[0].split("/")[-1].split(".")[-1].rstrip()
+            except Exception:
+                pass
         if energy is None:
             try:
                 energy = float(title) * ha_to_kcalmol
             except ValueError:
                 energy = None
             except AttributeError:
                 energy = None
@@ -622,14 +635,16 @@
         if noh:
             self.atoms = atoms[np.where(atoms > 1)]
             self.coordinates = V[np.where(atoms > 1)]
         else:
             self.atoms = atoms
             self.coordinates = V
         self.energy = energy
+        if self.name is None and self.name != posname:
+            self.name = posname
         if self.radii is None and self.atoms is not None:
             self.set_radii()
         self.set_am()
         self.set_graph()
 
     def set_radii(self):
         radii = np.array([covalent_radii[i] for i in self.atoms], dtype=float)
```

### Comparing `navicat_marc-0.1.8/navicat_marc/rmsd.py` & `navicat_marc-0.1.9/navicat_marc/rmsd.py`

 * *Files identical despite different names*

### Comparing `navicat_marc-0.1.8/navicat_marc/test_modules.py` & `navicat_marc-0.1.9/navicat_marc/test_modules.py`

 * *Files identical despite different names*

### Comparing `navicat_marc-0.1.8/navicat_marc.egg-info/PKG-INFO` & `navicat_marc-0.1.9/navicat_marc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: navicat-marc
-Version: 0.1.8
+Version: 0.1.9
 Summary: Modular Analysis of Representative Conformers
 Home-page: https://github.com/lcmd-epfl/marc/
 Author: rlaplaza, lcmd-epfl
 Author-email: "R. Laplaza" <rlaplaza@duck.com>
 Keywords: compchem
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `navicat_marc-0.1.8/navicat_marc.egg-info/SOURCES.txt` & `navicat_marc-0.1.9/navicat_marc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `navicat_marc-0.1.8/pyproject.toml` & `navicat_marc-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "navicat_marc"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="R. Laplaza", email="rlaplaza@duck.com" },
 ]
 description = "Modular Analysis of Representative Conformers"
 keywords = ["compchem"]
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `navicat_marc-0.1.8/setup.py` & `navicat_marc-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 this_directory = path.abspath(path.dirname(__file__))
 with io.open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="marc",
     packages=["navicat_marc"],
-    version="0.1.8",
+    version="0.1.9",
     description="Modular Analysis of Representative Conformers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="rlaplaza, lcmd-epfl",
     author_email="laplazasolanas@gmail.com",
     url="https://github.com/lcmd-epfl/marc/",
     keywords=["compchem"],
```

