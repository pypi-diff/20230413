# Comparing `tmp/vegafusion-1.2.0.tar.gz` & `tmp/vegafusion-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vegafusion-1.2.0.tar", last modified: Tue Apr 11 20:22:09 2023, max compression
+gzip compressed data, was "vegafusion-1.2.1.tar", last modified: Thu Apr 13 12:05:12 2023, max compression
```

## Comparing `vegafusion-1.2.0.tar` & `vegafusion-1.2.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:22:09.095437 vegafusion-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-11 20:21:07.000000 vegafusion-1.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-11 20:22:09.095437 vegafusion-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-11 20:21:07.000000 vegafusion-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-11 20:21:07.000000 vegafusion-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-11 20:22:09.095437 vegafusion-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 20:21:07.000000 vegafusion-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:22:09.091437 vegafusion-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-11 20:21:07.000000 vegafusion-1.2.0/tests/test_conext_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    18632 2023-04-11 20:21:07.000000 vegafusion-1.2.0/tests/test_input_utc.py
--rw-r--r--   0 runner    (1001) docker     (123)    32055 2023-04-11 20:21:07.000000 vegafusion-1.2.0/tests/test_pretransform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-04-11 20:21:07.000000 vegafusion-1.2.0/tests/test_pretransform_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-11 20:21:07.000000 vegafusion-1.2.0/tests/test_row_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-11 20:21:07.000000 vegafusion-1.2.0/tests/test_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-04-11 20:21:07.000000 vegafusion-1.2.0/tests/test_transformed_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-11 20:21:07.000000 vegafusion-1.2.0/tests/test_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:22:09.095437 vegafusion-1.2.0/vegafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-11 20:21:07.000000 vegafusion-1.2.0/vegafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 20:21:07.000000 vegafusion-1.2.0/vegafusion/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-11 20:21:07.000000 vegafusion-1.2.0/vegafusion/compilers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:22:09.095437 vegafusion-1.2.0/vegafusion/connection/
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-04-11 20:21:07.000000 vegafusion-1.2.0/vegafusion/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12895 2023-04-11 20:21:07.000000 vegafusion-1.2.0/vegafusion/connection/duckdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-11 20:21:07.000000 vegafusion-1.2.0/vegafusion/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-11 20:21:07.000000 vegafusion-1.2.0/vegafusion/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-11 20:21:07.000000 vegafusion-1.2.0/vegafusion/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-11 20:21:07.000000 vegafusion-1.2.0/vegafusion/local_tz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-11 20:21:07.000000 vegafusion-1.2.0/vegafusion/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20434 2023-04-11 20:21:07.000000 vegafusion-1.2.0/vegafusion/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-04-11 20:21:07.000000 vegafusion-1.2.0/vegafusion/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-04-11 20:21:07.000000 vegafusion-1.2.0/vegafusion/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-11 20:21:07.000000 vegafusion-1.2.0/vegafusion/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:22:09.095437 vegafusion-1.2.0/vegafusion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-11 20:22:09.000000 vegafusion-1.2.0/vegafusion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-11 20:22:09.000000 vegafusion-1.2.0/vegafusion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 20:22:09.000000 vegafusion-1.2.0/vegafusion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-11 20:22:09.000000 vegafusion-1.2.0/vegafusion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-11 20:22:09.000000 vegafusion-1.2.0/vegafusion.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:05:12.409984 vegafusion-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-13 12:03:45.000000 vegafusion-1.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-13 12:05:12.409984 vegafusion-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-13 12:03:45.000000 vegafusion-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-13 12:03:45.000000 vegafusion-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-13 12:05:12.409984 vegafusion-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 12:03:45.000000 vegafusion-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:05:12.409984 vegafusion-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-13 12:03:45.000000 vegafusion-1.2.1/tests/test_conext_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18632 2023-04-13 12:03:45.000000 vegafusion-1.2.1/tests/test_input_utc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36521 2023-04-13 12:03:45.000000 vegafusion-1.2.1/tests/test_pretransform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-04-13 12:03:45.000000 vegafusion-1.2.1/tests/test_pretransform_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-13 12:03:45.000000 vegafusion-1.2.1/tests/test_row_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-13 12:03:45.000000 vegafusion-1.2.1/tests/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-04-13 12:03:45.000000 vegafusion-1.2.1/tests/test_transformed_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-13 12:03:45.000000 vegafusion-1.2.1/tests/test_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:05:12.409984 vegafusion-1.2.1/vegafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-13 12:03:45.000000 vegafusion-1.2.1/vegafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 12:03:45.000000 vegafusion-1.2.1/vegafusion/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-13 12:03:45.000000 vegafusion-1.2.1/vegafusion/compilers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:05:12.409984 vegafusion-1.2.1/vegafusion/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-04-13 12:03:45.000000 vegafusion-1.2.1/vegafusion/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12904 2023-04-13 12:03:45.000000 vegafusion-1.2.1/vegafusion/connection/duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-13 12:03:45.000000 vegafusion-1.2.1/vegafusion/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-13 12:03:45.000000 vegafusion-1.2.1/vegafusion/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-13 12:03:45.000000 vegafusion-1.2.1/vegafusion/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-13 12:03:45.000000 vegafusion-1.2.1/vegafusion/local_tz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-13 12:03:45.000000 vegafusion-1.2.1/vegafusion/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20434 2023-04-13 12:03:45.000000 vegafusion-1.2.1/vegafusion/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-04-13 12:03:45.000000 vegafusion-1.2.1/vegafusion/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-04-13 12:03:45.000000 vegafusion-1.2.1/vegafusion/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-13 12:03:45.000000 vegafusion-1.2.1/vegafusion/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 12:05:12.409984 vegafusion-1.2.1/vegafusion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-13 12:05:12.000000 vegafusion-1.2.1/vegafusion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-13 12:05:12.000000 vegafusion-1.2.1/vegafusion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 12:05:12.000000 vegafusion-1.2.1/vegafusion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 12:05:12.000000 vegafusion-1.2.1/vegafusion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 12:05:12.000000 vegafusion-1.2.1/vegafusion.egg-info/top_level.txt
```

### Comparing `vegafusion-1.2.0/LICENSE.txt` & `vegafusion-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.0/PKG-INFO` & `vegafusion-1.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vegafusion
-Version: 1.2.0
+Version: 1.2.1
 Summary: Core tools for using VegaFusion from Python
 License: BSD-3-Clause
 Keywords: vega,altair,vegafusion,arrow
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vegafusion-1.2.0/README.md` & `vegafusion-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.0/setup.cfg` & `vegafusion-1.2.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [bdist_wheel]
 universal = 0
 
 [metadata]
 name = vegafusion
 description = Core tools for using VegaFusion from Python
