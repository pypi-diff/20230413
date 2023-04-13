# Comparing `tmp/singular_client-0.1.4.tar.gz` & `tmp/singular_client-0.1.5.tar.gz`

## Comparing `singular_client-0.1.4.tar` & `singular_client-0.1.5.tar`

### file list

```diff
@@ -1,30 +1,32 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 singular_client-0.1.4/.DS_Store
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 singular_client-0.1.4/.python-version
--rw-r--r--   0        0        0    40764 2020-02-02 00:00:00.000000 singular_client-0.1.4/ALL Dimensions and Metrics.csv
--rw-r--r--   0        0        0    27890 2020-02-02 00:00:00.000000 singular_client-0.1.4/ALL Dimensions and Metrics.xlsx
--rw-r--r--   0        0        0    40690 2020-02-02 00:00:00.000000 singular_client-0.1.4/all_dimensions_and_metrics.csv
--rw-r--r--   0        0        0    99036 2020-02-02 00:00:00.000000 singular_client-0.1.4/copilot magic documents.png
--rw-r--r--   0        0        0    66321 2020-02-02 00:00:00.000000 singular_client-0.1.4/dimensions_and_metrics.py
--rw-r--r--   0        0        0    15837 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client.zip
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 singular_client-0.1.4/test.json
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/.DS_Store
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/__init__.py
--rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/_bases.py
--rw-r--r--   0        0        0   133384 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/_generate_dim_and_metric_types.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/all_arguments.py
--rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/api.py
--rwxr-xr-x   0        0        0    15519 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/arguments.py
--rw-r--r--   0        0        0    67995 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/dimensions_and_metrics.py
--rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/documents.py
--rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/utils.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/endpoints/__init__.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/endpoints/governance.py
--rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/endpoints/links.py
--rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/endpoints/links_legacy.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/endpoints/monetization.py
--rw-r--r--   0        0        0     8534 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/endpoints/reporting.py
--rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 singular_client-0.1.4/singular_client/endpoints/skan.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 singular_client-0.1.4/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 singular_client-0.1.4/README.md
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 singular_client-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 singular_client-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 singular_client-0.1.5/.DS_Store
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 singular_client-0.1.5/.python-version
+-rw-r--r--   0        0        0    40764 2020-02-02 00:00:00.000000 singular_client-0.1.5/ALL Dimensions and Metrics.csv
+-rw-r--r--   0        0        0    27890 2020-02-02 00:00:00.000000 singular_client-0.1.5/ALL Dimensions and Metrics.xlsx
+-rw-r--r--   0        0        0    40690 2020-02-02 00:00:00.000000 singular_client-0.1.5/all_dimensions_and_metrics.csv
+-rw-r--r--   0        0        0    99036 2020-02-02 00:00:00.000000 singular_client-0.1.5/copilot magic documents.png
+-rw-r--r--   0        0        0    65639 2020-02-02 00:00:00.000000 singular_client-0.1.5/custom_fields.py
+-rw-r--r--   0        0        0    66321 2020-02-02 00:00:00.000000 singular_client-0.1.5/dimensions_and_metrics.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 singular_client-0.1.5/test.json
+-rw-r--r--   0        0        0    17741 2020-02-02 00:00:00.000000 singular_client-0.1.5/test_get_custom.pkl
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/__init__.py
+-rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/_bases.py
+-rw-r--r--   0        0        0    14536 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/_make_exceptions_module.py
+-rw-r--r--   0        0        0   134011 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/_make_fields_module.py
+-rw-r--r--   0        0        0     5873 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/api.py
+-rwxr-xr-x   0        0        0    14480 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/arguments.py
+-rw-r--r--   0        0        0     7433 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/documents.py
+-rw-r--r--   0        0        0     9161 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/exceptions.py
+-rw-r--r--   0        0        0    75071 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/fields.py
+-rw-r--r--   0        0        0     4308 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/make_custom_fields_module.py
+-rw-r--r--   0        0        0     8814 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/utils.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/endpoints/__init__.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/endpoints/governance.py
+-rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/endpoints/links.py
+-rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/endpoints/links_legacy.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/endpoints/monetization.py
+-rw-r--r--   0        0        0     9800 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/endpoints/reporting.py
+-rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/endpoints/skan.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 singular_client-0.1.5/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 singular_client-0.1.5/README.md
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 singular_client-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 singular_client-0.1.5/PKG-INFO
```

### Comparing `singular_client-0.1.4/.DS_Store` & `singular_client-0.1.5/.DS_Store`

 * *Files 13% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 00000230: 0073 0074 6d6f 4444 626c 6f62 0000 0008  .s.tmoDDblob....
 00000240: 9f50 81a7 c3f1 c441 0000 0004 0064 0069  .P.....A.....d.i
 00000250: 0073 0074 6d6f 6444 626c 6f62 0000 0008  .s.tmodDblob....
 00000260: 9f50 81a7 c3f1 c441 0000 0004 0064 0069  .P.....A.....d.i
 00000270: 0073 0074 7068 3153 636f 6d70 0000 0000  .s.tph1Scomp....
 00000280: 0000 7000 0000 000f 0073 0069 006e 0067  ..p......s.i.n.g
 00000290: 0075 006c 0061 0072 005f 0063 006c 0069  .u.l.a.r._.c.l.i
-000002a0: 0065 006e 0074 6473 636c 626f 6f6c 0100  .e.n.tdsclbool..
+000002a0: 0065 006e 0074 6473 636c 626f 6f6c 0000  .e.n.tdsclbool..
 000002b0: 0000 0f00 7300 6900 6e00 6700 7500 6c00  ....s.i.n.g.u.l.
 000002c0: 6100 7200 5f00 6300 6c00 6900 6500 6e00  a.r._.c.l.i.e.n.
 000002d0: 746c 6731 5363 6f6d 7000 0000 0000 0278  tlg1Scomp......x
 000002e0: 0300 0000 0f00 7300 6900 6e00 6700 7500  ......s.i.n.g.u.
 000002f0: 6c00 6100 7200 5f00 6300 6c00 6900 6500  l.a.r._.c.l.i.e.
 00000300: 6e00 746d 6f44 4462 6c6f 6200 0000 0800  n.tmoDDblob.....
 00000310: 0080 ccdb f1c4 4100 0000 0f00 7300 6900  ......A.....s.i.
```

### Comparing `singular_client-0.1.4/ALL Dimensions and Metrics.csv` & `singular_client-0.1.5/ALL Dimensions and Metrics.csv`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.4/ALL Dimensions and Metrics.xlsx` & `singular_client-0.1.5/ALL Dimensions and Metrics.xlsx`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.4/all_dimensions_and_metrics.csv` & `singular_client-0.1.5/all_dimensions_and_metrics.csv`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.4/copilot magic documents.png` & `singular_client-0.1.5/copilot magic documents.png`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.4/dimensions_and_metrics.py` & `singular_client-0.1.5/dimensions_and_metrics.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.4/singular_client/_bases.py` & `singular_client-0.1.5/singular_client/_bases.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+BASE CLASSES
+============
+Defines the inherited behavior of all endpoints, and response lists.
+"""
 from __future__ import annotations
 from typing import (
     TYPE_CHECKING,
     TypeVar,
     Union,
     Literal,
     Hashable,
@@ -76,15 +81,17 @@
             # `data` might contain dicts or lists. Ignore them.
             kwargs_key += tuple(
                 (k, v) for k, v in data.items() if not isinstance(v, (list, dict))
             )
 
         cache_found = self.cache.get(kwargs_key)
         if cache_found:
-            print("Using cached response from", f"{self.method.upper()} '{self.endpoint}'")
+            print(
+                "Using cached response from", f"{self.method.upper()} '{self.endpoint}'"
+            )
             return cache_found
 
         print("New request:", f"{self.method.upper()} '{self.endpoint}'")
 
         res = self.api.request(
             endpoint=self.endpoint, method=self.method, params=kwargs, data=data
         )
```

### Comparing `singular_client-0.1.4/singular_client/_generate_dim_and_metric_types.py` & `singular_client-0.1.5/singular_client/_make_fields_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,39 +21,34 @@
 from typing import List, overload, Literal, Iterable, Tuple, Optional, Union
 import pandas as pd, numpy as np
 import re
 from singular_client.utils import (
     format_type,
     format_constant,
     format_variable,
+    read_raw_html,
 )
 
-DEFAULT_TABLE_FILENAME = "all_dimensions_and_metrics.csv"
-DEFAULT_PY_MODULE_FILENAME = "dimensions_and_metrics.py"
+DEFAULT_TABLE_FILENAME = "fields.csv"
+DEFAULT_PY_MODULE_FILENAME = "fields.py"
 
 REPORT_CATEGORIES = dict(
-    in_general='general',
-    in_creative='creative',
-    in_skan='skan',
-    in_skan_raw='skan raw',
-    in_ad_mon='ad mon',
+    in_general="general",
+    in_creative="creative",
+    in_skan="skan",
+    in_skan_raw="skan raw",
+    in_ad_mon="ad mon",
 )
 SOURCE_CATEGORIES = dict(
-    from_network='network',
-    from_tracker='tracker',
+    from_network="network",
+    from_tracker="tracker",
 )
 
 CATEGORIES = {**SOURCE_CATEGORIES, **REPORT_CATEGORIES}
 
-class Naming:
-    """ Naming options for generated python code. """
-    # Type naming
-    field_args = lambda x: x + "_args"  # "from_network_dimension" -> "from_network_dimension_args"
-    validator_func = lambda x: "is_" + x  # "in_skan" -> def is_in_skan(x): ...
-    constant_list = lambda x: x
 
 def main(
     raw_html: Optional[str] = None,
     write_table: Union[str, bool] = True,
     write_py_module: Union[str, bool] = True,
 ) -> Tuple[pd.DataFrame, str]:
     """
