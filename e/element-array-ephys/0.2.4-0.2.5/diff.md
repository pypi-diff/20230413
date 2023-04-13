# Comparing `tmp/element-array-ephys-0.2.4.tar.gz` & `tmp/element-array-ephys-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "element-array-ephys-0.2.4.tar", last modified: Fri Mar 10 19:27:00 2023, max compression
+gzip compressed data, was "element-array-ephys-0.2.5.tar", last modified: Thu Apr 13 19:28:54 2023, max compression
```

## Comparing `element-array-ephys-0.2.4.tar` & `element-array-ephys-0.2.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:00.019565 element-array-ephys-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-10 19:26:53.000000 element-array-ephys-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-10 19:27:00.019565 element-array-ephys-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-03-10 19:26:53.000000 element-array-ephys-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:00.019565 element-array-ephys-0.2.4/element_array_ephys/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-03-10 19:26:53.000000 element-array-ephys-0.2.4/element_array_ephys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63666 2023-03-10 19:26:53.000000 element-array-ephys-0.2.4/element_array_ephys/ephys_acute.py
--rw-r--r--   0 runner    (1001) docker     (123)    60785 2023-03-10 19:26:53.000000 element-array-ephys-0.2.4/element_array_ephys/ephys_chronic.py
--rw-r--r--   0 runner    (1001) docker     (123)    61304 2023-03-10 19:26:53.000000 element-array-ephys-0.2.4/element_array_ephys/ephys_no_curation.py
--rw-r--r--   0 runner    (1001) docker     (123)    56785 2023-03-10 19:26:53.000000 element-array-ephys-0.2.4/element_array_ephys/ephys_precluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-03-10 19:26:53.000000 element-array-ephys-0.2.4/element_array_ephys/ephys_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:00.019565 element-array-ephys-0.2.4/element_array_ephys/export/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 19:26:53.000000 element-array-ephys-0.2.4/element_array_ephys/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:00.019565 element-array-ephys-0.2.4/element_array_ephys/export/nwb/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-10 19:26:53.000000 element-array-ephys-0.2.4/element_array_ephys/export/nwb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24154 2023-03-10 19:26:53.000000 element-array-ephys-0.2.4/element_array_ephys/export/nwb/nwb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:00.019565 element-array-ephys-0.2.4/element_array_ephys/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 19:26:53.000000 element-array-ephys-0.2.4/element_array_ephys/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-03-10 19:26:53.000000 element-array-ephys-0.2.4/element_array_ephys/plotting/corr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-03-10 19:26:53.000000 element-array-ephys-0.2.4/element_array_ephys/plotting/probe_level.py
--rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-03-10 19:26:53.000000 element-array-ephys-0.2.4/element_array_ephys/plotting/qc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-03-10 19:26:53.000000 element-array-ephys-0.2.4/element_array_ephys/plotting/unit_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-03-10 19:26:53.000000 element-array-ephys-0.2.4/element_array_ephys/plotting/widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-03-10 19:26:53.000000 element-array-ephys-0.2.4/element_array_ephys/probe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:00.019565 element-array-ephys-0.2.4/element_array_ephys/readers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 19:26:53.000000 element-array-ephys-0.2.4/element_array_ephys/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-03-10 19:26:53.000000 element-array-ephys-0.2.4/element_array_ephys/readers/kilosort.py
--rw-r--r--   0 runner    (1001) docker     (123)    30278 2023-03-10 19:26:53.000000 element-array-ephys-0.2.4/element_array_ephys/readers/kilosort_triggering.py
--rw-r--r--   0 runner    (1001) docker     (123)    19037 2023-03-10 19:26:53.000000 element-array-ephys-0.2.4/element_array_ephys/readers/openephys.py
--rw-r--r--   0 runner    (1001) docker     (123)    16561 2023-03-10 19:26:53.000000 element-array-ephys-0.2.4/element_array_ephys/readers/spikeglx.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-10 19:26:53.000000 element-array-ephys-0.2.4/element_array_ephys/readers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-10 19:26:53.000000 element-array-ephys-0.2.4/element_array_ephys/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:00.019565 element-array-ephys-0.2.4/element_array_ephys.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-10 19:26:59.000000 element-array-ephys-0.2.4/element_array_ephys.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-03-10 19:26:59.000000 element-array-ephys-0.2.4/element_array_ephys.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 19:26:59.000000 element-array-ephys-0.2.4/element_array_ephys.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-03-10 19:26:59.000000 element-array-ephys-0.2.4/element_array_ephys.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-10 19:26:59.000000 element-array-ephys-0.2.4/element_array_ephys.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 19:27:00.019565 element-array-ephys-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-03-10 19:26:53.000000 element-array-ephys-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:28:54.691341 element-array-ephys-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-13 19:28:52.000000 element-array-ephys-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-13 19:28:54.691341 element-array-ephys-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-13 19:28:52.000000 element-array-ephys-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:28:54.687341 element-array-ephys-0.2.5/element_array_ephys/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-13 19:28:52.000000 element-array-ephys-0.2.5/element_array_ephys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63666 2023-04-13 19:28:52.000000 element-array-ephys-0.2.5/element_array_ephys/ephys_acute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60785 2023-04-13 19:28:52.000000 element-array-ephys-0.2.5/element_array_ephys/ephys_chronic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61305 2023-04-13 19:28:52.000000 element-array-ephys-0.2.5/element_array_ephys/ephys_no_curation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56785 2023-04-13 19:28:52.000000 element-array-ephys-0.2.5/element_array_ephys/ephys_precluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-04-13 19:28:52.000000 element-array-ephys-0.2.5/element_array_ephys/ephys_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:28:54.687341 element-array-ephys-0.2.5/element_array_ephys/export/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:28:52.000000 element-array-ephys-0.2.5/element_array_ephys/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:28:54.687341 element-array-ephys-0.2.5/element_array_ephys/export/nwb/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-13 19:28:52.000000 element-array-ephys-0.2.5/element_array_ephys/export/nwb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24154 2023-04-13 19:28:52.000000 element-array-ephys-0.2.5/element_array_ephys/export/nwb/nwb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:28:54.691341 element-array-ephys-0.2.5/element_array_ephys/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:28:52.000000 element-array-ephys-0.2.5/element_array_ephys/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-04-13 19:28:52.000000 element-array-ephys-0.2.5/element_array_ephys/plotting/corr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-13 19:28:52.000000 element-array-ephys-0.2.5/element_array_ephys/plotting/probe_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15284 2023-04-13 19:28:52.000000 element-array-ephys-0.2.5/element_array_ephys/plotting/qc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-04-13 19:28:52.000000 element-array-ephys-0.2.5/element_array_ephys/plotting/unit_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-04-13 19:28:52.000000 element-array-ephys-0.2.5/element_array_ephys/plotting/widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-04-13 19:28:52.000000 element-array-ephys-0.2.5/element_array_ephys/probe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:28:54.691341 element-array-ephys-0.2.5/element_array_ephys/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:28:52.000000 element-array-ephys-0.2.5/element_array_ephys/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-04-13 19:28:52.000000 element-array-ephys-0.2.5/element_array_ephys/readers/kilosort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30278 2023-04-13 19:28:52.000000 element-array-ephys-0.2.5/element_array_ephys/readers/kilosort_triggering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19037 2023-04-13 19:28:52.000000 element-array-ephys-0.2.5/element_array_ephys/readers/openephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16561 2023-04-13 19:28:52.000000 element-array-ephys-0.2.5/element_array_ephys/readers/spikeglx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-13 19:28:52.000000 element-array-ephys-0.2.5/element_array_ephys/readers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-13 19:28:52.000000 element-array-ephys-0.2.5/element_array_ephys/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:28:54.687341 element-array-ephys-0.2.5/element_array_ephys.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-13 19:28:54.000000 element-array-ephys-0.2.5/element_array_ephys.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-13 19:28:54.000000 element-array-ephys-0.2.5/element_array_ephys.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 19:28:54.000000 element-array-ephys-0.2.5/element_array_ephys.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-13 19:28:54.000000 element-array-ephys-0.2.5/element_array_ephys.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-13 19:28:54.000000 element-array-ephys-0.2.5/element_array_ephys.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 19:28:54.691341 element-array-ephys-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-13 19:28:52.000000 element-array-ephys-0.2.5/setup.py
```

### Comparing `element-array-ephys-0.2.4/LICENSE` & `element-array-ephys-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.4/PKG-INFO` & `element-array-ephys-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: element-array-ephys
-Version: 0.2.4
+Version: 0.2.5
 Summary: DataJoint Element for Extracellular Array Electrophysiology
 Home-page: https://github.com/datajoint/element-array-ephys
 Author: DataJoint
 Author-email: info@datajoint.com
 License: MIT
 Keywords: neuroscience electrophysiology science datajoint
 Platform: UNKNOWN
