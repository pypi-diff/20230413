# Comparing `tmp/TraffiX-0.1.0a0.tar.gz` & `tmp/TraffiX-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TraffiX-0.1.0a0.tar", last modified: Mon Mar 13 10:12:04 2023, max compression
+gzip compressed data, was "TraffiX-0.1.1a0.tar", last modified: Thu Apr 13 15:19:58 2023, max compression
```

## Comparing `TraffiX-0.1.0a0.tar` & `TraffiX-0.1.1a0.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-03-13 10:12:04.580604 TraffiX-0.1.0a0/
--rw-r--r--   0 maman      (501) staff       (20)     1069 2022-11-13 05:40:08.000000 TraffiX-0.1.0a0/LICENSE
--rw-r--r--   0 maman      (501) staff       (20)     2862 2023-03-13 10:12:04.578876 TraffiX-0.1.0a0/PKG-INFO
--rw-r--r--   0 maman      (501) staff       (20)     1860 2023-03-13 09:26:19.000000 TraffiX-0.1.0a0/README.md
-drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-03-13 10:12:04.569939 TraffiX-0.1.0a0/TraffiX/
--rw-r--r--   0 maman      (501) staff       (20)      519 2023-03-13 09:26:19.000000 TraffiX-0.1.0a0/TraffiX/OD.py
-drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-03-13 10:12:04.576044 TraffiX-0.1.0a0/TraffiX/TraffiX.egg-info/
--rw-r--r--   0 maman      (501) staff       (20)     2862 2023-03-13 10:12:04.000000 TraffiX-0.1.0a0/TraffiX/TraffiX.egg-info/PKG-INFO
--rw-r--r--   0 maman      (501) staff       (20)      365 2023-03-13 10:12:04.000000 TraffiX-0.1.0a0/TraffiX/TraffiX.egg-info/SOURCES.txt
--rw-r--r--   0 maman      (501) staff       (20)        1 2023-03-13 10:12:04.000000 TraffiX-0.1.0a0/TraffiX/TraffiX.egg-info/dependency_links.txt
--rw-r--r--   0 maman      (501) staff       (20)       27 2023-03-13 10:12:04.000000 TraffiX-0.1.0a0/TraffiX/TraffiX.egg-info/requires.txt
--rw-r--r--   0 maman      (501) staff       (20)       46 2023-03-13 10:12:04.000000 TraffiX-0.1.0a0/TraffiX/TraffiX.egg-info/top_level.txt
--rw-r--r--   0 maman      (501) staff       (20)       75 2023-03-13 09:28:07.000000 TraffiX-0.1.0a0/TraffiX/__init__.py
--rw-r--r--   0 maman      (501) staff       (20)      622 2023-03-13 09:29:15.000000 TraffiX-0.1.0a0/TraffiX/_api.py
--rw-r--r--   0 maman      (501) staff       (20)       60 2023-03-13 09:29:02.000000 TraffiX-0.1.0a0/TraffiX/_version.py
--rw-r--r--   0 maman      (501) staff       (20)     5245 2023-03-13 09:26:19.000000 TraffiX-0.1.0a0/TraffiX/add.py
--rw-r--r--   0 maman      (501) staff       (20)     1322 2023-03-13 09:26:19.000000 TraffiX-0.1.0a0/TraffiX/flow.py
--rw-r--r--   0 maman      (501) staff       (20)      670 2023-03-13 09:26:19.000000 TraffiX-0.1.0a0/TraffiX/lpr.py
--rw-r--r--   0 maman      (501) staff       (20)      228 2023-03-13 09:26:19.000000 TraffiX-0.1.0a0/TraffiX/me2.py
--rw-r--r--   0 maman      (501) staff       (20)     2123 2023-03-13 09:26:19.000000 TraffiX-0.1.0a0/TraffiX/ue.py
--rw-r--r--   0 maman      (501) staff       (20)       38 2023-03-13 10:12:04.581030 TraffiX-0.1.0a0/setup.cfg
--rwxr-xr-x   0 maman      (501) staff       (20)     1505 2023-03-13 09:25:03.000000 TraffiX-0.1.0a0/setup.py
+drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 15:19:58.515046 TraffiX-0.1.1a0/
+-rw-r--r--   0 maman      (501) staff       (20)     1069 2022-11-13 05:40:08.000000 TraffiX-0.1.1a0/LICENSE
+-rwxr-xr-x   0 maman      (501) staff       (20)       26 2022-06-20 01:06:04.000000 TraffiX-0.1.1a0/MANIFEST.in
+-rw-r--r--   0 maman      (501) staff       (20)     2887 2023-04-13 15:19:58.514341 TraffiX-0.1.1a0/PKG-INFO
+-rw-r--r--   0 maman      (501) staff       (20)     1885 2023-04-13 14:57:03.000000 TraffiX-0.1.1a0/README.md
+drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 15:19:58.508232 TraffiX-0.1.1a0/TraffiX/
+-rw-r--r--   0 maman      (501) staff       (20)     4096 2023-03-13 09:26:19.000000 TraffiX-0.1.1a0/TraffiX/.___init__.py
+-rw-r--r--   0 maman      (501) staff       (20)     4096 2023-03-13 09:26:19.000000 TraffiX-0.1.1a0/TraffiX/.__api.py
+-rw-r--r--   0 maman      (501) staff       (20)     4096 2023-03-13 09:26:19.000000 TraffiX-0.1.1a0/TraffiX/.__version.py
+-rw-r--r--   0 maman      (501) staff       (20)      519 2023-03-13 09:26:19.000000 TraffiX-0.1.1a0/TraffiX/OD.py
+drwxr-xr-x   0 maman      (501) staff       (20)        0 2023-04-13 15:19:58.512992 TraffiX-0.1.1a0/TraffiX/TraffiX.egg-info/
+-rw-r--r--   0 maman      (501) staff       (20)     2887 2023-04-13 15:19:58.000000 TraffiX-0.1.1a0/TraffiX/TraffiX.egg-info/PKG-INFO
+-rw-r--r--   0 maman      (501) staff       (20)      439 2023-04-13 15:19:58.000000 TraffiX-0.1.1a0/TraffiX/TraffiX.egg-info/SOURCES.txt
+-rw-r--r--   0 maman      (501) staff       (20)        1 2023-04-13 15:19:58.000000 TraffiX-0.1.1a0/TraffiX/TraffiX.egg-info/dependency_links.txt
+-rw-r--r--   0 maman      (501) staff       (20)       39 2023-04-13 15:19:58.000000 TraffiX-0.1.1a0/TraffiX/TraffiX.egg-info/requires.txt
+-rw-r--r--   0 maman      (501) staff       (20)       46 2023-04-13 15:19:58.000000 TraffiX-0.1.1a0/TraffiX/TraffiX.egg-info/top_level.txt
+-rw-r--r--   0 maman      (501) staff       (20)       75 2023-03-13 09:28:07.000000 TraffiX-0.1.1a0/TraffiX/__init__.py
+-rw-r--r--   0 maman      (501) staff       (20)      622 2023-03-13 09:29:15.000000 TraffiX-0.1.1a0/TraffiX/_api.py
+-rw-r--r--   0 maman      (501) staff       (20)       60 2023-03-13 09:29:02.000000 TraffiX-0.1.1a0/TraffiX/_version.py
+-rw-r--r--   0 maman      (501) staff       (20)     5245 2023-03-13 09:26:19.000000 TraffiX-0.1.1a0/TraffiX/add.py
+-rw-r--r--   0 maman      (501) staff       (20)     1322 2023-03-13 09:26:19.000000 TraffiX-0.1.1a0/TraffiX/flow.py
+-rw-r--r--   0 maman      (501) staff       (20)      670 2023-03-13 09:26:19.000000 TraffiX-0.1.1a0/TraffiX/lpr.py
+-rw-r--r--   0 maman      (501) staff       (20)      228 2023-03-13 09:26:19.000000 TraffiX-0.1.1a0/TraffiX/me2.py
+-rw-r--r--   0 maman      (501) staff       (20)     2123 2023-03-13 09:26:19.000000 TraffiX-0.1.1a0/TraffiX/ue.py
+-rw-r--r--   0 maman      (501) staff       (20)       38 2023-04-13 15:19:58.515246 TraffiX-0.1.1a0/setup.cfg
+-rwxr-xr-x   0 maman      (501) staff       (20)     1220 2023-04-13 15:19:50.000000 TraffiX-0.1.1a0/setup.py
```

### Comparing `TraffiX-0.1.0a0/LICENSE` & `TraffiX-0.1.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `TraffiX-0.1.0a0/PKG-INFO` & `TraffiX-0.1.1a0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TraffiX
-Version: 0.1.0a0
+Version: 0.1.1a0
 Summary: A package for macroscopic transportation assignment.
 Home-page: https://github.com/Ultios/StraPy
 Author: Aulia Rahman
 Author-email: rahmancs02@gmail.com
 Keywords: Traffic Assignment,Transportation Planning,Macroscopic Transportation Planning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -15,36 +15,36 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# StraPy
-Sustainable Transportation Planning with Python. <br>
-It will soon be renamed into TraffiX, as the name "StraPy" clashed with other package name in PyPi.
+# TraffiX
+Traffic Assignment with NetworkX and osmnX. <br>
+Formerly known as "StraPy", the name clashed with other package name in PyPi.
 
 ## Purpose
-StraPy is aiming to create a free open access transportation simulation software for all, increasing reproducibility, transparency, and public accessibility while decreasing cost and subjective decision making in the transportation modelling domain.<br>
-StraPy is also intended as an environment and framework for student, researcher, public institution or any other interested parties to test all of their transportation modelling related problem for the advancement of the discipline itself.
+TraffiX is aiming to create a free open access transportation simulation software for all, increasing reproducibility, transparency, and public accessibility while decreasing cost and subjective decision making in the transportation modelling domain.<br>
+TraffiX is also intended as an environment and framework for student, researcher, public institution or any other interested parties to test all of their transportation modelling related problem for the advancement of the discipline itself.
 
 ## Current and Future Project Directions
 ### Now
-StraPy is currently developing macroscopic modelling assignment (User Equilibrium) described in Yosef Sheffi's Urban Transportation Networks and Maximum Entropy Matrix Estimation commonly used as the basic macroscopic transportation model in the four step transport plannning model. <br>
+TraffiX is currently developing macroscopic modelling assignment (User Equilibrium) described in Yosef Sheffi's Urban Transportation Networks and Maximum Entropy Matrix Estimation commonly used as the basic macroscopic transportation model in the four step transport plannning model. <br>
 ### In the near future
-StraPy short-term goals is supporting classical transportation modellling techniques and method described in Ortúzar & Willumsen's Modelling Transport. <br>
+TraffiX short-term goals is supporting classical transportation modellling techniques and method described in Ortúzar & Willumsen's Modelling Transport and Yosef Sheffi's Urban Transportation Network <br>
 ### In the distant future
 Although the current goals of StraPy are focusing on macroscopic aspect of transportation modelling, it is also expected to include functionalities to support on any other branches such as microscopic transportation modelling, behavioral model (discrete choice modelling), Agent-based Modelling (such as MATSim), dynamic modelling, etc.
 
 ## References
 1. Aulia Rahman's [working paper](https://drive.google.com/file/d/1EsmRboHHBDYEzDBGGMN8GfWzcz8Zja3M/view?usp=sharing "Working Paper") (Indonesian Language).
 2. Sheffi, Y. 1984. Urban Transportation Networks.
 3. Ortúzar, J. de D., Willumsen, L.G., Consultancy, L.W., 2011. Modelling Transport.
 
 
 # CHANGELOG
 
-## Version 0.1.0-alpha 01/23/1998
+## Version 0.1.1-alpha 04/13/2023
 This the first release of this package.
 
 User Equilibrium method
 Four Step model compatibility
```

