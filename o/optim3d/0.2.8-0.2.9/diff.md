# Comparing `tmp/optim3d-0.2.8.tar.gz` & `tmp/optim3d-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\optim3d-0.2.8.tar", last modified: Thu Apr 13 13:16:12 2023, max compression
+gzip compressed data, was "dist\optim3d-0.2.9.tar", last modified: Thu Apr 13 14:16:25 2023, max compression
```

## Comparing `optim3d-0.2.8.tar` & `optim3d-0.2.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 13:16:12.000000 optim3d-0.2.8/
--rw-rw-rw-   0        0        0     1243 2023-04-06 13:43:27.000000 optim3d-0.2.8/COPYING
--rw-rw-rw-   0        0        0     1613 2023-04-06 13:43:27.000000 optim3d-0.2.8/LICENSE
--rw-rw-rw-   0        0        0       34 2023-04-13 13:09:55.000000 optim3d-0.2.8/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-04-13 13:16:12.000000 optim3d-0.2.8/optim3d/
-drwxrwxrwx   0        0        0        0 2023-04-13 13:16:12.000000 optim3d-0.2.8/optim3d/config/
--rw-rw-rw-   0        0        0    20163 2023-04-06 13:43:27.000000 optim3d-0.2.8/optim3d/config/reconstruct.json
--rw-rw-rw-   0        0        0    43428 2023-04-06 13:43:27.000000 optim3d-0.2.8/optim3d/config/reconstruct_.json
--rw-rw-rw-   0        0        0    21861 2023-04-13 13:15:41.000000 optim3d-0.2.8/optim3d/main.py
--rw-rw-rw-   0        0        0        0 2023-04-13 12:09:44.000000 optim3d-0.2.8/optim3d/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:16:12.000000 optim3d-0.2.8/optim3d.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-13 13:16:12.000000 optim3d-0.2.8/optim3d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-13 13:16:12.000000 optim3d-0.2.8/optim3d.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0    14824 2023-04-13 13:16:12.000000 optim3d-0.2.8/optim3d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       29 2023-04-13 13:16:12.000000 optim3d-0.2.8/optim3d.egg-info/requires.txt
--rw-rw-rw-   0        0        0      335 2023-04-13 13:16:12.000000 optim3d-0.2.8/optim3d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-04-13 13:16:12.000000 optim3d-0.2.8/optim3d.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    14824 2023-04-13 13:16:12.000000 optim3d-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0    13741 2023-04-12 14:06:45.000000 optim3d-0.2.8/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 13:16:12.000000 optim3d-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0      841 2023-04-13 13:14:41.000000 optim3d-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:16:25.000000 optim3d-0.2.9/
+-rw-rw-rw-   0        0        0     1243 2023-04-06 13:43:27.000000 optim3d-0.2.9/COPYING
+-rw-rw-rw-   0        0        0     1613 2023-04-06 13:43:27.000000 optim3d-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-04-13 13:09:55.000000 optim3d-0.2.9/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-04-13 14:16:25.000000 optim3d-0.2.9/optim3d/
+drwxrwxrwx   0        0        0        0 2023-04-13 14:16:25.000000 optim3d-0.2.9/optim3d/config/
+-rw-rw-rw-   0        0        0    20163 2023-04-06 13:43:27.000000 optim3d-0.2.9/optim3d/config/reconstruct.json
+-rw-rw-rw-   0        0        0    43428 2023-04-06 13:43:27.000000 optim3d-0.2.9/optim3d/config/reconstruct_.json
+-rw-rw-rw-   0        0        0    21873 2023-04-13 14:15:19.000000 optim3d-0.2.9/optim3d/main.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:09:44.000000 optim3d-0.2.9/optim3d/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:16:25.000000 optim3d-0.2.9/optim3d.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-13 14:16:25.000000 optim3d-0.2.9/optim3d.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-13 14:16:25.000000 optim3d-0.2.9/optim3d.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0    14880 2023-04-13 14:16:25.000000 optim3d-0.2.9/optim3d.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-04-13 14:16:25.000000 optim3d-0.2.9/optim3d.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      335 2023-04-13 14:16:25.000000 optim3d-0.2.9/optim3d.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-04-13 14:16:25.000000 optim3d-0.2.9/optim3d.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    14880 2023-04-13 14:16:25.000000 optim3d-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0    13797 2023-04-13 14:15:40.000000 optim3d-0.2.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 14:16:25.000000 optim3d-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      841 2023-04-13 14:16:09.000000 optim3d-0.2.9/setup.py
```

### Comparing `optim3d-0.2.8/COPYING` & `optim3d-0.2.9/COPYING`

 * *Files identical despite different names*

### Comparing `optim3d-0.2.8/LICENSE` & `optim3d-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `optim3d-0.2.8/optim3d/config/reconstruct.json` & `optim3d-0.2.9/optim3d/config/reconstruct.json`

 * *Files identical despite different names*

### Comparing `optim3d-0.2.8/optim3d/config/reconstruct_.json` & `optim3d-0.2.9/optim3d/config/reconstruct_.json`

 * *Files identical despite different names*

### Comparing `optim3d-0.2.8/optim3d/main.py` & `optim3d-0.2.9/optim3d/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -420,18 +420,19 @@
     tmp = tempfile.mkdtemp()
 
     config = {
         "input":os.path.abspath(pointcloud),
         "output":os.path.abspath("{}/indexed_pointcloud".format(output))
     }
 
