# Comparing `tmp/mpltWrappers-0.0.1rc2.tar.gz` & `tmp/mpltWrappers-0.0.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpltWrappers-0.0.1rc2.tar", last modified: Thu Apr 13 10:26:04 2023, max compression
+gzip compressed data, was "mpltWrappers-0.0.1rc3.tar", last modified: Thu Apr 13 15:24:40 2023, max compression
```

## Comparing `mpltWrappers-0.0.1rc2.tar` & `mpltWrappers-0.0.1rc3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 cahit.kargi   (502) staff       (20)        0 2023-04-13 10:26:04.823423 mpltWrappers-0.0.1rc2/
--rw-r--r--   0 cahit.kargi   (502) staff       (20)       41 2023-04-13 10:08:58.000000 mpltWrappers-0.0.1rc2/MANIFEST.in
--rw-r--r--   0 cahit.kargi   (502) staff       (20)     1245 2023-04-13 10:26:04.823489 mpltWrappers-0.0.1rc2/PKG-INFO
--rw-r--r--   0 cahit.kargi   (502) staff       (20)       15 2023-04-13 10:02:53.000000 mpltWrappers-0.0.1rc2/README.md
--rw-r--r--   0 cahit.kargi   (502) staff       (20)      104 2023-04-13 10:08:09.000000 mpltWrappers-0.0.1rc2/pyproject.toml
--rw-r--r--   0 cahit.kargi   (502) staff       (20)       17 2023-04-13 09:59:35.000000 mpltWrappers-0.0.1rc2/requirements.txt
--rw-r--r--   0 cahit.kargi   (502) staff       (20)     1360 2023-04-13 10:26:04.823800 mpltWrappers-0.0.1rc2/setup.cfg
-drwxr-xr-x   0 cahit.kargi   (502) staff       (20)        0 2023-04-13 10:26:04.819716 mpltWrappers-0.0.1rc2/src/
-drwxr-xr-x   0 cahit.kargi   (502) staff       (20)        0 2023-04-13 10:26:04.822119 mpltWrappers-0.0.1rc2/src/mpltWrappers/
--rw-r--r--   0 cahit.kargi   (502) staff       (20)      130 2023-04-13 09:59:35.000000 mpltWrappers-0.0.1rc2/src/mpltWrappers/__init__.py
--rw-r--r--   0 cahit.kargi   (502) staff       (20)     3690 2023-04-13 09:59:35.000000 mpltWrappers-0.0.1rc2/src/mpltWrappers/colorFuncs.py
--rw-r--r--   0 cahit.kargi   (502) staff       (20)     3797 2023-04-13 09:59:35.000000 mpltWrappers-0.0.1rc2/src/mpltWrappers/colorPlots.py
--rw-r--r--   0 cahit.kargi   (502) staff       (20)     2444 2023-04-13 09:59:35.000000 mpltWrappers-0.0.1rc2/src/mpltWrappers/figCreate.py
--rw-r--r--   0 cahit.kargi   (502) staff       (20)     1163 2023-04-13 09:59:35.000000 mpltWrappers-0.0.1rc2/src/mpltWrappers/linePlots.py
--rw-r--r--   0 cahit.kargi   (502) staff       (20)     6463 2023-04-13 09:59:35.000000 mpltWrappers-0.0.1rc2/src/mpltWrappers/plotSettings.py
-drwxr-xr-x   0 cahit.kargi   (502) staff       (20)        0 2023-04-13 10:26:04.823009 mpltWrappers-0.0.1rc2/src/mpltWrappers.egg-info/
--rw-r--r--   0 cahit.kargi   (502) staff       (20)     1245 2023-04-13 10:26:04.000000 mpltWrappers-0.0.1rc2/src/mpltWrappers.egg-info/PKG-INFO
--rw-r--r--   0 cahit.kargi   (502) staff       (20)      446 2023-04-13 10:26:04.000000 mpltWrappers-0.0.1rc2/src/mpltWrappers.egg-info/SOURCES.txt
--rw-r--r--   0 cahit.kargi   (502) staff       (20)        1 2023-04-13 10:26:04.000000 mpltWrappers-0.0.1rc2/src/mpltWrappers.egg-info/dependency_links.txt
--rw-r--r--   0 cahit.kargi   (502) staff       (20)       17 2023-04-13 10:26:04.000000 mpltWrappers-0.0.1rc2/src/mpltWrappers.egg-info/requires.txt
--rw-r--r--   0 cahit.kargi   (502) staff       (20)       13 2023-04-13 10:26:04.000000 mpltWrappers-0.0.1rc2/src/mpltWrappers.egg-info/top_level.txt
+drwxr-xr-x   0 cahit.kargi   (502) staff       (20)        0 2023-04-13 15:24:40.463426 mpltWrappers-0.0.1rc3/
+-rw-r--r--   0 cahit.kargi   (502) staff       (20)       41 2023-04-13 10:08:58.000000 mpltWrappers-0.0.1rc3/MANIFEST.in
+-rw-r--r--   0 cahit.kargi   (502) staff       (20)     1245 2023-04-13 15:24:40.463489 mpltWrappers-0.0.1rc3/PKG-INFO
+-rw-r--r--   0 cahit.kargi   (502) staff       (20)       15 2023-04-13 10:02:53.000000 mpltWrappers-0.0.1rc3/README.md
+-rw-r--r--   0 cahit.kargi   (502) staff       (20)      104 2023-04-13 10:08:09.000000 mpltWrappers-0.0.1rc3/pyproject.toml
+-rw-r--r--   0 cahit.kargi   (502) staff       (20)       17 2023-04-13 09:59:35.000000 mpltWrappers-0.0.1rc3/requirements.txt
+-rw-r--r--   0 cahit.kargi   (502) staff       (20)     1360 2023-04-13 15:24:40.463796 mpltWrappers-0.0.1rc3/setup.cfg
+drwxr-xr-x   0 cahit.kargi   (502) staff       (20)        0 2023-04-13 15:24:40.460204 mpltWrappers-0.0.1rc3/src/
+drwxr-xr-x   0 cahit.kargi   (502) staff       (20)        0 2023-04-13 15:24:40.462324 mpltWrappers-0.0.1rc3/src/mpltWrappers/
+-rw-r--r--   0 cahit.kargi   (502) staff       (20)      130 2023-04-13 09:59:35.000000 mpltWrappers-0.0.1rc3/src/mpltWrappers/__init__.py
+-rw-r--r--   0 cahit.kargi   (502) staff       (20)     3690 2023-04-13 09:59:35.000000 mpltWrappers-0.0.1rc3/src/mpltWrappers/colorFuncs.py
+-rw-r--r--   0 cahit.kargi   (502) staff       (20)     3797 2023-04-13 09:59:35.000000 mpltWrappers-0.0.1rc3/src/mpltWrappers/colorPlots.py
+-rw-r--r--   0 cahit.kargi   (502) staff       (20)     2444 2023-04-13 09:59:35.000000 mpltWrappers-0.0.1rc3/src/mpltWrappers/figCreate.py
+-rw-r--r--   0 cahit.kargi   (502) staff       (20)     1163 2023-04-13 09:59:35.000000 mpltWrappers-0.0.1rc3/src/mpltWrappers/linePlots.py
+-rw-r--r--   0 cahit.kargi   (502) staff       (20)     6477 2023-04-13 15:23:22.000000 mpltWrappers-0.0.1rc3/src/mpltWrappers/plotSettings.py
+drwxr-xr-x   0 cahit.kargi   (502) staff       (20)        0 2023-04-13 15:24:40.463159 mpltWrappers-0.0.1rc3/src/mpltWrappers.egg-info/
+-rw-r--r--   0 cahit.kargi   (502) staff       (20)     1245 2023-04-13 15:24:40.000000 mpltWrappers-0.0.1rc3/src/mpltWrappers.egg-info/PKG-INFO
+-rw-r--r--   0 cahit.kargi   (502) staff       (20)      446 2023-04-13 15:24:40.000000 mpltWrappers-0.0.1rc3/src/mpltWrappers.egg-info/SOURCES.txt
+-rw-r--r--   0 cahit.kargi   (502) staff       (20)        1 2023-04-13 15:24:40.000000 mpltWrappers-0.0.1rc3/src/mpltWrappers.egg-info/dependency_links.txt
+-rw-r--r--   0 cahit.kargi   (502) staff       (20)       17 2023-04-13 15:24:40.000000 mpltWrappers-0.0.1rc3/src/mpltWrappers.egg-info/requires.txt
+-rw-r--r--   0 cahit.kargi   (502) staff       (20)       13 2023-04-13 15:24:40.000000 mpltWrappers-0.0.1rc3/src/mpltWrappers.egg-info/top_level.txt
```

### Comparing `mpltWrappers-0.0.1rc2/PKG-INFO` & `mpltWrappers-0.0.1rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpltWrappers
-Version: 0.0.1rc2
+Version: 0.0.1rc3
 Summary: Simple wrapper functions around matplotlib to create consistent and better looking figures
 Home-page: https://github.com/cahitkargi/python_plotting_helpers
 Author: Cahit Kargi
 Author-email: ckargi88@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://github.com/cahitkargi/python_plotting_helpers/blob/main/src/mpltWrappers/Tutorials/demo.ipynb
 Project-URL: Source Code, https://github.com/cahitkargi/python_plotting_helpers
