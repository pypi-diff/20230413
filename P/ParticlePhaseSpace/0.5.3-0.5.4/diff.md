# Comparing `tmp/ParticlePhaseSpace-0.5.3.tar.gz` & `tmp/ParticlePhaseSpace-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ParticlePhaseSpace-0.5.3.tar", last modified: Thu Apr 13 01:55:07 2023, max compression
+gzip compressed data, was "ParticlePhaseSpace-0.5.4.tar", last modified: Thu Apr 13 05:44:44 2023, max compression
```

## Comparing `ParticlePhaseSpace-0.5.3.tar` & `ParticlePhaseSpace-0.5.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:55:07.657383 ParticlePhaseSpace-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-13 01:55:07.657383 ParticlePhaseSpace-0.5.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:55:07.653383 ParticlePhaseSpace-0.5.3/ParticlePhaseSpace/
--rw-r--r--   0 runner    (1001) docker     (123)    12310 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/ParticlePhaseSpace/DataExporters.py
--rw-r--r--   0 runner    (1001) docker     (123)    29289 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/ParticlePhaseSpace/DataLoaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    82041 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/ParticlePhaseSpace/_ParticlePhaseSpace.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/ParticlePhaseSpace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/ParticlePhaseSpace/__particle_config__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/ParticlePhaseSpace/__phase_space_config__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/ParticlePhaseSpace/__unit_config__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/ParticlePhaseSpace/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:55:07.653383 ParticlePhaseSpace-0.5.3/ParticlePhaseSpace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-13 01:55:07.000000 ParticlePhaseSpace-0.5.3/ParticlePhaseSpace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-13 01:55:07.000000 ParticlePhaseSpace-0.5.3/ParticlePhaseSpace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 01:55:07.000000 ParticlePhaseSpace-0.5.3/ParticlePhaseSpace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-13 01:55:07.000000 ParticlePhaseSpace-0.5.3/ParticlePhaseSpace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-13 01:55:07.000000 ParticlePhaseSpace-0.5.3/ParticlePhaseSpace.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-13 01:55:07.657383 ParticlePhaseSpace-0.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:55:07.657383 ParticlePhaseSpace-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    16235 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/tests/test_ParticlePhaseSpace.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/tests/test_notebooks_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/tests/test_phase_space_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/tests/test_supported_particles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-04-13 01:54:57.000000 ParticlePhaseSpace-0.5.3/tests/test_unit_conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 05:44:44.399226 ParticlePhaseSpace-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 05:44:30.000000 ParticlePhaseSpace-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-13 05:44:44.399226 ParticlePhaseSpace-0.5.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 05:44:44.395226 ParticlePhaseSpace-0.5.4/ParticlePhaseSpace/
+-rw-r--r--   0 runner    (1001) docker     (123)    12310 2023-04-13 05:44:30.000000 ParticlePhaseSpace-0.5.4/ParticlePhaseSpace/DataExporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29377 2023-04-13 05:44:30.000000 ParticlePhaseSpace-0.5.4/ParticlePhaseSpace/DataLoaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82041 2023-04-13 05:44:30.000000 ParticlePhaseSpace-0.5.4/ParticlePhaseSpace/_ParticlePhaseSpace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-13 05:44:30.000000 ParticlePhaseSpace-0.5.4/ParticlePhaseSpace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-13 05:44:30.000000 ParticlePhaseSpace-0.5.4/ParticlePhaseSpace/__particle_config__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-13 05:44:30.000000 ParticlePhaseSpace-0.5.4/ParticlePhaseSpace/__phase_space_config__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-04-13 05:44:30.000000 ParticlePhaseSpace-0.5.4/ParticlePhaseSpace/__unit_config__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-13 05:44:30.000000 ParticlePhaseSpace-0.5.4/ParticlePhaseSpace/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 05:44:44.395226 ParticlePhaseSpace-0.5.4/ParticlePhaseSpace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-13 05:44:44.000000 ParticlePhaseSpace-0.5.4/ParticlePhaseSpace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-13 05:44:44.000000 ParticlePhaseSpace-0.5.4/ParticlePhaseSpace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 05:44:44.000000 ParticlePhaseSpace-0.5.4/ParticlePhaseSpace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-13 05:44:44.000000 ParticlePhaseSpace-0.5.4/ParticlePhaseSpace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-13 05:44:44.000000 ParticlePhaseSpace-0.5.4/ParticlePhaseSpace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-13 05:44:30.000000 ParticlePhaseSpace-0.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 05:44:30.000000 ParticlePhaseSpace-0.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-13 05:44:44.399226 ParticlePhaseSpace-0.5.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 05:44:44.399226 ParticlePhaseSpace-0.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17389 2023-04-13 05:44:30.000000 ParticlePhaseSpace-0.5.4/tests/test_ParticlePhaseSpace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-04-13 05:44:30.000000 ParticlePhaseSpace-0.5.4/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-04-13 05:44:30.000000 ParticlePhaseSpace-0.5.4/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-13 05:44:30.000000 ParticlePhaseSpace-0.5.4/tests/test_notebooks_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-13 05:44:30.000000 ParticlePhaseSpace-0.5.4/tests/test_phase_space_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-13 05:44:30.000000 ParticlePhaseSpace-0.5.4/tests/test_supported_particles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-04-13 05:44:30.000000 ParticlePhaseSpace-0.5.4/tests/test_unit_conversions.py
```

### Comparing `ParticlePhaseSpace-0.5.3/LICENSE` & `ParticlePhaseSpace-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.3/PKG-INFO` & `ParticlePhaseSpace-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ParticlePhaseSpace
-Version: 0.5.3
+Version: 0.5.4
 Summary: Import, analyze, manipulate, and export particle phase space data
 Home-page: https://github.com/bwheelz36/ParticlePhaseSpace
 Author: Brendan Whelan
 Author-email: bwheelz36@gmail.com
 Project-URL: Bug Tracker, https://github.com/bwheelz36/ParticlePhaseSpace/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `ParticlePhaseSpace-0.5.3/ParticlePhaseSpace/DataExporters.py` & `ParticlePhaseSpace-0.5.4/ParticlePhaseSpace/DataExporters.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.3/ParticlePhaseSpace/DataLoaders.py` & `ParticlePhaseSpace-0.5.4/ParticlePhaseSpace/DataLoaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,16 +91,17 @@
         # are NaNs present?
         if self.data.isnull().values.any():
             NaN_cols = self.data.columns[self.data.isna().any()].tolist()
             raise AttributeError(f'input data may not contain NaNs; the following columns contain NaN:'
                                  f'\n{NaN_cols}')
 
         tot_mom = np.sqrt(self.data[self._columns['px']]**2 + self.data[self._columns['py']]**2 + self.data[self._columns['pz']]**2)