```

### Comparing `element-array-ephys-0.2.4/README.md` & `element-array-ephys-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.4/element_array_ephys/ephys_acute.py` & `element-array-ephys-0.2.5/element_array_ephys/ephys_acute.py`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.4/element_array_ephys/ephys_chronic.py` & `element-array-ephys-0.2.5/element_array_ephys/ephys_chronic.py`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.4/element_array_ephys/ephys_no_curation.py` & `element-array-ephys-0.2.5/element_array_ephys/ephys_no_curation.py`

 * *Files 1% similar despite different names*

```diff
@@ -933,17 +933,17 @@
     """
 
     class Unit(dj.Part):
         """Single unit properties after clustering and curation.
 
         Attributes:
             CuratedClustering (foreign key): CuratedClustering primary key.
-            unit (foreign key, int): Unique integer identifying a single unit.
-            probe.ElectrodeConfig.Electrode (dict): probe.ElectrodeConfig.Electrode primary key.
-            ClusteringQualityLabel (dict): CLusteringQualityLabel primary key.
+            unit (int): Unique integer identifying a single unit.
+            probe.ElectrodeConfig.Electrode (foreign key): probe.ElectrodeConfig.Electrode primary key.
+            ClusteringQualityLabel (foreign key): CLusteringQualityLabel primary key.
             spike_count (int): Number of spikes in this recording for this unit.
             spike_times (longblob): Spike times of this unit, relative to start time of EphysRecording.
             spike_sites (longblob): Array of electrode associated with each spike.
             spike_depths (longblob): Array of depths associated with each spike, relative to each spike.
         """
 
         definition = """
