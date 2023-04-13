# Comparing `tmp/conformine-0.0.1b12.tar.gz` & `tmp/conformine-0.0.1b14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conformine-0.0.1b12.tar", last modified: Thu Apr 13 09:42:25 2023, max compression
+gzip compressed data, was "conformine-0.0.1b14.tar", last modified: Thu Apr 13 09:53:35 2023, max compression
```

## Comparing `conformine-0.0.1b12.tar` & `conformine-0.0.1b14.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2023-04-13 09:42:25.819651 conformine-0.0.1b12/
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)      272 2023-04-06 21:48:26.000000 conformine-0.0.1b12/MANIFEST.in
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     6895 2023-04-13 09:42:25.819223 conformine-0.0.1b12/PKG-INFO
-drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2023-04-13 09:42:25.780480 conformine-0.0.1b12/conformine/
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     5726 2023-04-13 09:29:48.000000 conformine-0.0.1b12/conformine/README.md
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)       57 2023-02-08 13:39:41.000000 conformine-0.0.1b12/conformine/__init__.py
-drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2023-04-13 09:42:25.788179 conformine-0.0.1b12/conformine/utils/
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)        0 2023-02-07 15:14:39.000000 conformine-0.0.1b12/conformine/utils/__init__.py
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)      607 2023-02-07 13:39:38.000000 conformine-0.0.1b12/conformine/utils/data_utils.py
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     1142 2023-02-07 16:22:52.000000 conformine-0.0.1b12/conformine/utils/dataset_utils.py
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     4696 2023-04-13 09:39:44.000000 conformine-0.0.1b12/conformine/utils/from_fasta_standalone_predictor.py
-drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2023-04-13 09:42:25.805810 conformine-0.0.1b12/conformine/utils/models/
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)      645 2023-02-16 23:19:48.000000 conformine-0.0.1b12/conformine/utils/models/113_correct_normalization_parameters.json
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)        0 2023-02-07 15:14:39.000000 conformine-0.0.1b12/conformine/utils/models/__init__.py
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)      521 2023-02-23 12:24:25.000000 conformine-0.0.1b12/conformine/utils/models/minmax_scaler_bw_0.13_ground_clean_1.2.1.pkl
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)      521 2023-02-23 10:18:36.000000 conformine-0.0.1b12/conformine/utils/models/minmax_scaler_bw_0.13_ground_clean_1.22.4.pkl
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)      521 2023-04-06 21:47:47.000000 conformine-0.0.1b12/conformine/utils/models/minmax_scaler_bw_0.13_ground_clean_pickle_version_1.2.1.pkl
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)      521 2023-02-10 16:36:35.000000 conformine-0.0.1b12/conformine/utils/models/minmax_scaler_bw_0.13_ground_sklearn_1.2.1.pkl
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)      521 2023-02-08 14:26:36.000000 conformine-0.0.1b12/conformine/utils/models/minmax_scaler_ground_sklearn_1.2.1.pkl
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)      719 2023-02-14 16:58:01.000000 conformine-0.0.1b12/conformine/utils/models/normalization_parameters.json
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)   384187 2023-02-08 12:20:02.000000 conformine-0.0.1b12/conformine/utils/models/state_dictionary_torch_model.pt
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)   956859 2023-02-20 16:42:14.000000 conformine-0.0.1b12/conformine/utils/models/state_dictionary_torch_model_bw_0.13.pt
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)   956859 2023-02-23 10:00:46.000000 conformine-0.0.1b12/conformine/utils/models/state_dictionary_torch_model_bw_0.13_clean.pt
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     2821 2023-04-06 21:43:23.000000 conformine-0.0.1b12/conformine/utils/network_utils.py
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     5450 2023-02-20 16:50:17.000000 conformine-0.0.1b12/conformine/utils/pytorch_models.py
-drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2023-04-13 09:42:25.818095 conformine-0.0.1b12/conformine/wrapper_source/
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)        0 2023-02-07 16:06:07.000000 conformine-0.0.1b12/conformine/wrapper_source/__init__.py
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)      794 2023-02-08 15:04:32.000000 conformine-0.0.1b12/conformine/wrapper_source/conformine_wrapper.py
-drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2023-04-13 09:42:25.783543 conformine-0.0.1b12/conformine.egg-info/
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     6895 2023-04-13 09:42:25.000000 conformine-0.0.1b12/conformine.egg-info/PKG-INFO
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     1237 2023-04-13 09:42:25.000000 conformine-0.0.1b12/conformine.egg-info/SOURCES.txt
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)        1 2023-04-13 09:42:25.000000 conformine-0.0.1b12/conformine.egg-info/dependency_links.txt
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)      143 2023-04-13 09:42:25.000000 conformine-0.0.1b12/conformine.egg-info/requires.txt
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)       11 2023-04-13 09:42:25.000000 conformine-0.0.1b12/conformine.egg-info/top_level.txt
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)       38 2023-04-13 09:42:25.819761 conformine-0.0.1b12/setup.cfg
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     2106 2023-04-13 09:42:14.000000 conformine-0.0.1b12/setup.py
+drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2023-04-13 09:53:35.044388 conformine-0.0.1b14/
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)      272 2023-04-06 21:48:26.000000 conformine-0.0.1b14/MANIFEST.in
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     6889 2023-04-13 09:53:35.043699 conformine-0.0.1b14/PKG-INFO
+drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2023-04-13 09:53:35.014318 conformine-0.0.1b14/conformine/
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     5720 2023-04-13 09:53:01.000000 conformine-0.0.1b14/conformine/README.md
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)       57 2023-02-08 13:39:41.000000 conformine-0.0.1b14/conformine/__init__.py
+drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2023-04-13 09:53:35.021497 conformine-0.0.1b14/conformine/utils/
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)        0 2023-02-07 15:14:39.000000 conformine-0.0.1b14/conformine/utils/__init__.py
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     1000 2023-04-13 09:50:30.000000 conformine-0.0.1b14/conformine/utils/data_utils.py
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     1142 2023-02-07 16:22:52.000000 conformine-0.0.1b14/conformine/utils/dataset_utils.py
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     4445 2023-04-13 09:50:21.000000 conformine-0.0.1b14/conformine/utils/from_fasta_standalone_predictor.py
+drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2023-04-13 09:53:35.037425 conformine-0.0.1b14/conformine/utils/models/
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)      645 2023-02-16 23:19:48.000000 conformine-0.0.1b14/conformine/utils/models/113_correct_normalization_parameters.json
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)        0 2023-02-07 15:14:39.000000 conformine-0.0.1b14/conformine/utils/models/__init__.py
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)      521 2023-02-23 12:24:25.000000 conformine-0.0.1b14/conformine/utils/models/minmax_scaler_bw_0.13_ground_clean_1.2.1.pkl
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)      521 2023-02-23 10:18:36.000000 conformine-0.0.1b14/conformine/utils/models/minmax_scaler_bw_0.13_ground_clean_1.22.4.pkl
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)      521 2023-04-06 21:47:47.000000 conformine-0.0.1b14/conformine/utils/models/minmax_scaler_bw_0.13_ground_clean_pickle_version_1.2.1.pkl
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)      521 2023-02-10 16:36:35.000000 conformine-0.0.1b14/conformine/utils/models/minmax_scaler_bw_0.13_ground_sklearn_1.2.1.pkl
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)      521 2023-02-08 14:26:36.000000 conformine-0.0.1b14/conformine/utils/models/minmax_scaler_ground_sklearn_1.2.1.pkl
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)      719 2023-02-14 16:58:01.000000 conformine-0.0.1b14/conformine/utils/models/normalization_parameters.json
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)   384187 2023-02-08 12:20:02.000000 conformine-0.0.1b14/conformine/utils/models/state_dictionary_torch_model.pt
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)   956859 2023-02-20 16:42:14.000000 conformine-0.0.1b14/conformine/utils/models/state_dictionary_torch_model_bw_0.13.pt
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)   956859 2023-02-23 10:00:46.000000 conformine-0.0.1b14/conformine/utils/models/state_dictionary_torch_model_bw_0.13_clean.pt
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     2821 2023-04-06 21:43:23.000000 conformine-0.0.1b14/conformine/utils/network_utils.py
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     5450 2023-02-20 16:50:17.000000 conformine-0.0.1b14/conformine/utils/pytorch_models.py
+drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2023-04-13 09:53:35.042324 conformine-0.0.1b14/conformine/wrapper_source/
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)        0 2023-02-07 16:06:07.000000 conformine-0.0.1b14/conformine/wrapper_source/__init__.py
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)      794 2023-02-08 15:04:32.000000 conformine-0.0.1b14/conformine/wrapper_source/conformine_wrapper.py
+drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2023-04-13 09:53:35.016781 conformine-0.0.1b14/conformine.egg-info/
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     6889 2023-04-13 09:53:34.000000 conformine-0.0.1b14/conformine.egg-info/PKG-INFO
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     1237 2023-04-13 09:53:34.000000 conformine-0.0.1b14/conformine.egg-info/SOURCES.txt
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)        1 2023-04-13 09:53:34.000000 conformine-0.0.1b14/conformine.egg-info/dependency_links.txt
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)      143 2023-04-13 09:53:34.000000 conformine-0.0.1b14/conformine.egg-info/requires.txt
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)       11 2023-04-13 09:53:34.000000 conformine-0.0.1b14/conformine.egg-info/top_level.txt
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)       38 2023-04-13 09:53:35.044548 conformine-0.0.1b14/setup.cfg
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     2106 2023-04-13 09:53:11.000000 conformine-0.0.1b14/setup.py
```

### Comparing `conformine-0.0.1b12/PKG-INFO` & `conformine-0.0.1b14/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conformine
-Version: 0.0.1b12
+Version: 0.0.1b14
 Summary: ConforMine, a predictor of conformational variability from amino acid sequence
 Author: Jose Gavalda-Garcia
 Author-email: jose.gavalda.garcia@vub.be
 Maintainer: Jose Gavalda-Garcia, Adrian Diaz, Wim Vranken
 Maintainer-email: jose.gavalda.garcia@vub.be, adrian.diaz@vub.be, wim.vranken@vub.be
 Keywords: b2bTools,biology,bioinformatics,bio-informatics,fasta,proteins,protein-conformation,conformational-variability
 Classifier: Natural Language :: English
