# Comparing `tmp/rframe-0.2.6.tar.gz` & `tmp/rframe-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rframe-0.2.6.tar", max compression
+gzip compressed data, was "rframe-0.2.7.tar", max compression
```

## Comparing `rframe-0.2.6.tar` & `rframe-0.2.7.tar`

### file list

```diff
@@ -1,37 +1,36 @@
--rw-r--r--   0        0        0     1073 2023-02-18 19:36:43.795440 rframe-0.2.6/LICENSE
--rw-r--r--   0        0        0     1026 2023-02-18 19:36:43.795440 rframe-0.2.6/README.rst
--rw-r--r--   0        0        0     3021 2023-02-18 19:36:43.799440 rframe-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      618 2023-02-18 19:36:43.799440 rframe-0.2.6/rframe/__init__.py
--rw-r--r--   0        0        0     2809 2023-02-18 19:36:43.799440 rframe-0.2.6/rframe/_hypothesis_plugin.py
--rw-r--r--   0        0        0     6601 2023-02-18 19:36:43.799440 rframe-0.2.6/rframe/data_accessor.py
--rw-r--r--   0        0        0     1026 2023-02-18 19:36:43.799440 rframe-0.2.6/rframe/dispatchers.py
--rw-r--r--   0        0        0      212 2023-02-18 19:36:43.799440 rframe-0.2.6/rframe/indexes/__init__.py
--rw-r--r--   0        0        0     2610 2023-02-18 19:36:43.799440 rframe-0.2.6/rframe/indexes/base.py
--rw-r--r--   0        0        0       63 2023-02-18 19:36:43.799440 rframe-0.2.6/rframe/indexes/index.py
--rw-r--r--   0        0        0     3205 2023-02-18 19:36:43.799440 rframe-0.2.6/rframe/indexes/interpolating_index.py
--rw-r--r--   0        0        0     1245 2023-02-18 19:36:43.799440 rframe-0.2.6/rframe/indexes/interval_index.py
--rw-r--r--   0        0        0     1999 2023-02-18 19:36:43.799440 rframe-0.2.6/rframe/indexes/multi_index.py
--rw-r--r--   0        0        0      472 2023-02-18 19:36:43.799440 rframe-0.2.6/rframe/interfaces/__init__.py
--rw-r--r--   0        0        0     3657 2023-02-18 19:36:43.799440 rframe-0.2.6/rframe/interfaces/base.py
--rw-r--r--   0        0        0    10732 2023-02-18 19:36:43.799440 rframe-0.2.6/rframe/interfaces/json.py
--rw-r--r--   0        0        0    26685 2023-02-18 19:36:43.799440 rframe-0.2.6/rframe/interfaces/mongo.py
--rw-r--r--   0        0        0    12136 2023-02-18 19:36:43.799440 rframe-0.2.6/rframe/interfaces/pandas.py
--rw-r--r--   0        0        0     3852 2023-02-18 19:36:43.799440 rframe-0.2.6/rframe/interfaces/rest.py
--rw-r--r--   0        0        0    11551 2023-02-18 19:36:43.799440 rframe-0.2.6/rframe/interfaces/tinydb.py
--rw-r--r--   0        0        0     6290 2023-02-18 19:36:43.799440 rframe-0.2.6/rframe/rest_client.py
--rw-r--r--   0        0        0    14089 2023-02-18 19:36:43.799440 rframe-0.2.6/rframe/rest_server.py
--rw-r--r--   0        0        0    13145 2023-02-18 19:36:43.799440 rframe-0.2.6/rframe/rframe.py
--rw-r--r--   0        0        0    19113 2023-02-18 19:36:43.799440 rframe-0.2.6/rframe/schema.py
--rw-r--r--   0        0        0     5516 2023-02-18 19:36:43.799440 rframe-0.2.6/rframe/types.py
--rw-r--r--   0        0        0     7529 2023-02-18 19:36:43.799440 rframe-0.2.6/rframe/utils.py
--rw-r--r--   0        0        0       36 2023-02-18 19:36:43.799440 rframe-0.2.6/tests/__init__.py
--rw-r--r--   0        0        0     1835 2023-02-18 19:36:43.799440 rframe-0.2.6/tests/test_basics.py
--rw-r--r--   0        0        0     1948 2023-02-18 19:36:43.799440 rframe-0.2.6/tests/test_json.py
--rw-r--r--   0        0        0     3306 2023-02-18 19:36:43.799440 rframe-0.2.6/tests/test_mongo.py
--rw-r--r--   0        0        0     2514 2023-02-18 19:36:43.799440 rframe-0.2.6/tests/test_pandas.py
--rw-r--r--   0        0        0     3510 2023-02-18 19:36:43.799440 rframe-0.2.6/tests/test_rest.py
--rw-r--r--   0        0        0     9442 2023-02-18 19:36:43.799440 rframe-0.2.6/tests/test_schemas.py
--rw-r--r--   0        0        0     2297 2023-02-18 19:36:43.799440 rframe-0.2.6/tests/test_tinydb.py
--rw-r--r--   0        0        0      478 2023-02-18 19:36:43.803440 rframe-0.2.6/tests/test_utils.py
--rw-r--r--   0        0        0     2129 1970-01-01 00:00:00.000000 rframe-0.2.6/setup.py
--rw-r--r--   0        0        0     2147 1970-01-01 00:00:00.000000 rframe-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-13 18:31:23.906425 rframe-0.2.7/LICENSE
+-rw-r--r--   0        0        0     1026 2023-04-13 18:31:23.906425 rframe-0.2.7/README.rst
+-rw-r--r--   0        0        0     3021 2023-04-13 18:31:23.910425 rframe-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      618 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/__init__.py
+-rw-r--r--   0        0        0     2809 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/_hypothesis_plugin.py
+-rw-r--r--   0        0        0     6601 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/data_accessor.py
+-rw-r--r--   0        0        0     1026 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/dispatchers.py
+-rw-r--r--   0        0        0      212 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/indexes/__init__.py
+-rw-r--r--   0        0        0     2610 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/indexes/base.py
+-rw-r--r--   0        0        0       63 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/indexes/index.py
+-rw-r--r--   0        0        0     3205 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/indexes/interpolating_index.py
+-rw-r--r--   0        0        0     1245 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/indexes/interval_index.py
+-rw-r--r--   0        0        0     1999 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/indexes/multi_index.py
+-rw-r--r--   0        0        0      472 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/interfaces/__init__.py
+-rw-r--r--   0        0        0     3657 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/interfaces/base.py
+-rw-r--r--   0        0        0    10732 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/interfaces/json.py
+-rw-r--r--   0        0        0    27454 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/interfaces/mongo.py
+-rw-r--r--   0        0        0    12136 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/interfaces/pandas.py
+-rw-r--r--   0        0        0     3852 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/interfaces/rest.py
+-rw-r--r--   0        0        0    11551 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/interfaces/tinydb.py
+-rw-r--r--   0        0        0     6290 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/rest_client.py
+-rw-r--r--   0        0        0    14218 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/rest_server.py
+-rw-r--r--   0        0        0    13145 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/rframe.py
+-rw-r--r--   0        0        0    19976 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/schema.py
+-rw-r--r--   0        0        0     5516 2023-04-13 18:31:23.910425 rframe-0.2.7/rframe/types.py
+-rw-r--r--   0        0        0     7529 2023-04-13 18:31:23.914425 rframe-0.2.7/rframe/utils.py
+-rw-r--r--   0        0        0       36 2023-04-13 18:31:23.914425 rframe-0.2.7/tests/__init__.py
+-rw-r--r--   0        0        0     1835 2023-04-13 18:31:23.914425 rframe-0.2.7/tests/test_basics.py
+-rw-r--r--   0        0        0     1948 2023-04-13 18:31:23.914425 rframe-0.2.7/tests/test_json.py
+-rw-r--r--   0        0        0     3306 2023-04-13 18:31:23.914425 rframe-0.2.7/tests/test_mongo.py
+-rw-r--r--   0        0        0     2514 2023-04-13 18:31:23.914425 rframe-0.2.7/tests/test_pandas.py
+-rw-r--r--   0        0        0     3510 2023-04-13 18:31:23.914425 rframe-0.2.7/tests/test_rest.py
+-rw-r--r--   0        0        0     9442 2023-04-13 18:31:23.914425 rframe-0.2.7/tests/test_schemas.py
+-rw-r--r--   0        0        0     2297 2023-04-13 18:31:23.914425 rframe-0.2.7/tests/test_tinydb.py
+-rw-r--r--   0        0        0      478 2023-04-13 18:31:23.914425 rframe-0.2.7/tests/test_utils.py
+-rw-r--r--   0        0        0     2147 1970-01-01 00:00:00.000000 rframe-0.2.7/PKG-INFO
```

### Comparing `rframe-0.2.6/LICENSE` & `rframe-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rframe-0.2.6/README.rst` & `rframe-0.2.7/README.rst`

 * *Files identical despite different names*

### Comparing `rframe-0.2.6/pyproject.toml` & `rframe-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "rframe"
-version = "0.2.6"
+version = "0.2.7"
 homepage = "https://github.com/jmosbacher/rframe"
 description = "Top-level package for rframe."
 authors = ["Yossi Mosbacher <joe.mosbacher@gmail.com>"]
 readme = "README.rst"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `rframe-0.2.6/rframe/__init__.py` & `rframe-0.2.7/rframe/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for rframe."""
 
 __author__ = """Yossi Mosbacher"""
 __email__ = "joe.mosbacher@gmail.com"
-__version__ = "0.2.6"
+__version__ = "0.2.7"
 
 from loguru import logger
 
 from . import schema, indexes, utils, dispatchers
 
 from .indexes import Index, InterpolatingIndex, IntervalIndex
 from .types import Interval, IntegerInterval, TimeInterval
```