```

### Comparing `element-array-ephys-0.2.4/element_array_ephys/ephys_precluster.py` & `element-array-ephys-0.2.5/element_array_ephys/ephys_precluster.py`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.4/element_array_ephys/ephys_report.py` & `element-array-ephys-0.2.5/element_array_ephys/ephys_report.py`

 * *Files 6% similar despite different names*

```diff
@@ -155,14 +155,24 @@
                 "depth_waveform_plotly": depth_waveform_fig.to_plotly_json(),
             }
         )
 
 
 @schema
 class QualityMetricCutoffs(dj.Lookup):
+    """Cut-off values for unit quality metrics.
+
+    Attributes:
+        cutoffs_id (smallint): Unique ID for the cut-off values.
+        amplitude_cutoff_maximum (float): Optional. Amplitude cut-off.
+        presence_ratio_minimum (float): Optional. Presence ratio cut-off.
+        isi_violations_maximum (float): Optional. ISI violation ratio cut-off.
+        cutoffs_hash (uuid): uuid for the cut-off values.
+    """
+    
     definition = """
     cutoffs_id                    : smallint
     ---
     amplitude_cutoff_maximum=null : float # Defaults to null, no cutoff applied
     presence_ratio_minimum=null   : float # Defaults to null, no cutoff applied
     isi_violations_maximum=null   : float # Defaults to null, no cutoff applied
     cutoffs_hash: uuid
@@ -214,22 +224,36 @@
             cls.insert1(
                 {"cutoffs_id": cutoffs_id, **param_dict, "cutoffs_hash": param_hash}
             )
 
 
 @schema
 class QualityMetricSet(dj.Manual):
+    """Set of quality metric values for clusters and its cut-offs.
+
+    Attributes:
+        ephys.QualityMetrics (foreign key): ephys.QualityMetrics primary key.
+        QualityMetricCutoffs (foreign key): QualityMetricCutoffs primary key.
+    """
+    
     definition = """
     -> ephys.QualityMetrics
     -> QualityMetricCutoffs
     """
 
 
 @schema
 class QualityMetricReport(dj.Computed):
+    """Table for storing quality metric figures.
+
+    Attributes:
+        QualityMetricSet (foreign key): QualityMetricSet primary key.
+        plot_grid (longblob): Plotly figure object.
+    """
+    
     definition = """
     -> QualityMetricSet
     ---
     plot_grid : longblob
     """
 
     def make(self, key):
```

### Comparing `element-array-ephys-0.2.4/element_array_ephys/export/nwb/nwb.py` & `element-array-ephys-0.2.5/element_array_ephys/export/nwb/nwb.py`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.4/element_array_ephys/plotting/corr.py` & `element-array-ephys-0.2.5/element_array_ephys/plotting/corr.py`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.4/element_array_ephys/plotting/probe_level.py` & `element-array-ephys-0.2.5/element_array_ephys/plotting/probe_level.py`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.4/element_array_ephys/plotting/qc.py` & `element-array-ephys-0.2.5/element_array_ephys/plotting/qc.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,22 +24,18 @@
         """Initialize QC metric class
 
         Args:
             ephys (module): datajoint module with a QualityMetric table
             key (dict, optional): key from ephys.QualityMetric table. Defaults to None.
             scale (float, optional): Scale at which to render figure. Defaults to 1.4.
             fig_width (int, optional): Figure width in pixels. Defaults to 800.
-            amplitude_cutoff_maximum (float, optional): Cutoff for unit amplitude in
-                visualizations. Defaults to None.
-            presence_ratio_minimum (float, optional): Cutoff for presence ratio in
-                visualizations. Defaults to None.
-            isi_violations_maximum (float, optional): Cutoff for isi violations in
-                visualizations. Defaults to None.
-            dark_mode (bool, optional): Set background to black, foreground white.
-                Default False, black on white.
+            amplitude_cutoff_maximum (float, optional): Cutoff for unit amplitude in visualizations. Defaults to None.
+            presence_ratio_minimum (float, optional): Cutoff for presence ratio in visualizations. Defaults to None.
+            isi_violations_maximum (float, optional): Cutoff for isi violations in visualizations. Defaults to None.
+            dark_mode (bool, optional): Set background to black, foreground white. Default False, black on white.
         """
         self._ephys = ephys
         self._key = key
         self._scale = scale
         self._plots = {}  # Empty default to defer set to dict property below
         self._fig_width = fig_width
         self._amplitude_cutoff_max = amplitude_cutoff_maximum