### Comparing `TraffiX-0.1.0a0/README.md` & `TraffiX-0.1.1a0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# StraPy
-Sustainable Transportation Planning with Python. <br>
-It will soon be renamed into TraffiX, as the name "StraPy" clashed with other package name in PyPi.
+# TraffiX
+Traffic Assignment with NetworkX and osmnX. <br>
+Formerly known as "StraPy", the name clashed with other package name in PyPi.
 
 ## Purpose
-StraPy is aiming to create a free open access transportation simulation software for all, increasing reproducibility, transparency, and public accessibility while decreasing cost and subjective decision making in the transportation modelling domain.<br>
-StraPy is also intended as an environment and framework for student, researcher, public institution or any other interested parties to test all of their transportation modelling related problem for the advancement of the discipline itself.
+TraffiX is aiming to create a free open access transportation simulation software for all, increasing reproducibility, transparency, and public accessibility while decreasing cost and subjective decision making in the transportation modelling domain.<br>
+TraffiX is also intended as an environment and framework for student, researcher, public institution or any other interested parties to test all of their transportation modelling related problem for the advancement of the discipline itself.
 
 ## Current and Future Project Directions
 ### Now
-StraPy is currently developing macroscopic modelling assignment (User Equilibrium) described in Yosef Sheffi's Urban Transportation Networks and Maximum Entropy Matrix Estimation commonly used as the basic macroscopic transportation model in the four step transport plannning model. <br>
+TraffiX is currently developing macroscopic modelling assignment (User Equilibrium) described in Yosef Sheffi's Urban Transportation Networks and Maximum Entropy Matrix Estimation commonly used as the basic macroscopic transportation model in the four step transport plannning model. <br>
 ### In the near future
