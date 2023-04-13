# Comparing `tmp/nhssynth-0.2.0.tar.gz` & `tmp/nhssynth-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhssynth-0.2.0.tar", max compression
+gzip compressed data, was "nhssynth-0.2.1.tar", max compression
```

## Comparing `nhssynth-0.2.0.tar` & `nhssynth-0.2.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1068 2023-03-31 11:03:40.629205 nhssynth-0.2.0/LICENSE
--rw-r--r--   0        0        0     6290 2023-04-05 14:58:26.929685 nhssynth-0.2.0/README.md
--rw-r--r--   0        0        0     1360 2023-04-13 14:44:05.536456 nhssynth-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       21 2023-03-21 11:15:21.821516 nhssynth-0.2.0/src/nhssynth/cli/__init__.py
--rw-r--r--   0        0        0     2690 2023-04-12 17:47:54.764686 nhssynth-0.2.0/src/nhssynth/cli/common_arguments.py
--rw-r--r--   0        0        0     8743 2023-04-13 12:22:56.987449 nhssynth-0.2.0/src/nhssynth/cli/config.py
--rw-r--r--   0        0        0     7024 2023-04-13 13:06:51.351173 nhssynth-0.2.0/src/nhssynth/cli/module_arguments.py
--rw-r--r--   0        0        0     6968 2023-04-13 10:55:06.840859 nhssynth-0.2.0/src/nhssynth/cli/module_setup.py
--rw-r--r--   0        0        0     1409 2023-04-13 13:03:16.862839 nhssynth-0.2.0/src/nhssynth/cli/run.py
--rw-r--r--   0        0        0       82 2023-04-04 13:59:35.254031 nhssynth-0.2.0/src/nhssynth/common/__init__.py
--rw-r--r--   0        0        0      292 2023-04-13 15:21:59.569403 nhssynth-0.2.0/src/nhssynth/common/common.py
--rw-r--r--   0        0        0     3339 2023-04-13 09:38:21.025865 nhssynth-0.2.0/src/nhssynth/common/constants.py
--rw-r--r--   0        0        0     2078 2023-04-04 13:59:35.254363 nhssynth-0.2.0/src/nhssynth/common/dicts.py
--rw-r--r--   0        0        0     2953 2023-04-12 15:31:20.079017 nhssynth-0.2.0/src/nhssynth/common/io.py
--rw-r--r--   0        0        0        0 2023-03-09 10:01:33.834460 nhssynth-0.2.0/src/nhssynth/modules/__init__.py
--rw-r--r--   0        0        0       20 2023-03-06 16:05:17.363712 nhssynth-0.2.0/src/nhssynth/modules/dataloader/__init__.py
--rw-r--r--   0        0        0     4082 2023-04-12 15:32:23.986086 nhssynth-0.2.0/src/nhssynth/modules/dataloader/io.py
--rw-r--r--   0        0        0     5253 2023-04-12 15:46:13.535858 nhssynth-0.2.0/src/nhssynth/modules/dataloader/metadata.py
--rw-r--r--   0        0        0    20155 2023-04-12 15:46:09.143287 nhssynth-0.2.0/src/nhssynth/modules/dataloader/metatransformer.py
--rw-r--r--   0        0        0     1596 2023-04-13 12:33:38.185534 nhssynth-0.2.0/src/nhssynth/modules/dataloader/run.py
--rw-r--r--   0        0        0       21 2023-03-07 10:58:04.573024 nhssynth-0.2.0/src/nhssynth/modules/evaluation/__init__.py
--rw-r--r--   0        0        0    13625 2023-04-13 15:23:11.578297 nhssynth-0.2.0/src/nhssynth/modules/evaluation/full_report.py
--rw-r--r--   0        0        0     2644 2023-04-13 10:57:28.285918 nhssynth-0.2.0/src/nhssynth/modules/evaluation/io.py
--rw-r--r--   0        0        0     3031 2023-04-11 16:04:10.935343 nhssynth-0.2.0/src/nhssynth/modules/evaluation/metrics.py
--rw-r--r--   0        0        0     1856 2023-04-13 15:24:02.908325 nhssynth-0.2.0/src/nhssynth/modules/evaluation/run.py
--rw-r--r--   0        0        0     8488 2023-04-13 12:51:55.098685 nhssynth-0.2.0/src/nhssynth/modules/model/DPVAE.py
--rw-r--r--   0        0        0       21 2023-03-07 10:57:59.963528 nhssynth-0.2.0/src/nhssynth/modules/model/__init__.py
--rw-r--r--   0        0        0     3092 2023-04-12 15:33:11.172294 nhssynth-0.2.0/src/nhssynth/modules/model/io.py
--rw-r--r--   0        0        0     3510 2023-04-13 12:45:23.368814 nhssynth-0.2.0/src/nhssynth/modules/model/run.py
--rw-r--r--   0        0        0       21 2023-03-07 10:58:07.632275 nhssynth-0.2.0/src/nhssynth/modules/plotting/__init__.py
--rw-r--r--   0        0        0     2611 2023-04-13 11:19:38.014249 nhssynth-0.2.0/src/nhssynth/modules/plotting/io.py
--rw-r--r--   0        0        0     6510 2023-04-13 12:13:35.989347 nhssynth-0.2.0/src/nhssynth/modules/plotting/plots.py
--rw-r--r--   0        0        0      727 2023-04-13 12:33:18.866696 nhssynth-0.2.0/src/nhssynth/modules/plotting/run.py
--rw-r--r--   0        0        0       21 2023-03-07 10:58:13.024183 nhssynth-0.2.0/src/nhssynth/modules/structure/__init__.py
--rw-r--r--   0        0        0       85 2023-03-07 10:58:26.227434 nhssynth-0.2.0/src/nhssynth/modules/structure/run.py
--rw-r--r--   0        0        0     7605 1970-01-01 00:00:00.000000 nhssynth-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-03-31 11:03:40.629205 nhssynth-0.2.1/LICENSE
+-rw-r--r--   0        0        0     6290 2023-04-05 14:58:26.929685 nhssynth-0.2.1/README.md
+-rw-r--r--   0        0        0     1438 2023-04-13 17:40:46.684939 nhssynth-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-03-21 11:15:21.821516 nhssynth-0.2.1/src/nhssynth/cli/__init__.py
+-rw-r--r--   0        0        0     2690 2023-04-12 17:47:54.764686 nhssynth-0.2.1/src/nhssynth/cli/common_arguments.py
+-rw-r--r--   0        0        0     8743 2023-04-13 12:22:56.987449 nhssynth-0.2.1/src/nhssynth/cli/config.py
+-rw-r--r--   0        0        0     7024 2023-04-13 13:06:51.351173 nhssynth-0.2.1/src/nhssynth/cli/module_arguments.py
+-rw-r--r--   0        0        0     6968 2023-04-13 10:55:06.840859 nhssynth-0.2.1/src/nhssynth/cli/module_setup.py
+-rw-r--r--   0        0        0     1409 2023-04-13 13:03:16.862839 nhssynth-0.2.1/src/nhssynth/cli/run.py
+-rw-r--r--   0        0        0       82 2023-04-04 13:59:35.254031 nhssynth-0.2.1/src/nhssynth/common/__init__.py
+-rw-r--r--   0        0        0      292 2023-04-13 15:21:59.569403 nhssynth-0.2.1/src/nhssynth/common/common.py
+-rw-r--r--   0        0        0     3339 2023-04-13 09:38:21.025865 nhssynth-0.2.1/src/nhssynth/common/constants.py
+-rw-r--r--   0        0        0     2078 2023-04-04 13:59:35.254363 nhssynth-0.2.1/src/nhssynth/common/dicts.py
+-rw-r--r--   0        0        0     2953 2023-04-12 15:31:20.079017 nhssynth-0.2.1/src/nhssynth/common/io.py
+-rw-r--r--   0        0        0        0 2023-03-09 10:01:33.834460 nhssynth-0.2.1/src/nhssynth/modules/__init__.py
+-rw-r--r--   0        0        0       20 2023-03-06 16:05:17.363712 nhssynth-0.2.1/src/nhssynth/modules/dataloader/__init__.py
+-rw-r--r--   0        0        0     4082 2023-04-12 15:32:23.986086 nhssynth-0.2.1/src/nhssynth/modules/dataloader/io.py
+-rw-r--r--   0        0        0     5253 2023-04-12 15:46:13.535858 nhssynth-0.2.1/src/nhssynth/modules/dataloader/metadata.py
+-rw-r--r--   0        0        0    20232 2023-04-13 16:21:20.147258 nhssynth-0.2.1/src/nhssynth/modules/dataloader/metatransformer.py
+-rw-r--r--   0        0        0     1596 2023-04-13 12:33:38.185534 nhssynth-0.2.1/src/nhssynth/modules/dataloader/run.py
+-rw-r--r--   0        0        0       21 2023-03-07 10:58:04.573024 nhssynth-0.2.1/src/nhssynth/modules/evaluation/__init__.py
+-rw-r--r--   0        0        0    14078 2023-04-13 17:25:24.470481 nhssynth-0.2.1/src/nhssynth/modules/evaluation/full_report.py
+-rw-r--r--   0        0        0     2644 2023-04-13 10:57:28.285918 nhssynth-0.2.1/src/nhssynth/modules/evaluation/io.py
+-rw-r--r--   0        0        0     3031 2023-04-11 16:04:10.935343 nhssynth-0.2.1/src/nhssynth/modules/evaluation/metrics.py
+-rw-r--r--   0        0        0     1856 2023-04-13 15:24:02.908325 nhssynth-0.2.1/src/nhssynth/modules/evaluation/run.py
+-rw-r--r--   0        0        0     8614 2023-04-13 16:21:55.328798 nhssynth-0.2.1/src/nhssynth/modules/model/DPVAE.py
+-rw-r--r--   0        0        0       21 2023-03-07 10:57:59.963528 nhssynth-0.2.1/src/nhssynth/modules/model/__init__.py
+-rw-r--r--   0        0        0     3092 2023-04-12 15:33:11.172294 nhssynth-0.2.1/src/nhssynth/modules/model/io.py
+-rw-r--r--   0        0        0     3510 2023-04-13 16:21:44.533892 nhssynth-0.2.1/src/nhssynth/modules/model/run.py
+-rw-r--r--   0        0        0       21 2023-03-07 10:58:07.632275 nhssynth-0.2.1/src/nhssynth/modules/plotting/__init__.py
+-rw-r--r--   0        0        0     2611 2023-04-13 11:19:38.014249 nhssynth-0.2.1/src/nhssynth/modules/plotting/io.py
+-rw-r--r--   0        0        0     6510 2023-04-13 12:13:35.989347 nhssynth-0.2.1/src/nhssynth/modules/plotting/plots.py
+-rw-r--r--   0        0        0      727 2023-04-13 12:33:18.866696 nhssynth-0.2.1/src/nhssynth/modules/plotting/run.py
+-rw-r--r--   0        0        0       21 2023-03-07 10:58:13.024183 nhssynth-0.2.1/src/nhssynth/modules/structure/__init__.py
+-rw-r--r--   0        0        0       85 2023-03-07 10:58:26.227434 nhssynth-0.2.1/src/nhssynth/modules/structure/run.py
+-rw-r--r--   0        0        0     7605 1970-01-01 00:00:00.000000 nhssynth-0.2.1/PKG-INFO
```

### Comparing `nhssynth-0.2.0/LICENSE` & `nhssynth-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nhssynth-0.2.0/README.md` & `nhssynth-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nhssynth-0.2.0/pyproject.toml` & `nhssynth-0.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nhssynth"
-version = "0.2.0"
+version = "0.2.1"
 description = "Synthetic data generation pipeline leveraging a Differentially Private Variational Auto Encoder assessed using a variety of metrics"
 authors = ["HarrisonWilde <harrisondwilde@outlook.com>"]
 maintainers = ["NHSE TDAU <england.tdau@nhs.net>"]
 license = "MIT"
 readme = ["README.md"]
 repository = "https://github.com/nhsx/NHSSynth"
 keywords = ["synthetic data", "privacy", "fairness", "machine learning"]