@@ -82,15 +82,15 @@
 ```python
 conf.predict()
 ```
 
 4) Get the prediction values after running the predictor for a specific sequence identifier:
 
 ```python
-predictions = single_seq.get_all_predictions()
+predictions = conf.get_all_predictions()
 ```
 
 **⚠️ Important note:** The method `get_all_predictions` will return a dictionary with the following structure:
 
 ```python
 {
   "SEQUENCE_ID_000": {
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: conformine Version: 0.0.1b12 Summary: ConforMine, a
+Metadata-Version: 2.1 Name: conformine Version: 0.0.1b14 Summary: ConforMine, a
 predictor of conformational variability from amino acid sequence Author: Jose
 Gavalda-Garcia Author-email: jose.gavalda.garcia@vub.be Maintainer: Jose
 Gavalda-Garcia, Adrian Diaz, Wim Vranken Maintainer-email:
 jose.gavalda.garcia@vub.be, adrian.diaz@vub.be, wim.vranken@vub.be Keywords:
 b2bTools,biology,bioinformatics,bio-informatics,fasta,proteins,protein-
 conformation,conformational-variability Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
@@ -29,16 +29,16 @@
 ('aa_position') plt.ylabel('pred_values') plt.show() ``` ### ð§­ Basic flow
 This section will explain you in details the script mentioned inside the Quick
 start section. 1) Import the `Conformine` class from the `conformine` package:
 ```python from conformine import Conformine ``` 2) Instantiate an object by
 passing the path to the input file in FASTA format: ```python conf = Conformine
 ("/path/to/example.fasta") ``` 3) Run the predictions: ```python conf.predict()
 ``` 4) Get the prediction values after running the predictor for a specific