```

### Comparing `mpltWrappers-0.0.1rc2/setup.cfg` & `mpltWrappers-0.0.1rc3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mpltWrappers
-version = 0.0.1rc2
+version = 0.0.1rc3
 author = Cahit Kargi
 author_email = ckargi88@gmail.com
 description = Simple wrapper functions around matplotlib to create consistent and better looking figures
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = plotting
 license = BSD 3-Clause License
```

### Comparing `mpltWrappers-0.0.1rc2/src/mpltWrappers/colorFuncs.py` & `mpltWrappers-0.0.1rc3/src/mpltWrappers/colorFuncs.py`

 * *Files identical despite different names*

### Comparing `mpltWrappers-0.0.1rc2/src/mpltWrappers/colorPlots.py` & `mpltWrappers-0.0.1rc3/src/mpltWrappers/colorPlots.py`

 * *Files identical despite different names*

### Comparing `mpltWrappers-0.0.1rc2/src/mpltWrappers/figCreate.py` & `mpltWrappers-0.0.1rc3/src/mpltWrappers/figCreate.py`

 * *Files identical despite different names*

### Comparing `mpltWrappers-0.0.1rc2/src/mpltWrappers/linePlots.py` & `mpltWrappers-0.0.1rc3/src/mpltWrappers/linePlots.py`

 * *Files identical despite different names*

### Comparing `mpltWrappers-0.0.1rc2/src/mpltWrappers/plotSettings.py` & `mpltWrappers-0.0.1rc3/src/mpltWrappers/plotSettings.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
     if not yonly:
         for tick in ax.xaxis.get_major_ticks():
             tick.label.set_fontsize(fontsize)
 
     for tick in ax.yaxis.get_major_ticks():
         tick.label.set_fontsize(fontsize)
 