@@ -40,10 +40,15 @@
 mkdocs-material = "^9.1.4"
 mkdocs-gen-files = "^0.4.0"
 mkdocs-literate-nav = "^0.6.0"
 mkdocs-section-index = "^0.3.5"
 mkdocs-git-revision-date-localized-plugin = "^1.2.0"
 pymdown-extensions = "^9.10"
 
+
+[tool.poetry.group.dev.dependencies]
+jupyter = "^1.0.0"
+notebook = "^6.5.4"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nhssynth-0.2.0/src/nhssynth/cli/common_arguments.py` & `nhssynth-0.2.1/src/nhssynth/cli/common_arguments.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.2.0/src/nhssynth/cli/config.py` & `nhssynth-0.2.1/src/nhssynth/cli/config.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.2.0/src/nhssynth/cli/module_arguments.py` & `nhssynth-0.2.1/src/nhssynth/cli/module_arguments.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.2.0/src/nhssynth/cli/module_setup.py` & `nhssynth-0.2.1/src/nhssynth/cli/module_setup.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.2.0/src/nhssynth/cli/run.py` & `nhssynth-0.2.1/src/nhssynth/cli/run.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.2.0/src/nhssynth/common/constants.py` & `nhssynth-0.2.1/src/nhssynth/common/constants.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.2.0/src/nhssynth/common/dicts.py` & `nhssynth-0.2.1/src/nhssynth/common/dicts.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.2.0/src/nhssynth/common/io.py` & `nhssynth-0.2.1/src/nhssynth/common/io.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.2.0/src/nhssynth/modules/dataloader/io.py` & `nhssynth-0.2.1/src/nhssynth/modules/dataloader/io.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.2.0/src/nhssynth/modules/dataloader/metadata.py` & `nhssynth-0.2.1/src/nhssynth/modules/dataloader/metadata.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.2.0/src/nhssynth/modules/dataloader/metatransformer.py` & `nhssynth-0.2.1/src/nhssynth/modules/dataloader/metatransformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -324,17 +324,17 @@
         """
         if not self.assembled_metadata:
             self.assembled_metadata = self.assemble()
         onehot_idxs = []
         single_idxs = []
         for cn, cd in self.assembled_metadata.items():
             if cd["transformer"].get("name") == "OneHotEncoder":
-                onehot_idxs.append(data.columns.get_indexer(data.filter(like=cn).columns).tolist())
+                onehot_idxs.append(data.columns.get_indexer(data.filter(like=cn + ".value").columns).tolist())
             elif cd["transformer"].get("name") == "ClusterBasedNormalizer":
-                onehot_idxs.append(data.columns.get_indexer(data.filter(like=cn + ".component").columns).tolist())
+                onehot_idxs.append(data.columns.get_indexer(data.filter(like=cn + ".component.value").columns).tolist())
                 single_idxs.append(data.columns.get_loc(cn + ".normalized"))
             elif cd["transformer"].get("name") != "RegexGenerator":
                 single_idxs.append(data.columns.get_loc(cn))
         return onehot_idxs, single_idxs
 
     def apply(self, data: pd.DataFrame) -> pd.DataFrame:
         """