-    with open('{}\\config.json'.format(tmp),'w') as file:
-        json.dumps(json.dump(config, file, indent=2))
+    config_file = os.path.join(tmp, "config.json")
+    with open(config_file, "w") as f:
+        json.dump(config, f, indent=2)
 
-    os.system('entwine build -c {}\\config.json'.format(tmp))
+    os.system('entwine build -c {}'.format(config_file))
 
 @click.command()
 @click.option('--areas', help='The calculated processing areas.', type=click.Path(exists=True), default="./output/processing_areas.gpkg", show_default=True)
 @click.option('--indexed', help='Indexed 3D point cloud directory.', type=click.Path(exists=True), default="./output/indexed_pointcloud", show_default=True)
 @click.option('--output', help='Output directory.', type=click.Path(exists=False), default="./output", show_default=True)
 
 def tiler3d(areas, indexed, output):
```

### Comparing `optim3d-0.2.8/optim3d.egg-info/PKG-INFO` & `optim3d-0.2.9/optim3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optim3d
-Version: 0.2.8
+Version: 0.2.9
 Summary: CLI application for efficient and optimized reconstruction of large-scale 3D building models.
 Home-page: https://github.com/Yarroudh/Optim3D
 Author: Anass Yarroudh
 Author-email: ayarroudh@uliege.be
 License: BSD 3-Clause BSD 3-Clause "New" or "Revised" License
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -36,15 +36,15 @@
 conda create --name optimenv python==3.6
 conda activate optimenv
 conda install -c conda-forge pdal python-pdal
 conda install -c conda-forge entwine
 pip install optim3d
 ```
 
-You can also build everything from source (see [INSTALL.md]()). A [Docker image](https://hub.docker.com/r/yarroudh/optim3d) is also available.
+You can also build everything from source (see [INSTALL.md](https://github.com/Yarroudh/Optim3D/blob/main/INSTALL.md)). A [Docker image](https://hub.docker.com/r/yarroudh/optim3d) is also available.
 
 **NOTE:** It is important to note that in order to use our program for 3D reconstruction of buildings, [GeoFlow-bundle](https://github.com/geoflow3d/geoflow-bundle/releases/tag/2022.06.17) must be installed. Please read the LICENSE file.
 
 ## Usage of the CLI
 
 ### Python package
```

### Comparing `optim3d-0.2.8/PKG-INFO` & `optim3d-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optim3d
-Version: 0.2.8
+Version: 0.2.9
 Summary: CLI application for efficient and optimized reconstruction of large-scale 3D building models.
 Home-page: https://github.com/Yarroudh/Optim3D
 Author: Anass Yarroudh
 Author-email: ayarroudh@uliege.be
 License: BSD 3-Clause BSD 3-Clause "New" or "Revised" License
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -36,15 +36,15 @@
 conda create --name optimenv python==3.6
 conda activate optimenv
 conda install -c conda-forge pdal python-pdal
 conda install -c conda-forge entwine
 pip install optim3d
 ```
 
-You can also build everything from source (see [INSTALL.md]()). A [Docker image](https://hub.docker.com/r/yarroudh/optim3d) is also available.
+You can also build everything from source (see [INSTALL.md](https://github.com/Yarroudh/Optim3D/blob/main/INSTALL.md)). A [Docker image](https://hub.docker.com/r/yarroudh/optim3d) is also available.
 
 **NOTE:** It is important to note that in order to use our program for 3D reconstruction of buildings, [GeoFlow-bundle](https://github.com/geoflow3d/geoflow-bundle/releases/tag/2022.06.17) must be installed. Please read the LICENSE file.
 
 ## Usage of the CLI
 
 ### Python package
```

### Comparing `optim3d-0.2.8/README.md` & `optim3d-0.2.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 conda create --name optimenv python==3.6
 conda activate optimenv
 conda install -c conda-forge pdal python-pdal
 conda install -c conda-forge entwine
 pip install optim3d
 ```
 
-You can also build everything from source (see [INSTALL.md]()). A [Docker image](https://hub.docker.com/r/yarroudh/optim3d) is also available.
+You can also build everything from source (see [INSTALL.md](https://github.com/Yarroudh/Optim3D/blob/main/INSTALL.md)). A [Docker image](https://hub.docker.com/r/yarroudh/optim3d) is also available.
 
 **NOTE:** It is important to note that in order to use our program for 3D reconstruction of buildings, [GeoFlow-bundle](https://github.com/geoflow3d/geoflow-bundle/releases/tag/2022.06.17) must be installed. Please read the LICENSE file.
 
 ## Usage of the CLI
 
 ### Python package
```

### Comparing `optim3d-0.2.8/setup.py` & `optim3d-0.2.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt", "r") as file:
     requirements = file.read().splitlines()
 
 setup(
     name="optim3d",
-    version='0.2.8',
+    version='0.2.9',
     description="CLI application for efficient and optimized reconstruction of large-scale 3D building models.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     license='BSD 3-Clause BSD 3-Clause "New" or "Revised" License',
     author = 'Anass Yarroudh',
     author_email = 'ayarroudh@uliege.be',
     url = 'https://github.com/Yarroudh/Optim3D',
```