@@ -63,15 +58,15 @@
     """
 
     # Use default html if none provided, or read file if text is short enough
     if not raw_html:
         raw_html = _RAW_HTML
 
     if len(raw_html) < 200:
-        with open(raw_html, 'r') as f:
+        with open(raw_html, "r") as f:
             raw_html = f.read()
 
     # Processing
     df = read_html(raw_html)
     code = generate_python_file(df.copy())
 
     # Writing
@@ -79,155 +74,193 @@
         if write_table == True:
             write_table = DEFAULT_TABLE_FILENAME
         df.copy().to_csv(write_table, index=False)
 
     if write_py_module:
         if write_py_module == True:
             write_py_module = DEFAULT_PY_MODULE_FILENAME
-        with open(write_py_module, 'w') as f:
+        with open(write_py_module, "w") as f:
             f.write(code)
 
     return df, code
 
+
 def generate_python_file(df: pd.DataFrame) -> pd.DataFrame:
 
-    df.dropna(subset=['name'], inplace=True)
-    df['field'] = True
-    df['dimension'] = np.where(df.kind == 'dimension', True, False)
-    df['metric'] = np.where(df.kind == 'metric', True, False)
+    df.dropna(subset=["name"], inplace=True)
+    df["field"] = True
+    df["dimension"] = np.where(df.kind == "dimension", True, False)
+    df["metric"] = np.where(df.kind == "metric", True, False)
 
     def prefix(s, prefix=None):
-        return f'{prefix}_{s}' if prefix else s
+        return f"{prefix}_{s}" if prefix else s
 
     s = DOC + IMPORTS
 
     base = "field"
     name = base
-    s += generate_spec(name, df['name'])
+    s += generate_spec(name, df.name)
 
-    for field in ['dimension', 'metric']:
+    for field in ["dimension", "metric"]:
         df_field = df[df[field]]
         name_field = field
-        s += generate_spec(name_field, df_field['name'])
+        s += generate_spec(name_field, df_field.name)
 
         for report in REPORT_CATEGORIES:
             df_report = df_field[df_field[report]]
             name_report = prefix(report, name_field)
-            s += generate_spec(name_report, df_report['name'])
+            s += generate_spec(name_report, df_report.name)
 
             for source in SOURCE_CATEGORIES:
                 df_source = df_report[df_report[source]]
                 name_source = prefix(source, name_report)
-                s += generate_spec(name_source, df_source['name'])
+                s += generate_spec(name_source, df_source.name)
 
         for source in SOURCE_CATEGORIES:
             df_source = df_field[df_field[source]]
             name_source = prefix(source, name_field)
-            s += generate_spec(name_source, df_source['name'])
+            s += generate_spec(name_source, df_source.name)
 
     for report in REPORT_CATEGORIES:
         df_report = df[df[report]]
         name_report = prefix(report, base)
-        s += generate_spec(name_report, df_report['name'])
+        s += generate_spec(name_report, df_report.name)
 
         for source in SOURCE_CATEGORIES:
             df_source = df_report[df_report[source]]
             name_source = prefix(source, name_report)
-            s += generate_spec(name_source, df_source['name'])
+            s += generate_spec(name_source, df_source.name)
 
     for source in SOURCE_CATEGORIES:
         df_source = df[df[source]]
         name_source = prefix(source, base)
-        s += generate_spec(name_source, df_source['name'])
+        s += generate_spec(name_source, df_source.name)
+
+    mapping = dict(zip(df.name, df.display_name))
+    s += gen_field_mapping("FIELD_MAPPING", mapping)
     return s
 
-def _list_value(value: str) -> str:
+
+def list_value(value: str) -> str:
     return f'    "{value}",\n'
 
-def _literal_type_name(name: str) -> str:
+
+def dict_item(key: str, value: str) -> str:
+    return f'    {key}="{value}",\n'
+
+
+def literal_type_name(name: str) -> str:
     return format_type(name)
 
-def _constant_type_name(name: str) -> str:
+
+def constant_type_name(name: str) -> str:
     return format_constant(name)
 
-def _args_type_name(name: str) -> str:
-    return format_type(name) + "Args"
 
-def _validator_func_name(name: str) -> str:
-    return "is_" + format_variable(name)
+def args_type_name(name: str) -> str:
+    return format_type(name + "_args")
+
+
+def validator_func_name(name: str) -> str:
+    return format_variable("is_" + name)
 
-def _gen_literal_type(name: str, values: Iterable[str]) -> str:
-    """ Create Literal type using `values` as args"""
-    type_name = _literal_type_name(name)
+
+def gen_literal_type(name: str, values: Iterable[str]) -> str:
+    """Create Literal type using `values` as args"""
+    type_name = literal_type_name(name)
     s = type_name + " = Literal[\n"
     for value in values:
-        s += _list_value(value)
+        s += list_value(value)
     return s + "]\n\n"
 
-def _gen_args_type(name: str) -> str:
+
+def gen_args_type(name: str) -> str:
     """
     Create a Union type that allows for an iterable of valid literals
     of a type, or a single string
     """
-    type_name = _literal_type_name(name)
-    args_name = _args_type_name(name)
+    type_name = literal_type_name(name)
+    args_name = args_type_name(name)
     return f"{args_name} = Union[Iterable[{type_name}], str]\n\n"
 
-def _gen_constant_list(name: str) -> str:
+
+def gen_constant_list(name: str) -> str:
     """Extract args from Literal, `name`"""
-    type_name = _literal_type_name(name)
-    const_name = _constant_type_name(name)
+    type_name = literal_type_name(name)
+    const_name = constant_type_name(name)
     return f"{const_name} = list(get_args({type_name}))\n\n"
 
-def _gen_validator_func_for_type(name: str) -> str:
+
+def gen_validator_func_for_type(name: str) -> str:
     """Create validator function for type `name`"""
-    constant_name = _constant_type_name(name)
-    validator_name = _validator_func_name(name)
-    type_name = _literal_type_name(name)
+    constant_name = constant_type_name(name)
+    validator_name = validator_func_name(name)
+    type_name = literal_type_name(name)
     return f'''def {validator_name}(name: Union[str, {type_name}]) -> bool:
     """
     Check if `name` is a valid non-custom `{type_name}` from Singular.
     """
     return name in {constant_name}
 
 
 '''
 
+
 def generate_spec(name: str, values: Iterable[str]) -> str:
     """Generate all 4 required items"""
     return (
         # _literal_type_name(name) + "\n"
-        _gen_literal_type(name, values)
-        + _gen_args_type(name)
-        + _gen_constant_list(name)
-        + _gen_validator_func_for_type(name)
+        gen_literal_type(name, values)
+        + gen_args_type(name)
+        + gen_constant_list(name)
+        + gen_validator_func_for_type(name)
     )
 
+
+def gen_field_mapping(name: str, mapping: dict) -> str:
+    """Generate dictionary with field name to display name mapping"""
+    s = format_constant(name) + " = dict(\n"
+    for k, v in mapping.items():
+        s += dict_item(k, v)
+    return s + ")\n\n"
+
+
 IMPORTS = "from typing import Literal, Iterable, Union, get_args\n\n\n"
 
 DOC = '''"""
 VALID PARAMETER TYPES FOR ENDPOINTS
 ===================================
 
+    Instant, real-time, as-you-type checking of dimension/metric names in your IDE.
+
+
 Defines Literal types, constant lists, and validator function for all combinations
-of dimensions and metrics in Singular.
+of dimension and metric categories in Singular.
+
+Literals allow your IDE to validate that the string you're typing is a valid
+option for the type-hinted parameter you're passing args to.
+
+Fields are broken down into 3 levels.
+
+Every combination of these 3 levels has a corresponding Literal type, constant list,
+validator function, and more.
 
 Level 1
     Field
     Dimension
     Metric
 
-Level 2
+Level 2  (Available in ...)
     InGeneral
     InCreative
     InSkan
-    InSkan Raw
-    InAd Mon
+    InSkanRaw
+    InAdMon
     
-Level 3
+Level 3  (Data came from ...)
     FromNetwork
     FromTracker
 
 For each combination, define (using DimensionFromNetwork as an example):
     FromNetworkDimension
         A Literal string type with all valid dimensions that come from ad networks.
         When something is type-hinted with this, your IDE will, in real time as