-StraPy short-term goals is supporting classical transportation modellling techniques and method described in Ortúzar & Willumsen's Modelling Transport. <br>
+TraffiX short-term goals is supporting classical transportation modellling techniques and method described in Ortúzar & Willumsen's Modelling Transport and Yosef Sheffi's Urban Transportation Network <br>
 ### In the distant future
 Although the current goals of StraPy are focusing on macroscopic aspect of transportation modelling, it is also expected to include functionalities to support on any other branches such as microscopic transportation modelling, behavioral model (discrete choice modelling), Agent-based Modelling (such as MATSim), dynamic modelling, etc.
 
 ## References
 1. Aulia Rahman's [working paper](https://drive.google.com/file/d/1EsmRboHHBDYEzDBGGMN8GfWzcz8Zja3M/view?usp=sharing "Working Paper") (Indonesian Language).
 2. Sheffi, Y. 1984. Urban Transportation Networks.
 3. Ortúzar, J. de D., Willumsen, L.G., Consultancy, L.W., 2011. Modelling Transport.
```

### Comparing `TraffiX-0.1.0a0/TraffiX/OD.py` & `TraffiX-0.1.1a0/TraffiX/OD.py`

 * *Files identical despite different names*

### Comparing `TraffiX-0.1.0a0/TraffiX/TraffiX.egg-info/PKG-INFO` & `TraffiX-0.1.1a0/TraffiX/TraffiX.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TraffiX
-Version: 0.1.0a0
+Version: 0.1.1a0
 Summary: A package for macroscopic transportation assignment.
 Home-page: https://github.com/Ultios/StraPy
 Author: Aulia Rahman
 Author-email: rahmancs02@gmail.com
 Keywords: Traffic Assignment,Transportation Planning,Macroscopic Transportation Planning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -15,36 +15,36 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# StraPy
