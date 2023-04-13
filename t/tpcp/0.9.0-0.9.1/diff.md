# Comparing `tmp/tpcp-0.9.0.tar.gz` & `tmp/tpcp-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tpcp-0.9.0.tar", max compression
+gzip compressed data, was "tpcp-0.9.1.tar", max compression
```

## Comparing `tpcp-0.9.0.tar` & `tpcp-0.9.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1073 2022-08-11 07:49:00.398973 tpcp-0.9.0/LICENSE
--rw-r--r--   0        0        0     8135 2022-08-11 07:49:00.398973 tpcp-0.9.0/README.md
--rw-r--r--   0        0        0     2330 2022-08-11 07:49:00.486978 tpcp-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     1212 2022-08-11 07:49:00.486978 tpcp-0.9.0/tpcp/__init__.py
--rw-r--r--   0        0        0     1184 2022-08-11 07:49:00.486978 tpcp-0.9.0/tpcp/_algorithm.py
--rw-r--r--   0        0        0    18483 2022-08-11 07:49:00.486978 tpcp-0.9.0/tpcp/_algorithm_utils.py
--rw-r--r--   0        0        0    24931 2022-08-11 07:49:00.486978 tpcp-0.9.0/tpcp/_base.py
--rw-r--r--   0        0        0    22807 2022-08-11 07:49:00.486978 tpcp-0.9.0/tpcp/_dataset.py
--rw-r--r--   0        0        0     3465 2022-08-11 07:49:00.486978 tpcp-0.9.0/tpcp/_hash.py
--rw-r--r--   0        0        0     1513 2022-08-11 07:49:00.486978 tpcp-0.9.0/tpcp/_optimize.py
--rw-r--r--   0        0        0     3186 2022-08-11 07:49:00.486978 tpcp-0.9.0/tpcp/_parameters.py
--rw-r--r--   0        0        0     5980 2022-08-11 07:49:00.486978 tpcp-0.9.0/tpcp/_pipeline.py
--rw-r--r--   0        0        0        0 2022-08-11 07:49:00.486978 tpcp-0.9.0/tpcp/_utils/__init__.py
--rw-r--r--   0        0        0     3496 2022-08-11 07:49:00.486978 tpcp-0.9.0/tpcp/_utils/_general.py
--rw-r--r--   0        0        0     1279 2022-08-11 07:49:00.486978 tpcp-0.9.0/tpcp/_utils/_multiprocess.py
--rw-r--r--   0        0        0    10331 2022-08-11 07:49:00.486978 tpcp-0.9.0/tpcp/_utils/_score.py
--rw-r--r--   0        0        0      522 2022-08-11 07:49:00.486978 tpcp-0.9.0/tpcp/exceptions.py
--rw-r--r--   0        0        0      276 2022-08-11 07:49:00.486978 tpcp-0.9.0/tpcp/optimize/__init__.py
--rw-r--r--   0        0        0    39174 2022-08-11 07:49:00.486978 tpcp-0.9.0/tpcp/optimize/_optimize.py
--rw-r--r--   0        0        0    13845 2022-08-11 07:49:00.486978 tpcp-0.9.0/tpcp/optimize/optuna.py
--rw-r--r--   0        0        0      806 2022-08-11 07:49:00.486978 tpcp-0.9.0/tpcp/types.py
--rw-r--r--   0        0        0      268 2022-08-11 07:49:00.486978 tpcp-0.9.0/tpcp/validate/__init__.py
--rw-r--r--   0        0        0    15061 2022-08-11 07:49:00.486978 tpcp-0.9.0/tpcp/validate/_scorer.py
--rw-r--r--   0        0        0     9793 2022-08-11 07:49:00.486978 tpcp-0.9.0/tpcp/validate/_validate.py
--rw-r--r--   0        0        0     9223 2022-08-11 07:49:09.126262 tpcp-0.9.0/setup.py
--rw-r--r--   0        0        0     9061 2022-08-11 07:49:09.127040 tpcp-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-09-09 07:46:29.586772 tpcp-0.9.1/LICENSE
+-rw-r--r--   0        0        0     8135 2022-09-09 07:46:29.586772 tpcp-0.9.1/README.md
+-rw-r--r--   0        0        0     2330 2022-09-09 07:46:29.674773 tpcp-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1212 2022-09-09 07:46:29.674773 tpcp-0.9.1/tpcp/__init__.py
+-rw-r--r--   0        0        0     1184 2022-09-09 07:46:29.674773 tpcp-0.9.1/tpcp/_algorithm.py
+-rw-r--r--   0        0        0    18483 2022-09-09 07:46:29.674773 tpcp-0.9.1/tpcp/_algorithm_utils.py
+-rw-r--r--   0        0        0    25673 2022-09-09 07:46:29.674773 tpcp-0.9.1/tpcp/_base.py
+-rw-r--r--   0        0        0    22807 2022-09-09 07:46:29.678773 tpcp-0.9.1/tpcp/_dataset.py
+-rw-r--r--   0        0        0     3465 2022-09-09 07:46:29.678773 tpcp-0.9.1/tpcp/_hash.py
+-rw-r--r--   0        0        0     1513 2022-09-09 07:46:29.678773 tpcp-0.9.1/tpcp/_optimize.py
+-rw-r--r--   0        0        0     3186 2022-09-09 07:46:29.678773 tpcp-0.9.1/tpcp/_parameters.py
+-rw-r--r--   0        0        0     5980 2022-09-09 07:46:29.678773 tpcp-0.9.1/tpcp/_pipeline.py
+-rw-r--r--   0        0        0        0 2022-09-09 07:46:29.678773 tpcp-0.9.1/tpcp/_utils/__init__.py
+-rw-r--r--   0        0        0     3496 2022-09-09 07:46:29.678773 tpcp-0.9.1/tpcp/_utils/_general.py
+-rw-r--r--   0        0        0     1279 2022-09-09 07:46:29.678773 tpcp-0.9.1/tpcp/_utils/_multiprocess.py
+-rw-r--r--   0        0        0    10331 2022-09-09 07:46:29.678773 tpcp-0.9.1/tpcp/_utils/_score.py
+-rw-r--r--   0        0        0      522 2022-09-09 07:46:29.678773 tpcp-0.9.1/tpcp/exceptions.py
+-rw-r--r--   0        0        0      276 2022-09-09 07:46:29.678773 tpcp-0.9.1/tpcp/optimize/__init__.py
+-rw-r--r--   0        0        0    39174 2022-09-09 07:46:29.678773 tpcp-0.9.1/tpcp/optimize/_optimize.py
+-rw-r--r--   0        0        0    13845 2022-09-09 07:46:29.678773 tpcp-0.9.1/tpcp/optimize/optuna.py
+-rw-r--r--   0        0        0      806 2022-09-09 07:46:29.678773 tpcp-0.9.1/tpcp/types.py
+-rw-r--r--   0        0        0      268 2022-09-09 07:46:29.678773 tpcp-0.9.1/tpcp/validate/__init__.py
+-rw-r--r--   0        0        0    15061 2022-09-09 07:46:29.678773 tpcp-0.9.1/tpcp/validate/_scorer.py
+-rw-r--r--   0        0        0     9793 2022-09-09 07:46:29.678773 tpcp-0.9.1/tpcp/validate/_validate.py
+-rw-r--r--   0        0        0     9227 1970-01-01 00:00:00.000000 tpcp-0.9.1/setup.py
+-rw-r--r--   0        0        0     9061 1970-01-01 00:00:00.000000 tpcp-0.9.1/PKG-INFO
```

### Comparing `tpcp-0.9.0/LICENSE` & `tpcp-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tpcp-0.9.0/README.md` & `tpcp-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `tpcp-0.9.0/pyproject.toml` & `tpcp-0.9.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tpcp"
-version = "0.9.0"
+version = "0.9.1"
 description = "Pipeline and Dataset helpers for complex algorithm evaluation."
 authors = [
     "Arne Küderle <arne.kuederle@fau.de>",
     "Robert Richer <robert.richer@fau.de>",
     "Raul C. Sîmpetru <raul.simpetru@fau.de>",
     "Björn Eskofier <björn.eskofier@fau.de>"
 ]
@@ -80,13 +80,13 @@
 _check_isort = "isort . --check"
 check = { sequence = ["_check_black", "_check_isort", "lint"], help = "Check all potential format and linting issues.", ignore_fail = false }
 test = { cmd = "pytest --cov=tpcp --cov-report=term-missing --cov-report=xml", help = "Run Pytest with coverage." }
 docs = { "script" = "_tasks:task_docs()",  help = "Build the html docs using Sphinx." }
 bump_version = { "script" = "_tasks:task_update_version()" }
 
 [tool.pyright]
-pythonVersion = "3.7"
+pythonVersion = "3.8"
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tpcp-0.9.0/tpcp/__init__.py` & `tpcp-0.9.1/tpcp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     Para,
     Parameter,
     PurePara,
     PureParameter,
 )
 from tpcp._pipeline import OptimizablePipeline, Pipeline
 
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 
 
 __all__ = [
     "make_action_safe",
     "make_optimize_safe",
     "clone",
     "cf",
```

