# Comparing `tmp/cbmos-0.2.0.tar.gz` & `tmp/cbmos-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbmos-0.2.0.tar", last modified: Thu Dec 16 11:39:56 2021, max compression
+gzip compressed data, was "cbmos-0.3.0.tar", last modified: Thu Apr 13 12:55:31 2023, max compression
```

## Comparing `cbmos-0.2.0.tar` & `cbmos-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-16 11:39:56.631715 cbmos-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2021-12-16 11:39:49.000000 cbmos-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3894 2021-12-16 11:39:56.631715 cbmos-0.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-16 11:39:56.627715 cbmos-0.2.0/cbmos/
--rw-r--r--   0 runner    (1001) docker     (121)       99 2021-12-16 11:39:49.000000 cbmos-0.2.0/cbmos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-16 11:39:56.627715 cbmos-0.2.0/cbmos/cbmodel/
--rw-r--r--   0 runner    (1001) docker     (121)    13743 2021-12-16 11:39:49.000000 cbmos-0.2.0/cbmos/cbmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1557 2021-12-16 11:39:49.000000 cbmos-0.2.0/cbmos/cbmodel/_eventqueue.py
--rw-r--r--   0 runner    (1001) docker     (121)     2410 2021-12-16 11:39:49.000000 cbmos-0.2.0/cbmos/cell.py
--rw-r--r--   0 runner    (1001) docker     (121)     3447 2021-12-16 11:39:49.000000 cbmos-0.2.0/cbmos/events.py
--rw-r--r--   0 runner    (1001) docker     (121)     9411 2021-12-16 11:39:49.000000 cbmos-0.2.0/cbmos/force_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-16 11:39:56.631715 cbmos-0.2.0/cbmos/solvers/
--rw-r--r--   0 runner    (1001) docker     (121)      110 2021-12-16 11:39:49.000000 cbmos-0.2.0/cbmos/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      949 2021-12-16 11:39:49.000000 cbmos-0.2.0/cbmos/solvers/adams_bashforth.py
--rw-r--r--   0 runner    (1001) docker     (121)     4719 2021-12-16 11:39:49.000000 cbmos-0.2.0/cbmos/solvers/euler_backward.py
--rw-r--r--   0 runner    (1001) docker     (121)     1633 2021-12-16 11:39:49.000000 cbmos-0.2.0/cbmos/solvers/euler_forward.py
--rw-r--r--   0 runner    (1001) docker     (121)      846 2021-12-16 11:39:49.000000 cbmos-0.2.0/cbmos/solvers/heun.py
--rw-r--r--   0 runner    (1001) docker     (121)      834 2021-12-16 11:39:49.000000 cbmos-0.2.0/cbmos/solvers/midpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-16 11:39:56.631715 cbmos-0.2.0/cbmos/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     2936 2021-12-16 11:39:49.000000 cbmos-0.2.0/cbmos/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-16 11:39:56.627715 cbmos-0.2.0/cbmos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3894 2021-12-16 11:39:56.000000 cbmos-0.2.0/cbmos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      511 2021-12-16 11:39:56.000000 cbmos-0.2.0/cbmos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-16 11:39:56.000000 cbmos-0.2.0/cbmos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       54 2021-12-16 11:39:56.000000 cbmos-0.2.0/cbmos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-12-16 11:39:56.000000 cbmos-0.2.0/cbmos.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       90 2021-12-16 11:39:49.000000 cbmos-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      719 2021-12-16 11:39:56.631715 cbmos-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-12-16 11:39:49.000000 cbmos-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:55:31.300734 cbmos-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-13 12:55:20.000000 cbmos-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-04-13 12:55:31.300734 cbmos-0.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:55:31.300734 cbmos-0.3.0/cbmos/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-13 12:55:20.000000 cbmos-0.3.0/cbmos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:55:31.300734 cbmos-0.3.0/cbmos/cbmodel/
+-rw-r--r--   0 runner    (1001) docker     (123)    14657 2023-04-13 12:55:20.000000 cbmos-0.3.0/cbmos/cbmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-13 12:55:20.000000 cbmos-0.3.0/cbmos/cbmodel/_eventqueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-13 12:55:20.000000 cbmos-0.3.0/cbmos/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-04-13 12:55:20.000000 cbmos-0.3.0/cbmos/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13181 2023-04-13 12:55:20.000000 cbmos-0.3.0/cbmos/force_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:55:31.300734 cbmos-0.3.0/cbmos/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-13 12:55:20.000000 cbmos-0.3.0/cbmos/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-13 12:55:20.000000 cbmos-0.3.0/cbmos/solvers/adams_bashforth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-04-13 12:55:20.000000 cbmos-0.3.0/cbmos/solvers/euler_backward.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27126 2023-04-13 12:55:20.000000 cbmos-0.3.0/cbmos/solvers/euler_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-13 12:55:20.000000 cbmos-0.3.0/cbmos/solvers/geshgorin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-13 12:55:20.000000 cbmos-0.3.0/cbmos/solvers/heun.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-13 12:55:20.000000 cbmos-0.3.0/cbmos/solvers/midpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:55:31.300734 cbmos-0.3.0/cbmos/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-04-13 12:55:20.000000 cbmos-0.3.0/cbmos/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:55:31.300734 cbmos-0.3.0/cbmos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-04-13 12:55:31.000000 cbmos-0.3.0/cbmos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-13 12:55:31.000000 cbmos-0.3.0/cbmos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 12:55:31.000000 cbmos-0.3.0/cbmos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-13 12:55:31.000000 cbmos-0.3.0/cbmos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 12:55:31.000000 cbmos-0.3.0/cbmos.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-13 12:55:20.000000 cbmos-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-04-13 12:55:20.000000 cbmos-0.3.0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-13 12:55:31.300734 cbmos-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 12:55:20.000000 cbmos-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:55:31.300734 cbmos-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17836 2023-04-13 12:55:20.000000 cbmos-0.3.0/tests/test_cbmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-13 12:55:20.000000 cbmos-0.3.0/tests/test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-13 12:55:20.000000 cbmos-0.3.0/tests/test_euler_backward.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-04-13 12:55:20.000000 cbmos-0.3.0/tests/test_euler_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-13 12:55:20.000000 cbmos-0.3.0/tests/test_eventqueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-13 12:55:20.000000 cbmos-0.3.0/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-13 12:55:20.000000 cbmos-0.3.0/tests/test_force_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-13 12:55:20.000000 cbmos-0.3.0/tests/test_geshgorin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-13 12:55:20.000000 cbmos-0.3.0/tests/test_utils.py
```

### Comparing `cbmos-0.2.0/LICENSE.txt` & `cbmos-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cbmos-0.2.0/PKG-INFO` & `cbmos-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: cbmos
-Version: 0.2.0
+Version: 0.3.0
 Summary: A framework for numerical analysis of center-based cell models
 Home-page: https://github.com/somathias/cbmos
 Author: Sonja Mathias et al.
 Author-email: sonja.mathias@it.uu.se
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/somathias/cbmos/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: gpu
 License-File: LICENSE.txt
 