-Sustainable Transportation Planning with Python. <br>
-It will soon be renamed into TraffiX, as the name "StraPy" clashed with other package name in PyPi.
+# TraffiX
+Traffic Assignment with NetworkX and osmnX. <br>
+Formerly known as "StraPy", the name clashed with other package name in PyPi.
 
 ## Purpose
-StraPy is aiming to create a free open access transportation simulation software for all, increasing reproducibility, transparency, and public accessibility while decreasing cost and subjective decision making in the transportation modelling domain.<br>
-StraPy is also intended as an environment and framework for student, researcher, public institution or any other interested parties to test all of their transportation modelling related problem for the advancement of the discipline itself.
+TraffiX is aiming to create a free open access transportation simulation software for all, increasing reproducibility, transparency, and public accessibility while decreasing cost and subjective decision making in the transportation modelling domain.<br>
+TraffiX is also intended as an environment and framework for student, researcher, public institution or any other interested parties to test all of their transportation modelling related problem for the advancement of the discipline itself.
 
 ## Current and Future Project Directions
 ### Now
-StraPy is currently developing macroscopic modelling assignment (User Equilibrium) described in Yosef Sheffi's Urban Transportation Networks and Maximum Entropy Matrix Estimation commonly used as the basic macroscopic transportation model in the four step transport plannning model. <br>
+TraffiX is currently developing macroscopic modelling assignment (User Equilibrium) described in Yosef Sheffi's Urban Transportation Networks and Maximum Entropy Matrix Estimation commonly used as the basic macroscopic transportation model in the four step transport plannning model. <br>
 ### In the near future