-sequence identifier: ```python predictions = single_seq.get_all_predictions()
-``` **â ï¸ Important note:** The method `get_all_predictions` will return a
+sequence identifier: ```python predictions = conf.get_all_predictions() ```
+**â ï¸ Important note:** The method `get_all_predictions` will return a
 dictionary with the following structure: ```python { "SEQUENCE_ID_000": { "id":
 "SEQUENCE_ID_000", "seq": "the input sequence 0", "result001": [0.001, 0.002,
 ..., 0.00], "result002": [0.001, 0.002, ..., 0.00], "...": [...], "resultN":
 [0.001, 0.002, ..., 0.00] }, "SEQUENCE_ID_001": { "id": "SEQUENCE_ID_001",
 "seq": "the input sequence 1", "result001": [0.001, 0.002, ..., 0.00],
 "result002": [0.001, 0.002, ..., 0.00], "...": [...], "resultN": [0.001, 0.002,
 ..., 0.00] }, "...": { ... }, "SEQUENCE_ID_N": { "id": "SEQUENCE_ID_N", "seq":
```

### Comparing `conformine-0.0.1b12/conformine/README.md` & `conformine-0.0.1b14/conformine/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 ```python
 conf.predict()
 ```
 
 4) Get the prediction values after running the predictor for a specific sequence identifier:
 
 ```python
