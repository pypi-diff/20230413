# Comparing `tmp/bmcs_utils-0.0.8a0.tar.gz` & `tmp/bmcs_utils-0.0.9a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bmcs_utils-0.0.8a0.tar", last modified: Mon Oct 26 10:30:48 2020, max compression
+gzip compressed data, was "dist/bmcs_utils-0.0.9a0.tar", last modified: Mon Oct 26 18:00:50 2020, max compression
```

## Comparing `bmcs_utils-0.0.8a0.tar` & `bmcs_utils-0.0.9a0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 rch       (1001) rch       (1001)        0 2020-10-26 10:30:48.000000 bmcs_utils-0.0.8a0/
--rw-r--r--   0 rch       (1001) rch       (1001)     1567 2020-10-26 10:30:48.000000 bmcs_utils-0.0.8a0/PKG-INFO
--rw-r--r--   0 rch       (1001) rch       (1001)      715 2020-10-25 17:11:32.000000 bmcs_utils-0.0.8a0/README.md
-drwxr-xr-x   0 rch       (1001) rch       (1001)        0 2020-10-26 10:30:48.000000 bmcs_utils-0.0.8a0/bmcs_utils.egg-info/
--rw-r--r--   0 rch       (1001) rch       (1001)     1567 2020-10-26 10:30:48.000000 bmcs_utils-0.0.8a0/bmcs_utils.egg-info/PKG-INFO
--rw-r--r--   0 rch       (1001) rch       (1001)      374 2020-10-26 10:30:48.000000 bmcs_utils-0.0.8a0/bmcs_utils.egg-info/SOURCES.txt
--rw-r--r--   0 rch       (1001) rch       (1001)        1 2020-10-26 10:30:48.000000 bmcs_utils-0.0.8a0/bmcs_utils.egg-info/dependency_links.txt
--rw-r--r--   0 rch       (1001) rch       (1001)        7 2020-10-26 10:30:48.000000 bmcs_utils-0.0.8a0/bmcs_utils.egg-info/top_level.txt
-drwxr-xr-x   0 rch       (1001) rch       (1001)        0 2020-10-26 10:30:48.000000 bmcs_utils-0.0.8a0/models/
--rw-r--r--   0 rch       (1001) rch       (1001)        0 2020-09-05 11:19:58.000000 bmcs_utils-0.0.8a0/models/__init__.py
--rw-r--r--   0 rch       (1001) rch       (1001)     2621 2020-10-25 17:08:30.000000 bmcs_utils-0.0.8a0/models/editors.py
--rw-r--r--   0 rch       (1001) rch       (1001)    10124 2020-10-25 17:08:30.000000 bmcs_utils-0.0.8a0/models/interactive_window.py
--rw-r--r--   0 rch       (1001) rch       (1001)      428 2020-10-26 09:36:17.000000 bmcs_utils-0.0.8a0/models/interactive_window_example.py
--rw-r--r--   0 rch       (1001) rch       (1001)      807 2020-09-16 15:19:07.000000 bmcs_utils-0.0.8a0/models/mpl_utils.py
--rw-r--r--   0 rch       (1001) rch       (1001)     3440 2020-10-26 09:37:39.000000 bmcs_utils-0.0.8a0/models/symb_expr.py
--rw-r--r--   0 rch       (1001) rch       (1001)     1526 2020-10-26 09:38:03.000000 bmcs_utils-0.0.8a0/models/symb_expr_quad_example.py
--rw-r--r--   0 rch       (1001) rch       (1001)      930 2020-10-26 10:02:52.000000 bmcs_utils-0.0.8a0/models/test_editor.py
--rw-r--r--   0 rch       (1001) rch       (1001)      770 2020-10-26 09:38:52.000000 bmcs_utils-0.0.8a0/models/trait_types.py
--rw-r--r--   0 rch       (1001) rch       (1001)       38 2020-10-26 10:30:48.000000 bmcs_utils-0.0.8a0/setup.cfg
--rwxr-xr-x   0 rch       (1001) rch       (1001)     3781 2020-10-26 10:29:32.000000 bmcs_utils-0.0.8a0/setup.py
+drwxr-xr-x   0 rch       (1001) rch       (1001)        0 2020-10-26 18:00:50.000000 bmcs_utils-0.0.9a0/
+-rw-r--r--   0 rch       (1001) rch       (1001)     1571 2020-10-26 18:00:50.000000 bmcs_utils-0.0.9a0/PKG-INFO
+-rw-r--r--   0 rch       (1001) rch       (1001)      715 2020-10-25 17:11:32.000000 bmcs_utils-0.0.9a0/README.md
+drwxr-xr-x   0 rch       (1001) rch       (1001)        0 2020-10-26 18:00:50.000000 bmcs_utils-0.0.9a0/bmcs_utils/
+-rw-r--r--   0 rch       (1001) rch       (1001)        0 2020-09-05 11:19:58.000000 bmcs_utils-0.0.9a0/bmcs_utils/__init__.py
+-rw-r--r--   0 rch       (1001) rch       (1001)      401 2020-10-26 18:00:11.000000 bmcs_utils-0.0.9a0/bmcs_utils/api.py
+-rw-r--r--   0 rch       (1001) rch       (1001)     2621 2020-10-25 17:08:30.000000 bmcs_utils-0.0.9a0/bmcs_utils/editors.py
+-rw-r--r--   0 rch       (1001) rch       (1001)    10136 2020-10-26 17:58:17.000000 bmcs_utils-0.0.9a0/bmcs_utils/interactive_window.py
+-rw-r--r--   0 rch       (1001) rch       (1001)      436 2020-10-26 17:58:16.000000 bmcs_utils-0.0.9a0/bmcs_utils/interactive_window_example.py
+-rw-r--r--   0 rch       (1001) rch       (1001)      807 2020-09-16 15:19:07.000000 bmcs_utils-0.0.9a0/bmcs_utils/mpl_utils.py
+-rw-r--r--   0 rch       (1001) rch       (1001)     3440 2020-10-26 09:37:39.000000 bmcs_utils-0.0.9a0/bmcs_utils/symb_expr.py
+-rw-r--r--   0 rch       (1001) rch       (1001)     1530 2020-10-26 17:58:16.000000 bmcs_utils-0.0.9a0/bmcs_utils/symb_expr_quad_example.py
+-rw-r--r--   0 rch       (1001) rch       (1001)      938 2020-10-26 17:58:16.000000 bmcs_utils-0.0.9a0/bmcs_utils/test_editor.py
+-rw-r--r--   0 rch       (1001) rch       (1001)      774 2020-10-26 17:58:16.000000 bmcs_utils-0.0.9a0/bmcs_utils/trait_types.py
+drwxr-xr-x   0 rch       (1001) rch       (1001)        0 2020-10-26 18:00:50.000000 bmcs_utils-0.0.9a0/bmcs_utils.egg-info/
+-rw-r--r--   0 rch       (1001) rch       (1001)     1571 2020-10-26 18:00:50.000000 bmcs_utils-0.0.9a0/bmcs_utils.egg-info/PKG-INFO
+-rw-r--r--   0 rch       (1001) rch       (1001)      428 2020-10-26 18:00:50.000000 bmcs_utils-0.0.9a0/bmcs_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 rch       (1001) rch       (1001)        1 2020-10-26 18:00:50.000000 bmcs_utils-0.0.9a0/bmcs_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 rch       (1001) rch       (1001)       11 2020-10-26 18:00:50.000000 bmcs_utils-0.0.9a0/bmcs_utils.egg-info/top_level.txt
+-rw-r--r--   0 rch       (1001) rch       (1001)       38 2020-10-26 18:00:50.000000 bmcs_utils-0.0.9a0/setup.cfg
+-rwxr-xr-x   0 rch       (1001) rch       (1001)     3779 2020-10-26 17:58:16.000000 bmcs_utils-0.0.9a0/setup.py
```

### Comparing `bmcs_utils-0.0.8a0/PKG-INFO` & `bmcs_utils-0.0.9a0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: bmcs_utils
-Version: 0.0.8a0
-Summary: Suite of utilities for to implementation of models for brittle-matrix composites.
+Version: 0.0.9a0
+Summary: Suite of utilities for to implementation of bmcs_utils for brittle-matrix composites.
 Home-page: https://github.com/bmcs-group/bmcs_utils
 Author: BMCS-Group
 Author-email: rostislav.chudoba@rwt-aachen.de
 License: MIT
 Description: 
         
         # General utilities and practices
