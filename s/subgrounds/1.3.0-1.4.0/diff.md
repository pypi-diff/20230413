# Comparing `tmp/subgrounds-1.3.0.tar.gz` & `tmp/subgrounds-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subgrounds-1.3.0.tar", max compression
+gzip compressed data, was "subgrounds-1.4.0.tar", max compression
```

## Comparing `subgrounds-1.3.0.tar` & `subgrounds-1.4.0.tar`

### file list

```diff
@@ -1,26 +1,33 @@
--rw-r--r--   0        0        0    11347 2023-04-07 18:51:29.779610 subgrounds-1.3.0/LICENSE
--rw-r--r--   0        0        0     8929 2023-04-07 18:51:29.779610 subgrounds-1.3.0/README.md
--rw-r--r--   0        0        0     1601 2023-04-07 18:51:52.139923 subgrounds-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      224 2023-04-07 18:51:52.123922 subgrounds-1.3.0/subgrounds/__init__.py
--rw-r--r--   0        0        0     4521 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/client.py
--rw-r--r--   0        0        0     4260 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/dash_wrappers.py
--rw-r--r--   0        0        0    10062 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/dataframe_utils.py
--rw-r--r--   0        0        0      395 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/errors.py
--rw-r--r--   0        0        0     1027 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/pagination/__init__.py
--rw-r--r--   0        0        0     4761 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/pagination/pagination.py
--rw-r--r--   0        0        0    10550 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/pagination/preprocess.py
--rw-r--r--   0        0        0    17076 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/pagination/strategies.py
--rw-r--r--   0        0        0     1530 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/pagination/utils.py
--rw-r--r--   0        0        0     6789 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/plotly_wrappers.py
--rw-r--r--   0        0        0    62357 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/query.py
--rw-r--r--   0        0        0    12755 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/schema.py
--rw-r--r--   0        0        0      308 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/subgraph/__init__.py
--rw-r--r--   0        0        0    38895 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/subgraph/fieldpath.py
--rw-r--r--   0        0        0     1669 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/subgraph/filter.py
--rw-r--r--   0        0        0     4754 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/subgraph/object.py
--rw-r--r--   0        0        0     2552 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/subgraph/subgraph.py
--rw-r--r--   0        0        0    21569 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/subgrounds.py
--rw-r--r--   0        0        0    20072 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/transform.py
--rw-r--r--   0        0        0     6901 2023-04-07 18:51:29.783610 subgrounds-1.3.0/subgrounds/utils.py
--rw-r--r--   0        0        0    10111 1970-01-01 00:00:00.000000 subgrounds-1.3.0/setup.py
--rw-r--r--   0        0        0     9799 1970-01-01 00:00:00.000000 subgrounds-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11347 2023-04-13 19:53:11.640867 subgrounds-1.4.0/LICENSE
+-rw-r--r--   0        0        0     8929 2023-04-13 19:53:11.640867 subgrounds-1.4.0/README.md
+-rw-r--r--   0        0        0     1755 2023-04-13 19:54:49.857116 subgrounds-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      224 2023-04-13 19:54:49.833116 subgrounds-1.4.0/subgrounds/__init__.py
+-rw-r--r--   0        0        0     4521 2023-04-13 19:53:11.644868 subgrounds-1.4.0/subgrounds/client.py
+-rw-r--r--   0        0        0     1427 2023-04-13 19:53:11.644868 subgrounds-1.4.0/subgrounds/contrib/README.md
+-rw-r--r--   0        0        0      349 2023-04-13 19:53:11.644868 subgrounds-1.4.0/subgrounds/contrib/dash/__init__.py
+-rw-r--r--   0        0        0      399 2023-04-13 19:53:11.644868 subgrounds-1.4.0/subgrounds/contrib/dash/abcs.py
+-rw-r--r--   0        0        0     3893 2023-04-13 19:53:11.644868 subgrounds-1.4.0/subgrounds/contrib/dash/components.py
+-rw-r--r--   0        0        0     1285 2023-04-13 19:53:11.644868 subgrounds-1.4.0/subgrounds/contrib/plotly/__init__.py
+-rw-r--r--   0        0        0     1316 2023-04-13 19:53:11.644868 subgrounds-1.4.0/subgrounds/contrib/plotly/figure.py
+-rw-r--r--   0        0        0     5866 2023-04-13 19:53:11.644868 subgrounds-1.4.0/subgrounds/contrib/plotly/traces.py
+-rw-r--r--   0        0        0      438 2023-04-13 19:53:11.644868 subgrounds-1.4.0/subgrounds/dash_wrappers.py
+-rw-r--r--   0        0        0    10062 2023-04-13 19:53:11.644868 subgrounds-1.4.0/subgrounds/dataframe_utils.py
+-rw-r--r--   0        0        0      395 2023-04-13 19:53:11.644868 subgrounds-1.4.0/subgrounds/errors.py
+-rw-r--r--   0        0        0     1027 2023-04-13 19:53:11.644868 subgrounds-1.4.0/subgrounds/pagination/__init__.py
+-rw-r--r--   0        0        0     4761 2023-04-13 19:53:11.644868 subgrounds-1.4.0/subgrounds/pagination/pagination.py
+-rw-r--r--   0        0        0    10550 2023-04-13 19:53:11.644868 subgrounds-1.4.0/subgrounds/pagination/preprocess.py
+-rw-r--r--   0        0        0    17076 2023-04-13 19:53:11.644868 subgrounds-1.4.0/subgrounds/pagination/strategies.py
+-rw-r--r--   0        0        0     1530 2023-04-13 19:53:11.644868 subgrounds-1.4.0/subgrounds/pagination/utils.py
+-rw-r--r--   0        0        0     1460 2023-04-13 19:53:11.644868 subgrounds-1.4.0/subgrounds/plotly_wrappers.py
+-rw-r--r--   0        0        0    62357 2023-04-13 19:53:11.644868 subgrounds-1.4.0/subgrounds/query.py
+-rw-r--r--   0        0        0    12755 2023-04-13 19:53:11.644868 subgrounds-1.4.0/subgrounds/schema.py
+-rw-r--r--   0        0        0      308 2023-04-13 19:53:11.644868 subgrounds-1.4.0/subgrounds/subgraph/__init__.py
+-rw-r--r--   0        0        0    38895 2023-04-13 19:53:11.644868 subgrounds-1.4.0/subgrounds/subgraph/fieldpath.py
+-rw-r--r--   0        0        0     1669 2023-04-13 19:53:11.644868 subgrounds-1.4.0/subgrounds/subgraph/filter.py
+-rw-r--r--   0        0        0     4754 2023-04-13 19:53:11.644868 subgrounds-1.4.0/subgrounds/subgraph/object.py
+-rw-r--r--   0        0        0     2552 2023-04-13 19:53:11.644868 subgrounds-1.4.0/subgrounds/subgraph/subgraph.py
+-rw-r--r--   0        0        0    21574 2023-04-13 19:53:11.644868 subgrounds-1.4.0/subgrounds/subgrounds.py
+-rw-r--r--   0        0        0    20072 2023-04-13 19:53:11.644868 subgrounds-1.4.0/subgrounds/transform.py
+-rw-r--r--   0        0        0     6901 2023-04-13 19:53:11.644868 subgrounds-1.4.0/subgrounds/utils.py
+-rw-r--r--   0        0        0    10200 1970-01-01 00:00:00.000000 subgrounds-1.4.0/setup.py
+-rw-r--r--   0        0        0     9799 1970-01-01 00:00:00.000000 subgrounds-1.4.0/PKG-INFO
```

### Comparing `subgrounds-1.3.0/LICENSE` & `subgrounds-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `subgrounds-1.3.0/README.md` & `subgrounds-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `subgrounds-1.3.0/pyproject.toml` & `subgrounds-1.4.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "subgrounds"
-version = "1.3.0"
+version = "1.4.0"
 description = "A Pythonic data access layer for applications querying data from The Graph Network."
 authors = [
     "cvauclair <cvauclair@playgrounds.network>",
     "0xMochan <mochan@playgrounds.network>",
 ]
 repository = "https://github.com/0xPlaygrounds/subgrounds"
 