@@ -111,9 +109,10 @@
 [somathias.github.io/cbmos/](https://somathias.github.io/cbmos/)
 
 ## Publications
 
 - Mathias, S., Coulier, A., Bouchnita, A. et al. Impact of Force Function
   Formulations on the Numerical Simulation of Centre-Based Models. Bull Math
   Biol 82, 132 (2020). [DOI](https://doi.org/10.1007/s11538-020-00810-2) (tag `exp-Mathias2020`)
-
-
+- Mathias, S., Coulier, A. & Hellander, A. CBMOS: a GPU-enabled Python
+  framework for the numerical study of center-based models. BMC Bioinformatics
+  23, 55 (2022). [DOI](https://doi.org/10.1186/s12859-022-04575-4) (tag `exp-Mathias2022`)
```

### Comparing `cbmos-0.2.0/cbmos/cbmodel/__init__.py` & `cbmos-0.3.0/cbmos/cbmodel/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,14 +49,16 @@
             force_args,
             solver_args,
             seed=None,
             raw_t=True,
             max_execution_time=None,
             min_event_resolution=0.,
             event_list=[],
+            n_target_cells=[],
+            throw_away_history=False
             ):
         """
         Run the simulation with the given arguments and return the position
         of the cells at each time steps in `t_data`
 
         Parameters
         ----------
@@ -125,25 +127,40 @@
         self._save_data()
 
         self._queue = EventQueue(
                 [_copy.copy(event) for event in event_list],
                 min_resolution=min_event_resolution,
                 )
 
+        if n_target_cells:
+            self.target_cell_count_checkpoints = []
+            n_target_cells_index = 0
+
         while t < t_end:
 
             # check if max_execution_time has elapsed
             exec_time = time.time() - exec_time_start
             if (
                     max_execution_time is not None
                     and exec_time >= max_execution_time
                     ):
                 self.last_exec_time = exec_time
                 return (self.t_data, self.history)
 
+            # check if max_n_cells is reached
+            if n_target_cells:
+                if len(self.history[-1]) >= n_target_cells[-1]:
+                    # target number of cells has been reached
+                    self.target_cell_count_checkpoints.append((t, len(self.history[-1]), exec_time))
+                    self.last_exec_time = exec_time
+                    return (self.t_data, self.history)
+                elif len(self.history[-1]) >= n_target_cells[n_target_cells_index]:
+                    self.target_cell_count_checkpoints.append((t, len(self.history[-1]), exec_time))
+                    n_target_cells_index += 1
+
             # generate next event(s)
             # NB: if events are aggregated,
             #     multiple events can happen at time `tau`
             try:
                 tau, events = self._queue.pop()
             except IndexError:
                 tau, events = _np.inf, None
@@ -225,14 +242,17 @@
             if tau <= t_end:
                 for event in events:
                     event.apply(self)
 
             # update current time t to min(tau, t_end)
             t = min(tau, t_end)
 
+            if throw_away_history:
+                self.history = [self.history[-1]]
+
         exec_time = time.time() - exec_time_start
         self.last_exec_time = exec_time
         return (self.t_data, self.history)
 
     def _save_data(self, positions=None):
         """
         Save the current positions of the cells to `self.history`. If
```

### Comparing `cbmos-0.2.0/cbmos/cbmodel/_eventqueue.py` & `cbmos-0.3.0/cbmos/cbmodel/_eventqueue.py`

 * *Files identical despite different names*

### Comparing `cbmos-0.2.0/cbmos/cell.py` & `cbmos-0.3.0/cbmos/cell.py`

 * *Files identical despite different names*

### Comparing `cbmos-0.2.0/cbmos/events.py` & `cbmos-0.3.0/cbmos/events.py`

 * *Files 26% similar despite different names*

```diff
@@ -96,7 +96,56 @@
             random_zenith_angle = _np.arccos(2 * v - 1)
             division_direction = _np.array([
                 _np.cos(random_azimuth_angle) * _np.sin(random_zenith_angle),
                 _np.sin(random_azimuth_angle) * _np.sin(random_zenith_angle),
                 _np.cos(random_zenith_angle)])
 
         return division_direction
+
+class PickRandomCellToDivideEvent(Event):
+    """
+    Pick a random cell from the current population and let it divide
+    """
+    def __init__(self, time):
+        self.tau = time
+
+    def apply(self, cbmodel):
+        target_cell_index = _npr.choice(_np.array([cell.ID for cell in cbmodel.cell_list]))
+        target_cell = cbmodel.cell_list[target_cell_index]
+
+        division_direction = self._get_division_direction(cbmodel)
+        updated_position_parent = target_cell.position \
+            - 0.5 * cbmodel.separation * division_direction
+        position_daughter = target_cell.position \
+            + 0.5 * cbmodel.separation * division_direction
+
+        daughter_cell = _cl.Cell(
+                cbmodel.next_cell_index, position_daughter)
+        cbmodel.next_cell_index += 1
+        cbmodel.cell_list.append(daughter_cell)
+
+        target_cell.position = updated_position_parent
+
+        _logging.debug("Division event: t={}, direction={}".format(
+            self.tau, division_direction))
+
+    def _get_division_direction(self, cbmodel):
+        if cbmodel.dim == 1:
+            division_direction = _np.array([-1.0 + 2.0 * _npr.randint(2)])
+
+        elif cbmodel.dim == 2:
+            random_angle = 2.0 * _np.pi * _npr.rand()
+            division_direction = _np.array([
+                _np.cos(random_angle),
+                _np.sin(random_angle)])
+
+        elif cbmodel.dim == 3:
+            u = _npr.rand()
+            v = _npr.rand()
+            random_azimuth_angle = 2 * _np.pi * u
+            random_zenith_angle = _np.arccos(2 * v - 1)
+            division_direction = _np.array([
+                _np.cos(random_azimuth_angle) * _np.sin(random_zenith_angle),
+                _np.sin(random_azimuth_angle) * _np.sin(random_zenith_angle),
+                _np.cos(random_zenith_angle)])
+
+        return division_direction
```

### Comparing `cbmos-0.2.0/cbmos/solvers/adams_bashforth.py` & `cbmos-0.3.0/cbmos/solvers/adams_bashforth.py`

 * *Files identical despite different names*

### Comparing `cbmos-0.2.0/cbmos/solvers/heun.py` & `cbmos-0.3.0/cbmos/solvers/heun.py`

 * *Files identical despite different names*

### Comparing `cbmos-0.2.0/cbmos/solvers/midpoint.py` & `cbmos-0.3.0/cbmos/solvers/midpoint.py`

 * *Files identical despite different names*

### Comparing `cbmos-0.2.0/cbmos.egg-info/PKG-INFO` & `cbmos-0.3.0/cbmos.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: cbmos
-Version: 0.2.0
+Version: 0.3.0
 Summary: A framework for numerical analysis of center-based cell models
 Home-page: https://github.com/somathias/cbmos
 Author: Sonja Mathias et al.
 Author-email: sonja.mathias@it.uu.se
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/somathias/cbmos/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: gpu
 License-File: LICENSE.txt
 
@@ -111,9 +109,10 @@
 [somathias.github.io/cbmos/](https://somathias.github.io/cbmos/)
 
 ## Publications
 
 - Mathias, S., Coulier, A., Bouchnita, A. et al. Impact of Force Function
   Formulations on the Numerical Simulation of Centre-Based Models. Bull Math
   Biol 82, 132 (2020). [DOI](https://doi.org/10.1007/s11538-020-00810-2) (tag `exp-Mathias2020`)
-
-
+- Mathias, S., Coulier, A. & Hellander, A. CBMOS: a GPU-enabled Python
+  framework for the numerical study of center-based models. BMC Bioinformatics
+  23, 55 (2022). [DOI](https://doi.org/10.1186/s12859-022-04575-4) (tag `exp-Mathias2022`)
```

### Comparing `cbmos-0.2.0/setup.cfg` & `cbmos-0.3.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cbmos
-version = 0.2.0
+version = 0.3.0
 author = Sonja Mathias et al.
 author_email = sonja.mathias@it.uu.se
 description = A framework for numerical analysis of center-based cell models
 long_description = file: readme.md
 long_description_content_type = text/markdown
 url = https://github.com/somathias/cbmos
 project_urls =
```