@@ -365,29 +365,29 @@
                 - transformer: A dictionary containing information about the transformer used for the column (if any). The dictionary has the following keys:
                     - name: The name of the transformer.
                     - Any other properties of the transformer that we want to record in output.
 
         Raises:
             ValueError: If the metadata has not yet been assembled.
         """
-        if not self.assembled_metadata:
+        if not hasattr(self, "assembled_metadata"):
             raise ValueError("Metadata has not yet been assembled. Call `my.apply(data)` (or `mt.assemble()`) first.")
         return self.assembled_metadata
 
     def get_sdtypes(self) -> dict[str, dict[str, dict[str, str]]]:
         """
         Returns the sdtypes extracted from the assembled metadata for SDMetrics.
 
         Returns:
             A dictionary mapping column names to sdtypes.
 
         Raises:
             ValueError: If the metadata has not yet been assembled.
         """
-        if not self.assembled_metadata:
+        if not hasattr(self, "assembled_metadata"):
             raise ValueError("Metadata has not yet been assembled. Call `my.apply(data)` (or `mt.assemble()`) first.")
         return get_sdtypes(self.assembled_metadata)
 
     def get_onehots_and_singles(self) -> tuple[list[list[int]], list[int]]:
         """
         Get the values of the MetaTransformer's `onehots` and `singles` attributes.
 