@@ -22,34 +22,40 @@
 
 [tool.poetry.extras]
 dash = ["dash"]
 
 # https://python-poetry.org/docs/managing-dependencies/#dependency-groups
 [tool.poetry.group.dev.dependencies]
 black = "^22.3.0"
-deepdiff = "^6.2.1"  # used for debugging data structures
+deepdiff = "^6.2.1"                 # used for debugging data structures
 ipykernel = "^6.13.0"
 mypy = "^0.950"
 nose2 = "^0.11.0"
 pytest = "^7.1.2"
 pytest-mock = "^3.8.2"
 python-semantic-release = "^7.33.1"
 ruff = "^0.0.253"
 
 [tool.poe.tasks]
-format = { shell = "black subgrounds examples tests"}
-check = { shell = "black subgrounds examples tests --check; ruff check subgrounds examples tests"}
+format = { shell = "black subgrounds examples tests" }
+check = { shell = "black subgrounds examples tests --check; ruff check subgrounds examples tests" }
 develop = { shell = "mudkip develop" }
 test = "pytest"
 generate-api-docs = { shell = "sphinx-apidoc --output docs/api subgrounds --separate --force" }
 
 [tool.semantic_release]
 branch = "main"
 upload_to_pypi = true
 version_variable = ["subgrounds/__init__.py:__version__"]
 version_toml = "pyproject.toml:tool.poetry.version"
 major_on_zero = false
 build_command = "poetry build"
 
