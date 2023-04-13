# Comparing `tmp/bluepyefe-2.2.45.tar.gz` & `tmp/bluepyefe-2.2.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluepyefe-2.2.45.tar", last modified: Fri Mar 31 07:43:24 2023, max compression
+gzip compressed data, was "bluepyefe-2.2.46.tar", last modified: Thu Apr 13 07:17:23 2023, max compression
```

## Comparing `bluepyefe-2.2.45.tar` & `bluepyefe-2.2.46.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 07:43:24.205685 bluepyefe-2.2.45/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-31 07:43:19.000000 bluepyefe-2.2.45/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-03-31 07:43:19.000000 bluepyefe-2.2.45/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-31 07:43:19.000000 bluepyefe-2.2.45/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-03-31 07:43:24.205685 bluepyefe-2.2.45/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-03-31 07:43:19.000000 bluepyefe-2.2.45/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 07:43:24.205685 bluepyefe-2.2.45/bluepyefe/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-31 07:43:19.000000 bluepyefe-2.2.45/bluepyefe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-03-31 07:43:24.205685 bluepyefe-2.2.45/bluepyefe/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-03-31 07:43:19.000000 bluepyefe-2.2.45/bluepyefe/auto_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-03-31 07:43:19.000000 bluepyefe-2.2.45/bluepyefe/cell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 07:43:24.205685 bluepyefe-2.2.45/bluepyefe/ecode/
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-03-31 07:43:19.000000 bluepyefe-2.2.45/bluepyefe/ecode/DeHyperPol.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-03-31 07:43:19.000000 bluepyefe-2.2.45/bluepyefe/ecode/HyperDePol.py
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-03-31 07:43:19.000000 bluepyefe-2.2.45/bluepyefe/ecode/SpikeRec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-03-31 07:43:19.000000 bluepyefe-2.2.45/bluepyefe/ecode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-03-31 07:43:19.000000 bluepyefe-2.2.45/bluepyefe/ecode/negCheops.py
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-03-31 07:43:19.000000 bluepyefe-2.2.45/bluepyefe/ecode/posCheops.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-03-31 07:43:19.000000 bluepyefe-2.2.45/bluepyefe/ecode/ramp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-03-31 07:43:19.000000 bluepyefe-2.2.45/bluepyefe/ecode/sAHP.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-03-31 07:43:19.000000 bluepyefe-2.2.45/bluepyefe/ecode/sineSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-03-31 07:43:19.000000 bluepyefe-2.2.45/bluepyefe/ecode/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-03-31 07:43:19.000000 bluepyefe-2.2.45/bluepyefe/ecode/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    34969 2023-03-31 07:43:19.000000 bluepyefe-2.2.45/bluepyefe/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 07:43:24.205685 bluepyefe-2.2.45/bluepyefe/igorpy/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3976 2023-03-31 07:43:19.000000 bluepyefe-2.2.45/bluepyefe/igorpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9498 2023-03-31 07:43:19.000000 bluepyefe-2.2.45/bluepyefe/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-03-31 07:43:19.000000 bluepyefe-2.2.45/bluepyefe/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-03-31 07:43:19.000000 bluepyefe-2.2.45/bluepyefe/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    14980 2023-03-31 07:43:19.000000 bluepyefe-2.2.45/bluepyefe/recording.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-03-31 07:43:19.000000 bluepyefe-2.2.45/bluepyefe/rheobase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-03-31 07:43:19.000000 bluepyefe-2.2.45/bluepyefe/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-03-31 07:43:19.000000 bluepyefe-2.2.45/bluepyefe/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-03-31 07:43:19.000000 bluepyefe-2.2.45/bluepyefe/translate_legacy_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 07:43:24.205685 bluepyefe-2.2.45/bluepyefe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-03-31 07:43:24.000000 bluepyefe-2.2.45/bluepyefe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-03-31 07:43:24.000000 bluepyefe-2.2.45/bluepyefe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 07:43:24.000000 bluepyefe-2.2.45/bluepyefe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-31 07:43:24.000000 bluepyefe-2.2.45/bluepyefe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-31 07:43:24.000000 bluepyefe-2.2.45/bluepyefe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 07:43:24.205685 bluepyefe-2.2.45/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-03-31 07:43:19.000000 bluepyefe-2.2.45/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-31 07:43:24.205685 bluepyefe-2.2.45/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-03-31 07:43:19.000000 bluepyefe-2.2.45/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    69513 2023-03-31 07:43:19.000000 bluepyefe-2.2.45/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:17:23.925902 bluepyefe-2.2.46/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-13 07:17:17.000000 bluepyefe-2.2.46/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-13 07:17:17.000000 bluepyefe-2.2.46/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-13 07:17:17.000000 bluepyefe-2.2.46/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-13 07:17:23.925902 bluepyefe-2.2.46/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-04-13 07:17:17.000000 bluepyefe-2.2.46/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:17:23.925902 bluepyefe-2.2.46/bluepyefe/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-13 07:17:17.000000 bluepyefe-2.2.46/bluepyefe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-13 07:17:23.925902 bluepyefe-2.2.46/bluepyefe/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-04-13 07:17:17.000000 bluepyefe-2.2.46/bluepyefe/auto_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-04-13 07:17:17.000000 bluepyefe-2.2.46/bluepyefe/cell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:17:23.921902 bluepyefe-2.2.46/bluepyefe/ecode/
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-04-13 07:17:17.000000 bluepyefe-2.2.46/bluepyefe/ecode/DeHyperPol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-04-13 07:17:17.000000 bluepyefe-2.2.46/bluepyefe/ecode/HyperDePol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-04-13 07:17:17.000000 bluepyefe-2.2.46/bluepyefe/ecode/SpikeRec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-13 07:17:17.000000 bluepyefe-2.2.46/bluepyefe/ecode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-04-13 07:17:17.000000 bluepyefe-2.2.46/bluepyefe/ecode/negCheops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-04-13 07:17:17.000000 bluepyefe-2.2.46/bluepyefe/ecode/posCheops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-04-13 07:17:17.000000 bluepyefe-2.2.46/bluepyefe/ecode/ramp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-04-13 07:17:17.000000 bluepyefe-2.2.46/bluepyefe/ecode/sAHP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-04-13 07:17:17.000000 bluepyefe-2.2.46/bluepyefe/ecode/sineSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-04-13 07:17:17.000000 bluepyefe-2.2.46/bluepyefe/ecode/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-13 07:17:17.000000 bluepyefe-2.2.46/bluepyefe/ecode/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34969 2023-04-13 07:17:17.000000 bluepyefe-2.2.46/bluepyefe/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:17:23.921902 bluepyefe-2.2.46/bluepyefe/igorpy/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3976 2023-04-13 07:17:17.000000 bluepyefe-2.2.46/bluepyefe/igorpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9498 2023-04-13 07:17:17.000000 bluepyefe-2.2.46/bluepyefe/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-04-13 07:17:17.000000 bluepyefe-2.2.46/bluepyefe/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-04-13 07:17:17.000000 bluepyefe-2.2.46/bluepyefe/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15562 2023-04-13 07:17:17.000000 bluepyefe-2.2.46/bluepyefe/recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-04-13 07:17:17.000000 bluepyefe-2.2.46/bluepyefe/rheobase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-04-13 07:17:17.000000 bluepyefe-2.2.46/bluepyefe/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-04-13 07:17:17.000000 bluepyefe-2.2.46/bluepyefe/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-04-13 07:17:17.000000 bluepyefe-2.2.46/bluepyefe/translate_legacy_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:17:23.921902 bluepyefe-2.2.46/bluepyefe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-13 07:17:23.000000 bluepyefe-2.2.46/bluepyefe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-13 07:17:23.000000 bluepyefe-2.2.46/bluepyefe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 07:17:23.000000 bluepyefe-2.2.46/bluepyefe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-13 07:17:23.000000 bluepyefe-2.2.46/bluepyefe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-13 07:17:23.000000 bluepyefe-2.2.46/bluepyefe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:17:23.925902 bluepyefe-2.2.46/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-13 07:17:17.000000 bluepyefe-2.2.46/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-13 07:17:23.925902 bluepyefe-2.2.46/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-13 07:17:17.000000 bluepyefe-2.2.46/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69513 2023-04-13 07:17:17.000000 bluepyefe-2.2.46/versioneer.py
```

### Comparing `bluepyefe-2.2.45/LICENSE.txt` & `bluepyefe-2.2.46/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.45/PKG-INFO` & `bluepyefe-2.2.46/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: bluepyefe
-Version: 2.2.45
+Version: 2.2.46
 Summary: Blue Brain Python E-feature extraction
 Home-page: https://github.com/BlueBrain/BluePyEfe
 Author: BlueBrain Project, EPFL
 License: LGPLv3
 Description: The Blue Brain Python E-feature extraction Library (BluePyEfe) aims at easing the process of reading experimental recordings and extracting batches of electrical features from them. To do so, it combines trace reading functions and features extraction functions from the eFel library. BluePyEfe outputs protocols and features files in a format that can then be used by BluePyOpt for electrical model building purposes.
 Keywords: neuroscience,BlueBrainProject
 Platform: UNKNOWN