-predictions = single_seq.get_all_predictions()
+predictions = conf.get_all_predictions()
 ```
 
 **⚠️ Important note:** The method `get_all_predictions` will return a dictionary with the following structure:
 
 ```python
 {
   "SEQUENCE_ID_000": {
```

#### html2text {}

```diff
@@ -13,16 +13,16 @@
 ('aa_position') plt.ylabel('pred_values') plt.show() ``` ### ð§­ Basic flow
 This section will explain you in details the script mentioned inside the Quick
 start section. 1) Import the `Conformine` class from the `conformine` package:
 ```python from conformine import Conformine ``` 2) Instantiate an object by
 passing the path to the input file in FASTA format: ```python conf = Conformine
 ("/path/to/example.fasta") ``` 3) Run the predictions: ```python conf.predict()
 ``` 4) Get the prediction values after running the predictor for a specific
-sequence identifier: ```python predictions = single_seq.get_all_predictions()
-``` **â ï¸ Important note:** The method `get_all_predictions` will return a
+sequence identifier: ```python predictions = conf.get_all_predictions() ```
+**â ï¸ Important note:** The method `get_all_predictions` will return a
 dictionary with the following structure: ```python { "SEQUENCE_ID_000": { "id":
 "SEQUENCE_ID_000", "seq": "the input sequence 0", "result001": [0.001, 0.002,
 ..., 0.00], "result002": [0.001, 0.002, ..., 0.00], "...": [...], "resultN":
 [0.001, 0.002, ..., 0.00] }, "SEQUENCE_ID_001": { "id": "SEQUENCE_ID_001",
 "seq": "the input sequence 1", "result001": [0.001, 0.002, ..., 0.00],
 "result002": [0.001, 0.002, ..., 0.00], "...": [...], "resultN": [0.001, 0.002,
 ..., 0.00] }, "...": { ... }, "SEQUENCE_ID_N": { "id": "SEQUENCE_ID_N", "seq":
```

### Comparing `conformine-0.0.1b12/conformine/utils/data_utils.py` & `conformine-0.0.1b14/conformine/utils/data_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from Bio import SeqIO
 import numpy as np
 
 
 def read_fasta(fasta_path):
     fasta_dict = {}
     for record in SeqIO.parse(fasta_path, 'fasta'):
-        fasta_dict[record.id] = record.seq
+        record.description = record.description.replace(" ", "_").replace(".", "").replace("|", "_").replace(",",
+                                                                                                             "_")
+        first_20_description = record.description[:20]
+
+        # fasta_dict[record.id] = record.seq  # Changed so that the code can handle spaces and so
+        fasta_dict[first_20_description] = record.seq
 
     return fasta_dict
 
 
 def fasta_to_index(fasta_dict):
     index_dict = {}
```

### Comparing `conformine-0.0.1b12/conformine/utils/dataset_utils.py` & `conformine-0.0.1b14/conformine/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `conformine-0.0.1b12/conformine/utils/from_fasta_standalone_predictor.py` & `conformine-0.0.1b14/conformine/utils/from_fasta_standalone_predictor.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,23 +53,14 @@
     predictions_dict = model_wrapper.predict(dataset, batch_size=100)
 
     # corrected_parameters_path = os.path.join(rootdir, 'utils/models/normalization_parameters.json')
     corrected_parameters_path = os.path.join(rootdir, 'utils/models/113_correct_normalization_parameters.json')
     with open(corrected_parameters_path, 'r') as f:
         corrected_parameters_dict = json.load(f)
 
-    # positional_to_name = {
-    #     'ConVa': '0',
-    #     'core_alpha': '1',
-    #     'core_beta': '2',
-    #     'other_conformation': '3',
-    #     'surr_alpha': '4',
-    #     'surr_beta': '5',
-    #     'Predicted_ShiftCrypt': '6',
-    # }
     positional_to_name = {
         'ConVa': '0',
         'core_helix': '1',
         'core_sheet': '2',
         'other_conformation': '3',
         'surr_helix': '4',
         'surr_sheet': '5',
```

### Comparing `conformine-0.0.1b12/conformine/utils/models/113_correct_normalization_parameters.json` & `conformine-0.0.1b14/conformine/utils/models/113_correct_normalization_parameters.json`

 * *Files identical despite different names*

### Comparing `conformine-0.0.1b12/conformine/utils/models/minmax_scaler_bw_0.13_ground_clean_1.2.1.pkl` & `conformine-0.0.1b14/conformine/utils/models/minmax_scaler_bw_0.13_ground_clean_1.2.1.pkl`

 * *Files identical despite different names*

### Comparing `conformine-0.0.1b12/conformine/utils/models/minmax_scaler_bw_0.13_ground_clean_1.22.4.pkl` & `conformine-0.0.1b14/conformine/utils/models/minmax_scaler_bw_0.13_ground_clean_1.22.4.pkl`

 * *Files identical despite different names*

### Comparing `conformine-0.0.1b12/conformine/utils/models/minmax_scaler_bw_0.13_ground_clean_pickle_version_1.2.1.pkl` & `conformine-0.0.1b14/conformine/utils/models/minmax_scaler_bw_0.13_ground_clean_pickle_version_1.2.1.pkl`

 * *Files identical despite different names*

### Comparing `conformine-0.0.1b12/conformine/utils/models/minmax_scaler_bw_0.13_ground_sklearn_1.2.1.pkl` & `conformine-0.0.1b14/conformine/utils/models/minmax_scaler_bw_0.13_ground_sklearn_1.2.1.pkl`

 * *Files identical despite different names*

### Comparing `conformine-0.0.1b12/conformine/utils/models/minmax_scaler_ground_sklearn_1.2.1.pkl` & `conformine-0.0.1b14/conformine/utils/models/minmax_scaler_ground_sklearn_1.2.1.pkl`

 * *Files identical despite different names*

### Comparing `conformine-0.0.1b12/conformine/utils/models/normalization_parameters.json` & `conformine-0.0.1b14/conformine/utils/models/normalization_parameters.json`

 * *Files identical despite different names*

### Comparing `conformine-0.0.1b12/conformine/utils/models/state_dictionary_torch_model.pt` & `conformine-0.0.1b14/conformine/utils/models/state_dictionary_torch_model.pt`

 * *Files identical despite different names*

### Comparing `conformine-0.0.1b12/conformine/utils/models/state_dictionary_torch_model_bw_0.13.pt` & `conformine-0.0.1b14/conformine/utils/models/state_dictionary_torch_model_bw_0.13.pt`

 * *Files identical despite different names*

### Comparing `conformine-0.0.1b12/conformine/utils/models/state_dictionary_torch_model_bw_0.13_clean.pt` & `conformine-0.0.1b14/conformine/utils/models/state_dictionary_torch_model_bw_0.13_clean.pt`

 * *Files identical despite different names*

### Comparing `conformine-0.0.1b12/conformine/utils/network_utils.py` & `conformine-0.0.1b14/conformine/utils/network_utils.py`

 * *Files identical despite different names*

### Comparing `conformine-0.0.1b12/conformine/utils/pytorch_models.py` & `conformine-0.0.1b14/conformine/utils/pytorch_models.py`

 * *Files identical despite different names*

### Comparing `conformine-0.0.1b12/conformine/wrapper_source/conformine_wrapper.py` & `conformine-0.0.1b14/conformine/wrapper_source/conformine_wrapper.py`

 * *Files identical despite different names*

### Comparing `conformine-0.0.1b12/conformine.egg-info/PKG-INFO` & `conformine-0.0.1b14/conformine.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conformine
-Version: 0.0.1b12
+Version: 0.0.1b14
 Summary: ConforMine, a predictor of conformational variability from amino acid sequence
 Author: Jose Gavalda-Garcia
 Author-email: jose.gavalda.garcia@vub.be
 Maintainer: Jose Gavalda-Garcia, Adrian Diaz, Wim Vranken
 Maintainer-email: jose.gavalda.garcia@vub.be, adrian.diaz@vub.be, wim.vranken@vub.be
 Keywords: b2bTools,biology,bioinformatics,bio-informatics,fasta,proteins,protein-conformation,conformational-variability
 Classifier: Natural Language :: English
@@ -82,15 +82,15 @@
 ```python
 conf.predict()
 ```
 
 4) Get the prediction values after running the predictor for a specific sequence identifier:
 
 ```python
-predictions = single_seq.get_all_predictions()
+predictions = conf.get_all_predictions()
 ```
 
 **⚠️ Important note:** The method `get_all_predictions` will return a dictionary with the following structure:
 
 ```python
 {
   "SEQUENCE_ID_000": {
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: conformine Version: 0.0.1b12 Summary: ConforMine, a
+Metadata-Version: 2.1 Name: conformine Version: 0.0.1b14 Summary: ConforMine, a
 predictor of conformational variability from amino acid sequence Author: Jose
 Gavalda-Garcia Author-email: jose.gavalda.garcia@vub.be Maintainer: Jose
 Gavalda-Garcia, Adrian Diaz, Wim Vranken Maintainer-email:
 jose.gavalda.garcia@vub.be, adrian.diaz@vub.be, wim.vranken@vub.be Keywords:
 b2bTools,biology,bioinformatics,bio-informatics,fasta,proteins,protein-
 conformation,conformational-variability Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
@@ -29,16 +29,16 @@
 ('aa_position') plt.ylabel('pred_values') plt.show() ``` ### ð§­ Basic flow
 This section will explain you in details the script mentioned inside the Quick
 start section. 1) Import the `Conformine` class from the `conformine` package:
 ```python from conformine import Conformine ``` 2) Instantiate an object by
 passing the path to the input file in FASTA format: ```python conf = Conformine
 ("/path/to/example.fasta") ``` 3) Run the predictions: ```python conf.predict()
 ``` 4) Get the prediction values after running the predictor for a specific