+[tool.ruff]
+
+[tool.ruff.per-file-ignores]
+"subgrounds/plotly_wrappers" = ["F405", "F403"]
+"subgrounds/dash_wrappers" = ["F405", "F403"]
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `subgrounds-1.3.0/subgrounds/client.py` & `subgrounds-1.4.0/subgrounds/client.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.3.0/subgrounds/dash_wrappers.py` & `subgrounds-1.4.0/subgrounds/contrib/dash/components.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,20 @@
 from __future__ import annotations
 
-from abc import ABC, abstractmethod
-from typing import Any, ClassVar, Optional
+from typing import Any, ClassVar
 
 import pandas as pd
 from dash import dash_table, dcc, html
 from dash.dependencies import Input, Output
 from pipe import map, where
 
-from subgrounds.plotly_wrappers import Figure
-from subgrounds.subgraph import FieldPath
-from subgrounds.subgrounds import Subgrounds
+from subgrounds import FieldPath, Subgrounds
+from subgrounds.contrib.plotly import Figure
 
-
-class Refreshable(ABC):
-    @property
-    @abstractmethod
-    def dash_dependencies(self) -> list[Output]:
-        raise NotImplementedError
-
-    @property
-    @abstractmethod
-    def dash_dependencies_outputs(self) -> list[Any]:
-        raise NotImplementedError
+from .abcs import Refreshable
 
 
 class Graph(dcc.Graph, Refreshable):
     counter: ClassVar[int] = 0
     wrapped_figure: Figure
 
     def __init__(self, fig: Figure, **kwargs) -> None:
@@ -45,24 +33,24 @@
 
 
 class DataTable(dash_table.DataTable, Refreshable):
     counter: ClassVar[int] = 0
 
     subgrounds: Subgrounds
     data: list[FieldPath]
-    columns: Optional[list[str]]
+    columns: list[str] | None
     concat: bool
     append: bool
-    df: Optional[pd.DataFrame | list[pd.DataFrame]]
+    df: pd.DataFrame | list[pd.DataFrame] | None
 
     def __init__(
         self,
         subgrounds: Subgrounds,
         data: FieldPath | list[FieldPath],
-        columns: Optional[list[str]] = None,
+        columns: list[str] | None = None,
         concat: bool = False,
         append: bool = False,
         **kwargs,
     ):
         self.subgrounds = subgrounds
         self.fpaths = data if type(data) == list else [data]
         self.column_names = columns
@@ -118,16 +106,16 @@
                 *children,
             ],
             **kwargs,
         )
 
         AutoUpdate.counter += 1
 
-        def flatten(l):
-            return [item for sublist in l for item in sublist]
+        def flatten(input: list[Any]):
+            return [item for sublist in input for item in sublist]
 
         subgrounds_children = list(
             children | where(lambda child: isinstance(child, Refreshable))
         )
         deps = flatten(
             list(subgrounds_children | map(lambda child: child.dash_dependencies))
         )
@@ -136,14 +124,11 @@
             outputs = flatten(
                 list(
                     subgrounds_children
                     | map(lambda child: child.dash_dependencies_outputs)
                 )
             )
 
-            if len(outputs) == 1:
-                return outputs[0]
-            else:
-                return outputs
+            return outputs[0] if len(outputs) == 1 else outputs
 
         # Register callback
         app.callback(*deps, Input(id, "n_intervals"))(update)
```