-def createLegend(ax, **kwargs):
+def createLegend(ax, *args, **kwargs):
     """
     Creates a legend for the given axes and pplies certain settings to the legend.
     You can use any kwargs for legend settings to overwrite the default values or modify futher.
 
     Parameters
     ----------
     ax : axes
@@ -146,15 +146,15 @@
         'columnspacing':0.5,
         'labelcolor':'linecolor',
         'ncol':3,
         'handleheight':1,
         'labelspacing':0.2,
         'prop':dict(size=8)
     }
-    leg = ax.legend(**kwargs, **{k:v for k, v in defaultKwargs.items() if k not in kwargs})
+    leg = ax.legend(*args, **kwargs, **{k:v for k, v in defaultKwargs.items() if k not in kwargs})
     for line in leg.get_lines():
         line.set_linewidth(1)
     return leg
 
 def rcSettings():
     """
     Upon calling, this function changes some of the default matplotlib configurations.
```

### Comparing `mpltWrappers-0.0.1rc2/src/mpltWrappers.egg-info/PKG-INFO` & `mpltWrappers-0.0.1rc3/src/mpltWrappers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpltWrappers
-Version: 0.0.1rc2
+Version: 0.0.1rc3
 Summary: Simple wrapper functions around matplotlib to create consistent and better looking figures
 Home-page: https://github.com/cahitkargi/python_plotting_helpers
 Author: Cahit Kargi
 Author-email: ckargi88@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://github.com/cahitkargi/python_plotting_helpers/blob/main/src/mpltWrappers/Tutorials/demo.ipynb
 Project-URL: Source Code, https://github.com/cahitkargi/python_plotting_helpers
```

