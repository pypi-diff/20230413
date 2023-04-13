# Comparing `tmp/ParticlePhaseSpace-0.5.2.tar.gz` & `tmp/ParticlePhaseSpace-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ParticlePhaseSpace-0.5.2.tar", last modified: Tue Apr  4 04:59:46 2023, max compression
+gzip compressed data, was "ParticlePhaseSpace-0.5.3.tar", last modified: Thu Apr 13 01:55:07 2023, max compression
```

## Comparing `ParticlePhaseSpace-0.5.2.tar` & `ParticlePhaseSpace-0.5.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:59:46.502036 ParticlePhaseSpace-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-04 04:59:35.000000 ParticlePhaseSpace-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-04 04:59:46.502036 ParticlePhaseSpace-0.5.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:59:46.498036 ParticlePhaseSpace-0.5.2/ParticlePhaseSpace/
--rw-r--r--   0 runner    (1001) docker     (123)    12310 2023-04-04 04:59:35.000000 ParticlePhaseSpace-0.5.2/ParticlePhaseSpace/DataExporters.py
--rw-r--r--   0 runner    (1001) docker     (123)    29289 2023-04-04 04:59:35.000000 ParticlePhaseSpace-0.5.2/ParticlePhaseSpace/DataLoaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    81893 2023-04-04 04:59:35.000000 ParticlePhaseSpace-0.5.2/ParticlePhaseSpace/_ParticlePhaseSpace.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-04 04:59:35.000000 ParticlePhaseSpace-0.5.2/ParticlePhaseSpace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-04 04:59:35.000000 ParticlePhaseSpace-0.5.2/ParticlePhaseSpace/__particle_config__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-04 04:59:35.000000 ParticlePhaseSpace-0.5.2/ParticlePhaseSpace/__phase_space_config__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-04-04 04:59:35.000000 ParticlePhaseSpace-0.5.2/ParticlePhaseSpace/__unit_config__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-04 04:59:35.000000 ParticlePhaseSpace-0.5.2/ParticlePhaseSpace/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:59:46.502036 ParticlePhaseSpace-0.5.2/ParticlePhaseSpace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-04 04:59:46.000000 ParticlePhaseSpace-0.5.2/ParticlePhaseSpace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-04 04:59:46.000000 ParticlePhaseSpace-0.5.2/ParticlePhaseSpace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 04:59:46.000000 ParticlePhaseSpace-0.5.2/ParticlePhaseSpace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-04 04:59:46.000000 ParticlePhaseSpace-0.5.2/ParticlePhaseSpace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-04 04:59:46.000000 ParticlePhaseSpace-0.5.2/ParticlePhaseSpace.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-04 04:59:35.000000 ParticlePhaseSpace-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-04 04:59:35.000000 ParticlePhaseSpace-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-04 04:59:46.502036 ParticlePhaseSpace-0.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 04:59:46.502036 ParticlePhaseSpace-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    16235 2023-04-04 04:59:35.000000 ParticlePhaseSpace-0.5.2/tests/test_ParticlePhaseSpace.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-04-04 04:59:35.000000 ParticlePhaseSpace-0.5.2/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-04-04 04:59:35.000000 ParticlePhaseSpace-0.5.2/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-04 04:59:35.000000 ParticlePhaseSpace-0.5.2/tests/test_notebooks_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-04 04:59:35.000000 ParticlePhaseSpace-0.5.2/tests/test_phase_space_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-04 04:59:35.000000 ParticlePhaseSpace-0.5.2/tests/test_supported_particles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-04-04 04:59:35.000000 ParticlePhaseSpace-0.5.2/tests/test_unit_conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:55:07.657383 ParticlePhaseSpace-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-13 01:55:07.657383 ParticlePhaseSpace-0.5.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:55:07.653383 ParticlePhaseSpace-0.5.3/ParticlePhaseSpace/
+-rw-r--r--   0 runner    (1001) docker     (123)    12310 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/ParticlePhaseSpace/DataExporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29289 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/ParticlePhaseSpace/DataLoaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82041 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/ParticlePhaseSpace/_ParticlePhaseSpace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/ParticlePhaseSpace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/ParticlePhaseSpace/__particle_config__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/ParticlePhaseSpace/__phase_space_config__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/ParticlePhaseSpace/__unit_config__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/ParticlePhaseSpace/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:55:07.653383 ParticlePhaseSpace-0.5.3/ParticlePhaseSpace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-13 01:55:07.000000 ParticlePhaseSpace-0.5.3/ParticlePhaseSpace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-13 01:55:07.000000 ParticlePhaseSpace-0.5.3/ParticlePhaseSpace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 01:55:07.000000 ParticlePhaseSpace-0.5.3/ParticlePhaseSpace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-13 01:55:07.000000 ParticlePhaseSpace-0.5.3/ParticlePhaseSpace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-13 01:55:07.000000 ParticlePhaseSpace-0.5.3/ParticlePhaseSpace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-13 01:55:07.657383 ParticlePhaseSpace-0.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:55:07.657383 ParticlePhaseSpace-0.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    16235 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/tests/test_ParticlePhaseSpace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/tests/test_notebooks_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/tests/test_phase_space_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/tests/test_supported_particles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/tests/test_unit_conversions.py
```

### Comparing `ParticlePhaseSpace-0.5.2/LICENSE` & `ParticlePhaseSpace-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.2/PKG-INFO` & `ParticlePhaseSpace-0.5.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,12 @@
-Metadata-Version: 2.1
-Name: ParticlePhaseSpace
-Version: 0.5.2
-Summary: Import, analyze, manipulate, and export particle phase space data
-Home-page: https://github.com/bwheelz36/ParticlePhaseSpace
-Author: Brendan Whelan
-Author-email: bwheelz36@gmail.com
-Project-URL: Bug Tracker, https://github.com/bwheelz36/ParticlePhaseSpace/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ParticlePhaseSpace
 
 ![tests](https://github.com/bwheelz36/ParticlePhaseSpace/actions/workflows/run_tests.yml/badge.svg)![tests](https://github.com/bwheelz36/ParticlePhaseSpace/actions/workflows/build_docs.yml/badge.svg)[![codecov](https://codecov.io/gh/bwheelz36/ParticlePhaseSpace/branch/main/graph/badge.svg?token=T44KBJ7INR)](https://codecov.io/gh/bwheelz36/ParticlePhaseSpace)[![PyPI version](https://badge.fury.io/py/ParticlePhaseSpace.svg)](https://badge.fury.io/py/ParticlePhaseSpace)
 
-Common library for dealing with particle phase spaces. This library supports the read in, analysis, and export of particle phase space data with extesnible support for different unit sets.
-It also provides an extensible mechanisms for the import and export of phase space data in different formats.
+Common library for dealing with particle phase spaces, revolving around the simple workflow of `import`, `analyse`, `export`. If you have a data format that we can't already work with, extension mechanisms are provided for writing new `DataLoaders` and `DataExporters`.
 
 ## Install and Requirements
 
 To install: ```pip install ParticlePhaseSpace```
 
 ## Usage and Documentation
```

### Comparing `ParticlePhaseSpace-0.5.2/ParticlePhaseSpace/DataExporters.py` & `ParticlePhaseSpace-0.5.3/ParticlePhaseSpace/DataExporters.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.2/ParticlePhaseSpace/DataLoaders.py` & `ParticlePhaseSpace-0.5.3/ParticlePhaseSpace/DataLoaders.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.2/ParticlePhaseSpace/_ParticlePhaseSpace.py` & `ParticlePhaseSpace-0.5.3/ParticlePhaseSpace/_ParticlePhaseSpace.py`

 * *Files 0% similar despite different names*

```diff
@@ -1391,15 +1391,16 @@
         """
         ind = np.logical_and(self._ps_data[self.columns['time']] >= t_start,
                              self._ps_data[self.columns['time']] <= t_finish)
         new_PS = self.filter_by_boolean_index(ind, in_place=in_place)
         return new_PS
 
 
-    def filter_by_boolean_index(self, boolean_index, in_place: bool = False, split: bool = False):
+    def filter_by_boolean_index(self, boolean_index, in_place: bool = False, split: bool = False,
+                                verbose: bool=True):
         """
         filter data by input boolean index, keeping 'True' and discarding 'False'
 
         :param boolean_index: an 1D array like structure of True and False values
         :param in_place: if True, existing object is modified; if False a new object is returned
         :param split: if True, will return two phase space objects: one where boolan_index=True and one where it equals
             False
@@ -1412,26 +1413,29 @@
             ps_data = self.ps_data[boolean_index].reset_index().drop('index', axis=1)
             ps_data = DataLoaders.Load_PandasData(ps_data, units=self._units)
             boolean_index_true_PS = PhaseSpace(ps_data)
 
             ps_data = self.ps_data[np.logical_not(boolean_index)].reset_index().drop('index', axis=1)
             ps_data = DataLoaders.Load_PandasData(ps_data, units=self._units)
             boolean_index_false_PS = PhaseSpace(ps_data)
-            print(f'data where boolean_index=True accounts for'
-                  f' {(np.count_nonzero(boolean_index) * 100 / len(boolean_index)): 1.1f} %'
-                  f' of the original data')
-            return boolean_index_true_PS, boolean_index_false_PS
+            if verbose:
+                print(f'data where boolean_index=True accounts for'
+                      f' {(np.count_nonzero(boolean_index) * 100 / len(boolean_index)): 1.1f} %'
+                      f' of the original data')
+                return boolean_index_true_PS, boolean_index_false_PS
         if in_place:
             self.ps_data = self.ps_data[boolean_index].reset_index().drop('index', axis=1)
-            print(f'removed {100 - (np.count_nonzero(boolean_index) * 100 / len(boolean_index)): 1.1f} % of particles')
+            if verbose:
+                print(f'removed {100 - (np.count_nonzero(boolean_index) * 100 / len(boolean_index)): 1.1f} % of particles')
         else:
             ps_data = self.ps_data[boolean_index].reset_index().drop('index', axis=1)
             ps_data = DataLoaders.Load_PandasData(ps_data, units=self._units)
             new_PS = PhaseSpace(ps_data)
-            print(f'removed {100 - (np.count_nonzero(boolean_index) * 100 / len(boolean_index)): 1.1f} % of particles')
+            if verbose:
+                print(f'removed {100 - (np.count_nonzero(boolean_index) * 100 / len(boolean_index)): 1.1f} % of particles')
             return new_PS
 
     def set_units(self, new_units: UnitSet):
         """
         converts ps_data to a new unit set.
         This will also reset the phase space to just the required columns
```

### Comparing `ParticlePhaseSpace-0.5.2/ParticlePhaseSpace/__particle_config__.py` & `ParticlePhaseSpace-0.5.3/ParticlePhaseSpace/__particle_config__.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.2/ParticlePhaseSpace/__phase_space_config__.py` & `ParticlePhaseSpace-0.5.3/ParticlePhaseSpace/__phase_space_config__.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.2/ParticlePhaseSpace/__unit_config__.py` & `ParticlePhaseSpace-0.5.3/ParticlePhaseSpace/__unit_config__.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.2/ParticlePhaseSpace/utilities.py` & `ParticlePhaseSpace-0.5.3/ParticlePhaseSpace/utilities.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.2/ParticlePhaseSpace.egg-info/SOURCES.txt` & `ParticlePhaseSpace-0.5.3/ParticlePhaseSpace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.2/README.md` & `ParticlePhaseSpace-0.5.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,26 @@
+Metadata-Version: 2.1
+Name: ParticlePhaseSpace
+Version: 0.5.3
+Summary: Import, analyze, manipulate, and export particle phase space data
+Home-page: https://github.com/bwheelz36/ParticlePhaseSpace
+Author: Brendan Whelan
+Author-email: bwheelz36@gmail.com
+Project-URL: Bug Tracker, https://github.com/bwheelz36/ParticlePhaseSpace/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # ParticlePhaseSpace
 
 ![tests](https://github.com/bwheelz36/ParticlePhaseSpace/actions/workflows/run_tests.yml/badge.svg)![tests](https://github.com/bwheelz36/ParticlePhaseSpace/actions/workflows/build_docs.yml/badge.svg)[![codecov](https://codecov.io/gh/bwheelz36/ParticlePhaseSpace/branch/main/graph/badge.svg?token=T44KBJ7INR)](https://codecov.io/gh/bwheelz36/ParticlePhaseSpace)[![PyPI version](https://badge.fury.io/py/ParticlePhaseSpace.svg)](https://badge.fury.io/py/ParticlePhaseSpace)
 
-Common library for dealing with particle phase spaces. This library supports the read in, analysis, and export of particle phase space data with extesnible support for different unit sets.
-It also provides an extensible mechanisms for the import and export of phase space data in different formats.
+Common library for dealing with particle phase spaces, revolving around the simple workflow of `import`, `analyse`, `export`. If you have a data format that we can't already work with, extension mechanisms are provided for writing new `DataLoaders` and `DataExporters`.
 
 ## Install and Requirements
 
 To install: ```pip install ParticlePhaseSpace```
 
 ## Usage and Documentation
```

### Comparing `ParticlePhaseSpace-0.5.2/setup.cfg` & `ParticlePhaseSpace-0.5.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.2/tests/test_ParticlePhaseSpace.py` & `ParticlePhaseSpace-0.5.3/tests/test_ParticlePhaseSpace.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.2/tests/test_export.py` & `ParticlePhaseSpace-0.5.3/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.2/tests/test_import.py` & `ParticlePhaseSpace-0.5.3/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.2/tests/test_notebooks_run.py` & `ParticlePhaseSpace-0.5.3/tests/test_notebooks_run.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.2/tests/test_phase_space_config.py` & `ParticlePhaseSpace-0.5.3/tests/test_phase_space_config.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.2/tests/test_supported_particles.py` & `ParticlePhaseSpace-0.5.3/tests/test_supported_particles.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.2/tests/test_unit_conversions.py` & `ParticlePhaseSpace-0.5.3/tests/test_unit_conversions.py`

 * *Files identical despite different names*