### Comparing `rframe-0.2.6/rframe/_hypothesis_plugin.py` & `rframe-0.2.7/rframe/_hypothesis_plugin.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.6/rframe/data_accessor.py` & `rframe-0.2.7/rframe/data_accessor.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.6/rframe/dispatchers.py` & `rframe-0.2.7/rframe/dispatchers.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.6/rframe/indexes/base.py` & `rframe-0.2.7/rframe/indexes/base.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.6/rframe/indexes/interpolating_index.py` & `rframe-0.2.7/rframe/indexes/interpolating_index.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.6/rframe/indexes/interval_index.py` & `rframe-0.2.7/rframe/indexes/interval_index.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.6/rframe/indexes/multi_index.py` & `rframe-0.2.7/rframe/indexes/multi_index.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.6/rframe/interfaces/base.py` & `rframe-0.2.7/rframe/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.6/rframe/interfaces/json.py` & `rframe-0.2.7/rframe/interfaces/json.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.6/rframe/interfaces/mongo.py` & `rframe-0.2.7/rframe/interfaces/mongo.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from typing import List, Union
 from loguru import logger
 
 import pandas as pd
 from pydantic import BaseModel
 
 from pymongo.collection import Collection
+
+from rframe.interfaces.json import from_json
 from ..types import Interval
 
 from ..indexes import Index, InterpolatingIndex, IntervalIndex, MultiIndex
 from ..utils import singledispatchmethod, hashable_doc, unhashable_doc
 from .base import BaseDataQuery, DatasourceInterface
 
 