```

### Comparing `bluepyefe-2.2.45/README.md` & `bluepyefe-2.2.46/README.md`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.45/bluepyefe/__init__.py` & `bluepyefe-2.2.46/bluepyefe/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.45/bluepyefe/auto_targets.py` & `bluepyefe-2.2.46/bluepyefe/auto_targets.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.45/bluepyefe/cell.py` & `bluepyefe-2.2.46/bluepyefe/cell.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.45/bluepyefe/ecode/DeHyperPol.py` & `bluepyefe-2.2.46/bluepyefe/ecode/DeHyperPol.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.45/bluepyefe/ecode/HyperDePol.py` & `bluepyefe-2.2.46/bluepyefe/ecode/HyperDePol.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.45/bluepyefe/ecode/SpikeRec.py` & `bluepyefe-2.2.46/bluepyefe/ecode/SpikeRec.py`

 * *Files 8% similar despite different names*

```diff
@@ -128,14 +128,22 @@
     def ton(self):
         return 0.0
 
     @property
     def toff(self):
         return self.tend
 
+    @property
+    def multi_stim_start(self):
+        return list(self.tspike)
+
+    @property
+    def multi_stim_end(self):
+        return [t + self.spike_duration for t in self.tspike]
+
     def get_stimulus_parameters(self):
         """Returns the eCode parameters"""
 
         ecode_params = {
             "delay": self.tspike[0],
             "n_spikes": len(self.tspike),
             "delta": self.delta,
```