@@ -130,15 +126,15 @@
         """Return formatted figure or apply formatting to existing figure
 
         Args:
             fig (go.Figure, optional): Apply formatting to this plotly graph object
                 Figure to apply formatting. Defaults to empty.
             scale (float, optional): Scale to render figure. Defaults to scale from
                 class init, 1.
-            ratio (float, optional): Figure aspect ratio width/height . Defaults to 1.
+            ratio (float, optional): Figure aspect ratio width/height. Defaults to 1.
 
         Returns:
             go.Figure: Formatted figure
         """
         if not fig:
             fig = go.Figure()
         if not scale:
@@ -198,29 +194,28 @@
         else:
             # To quiet divide by zero error when no data
             histogram, histogram_bins = np.ndarray(0), np.ndarray(0)
 
         return fig.add_trace(
             go.Scatter(
                 x=histogram_bins[:-1],
-                y=gaussian_filter1d(histogram, 1),  # TODO: remove smoothing
+                y=gaussian_filter1d(histogram, 1),  
                 mode="lines",
                 line=dict(color="rgb(0, 160, 223)", width=2 * scale),  # DataJoint Blue
                 hovertemplate="%{x:.2f}<br>%{y:.2f}<extra></extra>",
             ),
             **trace_kwargs,
         )
 
     def get_single_fig(self, fig_name: str, scale: float = None) -> go.Figure:
         """Return a single figure of the plots listed in the plot_list property
 
         Args:
             fig_name (str): Name of figure to be rendered
-            scale (float, optional): Scale to render fig. Defaults to scale at class
-                init, 1.
+            scale (float, optional): Scale to render fig. Defaults to scale at class init, 1.
 
         Returns:
             go.Figure: Histogram plot
         """
         if not self._key:
             return self._empty_fig()
         if not scale:
@@ -249,16 +244,15 @@
         return fig
 
     def get_grid(self, n_columns: int = 4, scale: float = 1.0) -> go.Figure:
         """Plot grid of histograms as subplots in go.Figure using n_columns
 
         Args:
             n_columns (int, optional): Number of column in grid. Defaults to 4.
-            scale (float, optional): Scale to render fig. Defaults to scale at class
-                init, 1.
+            scale (float, optional): Scale to render fig. Defaults to scale at class init, 1.
 
         Returns:
             go.Figure: grid of available plots
         """
         from plotly.subplots import make_subplots
 
         if not self._key:
```

### Comparing `element-array-ephys-0.2.4/element_array_ephys/plotting/unit_level.py` & `element-array-ephys-0.2.5/element_array_ephys/plotting/unit_level.py`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.4/element_array_ephys/plotting/widget.py` & `element-array-ephys-0.2.5/element_array_ephys/plotting/widget.py`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.4/element_array_ephys/probe.py` & `element-array-ephys-0.2.5/element_array_ephys/probe.py`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.4/element_array_ephys/readers/kilosort.py` & `element-array-ephys-0.2.5/element_array_ephys/readers/kilosort.py`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.4/element_array_ephys/readers/kilosort_triggering.py` & `element-array-ephys-0.2.5/element_array_ephys/readers/kilosort_triggering.py`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.4/element_array_ephys/readers/openephys.py` & `element-array-ephys-0.2.5/element_array_ephys/readers/openephys.py`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.4/element_array_ephys/readers/spikeglx.py` & `element-array-ephys-0.2.5/element_array_ephys/readers/spikeglx.py`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.4/element_array_ephys.egg-info/PKG-INFO` & `element-array-ephys-0.2.5/element_array_ephys.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: element-array-ephys
-Version: 0.2.4
+Version: 0.2.5
 Summary: DataJoint Element for Extracellular Array Electrophysiology
 Home-page: https://github.com/datajoint/element-array-ephys
 Author: DataJoint
 Author-email: info@datajoint.com
 License: MIT
 Keywords: neuroscience electrophysiology science datajoint
 Platform: UNKNOWN
```

### Comparing `element-array-ephys-0.2.4/element_array_ephys.egg-info/SOURCES.txt` & `element-array-ephys-0.2.5/element_array_ephys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `element-array-ephys-0.2.4/setup.py` & `element-array-ephys-0.2.5/setup.py`

 * *Files identical despite different names*