-StraPy short-term goals is supporting classical transportation modellling techniques and method described in Ortúzar & Willumsen's Modelling Transport. <br>
+TraffiX short-term goals is supporting classical transportation modellling techniques and method described in Ortúzar & Willumsen's Modelling Transport and Yosef Sheffi's Urban Transportation Network <br>
 ### In the distant future
 Although the current goals of StraPy are focusing on macroscopic aspect of transportation modelling, it is also expected to include functionalities to support on any other branches such as microscopic transportation modelling, behavioral model (discrete choice modelling), Agent-based Modelling (such as MATSim), dynamic modelling, etc.
 
 ## References
 1. Aulia Rahman's [working paper](https://drive.google.com/file/d/1EsmRboHHBDYEzDBGGMN8GfWzcz8Zja3M/view?usp=sharing "Working Paper") (Indonesian Language).
 2. Sheffi, Y. 1984. Urban Transportation Networks.
 3. Ortúzar, J. de D., Willumsen, L.G., Consultancy, L.W., 2011. Modelling Transport.
 
 
 # CHANGELOG
 
-## Version 0.1.0-alpha 01/23/1998
+## Version 0.1.1-alpha 04/13/2023
 This the first release of this package.
 
 User Equilibrium method
 Four Step model compatibility
```

### Comparing `TraffiX-0.1.0a0/TraffiX/_api.py` & `TraffiX-0.1.1a0/TraffiX/_api.py`

 * *Files identical despite different names*

### Comparing `TraffiX-0.1.0a0/TraffiX/add.py` & `TraffiX-0.1.1a0/TraffiX/add.py`

 * *Files identical despite different names*

### Comparing `TraffiX-0.1.0a0/TraffiX/flow.py` & `TraffiX-0.1.1a0/TraffiX/flow.py`

 * *Files identical despite different names*

### Comparing `TraffiX-0.1.0a0/TraffiX/lpr.py` & `TraffiX-0.1.1a0/TraffiX/lpr.py`

 * *Files identical despite different names*

### Comparing `TraffiX-0.1.0a0/TraffiX/ue.py` & `TraffiX-0.1.1a0/TraffiX/ue.py`

 * *Files identical despite different names*

### Comparing `TraffiX-0.1.0a0/setup.py` & `TraffiX-0.1.1a0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import os
 
 from setuptools import setup
 
-######################################################################################################
-################ You May Remove All the Comments Once You Finish Modifying the Script ################
-######################################################################################################
 
 setup(
     name="TraffiX", 
-    version = "0.1.0-alpha",
+    version = "0.1.1-alpha",
     description = "A package for macroscopic transportation assignment.",
     package_dir = {"":"TraffiX"},
     author = "Aulia Rahman",
     author_email = "rahmancs02@gmail.com",
     long_description = open("README.md").read() + "\n\n" + open("CHANGELOG.md").read(),
     long_description_content_type = "text/markdown",
     url="https://github.com/Ultios/StraPy",
@@ -26,12 +23,13 @@
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: GIS",
         "Operating System :: OS Independent",
     ],
     install_requires = [
+        "python >=3.6",
         "osmnx ~= 1.3.0",
         "pandas ~= 1.2.4",
     ],
     keywords = ["Traffic Assignment", "Transportation Planning", "Macroscopic Transportation Planning"],
 )
```