-sequence identifier: ```python predictions = single_seq.get_all_predictions()
-``` **â ï¸ Important note:** The method `get_all_predictions` will return a
+sequence identifier: ```python predictions = conf.get_all_predictions() ```
+**â ï¸ Important note:** The method `get_all_predictions` will return a
 dictionary with the following structure: ```python { "SEQUENCE_ID_000": { "id":
 "SEQUENCE_ID_000", "seq": "the input sequence 0", "result001": [0.001, 0.002,
 ..., 0.00], "result002": [0.001, 0.002, ..., 0.00], "...": [...], "resultN":
 [0.001, 0.002, ..., 0.00] }, "SEQUENCE_ID_001": { "id": "SEQUENCE_ID_001",
 "seq": "the input sequence 1", "result001": [0.001, 0.002, ..., 0.00],
 "result002": [0.001, 0.002, ..., 0.00], "...": [...], "resultN": [0.001, 0.002,
 ..., 0.00] }, "...": { ... }, "SEQUENCE_ID_N": { "id": "SEQUENCE_ID_N", "seq":
```

### Comparing `conformine-0.0.1b12/conformine.egg-info/SOURCES.txt` & `conformine-0.0.1b14/conformine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `conformine-0.0.1b12/setup.py` & `conformine-0.0.1b14/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 with open(os.path.join(os.path.abspath(get_project_root()), "conformine/README.md"), "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name='conformine',
-    version='0.0.1b12',
+    version='0.0.1b14',
     description='ConforMine, a predictor of conformational variability from amino acid sequence',
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="b2bTools,biology,bioinformatics,bio-informatics,fasta,proteins,protein-conformation,"
              "conformational-variability",
     # url='https://github.com/your-username/your-package-name',
     author='Jose Gavalda-Garcia',
```

