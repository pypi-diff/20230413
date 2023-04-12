# Comparing `tmp/qudi_hira_analysis-1.4.0.tar.gz` & `tmp/qudi_hira_analysis-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qudi_hira_analysis-1.4.0.tar", max compression
+gzip compressed data, was "qudi_hira_analysis-1.4.1.tar", max compression
```

## Comparing `qudi_hira_analysis-1.4.0.tar` & `qudi_hira_analysis-1.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1069 2023-02-26 15:52:31.954729 qudi_hira_analysis-1.4.0/LICENSE
--rw-r--r--   0        0        0    10431 2023-04-12 19:37:13.223794 qudi_hira_analysis-1.4.0/README.md
--rw-r--r--   0        0        0      868 2023-04-12 19:39:36.964668 qudi_hira_analysis-1.4.0/pyproject.toml
--rw-r--r--   0        0        0      171 2023-03-05 21:19:20.709702 qudi_hira_analysis-1.4.0/qudi_hira_analysis/__init__.py
--rw-r--r--   0        0        0    11044 2023-04-12 19:03:20.871413 qudi_hira_analysis-1.4.0/qudi_hira_analysis/analysis_logic.py
--rw-r--r--   0        0        0    13112 2023-04-12 19:28:24.073699 qudi_hira_analysis-1.4.0/qudi_hira_analysis/data_handler.py
--rw-r--r--   0        0        0        0 2023-03-05 21:19:20.710018 qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/__init__.py
--rw-r--r--   0        0        0     1936 2023-03-05 21:19:20.710848 qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/antibunchingmethods.py
--rw-r--r--   0        0        0    24480 2023-03-05 21:19:20.711380 qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/decaylikemethods.py
--rw-r--r--   0        0        0    40854 2023-03-05 21:19:20.711692 qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/gaussianlikemethods.py
--rw-r--r--   0        0        0    23150 2023-03-05 21:19:20.711989 qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/generalmethods.py
--rw-r--r--   0        0        0     5848 2023-03-05 21:19:20.712252 qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/hyperbolicsaturationmethods.py
--rw-r--r--   0        0        0    10577 2023-03-05 21:19:20.712412 qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/linearmethods.py
--rw-r--r--   0        0        0    41457 2023-03-05 21:19:20.712635 qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/lorentzianlikemethods.py
--rw-r--r--   0        0        0    16450 2023-03-05 21:19:20.712885 qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/poissonianlikemethods.py
--rw-r--r--   0        0        0   106110 2023-03-05 21:19:20.713199 qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/sinemethods.py
--rw-r--r--   0        0        0     1792 2023-04-12 17:43:42.063526 qudi_hira_analysis-1.4.0/qudi_hira_analysis/helper_functions.py
--rw-r--r--   0        0        0    12696 2023-04-12 17:43:42.063710 qudi_hira_analysis-1.4.0/qudi_hira_analysis/io_handler.py
--rw-r--r--   0        0        0     6758 2023-04-12 17:43:42.063880 qudi_hira_analysis-1.4.0/qudi_hira_analysis/measurement_dataclass.py
--rw-r--r--   0        0        0    18729 2023-03-05 21:19:20.714069 qudi_hira_analysis-1.4.0/qudi_hira_analysis/qudi_fit_logic.py
--rw-r--r--   0        0        0    11429 1970-01-01 00:00:00.000000 qudi_hira_analysis-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-02-26 15:52:31.954729 qudi_hira_analysis-1.4.1/LICENSE
+-rw-r--r--   0        0        0    12051 2023-04-12 22:48:36.514126 qudi_hira_analysis-1.4.1/README.md
+-rw-r--r--   0        0        0      868 2023-04-12 22:48:36.517143 qudi_hira_analysis-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0      171 2023-03-05 21:19:20.709702 qudi_hira_analysis-1.4.1/qudi_hira_analysis/__init__.py
+-rw-r--r--   0        0        0    11044 2023-04-12 19:03:20.871413 qudi_hira_analysis-1.4.1/qudi_hira_analysis/analysis_logic.py
+-rw-r--r--   0        0        0    12658 2023-04-12 22:48:36.510553 qudi_hira_analysis-1.4.1/qudi_hira_analysis/data_handler.py
+-rw-r--r--   0        0        0        0 2023-03-05 21:19:20.710018 qudi_hira_analysis-1.4.1/qudi_hira_analysis/fitmethods/__init__.py
+-rw-r--r--   0        0        0     1936 2023-03-05 21:19:20.710848 qudi_hira_analysis-1.4.1/qudi_hira_analysis/fitmethods/antibunchingmethods.py
+-rw-r--r--   0        0        0    24480 2023-03-05 21:19:20.711380 qudi_hira_analysis-1.4.1/qudi_hira_analysis/fitmethods/decaylikemethods.py
+-rw-r--r--   0        0        0    40854 2023-03-05 21:19:20.711692 qudi_hira_analysis-1.4.1/qudi_hira_analysis/fitmethods/gaussianlikemethods.py
+-rw-r--r--   0        0        0    23150 2023-03-05 21:19:20.711989 qudi_hira_analysis-1.4.1/qudi_hira_analysis/fitmethods/generalmethods.py
+-rw-r--r--   0        0        0     5848 2023-03-05 21:19:20.712252 qudi_hira_analysis-1.4.1/qudi_hira_analysis/fitmethods/hyperbolicsaturationmethods.py
+-rw-r--r--   0        0        0    10577 2023-03-05 21:19:20.712412 qudi_hira_analysis-1.4.1/qudi_hira_analysis/fitmethods/linearmethods.py
+-rw-r--r--   0        0        0    41457 2023-03-05 21:19:20.712635 qudi_hira_analysis-1.4.1/qudi_hira_analysis/fitmethods/lorentzianlikemethods.py
+-rw-r--r--   0        0        0    16450 2023-03-05 21:19:20.712885 qudi_hira_analysis-1.4.1/qudi_hira_analysis/fitmethods/poissonianlikemethods.py
+-rw-r--r--   0        0        0   106110 2023-03-05 21:19:20.713199 qudi_hira_analysis-1.4.1/qudi_hira_analysis/fitmethods/sinemethods.py
+-rw-r--r--   0        0        0     1792 2023-04-12 17:43:42.063526 qudi_hira_analysis-1.4.1/qudi_hira_analysis/helper_functions.py
+-rw-r--r--   0        0        0    12696 2023-04-12 17:43:42.063710 qudi_hira_analysis-1.4.1/qudi_hira_analysis/io_handler.py
+-rw-r--r--   0        0        0     6758 2023-04-12 17:43:42.063880 qudi_hira_analysis-1.4.1/qudi_hira_analysis/measurement_dataclass.py
+-rw-r--r--   0        0        0    18729 2023-03-05 21:19:20.714069 qudi_hira_analysis-1.4.1/qudi_hira_analysis/qudi_fit_logic.py
+-rw-r--r--   0        0        0    13049 1970-01-01 00:00:00.000000 qudi_hira_analysis-1.4.1/PKG-INFO
```

### Comparing `qudi_hira_analysis-1.4.0/LICENSE` & `qudi_hira_analysis-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.4.0/README.md` & `qudi_hira_analysis-1.4.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: qudi-hira-analysis
+Version: 1.4.1
+Summary: A Python toolkit to analzye photon timetrace data from qubit sensors
+Home-page: https://github.com/dineshpinto/qudi-hira-analysis
+License: MIT
+Keywords: python,qubit,analysis,nv centers,photon timetrace
+Author: dineshpinto
+Author-email: annual.fallout_0z@icloud.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: lmfit (>=1.1.0,<2.0.0)
+Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
+Requires-Dist: numpy (>=1.24.0,<2.0.0)
+Requires-Dist: openpyxl (>=3.0.10,<4.0.0)
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
+Requires-Dist: pyspm (>=0.3.0,<0.4.0)
+Requires-Dist: tqdm (>=4.64.1,<5.0.0)
+Requires-Dist: xlrd (>=2.0.1,<3.0.0)
+Project-URL: Repository, https://github.com/dineshpinto/qudi-hira-analysis
+Description-Content-Type: text/markdown
+
 [![DOI](https://zenodo.org/badge/288670453.svg)](https://zenodo.org/badge/latestdoi/288670453)
 [![Downloads](https://pepy.tech/badge/qudi-hira-analysis)](https://pepy.tech/project/qudi-hira-analysis)
 [![PyPi version](https://img.shields.io/pypi/v/qudi-hira-analysis)](https://pypi.python.org/pypi/qudi-hira-analysis/)
 [![Python 3.10](https://img.shields.io/badge/python-3.10-orange.svg)](https://www.python.org/downloads/release/python-3100//)
 [![Python 3.11](https://img.shields.io/badge/python-3.11-orange.svg)](https://www.python.org/downloads/release/python-3110//)
 
 # Qudi Hira Analysis
@@ -29,67 +54,160 @@
 pip install qudi-hira-analysis
 ```
 
 ## Citation
 
 If you are publishing scientific results, you can cite this work as:  https://doi.org/10.5281/zenodo.7604670
 
-## Schema
+## Examples
 
-The visual structure of the toolkit is shown in the schema below. It largely consists of three portions:
+First set up the `DataHandler` object (henceforth referred to as `dh`) with the correct paths to the data and figure
+folders.
 
-- `IOHandler` assumes a central store of raw data, which is never modified (read-only)
-- `DataHandler` automates the extraction of large amounts of data from the `IOHandler` interface
-- `AnalysisLogic` contains a set of automated fitting routines using `lmfit` internally (built on top of fitting
-  routines from the [qudi](https://github.com/Ulm-IQO/qudi) project)
+Everything revolves around the `dh` object. It is the main interface to the toolkit and is initialized with the
+following required arguments:
 
-This license of this project is located in the top level folder under `LICENSE`. Some specific files contain their
-individual licenses in the file header docstring.
+- `data_folder` is the main folder where all the data is stored, it can be the direct path to the data, or composed of
+  several sub-folders, each containing the data for a specific measurement
+- `figure_folder` is the folder where the output figures will be saved
 
-```mermaid
-flowchart TD;
-    IOHandler<-- Handle all IO operations -->DataLoader;
-    DataLoader<-- Map IO callables to data -->DataHandler;
-    DataHandler-- Structure extracted data -->MeasurementDataclass;
-    MeasurementDataclass-- Plot fitted data --> Plot[Visualize data and add context in JupyterLab];
-    Plot-- Save plotted data --> DataHandler;
-    style MeasurementDataclass fill:#bbf,stroke:#f66,stroke-width:2px,color:#fff,stroke-dasharray: 5 5
+Optional arguments:
+
+- `measurement_folder` is the specific sub-folder in `data_folder` where the data for a specific measurement is stored
+
+```python
+from pathlib import Path
+import matplotlib.pyplot as plt
+import seaborn as sns
+
+from qudi_hira_analysis import DataHandler
+
+dh = DataHandler(
+    data_folder=Path("C:\\", "Data"),
+    figure_folder=Path("C:\\", "QudiHiraAnalysis"),
+    measurement_folder=Path("20230101_NV1")
+)
+```
+
+To load a specific set of measurements from the data folder, use the `dh.load_measurements()` method, which takes the
+following required arguments:
+
+- `measurement_str` is the string that is used to identify the measurement. It is used to filter the data files in the
+  `data_folder` and `measurement_folder` (if specified)
+
+Optional arguments:
+
+- `qudi` is a boolean. If `True`, the data is assumed to be in the format used by Qudi (default: True)
+- `pulsed` is a boolean. If `True`, the data is assumed to be in the format used by Qudi for pulsed measurements (
+  default: False)
+- `extension` is the extension of the data files (default: ".dat")
+
+The `load_measurements` function returns a dictionary containing the measurement data filtered by `measurement_str`.
+
+- The dictionary keys are measurement timestamps in "(year)(month)(day)-(hour)(minute)-(second)" format.
+
+- The dictionary values are `MeasurementDataclass` objects whose schema is shown
+  visually [here](#measurement-dataclass-schema).
+
+### Example 1: Autocorrelation measurements (Antibunching fit)
+
+```python
+autocorrelation_measurements = dh.load_measurements(measurement_str="Autocorrelation")
+
+fig, ax = plt.subplots()
+
+for autocorrelation in autocorrelation_measurements.values():
+    # Plot the data
+    sns.lineplot(data=autocorrelation.data, x="Controlled variable(s)", y="g2(t)", ax=ax)
+    # Fit the data using the antibunching function
+    fit_x, fit_y, result = dh.fit(x="Controlled variable(s)", y="g2(t)", data=autocorrelation.data,
+                                  fit_function=dh.fit_function.antibunching)
+    # Plot the fit
+    sns.lineplot(x=fit_x, y=fit_y, ax=ax)
+
+# Save the figure to the figure folder specified earlier
+dh.save_figures(filepath="autocorrelation_variation", fig=fig)
 ```
 
-### Measurement Dataclass
+### Example 2: ODMR measurements (double Lorentzian 15N fit)
+
+```python
+odmr_measurements = dh.load_measurements(measurement_str="ODMR", pulsed=True)
+
+fig, ax = plt.subplots()
+
+for odmr in odmr_measurements.values():
+    sns.scatterplot(data=odmr.data, x="Controlled variable(Hz)", y="Signal", ax=ax)
+    fit_x, fit_y, result = dh.fit(x="Controlled variable(Hz)", y="Signal", data=odmr.data,
+                                  fit_function=dh.fit_function.lorentzian_double)
+    sns.lineplot(x=fit_x, y=fit_y, ax=ax)
+
+dh.save_figures(filepath="odmr_variation", fig=fig)
+```
+
+### Example 3: Rabi measurements (sine exponential decay fit)
+
+```python
+rabi_measurements = dh.load_measurements(measurement_str="Rabi", pulsed=True)
+
+fig, ax = plt.subplots()
+
+for rabi in rabi_measurements.values():
+    sns.scatterplot(data=rabi.data, x="Controlled variable(s)", y="Signal", ax=ax)
+    fit_x, fit_y, result = dh.fit(x="Controlled variable(s)", y="Signal", data=rabi.data,
+                                  fit_function=dh.fit_function.sineexponentialdecay)
+    sns.lineplot(x=fit_x, y=fit_y, ax=ax)
+
+dh.save_figures(filepath="rabi_variation", fig=fig)
+```
+
+### Example 4: Temperature data
+
+```python
+temperature_measurements = dh.load_measurements(measurement_str="Temperature")
+
+temperature = pd.concat([t.data for t in temperature_measurements.values()])
+
+fig, ax = plt.subplots()
+sns.lineplot(data=temperature, x="Time", y="Temperature", ax=ax)
+dh.save_figures(filepath="temperature_monitoring", fig=fig)
+```
+
+## Measurement Dataclass Schema
 
 ```mermaid
-flowchart LR;
+flowchart LR
     subgraph Standard Data
-        MeasurementDataclass-->filepath1[filepath: Path];
-        MeasurementDataclass-->data1[data: DataFrame];
-        MeasurementDataclass-->params1[params: dict];
-        MeasurementDataclass-->timestamp1[timestamp: datetime];
-        MeasurementDataclass-- analysis --oAnalysisLogic;
+        MeasurementDataclass --o filepath1[filepath: Path];
+        MeasurementDataclass --o data1[data: DataFrame];
+        MeasurementDataclass --o params1[params: dict];
+        MeasurementDataclass --o timestamp1[timestamp: datetime.datetime];
+        MeasurementDataclass --o methods1[get_param_from_filename: Callable];
+        MeasurementDataclass --o methods2[set_datetime_index: Callable];
     end
     subgraph Pulsed Data
-        MeasurementDataclass-- pulsed --oPulsedMeasurementDataclass;
-        PulsedMeasurementDataclass-- measurement --oPulsedMeasurement;
-        PulsedMeasurement--> filepath2[filepath: Path];
-        PulsedMeasurement--> data2[data: DataFrame];
-        PulsedMeasurement--> params2[params: dict];
-        PulsedMeasurementDataclass-- laser_pulses --oLaserPulses; 
-        LaserPulses--> filepath3[filepath: Path];
-        LaserPulses--> data3[data: DataFrame];
-        LaserPulses--> params3[params: dict];
-        PulsedMeasurementDataclass-- timetrace --oRawTimetrace;
-        RawTimetrace--> filepath4[filepath: Path];
-        RawTimetrace--> data4[data: DataFrame];
-        RawTimetrace--> params4[params: dict];
+        MeasurementDataclass -- pulsed --> PulsedMeasurementDataclass;
+        PulsedMeasurementDataclass -- measurement --> PulsedMeasurement;
+        PulsedMeasurement --o filepath2[filepath: Path];
+        PulsedMeasurement --o data2[data: DataFrame];
+        PulsedMeasurement --o params2[params: dict];
+        PulsedMeasurementDataclass -- laser_pulses --> LaserPulses;
+        LaserPulses --o filepath3[filepath: Path];
+        LaserPulses --o data3[data: DataFrame];
+        LaserPulses --o params3[params: dict];
+        PulsedMeasurementDataclass -- timetrace --> RawTimetrace;
+        RawTimetrace --o filepath4[filepath: Path];
+        RawTimetrace --o data4[data: DataFrame];
+        RawTimetrace --o params4[params: dict];
     end
 ```
 
-### Supports common fitting routines
+## Supports common fitting routines
 
-Fit routines included in `AnalysisLogic`
+To get the full list of available fit routines, use the `dh.fit_function` attribute. The fit functions are:
 
 | Dimension | Fit                           |
 |-----------|-------------------------------|
 | 1d        | decayexponential              |
 |           | biexponential                 |
 |           | decayexponentialstretched     |
 |           | gaussian                      |
@@ -107,20 +225,20 @@
 |           | sineexponentialdecay          |
 |           | sinestretchedexponentialdecay |
 |           | sinetriple                    |
 |           | sinetriplewithexpdecay        |
 |           | sinetriplewiththreeexpdecay   |
 | 2d        | twoDgaussian                  |
 
-### Inbuilt measurement tree visualizer
+## Inbuilt measurement tree visualizer
 
 ```ipython
->>> tip_2S6 = DataHandler(data_folder="C:\\Data", figure_folder="C:\\QudiHiraAnalysis",
+>>> data = DataHandler(data_folder="C:\\Data", figure_folder="C:\\QudiHiraAnalysis",
                       measurement_folder="20220621_FR0612-F2-2S6_uhv")
->>> tip_2S6.data_folder_tree()
+>>> data.data_folder_tree()
 
 # Output
 ├── 20211116_NetworkAnalysis_SampleIn_UpperPin.csv
 ├── 20211116_NetworkAnalysis_SampleOut_UpperPin.csv
 ├── 20211116_NetworkAnalysis_TipIn_LowerPin.csv
 ├── 20211116_NetworkAnalysis_TipIn_UpperPin.csv
 ├── 20211116_NetworkAnalysis_TipOut_LowerPin.csv
@@ -132,94 +250,33 @@
 │   ├── C2_TipLowerPin.txt
 │   └── C2_TipUpperPin.txt
 ├── Sample_MW_Pin_comparision.png
 ├── Tip_MW_Pin_comparision.png
 └── Tip_Sample_MW_Pin_comparision.png
 ```
 
-### Automated data extraction
-
-First set up the `DataHandler` object with the correct paths to the data and figure folders.
-
-```python
-from pathlib import Path
-import matplotlib.pyplot as plt
-import seaborn as sns
-
-from qudi_hira_analysis import DataHandler
-
-data = DataHandler(
-  data_folder=Path("C:\\", "Data"), 
-  figure_folder=Path("C:\\", "QudiHiraAnalysis"),
-  measurement_folder=Path("20230101_NV1")
-)
-```
-
-#### Example 1: Extract autocorrelation measurements, fit and save
-
-```python
-autocorrelation_measurements = data.load_measurements(measurement_str="Autocorrelation")
-
-fig, ax = plt.subplots()
-
-for autocorrelation in autocorrelation_measurements.values():
-  sns.lineplot(data=autocorrelation.data, x="Controlled variable(s)", y="g2(t)", ax=ax)
-  fit_x, fit_y, result = data.fit(
-    x="Controlled variable(s)", y="g2(t)", data=autocorrelation.data, fit_function=data.fit_function.antibunching
-  )
-  sns.lineplot(x=fit_x, y=fit_y, ax=ax)
-  
-data.save_figures(filepath="autocorrelation_variation", fig=fig)
-```
-
-#### Example 2: Extract ODMR measurements, fit and save
+## Overall Schema
 
-```python
-odmr_measurements = data.load_measurements(measurement_str="ODMR", pulsed=True)
-
-fig, ax = plt.subplots()
-
-for odmr in odmr_measurements.values():
-  sns.scatterplot(data=odmr.data, x="Controlled variable(Hz)", y="Signal", ax=ax)
-  fit_x, fit_y, result = data.fit(
-    x="Controlled variable(Hz)", y="Signal", data=odmr.data, fit_function=data.fit_function.lorentzian_double
-  )
-  sns.lineplot(x=fit_x, y=fit_y, ax=ax)
-
-data.save_figures(filepath="odmr_variation", fig=fig)
-```
-
-#### Example 3: Extract Rabi measurements, fit and save
-
-```python
-rabi_measurements = data.load_measurements(measurement_str="Rabi", pulsed=True)
-
-fig, ax = plt.subplots()
-
-for rabi in rabi_measurements.values():
-  sns.scatterplot(data=rabi.data, x="Controlled variable(s)", y="Signal", ax=ax)
-  fit_x, fit_y, result = data.fit(
-    x="Controlled variable(s)", y="Signal", data=rabi.data, fit_function=data.fit_function.sineexponentialdecay
-  )
-  sns.lineplot(x=fit_x, y=fit_y, ax=ax)
-
-data.save_figures(filepath="rabi_variation", fig=fig)
+```mermaid
+flowchart TD
+    IOHandler <-- Handle IO operations --> DataLoader;
+    DataLoader <-- Map IO callables --> DataHandler;
+    Qudi[Qudi FitLogic] --> AnalysisLogic;
+    AnalysisLogic -- Inject fit functions --> DataHandler;
+    DataHandler -- Fit data --> Plot;
+    DataHandler -- Structure data --> MeasurementDataclass;
+    MeasurementDataclass -- Plot data --> Plot[JupyterLab Notebook];
+    Plot -- Save plotted data --> DataHandler;
+    style MeasurementDataclass fill: #bbf, stroke: #f66, stroke-width: 2px, color: #fff, stroke-dasharray: 5 5
 ```
 
-#### Example 4: Extract all temperature data, plot and save
-
-```python
-temperature_measurements = data.load_measurements(measurement_str="Temperature")
-
-dft = pd.concat([t.data for t in temperature_measurements.values()])
+## License
 
-fig, ax = plt.subplots()
-sns.lineplot(data=dft, x="Time", y="Temperature", ax=ax)
-data.save_figures(filepath="temperature_monitoring", fig=fig)
-```
+This license of this project is located in the top level folder under `LICENSE`. Some specific files contain their
+individual licenses in the file header docstring.
 
 ## Build
 
 ### Prerequisites
 
 Latest version of:
 
@@ -290,7 +347,8 @@
 + `make pdf` : Converts all notebooks to PDF (requires LaTeX backend)
 + `make html`: Converts all notebooks to HTML
 + `make py`  : Converts all notebooks to Python (can be useful for VCS)
 + `make all` : Sequentially runs all the notebooks in folder
 
 To use the `make` command on Windows you can install [Chocolatey](https://chocolatey.org/install), then
 install make with `choco install make`
+
```

### Comparing `qudi_hira_analysis-1.4.0/pyproject.toml` & `qudi_hira_analysis-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qudi-hira-analysis"
-version = "1.4.0"
+version = "1.4.1"
 repository = "https://github.com/dineshpinto/qudi-hira-analysis"
 homepage = "https://github.com/dineshpinto/qudi-hira-analysis"
 keywords = ["python", "qubit", "analysis", "nv centers", "photon timetrace"]
 description = "A Python toolkit to analzye photon timetrace data from qubit sensors"
 authors = ["dineshpinto <annual.fallout_0z@icloud.com>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `qudi_hira_analysis-1.4.0/qudi_hira_analysis/analysis_logic.py` & `qudi_hira_analysis-1.4.1/qudi_hira_analysis/analysis_logic.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.4.0/qudi_hira_analysis/data_handler.py` & `qudi_hira_analysis-1.4.1/qudi_hira_analysis/data_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,44 +66,36 @@
     ----------
         data_folder: pathlib.Path
             Path to the data folder.
         figure_folder: pathlib.Path
             Path to the figure folder.
         measurement_folder: str or pathlib.Path
             Path to the measurement folder.
-        copy_measurement_folder_structure: bool
-            Replicate the measurement folder structure into the figure folder. (default: True)
 
     Examples
     --------
     Create an instance of the DataHandler class:
 
-    Set up the source data folder, the figure folder and the measurement folder.
-
-    >>> data = DataHandler(
+    >>> dh = DataHandler(
     >>>     data_folder=Path('C:\\'', 'Data'),
     >>>     figure_folder=Path('C:\\'', 'QudiHiraAnalysis'),
     >>>     measurement_folder=Path('20230101_Bakeout'),
     >>> )
     """
 
     def __init__(
             self,
             data_folder: Path,
             figure_folder: Path,
-            measurement_folder: Path,
-            copy_measurement_folder_structure: bool = True
+            measurement_folder: Path = Path(),
     ):
         self.log = logging.getLogger(__name__)
 
         self.data_folder_path = self.__get_data_folder_path(data_folder, measurement_folder)
-        if copy_measurement_folder_structure:
-            self.figure_folder_path = self.__get_figure_folder_path(figure_folder, measurement_folder)
-        else:
-            self.figure_folder_path = figure_folder
+        self.figure_folder_path = self.__get_figure_folder_path(figure_folder, measurement_folder)
 
         super().__init__(base_read_path=self.data_folder_path, base_write_path=self.figure_folder_path)
 
         self.timestamp_format_str = "%Y%m%d-%H%M-%S"
 
     def __get_data_folder_path(self, data_folder: Path, folder_name: Path) -> Path:
         """ Check if folder exists, if not, create it and return absolute folder paths. """
@@ -316,31 +308,31 @@
         Returns
         -------
             measurement_list: dict[str: MeasurementDataclass]
                 A dictionary of dataclasses containing the measurement data.
 
         Examples
         --------
-        `data` is an instance of the `DataHandler` class.
+        `dh` is an instance of the `DataHandler` class.
 
         Load all T1 measurements:
 
-        >>> data.load_measurements(measurement_str="ODMR", qudi=True, pulsed=True)
+        >>> dh.load_measurements(measurement_str="ODMR", pulsed=True)
 
         Load all confocal data:
 
-        >>> data.load_measurements(measurement_str="Confocal", qudi=True)
+        >>> dh.load_measurements(measurement_str="Confocal")
 
         Load all temperature monitoring data:
 
-        >>> data.load_measurements(measurement_str="Temperature", extension=".xls")
+        >>> dh.load_measurements(measurement_str="Temperature")
 
         Load all pressure monitoring data:
 
-        >>> data.load_measurements(measurement_str="Pressure", qudi=True)
+        >>> dh.load_measurements(measurement_str="Pressure")
         """
 
         measurement_str = measurement_str.lower()
         if qudi:
             return self.__load_qudi_measurements_into_dataclass(measurement_str, pulsed=pulsed, extension=".dat")
         else:
             return self.__load_standard_measurements_into_dataclass(measurement_str, extension=extension)
```

### Comparing `qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/antibunchingmethods.py` & `qudi_hira_analysis-1.4.1/qudi_hira_analysis/fitmethods/antibunchingmethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/decaylikemethods.py` & `qudi_hira_analysis-1.4.1/qudi_hira_analysis/fitmethods/decaylikemethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/gaussianlikemethods.py` & `qudi_hira_analysis-1.4.1/qudi_hira_analysis/fitmethods/gaussianlikemethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/generalmethods.py` & `qudi_hira_analysis-1.4.1/qudi_hira_analysis/fitmethods/generalmethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/hyperbolicsaturationmethods.py` & `qudi_hira_analysis-1.4.1/qudi_hira_analysis/fitmethods/hyperbolicsaturationmethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/linearmethods.py` & `qudi_hira_analysis-1.4.1/qudi_hira_analysis/fitmethods/linearmethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/lorentzianlikemethods.py` & `qudi_hira_analysis-1.4.1/qudi_hira_analysis/fitmethods/lorentzianlikemethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/poissonianlikemethods.py` & `qudi_hira_analysis-1.4.1/qudi_hira_analysis/fitmethods/poissonianlikemethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.4.0/qudi_hira_analysis/fitmethods/sinemethods.py` & `qudi_hira_analysis-1.4.1/qudi_hira_analysis/fitmethods/sinemethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.4.0/qudi_hira_analysis/helper_functions.py` & `qudi_hira_analysis-1.4.1/qudi_hira_analysis/helper_functions.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.4.0/qudi_hira_analysis/io_handler.py` & `qudi_hira_analysis-1.4.1/qudi_hira_analysis/io_handler.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.4.0/qudi_hira_analysis/measurement_dataclass.py` & `qudi_hira_analysis-1.4.1/qudi_hira_analysis/measurement_dataclass.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.4.0/qudi_hira_analysis/qudi_fit_logic.py` & `qudi_hira_analysis-1.4.1/qudi_hira_analysis/qudi_fit_logic.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.4.0/PKG-INFO` & `qudi_hira_analysis-1.4.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: qudi-hira-analysis
-Version: 1.4.0
-Summary: A Python toolkit to analzye photon timetrace data from qubit sensors
-Home-page: https://github.com/dineshpinto/qudi-hira-analysis
-License: MIT
-Keywords: python,qubit,analysis,nv centers,photon timetrace
-Author: dineshpinto
-Author-email: annual.fallout_0z@icloud.com
-Requires-Python: >=3.10,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: lmfit (>=1.1.0,<2.0.0)
-Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
-Requires-Dist: numpy (>=1.24.0,<2.0.0)
-Requires-Dist: openpyxl (>=3.0.10,<4.0.0)
-Requires-Dist: pandas (>=2.0.0,<3.0.0)
-Requires-Dist: pyspm (>=0.3.0,<0.4.0)
-Requires-Dist: tqdm (>=4.64.1,<5.0.0)
-Requires-Dist: xlrd (>=2.0.1,<3.0.0)
-Project-URL: Repository, https://github.com/dineshpinto/qudi-hira-analysis
-Description-Content-Type: text/markdown
-
 [![DOI](https://zenodo.org/badge/288670453.svg)](https://zenodo.org/badge/latestdoi/288670453)
 [![Downloads](https://pepy.tech/badge/qudi-hira-analysis)](https://pepy.tech/project/qudi-hira-analysis)
 [![PyPi version](https://img.shields.io/pypi/v/qudi-hira-analysis)](https://pypi.python.org/pypi/qudi-hira-analysis/)
 [![Python 3.10](https://img.shields.io/badge/python-3.10-orange.svg)](https://www.python.org/downloads/release/python-3100//)
 [![Python 3.11](https://img.shields.io/badge/python-3.11-orange.svg)](https://www.python.org/downloads/release/python-3110//)
 
 # Qudi Hira Analysis
@@ -54,67 +29,160 @@
 pip install qudi-hira-analysis
 ```
 
 ## Citation
 
 If you are publishing scientific results, you can cite this work as:  https://doi.org/10.5281/zenodo.7604670
 
-## Schema
+## Examples
 
-The visual structure of the toolkit is shown in the schema below. It largely consists of three portions:
+First set up the `DataHandler` object (henceforth referred to as `dh`) with the correct paths to the data and figure
+folders.
 
-- `IOHandler` assumes a central store of raw data, which is never modified (read-only)
-- `DataHandler` automates the extraction of large amounts of data from the `IOHandler` interface
-- `AnalysisLogic` contains a set of automated fitting routines using `lmfit` internally (built on top of fitting
-  routines from the [qudi](https://github.com/Ulm-IQO/qudi) project)
+Everything revolves around the `dh` object. It is the main interface to the toolkit and is initialized with the
+following required arguments:
 
-This license of this project is located in the top level folder under `LICENSE`. Some specific files contain their
-individual licenses in the file header docstring.
+- `data_folder` is the main folder where all the data is stored, it can be the direct path to the data, or composed of
+  several sub-folders, each containing the data for a specific measurement
+- `figure_folder` is the folder where the output figures will be saved
 
-```mermaid
-flowchart TD;
-    IOHandler<-- Handle all IO operations -->DataLoader;
-    DataLoader<-- Map IO callables to data -->DataHandler;
-    DataHandler-- Structure extracted data -->MeasurementDataclass;
-    MeasurementDataclass-- Plot fitted data --> Plot[Visualize data and add context in JupyterLab];
-    Plot-- Save plotted data --> DataHandler;
-    style MeasurementDataclass fill:#bbf,stroke:#f66,stroke-width:2px,color:#fff,stroke-dasharray: 5 5
+Optional arguments:
+
+- `measurement_folder` is the specific sub-folder in `data_folder` where the data for a specific measurement is stored
+
+```python
+from pathlib import Path
+import matplotlib.pyplot as plt
+import seaborn as sns
+
+from qudi_hira_analysis import DataHandler
+
+dh = DataHandler(
+    data_folder=Path("C:\\", "Data"),
+    figure_folder=Path("C:\\", "QudiHiraAnalysis"),
+    measurement_folder=Path("20230101_NV1")
+)
+```
+
+To load a specific set of measurements from the data folder, use the `dh.load_measurements()` method, which takes the
+following required arguments:
+
+- `measurement_str` is the string that is used to identify the measurement. It is used to filter the data files in the
+  `data_folder` and `measurement_folder` (if specified)
+
+Optional arguments:
+
+- `qudi` is a boolean. If `True`, the data is assumed to be in the format used by Qudi (default: True)
+- `pulsed` is a boolean. If `True`, the data is assumed to be in the format used by Qudi for pulsed measurements (
+  default: False)
+- `extension` is the extension of the data files (default: ".dat")
+
+The `load_measurements` function returns a dictionary containing the measurement data filtered by `measurement_str`.
+
+- The dictionary keys are measurement timestamps in "(year)(month)(day)-(hour)(minute)-(second)" format.
+
+- The dictionary values are `MeasurementDataclass` objects whose schema is shown
+  visually [here](#measurement-dataclass-schema).
+
+### Example 1: Autocorrelation measurements (Antibunching fit)
+
+```python
+autocorrelation_measurements = dh.load_measurements(measurement_str="Autocorrelation")
+
+fig, ax = plt.subplots()
+
+for autocorrelation in autocorrelation_measurements.values():
+    # Plot the data
+    sns.lineplot(data=autocorrelation.data, x="Controlled variable(s)", y="g2(t)", ax=ax)
+    # Fit the data using the antibunching function
+    fit_x, fit_y, result = dh.fit(x="Controlled variable(s)", y="g2(t)", data=autocorrelation.data,
+                                  fit_function=dh.fit_function.antibunching)
+    # Plot the fit
+    sns.lineplot(x=fit_x, y=fit_y, ax=ax)
+
+# Save the figure to the figure folder specified earlier
+dh.save_figures(filepath="autocorrelation_variation", fig=fig)
 ```
 
-### Measurement Dataclass
+### Example 2: ODMR measurements (double Lorentzian 15N fit)
+
+```python
+odmr_measurements = dh.load_measurements(measurement_str="ODMR", pulsed=True)
+
+fig, ax = plt.subplots()
+
+for odmr in odmr_measurements.values():
+    sns.scatterplot(data=odmr.data, x="Controlled variable(Hz)", y="Signal", ax=ax)
+    fit_x, fit_y, result = dh.fit(x="Controlled variable(Hz)", y="Signal", data=odmr.data,
+                                  fit_function=dh.fit_function.lorentzian_double)
+    sns.lineplot(x=fit_x, y=fit_y, ax=ax)
+
+dh.save_figures(filepath="odmr_variation", fig=fig)
+```
+
+### Example 3: Rabi measurements (sine exponential decay fit)
+
+```python
+rabi_measurements = dh.load_measurements(measurement_str="Rabi", pulsed=True)
+
+fig, ax = plt.subplots()
+
+for rabi in rabi_measurements.values():
+    sns.scatterplot(data=rabi.data, x="Controlled variable(s)", y="Signal", ax=ax)
+    fit_x, fit_y, result = dh.fit(x="Controlled variable(s)", y="Signal", data=rabi.data,
+                                  fit_function=dh.fit_function.sineexponentialdecay)
+    sns.lineplot(x=fit_x, y=fit_y, ax=ax)
+
+dh.save_figures(filepath="rabi_variation", fig=fig)
+```
+
+### Example 4: Temperature data
+
+```python
+temperature_measurements = dh.load_measurements(measurement_str="Temperature")
+
+temperature = pd.concat([t.data for t in temperature_measurements.values()])
+
+fig, ax = plt.subplots()
+sns.lineplot(data=temperature, x="Time", y="Temperature", ax=ax)
+dh.save_figures(filepath="temperature_monitoring", fig=fig)
+```
+
+## Measurement Dataclass Schema
 
 ```mermaid
-flowchart LR;
+flowchart LR
     subgraph Standard Data
-        MeasurementDataclass-->filepath1[filepath: Path];
-        MeasurementDataclass-->data1[data: DataFrame];
-        MeasurementDataclass-->params1[params: dict];
-        MeasurementDataclass-->timestamp1[timestamp: datetime];
-        MeasurementDataclass-- analysis --oAnalysisLogic;
+        MeasurementDataclass --o filepath1[filepath: Path];
+        MeasurementDataclass --o data1[data: DataFrame];
+        MeasurementDataclass --o params1[params: dict];
+        MeasurementDataclass --o timestamp1[timestamp: datetime.datetime];
+        MeasurementDataclass --o methods1[get_param_from_filename: Callable];
+        MeasurementDataclass --o methods2[set_datetime_index: Callable];
     end
     subgraph Pulsed Data
-        MeasurementDataclass-- pulsed --oPulsedMeasurementDataclass;
-        PulsedMeasurementDataclass-- measurement --oPulsedMeasurement;
-        PulsedMeasurement--> filepath2[filepath: Path];
-        PulsedMeasurement--> data2[data: DataFrame];
-        PulsedMeasurement--> params2[params: dict];
-        PulsedMeasurementDataclass-- laser_pulses --oLaserPulses; 
-        LaserPulses--> filepath3[filepath: Path];
-        LaserPulses--> data3[data: DataFrame];
-        LaserPulses--> params3[params: dict];
-        PulsedMeasurementDataclass-- timetrace --oRawTimetrace;
-        RawTimetrace--> filepath4[filepath: Path];
-        RawTimetrace--> data4[data: DataFrame];
-        RawTimetrace--> params4[params: dict];
+        MeasurementDataclass -- pulsed --> PulsedMeasurementDataclass;
+        PulsedMeasurementDataclass -- measurement --> PulsedMeasurement;
+        PulsedMeasurement --o filepath2[filepath: Path];
+        PulsedMeasurement --o data2[data: DataFrame];
+        PulsedMeasurement --o params2[params: dict];
+        PulsedMeasurementDataclass -- laser_pulses --> LaserPulses;
+        LaserPulses --o filepath3[filepath: Path];
+        LaserPulses --o data3[data: DataFrame];
+        LaserPulses --o params3[params: dict];
+        PulsedMeasurementDataclass -- timetrace --> RawTimetrace;
+        RawTimetrace --o filepath4[filepath: Path];
+        RawTimetrace --o data4[data: DataFrame];
+        RawTimetrace --o params4[params: dict];
     end
 ```
 
-### Supports common fitting routines
+## Supports common fitting routines
 
-Fit routines included in `AnalysisLogic`
+To get the full list of available fit routines, use the `dh.fit_function` attribute. The fit functions are:
 
 | Dimension | Fit                           |
 |-----------|-------------------------------|
 | 1d        | decayexponential              |
 |           | biexponential                 |
 |           | decayexponentialstretched     |
 |           | gaussian                      |
@@ -132,20 +200,20 @@
 |           | sineexponentialdecay          |
 |           | sinestretchedexponentialdecay |
 |           | sinetriple                    |
 |           | sinetriplewithexpdecay        |
 |           | sinetriplewiththreeexpdecay   |
 | 2d        | twoDgaussian                  |
 
-### Inbuilt measurement tree visualizer
+## Inbuilt measurement tree visualizer
 
 ```ipython
->>> tip_2S6 = DataHandler(data_folder="C:\\Data", figure_folder="C:\\QudiHiraAnalysis",
+>>> data = DataHandler(data_folder="C:\\Data", figure_folder="C:\\QudiHiraAnalysis",
                       measurement_folder="20220621_FR0612-F2-2S6_uhv")
->>> tip_2S6.data_folder_tree()
+>>> data.data_folder_tree()
 
 # Output
 ├── 20211116_NetworkAnalysis_SampleIn_UpperPin.csv
 ├── 20211116_NetworkAnalysis_SampleOut_UpperPin.csv
 ├── 20211116_NetworkAnalysis_TipIn_LowerPin.csv
 ├── 20211116_NetworkAnalysis_TipIn_UpperPin.csv
 ├── 20211116_NetworkAnalysis_TipOut_LowerPin.csv
@@ -157,94 +225,33 @@
 │   ├── C2_TipLowerPin.txt
 │   └── C2_TipUpperPin.txt
 ├── Sample_MW_Pin_comparision.png
 ├── Tip_MW_Pin_comparision.png
 └── Tip_Sample_MW_Pin_comparision.png
 ```
 
-### Automated data extraction
-
-First set up the `DataHandler` object with the correct paths to the data and figure folders.
-
-```python
-from pathlib import Path
-import matplotlib.pyplot as plt
-import seaborn as sns
-
-from qudi_hira_analysis import DataHandler
-
-data = DataHandler(
-  data_folder=Path("C:\\", "Data"), 
-  figure_folder=Path("C:\\", "QudiHiraAnalysis"),
-  measurement_folder=Path("20230101_NV1")
-)
-```
-
-#### Example 1: Extract autocorrelation measurements, fit and save
-
-```python
-autocorrelation_measurements = data.load_measurements(measurement_str="Autocorrelation")
-
-fig, ax = plt.subplots()
-
-for autocorrelation in autocorrelation_measurements.values():
-  sns.lineplot(data=autocorrelation.data, x="Controlled variable(s)", y="g2(t)", ax=ax)
-  fit_x, fit_y, result = data.fit(
-    x="Controlled variable(s)", y="g2(t)", data=autocorrelation.data, fit_function=data.fit_function.antibunching
-  )
-  sns.lineplot(x=fit_x, y=fit_y, ax=ax)
-  
-data.save_figures(filepath="autocorrelation_variation", fig=fig)
-```
-
-#### Example 2: Extract ODMR measurements, fit and save
+## Overall Schema
 
-```python
-odmr_measurements = data.load_measurements(measurement_str="ODMR", pulsed=True)
-
-fig, ax = plt.subplots()
-
-for odmr in odmr_measurements.values():
-  sns.scatterplot(data=odmr.data, x="Controlled variable(Hz)", y="Signal", ax=ax)
-  fit_x, fit_y, result = data.fit(
-    x="Controlled variable(Hz)", y="Signal", data=odmr.data, fit_function=data.fit_function.lorentzian_double
-  )
-  sns.lineplot(x=fit_x, y=fit_y, ax=ax)
-
-data.save_figures(filepath="odmr_variation", fig=fig)
-```
-
-#### Example 3: Extract Rabi measurements, fit and save
-
-```python
-rabi_measurements = data.load_measurements(measurement_str="Rabi", pulsed=True)
-
-fig, ax = plt.subplots()
-
-for rabi in rabi_measurements.values():
-  sns.scatterplot(data=rabi.data, x="Controlled variable(s)", y="Signal", ax=ax)
-  fit_x, fit_y, result = data.fit(
-    x="Controlled variable(s)", y="Signal", data=rabi.data, fit_function=data.fit_function.sineexponentialdecay
-  )
-  sns.lineplot(x=fit_x, y=fit_y, ax=ax)
-
-data.save_figures(filepath="rabi_variation", fig=fig)
+```mermaid
+flowchart TD
+    IOHandler <-- Handle IO operations --> DataLoader;
+    DataLoader <-- Map IO callables --> DataHandler;
+    Qudi[Qudi FitLogic] --> AnalysisLogic;
+    AnalysisLogic -- Inject fit functions --> DataHandler;
+    DataHandler -- Fit data --> Plot;
+    DataHandler -- Structure data --> MeasurementDataclass;
+    MeasurementDataclass -- Plot data --> Plot[JupyterLab Notebook];
+    Plot -- Save plotted data --> DataHandler;
+    style MeasurementDataclass fill: #bbf, stroke: #f66, stroke-width: 2px, color: #fff, stroke-dasharray: 5 5
 ```
 
-#### Example 4: Extract all temperature data, plot and save
-
-```python
-temperature_measurements = data.load_measurements(measurement_str="Temperature")
-
-dft = pd.concat([t.data for t in temperature_measurements.values()])
+## License
 
-fig, ax = plt.subplots()
-sns.lineplot(data=dft, x="Time", y="Temperature", ax=ax)
-data.save_figures(filepath="temperature_monitoring", fig=fig)
-```
+This license of this project is located in the top level folder under `LICENSE`. Some specific files contain their
+individual licenses in the file header docstring.
 
 ## Build
 
 ### Prerequisites
 
 Latest version of:
 
@@ -315,8 +322,7 @@
 + `make pdf` : Converts all notebooks to PDF (requires LaTeX backend)
 + `make html`: Converts all notebooks to HTML
 + `make py`  : Converts all notebooks to Python (can be useful for VCS)
 + `make all` : Sequentially runs all the notebooks in folder
 
 To use the `make` command on Windows you can install [Chocolatey](https://chocolatey.org/install), then
 install make with `choco install make`
-
```