-        if not np.min(tot_mom)>0:
-            raise Exception('particles with zero absolute momentum make no sense')
+        if not np.min(tot_mom) > 0:
+            ind = tot_mom <= 0
+            warnings.warn(f'{np.count_nonzero(ind)} particles have zero absolute momentum; this makes no sense and they will be removed')
 
         # is every particle ID unique?
         if not len(self.data[self._columns['particle id']].unique()) == len(self.data[self._columns['particle id']]):
             raise Exception('you have attempted to create a data set with non'
                                  'unique "particle id" fields, which is not allowed')
 
         #all pdg codes valid?
```

### Comparing `ParticlePhaseSpace-0.5.3/ParticlePhaseSpace/_ParticlePhaseSpace.py` & `ParticlePhaseSpace-0.5.4/ParticlePhaseSpace/_ParticlePhaseSpace.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.3/ParticlePhaseSpace/__particle_config__.py` & `ParticlePhaseSpace-0.5.4/ParticlePhaseSpace/__particle_config__.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.3/ParticlePhaseSpace/__phase_space_config__.py` & `ParticlePhaseSpace-0.5.4/ParticlePhaseSpace/__phase_space_config__.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.3/ParticlePhaseSpace/__unit_config__.py` & `ParticlePhaseSpace-0.5.4/ParticlePhaseSpace/__unit_config__.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.3/ParticlePhaseSpace/utilities.py` & `ParticlePhaseSpace-0.5.4/ParticlePhaseSpace/utilities.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.3/ParticlePhaseSpace.egg-info/PKG-INFO` & `ParticlePhaseSpace-0.5.4/ParticlePhaseSpace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ParticlePhaseSpace
-Version: 0.5.3
+Version: 0.5.4
 Summary: Import, analyze, manipulate, and export particle phase space data
 Home-page: https://github.com/bwheelz36/ParticlePhaseSpace
 Author: Brendan Whelan
 Author-email: bwheelz36@gmail.com
 Project-URL: Bug Tracker, https://github.com/bwheelz36/ParticlePhaseSpace/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `ParticlePhaseSpace-0.5.3/ParticlePhaseSpace.egg-info/SOURCES.txt` & `ParticlePhaseSpace-0.5.4/ParticlePhaseSpace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.3/README.md` & `ParticlePhaseSpace-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.3/setup.cfg` & `ParticlePhaseSpace-0.5.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.3/tests/test_ParticlePhaseSpace.py` & `ParticlePhaseSpace-0.5.4/tests/test_ParticlePhaseSpace.py`

 * *Files 6% similar despite different names*