```

### Comparing `bmcs_utils-0.0.8a0/README.md` & `bmcs_utils-0.0.9a0/README.md`

 * *Files identical despite different names*

### Comparing `bmcs_utils-0.0.8a0/bmcs_utils.egg-info/PKG-INFO` & `bmcs_utils-0.0.9a0/bmcs_utils.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: bmcs-utils
-Version: 0.0.8a0
-Summary: Suite of utilities for to implementation of models for brittle-matrix composites.
+Version: 0.0.9a0
+Summary: Suite of utilities for to implementation of bmcs_utils for brittle-matrix composites.
 Home-page: https://github.com/bmcs-group/bmcs_utils
 Author: BMCS-Group
 Author-email: rostislav.chudoba@rwt-aachen.de
 License: MIT
 Description: 
         
         # General utilities and practices
```

### Comparing `bmcs_utils-0.0.8a0/models/editors.py` & `bmcs_utils-0.0.9a0/bmcs_utils/editors.py`

 * *Files identical despite different names*

### Comparing `bmcs_utils-0.0.8a0/models/interactive_window.py` & `bmcs_utils-0.0.9a0/bmcs_utils/interactive_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,20 +94,20 @@
             self.item_names.append(item.name)
 
     simulator = tr.Str
     """Name of the method running the model simulation
     """
 
 class IInteractiveModel(tr.Interface):