### Comparing `subgrounds-1.3.0/subgrounds/dataframe_utils.py` & `subgrounds-1.4.0/subgrounds/dataframe_utils.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.3.0/subgrounds/pagination/__init__.py` & `subgrounds-1.4.0/subgrounds/pagination/__init__.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.3.0/subgrounds/pagination/pagination.py` & `subgrounds-1.4.0/subgrounds/pagination/pagination.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.3.0/subgrounds/pagination/preprocess.py` & `subgrounds-1.4.0/subgrounds/pagination/preprocess.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.3.0/subgrounds/pagination/strategies.py` & `subgrounds-1.4.0/subgrounds/pagination/strategies.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.3.0/subgrounds/pagination/utils.py` & `subgrounds-1.4.0/subgrounds/pagination/utils.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.3.0/subgrounds/query.py` & `subgrounds-1.4.0/subgrounds/query.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.3.0/subgrounds/schema.py` & `subgrounds-1.4.0/subgrounds/schema.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.3.0/subgrounds/subgraph/fieldpath.py` & `subgrounds-1.4.0/subgrounds/subgraph/fieldpath.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.3.0/subgrounds/subgraph/filter.py` & `subgrounds-1.4.0/subgrounds/subgraph/filter.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.3.0/subgrounds/subgraph/object.py` & `subgrounds-1.4.0/subgrounds/subgraph/object.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.3.0/subgrounds/subgraph/subgraph.py` & `subgrounds-1.4.0/subgrounds/subgraph/subgraph.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.3.0/subgrounds/subgrounds.py` & `subgrounds-1.4.0/subgrounds/subgrounds.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
                     subgraph._schema,
                     doc,
                     pagination_strategy=pagination_strategy,
                     headers=self.headers,
                 )
             else:
                 return client.query(
-                    doc.url, doc.graphql, variables=doc.variables, headers=headers
+                    doc.url, doc.graphql, variables=doc.variables, headers=self.headers
                 )
 
         def transform_doc(transforms: list[DocumentTransform], doc: Document) -> dict:
             logger.debug(f"execute.transform_doc: doc = \n{doc.graphql}")
             match transforms:
                 case []:
                     return execute_document(doc)
```

### Comparing `subgrounds-1.3.0/subgrounds/transform.py` & `subgrounds-1.4.0/subgrounds/transform.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.3.0/subgrounds/utils.py` & `subgrounds-1.4.0/subgrounds/utils.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.3.0/setup.py` & `subgrounds-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['subgrounds', 'subgrounds.pagination', 'subgrounds.subgraph']
+['subgrounds',
+ 'subgrounds.contrib.dash',
+ 'subgrounds.contrib.plotly',
+ 'subgrounds.pagination',
+ 'subgrounds.subgraph']
 
 package_data = \