@@ -395,15 +395,15 @@
             A pair of lists:
                 - One-hotted column index groups (i.e. one inner list with all corresponding indices per categorical variable)
                 - Non-one-hotted column indices
 
         Raises:
             ValueError: If `self.onehots` and `self.singles` have yet to be counted.
         """
-        if not self.onehots or not self.singles:
+        if not hasattr(self, "onehots") or not hasattr(self, "singles"):
             raise ValueError(
                 "Some metadata is missing. Call `mt.apply(data)` first (or `mt.count_onehots_and_singles(data)`)."
             )
         return self.onehots, self.singles
 
     def inverse_apply(self, data: pd.DataFrame) -> pd.DataFrame:
         """
@@ -414,15 +414,15 @@
 
         Returns:
             The original data.
 
         Raises:
             ValueError: If the metatransformer has not yet been instantiated.
         """
-        if not self.metatransformer:
+        if not hasattr(self, "metatransformer"):
             raise ValueError(
                 "The metatransformer has not yet been instantiated. Call `mt.apply(data)` first (or `mt.instantiate(data)`)."
             )
         for transformer in self.component_transformer.values():
             data = transformer.reverse_transform(data)
         if self.sdv_workflow:
             return self.metatransformer._data_processor.reverse_transform(data)
```

### Comparing `nhssynth-0.2.0/src/nhssynth/modules/dataloader/run.py` & `nhssynth-0.2.1/src/nhssynth/modules/dataloader/run.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.2.0/src/nhssynth/modules/evaluation/full_report.py` & `nhssynth-0.2.1/src/nhssynth/modules/evaluation/full_report.py`

 * *Files 6% similar despite different names*

```diff
@@ -198,14 +198,17 @@
         elif property_name == "Synthesis":
             fig = get_synthesis_plot(score_breakdowns.get("NewRowSynthesis", {}))
             fig.show()
 
         elif property_name == "Detection":
             print("WARNING: Detection plots not currently implemented.")
 
+        elif property_name == "Divergence":
+            print("WARNING: Divergence plots not currently implemented.")
+
         else:
             raise ValueError(f"Property name `{property_name}` is not recognized / supported.")
 
     def get_details(self, property_name):
         """Return the details for each score for the given property name.
 
         Args:
@@ -218,22 +221,31 @@
         """
         columns = []
         metrics = []
         scores = []
         errors = []
         details = pd.DataFrame()
 
-        if property_name in SDV_DETECTION_METRIC_CHOICES:
+        if property_name == "Detection":
             for metric in self._metrics[property_name]:
-                for column, score_breakdown in self._metric_results[metric.__name__].items():
-                    print(metric)
-                    print(column)
-                    print(score_breakdown)
+                metric_results = self._metric_results[metric.__name__]
+                if "score" in metric_results and pd.isna(metric_results["score"]):
+                    continue
+                metrics.append(metric.__name__)
+                scores.append(metric_results.get("score", np.nan))
+                errors.append(metric_results.get("error", np.nan))
+
+            details = pd.DataFrame(
+                {
+                    "Metric": metrics,
+                    "Overall Score": scores,
+                }
+            )
 
-        elif property_name in SDV_COLUMN_SHAPE_METRIC_CHOICES:
+        elif property_name == "Column Shape":
             for metric in self._metrics[property_name]:
                 for column, score_breakdown in self._metric_results[metric.__name__].items():
                     if "score" in score_breakdown and pd.isna(score_breakdown["score"]):
                         continue
 
                     columns.append(column)
                     metrics.append(metric.__name__)
@@ -244,38 +256,39 @@
                 {
                     "Column": columns,
                     "Metric": metrics,
                     "Overall Score": scores,
                 }
             )
 
-        elif property_name in SDV_COLUMN_SIMILARITY_METRIC_CHOICES:
+        elif property_name == "Column Similarity" or property_name == "Divergence":
             real_scores = []
             synthetic_scores = []
             for metric in self._metrics[property_name]:
                 for column_pair, score_breakdown in self._metric_results[metric.__name__].items():
                     columns.append(column_pair)
                     metrics.append(metric.__name__)
                     scores.append(score_breakdown.get("score", np.nan))
-                    real_scores.append(score_breakdown.get("real", np.nan))
-                    synthetic_scores.append(score_breakdown.get("synthetic", np.nan))
+                    if property_name == "Column Similarity":
+                        real_scores.append(score_breakdown.get("real", np.nan))
+                        synthetic_scores.append(score_breakdown.get("synthetic", np.nan))
                     errors.append(score_breakdown.get("error", np.nan))
 
             details = pd.DataFrame(
                 {
                     "Column 1": [col1 for col1, _ in columns],
                     "Column 2": [col2 for _, col2 in columns],
                     "Metric": metrics,
                     "Overall Score": scores,
                     "Real Correlation": real_scores,
                     "Synthetic Correlation": synthetic_scores,
                 }
             )
 
-        elif property_name in SDV_SYNTHESIS_METRIC_CHOICES + SDV_DETECTION_METRIC_CHOICES:
+        elif property_name == "Synthesis":
             metric_name = self._metrics[property_name][0].__name__
             metric_result = self._metric_results[metric_name]
             details = pd.DataFrame(
                 {
                     "Metric": [metric_name],
                     "Overall Score": [metric_result.get("score", np.nan)],
                     "Num Matched Rows": [metric_result.get("num_matched_rows", np.nan)],
```

### Comparing `nhssynth-0.2.0/src/nhssynth/modules/evaluation/io.py` & `nhssynth-0.2.1/src/nhssynth/modules/evaluation/io.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.2.0/src/nhssynth/modules/evaluation/metrics.py` & `nhssynth-0.2.1/src/nhssynth/modules/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.2.0/src/nhssynth/modules/evaluation/run.py` & `nhssynth-0.2.1/src/nhssynth/modules/evaluation/run.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.2.0/src/nhssynth/modules/model/DPVAE.py` & `nhssynth-0.2.1/src/nhssynth/modules/model/DPVAE.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,18 @@
                 self.optimizer.zero_grad()
                 losses = self.loss(Y_subset.to(self.encoder.device))
                 losses["ELBO"].backward()
                 self.optimizer.step()
 
                 for key in metrics.keys():
                     if key in losses:
-                        metrics[key][-1] += losses[key].item()
+                        if losses[key]:
+                            metrics[key][-1] += losses[key].item()
+                        else:
+                            metrics[key][-1] += 0.0
 
             for key, stats_bar in stats_bars.items():
                 if key == "Privacy" and privacy_engine is not None:
                     epsilon_e = self.privacy_engine.get_privacy_spent()
                     # epsilon_e = self.privacy_engine.accountant.get_epsilon()
                     stats_bar.set_description_str(
                         f"{(key + ':').ljust(max_length)}  \u03B5 = {epsilon_e[0]:.2f}\tbest \u03B1 = {epsilon_e[1]:.2f}"
```

### Comparing `nhssynth-0.2.0/src/nhssynth/modules/model/io.py` & `nhssynth-0.2.1/src/nhssynth/modules/model/io.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.2.0/src/nhssynth/modules/model/run.py` & `nhssynth-0.2.1/src/nhssynth/modules/model/run.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.2.0/src/nhssynth/modules/plotting/io.py` & `nhssynth-0.2.1/src/nhssynth/modules/plotting/io.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.2.0/src/nhssynth/modules/plotting/plots.py` & `nhssynth-0.2.1/src/nhssynth/modules/plotting/plots.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.2.0/src/nhssynth/modules/plotting/run.py` & `nhssynth-0.2.1/src/nhssynth/modules/plotting/run.py`

 * *Files identical despite different names*

### Comparing `nhssynth-0.2.0/PKG-INFO` & `nhssynth-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nhssynth
-Version: 0.2.0
+Version: 0.2.1
 Summary: Synthetic data generation pipeline leveraging a Differentially Private Variational Auto Encoder assessed using a variety of metrics
 Home-page: https://github.com/nhsx/NHSSynth
 License: MIT
 Keywords: synthetic data,privacy,fairness,machine learning
 Author: HarrisonWilde
 Author-email: harrisondwilde@outlook.com
 Maintainer: NHSE TDAU
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nhssynth Version: 0.2.0 Summary: Synthetic data
+Metadata-Version: 2.1 Name: nhssynth Version: 0.2.1 Summary: Synthetic data
 generation pipeline leveraging a Differentially Private Variational Auto
 Encoder assessed using a variety of metrics Home-page: https://github.com/nhsx/
 NHSSynth License: MIT Keywords: synthetic data,privacy,fairness,machine
 learning Author: HarrisonWilde Author-email: harrisondwilde@outlook.com
 Maintainer: NHSE TDAU Maintainer-email: england.tdau@nhs.net Requires-Python:
 >=3.9,<3.11 Classifier: Development Status :: 3 - Alpha Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
```