-version = 1.2.0
+version = 1.2.1
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = vega, altair, vegafusion, arrow
 license = BSD-3-Clause
 license_file = LICENSE.txt
 python = "^3.7"
 homepage = "https://vegafusion.io"
@@ -30,14 +30,14 @@
 	altair>=4.2.0
 	pyarrow>=5
 	pandas
 	psutil
 
 [options.extras_require]
 embed = 
-	vegafusion-python-embed==1.2.0
+	vegafusion-python-embed==1.2.1
 	vl-convert-python>=0.7.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `vegafusion-1.2.0/tests/test_conext_manager.py` & `vegafusion-1.2.1/tests/test_conext_manager.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.0/tests/test_input_utc.py` & `vegafusion-1.2.1/tests/test_input_utc.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.0/tests/test_pretransform.py` & `vegafusion-1.2.1/tests/test_pretransform.py`

 * *Files 4% similar despite different names*

```diff
@@ -799,14 +799,190 @@
     "range": {"ramp": {"scheme": "yellowgreenblue"}},
     "axis": {"domain": false}
   }
 }
     """)
 
 
+def date32_timeunit_spec():
+    return json.loads(r"""
+{
+  "$schema": "https://vega.github.io/schema/vega/v5.json",
+  "autosize": {
+    "type": "fit",
+    "contains": "padding"
+  },
+  "background": "white",
+  "padding": 5,
+  "style": "cell",
+  "data": [
+    {
+      "name": "dataframe",
+      "url": "vegafusion+dataset://dataframe"
+    },
+    {
+      "name": "data_0",
+      "source": "dataframe",
+      "transform": [
+        {
+          "type": "filter",
+          "expr": "isValid(datum[\"GO_LIVE_MONTH\"])"
+        },
+        {
+          "field": "GO_LIVE_MONTH",
+          "type": "timeunit",
+          "units": [
+            "year",
+            "month"
+          ],
+          "as": [
+            "go_live_start",
+            "go_live_end"
+          ]
+        },
+        {
+          "type": "stack",
+          "groupby": [
+            "go_live_start"
+          ],
+          "field": "PERCENT_GO_LIVES",
+          "sort": {
+            "field": [],
+            "order": []
+          },
+          "as": [
+            "percent_go_lives_start",
+            "percent_go_lives_end"
+          ],
+          "offset": "normalize"
+        },
+        {
+          "type": "formula",
+          "expr": "datum['percent_go_lives_end']-datum['percent_go_lives_start']",
+          "as": "percent_go_lives_delta"
+        }
+      ]
+    },
+    {
+      "name": "data_1",
+      "source": "data_0",
+      "transform": [
+        {
+          "field": "go_live_start",
+          "type": "timeunit",
+          "units": [
+            "year",
+            "month"
+          ],
+          "as": [
+            "go_live_start_start",
+            "go_live_start_end"
+          ]
+        },
+        {
+          "type": "filter",
+          "expr": "(isDate(datum[\"go_live_start_start\"]) || (isValid(datum[\"go_live_start_start\"]) && isFinite(+datum[\"go_live_start_start\"]))) && isValid(datum[\"percent_go_lives_start\"]) && isFinite(+datum[\"percent_go_lives_start\"])"
+        }
+      ]
+    }
+  ],
+  "marks": [
+    {
+      "name": "layer_0_layer_0_layer_0_marks",
+      "type": "rect",
+      "clip": true,
+      "style": [
+        "bar"
+      ],
+      "from": {
+        "data": "data_1"
+      },
+      "encode": {
+        "update": {
+          "fill": {
+            "value": "#ff4c00"
+          },
+          "opacity": {
+            "value": 1
+          },
+          "ariaRoleDescription": {
+            "value": "bar"
+          },
+          "x": {
+            "scale": "x",
+            "field": "go_live_start_start"
+          },
+          "x2": {
+            "scale": "x",
+            "field": "go_live_end",
+            "offset": -1
+          },
+          "y": {
+            "scale": "y",
+            "field": "percent_go_lives_start"
+          },
+          "y2": {
+            "scale": "y",
+            "field": "percent_go_lives_end"
+          }
+        }
+      }
+    }
+  ],
+  "scales": [
+    {
+      "name": "x",
+      "type": "time",
+      "domain": {
+        "fields": [
+          {
+            "data": "data_1",
+            "field": "go_live_start_start"
+          },
+          {
+            "data": "data_1",
+            "field": "go_live_end"
+          }
+        ]
+      },
+      "range": [
+        0,
+        {
+          "signal": "width"
+        }
+      ]
+    },
+    {
+      "name": "y",
+      "type": "linear",
+      "domain": {
+        "fields": [
+          {
+            "data": "data_1",
+            "field": "percent_go_lives_start"
+          },
+          {
+            "data": "data_1",
+            "field": "percent_go_lives_end"
+          }
+        ]
+      },
+      "range": [
+        {
+          "signal": "height"
+        },
+        0
+      ],
+      "nice": true,
+      "zero": true
+    }
+  ]
+}
+
+""")
 def test_pre_transform_multi_partition():
     n = 4050
     order_items = pd.DataFrame({
         "menu_item": [0] * n + [1] * n
     })
 
     vega_spec = order_items_spec()
@@ -917,14 +1093,39 @@
     assert list(output_ds.date_col) == [
         pd.Timestamp('2022-01-01 00:00:00-0500', tz='America/New_York'),
         pd.Timestamp('2022-01-02 00:00:00-0500', tz='America/New_York'),
         pd.Timestamp('2022-01-03 00:00:00-0500', tz='America/New_York')
     ]
 
 
+def test_date32_in_timeunit_duckdb_crash():
+    try:
+        # Set this as the active connection
+        vf.runtime.set_connection("duckdb")
+
+        # order_items includes a table://order_items data url
+        vega_spec = date32_timeunit_spec()
+        dataframe = pd.DataFrame({
+            "GO_LIVE_MONTH": [date(2021, 1, 1), date(2021, 2, 1)],
+            "PERCENT_GO_LIVES": [0.2, 0.3],
+        })
+
+        datasets, warnings = vf.runtime.pre_transform_datasets(
+            vega_spec,
+            ["data_1"],
+            "UTC",
+            inline_datasets=dict(dataframe=dataframe)
+        )
+        assert len(warnings) == 0
+        assert len(datasets) == 1
+        assert len(datasets[0]) == 2
+    finally:
+        vf.runtime.set_connection("datafusion")
+
+
 def test_period_in_column_name():
     df_period = pd.DataFrame([[1, 2]], columns=['normal', 'a.b'])
     spec = period_in_col_name_spec()
     datasets, warnings = vf.runtime.pre_transform_datasets(spec, ["data_0"], "UTC", inline_datasets=dict(
         df_period=df_period
     ))
     assert len(warnings) == 0
```