-{'': ['*']}
+{'': ['*'], 'subgrounds': ['contrib/*']}
 
 install_requires = \
 ['pandas>=1.4.2,<2.0.0',
  'pathlib>=1.0.1,<2.0.0',
  'pipe>=2.0,<3.0',
  'pydantic>=1.10.2,<2.0.0',
  'requests>=2.27.1,<3.0.0']
 
 extras_require = \
 {'dash': ['dash>=2.3.1,<3.0.0']}
 
 setup_kwargs = {
     'name': 'subgrounds',
-    'version': '1.3.0',
+    'version': '1.4.0',
     'description': 'A Pythonic data access layer for applications querying data from The Graph Network.',
     'long_description': "# Subgrounds\n<!-- [![GitHub Actions](https://github.com/0xPlaygrounds/subgrounds/workflows/CI/badge.svg)](https://github.com/0xPlaygrounds/subgrounds/actions) -->\n[![PyPI](https://img.shields.io/pypi/v/subgrounds.svg)](https://pypi.org/project/subgrounds/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/subgrounds.svg)](https://pypi.org/project/subgrounds/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n<br>\n\n[![Discord](https://img.shields.io/discord/896944341598208070?color=7289DA&label=discord&logo=discord&logoColor=fff)](https://discord.gg/gMSSh5bjvk)\n[![Twitter Follow](https://img.shields.io/twitter/follow/Playgrounds0x?color=%231fa1f2&label=Playgrounds%20Analytics&logo=Twitter&logoColor=1fa1f2&style=flat-square)](https://twitter.com/Playgrounds0x)\n\n\n<!-- start elevator-pitch -->\nAn intuitive python library for interfacing with Subgraphs.\n\n## Features\n- **Simple**: Leverage a Pythonic API to easily build queries and transformations without the need for raw GraphQL manipulation.\n- **Automated**: Automatically handle pagination and schema introspection for effortless data retrieval.\n- **Powerful**: Create sophisticated queries using the `SyntheticFields` transformation system.\n\n<!-- end elevator-pitch -->\n\n## Resources\n- [**Subgrounds Docs**](http://docs.playgrounds.network/): User guide and API documentation\n- [**Examples**](https://github.com/0xPlaygrounds/subgrounds/tree/main/examples): A list of examples showcasing Subgrounds integration with Dash and Plotly\n- [**Community projects**](http://docs.playgrounds.network//examples/): An ever growing list of projects created by our community members\n- [**MetricsDAO Subgrounds Workshop**](https://docs.metricsdao.xyz/get-involved/workshops/2022-03-30+-subgrounds-workshop-series): Subgrounds workshop series hosted by MetricsDAO \n\n## Installation\n> Subgrounds **requires** atleast Python 3.10+\n\nSubgrounds is available on PyPi. To install it, run the following:<br>\n`pip install subgrounds`.\n\nSubgrounds also comes bundled with some handy `dash` wrappers. To use those wrappers, you can install the extra `dash` dependencies.<br>\n`pip install subgrounds[dash]`.\n\n## Simple example\n<!-- start simple-example -->\n```python\n>>> from subgrounds import Subgrounds\n\n>>> sg = Subgrounds()\n\n>>> # Load\n>>> aave_v2 = sg.load_subgraph('https://api.thegraph.com/subgraphs/name/messari/aave-v2-ethereum')\n\n>>> # Construct the query\n>>> latest = aave_v2.Query.markets(\n  orderBy=aave_v2.Market.totalValueLockedUSD,\n  orderDirection='desc',\n  first=5,\n)\n\n>>> # Return query to a dataframe\n>>> sg.query_df([\n  latest.name,\n  latest.totalValueLockedUSD,\n])\n                  markets_name  markets_totalValueLockedUSD\n0  Aave interest bearing STETH                 1.522178e+09\n1   Aave interest bearing WETH                 1.221299e+09\n2   Aave interest bearing USDC                 8.140547e+08\n3   Aave interest bearing WBTC                 6.615692e+08\n4   Aave interest bearing USDT                 3.734017e+08\n```\n<!-- end simple-example -->\n\n\n## About Us\nPlaygrounds Analytics is a data solutions company providing serverless on-chain data infrastructures and services for data teams, analysts, and engineers. Checkout us out [here](https://playgrounds.network/) to learn more!\n\n\n\n\n<!-- TODO: Move this to github pages docs -->\n<!-- # Dash and Plotly wrappers\nSubgrounds provides wrappers for Plotly objects and Dash components to facilitate visualization of data from The Graph.\n\nPlotly wrappers can be found in the `subgrounds.plotly_wrappers` submodule. The wrappers include a `Figure` wrapper as well as wrappers for most Plotly traces (see https://plotly.com/python/reference/). All Plotly trace wrappers accept the same arguments as their underlying Plotly trace with the notable difference being that Subgrounds `FieldPath` objects can be used as arguments wherever one would usually provide data to the traces.\n\n```python\nfrom subgrounds.plotly_wrappers import Bar, Figure\nfrom subgrounds.dash_wrappers import Graph\n\nborrows = aave_v2.Query.borrows(\n  orderBy=aave_v2.Borrow.timestamp,\n  orderDirection='desc',\n  first=100\n)\n\nrepays = aave_v2.Query.repays(\n  orderBy=aave_v2.Repay.timestamp,\n  orderDirection='desc',\n  first=100\n)\n\n# Dashboard\napp = dash.Dash(__name__)\n\napp.layout = html.Div(\n  html.Div([\n    html.H4('Entities'),\n    html.Div([\n      # Subgrounds Graph Dash component\n      Graph(\n        # A Subgrounds Plotly figure \n        Figure(\n          subgrounds=sg,\n          traces=[\n            # Subgrounds Plotly traces\n            Bar(x=borrows.reserve.symbol, y=borrows.amount),\n            Bar(x=repays.reserve.symbol, y=repays.amount)\n          ]\n        )\n      )\n    ])\n  ])\n)\n``` -->\n\n<!-- Generates the following Dash dashboard (at time of writing):\n![Alt text](https://raw.githubusercontent.com/Protean-Labs/subgrounds/main/img/bar-chart-example.png) -->\n\n<!-- # Examples and resources\nSee the `examples/` directory for an evergrowing list of examples. -->\n\n\n## Acknowledgments\nThis software project would not be possible without the support of The Graph Foundation. You can learn more about The Graph and its mission [here](https://thegraph.com/).\n\n<!-- TODO: Move this to github pages docs -->\n<!-- # Notes\n## Non-subgraph GraphQL APIs\nAlthough Subgrounds has been developed with subgraph APIs in mind, most features will also work with any GraphQL API. However, Subgrounds has not been tested with non-subgraph GraphQL APIs and some features will definitely break if the non-subgraph APIs do not follow the same conventions as subgraph APIs (e.g.: automatic pagination relies on each entity having a unique `id` field).\n\nIt is nonetheless possible to use Subgrounds with non-subgraph GraphQL APIs by using `load_api` instead of `load_subgraph`. This will bypass Subgrounds automatic pagination feature and pagination will therefore have to be done manually. Below is an example of using Subgrounds with the snapshot GraphQL API.\n```python\n>>> from datetime import datetime\n\n>>> from subgrounds.subgrounds import Subgrounds\n>>> from subgrounds.subgraph import SyntheticField\n\n>>> sg = Subgrounds()\n>>> snapshot = sg.load_api('https://hub.snapshot.org/graphql')\n\n>>> snapshot.Proposal.datetime = SyntheticField(\n...   lambda timestamp: str(datetime.fromtimestamp(timestamp)),\n...   SyntheticField.STRING,\n...   snapshot.Proposal.end,\n... )\n\n>>> proposals = snapshot.Query.proposals(\n...   orderBy='created',\n...   orderDirection='desc',\n...   first=100,\n...   where=[\n...     snapshot.Proposal.space == 'olympusdao.eth',\n...     snapshot.Proposal.state == 'closed'\n...   ]\n... )\n\n>>> sg.query_df([\n...   proposals.datetime,\n...   proposals.title,\n...   proposals.votes,\n... ])\n     proposals_datetime                                    proposals_title  proposals_votes\n0   2022-03-25 15:33:00  OIP-87: BeraChain Investment + Strategic Partn...              184\n1   2022-03-25 12:00:00                 OIP-86: Uniswap Migration Proposal              146\n2   2022-03-25 13:12:00                    TAP 8 - Yearn Finance Whitelist              137\n3   2022-03-22 15:10:10                      OIP-85: Emissions Adjustments              167\n4   2022-03-13 20:17:26                  TAP 7 - Anchor Protocol Whitelist              141\n..                  ...                                                ...              ...\n95  2021-11-20 23:00:00                 OlympusDAO Add ETH to the Treasury               52\n96  2022-01-31 12:00:00                            Add BTC to the Treasury              232\n97  2021-11-29 23:00:00   OlympusDAO OlympusDAO Launch OHM on POLYGON c...              234\n98  2021-11-29 23:00:00                 OlympusDAO Launch OHM on BSC chain               92\n99  2021-11-20 23:00:00  Suggestions to add more video operation guidan...               53\n\n[100 rows x 3 columns]\n```\n\n## GraphQL Aliases\nThe use of the alias `xf608864358427cfb` in the query string is to prevent conflict when merging fieldpaths that select the same fields with different arguments. For example, in the following code, the `borrows` query field is selected twice with different arguments:\n```python\n>>> latest_borrows = aave_v2.Query.borrows(\n...  orderBy=aave_v2.Borrow.timestamp,\n...  orderDirection='desc',\n...  first=100\n...)\n\n>>> largest_borrows = aave_v2.Query.borrows(\n...  orderBy=aave_v2.Borrow.amount,\n...  orderDirection='desc',\n...  first=100\n...)\n\n>>> req = sg.mk_request([\n...   latest_borrows.reserve.symbol,\n...   latest_borrows.amount,\n...   largest_borrows.reserve.symbol,\n...   largest_borrows.amount,\n... ])\n>>> print(req.graphql)\nquery {\n  x8b3edf3dc6501837: borrows(first: 100, orderBy: amount, orderDirection: desc) {\n    reserve {\n      symbol\n    }\n    amount\n  }\n  xf608864358427cfb: borrows(first: 100, orderBy: timestamp, orderDirection: desc) {\n    reserve {\n      symbol\n    }\n    amount\n  }\n}\n``` -->\n",
     'author': 'cvauclair',
     'author_email': 'cvauclair@playgrounds.network',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/0xPlaygrounds/subgrounds',
```

### Comparing `subgrounds-1.3.0/PKG-INFO` & `subgrounds-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subgrounds
-Version: 1.3.0
+Version: 1.4.0
 Summary: A Pythonic data access layer for applications querying data from The Graph Network.
 Home-page: https://github.com/0xPlaygrounds/subgrounds
 Keywords: graph,subgrounds,graphql,subgraph
 Author: cvauclair
 Author-email: cvauclair@playgrounds.network
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
```