### Comparing `bluepyefe-2.2.45/bluepyefe/ecode/__init__.py` & `bluepyefe-2.2.46/bluepyefe/ecode/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.45/bluepyefe/ecode/negCheops.py` & `bluepyefe-2.2.46/bluepyefe/ecode/negCheops.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.45/bluepyefe/ecode/posCheops.py` & `bluepyefe-2.2.46/bluepyefe/ecode/posCheops.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.45/bluepyefe/ecode/ramp.py` & `bluepyefe-2.2.46/bluepyefe/ecode/ramp.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.45/bluepyefe/ecode/sAHP.py` & `bluepyefe-2.2.46/bluepyefe/ecode/sAHP.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.45/bluepyefe/ecode/sineSpec.py` & `bluepyefe-2.2.46/bluepyefe/ecode/sineSpec.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.45/bluepyefe/ecode/step.py` & `bluepyefe-2.2.46/bluepyefe/ecode/step.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.45/bluepyefe/ecode/tools.py` & `bluepyefe-2.2.46/bluepyefe/ecode/tools.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.45/bluepyefe/extract.py` & `bluepyefe-2.2.46/bluepyefe/extract.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.45/bluepyefe/igorpy/__init__.py` & `bluepyefe-2.2.46/bluepyefe/igorpy/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.45/bluepyefe/plotting.py` & `bluepyefe-2.2.46/bluepyefe/plotting.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.45/bluepyefe/protocol.py` & `bluepyefe-2.2.46/bluepyefe/protocol.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.45/bluepyefe/reader.py` & `bluepyefe-2.2.46/bluepyefe/reader.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.45/bluepyefe/recording.py` & `bluepyefe-2.2.46/bluepyefe/recording.py`

 * *Files 8% similar despite different names*