### Comparing `tpcp-0.9.0/tpcp/_algorithm.py` & `tpcp-0.9.1/tpcp/_algorithm.py`

 * *Files identical despite different names*

### Comparing `tpcp-0.9.0/tpcp/_algorithm_utils.py` & `tpcp-0.9.1/tpcp/_algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `tpcp-0.9.0/tpcp/_base.py` & `tpcp-0.9.1/tpcp/_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,29 @@
 import dataclasses
 import inspect
 import sys
 import warnings
 from collections import defaultdict
 from functools import wraps
 from types import MethodWrapperType
-from typing import Any, Callable, DefaultDict, Dict, Generic, Iterable, List, Optional, Tuple, Type, TypeVar, Union
+from typing import (
+    Any,
+    Callable,
+    ClassVar,
+    DefaultDict,
+    Dict,
+    Generic,
+    Iterable,
+    List,
+    Optional,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+)
 
 import numpy as np
 import pandas as pd
 from sklearn.base import BaseEstimator
 from typing_extensions import Annotated, Literal, Self, get_args, get_origin
 
 from tpcp._parameters import _ParaTypes
@@ -102,16 +116,14 @@
         try:
             val = eval(expression, globalns, localns)  # noqa: eval-used
             break
         except NameError as e:
             missing = str(e).split("'")[1]
             localns[missing] = None
         except AttributeError as e:
-            if "'NoneType' object has no attribute 'GridSearch'" not in str(e):
-                raise e
             raise RuntimeError(
                 "You ran into an edge case of the builtin type resolver. "
                 "This happens if you use a nested type annotation that is only valid during runtime. "
                 "This usually happens if you are using a `if TYPE_CHECKING:` guard for some of your imports to avoid "
                 "circular dependencies.\n"
                 "For most of these cases we have a built in workaround, but only if you provide the type directly and "
                 "not in an attribute notation:\n"
@@ -161,41 +173,52 @@
                 # TODO: This does not check if the str is a valid expression.
                 #   This might not be an issue, but could lead to obscure error messages.
                 value = _retry_eval_with_missing_locals(value, base_globals)
             hints[name] = value
     return hints
 
 
-def _extract_annotations(
-    cls: Type[_BaseTpcpObject], init_fields: Dict[str, inspect.Parameter]
-) -> Dict[str, _ParaTypes]:
+def _extract_partial_annotations(cls: Type[_BaseTpcpObject]) -> Dict[str, _ParaTypes]:
     cls_annotations = _custom_get_type_hints(cls)
     para_annotations = {}
     for k, v in cls_annotations.items():
-        if get_origin(v) is Annotated:
+        origin = get_origin(v)
+        if origin is ClassVar:
+            # If the parameter is a ClassVar, we go one level deeper and check, if its argument was annotated.
+            v = get_args(v)[0]
+            origin = get_origin(v)
+        if origin is Annotated:
             for annot in get_args(v)[1:]:
                 if isinstance(annot, _ParaTypes):
                     para_annotations[k] = annot
                     break
-        elif k in init_fields:
-            para_annotations[k] = _ParaTypes.SIMPLE
+
     return para_annotations
 
 
+def _add_missing_init_fields_to_annotations(
+    para_annotations: Dict[str, _ParaTypes], init_fields: Dict[str, inspect.Parameter]
+):
+    for k in init_fields:
+        if k not in para_annotations:
+            para_annotations[k] = _ParaTypes.SIMPLE
+
+
 def _run_field_checks(cls, fields: Dict[str, Any]) -> None:
     _has_dangerous_mutable_default(fields, cls)
     _has_invalid_name(fields, cls)
     _annotations_are_valid(fields, cls)
 
 
 def _process_tpcp_class(cls: Type[_BaseTpcpObject]):
     # We extract the fields of the init
     fields = _get_init_defaults(cls)
-    # Then we extract our metadata annotations
-    cls.__field_annotations__ = _extract_annotations(cls, init_fields=fields)
+
+    # Now that we know the init fields for sure, we can complete our parameter extraction
+    _add_missing_init_fields_to_annotations(cls.__field_annotations__, fields)
 
     # Validation
     if cls.__skip_validation__ is not True:
         _run_field_checks(cls, fields)
 
     if dataclasses.is_dataclass(cls) and any(isinstance(field.default, BaseFactory) for field in fields.values()):
         # If the class is already a data class when this check runs (aka when it is triggered by the custom
@@ -209,14 +232,19 @@
         )
 
     cls.__tpcp_cls_processed__ = True
 
 
 def _requires_processed_class(instance: _BaseTpcpObject, method_name: str) -> None:
     if not instance.__tpcp_cls_processed__:
+        if not instance.__field_annotations__ and type(instance).__init__ == object.__init__:
+            # If there are no annotations and no init, it was just a simple class without parameters or init.
+            # This is fine and we mark it as processed to speed up future checks.
+            type(instance).__tpcp_cls_processed__ = True
+            return
         raise RuntimeError(
             f"You are calling {method_name} on a class that has not been processed by tpcp. "
             "This should not happen!\n\n"
             "The only case we know of, is when you defined a class with class annotations, but without an init or a"
             "dataclass decorator. "
             "This is likely a user error.\n\n"
             "If this is not what happened, please open an issue on GitHub with an example explaining how you "
@@ -230,28 +258,27 @@
     __tpcp_cls_processed__: bool
 
     def __init_subclass__(cls, *, _skip_validation: bool = False, **kwargs: Any):
         super().__init_subclass__(**kwargs)
         cls.__skip_validation__ = _skip_validation
         # We set that here to make sure the value is not inherited from the parent class.
         cls.__tpcp_cls_processed__ = False
+        cls.__tpcp_might_have_empty_init__ = False
 
+        # Then we extract all custom annotations that have been made.
+        # We can do that safely, even before a dataclass decorator might process the class
+        cls.__field_annotations__ = _extract_partial_annotations(cls)
+
+        # If the class has no init or is a dataclass (aka a subclass of a dataclass), we don't need to do anything.
+        # It could be that it is a dataclass, but then the dataclass wrapper will already call the post_init
+        # correctly.
+        #
+        # If our class simply does not have an __init__ and will not get one via the dataclass wrapper, there is
+        # nothing to do anyway.
         if cls.__init__ is object.__init__ or dataclasses.is_dataclass(cls):
-            # If the class has no init or is a dataclass (aka a subclass of a dataclass), we don't need to do anything.
-            # It could be that it is a dataclass, but then the dataclass wrapper will already call the post_init
-            # correctly.
-            #
-            # WARNING: This misses one case! Namely, when someone creates a class without an init,
-            # but with annotations that should be processed.
-            # This is not a valid class, but we can not check this, as we will not process the class, because the
-            # `post_init` will never be called.
-            #
-            # For this (and potential other cases), we have simple checks on the basic methods, that raise errors if
-            # the class has not been processed yet...
-
             return
 
         # If we have a custom init, we need to wrap it to call the post_init method.
         setattr(cls, "__init__", _replace_defaults_wrapper(cls.__init__))
 
 
 class BaseTpcpObject(_BaseTpcpObject, _skip_validation=True):
@@ -455,18 +482,19 @@
 def _has_invalid_name(fields: Dict[str, inspect.Parameter], cls: Type[_BaseTpcpObject]) -> None:
     invalid_names = [f for f in fields if "__" in f]
     if len(invalid_names) > 0:
         raise ValidationError(
             f"The parameters {invalid_names} of {cls.__name__} have a double-underscore in their name. "
             "This is not allowed, as it interferes with the nested naming conventions in tpcp.\n\n"
             "If you are seeing this while using `dataclasses`, and trying to annotate nested parameters, make sure to "
-            "exclude from the init using the explicit field syntax:\n\n"
+            "exclude from the init using the explicit field syntax or by wrapping it with `ClassVar`:\n\n"
             ">>> @dataclasses.dataclass\n"
             "... class MyClass(BaseTpcpObject, dataclass=True):  # Yes, this valid Python!\n"
-            "...    nested__parameter: OptiPara[int] = dataclasses.field(init=False)\n\n"
+            "...    nested__parameter: OptiPara[int] = dataclasses.field(init=False)\n"
+            "...    other_nested__parameter: ClassVar[OptiPara[int]]\n\n"
         )
 
 
 def _get_dangerous_mutable_types() -> Tuple[type, ...]:
     # TODO: Update this list or even make it a white list?
     return _BaseTpcpObject, list, dict, np.ndarray, pd.DataFrame, BaseEstimator
```

### Comparing `tpcp-0.9.0/tpcp/_dataset.py` & `tpcp-0.9.1/tpcp/_dataset.py`

 * *Files identical despite different names*

### Comparing `tpcp-0.9.0/tpcp/_hash.py` & `tpcp-0.9.1/tpcp/_hash.py`

 * *Files identical despite different names*

### Comparing `tpcp-0.9.0/tpcp/_optimize.py` & `tpcp-0.9.1/tpcp/_optimize.py`

 * *Files identical despite different names*

### Comparing `tpcp-0.9.0/tpcp/_parameters.py` & `tpcp-0.9.1/tpcp/_parameters.py`

 * *Files identical despite different names*

### Comparing `tpcp-0.9.0/tpcp/_pipeline.py` & `tpcp-0.9.1/tpcp/_pipeline.py`

 * *Files identical despite different names*

### Comparing `tpcp-0.9.0/tpcp/_utils/_general.py` & `tpcp-0.9.1/tpcp/_utils/_general.py`

 * *Files identical despite different names*

### Comparing `tpcp-0.9.0/tpcp/_utils/_multiprocess.py` & `tpcp-0.9.1/tpcp/_utils/_multiprocess.py`

 * *Files identical despite different names*

### Comparing `tpcp-0.9.0/tpcp/_utils/_score.py` & `tpcp-0.9.1/tpcp/_utils/_score.py`

 * *Files identical despite different names*

### Comparing `tpcp-0.9.0/tpcp/exceptions.py` & `tpcp-0.9.1/tpcp/exceptions.py`

 * *Files identical despite different names*

### Comparing `tpcp-0.9.0/tpcp/optimize/_optimize.py` & `tpcp-0.9.1/tpcp/optimize/_optimize.py`

 * *Files identical despite different names*

### Comparing `tpcp-0.9.0/tpcp/optimize/optuna.py` & `tpcp-0.9.1/tpcp/optimize/optuna.py`

 * *Files identical despite different names*

### Comparing `tpcp-0.9.0/tpcp/types.py` & `tpcp-0.9.1/tpcp/types.py`

 * *Files identical despite different names*

### Comparing `tpcp-0.9.0/tpcp/validate/_scorer.py` & `tpcp-0.9.1/tpcp/validate/_scorer.py`

 * *Files identical despite different names*

### Comparing `tpcp-0.9.0/tpcp/validate/_validate.py` & `tpcp-0.9.1/tpcp/validate/_validate.py`

 * *Files identical despite different names*

### Comparing `tpcp-0.9.0/setup.py` & `tpcp-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,21 +16,21 @@
  'typing-extensions>=4.1.1']
 
 extras_require = \
 {'optuna': ['optuna>=2.10.0,<3.0.0'], 'torch': ['torch>=1.6.0']}
 
 setup_kwargs = {
     'name': 'tpcp',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'Pipeline and Dataset helpers for complex algorithm evaluation.',
     'long_description': '[![PyPI](https://img.shields.io/pypi/v/tpcp)](https://pypi.org/project/tpcp/)\n[![Documentation Status](https://readthedocs.org/projects/tpcp/badge/?version=latest)](https://tpcp.readthedocs.io/en/latest/?badge=latest)\n[![codecov](https://codecov.io/gh/mad-lab-fau/tpcp/branch/main/graph/badge.svg?token=ZNVT5LNYHO)](https://codecov.io/gh/mad-lab-fau/tpcp)\n[![Test and Lint](https://github.com/mad-lab-fau/tpcp/actions/workflows/test-and-lint.yml/badge.svg?branch=main)](https://github.com/mad-lab-fau/tpcp/actions/workflows/test-and-lint.yml)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/tpcp)\n\n# tpcp - Tiny Pipelines for Complex Problems\n\nA generic way to build object-oriented datasets and algorithm pipelines and tools to evaluate them.\n\nEasily install `tpcp` via pip:\n```bash\npip install tpcp\n```\n\nOr add it to your project with [poetry](https://python-poetry.org/):\n```bash\npoetry add tpcp\n```\n\n## Why?\n\nEvaluating Algorithms - in particular when they contain machine learning - is hard.\nBesides understanding required concepts (cross validation, bias, overfitting, ...), you need to implement the required \nsteps and make them work together with your algorithms and data.\nIf you are doing something "regular" like training an SVM on tabular data, amazing libraries like [sklearn](https://scikit-learn.org), \n[tslearn](https://github.com/tslearn-team/tslearn), [pytorch](https://pytorch.org), and many others, have your back.\nBy using their built-in tools (e.g. `sklearn.evaluation.GridSearchCV`) you prevent implementation errors, and you are\nprovided with a sensible structure to organize your code that is well understood in the community.\n\nHowever, often the problems we are trying to solve are not regular.\nThey are **complex**.\nAs an example, here is the summary of the method from one of our [recent papers](https://jneuroengrehab.biomedcentral.com/articles/10.1186/s12984-021-00883-7):\n- We have continuous multi-dimensional sensor recordings from multiple participants from a hospital visit and multiple days at home\n- For each participant we have global metadata (age, diagnosis) and daily annotations\n- We want to train a Hidden-Markov-Model that can find events in the data streams\n- We need to tune hyper-parameters of the algorithm using a participant-wise cross validation\n- We want to evaluate the final performance of the algorithm for the settings trained on the hospital data -> tested on home data and trained on home data -> tested on home data\n- Using the same structure we want to evaluate a state-of-the-art algorithm to compare the results\n\nNone of the standard frameworks can easily abstract this problem, because here we have none-tabular data, multiple data \nsources per participant, a non-traditional ML algorithm, and a complex train-test split logic.\n\nWith `tpcp` we want to provide a flexible framework to approach such complex problems with structure and confidence.\n\n## How?\n\nTo make `tpcp` easy to use, we try to focus on a couple of key ideas:\n\n- Datasets are Python classes (think of [`pytorch.datasets`](https://pytorch.org/tutorials/beginner/basics/data_tutorial.html), but more flexible) that can be split, iterated over, and queried.\n- Algorithms and Pipelines are Python classes with a simple `run` and `optimize` interface, that can be implemented to fit any problem.\n- Everything is a parameter and everything is optimization: In regular ML we differentiate *training* and *hyper-parameter optimization*.\n  In `tpcp` we consider everything that modifies parameters or weights as an *optimization*.\n  This allows to use the same concepts and code interfaces from simple algorithms that just require a grid search to optimize a parameter to neuronal network pipelines with hyperparameter tuning.\n- Provide what is difficult, allow to change everything else:\n  `tpcp` implements complicated constructs like cross validation and grid search and, whenever possible, tries to catch obvious errors in your approach.\n  However, for the actual algorithm and dataset you are free to do whatever is required to solve your current research question.\n\n## Should you use tpcp?\n\n### Datasets\n\n**Yes** - the object-oriented Datasets have proven themselves to be a really nice and flexible way to encapsulate Datasets with data from multiple modalities.\nThere is a clear path of integrating lazy-loading, load-cashing, data filtering, or pre-processing on loading.\nFrom our experience, even if you ignore all the other tpcp features, Datasets can greatly simplify how you interact with your data sources and can serve as a self-documenting API for your data.\n\n[Learn more](https://tpcp.readthedocs.io/en/latest/guides/algorithms_pipelines_datasets.html#datasets) \n([Examples](https://tpcp.readthedocs.io/en/latest/auto_examples/index.html#datasets))\n\nOther projects using Datasets:\n- [sensor_position_dataset_helper](https://github.com/mad-lab-fau/sensor_position_dataset_helper/blob/master/sensor_position_dataset_helper/tpcp_dataset.py)\n- [cold-face-test-analysis](https://github.com/mad-lab-fau/cft-analysis/tree/main/cft_analysis/datasets)\n- [mad-datasets](https://github.com/mad-lab-fau/mad-datasets)\n\n### Parameter Optimization and Cross Validation\n\n**Maybe** - All parameter optimization features in tpcp exist to provide a unified API, in case other specific frameworks are to specialised.\nIn cases where all your algorithms can be abstracted by `sklearn`, `pytorch` (with the `skorch` wrapper), `tensorflow`/`Keras` (with the `scikeras` wrapper), \nor any other framework that provides a nice scikit-learn API, you will get all the features tpcp can provide with much less boilerplate by just using `sklearn` and `optuna` directly.\nEven, if you need to implement completely custom algorithms, we would encourage you to see if you can emulate a sklearn-like API to make use of its fast ecosystem.\n\nThis will usually work well for all algorithms that can be abstracted by the fit-predict paradigm.\nHowever, for more "traditional" algorithms with no "fit" step or complicated optimizations, the `run` (with optional `self_optimize`) API of tpcp might be a better fit.\nSo if you are using or developing algorithms across library domains, that don\'t all work well with a sklearn API, then **Yes**, tpcp is a good choice.\n\nLearn more:\n[General Concepts](https://tpcp.readthedocs.io/en/latest/guides/index.html#user-guides),\n[Custom Algorithms](https://tpcp.readthedocs.io/en/latest/auto_examples/index.html#algorithms), \n[Parameter Optimization](https://tpcp.readthedocs.io/en/latest/auto_examples/index.html#parameter-optimization), \n[Cross Validation](https://tpcp.readthedocs.io/en/latest/auto_examples/index.html#validation)\n\n\n## Dev Setup\n\nWe are using [poetry](https://python-poetry.org/) to manage dependencies and \n[poethepoet](https://github.com/nat-n/poethepoet) to run and manage dev tasks.\n\nTo set up the dev environment *including* the required dependencies for using `tpcp` together with `optuna` \nrun the following commands: \n```bash\ngit clone https://github.com/mad-lab-fau/tpcp\ncd tpcp\npoetry install -E optuna -E torch # This might take a while\n```\n\n\nAfterwards you can start to develop and change things.\nIf you want to run tests, format your code, build the docs, ..., you can run one of the following `poethepoet` commands\n\n```\nCONFIGURED TASKS\n  format         \n  lint           Lint all files with Prospector.\n  check          Check all potential format and linting issues.\n  test           Run Pytest with coverage.\n  docs           Build the html docs using Sphinx.\n  bump_version   \n```\n\nby calling\n\n```bash\npoetry run poe <command name>\n````\n\nIf you installed `poethepoet` globally, you can skip the `poetry run` part at the beginning.\n\n## Contribution\n\nThe entire development is managed via [GitHub](https://github.com/mad-lab-fau/tpcp).\nIf you run into any issues, want to discuss certain decisions, want to contribute features or feature requests, just \nreach out to us by [opening a new issue](https://github.com/mad-lab-fau/tpcp/issues/new/choose).\n',
     'author': 'Arne Küderle',
     'author_email': 'arne.kuederle@fau.de',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/mad-lab-fau/tpcp',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'python_requires': '>=3.8,<3.11',
 }
```

### Comparing `tpcp-0.9.0/PKG-INFO` & `tpcp-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: tpcp
-Version: 0.9.0
+Version: 0.9.1
 Summary: Pipeline and Dataset helpers for complex algorithm evaluation.
 Home-page: https://github.com/mad-lab-fau/tpcp
 Author: Arne Küderle
 Author-email: arne.kuederle@fau.de
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: optuna
 Provides-Extra: torch
 Requires-Dist: joblib (>=1.1.0,<2.0.0)
 Requires-Dist: numpy (>=1,<2)
 Requires-Dist: optuna (>=2.10.0,<3.0.0); extra == "optuna"
 Requires-Dist: pandas (>=1,<2)
 Requires-Dist: scikit-learn (>=1,<2)
```