@@ -442,17 +444,38 @@
         logger.debug(
             "Building mongo interpolating-query for index: "
             f"{index} with label: {label}"
         )
 
         label = to_mongo(label)
 
+        if isinstance(label, dict):
+            label = from_json(label)
+
         if label is None or label == slice(None):
             labels = {index.name: label}
             return MongoAggregation(index, labels, self.source, [])
+        
+        if isinstance(label, slice):
+            start = label.start
+            stop = label.stop
+            step = label.step
+            if step is None:
+                labels = {index.name: label}
+                pipeline = mongo_overlap_query(index.name, (start, stop))
+                return MongoAggregation(index, labels, self.source, pipeline)
+            else:
+                # create the range of values manually so it works with non-numeric values
+                
+                label = []
+                val = start
+                while val < stop:
+                    label.append(val)
+                    val += step
+
         limit = 1 if others is None else others
 
         if not isinstance(label, list):
             # pipelines = dict(
             #     before=mongo_before_query(index.name, label, limit=limit),
             #     after=mongo_after_query(index.name, label, limit=limit),
             # )
```

### Comparing `rframe-0.2.6/rframe/interfaces/pandas.py` & `rframe-0.2.7/rframe/interfaces/pandas.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.6/rframe/interfaces/rest.py` & `rframe-0.2.7/rframe/interfaces/rest.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.6/rframe/interfaces/tinydb.py` & `rframe-0.2.7/rframe/interfaces/tinydb.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.6/rframe/rest_client.py` & `rframe-0.2.7/rframe/rest_client.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.6/rframe/rest_server.py` & `rframe-0.2.7/rframe/rest_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,16 @@
     Optional,
     Sequence,
     Type,
     TypeVar,
     Union,
 )
 