```diff
@@ -220,36 +220,49 @@
 
         if "repetition" in reader_data:
             self.repetition = reader_data["repetition"]
 
         return t, current, voltage
 
     def call_efel(self, efeatures, efel_settings=None):
-        """ Calls efel to computed the wanted efeature """
+        """ Calls efel to compute the wanted efeatures """
 
         if efel_settings is None:
             efel_settings = {}
 
         settings = {"stimulus_current": self.amp}
 
         if "Threshold" not in efel_settings and self.auto_threshold is not None:
             logger.warning(f"Threshold was not provided and was automatically"
                            f" set to {self.auto_threshold}")
             settings["Threshold"] = self.auto_threshold
 
         for setting in efel_settings:
             if setting not in ['stim_start', 'stim_end']:
                 settings[setting] = efel_settings[setting]
+
+        stim_start = efel_settings.get('stim_start', self.ton)
+        stim_end = efel_settings.get('stim_end', self.toff)
+
+        # Special case for SpikeRec
+        if "multiple_decay_time_constant_after_stim" in efeatures:
+            if hasattr(self, "multi_stim_start") and hasattr(self, "multi_stim_end"):
+                settings["multi_stim_start"] = self.multi_stim_start
+                settings["multi_stim_end"] = self.multi_stim_end
+            elif "stim_start" in efel_settings and "stim_end" in efel_settings:
+                settings["multi_stim_start"] = [stim_start]
+                settings["multi_stim_end"] = [stim_end]
+
         set_efel_settings(settings)
 
         efel_trace = {
             "T": self.t,
             "V": self.voltage,
-            'stim_start': [efel_settings.get('stim_start', self.ton)],
-            'stim_end': [efel_settings.get('stim_end', self.toff)]
+            'stim_start': [stim_start],
+            'stim_end': [stim_end]
         }
 
         try:
             return efel.getFeatureValues(
                 [efel_trace], efeatures, raise_warnings=False
             )
         except TypeError as e:
```

### Comparing `bluepyefe-2.2.45/bluepyefe/rheobase.py` & `bluepyefe-2.2.46/bluepyefe/rheobase.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.45/bluepyefe/target.py` & `bluepyefe-2.2.46/bluepyefe/target.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.45/bluepyefe/tools.py` & `bluepyefe-2.2.46/bluepyefe/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
         if setting == 'Threshold':
             efel.setThreshold(value)
 
         elif isinstance(value, bool) or isinstance(value, int):
             efel.setIntSetting(setting, int(value))
 
-        elif isinstance(value, float):
+        elif isinstance(value, (float, list)):
             efel.setDoubleSetting(setting, value)
 
         elif isinstance(value, str):
             efel.setStrSetting(setting, value)
 
 
 def dict_to_json(data, path):
```

### Comparing `bluepyefe-2.2.45/bluepyefe/translate_legacy_config.py` & `bluepyefe-2.2.46/bluepyefe/translate_legacy_config.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.45/bluepyefe.egg-info/PKG-INFO` & `bluepyefe-2.2.46/bluepyefe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: bluepyefe
-Version: 2.2.45
+Version: 2.2.46
 Summary: Blue Brain Python E-feature extraction
 Home-page: https://github.com/BlueBrain/BluePyEfe
 Author: BlueBrain Project, EPFL
 License: LGPLv3
 Description: The Blue Brain Python E-feature extraction Library (BluePyEfe) aims at easing the process of reading experimental recordings and extracting batches of electrical features from them. To do so, it combines trace reading functions and features extraction functions from the eFel library. BluePyEfe outputs protocols and features files in a format that can then be used by BluePyOpt for electrical model building purposes.
 Keywords: neuroscience,BlueBrainProject
 Platform: UNKNOWN
```

### Comparing `bluepyefe-2.2.45/bluepyefe.egg-info/SOURCES.txt` & `bluepyefe-2.2.46/bluepyefe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.45/examples/__init__.py` & `bluepyefe-2.2.46/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.45/setup.py` & `bluepyefe-2.2.46/setup.py`

 * *Files identical despite different names*

### Comparing `bluepyefe-2.2.45/versioneer.py` & `bluepyefe-2.2.46/versioneer.py`

 * *Files identical despite different names*