### Comparing `vegafusion-1.2.0/tests/test_pretransform_specs.py` & `vegafusion-1.2.1/tests/test_pretransform_specs.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.0/tests/test_row_limit.py` & `vegafusion-1.2.1/tests/test_row_limit.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.0/tests/test_save.py` & `vegafusion-1.2.1/tests/test_save.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.0/tests/test_transformed_data.py` & `vegafusion-1.2.1/tests/test_transformed_data.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.0/tests/test_transformer.py` & `vegafusion-1.2.1/tests/test_transformer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.0/vegafusion/__init__.py` & `vegafusion-1.2.1/vegafusion/__init__.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.0/vegafusion/compilers.py` & `vegafusion-1.2.1/vegafusion/compilers.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.0/vegafusion/connection/__init__.py` & `vegafusion-1.2.1/vegafusion/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.0/vegafusion/connection/duckdb.py` & `vegafusion-1.2.1/vegafusion/connection/duckdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,23 +150,23 @@
             # ability to install extensions
             try:
                 connection.install_extension("httpfs")
                 connection.load_extension("httpfs")
             except (IOError, duckdb.IOException, duckdb.InvalidInputException) as e:
                 warnings.warn(f"Failed to install and load the DuckDB httpfs extension:\n{e}")
 
+            # Use a less round number for pandas_analyze_sample (default is 1000)
+            connection.execute("SET GLOBAL pandas_analyze_sample=1007")
+
         # The icu extension is pre-bundled in Python, so no need to install it
         connection.load_extension("icu")
 
         self.conn = connection
         self.logger = logging.getLogger("DuckDbConnection")
 