-    """Interface of interactive models"""
+    """Interface of interactive bmcs_utils"""
 
 
 @tr.provides(IInteractiveModel)
 class InteractiveModel(tr.HasTraits):
-    """Base class for interactive models
+    """Base class for interactive bmcs_utils
     """
 
     name = tr.Str("<unnamed>")
 
     def subplots(self, fig):
         return fig.subplots(1, 1)
 
@@ -167,15 +167,15 @@
         return self.tab
 
     def change_tab(self, change=None):
         index = self.tab.selected_index
         self.update_plot(index)
 
     def update_plot(self, index):
-        '''update the visualization with updated models'''
+        '''update the visualization with updated bmcs_utils'''
         self.fig.clf()
         self.axes = self.ipw_model_tabs[index].subplots(self.fig)
         _axes = self.axes
         if not hasattr(_axes, '__iter__'):
             _axes = [_axes]
         for ax in _axes:
             ax.clear()
```

### Comparing `bmcs_utils-0.0.8a0/models/mpl_utils.py` & `bmcs_utils-0.0.9a0/bmcs_utils/mpl_utils.py`

 * *Files identical despite different names*

### Comparing `bmcs_utils-0.0.8a0/models/symb_expr.py` & `bmcs_utils-0.0.9a0/bmcs_utils/symb_expr.py`

 * *Files identical despite different names*

### Comparing `bmcs_utils-0.0.8a0/models/symb_expr_quad_example.py` & `bmcs_utils-0.0.9a0/bmcs_utils/symb_expr_quad_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sympy as sp
 import traits.api as tr
 import numpy as np
-from models.symb_expr import SymbExpr, InjectSymbExpr
+from bmcs_utils.symb_expr import SymbExpr, InjectSymbExpr
 
 class QuadraticSym(SymbExpr):
     # -------------------------------------------------------------------------
     # Symbolic derivation of variables
     # -------------------------------------------------------------------------
     x = sp.Symbol(
         r'x', real=True,
```

### Comparing `bmcs_utils-0.0.8a0/models/test_editor.py` & `bmcs_utils-0.0.9a0/bmcs_utils/test_editor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from models.trait_types import \
+from bmcs_utils.trait_types import \
     Float, Int, Bool, FloatRangeEditor, Range
-from models.interactive_window import InteractiveModel, Item, View
+from bmcs_utils.interactive_window import InteractiveModel, Item, View
 import numpy as np
 
 class ExampleModel(InteractiveModel):
     name = 'Example'
 
     a = Float(0, desc=r'first material parameter')
     b = Int(5, desc='input parameter')
```

### Comparing `bmcs_utils-0.0.8a0/models/trait_types.py` & `bmcs_utils-0.0.9a0/bmcs_utils/trait_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import traits.api as tr
-from models.editors import \
+from bmcs_utils.editors import \
     IntEditor, BoolEditor, FloatEditor, FloatRangeEditor, \
     ProgressEditor, ButtonEditor
 
 ## Specialized traits
 class Int(tr.BaseInt):
     editor_factory = IntEditor
```

### Comparing `bmcs_utils-0.0.8a0/setup.py` & `bmcs_utils-0.0.9a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from shutil import rmtree
 
 from setuptools import find_packages, setup, Command
 from version import CURRENT_VERSION
 
 # Package meta-data.
 NAME = 'bmcs_utils'
-DESCRIPTION = "Suite of utilities for to implementation of models for brittle-matrix composites."
+DESCRIPTION = "Suite of utilities for to implementation of bmcs_utils for brittle-matrix composites."
 URL = 'https://github.com/bmcs-group/bmcs_utils'
 EMAIL = 'rostislav.chudoba@rwt-aachen.de'
 AUTHOR = 'BMCS-Group'
 REQUIRES_PYTHON = '>=3.6.0'
 VERSION = CURRENT_VERSION
 
 # What packages are required for this module to be executed?
@@ -81,17 +81,17 @@
 
         self.status('Building Source and Wheel (universal) distribution…')
         os.system('{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
 
         self.status('Uploading the package to PyPI via Twine…')
         os.system('twine upload dist/*')
 
-        # self.status('Pushing git tags…')
-        # os.system('git tag v{0}'.format(about['__version__']))
-        # os.system('git push --tags')
+        self.status('Pushing git tags…')
+        os.system('git tag v{0}'.format(about['__version__']))
+        os.system('git push --tags')
 
         sys.exit()
 
 
 # Where the magic happens:
 setup(
     name=NAME,
```