+from rframe.interfaces.json import from_json
+
 from .schema import BaseSchema
 from .utils import camel_to_snake
 
 from fastapi import APIRouter, HTTPException, Query
 from fastapi.types import DecoratedCallable
 from fastapi.params import Depends
 
@@ -271,14 +273,15 @@
 
     def _query_route(self, *args, **kwargs) -> Callable[..., Any]:
         # This is the actual implementation that will be called when
         # a request is made to the route.
         def query_func_impl(
             limit: int = None, skip: int = None, sort=None, **kwargs
         ) -> List[BaseSchema]:
+            kwargs = {k: from_json(v) for k, v in kwargs.items() if v is not None}
             query = self.schema.compile_query(self.datasource, **kwargs)
             return [
                 self.schema(**d)
                 for d in query.execute(limit=limit, skip=skip, sort=sort)
             ]
 
         # fastapi uses the function signature to generate the openapi docs
```

### Comparing `rframe-0.2.6/rframe/rframe.py` & `rframe-0.2.7/rframe/rframe.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.6/rframe/schema.py` & `rframe-0.2.7/rframe/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from collections import defaultdict
 import inspect
+from itertools import product
 import json
 
 import pandas as pd
-from pydantic import BaseModel, ValidationError
+from pydantic import BaseModel, ValidationError, validate_model
 from pydantic.fields import FieldInfo, ModelField
 from typing import Any, Dict, List, Mapping, Optional, Union, Generator
 
 
 from .dispatchers import are_equal
 from .indexes import BaseIndex, Index, MultiIndex
 from .interfaces import get_interface
@@ -184,28 +186,45 @@
         import rframe
 
         if datasource is None:
             datasource = cls.default_datasource()
         return rframe.RemoteFrame(cls, datasource)
 
     @classmethod
+    def _validate_labels(cls, **labels):
+        """Validate labels against schema"""
+        labels = [
+            [(name, l) for l in label] if isinstance(label, list) else [(name, label)]
+            for name, label in labels.items()
+        ]
+        validated = []
+        for label_vals in product(*labels):
+            label_dict = dict(label_vals)
+            valid_dict, names, error = validate_model(cls, label_dict)
+            if len(valid_dict) < len(label_dict):
+                raise error
+            validated.append(valid_dict)
+        labels = defaultdict(list)
+        for d in validated:
+            for k, v in d.items():
+                labels[k].append(v)
+        labels = {k: v[0] if len(v) == 1 else v for k, v in labels.items()}
+        return labels
+
+    @classmethod
     def extract_labels(cls, **kwargs):
         """Extract query labels from kwargs
 
         returns extracted labels and remaining kwargs
         """
-        labels = {}
+        labels = {k:v for k,v in kwargs.items() if k in cls.__fields__ and v is not None}
+        labels = cls._validate_labels(**labels)
 
-        for name, field in cls.__fields__.items():
-            label = kwargs.pop(name, None)
-            if label is None:
-                label = kwargs.pop(field.alias, None)
-            if label is None:
-                continue
-            labels[name] = label
+        labels = {k:v for k,v in labels.items() if k in kwargs}
+        kwargs = {k:v for k,v in kwargs.items() if k not in labels}
 
         return labels, kwargs
 
     @classmethod
     def compile_query(cls, datasource=None, **labels):
         if datasource is None:
             datasource = cls.default_datasource()
```

### Comparing `rframe-0.2.6/rframe/types.py` & `rframe-0.2.7/rframe/types.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.6/rframe/utils.py` & `rframe-0.2.7/rframe/utils.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.6/tests/test_basics.py` & `rframe-0.2.7/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.6/tests/test_json.py` & `rframe-0.2.7/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.6/tests/test_mongo.py` & `rframe-0.2.7/tests/test_mongo.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.6/tests/test_pandas.py` & `rframe-0.2.7/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.6/tests/test_rest.py` & `rframe-0.2.7/tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.6/tests/test_schemas.py` & `rframe-0.2.7/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.6/tests/test_tinydb.py` & `rframe-0.2.7/tests/test_tinydb.py`

 * *Files identical despite different names*

### Comparing `rframe-0.2.6/PKG-INFO` & `rframe-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rframe
-Version: 0.2.6
+Version: 0.2.7
 Summary: Top-level package for rframe.
 Home-page: https://github.com/jmosbacher/rframe
 License: MIT
 Author: Yossi Mosbacher
 Author-email: joe.mosbacher@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