```diff
@@ -391,8 +391,41 @@
     assert np.allclose(PS.ps_data['pz [MeV/c]'], PS_rotate.ps_data['py [MeV/c]'])
     assert np.allclose(PS.ps_data['z [mm]'], PS_rotate.ps_data['y [mm]'])
     PS_rotate = PS.transform.rotate(rotation_axis='y', angle=-90, rotate_momentum_vector=True)
     assert np.allclose(PS.ps_data['px [MeV/c]'], PS_rotate.ps_data['pz [MeV/c]'])
     assert np.allclose(PS.ps_data['x [mm]'], PS_rotate.ps_data['z [mm]'])
     PS_rotate = PS.transform.rotate(rotation_axis='z', angle=90, rotate_momentum_vector=True)
     assert np.allclose(PS.ps_data['px [MeV/c]'], PS_rotate.ps_data['py [MeV/c]'])
-    assert np.allclose(PS.ps_data['x [mm]'], PS_rotate.ps_data['y [mm]'])
+    assert np.allclose(PS.ps_data['x [mm]'], PS_rotate.ps_data['y [mm]'])
+
+
+def test_zero_momentum_particle():
+    """
+    occasionally due to precision issues, particles are read in with
+    zero absolute momnentum. I just want to make sure such cases still
+    run
+    :return:
+    """
+
+    units = ParticlePhaseSpaceUnits()('mm_MeV')
+    all_allowed_columns = ps_cfg.get_all_column_names(units)
+    demo_data = pd.DataFrame(
+        {all_allowed_columns['x']: [0., 1., 2.],
+         all_allowed_columns['y']: [2., 3., 4.],
+         all_allowed_columns['z']: [5., 6., 7.],
+         all_allowed_columns['px']: [1000, 1000, 0],
+         all_allowed_columns['py']: [1000, 1000, 0],
+         all_allowed_columns['pz']: [10000, 100000, 0],
+         all_allowed_columns['particle type']: [11, 11, 11],
+         all_allowed_columns['weight']: [1, 1, 2],
+         all_allowed_columns['particle id']: [0, 1, 2],
+         all_allowed_columns['time']: [0, 0, 0]})
+
+    data = DataLoaders.Load_PandasData(demo_data)
+    PS = PhaseSpace(data)
+    PS.fill.absolute_momentum()
+    PS.fill.beta_and_gamma()
+    PS.fill.direction_cosines()
+    PS.fill.kinetic_E()
+    PS.fill.relativistic_mass()
+    PS.fill.rest_mass()
+    PS.fill.velocity()
```

### Comparing `ParticlePhaseSpace-0.5.3/tests/test_export.py` & `ParticlePhaseSpace-0.5.4/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.3/tests/test_import.py` & `ParticlePhaseSpace-0.5.4/tests/test_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
          'pz [MeV/c]': [0, 1, 2],
          'particle type [pdg_code]': [11, 11, 11],
          'weight': [0, 1, 2],
          'particle id': [0, 1, 2],
          'time [ps]': [0, 1, 2]})
 
     with pytest.raises(Exception):
-        data = DataLoaders.Load_PandasData(demo_data)
+        data = DataLoaders.Load_PandasData(demo_data, particle_type='electrons')
 
 
 def test_tibaray_import():
     data_loc = this_file_loc / 'test_data' / 'tibaray_test.dat'
     data = DataLoaders.Load_TibarayData(data_loc, particle_type='electrons')
     PS = PhaseSpace(data)
     # check that energy is stable
```

### Comparing `ParticlePhaseSpace-0.5.3/tests/test_notebooks_run.py` & `ParticlePhaseSpace-0.5.4/tests/test_notebooks_run.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.3/tests/test_phase_space_config.py` & `ParticlePhaseSpace-0.5.4/tests/test_phase_space_config.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.3/tests/test_supported_particles.py` & `ParticlePhaseSpace-0.5.4/tests/test_supported_particles.py`

 * *Files identical despite different names*

### Comparing `ParticlePhaseSpace-0.5.3/tests/test_unit_conversions.py` & `ParticlePhaseSpace-0.5.4/tests/test_unit_conversions.py`

 * *Files identical despite different names*