-        # Use a less round number for pandas_analyze_sample (default is 1000)
-        self.conn.execute("SET GLOBAL pandas_analyze_sample=1007")
-
         self._registered_table_schemas = dict()
         # Call self.tables to warm the cache of table schemas
         self.tables()
 
     @classmethod
     def dialect(cls) -> str:
         return "duckdb"
```

### Comparing `vegafusion-1.2.0/vegafusion/evaluation.py` & `vegafusion-1.2.1/vegafusion/evaluation.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.0/vegafusion/local_tz.py` & `vegafusion-1.2.1/vegafusion/local_tz.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.0/vegafusion/renderer.py` & `vegafusion-1.2.1/vegafusion/renderer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.0/vegafusion/runtime.py` & `vegafusion-1.2.1/vegafusion/runtime.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.0/vegafusion/save.py` & `vegafusion-1.2.1/vegafusion/save.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.0/vegafusion/transformer.py` & `vegafusion-1.2.1/vegafusion/transformer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.0/vegafusion/utils.py` & `vegafusion-1.2.1/vegafusion/utils.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.2.0/vegafusion.egg-info/PKG-INFO` & `vegafusion-1.2.1/vegafusion.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vegafusion
-Version: 1.2.0
+Version: 1.2.1
 Summary: Core tools for using VegaFusion from Python
 License: BSD-3-Clause
 Keywords: vega,altair,vegafusion,arrow
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vegafusion-1.2.0/vegafusion.egg-info/SOURCES.txt` & `vegafusion-1.2.1/vegafusion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