@@ -262,72 +295,70 @@
 '''
 
 
 # ==============================================================================
 # ==============================================================================
 # HTML READING
 
+
 def read_html(raw_html: Optional[str] = None) -> pd.DataFrame:
     """
     1. Go to this link: https://support.singular.net/hc/en-us/articles/203389179-Singular-Metrics-and-Dimensions-Descriptions
     2. Inspect element. Copy table HTML. Make sure "Show:" filter is set to "All"
     3. Paste the HTML into the _RAW_HTML variable below, and run this script.
     """
-    if not raw_html:
-        raw_html = _RAW_HTML
-    dfs = pd.read_html(raw_html)
-    assert len(dfs) >= 1, "No tables found in HTML"
-    df = dfs[0]
+    df = read_raw_html(raw_html, default=_RAW_HTML)
     df = df.drop(0).reset_index(drop=True)
 
     df.columns = [
-        'display_name',
-        'name',
-        'desc',
-        'available_in',
-        'pulled_from',
+        "display_name",
+        "name",
+        "desc",
+        "available_in",
+        "pulled_from",
     ]
 
     def bool_if_contains(df, col, val) -> pd.Series:
-        return np.where(
-            df[col].str.lower().str.contains(val.lower()),
-            True, False
-        )
+        return np.where(df[col].str.lower().str.contains(val.lower()), True, False)
+
+    # Replace nulls with actual null
+    df.replace(r"\bN/A\b", np.nan, regex=True, inplace=True)
+
+    # Fix names
+    df.name = df.name.str.replace(r"_ ", r"_", regex=False)
+    with_spaces = [x for x in list(df.name) if not pd.isnull(x) and " " in str(x)]
+    assert not with_spaces, with_spaces
 
     # Separate data availability to boolean columns
     for new_name, name in SOURCE_CATEGORIES.items():
-        df[new_name] = bool_if_contains(df, 'pulled_from', name)
+        df[new_name] = bool_if_contains(df, "pulled_from", name)
 
     for new_name, name in REPORT_CATEGORIES.items():
-        df[new_name] = bool_if_contains(df, 'available_in', name)
+        df[new_name] = bool_if_contains(df, "available_in", name)
 
     # Fill nulls wil False
     for col in CATEGORIES:
         df.loc[:, col] = df[col].fillna(False).astype(bool)
 
-    df.drop(
-        columns=['pulled_from', 'available_in'],
-        inplace=True
-    )
+    df.drop(columns=["pulled_from", "available_in"], inplace=True)
 
     # Separate dimensions and metrics
-    delimiter_index = df[df['display_name'] == 'Metrics'].index[0]
-    df.insert(0, 'kind', 'dimension')
-    df.loc[delimiter_index+1:, 'kind'] = 'metric'
+    delimiter_index = df[df["display_name"] == "Metrics"].index[0]
+    df.insert(0, "kind", "dimension")
+    df.loc[delimiter_index + 1 :, "kind"] = "metric"
 
     # Remove delimiter row
-    df = df[df['display_name'] != 'Metrics']
-
-    # Replace nulls with actual null
-    df.replace(r"\bN/A\b", np.nan, regex=True, inplace=True)
+    df = df[df["display_name"] != "Metrics"]
 
     # Moving stuff around
-    df.insert(len(df.columns)-1, 'desc', df.pop('desc'))
+    df.insert(len(df.columns) - 1, "desc", df.pop("desc"))
     df.reset_index(drop=True, inplace=True)
     df = df.copy()
+    global field_table
+    field_table = df.copy()
     return df
 
 
 _RAW_HTML = """
 <table id="table1" class="table small-font" style="table-layout: fixed; width: 100%;">
 <tbody>
 <tr class="always-visible">
@@ -4232,9 +4263,9 @@
 </tr>
 </tbody>
 </table>
 
 """
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main(write_table=False)
```

### Comparing `singular_client-0.1.4/singular_client/arguments.py` & `singular_client-0.1.5/singular_client/arguments.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,16 @@
 """
-VALID PARAMETER TYPES FOR ENDPOINTS
-===================================
+DEPRECATED: See the `fields` module for a full list of dimensions
+and metrics by report type and source.
 
-T
+---
 
-Use cases
----------
-
-Static type checking
-    Any endpoint parameter for which there is a fixed set of valid values is
-    typed as a Literal. Your IDE will statically check that you are passing
-    valid options and bark at you otherwise. Parameters that require a list of
-    valid values (dimensions and metrics) allow you to override this behavior
-    by joining options to a comma-sep string before passing.
-
-Filling default values
-    The arguments stored in each Literal are also stored as regular lists (see
-    bottom of file). These are used to fill in default values for parameters
-    that are left empty. For instance, any endpoint which requires a list of
-    dimensions or metrics will defualt to returning all available attributes
-    if param is left null.
-
-Easy user-access to available options for an endpoint
-    Endpoints which require a list of valid dimensions or metrics will have
-    a `available_dimensions` class attribute, etc.
-
-
-Notes
------
-When a parameter requires a list of valid Literal options, (rather than
-just a single one), your type checker will be unhappy if you pass this list
-as a variable, rather than a hardcoded list. These parameters also accept
-a string, so you can override this behavior by joining the list first.
+Reporting parameter options for dimensions and metrics, from the
+endpoints' documentation pages. These are missing/incomplete, when
+compared to the full list provided in the Glossary page.
 """
 from typing import Literal, get_args
 
 TimeBreakdown = Literal["day", "week", "month", "all"]
 FileFormat = Literal["json", "csv"]
 CountryCodeFormat = Literal["iso3", "iso"]
 LinkType = Literal["custom", "partner", "mobile_web_to_app"]
```

### Comparing `singular_client-0.1.4/singular_client/dimensions_and_metrics.py` & `singular_client-0.1.5/singular_client/fields.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,38 @@
 """
 VALID PARAMETER TYPES FOR ENDPOINTS
 ===================================
 
+    Instant, real-time, as-you-type checking of dimension/metric names in your IDE.
+
+
 Defines Literal types, constant lists, and validator function for all combinations
-of dimensions and metrics in Singular.
+of dimension and metric categories in Singular.
+
+Literals allow your IDE to validate that the string you're typing is a valid
+option for the type-hinted parameter you're passing args to.
+
+Fields are broken down into 3 levels.
+
+Every combination of these 3 levels has a corresponding Literal type, constant list,
+validator function, and more.
 
 Level 1
     Field
     Dimension
     Metric
 
-Level 2
+Level 2  (Available in ...)
     InGeneral
     InCreative
     InSkan
-    InSkan Raw
-    InAd Mon
+    InSkanRaw
+    InAdMon
     
-Level 3
+Level 3  (Data came from ...)
     FromNetwork
     FromTracker
 
 For each combination, define (using DimensionFromNetwork as an example):
     FromNetworkDimension
         A Literal string type with all valid dimensions that come from ad networks.
         When something is type-hinted with this, your IDE will, in real time as
@@ -112,15 +123,15 @@
     "adn_creative_id",
     "adn_creative_name",
     "adn_sub_campaign_id",
     "adn_sub_campaign_name",
     "creative_type",
     "install_app_store",
     "original_bid_amount",
-    "original_ metadata_currency",
+    "original_metadata_currency",
     "adn_original_currency",
     "os",
     "placement",
     "platform",
     "publisher_id",
     "publisher_site_id",
     "publisher_site_name",
@@ -144,15 +155,15 @@
     "tracker_campaign_id",
     "tracker_campaign_name",
     "tracker_creative_id",
     "tracker_creative_name",
     "tracker_name",
     "tracker_source_name",
     "tracker_sub_campaign_id",
-    "tracker_sub_campaign_ name",
+    "tracker_sub_campaign_name",
     "adn_utc_offset",
     "utm_campaign",
     "utm_content",
     "utm_medium",
     "utm_source",
     "utm_term",
     "skan_validated",
@@ -223,15 +234,15 @@
 
 FieldArgs = Union[Iterable[Field], str]
 
 FIELD = list(get_args(Field))
 
 def is_field(name: Union[str, Field]) -> bool:
     """
-    Check if `name` is a valid non-custom `Field` from **Singular**.
+    Check if `name` is a valid non-custom `Field` from Singular.
     """
     return name in FIELD
 
 
 Dimension = Literal[
     "adn_account_id",
     "adn_account_name",
@@ -288,15 +299,15 @@
     "adn_creative_id",
     "adn_creative_name",
     "adn_sub_campaign_id",
     "adn_sub_campaign_name",
     "creative_type",
     "install_app_store",
     "original_bid_amount",
-    "original_ metadata_currency",
+    "original_metadata_currency",
     "adn_original_currency",
     "os",
     "placement",
     "platform",
     "publisher_id",
     "publisher_site_id",
     "publisher_site_name",
@@ -320,15 +331,15 @@
     "tracker_campaign_id",
     "tracker_campaign_name",
     "tracker_creative_id",
     "tracker_creative_name",
     "tracker_name",
     "tracker_source_name",
     "tracker_sub_campaign_id",
-    "tracker_sub_campaign_ name",
+    "tracker_sub_campaign_name",
     "adn_utc_offset",
     "utm_campaign",
     "utm_content",
     "utm_medium",
     "utm_source",
     "utm_term",
     "skan_validated",
@@ -347,15 +358,15 @@
 
 DimensionArgs = Union[Iterable[Dimension], str]
 
 DIMENSION = list(get_args(Dimension))
 
 def is_dimension(name: Union[str, Dimension]) -> bool:
     """
-    Check if `name` is a valid non-custom `Dimension` from **Singular**.
+    Check if `name` is a valid non-custom `Dimension` from Singular.
     """
     return name in DIMENSION
 
 
 DimensionInGeneral = Literal[
     "adn_account_id",
     "adn_account_name",
@@ -391,15 +402,15 @@
     "keyword_match_type",
     "adn_campaign_id",
     "adn_campaign_name",
     "adn_sub_campaign_id",
     "adn_sub_campaign_name",
     "install_app_store",
     "original_bid_amount",
-    "original_ metadata_currency",
+    "original_metadata_currency",
     "adn_original_currency",
     "os",
     "placement",
     "platform",
     "publisher_id",
     "publisher_site_id",
     "publisher_site_name",
@@ -415,15 +426,15 @@
     "sub_campaign_name",
     "tracking_url",
     "tracker_campaign_id",
     "tracker_campaign_name",
     "tracker_name",
     "tracker_source_name",
     "tracker_sub_campaign_id",
-    "tracker_sub_campaign_ name",
+    "tracker_sub_campaign_name",
     "adn_utc_offset",
     "admon_data_source",
     "data_connector_id",
     "data_connector_source_name",
     "data_connector_timestamp_utc",
     "data_connector_username",
     "singular_campaign_id",
@@ -431,15 +442,15 @@
 
 DimensionInGeneralArgs = Union[Iterable[DimensionInGeneral], str]
 
 DIMENSION_IN_GENERAL = list(get_args(DimensionInGeneral))
 
 def is_dimension_in_general(name: Union[str, DimensionInGeneral]) -> bool:
     """
-    Check if `name` is a valid non-custom `DimensionInGeneral` from **Singular**.
+    Check if `name` is a valid non-custom `DimensionInGeneral` from Singular.
     """
     return name in DIMENSION_IN_GENERAL
 
 
 DimensionInGeneralFromNetwork = Literal[
     "adn_account_id",
     "adn_account_name",
@@ -472,15 +483,15 @@
     "keyword_match_type",
     "adn_campaign_id",
     "adn_campaign_name",
     "adn_sub_campaign_id",
     "adn_sub_campaign_name",
     "install_app_store",
     "original_bid_amount",
-    "original_ metadata_currency",
+    "original_metadata_currency",
     "adn_original_currency",
     "os",
     "placement",
     "platform",
     "publisher_id",
     "publisher_site_id",
     "publisher_site_name",
@@ -506,15 +517,15 @@
 
 DimensionInGeneralFromNetworkArgs = Union[Iterable[DimensionInGeneralFromNetwork], str]
 
 DIMENSION_IN_GENERAL_FROM_NETWORK = list(get_args(DimensionInGeneralFromNetwork))
 
 def is_dimension_in_general_from_network(name: Union[str, DimensionInGeneralFromNetwork]) -> bool:
     """
-    Check if `name` is a valid non-custom `DimensionInGeneralFromNetwork` from **Singular**.
+    Check if `name` is a valid non-custom `DimensionInGeneralFromNetwork` from Singular.
     """
     return name in DIMENSION_IN_GENERAL_FROM_NETWORK
 
 
 DimensionInGeneralFromTracker = Literal[
     "app",
     "site_public_id",
@@ -532,44 +543,44 @@
     "country_field",
     "min_roas",
     "installer_source",
     "adn_sub_campaign_id",
     "adn_sub_campaign_name",
     "install_app_store",
     "original_bid_amount",
-    "original_ metadata_currency",
+    "original_metadata_currency",
     "os",
     "platform",
     "region_field",
     "retention",
     "source",
     "standardized_bid_strategy",
     "sub_campaign_id",
     "sub_campaign_name",
     "tracker_campaign_id",
     "tracker_campaign_name",
     "tracker_name",
     "tracker_source_name",
     "tracker_sub_campaign_id",
-    "tracker_sub_campaign_ name",
+    "tracker_sub_campaign_name",
     "admon_data_source",
     "data_connector_id",
     "data_connector_source_name",
     "data_connector_timestamp_utc",
     "data_connector_username",
     "singular_campaign_id",
 ]
 
 DimensionInGeneralFromTrackerArgs = Union[Iterable[DimensionInGeneralFromTracker], str]
 
 DIMENSION_IN_GENERAL_FROM_TRACKER = list(get_args(DimensionInGeneralFromTracker))
 
 def is_dimension_in_general_from_tracker(name: Union[str, DimensionInGeneralFromTracker]) -> bool:
     """
-    Check if `name` is a valid non-custom `DimensionInGeneralFromTracker` from **Singular**.
+    Check if `name` is a valid non-custom `DimensionInGeneralFromTracker` from Singular.
     """
     return name in DIMENSION_IN_GENERAL_FROM_TRACKER
 
 
 DimensionInCreative = Literal[
     "adn_account_id",
     "adn_account_name",
@@ -610,15 +621,15 @@
 
 DimensionInCreativeArgs = Union[Iterable[DimensionInCreative], str]
 
 DIMENSION_IN_CREATIVE = list(get_args(DimensionInCreative))
 
 def is_dimension_in_creative(name: Union[str, DimensionInCreative]) -> bool:
     """
-    Check if `name` is a valid non-custom `DimensionInCreative` from **Singular**.
+    Check if `name` is a valid non-custom `DimensionInCreative` from Singular.
     """
     return name in DIMENSION_IN_CREATIVE
 
 
 DimensionInCreativeFromNetwork = Literal[
     "adn_account_id",
     "adn_account_name",
@@ -657,15 +668,15 @@
 
 DimensionInCreativeFromNetworkArgs = Union[Iterable[DimensionInCreativeFromNetwork], str]
 
 DIMENSION_IN_CREATIVE_FROM_NETWORK = list(get_args(DimensionInCreativeFromNetwork))
 
 def is_dimension_in_creative_from_network(name: Union[str, DimensionInCreativeFromNetwork]) -> bool:
     """
-    Check if `name` is a valid non-custom `DimensionInCreativeFromNetwork` from **Singular**.
+    Check if `name` is a valid non-custom `DimensionInCreativeFromNetwork` from Singular.
     """
     return name in DIMENSION_IN_CREATIVE_FROM_NETWORK
 
 
 DimensionInCreativeFromTracker = Literal[
     "app",
     "unified_campaign_id",
@@ -697,15 +708,15 @@
 
 DimensionInCreativeFromTrackerArgs = Union[Iterable[DimensionInCreativeFromTracker], str]
 
 DIMENSION_IN_CREATIVE_FROM_TRACKER = list(get_args(DimensionInCreativeFromTracker))
 
 def is_dimension_in_creative_from_tracker(name: Union[str, DimensionInCreativeFromTracker]) -> bool:
     """
-    Check if `name` is a valid non-custom `DimensionInCreativeFromTracker` from **Singular**.
+    Check if `name` is a valid non-custom `DimensionInCreativeFromTracker` from Singular.
     """
     return name in DIMENSION_IN_CREATIVE_FROM_TRACKER
 
 
 DimensionInSkan = Literal[
     "app",
     "unified_campaign_id",
@@ -724,15 +735,15 @@
 
 DimensionInSkanArgs = Union[Iterable[DimensionInSkan], str]
 
 DIMENSION_IN_SKAN = list(get_args(DimensionInSkan))
 
 def is_dimension_in_skan(name: Union[str, DimensionInSkan]) -> bool:
     """
-    Check if `name` is a valid non-custom `DimensionInSkan` from **Singular**.
+    Check if `name` is a valid non-custom `DimensionInSkan` from Singular.
     """
     return name in DIMENSION_IN_SKAN
 
 
 DimensionInSkanFromNetwork = Literal[
     "app",
     "unified_campaign_id",
@@ -751,15 +762,15 @@
 
 DimensionInSkanFromNetworkArgs = Union[Iterable[DimensionInSkanFromNetwork], str]
 
 DIMENSION_IN_SKAN_FROM_NETWORK = list(get_args(DimensionInSkanFromNetwork))
 
 def is_dimension_in_skan_from_network(name: Union[str, DimensionInSkanFromNetwork]) -> bool:
     """
-    Check if `name` is a valid non-custom `DimensionInSkanFromNetwork` from **Singular**.
+    Check if `name` is a valid non-custom `DimensionInSkanFromNetwork` from Singular.
     """
     return name in DIMENSION_IN_SKAN_FROM_NETWORK
 
 
 DimensionInSkanFromTracker = Literal[
     "app",
     "unified_campaign_id",
@@ -778,15 +789,15 @@
 
 DimensionInSkanFromTrackerArgs = Union[Iterable[DimensionInSkanFromTracker], str]
 
 DIMENSION_IN_SKAN_FROM_TRACKER = list(get_args(DimensionInSkanFromTracker))
 
 def is_dimension_in_skan_from_tracker(name: Union[str, DimensionInSkanFromTracker]) -> bool:
     """
-    Check if `name` is a valid non-custom `DimensionInSkanFromTracker` from **Singular**.
+    Check if `name` is a valid non-custom `DimensionInSkanFromTracker` from Singular.
     """
     return name in DIMENSION_IN_SKAN_FROM_TRACKER
 
 
 DimensionInSkanRaw = Literal[
     "app",
     "skan_conversion_value",
@@ -803,15 +814,15 @@
 
 DimensionInSkanRawArgs = Union[Iterable[DimensionInSkanRaw], str]
 
 DIMENSION_IN_SKAN_RAW = list(get_args(DimensionInSkanRaw))
 
 def is_dimension_in_skan_raw(name: Union[str, DimensionInSkanRaw]) -> bool:
     """
-    Check if `name` is a valid non-custom `DimensionInSkanRaw` from **Singular**.
+    Check if `name` is a valid non-custom `DimensionInSkanRaw` from Singular.
     """
     return name in DIMENSION_IN_SKAN_RAW
 
 
 DimensionInSkanRawFromNetwork = Literal[
     "app",
     "skan_conversion_value",
@@ -828,15 +839,15 @@
 
 DimensionInSkanRawFromNetworkArgs = Union[Iterable[DimensionInSkanRawFromNetwork], str]
 
 DIMENSION_IN_SKAN_RAW_FROM_NETWORK = list(get_args(DimensionInSkanRawFromNetwork))
 
 def is_dimension_in_skan_raw_from_network(name: Union[str, DimensionInSkanRawFromNetwork]) -> bool:
     """
-    Check if `name` is a valid non-custom `DimensionInSkanRawFromNetwork` from **Singular**.
+    Check if `name` is a valid non-custom `DimensionInSkanRawFromNetwork` from Singular.
     """
     return name in DIMENSION_IN_SKAN_RAW_FROM_NETWORK
 
 
 DimensionInSkanRawFromTracker = Literal[
     "app",
     "skan_conversion_value",
@@ -853,15 +864,15 @@
 
 DimensionInSkanRawFromTrackerArgs = Union[Iterable[DimensionInSkanRawFromTracker], str]
 
 DIMENSION_IN_SKAN_RAW_FROM_TRACKER = list(get_args(DimensionInSkanRawFromTracker))
 
 def is_dimension_in_skan_raw_from_tracker(name: Union[str, DimensionInSkanRawFromTracker]) -> bool:
     """
-    Check if `name` is a valid non-custom `DimensionInSkanRawFromTracker` from **Singular**.
+    Check if `name` is a valid non-custom `DimensionInSkanRawFromTracker` from Singular.
     """
     return name in DIMENSION_IN_SKAN_RAW_FROM_TRACKER
 
 
 DimensionInAdMon = Literal[
     "instance_id",
     "instance_name",
@@ -876,15 +887,15 @@
 
 DimensionInAdMonArgs = Union[Iterable[DimensionInAdMon], str]
 
 DIMENSION_IN_AD_MON = list(get_args(DimensionInAdMon))
 
 def is_dimension_in_ad_mon(name: Union[str, DimensionInAdMon]) -> bool:
     """
-    Check if `name` is a valid non-custom `DimensionInAdMon` from **Singular**.
+    Check if `name` is a valid non-custom `DimensionInAdMon` from Singular.
     """
     return name in DIMENSION_IN_AD_MON
 
 
 DimensionInAdMonFromNetwork = Literal[
     "instance_id",
     "instance_name",
@@ -899,15 +910,15 @@
 
 DimensionInAdMonFromNetworkArgs = Union[Iterable[DimensionInAdMonFromNetwork], str]
 
 DIMENSION_IN_AD_MON_FROM_NETWORK = list(get_args(DimensionInAdMonFromNetwork))
 
 def is_dimension_in_ad_mon_from_network(name: Union[str, DimensionInAdMonFromNetwork]) -> bool:
     """
-    Check if `name` is a valid non-custom `DimensionInAdMonFromNetwork` from **Singular**.
+    Check if `name` is a valid non-custom `DimensionInAdMonFromNetwork` from Singular.
     """
     return name in DIMENSION_IN_AD_MON_FROM_NETWORK
 
 
 DimensionInAdMonFromTracker = Literal[
     "instance_id",
     "instance_name",
@@ -922,15 +933,15 @@
 
 DimensionInAdMonFromTrackerArgs = Union[Iterable[DimensionInAdMonFromTracker], str]
 
 DIMENSION_IN_AD_MON_FROM_TRACKER = list(get_args(DimensionInAdMonFromTracker))
 
 def is_dimension_in_ad_mon_from_tracker(name: Union[str, DimensionInAdMonFromTracker]) -> bool:
     """
-    Check if `name` is a valid non-custom `DimensionInAdMonFromTracker` from **Singular**.
+    Check if `name` is a valid non-custom `DimensionInAdMonFromTracker` from Singular.
     """
     return name in DIMENSION_IN_AD_MON_FROM_TRACKER
 
 
 DimensionFromNetwork = Literal[
     "adn_account_id",
     "adn_account_name",
@@ -984,15 +995,15 @@
     "adn_creative_id",
     "adn_creative_name",
     "adn_sub_campaign_id",
     "adn_sub_campaign_name",
     "creative_type",
     "install_app_store",
     "original_bid_amount",
-    "original_ metadata_currency",
+    "original_metadata_currency",
     "adn_original_currency",
     "os",
     "placement",
     "platform",
     "publisher_id",
     "publisher_site_id",
     "publisher_site_name",
@@ -1035,15 +1046,15 @@
 
 DimensionFromNetworkArgs = Union[Iterable[DimensionFromNetwork], str]
 
 DIMENSION_FROM_NETWORK = list(get_args(DimensionFromNetwork))
 
 def is_dimension_from_network(name: Union[str, DimensionFromNetwork]) -> bool:
     """
-    Check if `name` is a valid non-custom `DimensionFromNetwork` from **Singular**.
+    Check if `name` is a valid non-custom `DimensionFromNetwork` from Singular.
     """
     return name in DIMENSION_FROM_NETWORK
 
 
 DimensionFromTracker = Literal[
     "instance_id",
     "instance_name",
@@ -1078,15 +1089,15 @@
     "min_roas",
     "installer_source",
     "adn_sub_campaign_id",
     "adn_sub_campaign_name",
     "creative_type",
     "install_app_store",
     "original_bid_amount",
-    "original_ metadata_currency",
+    "original_metadata_currency",
     "os",
     "platform",
     "region_field",
     "skan_redownloads",
     "retention",
     "skan_app_id",
     "skan_campaign_id",
@@ -1100,15 +1111,15 @@
     "tracker_campaign_id",
     "tracker_campaign_name",
     "tracker_creative_id",
     "tracker_creative_name",
     "tracker_name",
     "tracker_source_name",
     "tracker_sub_campaign_id",
-    "tracker_sub_campaign_ name",
+    "tracker_sub_campaign_name",
     "utm_campaign",
     "utm_content",
     "utm_medium",
     "utm_source",
     "utm_term",
     "skan_validated",
     "admon_data_source",
@@ -1126,15 +1137,15 @@
 
 DimensionFromTrackerArgs = Union[Iterable[DimensionFromTracker], str]
 
 DIMENSION_FROM_TRACKER = list(get_args(DimensionFromTracker))
 
 def is_dimension_from_tracker(name: Union[str, DimensionFromTracker]) -> bool:
     """
-    Check if `name` is a valid non-custom `DimensionFromTracker` from **Singular**.
+    Check if `name` is a valid non-custom `DimensionFromTracker` from Singular.
     """
     return name in DIMENSION_FROM_TRACKER
 
 
 Metric = Literal[
     "ad_clicks",
     "ad_impressions",
@@ -1192,15 +1203,15 @@
 
 MetricArgs = Union[Iterable[Metric], str]
 
 METRIC = list(get_args(Metric))
 
 def is_metric(name: Union[str, Metric]) -> bool:
     """
-    Check if `name` is a valid non-custom `Metric` from **Singular**.
+    Check if `name` is a valid non-custom `Metric` from Singular.
     """
     return name in METRIC
 
 
 MetricInGeneral = Literal[
     "frequency",
     "custom_clicks",
@@ -1232,15 +1243,15 @@
 
 MetricInGeneralArgs = Union[Iterable[MetricInGeneral], str]
 
 METRIC_IN_GENERAL = list(get_args(MetricInGeneral))
 
 def is_metric_in_general(name: Union[str, MetricInGeneral]) -> bool:
     """
-    Check if `name` is a valid non-custom `MetricInGeneral` from **Singular**.
+    Check if `name` is a valid non-custom `MetricInGeneral` from Singular.
     """
     return name in METRIC_IN_GENERAL
 
 
 MetricInGeneralFromNetwork = Literal[
     "frequency",
     "custom_clicks",
@@ -1272,15 +1283,15 @@
 
 MetricInGeneralFromNetworkArgs = Union[Iterable[MetricInGeneralFromNetwork], str]
 
 METRIC_IN_GENERAL_FROM_NETWORK = list(get_args(MetricInGeneralFromNetwork))
 
 def is_metric_in_general_from_network(name: Union[str, MetricInGeneralFromNetwork]) -> bool:
     """
-    Check if `name` is a valid non-custom `MetricInGeneralFromNetwork` from **Singular**.
+    Check if `name` is a valid non-custom `MetricInGeneralFromNetwork` from Singular.
     """
     return name in METRIC_IN_GENERAL_FROM_NETWORK
 
 
 MetricInGeneralFromTracker = Literal[
     "frequency",
     "custom_clicks",
@@ -1312,15 +1323,15 @@
 
 MetricInGeneralFromTrackerArgs = Union[Iterable[MetricInGeneralFromTracker], str]
 
 METRIC_IN_GENERAL_FROM_TRACKER = list(get_args(MetricInGeneralFromTracker))
 
 def is_metric_in_general_from_tracker(name: Union[str, MetricInGeneralFromTracker]) -> bool:
     """
-    Check if `name` is a valid non-custom `MetricInGeneralFromTracker` from **Singular**.
+    Check if `name` is a valid non-custom `MetricInGeneralFromTracker` from Singular.
     """
     return name in METRIC_IN_GENERAL_FROM_TRACKER
 
 
 MetricInCreative = Literal[
     "completed_video_views",
     "video_views",
@@ -1331,15 +1342,15 @@
 
 MetricInCreativeArgs = Union[Iterable[MetricInCreative], str]
 
 METRIC_IN_CREATIVE = list(get_args(MetricInCreative))
 
 def is_metric_in_creative(name: Union[str, MetricInCreative]) -> bool:
     """
-    Check if `name` is a valid non-custom `MetricInCreative` from **Singular**.
+    Check if `name` is a valid non-custom `MetricInCreative` from Singular.
     """
     return name in METRIC_IN_CREATIVE
 
 
 MetricInCreativeFromNetwork = Literal[
     "completed_video_views",
     "video_views",
@@ -1350,15 +1361,15 @@
 
 MetricInCreativeFromNetworkArgs = Union[Iterable[MetricInCreativeFromNetwork], str]
 
 METRIC_IN_CREATIVE_FROM_NETWORK = list(get_args(MetricInCreativeFromNetwork))
 
 def is_metric_in_creative_from_network(name: Union[str, MetricInCreativeFromNetwork]) -> bool:
     """
-    Check if `name` is a valid non-custom `MetricInCreativeFromNetwork` from **Singular**.
+    Check if `name` is a valid non-custom `MetricInCreativeFromNetwork` from Singular.
     """
     return name in METRIC_IN_CREATIVE_FROM_NETWORK
 
 
 MetricInCreativeFromTracker = Literal[
     "completed_video_views",
     "video_views",
@@ -1369,15 +1380,15 @@
 
 MetricInCreativeFromTrackerArgs = Union[Iterable[MetricInCreativeFromTracker], str]
 
 METRIC_IN_CREATIVE_FROM_TRACKER = list(get_args(MetricInCreativeFromTracker))
 
 def is_metric_in_creative_from_tracker(name: Union[str, MetricInCreativeFromTracker]) -> bool:
     """
-    Check if `name` is a valid non-custom `MetricInCreativeFromTracker` from **Singular**.
+    Check if `name` is a valid non-custom `MetricInCreativeFromTracker` from Singular.
     """
     return name in METRIC_IN_CREATIVE_FROM_TRACKER
 
 
 MetricInSkan = Literal[
     "skan_report_network_clicks",
     "skan_conversion_values_count",
@@ -1393,15 +1404,15 @@
 
 MetricInSkanArgs = Union[Iterable[MetricInSkan], str]
 
 METRIC_IN_SKAN = list(get_args(MetricInSkan))
 
 def is_metric_in_skan(name: Union[str, MetricInSkan]) -> bool:
     """
-    Check if `name` is a valid non-custom `MetricInSkan` from **Singular**.
+    Check if `name` is a valid non-custom `MetricInSkan` from Singular.
     """
     return name in METRIC_IN_SKAN
 
 
 MetricInSkanFromNetwork = Literal[
     "skan_report_network_clicks",
     "skan_conversion_values_count",
@@ -1417,15 +1428,15 @@
 
 MetricInSkanFromNetworkArgs = Union[Iterable[MetricInSkanFromNetwork], str]
 
 METRIC_IN_SKAN_FROM_NETWORK = list(get_args(MetricInSkanFromNetwork))
 
 def is_metric_in_skan_from_network(name: Union[str, MetricInSkanFromNetwork]) -> bool:
     """
-    Check if `name` is a valid non-custom `MetricInSkanFromNetwork` from **Singular**.
+    Check if `name` is a valid non-custom `MetricInSkanFromNetwork` from Singular.
     """
     return name in METRIC_IN_SKAN_FROM_NETWORK
 
 
 MetricInSkanFromTracker = Literal[
     "skan_report_network_clicks",
     "skan_conversion_values_count",
@@ -1441,15 +1452,15 @@
 
 MetricInSkanFromTrackerArgs = Union[Iterable[MetricInSkanFromTracker], str]
 
 METRIC_IN_SKAN_FROM_TRACKER = list(get_args(MetricInSkanFromTracker))
 
 def is_metric_in_skan_from_tracker(name: Union[str, MetricInSkanFromTracker]) -> bool:
     """
-    Check if `name` is a valid non-custom `MetricInSkanFromTracker` from **Singular**.
+    Check if `name` is a valid non-custom `MetricInSkanFromTracker` from Singular.
     """
     return name in METRIC_IN_SKAN_FROM_TRACKER
 
 
 MetricInSkanRaw = Literal[
     "skan_conversion_values_count",
     "skan_installs",
@@ -1457,15 +1468,15 @@
 
 MetricInSkanRawArgs = Union[Iterable[MetricInSkanRaw], str]
 
 METRIC_IN_SKAN_RAW = list(get_args(MetricInSkanRaw))
 
 def is_metric_in_skan_raw(name: Union[str, MetricInSkanRaw]) -> bool:
     """
-    Check if `name` is a valid non-custom `MetricInSkanRaw` from **Singular**.
+    Check if `name` is a valid non-custom `MetricInSkanRaw` from Singular.
     """
     return name in METRIC_IN_SKAN_RAW
 
 
 MetricInSkanRawFromNetwork = Literal[
     "skan_conversion_values_count",
     "skan_installs",
@@ -1473,15 +1484,15 @@
 
 MetricInSkanRawFromNetworkArgs = Union[Iterable[MetricInSkanRawFromNetwork], str]
 
 METRIC_IN_SKAN_RAW_FROM_NETWORK = list(get_args(MetricInSkanRawFromNetwork))
 
 def is_metric_in_skan_raw_from_network(name: Union[str, MetricInSkanRawFromNetwork]) -> bool:
     """
-    Check if `name` is a valid non-custom `MetricInSkanRawFromNetwork` from **Singular**.
+    Check if `name` is a valid non-custom `MetricInSkanRawFromNetwork` from Singular.
     """
     return name in METRIC_IN_SKAN_RAW_FROM_NETWORK
 
 
 MetricInSkanRawFromTracker = Literal[
     "skan_conversion_values_count",
     "skan_installs",
@@ -1489,15 +1500,15 @@
 
 MetricInSkanRawFromTrackerArgs = Union[Iterable[MetricInSkanRawFromTracker], str]
 
 METRIC_IN_SKAN_RAW_FROM_TRACKER = list(get_args(MetricInSkanRawFromTracker))
 
 def is_metric_in_skan_raw_from_tracker(name: Union[str, MetricInSkanRawFromTracker]) -> bool:
     """
-    Check if `name` is a valid non-custom `MetricInSkanRawFromTracker` from **Singular**.
+    Check if `name` is a valid non-custom `MetricInSkanRawFromTracker` from Singular.
     """
     return name in METRIC_IN_SKAN_RAW_FROM_TRACKER
 
 
 MetricInAdMon = Literal[
     "ad_clicks",
     "ad_impressions",
@@ -1513,15 +1524,15 @@
 
 MetricInAdMonArgs = Union[Iterable[MetricInAdMon], str]
 
 METRIC_IN_AD_MON = list(get_args(MetricInAdMon))
 
 def is_metric_in_ad_mon(name: Union[str, MetricInAdMon]) -> bool:
     """
-    Check if `name` is a valid non-custom `MetricInAdMon` from **Singular**.
+    Check if `name` is a valid non-custom `MetricInAdMon` from Singular.
     """
     return name in METRIC_IN_AD_MON
 
 
 MetricInAdMonFromNetwork = Literal[
     "ad_clicks",
     "ad_impressions",
@@ -1537,15 +1548,15 @@
 
 MetricInAdMonFromNetworkArgs = Union[Iterable[MetricInAdMonFromNetwork], str]
 
 METRIC_IN_AD_MON_FROM_NETWORK = list(get_args(MetricInAdMonFromNetwork))
 
 def is_metric_in_ad_mon_from_network(name: Union[str, MetricInAdMonFromNetwork]) -> bool:
     """
-    Check if `name` is a valid non-custom `MetricInAdMonFromNetwork` from **Singular**.
+    Check if `name` is a valid non-custom `MetricInAdMonFromNetwork` from Singular.
     """
     return name in METRIC_IN_AD_MON_FROM_NETWORK
 
 
 MetricInAdMonFromTracker = Literal[
     "ad_clicks",
     "ad_impressions",
@@ -1561,15 +1572,15 @@
 
 MetricInAdMonFromTrackerArgs = Union[Iterable[MetricInAdMonFromTracker], str]
 
 METRIC_IN_AD_MON_FROM_TRACKER = list(get_args(MetricInAdMonFromTracker))
 
 def is_metric_in_ad_mon_from_tracker(name: Union[str, MetricInAdMonFromTracker]) -> bool:
     """
-    Check if `name` is a valid non-custom `MetricInAdMonFromTracker` from **Singular**.
+    Check if `name` is a valid non-custom `MetricInAdMonFromTracker` from Singular.
     """
     return name in METRIC_IN_AD_MON_FROM_TRACKER
 
 
 MetricFromNetwork = Literal[
     "ad_clicks",
     "ad_impressions",
@@ -1627,15 +1638,15 @@
 
 MetricFromNetworkArgs = Union[Iterable[MetricFromNetwork], str]
 
 METRIC_FROM_NETWORK = list(get_args(MetricFromNetwork))
 
 def is_metric_from_network(name: Union[str, MetricFromNetwork]) -> bool:
     """
-    Check if `name` is a valid non-custom `MetricFromNetwork` from **Singular**.
+    Check if `name` is a valid non-custom `MetricFromNetwork` from Singular.
     """
     return name in METRIC_FROM_NETWORK
 
 
 MetricFromTracker = Literal[
     "ad_clicks",
     "ad_impressions",
@@ -1693,15 +1704,15 @@
 
 MetricFromTrackerArgs = Union[Iterable[MetricFromTracker], str]
 
 METRIC_FROM_TRACKER = list(get_args(MetricFromTracker))
 
 def is_metric_from_tracker(name: Union[str, MetricFromTracker]) -> bool:
     """
-    Check if `name` is a valid non-custom `MetricFromTracker` from **Singular**.
+    Check if `name` is a valid non-custom `MetricFromTracker` from Singular.
     """
     return name in METRIC_FROM_TRACKER
 
 
 FieldInGeneral = Literal[
     "adn_account_id",
     "adn_account_name",
@@ -1737,15 +1748,15 @@
     "keyword_match_type",
     "adn_campaign_id",
     "adn_campaign_name",
     "adn_sub_campaign_id",
     "adn_sub_campaign_name",
     "install_app_store",
     "original_bid_amount",
-    "original_ metadata_currency",
+    "original_metadata_currency",
     "adn_original_currency",
     "os",
     "placement",
     "platform",
     "publisher_id",
     "publisher_site_id",
     "publisher_site_name",
@@ -1761,15 +1772,15 @@
     "sub_campaign_name",
     "tracking_url",
     "tracker_campaign_id",
     "tracker_campaign_name",
     "tracker_name",
     "tracker_source_name",
     "tracker_sub_campaign_id",
-    "tracker_sub_campaign_ name",
+    "tracker_sub_campaign_name",
     "adn_utc_offset",
     "admon_data_source",
     "data_connector_id",
     "data_connector_source_name",
     "data_connector_timestamp_utc",
     "data_connector_username",
     "singular_campaign_id",
@@ -1803,15 +1814,15 @@
 
 FieldInGeneralArgs = Union[Iterable[FieldInGeneral], str]
 
 FIELD_IN_GENERAL = list(get_args(FieldInGeneral))
 
 def is_field_in_general(name: Union[str, FieldInGeneral]) -> bool:
     """
-    Check if `name` is a valid non-custom `FieldInGeneral` from **Singular**.
+    Check if `name` is a valid non-custom `FieldInGeneral` from Singular.
     """
     return name in FIELD_IN_GENERAL
 
 
 FieldInGeneralFromNetwork = Literal[
     "adn_account_id",
     "adn_account_name",
@@ -1844,15 +1855,15 @@
     "keyword_match_type",
     "adn_campaign_id",
     "adn_campaign_name",
     "adn_sub_campaign_id",
     "adn_sub_campaign_name",
     "install_app_store",
     "original_bid_amount",
-    "original_ metadata_currency",
+    "original_metadata_currency",
     "adn_original_currency",
     "os",
     "placement",
     "platform",
     "publisher_id",
     "publisher_site_id",
     "publisher_site_name",
@@ -1904,15 +1915,15 @@
 
 FieldInGeneralFromNetworkArgs = Union[Iterable[FieldInGeneralFromNetwork], str]
 
 FIELD_IN_GENERAL_FROM_NETWORK = list(get_args(FieldInGeneralFromNetwork))
 
 def is_field_in_general_from_network(name: Union[str, FieldInGeneralFromNetwork]) -> bool:
     """
-    Check if `name` is a valid non-custom `FieldInGeneralFromNetwork` from **Singular**.
+    Check if `name` is a valid non-custom `FieldInGeneralFromNetwork` from Singular.
     """
     return name in FIELD_IN_GENERAL_FROM_NETWORK
 
 
 FieldInGeneralFromTracker = Literal[
     "app",
     "site_public_id",
@@ -1930,29 +1941,29 @@
     "country_field",
     "min_roas",
     "installer_source",
     "adn_sub_campaign_id",
     "adn_sub_campaign_name",
     "install_app_store",
     "original_bid_amount",
-    "original_ metadata_currency",
+    "original_metadata_currency",
     "os",
     "platform",
     "region_field",
     "retention",
     "source",
     "standardized_bid_strategy",
     "sub_campaign_id",
     "sub_campaign_name",
     "tracker_campaign_id",
     "tracker_campaign_name",
     "tracker_name",
     "tracker_source_name",
     "tracker_sub_campaign_id",
-    "tracker_sub_campaign_ name",
+    "tracker_sub_campaign_name",
     "admon_data_source",
     "data_connector_id",
     "data_connector_source_name",
     "data_connector_timestamp_utc",
     "data_connector_username",
     "singular_campaign_id",
     "frequency",
@@ -1985,15 +1996,15 @@
 
 FieldInGeneralFromTrackerArgs = Union[Iterable[FieldInGeneralFromTracker], str]
 
 FIELD_IN_GENERAL_FROM_TRACKER = list(get_args(FieldInGeneralFromTracker))
 
 def is_field_in_general_from_tracker(name: Union[str, FieldInGeneralFromTracker]) -> bool:
     """
-    Check if `name` is a valid non-custom `FieldInGeneralFromTracker` from **Singular**.
+    Check if `name` is a valid non-custom `FieldInGeneralFromTracker` from Singular.
     """
     return name in FIELD_IN_GENERAL_FROM_TRACKER
 
 
 FieldInCreative = Literal[
     "adn_account_id",
     "adn_account_name",
@@ -2039,15 +2050,15 @@
 
 FieldInCreativeArgs = Union[Iterable[FieldInCreative], str]
 
 FIELD_IN_CREATIVE = list(get_args(FieldInCreative))
 
 def is_field_in_creative(name: Union[str, FieldInCreative]) -> bool:
     """
-    Check if `name` is a valid non-custom `FieldInCreative` from **Singular**.
+    Check if `name` is a valid non-custom `FieldInCreative` from Singular.
     """
     return name in FIELD_IN_CREATIVE
 
 
 FieldInCreativeFromNetwork = Literal[
     "adn_account_id",
     "adn_account_name",
@@ -2091,15 +2102,15 @@
 
 FieldInCreativeFromNetworkArgs = Union[Iterable[FieldInCreativeFromNetwork], str]
 
 FIELD_IN_CREATIVE_FROM_NETWORK = list(get_args(FieldInCreativeFromNetwork))
 
 def is_field_in_creative_from_network(name: Union[str, FieldInCreativeFromNetwork]) -> bool:
     """
-    Check if `name` is a valid non-custom `FieldInCreativeFromNetwork` from **Singular**.
+    Check if `name` is a valid non-custom `FieldInCreativeFromNetwork` from Singular.
     """
     return name in FIELD_IN_CREATIVE_FROM_NETWORK
 
 
 FieldInCreativeFromTracker = Literal[
     "app",
     "unified_campaign_id",
@@ -2136,15 +2147,15 @@
 
 FieldInCreativeFromTrackerArgs = Union[Iterable[FieldInCreativeFromTracker], str]
 
 FIELD_IN_CREATIVE_FROM_TRACKER = list(get_args(FieldInCreativeFromTracker))
 
 def is_field_in_creative_from_tracker(name: Union[str, FieldInCreativeFromTracker]) -> bool:
     """
-    Check if `name` is a valid non-custom `FieldInCreativeFromTracker` from **Singular**.
+    Check if `name` is a valid non-custom `FieldInCreativeFromTracker` from Singular.
     """
     return name in FIELD_IN_CREATIVE_FROM_TRACKER
 
 
 FieldInSkan = Literal[
     "app",
     "unified_campaign_id",
@@ -2173,15 +2184,15 @@
 
 FieldInSkanArgs = Union[Iterable[FieldInSkan], str]
 
 FIELD_IN_SKAN = list(get_args(FieldInSkan))
 
 def is_field_in_skan(name: Union[str, FieldInSkan]) -> bool:
     """
-    Check if `name` is a valid non-custom `FieldInSkan` from **Singular**.
+    Check if `name` is a valid non-custom `FieldInSkan` from Singular.
     """
     return name in FIELD_IN_SKAN
 
 
 FieldInSkanFromNetwork = Literal[
     "app",
     "unified_campaign_id",
@@ -2210,15 +2221,15 @@
 
 FieldInSkanFromNetworkArgs = Union[Iterable[FieldInSkanFromNetwork], str]
 
 FIELD_IN_SKAN_FROM_NETWORK = list(get_args(FieldInSkanFromNetwork))
 
 def is_field_in_skan_from_network(name: Union[str, FieldInSkanFromNetwork]) -> bool:
     """
-    Check if `name` is a valid non-custom `FieldInSkanFromNetwork` from **Singular**.
+    Check if `name` is a valid non-custom `FieldInSkanFromNetwork` from Singular.
     """
     return name in FIELD_IN_SKAN_FROM_NETWORK
 
 
 FieldInSkanFromTracker = Literal[
     "app",
     "unified_campaign_id",
@@ -2247,15 +2258,15 @@
 
 FieldInSkanFromTrackerArgs = Union[Iterable[FieldInSkanFromTracker], str]
 
 FIELD_IN_SKAN_FROM_TRACKER = list(get_args(FieldInSkanFromTracker))
 
 def is_field_in_skan_from_tracker(name: Union[str, FieldInSkanFromTracker]) -> bool:
     """
-    Check if `name` is a valid non-custom `FieldInSkanFromTracker` from **Singular**.
+    Check if `name` is a valid non-custom `FieldInSkanFromTracker` from Singular.
     """
     return name in FIELD_IN_SKAN_FROM_TRACKER
 
 
 FieldInSkanRaw = Literal[
     "app",
     "skan_conversion_value",
@@ -2274,15 +2285,15 @@
 
 FieldInSkanRawArgs = Union[Iterable[FieldInSkanRaw], str]
 
 FIELD_IN_SKAN_RAW = list(get_args(FieldInSkanRaw))
 
 def is_field_in_skan_raw(name: Union[str, FieldInSkanRaw]) -> bool:
     """
-    Check if `name` is a valid non-custom `FieldInSkanRaw` from **Singular**.
+    Check if `name` is a valid non-custom `FieldInSkanRaw` from Singular.
     """
     return name in FIELD_IN_SKAN_RAW
 
 
 FieldInSkanRawFromNetwork = Literal[
     "app",
     "skan_conversion_value",
@@ -2301,15 +2312,15 @@
 
 FieldInSkanRawFromNetworkArgs = Union[Iterable[FieldInSkanRawFromNetwork], str]
 
 FIELD_IN_SKAN_RAW_FROM_NETWORK = list(get_args(FieldInSkanRawFromNetwork))
 
 def is_field_in_skan_raw_from_network(name: Union[str, FieldInSkanRawFromNetwork]) -> bool:
     """
-    Check if `name` is a valid non-custom `FieldInSkanRawFromNetwork` from **Singular**.
+    Check if `name` is a valid non-custom `FieldInSkanRawFromNetwork` from Singular.
     """
     return name in FIELD_IN_SKAN_RAW_FROM_NETWORK
 
 
 FieldInSkanRawFromTracker = Literal[
     "app",
     "skan_conversion_value",
@@ -2328,15 +2339,15 @@
 
 FieldInSkanRawFromTrackerArgs = Union[Iterable[FieldInSkanRawFromTracker], str]
 
 FIELD_IN_SKAN_RAW_FROM_TRACKER = list(get_args(FieldInSkanRawFromTracker))
 
 def is_field_in_skan_raw_from_tracker(name: Union[str, FieldInSkanRawFromTracker]) -> bool:
     """
-    Check if `name` is a valid non-custom `FieldInSkanRawFromTracker` from **Singular**.
+    Check if `name` is a valid non-custom `FieldInSkanRawFromTracker` from Singular.
     """
     return name in FIELD_IN_SKAN_RAW_FROM_TRACKER
 
 
 FieldInAdMon = Literal[
     "instance_id",
     "instance_name",
@@ -2361,15 +2372,15 @@
 
 FieldInAdMonArgs = Union[Iterable[FieldInAdMon], str]
 
 FIELD_IN_AD_MON = list(get_args(FieldInAdMon))
 
 def is_field_in_ad_mon(name: Union[str, FieldInAdMon]) -> bool:
     """
-    Check if `name` is a valid non-custom `FieldInAdMon` from **Singular**.
+    Check if `name` is a valid non-custom `FieldInAdMon` from Singular.
     """
     return name in FIELD_IN_AD_MON
 
 
 FieldInAdMonFromNetwork = Literal[
     "instance_id",
     "instance_name",
@@ -2394,15 +2405,15 @@
 
 FieldInAdMonFromNetworkArgs = Union[Iterable[FieldInAdMonFromNetwork], str]
 
 FIELD_IN_AD_MON_FROM_NETWORK = list(get_args(FieldInAdMonFromNetwork))
 
 def is_field_in_ad_mon_from_network(name: Union[str, FieldInAdMonFromNetwork]) -> bool:
     """
-    Check if `name` is a valid non-custom `FieldInAdMonFromNetwork` from **Singular**.
+    Check if `name` is a valid non-custom `FieldInAdMonFromNetwork` from Singular.
     """
     return name in FIELD_IN_AD_MON_FROM_NETWORK
 
 
 FieldInAdMonFromTracker = Literal[
     "instance_id",
     "instance_name",
@@ -2427,15 +2438,15 @@
 
 FieldInAdMonFromTrackerArgs = Union[Iterable[FieldInAdMonFromTracker], str]
 
 FIELD_IN_AD_MON_FROM_TRACKER = list(get_args(FieldInAdMonFromTracker))
 
 def is_field_in_ad_mon_from_tracker(name: Union[str, FieldInAdMonFromTracker]) -> bool:
     """
-    Check if `name` is a valid non-custom `FieldInAdMonFromTracker` from **Singular**.
+    Check if `name` is a valid non-custom `FieldInAdMonFromTracker` from Singular.
     """
     return name in FIELD_IN_AD_MON_FROM_TRACKER
 
 
 FieldFromNetwork = Literal[
     "adn_account_id",
     "adn_account_name",
@@ -2489,15 +2500,15 @@
     "adn_creative_id",
     "adn_creative_name",
     "adn_sub_campaign_id",
     "adn_sub_campaign_name",
     "creative_type",
     "install_app_store",
     "original_bid_amount",
-    "original_ metadata_currency",
+    "original_metadata_currency",
     "adn_original_currency",
     "os",
     "placement",
     "platform",
     "publisher_id",
     "publisher_site_id",
     "publisher_site_name",
@@ -2592,15 +2603,15 @@
 
 FieldFromNetworkArgs = Union[Iterable[FieldFromNetwork], str]
 
 FIELD_FROM_NETWORK = list(get_args(FieldFromNetwork))
 
 def is_field_from_network(name: Union[str, FieldFromNetwork]) -> bool:
     """
-    Check if `name` is a valid non-custom `FieldFromNetwork` from **Singular**.
+    Check if `name` is a valid non-custom `FieldFromNetwork` from Singular.
     """
     return name in FIELD_FROM_NETWORK
 
 
 FieldFromTracker = Literal[
     "instance_id",
     "instance_name",
@@ -2635,15 +2646,15 @@
     "min_roas",
     "installer_source",
     "adn_sub_campaign_id",
     "adn_sub_campaign_name",
     "creative_type",
     "install_app_store",
     "original_bid_amount",
-    "original_ metadata_currency",
+    "original_metadata_currency",
     "os",
     "platform",
     "region_field",
     "skan_redownloads",
     "retention",
     "skan_app_id",
     "skan_campaign_id",
@@ -2657,15 +2668,15 @@
     "tracker_campaign_id",
     "tracker_campaign_name",
     "tracker_creative_id",
     "tracker_creative_name",
     "tracker_name",
     "tracker_source_name",
     "tracker_sub_campaign_id",
-    "tracker_sub_campaign_ name",
+    "tracker_sub_campaign_name",
     "utm_campaign",
     "utm_content",
     "utm_medium",
     "utm_source",
     "utm_term",
     "skan_validated",
     "admon_data_source",
@@ -2735,12 +2746,175 @@
 
 FieldFromTrackerArgs = Union[Iterable[FieldFromTracker], str]
 
 FIELD_FROM_TRACKER = list(get_args(FieldFromTracker))
 
 def is_field_from_tracker(name: Union[str, FieldFromTracker]) -> bool:
     """
-    Check if `name` is a valid non-custom `FieldFromTracker` from **Singular**.
+    Check if `name` is a valid non-custom `FieldFromTracker` from Singular.
     """
     return name in FIELD_FROM_TRACKER
 
 
+FIELD_MAPPING = dict(
+    adn_account_id="Account ID",
+    adn_account_name="Account Name",
+    instance_id="Ad Instance ID",
+    instance_name="Ad Instance Name",
+    source="Source",
+    ad_placement_id="Ad PlacementPlacement: A field in Singular reporting that says where/when the ad was displayed in the website/app (the precise meaning varies between networks). Not to be confused with Ad Placement (which is an Ad Mon-specific dimension). ID",
+    ad_placement_name="Ad Placement Name",
+    ad_type_id="Ad Type ID",
+    ad_type_name="Ad Type Name",
+    affiliate_id="Affiliate ID",
+    affiliate_name="Affiliate Name",
+    app="App",
+    site_public_id="App ID",
+    asset_id="Asset ID",
+    asset_name="Asset Name",
+    opt_in="ATT opt in",
+    banner_name="Banner Name",
+    bid_amount="Bid Amount",
+    bid_strategy="Bid Strategy",
+    bid_type="Bid Type",
+    unified_campaign_id="Campaign ID",
+    unified_campaign_name="Campaign Name",
+    campaign_objective="Campaign Objective",
+    campaign_status="Campaign Status",
+    adn_campaign_url="Campaign URL",
+    city_field="City",
+    adn_click_type="Click Type",
+    conversion_type="Conversion Type",
+    skan_conversion_value="Conversion ValueConversion Value: A single number between 0 and 63 included in an SKAdNetwork postback. The conversion value is the only way to get any information about an install and the user's post-install activity in the SKAdNetwork framework. Learn more",
+    skan_conversion_value_description="Conversion Value Description",
+    country_field="Country",
+    ad_country="Country",
+    creative_format="Creative Format",
+    creative_height="Creative Height",
+    creative_id="Creative ID",
+    creative_name="Creative Name",
+    creative_reported_url="Creative Reported URL",
+    creative_width="Creative Width",
+    device_model="Device Model",
+    dma_id_field="DMA ID",
+    dma_name_field="DMA Name",
+    fb_adset_id="Facebook Ad Set ID",
+    fb_campaign_id="Facebook Campaign ID",
+    min_roas="Facebook ROAS Bid",
+    final_url="Final URL",
+    installer_source="Installer Source",
+    is_uac="Is UAC",
+    keyword="Keyword",
+    keyword_id="Keyword ID",
+    keyword_match_type="Keyword Match Type",
+    adn_campaign_id="Network Campaign ID",
+    adn_campaign_name="Network Campaign Name",
+    adn_creative_id="Network Creative ID",
+    adn_creative_name="Network Creative Name",
+    adn_sub_campaign_id="Network Sub Campaign ID",
+    adn_sub_campaign_name="Network Sub Campaign Name",
+    creative_type="Normalized Creative Type",
+    install_app_store="Normalized Installer Source",
+    original_bid_amount="Original Bid Amount",
+    original_metadata_currency="Original Bid Currency",
+    adn_original_currency="Original Currency",
+    os="OS",
+    placement="Placement",
+    platform="Platform",
+    publisher_id="Publisher ID",
+    publisher_site_id="Publisher Site ID",
+    publisher_site_name="Publisher Site Name",
+    quality_score="Quality ScoreQuality Score: A field in Singular reporting that contains the rating for the quality of ad content and landing pages, as compared to advertisers. Learn more in the Metrics and Dimensions Glossary",
+    region_field="Region",
+    skan_redownloads="Re-Downloads",
+    retention="RetargetingRetargeting: A type of mobile marketing campaign that targets existing users of an app/website and aims to get them to re-engage with the product. Learn more",
+    skan_app_id="SKANSKAN: Singular's SKAdNetwork solution, offering smart conversion value management that can be configured through the Singular app. Learn more  App ID",
+    skan_campaign_id="SKAN Campaign ID",
+    skan_network_id="SKAN Network ID",
+    skan_publisher_id="SKAN Publisher ID",
+    standardized_bid_strategy="Standardized Bid Strategy",
+    standardized_bid_type="Standardized Bid Type",
+    adn_status="Status",
+    adn_subadnetwork="Sub Ad Network",
+    sub_campaign_id="Sub Campaign ID",
+    sub_campaign_name="Sub Campaign Name",
+    creative_text="Text",
+    tracking_url="Tracking URL",
+    tracker_campaign_id="Tracker Campaign ID",
+    tracker_campaign_name="Tracker Campaign Name",
+    tracker_creative_id="Tracker Creative ID",
+    tracker_creative_name="Tracker Creative Name",
+    tracker_name="Tracker Name",
+    tracker_source_name="Tracker Source Name",
+    tracker_sub_campaign_id="Tracker Sub Campaign ID",
+    tracker_sub_campaign_name="Tracker Sub Campaign Name",
+    adn_utc_offset="UTC Offset",
+    utm_campaign="UTM Campaign",
+    utm_content="UTM Content",
+    utm_medium="UTM Medium",
+    utm_source="UTM Source",
+    utm_term="UTM Term",
+    skan_validated="Validated",
+    admon_data_source="nan",
+    creative_hash="nan",
+    creative_is_video="nan",
+    creative_url="nan",
+    creative_image_hash="nan",
+    data_connector_id="nan",
+    data_connector_source_name="nan",
+    data_connector_timestamp_utc="nan",
+    data_connector_username="nan",
+    singular_campaign_id="nan",
+    singular_creative_id="nan",
+    ad_clicks="Ad Clicks",
+    ad_impressions="Ad Impressions",
+    ad_requests="Ad Requests",
+    ad_revenue="Ad Revenue",
+    frequency="Average Frequency",
+    bid_requests="Bid Requests",
+    bid_responses="Bid Responses",
+    custom_clicks="Clicks",
+    skan_report_network_clicks="Clicks",
+    clicks_discrepancy="Clicks Discrepancy",
+    adn_comments="Comments",
+    completed_video_views="Completed Video Views",
+    ad_completed_video_views="Completed Video Views",
+    skan_conversion_values_count="Conversion Values - Count",
+    adn_cost="Cost",
+    daily_active_users="DAU",
+    adn_estimated_total_conversions="Est. Conversions",
+    skan_estimated_revenue="Estimated Revenue",
+    skan_estimated_ROI="Estimated ROI",
+    filled_ad_requests="Filled Ad Requests",
+    custom_impressions="Impressions",
+    skan_report_network_impressions="Impressions",
+    impressions_discrepancy="Impressions Discrepancy",
+    custom_installs="Installs",
+    installs_discrepancy="Installs Discrepancy",
+    adn_likes="Likes",
+    adn_clicks="Network Clicks",
+    adn_impressions="Network Impressions",
+    adn_installs="Network Installs",
+    new_visitors="New Visitors",
+    adn_original_cost="Original Cost",
+    original_revenue="Original Revenue",
+    page_follows="Page Follows",
+    posts_saved="Posts saved",
+    re_engaged_visitors="Re-engaged Visitors",
+    tracker_reengagements="Re-Engagements",
+    reach="Reach",
+    revenue="Revenue",
+    adn_shares="Shares",
+    skan_installs="SKAN Installs",
+    skan_revenue="SKAN Revenue",
+    skan_roi="SKAN ROI",
+    total_revenue="Total Revenue",
+    total_web_conversions="Total Web Conversions",
+    tracker_clicks="Tracker Clicks",
+    tracker_installs="Tracker Installs",
+    video_views="Video Views",
+    ad_video_views="Video Views",
+    video_views_25pct="Video Views 25%",
+    video_views_50pct="Video Views 50%",
+    video_views_75pct="Video Views 75%",
+)
+
```

### Comparing `singular_client-0.1.4/singular_client/documents.py` & `singular_client-0.1.5/singular_client/documents.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 """
 Data structures returned by Singular API.
 
 --------------------------------------------------------------------------------
 USED FOR STATIC TYPE CHECKING ONLY. Do not create instances of these classes.
 --------------------------------------------------------------------------------
 
+Endpoints are type-hinted using these classes as the structure of an individual
+document within a list of documents in a response. They serve two purposes:
+1. Easy access by the user for referencing the expected response data structure
+2. Static type checking. The user's IDE will bark at them or give red underline
+   if they try to access an attribute from a response that is not present.
+
 Tip: Github Copilot will write these for you (including the class name) if you
-paste an example json from documentation into a comment block above the class
+paste an example json from documentation into a comment block above the class.
 """
 from typing import TypedDict, List, Optional, Literal, Union, Dict
 
 
 class NameDoc(TypedDict):
     display_name: str
     name: str
```

### Comparing `singular_client-0.1.4/singular_client/endpoints/links.py` & `singular_client-0.1.5/singular_client/endpoints/links.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,40 +7,31 @@
 
 class DomainsEndpoint(_Endpoint[ResponseDocList[DomainDoc]]):
     endpoint = "v1/singular_links/domains"
     data_path = ["available_domains"]
     res_type = ResponseDocList[DomainDoc]
 
 
-# ==============================================================================
-
-
 class AppsEndpoint(_Endpoint[ResponseDocList[AppDoc]]):
     endpoint = "v1/singular_links/apps"
     data_path = ["available_apps"]
     res_type = ResponseDocList[AppDoc]
 
 
-# ==============================================================================
-
-
 class AllPartnersEndpoint(_Endpoint[ResponseDocList[PartnerDoc]]):
     endpoint = "v1/singular_links/all_partners"
     data_path = ["partners"]
     res_type = ResponseDocList[PartnerDoc]
 
     def request(self, singular_partner_id: Optional[List[str]] = None):
         return super().request(
             singular_partner_id=_convert_list_arg(singular_partner_id)
         )
 
 
-# ==============================================================================
-
-
 class CreateLinkEndpoint(_Endpoint[CreateLinkDoc]):
     endpoint = "v1/singular_links/links"
     data_path = []
     res_type = CreateLinkDoc
     returns_collection = False
     method = "POST"
 
@@ -105,17 +96,14 @@
                 view_probabilistic_window=view_probabilistic_window,
                 click_reengagement_window=click_reengagement_window,
                 enable_ctv=enable_ctv,
             ),
         )
 
 
-# ==============================================================================
-
-
 class ViewLinksEndpoint(_Endpoint[ResponseDocList[LinkDoc]]):
     endpoint = "v1/singular_links/links"
     data_path = []
     res_type = ResponseDocList[LinkDoc]
 
     def request(
         self,
@@ -130,17 +118,14 @@
             partner_id=partner_id,
             app_id=app_id,
             app_site_id=app_site_id,
             tracking_link_id=tracking_link_id,
         )
 
 
-# ==============================================================================
-
-
 class ConfiguredPartnersEndpoint(_Endpoint[ResponseDocList[PartnerAppDoc]]):
     endpoint = "v1/singular_links/configured_partners"
     data_path = ["available_partners"]
     res_type = ResponseDocList[PartnerAppDoc]
 
     def request(
         self,
```

### Comparing `singular_client-0.1.4/singular_client/endpoints/links_legacy.py` & `singular_client-0.1.5/singular_client/endpoints/links_legacy.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.4/singular_client/endpoints/monetization.py` & `singular_client-0.1.5/singular_client/endpoints/monetization.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.4/singular_client/endpoints/reporting.py` & `singular_client-0.1.5/singular_client/endpoints/reporting.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,65 @@
+"""
+General Async Reporting Endpoints
+=================================
+
+Async reporting for network and tracker data. Includes a variety of
+helper-endpoints to quickly retrieve the information needed to make an async reporting
+request.
+
+Once you're ready to create a report, here is some example code:
+```
+api = SingularAPI(<api key>)
+report_queue = api.combined_report(...)
+while not (status := report_queue.check_status()):
+    time.sleep(10)
+if status.failed:
+    raise Exception("Report failed")
+data = status.read()
+```
+
+https://support.singular.net/hc/en-us/articles/360045245692-Reporting-API-Reference?navigation_side_bar=true
+"""
 from singular_client._bases import _Endpoint, ResponseDocList
 from singular_client.documents import *
 from singular_client.arguments import *
+from singular_client.fields import *
 from singular_client.utils import _convert_list_arg
 import json
 import time
 import requests
 import io
 from typing import *
 
 if TYPE_CHECKING:
     from singular_client.api import SingularAPI
     import pandas as pd
 
 
 class ReportStatusResponse:
+    """
+    Returned by a check on the status of a report, through the ReportStatusEndpoint,
+    or indirectly, through the CreateReportResponse object.
+
+    Its boolean value is True if the report is done, OR if it has failed.
+    """
     cached_download: Optional[Union[requests.Response, "pd.DataFrame"]]
-    status: ReportStatusDoc
+    raw: ReportStatusDoc
     failed = property(lambda x: x.status["status"] == "FAILED")
     done = property(lambda x: x.status["status"] == "DONE")
     queued = property(lambda x: x.status["status"] == "QUEUED")
     started = property(lambda x: x.status["status"] == "STARTED")
     url = property(lambda x: x.status["download_url"])
 
     def __init__(self, doc: dict):
-        self.status = cast(ReportStatusDoc, doc)
+        self.raw = cast(ReportStatusDoc, doc)
         self.cached_download = None
 
     def __bool__(self) -> bool:
-        return self.done
+        return self.done or self.failed
 
     def read(self, no_cache: bool = False) -> Optional[Union[dict, "pd.DataFrame"]]:
         """
         Download from `status['download_url']`, and read the report without knowing
         whether it is a json or csv report.
         ---
         - If csv, pandas is required.
@@ -39,15 +67,15 @@
         """
         if not self:
             return None
 
         if self.cached_download and not no_cache:
             res = self.cached_download
         else:
-            res = requests.get(self.status["download_url"])
+            res = requests.get(self.raw["download_url"])
             self.cached_download = res
         try:
             return res.json()
         except json.JSONDecodeError:
             try:
                 import pandas as pd
             except ImportError:
@@ -62,15 +90,14 @@
 
     - Rate limited to 1 request per 10 seconds, per report.
 
     Returns a ReportStatusResponse object, whose boolean value indicates
     whether the report is ready. If True, the report can be downloaded with
     its `.read()` method.
     """
-
     endpoint = "v2.0/get_report_status"
     data_path = ["value"]
     res_type = ReportStatusResponse
     cacheable = False
     request_times: Dict[str, float] = {}
     returns_collection = False
     report_id: str
@@ -96,15 +123,15 @@
     endpoint = "cohort_metrics"
     data_path = ["value"]
     res_type = CohortMetricsDoc
     returns_collection = False
 
 
 class CustomDimensionsEndpoint(_Endpoint[ResponseDocList[IDDoc]]):
-    endpoint = "v2.0/reporting/filters"
+    endpoint = "custom_dimensions"
     data_path = ["value", "custom_dimensions"]
     res_type = ResponseDocList[IDDoc]
 
 
 class ConversionMetricsEndpoint(_Endpoint[ResponseDocList[NameDoc]]):
     endpoint = "conversion_metrics"
     data_path = ["value", "metrics"]
@@ -114,16 +141,16 @@
 class DataAvailabilityEndpoint(_Endpoint[ResponseDocList[DataConnectorDoc]]):
     endpoint = "v2.0/data_availability_status"
     data_path = ["value", "data_connectors"]
     res_type = ResponseDocList[DataConnectorDoc]
 
     def request(
         self,
-        format: str,
         data_date: str,
+        format: Literal['json', 'csv'] = 'json',
         expanded: bool = True,
         display_non_active_sources: bool = False,
     ):
         return super().request(
             format=format,
             data_date=data_date,
             expanded=expanded,
@@ -132,22 +159,32 @@
 
 
 # ==============================================================================
 
 
 class CreateReportResponse(str):
     api: "SingularAPI"
+    # Response gets cached whent the report has failed or completed,
+    # so requests can no longer be sent after that.
+    cached_status: Optional[ReportStatusResponse]
 
     def check_status(
         self, api: Optional["SingularAPI"] = None
     ) -> Optional[ReportStatusResponse]:
+        if hasattr(self, "cached_status") and self.cached_status:
+            return self.cached_status
+
         assert api or self.api, "An API must be provided"
         if not api:
             api = self.api
-        return api.report_status.request(str(self))
+
+        status = api.report_status.request(str(self))
+        if status:
+            self.cached_status = status
+        return status
 
 
 DimensionType = TypeVar("DimensionType")
 MetricType = TypeVar("MetricType")
 
 
 class _AggReportEndpoint(
@@ -220,22 +257,20 @@
                 display_unenriched=display_unenriched,
             ),
         )
         report_id.api = self.api
         return report_id
 
 
-# class GeneralReportEndpoint(_AggReportEndpoint[DimensionInGeneral, MetricInGeneral]):
-
-class CombinedReportEndpoint(_AggReportEndpoint[CombinedDimension, CombinedMetric]):
+class CombinedReportEndpoint(_AggReportEndpoint[DimensionInGeneral, MetricInGeneral]):
     available_dimensions = COMBINED_DIMENSIONS
     available_metrics = COMBINED_METRICS
 
 
-class NetworkReportEndpoint(_AggReportEndpoint[NetworkDimension, NetworkMetric]):
+class NetworkReportEndpoint(_AggReportEndpoint[DimensionInGeneralFromNetwork, MetricInGeneralFromNetwork]):
     available_dimensions = NETWORK_DIMENSIONS
     available_metrics = NETWORK_METRICS
 
 
-class TrackerReportEndpoint(_AggReportEndpoint[TrackerDimension, TrackerMetric]):
+class TrackerReportEndpoint(_AggReportEndpoint[DimensionInGeneralFromTracker, MetricInGeneralFromTracker]):
     available_dimensions = TRACKER_DIMENSIONS
     available_metrics = TRACKER_METRICS
```

### Comparing `singular_client-0.1.4/singular_client/endpoints/skan.py` & `singular_client-0.1.5/singular_client/endpoints/skan.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,55 @@
+"""
+SKAN Reporting:
+    Skan Raw
+    Skan
+    Skan Events
+
+https://support.singular.net/hc/en-us/articles/360056377792-Singular-SKAdNetwork-API-Reference?navigation_side_bar=true#Create_Async_SKAdNetwork_Raw_Report_Endpoint
+"""
 from singular_client._bases import _Endpoint, ResponseDocList
 from singular_client.documents import *
 from singular_client.arguments import *
+from singular_client.fields import *
 from singular_client.endpoints.reporting import CreateReportResponse
 from typing import *
 from singular_client.utils import _convert_list_arg
 
 
 class SkanEventsEndpoint(_Endpoint[ResponseDocList[NameDoc]]):
+    """
+    Retrieve a list of available SKAN events for use in Create Async SKAdNetwork
+    Report queries. Events are displayed as "display_name" and "name" pairs.
+    """
     endpoint = "v2.0/skan_events"
     data_path = ["value", "skan_events"]
     res_type = ResponseDocList[NameDoc]
 
 
 class SkanRawReportEndpoint(_Endpoint[CreateReportResponse]):
+    """
+    Query an asynchronous report for raw SKAdNetwork data collected from postbacks.
+    This endpoint provides the number of SKAdNetwork conversions per network and app.
+    """
     endpoint = "v2.0/create_async_skadnetwork_raw_report"
     data_path = ["value", "report_id"]
     available_dimensions = SKAN_RAW_DIMENSIONS
     available_metrics = SKAN_RAW_METRICS
     res_type = CreateReportResponse
     returns_collection = False
     method = "POST"
 
     def request(
         self,
         start_date: str,
         time_breakdown: TimeBreakdown = "all",
         end_date: Optional[str] = None,
         skadnetwork_date_type: SkadDateType = "skan_postback_date",
-        dimensions: Optional[Union[List[SkanRawDimension], str]] = None,
-        metrics: Optional[Union[List[SkanRawMetric], str]] = None,
+        dimensions: Optional[Union[List[DimensionInSkanRaw], str]] = None,
+        metrics: Optional[Union[List[MetricInSkanRaw], str]] = None,
         app: Optional[List[str]] = None,
         source: Optional[List[str]] = None,
         filters: Optional[List[dict]] = None,
         format: FileFormat = "csv",
         country_code_format: CountryCodeFormat = "iso3",
     ):
         report_id = super().request(
@@ -51,30 +68,35 @@
             ),
         )
         report_id.api = self.api
         return report_id
 
 
 class SkanReportEndpoint(_Endpoint[CreateReportResponse]):
+    """
+    Generate an asynchronous report query for SKAdNetwork data combined with ad network
+    and tracker data. Use it to measure metrics like CPI, click-through rate,
+    etc., for SKAdNetwork campaigns, grouped by network and/or campaign.
+    """
     endpoint = "v2.0/create_async_skadnetwork_report"
     data_path = ["value", "report_id"]
     res_type = CreateReportResponse
     available_dimensions = SKAN_DIMENSIONS
     available_metrics = SKAN_METRICS
     returns_collection = False
     method = "POST"
 
     def request(
         self,
         start_date: str,
         time_breakdown: TimeBreakdown = "all",
         end_date: Optional[str] = None,
         skadnetwork_date_type: SkadDateType = "skan_postback_date",
-        dimensions: Optional[Union[List[SkanDimension], str]] = None,
-        metrics: Optional[Union[List[SkanMetric], str]] = None,
+        dimensions: Optional[Union[List[DimensionInSkan], str]] = None,
+        metrics: Optional[Union[List[MetricInSkan], str]] = None,
         skan_events: Optional[List[str]] = None,
         format: FileFormat = "csv",
     ):
         report_id = super().request(
             data=dict(
                 start_date=start_date,
                 end_date=end_date or start_date,
```

### Comparing `singular_client-0.1.4/pyproject.toml` & `singular_client-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "singular-client"
-version = "0.1.4"
+version = "0.1.5"
 python_requires = ">=3.8"
 description = "A modern Singular API client, with rigorous static type checking."
 authors = [
     {name = "Ryan Young", email = "dev@ryayoung.com"}
 ]
 readme = "README.md"
 license = "MIT"
```

### Comparing `singular_client-0.1.4/PKG-INFO` & `singular_client-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singular-client
-Version: 0.1.4
+Version: 0.1.5
 Summary: A modern Singular API client, with rigorous static type checking.
 Author-email: Ryan Young <dev@ryayoung.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
```

