# Comparing `tmp/concrete_ml-0.6.1-py3-none-any.whl.zip` & `tmp/concrete_ml-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,46 +1,57 @@
-Zip file size: 119221 bytes, number of entries: 44
+Zip file size: 168782 bytes, number of entries: 55
 -rw-r--r--  2.0 unx      284 b- defN 80-Jan-01 00:00 concrete/__init__.py
--rw-r--r--  2.0 unx       50 b- defN 80-Jan-01 00:00 concrete/ml/__init__.py
+-rw-r--r--  2.0 unx     1722 b- defN 80-Jan-01 00:00 concrete/ml/__init__.py
 -rw-r--r--  2.0 unx       95 b- defN 80-Jan-01 00:00 concrete/ml/common/__init__.py
--rw-r--r--  2.0 unx     1574 b- defN 80-Jan-01 00:00 concrete/ml/common/check_inputs.py
+-rw-r--r--  2.0 unx     2519 b- defN 80-Jan-01 00:00 concrete/ml/common/check_inputs.py
 -rw-r--r--  2.0 unx      101 b- defN 80-Jan-01 00:00 concrete/ml/common/debugging/__init__.py
 -rw-r--r--  2.0 unx     2377 b- defN 80-Jan-01 00:00 concrete/ml/common/debugging/custom_assert.py
--rw-r--r--  2.0 unx     6116 b- defN 80-Jan-01 00:00 concrete/ml/common/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 concrete/ml/common/serialization/__init__.py
+-rw-r--r--  2.0 unx     1310 b- defN 80-Jan-01 00:00 concrete/ml/common/serialization/dumpers.py
+-rw-r--r--  2.0 unx     2018 b- defN 80-Jan-01 00:00 concrete/ml/common/serialization/encoder.py
+-rw-r--r--  2.0 unx     2856 b- defN 80-Jan-01 00:00 concrete/ml/common/serialization/loaders.py
+-rw-r--r--  2.0 unx    17216 b- defN 80-Jan-01 00:00 concrete/ml/common/utils.py
+-rw-r--r--  2.0 unx      235 b- defN 80-Jan-01 00:00 concrete/ml/deployment/Dockerfile.server
 -rw-r--r--  2.0 unx      121 b- defN 80-Jan-01 00:00 concrete/ml/deployment/__init__.py
--rw-r--r--  2.0 unx    12249 b- defN 80-Jan-01 00:00 concrete/ml/deployment/fhe_client_server.py
+-rw-r--r--  2.0 unx    17568 b- defN 80-Jan-01 00:00 concrete/ml/deployment/deploy_to_aws.py
+-rw-r--r--  2.0 unx     3800 b- defN 80-Jan-01 00:00 concrete/ml/deployment/deploy_to_docker.py
+-rw-r--r--  2.0 unx    15080 b- defN 80-Jan-01 00:00 concrete/ml/deployment/fhe_client_server.py
+-rw-r--r--  2.0 unx     4321 b- defN 80-Jan-01 00:00 concrete/ml/deployment/server.py
+-rw-r--r--  2.0 unx       33 b- defN 80-Jan-01 00:00 concrete/ml/deployment/server_requirements.txt
+-rw-r--r--  2.0 unx     3285 b- defN 80-Jan-01 00:00 concrete/ml/deployment/utils.py
 -rw-r--r--  2.0 unx       19 b- defN 80-Jan-01 00:00 concrete/ml/onnx/__init__.py
--rw-r--r--  2.0 unx     3467 b- defN 80-Jan-01 00:00 concrete/ml/onnx/convert.py
--rw-r--r--  2.0 unx     9416 b- defN 80-Jan-01 00:00 concrete/ml/onnx/onnx_impl_utils.py
--rw-r--r--  2.0 unx     9227 b- defN 80-Jan-01 00:00 concrete/ml/onnx/onnx_model_manipulations.py
--rw-r--r--  2.0 unx     9115 b- defN 80-Jan-01 00:00 concrete/ml/onnx/onnx_utils.py
--rw-r--r--  2.0 unx    50990 b- defN 80-Jan-01 00:00 concrete/ml/onnx/ops_impl.py
+-rw-r--r--  2.0 unx     3472 b- defN 80-Jan-01 00:00 concrete/ml/onnx/convert.py
+-rw-r--r--  2.0 unx     9401 b- defN 80-Jan-01 00:00 concrete/ml/onnx/onnx_impl_utils.py
+-rw-r--r--  2.0 unx     9684 b- defN 80-Jan-01 00:00 concrete/ml/onnx/onnx_model_manipulations.py
+-rw-r--r--  2.0 unx    20192 b- defN 80-Jan-01 00:00 concrete/ml/onnx/onnx_utils.py
+-rw-r--r--  2.0 unx    58040 b- defN 80-Jan-01 00:00 concrete/ml/onnx/ops_impl.py
 -rw-r--r--  2.0 unx      101 b- defN 80-Jan-01 00:00 concrete/ml/pytest/__init__.py
--rw-r--r--  2.0 unx    27539 b- defN 80-Jan-01 00:00 concrete/ml/pytest/torch_models.py
--rw-r--r--  2.0 unx     4767 b- defN 80-Jan-01 00:00 concrete/ml/pytest/utils.py
+-rw-r--r--  2.0 unx    42028 b- defN 80-Jan-01 00:00 concrete/ml/pytest/torch_models.py
+-rw-r--r--  2.0 unx     8787 b- defN 80-Jan-01 00:00 concrete/ml/pytest/utils.py
 -rw-r--r--  2.0 unx     1081 b- defN 80-Jan-01 00:00 concrete/ml/quantization/__init__.py
--rw-r--r--  2.0 unx    29563 b- defN 80-Jan-01 00:00 concrete/ml/quantization/base_quantized_op.py
--rw-r--r--  2.0 unx    40067 b- defN 80-Jan-01 00:00 concrete/ml/quantization/post_training.py
--rw-r--r--  2.0 unx    16579 b- defN 80-Jan-01 00:00 concrete/ml/quantization/quantized_module.py
--rw-r--r--  2.0 unx    67819 b- defN 80-Jan-01 00:00 concrete/ml/quantization/quantized_ops.py
--rw-r--r--  2.0 unx    26653 b- defN 80-Jan-01 00:00 concrete/ml/quantization/quantizers.py
--rw-r--r--  2.0 unx      452 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/__init__.py
--rw-r--r--  2.0 unx    63178 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/base.py
--rw-r--r--  2.0 unx    10913 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/glm.py
--rw-r--r--  2.0 unx     9283 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/linear_model.py
--rw-r--r--  2.0 unx     6926 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/protocols.py
--rw-r--r--  2.0 unx    20369 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/qnn.py
--rw-r--r--  2.0 unx     4043 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/rf.py
--rw-r--r--  2.0 unx     3813 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/svm.py
--rw-r--r--  2.0 unx     1393 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/torch_modules.py
--rw-r--r--  2.0 unx     3676 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/tree.py
--rw-r--r--  2.0 unx     8292 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/tree_to_numpy.py
--rw-r--r--  2.0 unx    13273 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/xgb.py
+-rw-r--r--  2.0 unx    35250 b- defN 80-Jan-01 00:00 concrete/ml/quantization/base_quantized_op.py
+-rw-r--r--  2.0 unx    43507 b- defN 80-Jan-01 00:00 concrete/ml/quantization/post_training.py
+-rw-r--r--  2.0 unx    24344 b- defN 80-Jan-01 00:00 concrete/ml/quantization/quantized_module.py
+-rw-r--r--  2.0 unx    80967 b- defN 80-Jan-01 00:00 concrete/ml/quantization/quantized_ops.py
+-rw-r--r--  2.0 unx    37503 b- defN 80-Jan-01 00:00 concrete/ml/quantization/quantizers.py
+-rw-r--r--  2.0 unx       77 b- defN 80-Jan-01 00:00 concrete/ml/search_parameters/__init__.py
+-rw-r--r--  2.0 unx    21176 b- defN 80-Jan-01 00:00 concrete/ml/search_parameters/p_error_search.py
+-rw-r--r--  2.0 unx     4679 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/__init__.py
+-rw-r--r--  2.0 unx    62686 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/base.py
+-rw-r--r--  2.0 unx    13633 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/glm.py
+-rw-r--r--  2.0 unx    25212 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/linear_model.py
+-rw-r--r--  2.0 unx    13339 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/qnn.py
+-rw-r--r--  2.0 unx    12567 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/qnn_module.py
+-rw-r--r--  2.0 unx    12243 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/rf.py
+-rw-r--r--  2.0 unx    10614 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/svm.py
+-rw-r--r--  2.0 unx    10394 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/tree.py
+-rw-r--r--  2.0 unx    10920 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/tree_to_numpy.py
+-rw-r--r--  2.0 unx    20074 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/xgb.py
 -rw-r--r--  2.0 unx       83 b- defN 80-Jan-01 00:00 concrete/ml/torch/__init__.py
--rw-r--r--  2.0 unx    15356 b- defN 80-Jan-01 00:00 concrete/ml/torch/compile.py
+-rw-r--r--  2.0 unx    17532 b- defN 80-Jan-01 00:00 concrete/ml/torch/compile.py
 -rw-r--r--  2.0 unx     3174 b- defN 80-Jan-01 00:00 concrete/ml/torch/numpy_module.py
 -rw-r--r--  2.0 unx      124 b- defN 80-Jan-01 00:00 concrete/ml/version.py
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 concrete_ml-0.6.1.dist-info/WHEEL
--rw-r--r--  2.0 unx     1546 b- defN 80-Jan-01 00:00 concrete_ml-0.6.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2307 b- defN 80-Jan-01 00:00 concrete_ml-0.6.1.dist-info/METADATA
-?rw-r--r--  2.0 unx     3878 b- defN 16-Jan-01 00:00 concrete_ml-0.6.1.dist-info/RECORD
-44 files, 491537 bytes uncompressed, 113001 bytes compressed:  77.0%
+-rw-r--r--  2.0 unx     1546 b- defN 80-Jan-01 00:00 concrete_ml-1.0.0.dist-info/LICENSE
+?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 concrete_ml-1.0.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx    11662 b- defN 16-Jan-01 00:00 concrete_ml-1.0.0.dist-info/METADATA
+?rw-r--r--  2.0 unx     4967 b- defN 16-Jan-01 00:00 concrete_ml-1.0.0.dist-info/RECORD
+55 files, 706107 bytes uncompressed, 160814 bytes compressed:  77.2%
```

## zipnote {}

```diff
@@ -12,23 +12,53 @@
 
 Filename: concrete/ml/common/debugging/__init__.py
 Comment: 
 
 Filename: concrete/ml/common/debugging/custom_assert.py
 Comment: 
 
+Filename: concrete/ml/common/serialization/__init__.py
+Comment: 
+
+Filename: concrete/ml/common/serialization/dumpers.py
+Comment: 
+
+Filename: concrete/ml/common/serialization/encoder.py
+Comment: 
+
+Filename: concrete/ml/common/serialization/loaders.py
+Comment: 
+
 Filename: concrete/ml/common/utils.py
 Comment: 
 
+Filename: concrete/ml/deployment/Dockerfile.server
+Comment: 
+
 Filename: concrete/ml/deployment/__init__.py
 Comment: 
 
+Filename: concrete/ml/deployment/deploy_to_aws.py
+Comment: 
+
+Filename: concrete/ml/deployment/deploy_to_docker.py
+Comment: 
+
 Filename: concrete/ml/deployment/fhe_client_server.py
 Comment: 
 
+Filename: concrete/ml/deployment/server.py
+Comment: 
+
+Filename: concrete/ml/deployment/server_requirements.txt
+Comment: 
+
+Filename: concrete/ml/deployment/utils.py
+Comment: 
+
 Filename: concrete/ml/onnx/__init__.py
 Comment: 
 
 Filename: concrete/ml/onnx/convert.py
 Comment: 
 
 Filename: concrete/ml/onnx/onnx_impl_utils.py
@@ -66,41 +96,44 @@
 
 Filename: concrete/ml/quantization/quantized_ops.py
 Comment: 
 
 Filename: concrete/ml/quantization/quantizers.py
 Comment: 
 
+Filename: concrete/ml/search_parameters/__init__.py
+Comment: 
+
+Filename: concrete/ml/search_parameters/p_error_search.py
+Comment: 
+
 Filename: concrete/ml/sklearn/__init__.py
 Comment: 
 
 Filename: concrete/ml/sklearn/base.py
 Comment: 
 
 Filename: concrete/ml/sklearn/glm.py
 Comment: 
 
 Filename: concrete/ml/sklearn/linear_model.py
 Comment: 
 
-Filename: concrete/ml/sklearn/protocols.py
+Filename: concrete/ml/sklearn/qnn.py
 Comment: 
 
-Filename: concrete/ml/sklearn/qnn.py
+Filename: concrete/ml/sklearn/qnn_module.py
 Comment: 
 
 Filename: concrete/ml/sklearn/rf.py
 Comment: 
 
 Filename: concrete/ml/sklearn/svm.py
 Comment: 
 
-Filename: concrete/ml/sklearn/torch_modules.py
-Comment: 
-
 Filename: concrete/ml/sklearn/tree.py
 Comment: 
 
 Filename: concrete/ml/sklearn/tree_to_numpy.py
 Comment: 
 
 Filename: concrete/ml/sklearn/xgb.py
@@ -114,20 +147,20 @@
 
 Filename: concrete/ml/torch/numpy_module.py
 Comment: 
 
 Filename: concrete/ml/version.py
 Comment: 
 
-Filename: concrete_ml-0.6.1.dist-info/WHEEL
+Filename: concrete_ml-1.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: concrete_ml-0.6.1.dist-info/LICENSE
+Filename: concrete_ml-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: concrete_ml-0.6.1.dist-info/METADATA
+Filename: concrete_ml-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: concrete_ml-0.6.1.dist-info/RECORD
+Filename: concrete_ml-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## concrete/ml/__init__.py

```diff
@@ -1,2 +1,48 @@
 """ML module."""
+import os
+
 from .version import __version__
+
+# If the use of skops needs to be disabled.
+# This could be useful when loading a model with python 3.7 with a higher version
+USE_SKOPS = int(os.environ.get("USE_SKOPS", 1))
+
+# These are all the trusted types that are considered by skops
+TRUSTED_SKOPS = [
+    "numpy.int64",
+    "numpy.float64",
+    "numpy.int32",
+    "xgboost.core.Booster",
+    "xgboost.sklearn.XGBClassifier",
+    "xgboost.sklearn.XGBRegressor",
+    "sklearn._loss.glm_distribution.DistributionBoundary",
+    "sklearn._loss.glm_distribution.TweedieDistribution",
+    "sklearn._loss.glm_distribution.GammaDistribution",
+    "sklearn._loss.glm_distribution.PoissonDistribution",
+    "sklearn.linear_model._glm.link.LogLink",
+    "sklearn.linear_model._glm.link.IdentityLink",
+    "sklearn._loss.link.IdentityLink",
+    "sklearn._loss.link.Interval",
+    "sklearn._loss.link.LogLink",
+    "sklearn._loss.link.LogLink",
+    "sklearn._loss._loss.CyHalfTweedieLossIdentity",
+    "sklearn._loss.loss.HalfTweedieLossIdentity",
+    "sklearn._loss._loss.CyHalfPoissonLoss",
+    "sklearn._loss.loss.HalfPoissonLoss",
+    "sklearn._loss._loss.CyHalfGammaLoss",
+    "sklearn._loss.loss.HalfGammaLoss",
+    "sklearn._loss._loss.CyHalfTweedieLoss",
+    "sklearn._loss.loss.HalfTweedieLoss",
+]
+
+# If USE_SKOPS is False or skops can't be imported we default to pickle
+try:
+    if USE_SKOPS:
+        from skops.io import dumps as dumps_sklearn
+        from skops.io import loads as loads_sklearn
+    else:  # pragma: no cover
+        raise ImportError()
+except ImportError:  # pragma: no cover
+    USE_SKOPS = False
+    from pickle import dumps as dumps_sklearn
+    from pickle import loads as loads_sklearn
```

## concrete/ml/common/check_inputs.py

```diff
@@ -9,46 +9,69 @@
 
 from ..common.debugging.custom_assert import assert_true
 
 # Disable pylint invalid name since scikit learn uses "X" as variable name for data
 # pylint: disable=invalid-name
 
 
-def check_array_and_assert(X):
+def check_array_and_assert(X, *args, **kwargs):
     """sklearn.utils.check_array with an assert.
 
     Equivalent of sklearn.utils.check_array, with a final assert that the type is one which
-    is supported by Concrete-ML.
+    is supported by Concrete ML.
 
     Args:
         X (object): Input object to check / convert
+        *args: The arguments to pass to check_array
+        **kwargs: The keyword arguments to pass to check_array
 
     Returns:
         The converted and validated array
     """
-    X = sklearn.utils.check_array(X)
+    X = sklearn.utils.check_array(X, *args, **kwargs)
     assert_true(isinstance(X, numpy.ndarray), f"wrong type {type(X)}")
     return X
 
 
 def check_X_y_and_assert(X, y, *args, **kwargs):
     """sklearn.utils.check_X_y with an assert.
 
     Equivalent of sklearn.utils.check_X_y, with a final assert that the type is one which
-    is supported by Concrete-ML.
+    is supported by Concrete ML.
 
     Args:
         X (ndarray, list, sparse matrix): Input data
         y (ndarray, list, sparse matrix): Labels
         *args: The arguments to pass to check_X_y
         **kwargs: The keyword arguments to pass to check_X_y
 
     Returns:
         The converted and validated arrays
     """
+
     X, y = sklearn.utils.check_X_y(X, y, *args, **kwargs)
     assert_true(isinstance(X, numpy.ndarray), f"wrong type {type(X)}")
     assert_true(isinstance(y, numpy.ndarray), f"wrong type {type(y)}")
     return X, y
 
 
+def check_X_y_and_assert_multi_output(X, y, *args, **kwargs):
+    """sklearn.utils.check_X_y with an assert and multi-output handling.
+
+    Equivalent of sklearn.utils.check_X_y, with a final assert that the type is one which
+    is supported by Concrete ML. If y is 2D, allows multi-output.
+
+    Args:
+        X (ndarray, list, sparse matrix): Input data
+        y (ndarray, list, sparse matrix): Labels
+        *args: The arguments to pass to check_X_y
+        **kwargs: The keyword arguments to pass to check_X_y
+
+    Returns:
+        The converted and validated arrays with multi-output targets.
+    """
+    multi_output = isinstance(y[0], list) if isinstance(y, list) else len(y.shape) > 1
+    X, y = check_X_y_and_assert(X, y, *args, multi_output=multi_output, **kwargs)
+    return X, y
+
+
 # pylint: enable=invalid-name
```

## concrete/ml/common/utils.py

```diff
@@ -1,22 +1,85 @@
 """Utils that can be re-used by other pieces of code in the module."""
 
+import enum
 import string
+from functools import partial
 from types import FunctionType
-from typing import Callable, Dict, Iterable, Optional, Tuple
+from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Union
 
+import numpy
 import onnx
+import torch
+from concrete.fhe.dtypes import Integer
+from sklearn.base import is_classifier, is_regressor
 
+from ..common.check_inputs import check_array_and_assert
 from ..common.debugging import assert_true
 
 _VALID_ARG_CHARS = set(string.ascii_letters).union(str(i) for i in range(10)).union(("_",))
 
+
+SUPPORTED_FLOAT_TYPES = {
+    "float64": torch.float64,
+    "float32": torch.float32,
+}
+
+SUPPORTED_INT_TYPES = {
+    "int64": torch.int64,
+    "int32": torch.int32,
+    "int16": torch.int16,
+    "int8": torch.int8,
+}
+
 MAX_BITWIDTH_BACKWARD_COMPATIBLE = 8
 
 
+class FheMode(str, enum.Enum):
+    """Enum representing the execution mode.
+
+    This enum inherits from str in order to be able to easily compare a string parameter to its
+    equivalent Enum attribute.
+
+    Examples:
+        fhe_disable = FheMode.DISABLE
+
+        >>> fhe_disable == "disable"
+        True
+
+        >>> fhe_disable == "execute"
+        False
+
+        >>> FheMode.is_valid("simulate")
+        True
+
+        >>> FheMode.is_valid(FheMode.EXECUTE)
+        True
+
+        >>> FheMode.is_valid("predict_in_fhe")
+        False
+
+    """
+
+    DISABLE = "disable"
+    SIMULATE = "simulate"
+    EXECUTE = "execute"
+
+    @staticmethod
+    def is_valid(fhe: Union["FheMode", str]) -> bool:
+        """Indicate if the given name is a supported FHE mode.
+
+        Args:
+            fhe (Union[FheMode, str]): The FHE mode to check.
+
+        Returns:
+            bool: Whether the FHE mode is supported or not.
+        """
+        return fhe in FheMode.__members__.values()
+
+
 def replace_invalid_arg_name_chars(arg_name: str) -> str:
     """Sanitize arg_name, replacing invalid chars by _.
 
     This does not check that the starting character of arg_name is valid.
 
     Args:
         arg_name (str): the arg name to sanitize.
@@ -88,45 +151,43 @@
     return info.version
 
 
 def manage_parameters_for_pbs_errors(
     p_error: Optional[float] = None,
     global_p_error: Optional[float] = None,
 ):
-    """Return (p_error, global_p_error) that we want to give to Concrete-Numpy and the compiler.
+    """Return (p_error, global_p_error) that we want to give to Concrete.
 
     The returned (p_error, global_p_error) depends on user's parameters and the way we want to
-    manage defaults in Concrete-ML, which may be different from the way defaults are managed in
-    Concrete-Numpy
+    manage defaults in Concrete ML, which may be different from the way defaults are managed in
+    Concrete.
 
     Principle:
         - if none are set, we set global_p_error to a default value of our choice
         - if both are set, we raise an error
-        - if one is set, we use it and forward it to Concrete-Numpy and the compiler
+        - if one is set, we use it and forward it to Concrete
 
-    Note that global_p_error is currently not simulated by the VL, i.e., taken as 0.
+    Note that global_p_error is currently set to 0 in the FHE simulation mode.
 
     Args:
         p_error (Optional[float]): probability of error of a single PBS.
         global_p_error (Optional[float]): probability of error of the full circuit.
 
     Returns:
         (p_error, global_p_error): parameters to give to the compiler
 
     Raises:
-        ValueError: if the two parameters are set (this is _not_ as in Concrete-Numpy)
+        ValueError: if the two parameters are set (this is _not_ as in Concrete-Python)
 
     """
-
     # Default probability of error of a circuit. Only used if p_error is set to None
-    # FIXME #2223: we'll find the most appropriate value for default_global_p_error_pbs
-    default_global_p_error_pbs = 0.01
+    default_p_error_pbs = 2**-40
 
     if (p_error, global_p_error) == (None, None):
-        p_error, global_p_error = (None, default_global_p_error_pbs)
+        p_error, global_p_error = (default_p_error_pbs, None)
     elif p_error is None:
         # Nothing to do, use user's parameters
         pass
     elif global_p_error is None:
         # Nothing to do, use user's parameters
         pass
     else:
@@ -134,28 +195,347 @@
 
     return p_error, global_p_error
 
 
 def check_there_is_no_p_error_options_in_configuration(configuration):
     """Check the user did not set p_error or global_p_error in configuration.
 
-    It would be dangerous, since we set them in direct arguments in our calls to Concrete-Numpy.
+    It would be dangerous, since we set them in direct arguments in our calls to Concrete-Python.
 
     Args:
         configuration: Configuration object to use
             during compilation
 
     """
     if configuration is not None:
-        assert_true(  # Defaults for Configuration object
-            not (configuration.p_error is None and configuration.global_p_error == 1 / 100_000),
-            "Setting p_error or global_p_error in the configuration is not supported, "
-            "use kwargs instead.\n"
-            "Please consider setting p_error and global_p_error to None in"
-            " the Configuration object.\n"
-            "Default value for Configuration.global_p_error is not None.",
+        assert_true(
+            configuration.p_error is None,
+            "Don't set p_error in configuration, use kwargs",
         )
-        assert_true(configuration.p_error is None, "Don't set p_error in configuration, use kwargs")
         assert_true(
             configuration.global_p_error is None,
             "Don't set global_p_error in configuration, use kwargs",
         )
+
+
+def get_model_class(model_class):
+    """Return the class of the model (instantiated or not), which can be a partial() instance.
+
+    Args:
+        model_class: The model, which can be a partial() instance.
+
+    Returns:
+        The model's class.
+
+    """
+    # If model_class is a functool.partial instance
+    if isinstance(model_class, partial):
+        return model_class.func
+
+    # If model_class is a instantiated model
+    if not isinstance(model_class, type) and hasattr(model_class, "__class__"):
+        return model_class.__class__
+
+    # Else, it is already a (not instantiated) model class
+    return model_class
+
+
+def is_model_class_in_a_list(model_class, a_list):
+    """Indicate if a model class, which can be a partial() instance, is an element of a_list.
+
+    Args:
+        model_class: The model, which can be a partial() instance.
+        a_list: The list in which to look into.
+
+    Returns:
+        If the model's class is in the list or not.
+
+    """
+    return get_model_class(model_class) in a_list
+
+
+def get_model_name(model_class):
+    """Return the name of the model, which can be a partial() instance.
+
+    Args:
+        model_class: The model, which can be a partial() instance.
+
+    Returns:
+        the model's name.
+
+    """
+    return get_model_class(model_class).__name__
+
+
+def is_classifier_or_partial_classifier(model_class):
+    """Indicate if the model class represents a classifier.
+
+    Args:
+        model_class: The model class, which can be a functool's `partial` class.
+
+    Returns:
+        bool: If the model class represents a classifier.
+    """
+    return is_classifier(get_model_class(model_class))
+
+
+def is_regressor_or_partial_regressor(model_class):
+    """Indicate if the model class represents a regressor.
+
+    Args:
+        model_class: The model class, which can be a functool's `partial` class.
+
+    Returns:
+        bool: If the model class represents a regressor.
+    """
+    return is_regressor(get_model_class(model_class))
+
+
+def is_pandas_dataframe(input_container: Any) -> bool:
+    """Indicate if the input container is a Pandas DataFrame.
+
+    This function is inspired from Scikit-Learn's test validation tools and avoids the need to add
+    and import Pandas as an additional dependency to the project.
+    See https://github.com/scikit-learn/scikit-learn/blob/98cf537f5/sklearn/utils/validation.py#L629
+
+    Args:
+        input_container (Any): The input container to consider
+
+    Returns:
+        bool: If the input container is a DataFrame
+    """
+    return hasattr(input_container, "dtypes") and hasattr(input_container.dtypes, "__array__")
+
+
+def is_pandas_series(input_container: Any) -> bool:
+    """Indicate if the input container is a Pandas Series.
+
+    This function is inspired from Scikit-Learn's test validation tools and avoids the need to add
+    and import Pandas as an additional dependency to the project.
+    See https://github.com/scikit-learn/scikit-learn/blob/98cf537f5/sklearn/utils/validation.py#L629
+
+    Args:
+        input_container (Any): The input container to consider
+
+    Returns:
+        bool: If the input container is a Series
+    """
+    return hasattr(input_container, "iloc") and hasattr(input_container, "dtype")
+
+
+def is_pandas_type(input_container: Any) -> bool:
+    """Indicate if the input container is a Pandas DataFrame or Series.
+
+    Args:
+        input_container (Any): The input container to consider
+
+    Returns:
+        bool: If the input container is a DataFrame orSeries
+    """
+    return is_pandas_dataframe(input_container) or is_pandas_series(input_container)
+
+
+def _get_dtype(values: Any):
+    """Get a set of values' dtype in a string format to facilitate opetations between sets.
+
+    Args:
+        values (Any): The values to consider
+
+    Returns:
+        set[str]: The values' dtype(s) in string format.
+
+    Examples:
+        X_pandas = pandas.DataFrame([[1, 0.5, '1']])
+        X_tensor = torch.tensor([[12, 45, 747.00]])
+
+        >>> X_pandas.dtypes
+        0      int64
+        1    float64
+        2     object
+        dtype: object
+
+        >>> _get_dtype(X_pandas)
+        {'float64', 'int64', 'object'}
+
+        >>> X_tensor.dtype
+        torch.float32
+
+        >>> _get_dtype(X_tensor)
+        {'torch.float32'}
+    """
+    # Specific case: if `values` is a Dict, return all items in a string format and in a single set
+    if isinstance(values, Dict):
+        return set(map(str, sum(values.items(), ())))
+
+    # If the `values` is a pandas.DataFrame, retrieve all the different dtypes found in it
+    if is_pandas_dataframe(values):
+        return set(map(str, values.dtypes))
+
+    # Note that numpy.ndarray, pandas.Series and torch.Tensor objects support the dtype attribute
+    return set(map(str, (values.dtype,)))
+
+
+def _is_of_dtype(values: Any, valid_dtypes: Dict) -> bool:
+    """Indicate if the values' dtype(s) matches the given one(s).
+
+    Args:
+        values (Any): The values to consider.
+        valid_dtypes (Dict): The only dtype(s) to consider.
+
+    Returns:
+        bool: If the values' dtype(s) matche the given ones.
+
+    Examples:
+        values_types = _get_dtype(pandas.DataFrame([[1, 0.5, '1']]))
+        valid_dtypes = _get_dtype(SUPPORTED_INT_TYPE)
+
+        >>> values_types
+        {'float64', 'int64', 'object'}
+
+        >>> valid_dtypes
+        {'int16', 'int32', 'int64', 'int8', 'torch.int16',
+         'torch.int32', 'torch.int64', 'torch.int8'}
+
+        >>> values_types - valid_dtypes
+        {'float64', 'object'}
+        # The only supported types are integers, {'float64', 'object'} are not valid in this case.
+
+    """
+    assert_true(isinstance(valid_dtypes, Dict))
+
+    # Convert the list to numpy
+    if isinstance(values, list):
+        values = numpy.array(values)
+
+    # Get the values' types in string format + set type
+    values_types = _get_dtype(values)
+    valid_dtypes = _get_dtype(valid_dtypes)
+
+    # All the elements in first set that are not present in the second set
+    uncommon_types = values_types - valid_dtypes
+
+    return len(uncommon_types) == 0
+
+
+# pylint: disable=unexpected-keyword-arg
+def check_dtype_and_cast(values: Any, expected_dtype: str, error_information: Optional[str] = ""):
+    """Convert any allowed type into an array and cast it if required.
+
+    If values types don't match with any supported type or the expected dtype, raise a ValueError.
+
+    Args:
+        values (Any): The values to consider
+        expected_dtype (str): The expected dtype, either "float32" or "int64"
+        error_information (str): Additional information to put in front of the error message when
+            raising a ValueError. Default to None.
+
+    Returns:
+        (Union[numpy.ndarray, torch.utils.data.dataset.Subset]): The values with proper dtype.
+
+    Raises:
+        ValueError: If the values' dtype don't match the expected one or casting is not possible.
+    """
+    assert_true(
+        expected_dtype in ("float32", "int64"),
+        f'Expected dtype parameter should either be "float32" or "int64". Got {expected_dtype}',
+    )
+
+    assert_true(
+        isinstance(values, (numpy.ndarray, torch.Tensor, List)) or is_pandas_type(values),
+        "Unsupported type. Expected numpy.ndarray, pandas.DataFrame, pandas.Series, list "
+        f"or torch.Tensor but got {type(values)}.",
+    )
+
+    if (expected_dtype == "int64" and _is_of_dtype(values, SUPPORTED_INT_TYPES)) or (
+        expected_dtype == "float32" and _is_of_dtype(values, SUPPORTED_FLOAT_TYPES)
+    ):
+        # If the expected dtype is an int64 and the values are integers of lower precision, we can
+        # safely cast them to int64
+        # If the expected dtype is a float32 and the values are float64, we chose to cast them to
+        # float32 in order to give the user more flexibility. This should not have a great impact on
+        # the models' performances
+        values = check_array_and_assert(values, ensure_2d=False)
+        values = values.astype(expected_dtype)
+
+    else:
+        # Else, if the values' dtype doesn't match the expected one, raise an error
+        error_message = (
+            f"{error_information} dtype does not match the expected dtype and values cannot be "
+            f"properly casted using that latter. Expected dtype {expected_dtype} and got "
+            f"{_get_dtype(values)} with type {type(values)}."
+        )
+
+        raise ValueError(error_message)
+
+    return values
+
+
+def compute_bits_precision(x: numpy.ndarray) -> int:
+    """Compute the number of bits required to represent x.
+
+    Args:
+        x (numpy.ndarray): Integer data
+
+    Returns:
+        int: the number of bits required to represent x
+    """
+    return Integer.that_can_represent([x.min(), x.max()]).bit_width
+
+
+def is_brevitas_model(model: torch.nn.Module) -> bool:
+    """Check if a model is a Brevitas type.
+
+    Args:
+        model: PyTorch model.
+
+    Returns:
+        bool: True if `model` is a Brevitas network.
+
+    """
+    return isinstance(model, torch.nn.Module) and any(
+        hasattr(module, "__class__")
+        and module.__class__.__name__
+        in ["QuantConv1d", "QuantConv2d", "QuantIdentity", "QuantLinear", "QuantReLU"]
+        for module in model.modules()
+    )
+
+
+def to_tuple(x: Any) -> tuple:
+    """Make the input a tuple if it is not already the case.
+
+    Args:
+        x (Any): The input to consider. It can already be an input.
+
+    Returns:
+        tuple: The input as a tuple.
+    """
+    # If the input is not a tuple, return a tuple of a single element
+    if not isinstance(x, tuple):
+        return (x,)
+
+    return x
+
+
+def all_values_are_integers(*values: Any) -> bool:
+    """Indicate that all unpacked values are of a supported integer dtype.
+
+    Args:
+        *values (Any): The values to consider.
+
+    Returns:
+        bool: Wether all values are supported integers or not.
+
+    """
+    return all(_is_of_dtype(value, SUPPORTED_INT_TYPES) for value in values)
+
+
+def all_values_are_floats(*values: Any) -> bool:
+    """Indicate that all unpacked values are of a supported float dtype.
+
+    Args:
+        *values (Any): The values to consider.
+
+    Returns:
+        bool: Wether all values are supported floating points or not.
+
+    """
+    return all(_is_of_dtype(value, SUPPORTED_FLOAT_TYPES) for value in values)
```

## concrete/ml/deployment/fhe_client_server.py

```diff
@@ -1,20 +1,23 @@
 """APIs for FHE deployment."""
 
 import json
-from copy import deepcopy
+import sys
+import zipfile
 from pathlib import Path
-from typing import Any
+from typing import Any, Optional
 
-import concrete.numpy as cnp
 import numpy
 
+from concrete import fhe
+
 from ..common.debugging.custom_assert import assert_true
+from ..common.serialization.encoder import CustomEncoder
+from ..common.serialization.loaders import load_dict
 from ..quantization.quantized_module import QuantizedModule
-from ..quantization.quantizers import UniformQuantizer
 from ..sklearn import (
     DecisionTreeClassifier,
     DecisionTreeRegressor,
     ElasticNet,
     GammaRegressor,
     Lasso,
     LinearRegression,
@@ -52,56 +55,94 @@
     TweedieRegressor,
     GammaRegressor,
     PoissonRegressor,
     QuantizedModule,
 ]
 
 
+try:
+    # 3.8 and above
+    # pylint: disable-next=no-name-in-module
+    from importlib.metadata import version
+except ImportError:  # pragma: no cover
+    # 3.7 and below
+    # pylint: disable-next=no-name-in-module
+    from importlib_metadata import version
+
+
 class FHEModelServer:
     """Server API to load and run the FHE circuit."""
 
-    server: cnp.Server
+    server: fhe.Server
 
     def __init__(self, path_dir: str):
         """Initialize the FHE API.
 
         Args:
             path_dir (str): the path to the directory where the circuit is saved
         """
 
         self.path_dir = path_dir
 
         # Load the FHE circuit
         self.load()
 
     def load(self):
-        """Load the circuit."""
-        self.server = cnp.Server.load(Path(self.path_dir).joinpath("server.zip"))
+        """Load the circuit.
+
+        Raises:
+            ValueError: if mismatch in versions between serialized file and runtime
+        """
+        # Load versions for checking
+        with zipfile.ZipFile(Path(self.path_dir).joinpath("server.zip")) as client_zip:
+            with client_zip.open("versions.json", mode="r") as file:
+                versions = json.load(file)
+
+        errors = []
+        packages_to_check = {"concrete-python"}
+        for package_name, package_version in versions.items():
+            if package_name not in packages_to_check:
+                continue
+            current_version = version(package_name)
+            if package_version != current_version:  # pragma: no cover
+                errors.append((package_name, package_version, current_version))
+        if errors:  # pragma: no cover
+            raise ValueError(
+                "Version mismatch for packages: \n"
+                + "\n".join(f"{error[0]}: {error[1]} != {error[2]}" for error in errors)
+            )
+
+        if not versions["python"].startswith(
+            f"{sys.version_info.major}.{sys.version_info.minor}"
+        ):  # pragma: no cover
+            raise ValueError("Not the same python version between the compiler and the server.")
+
+        self.server = fhe.Server.load(Path(self.path_dir).joinpath("server.zip"))
 
     def run(
         self,
-        serialized_encrypted_quantized_data: cnp.PublicArguments,
-        serialized_evaluation_keys: cnp.EvaluationKeys,
-    ) -> cnp.PublicResult:
+        serialized_encrypted_quantized_data: bytes,
+        serialized_evaluation_keys: bytes,
+    ) -> bytes:
         """Run the model on the server over encrypted data.
 
         Args:
-            serialized_encrypted_quantized_data (cnp.PublicArguments): the encrypted, quantized
+            serialized_encrypted_quantized_data (bytes): the encrypted, quantized
                 and serialized data
-            serialized_evaluation_keys (cnp.EvaluationKeys): the serialized evaluation keys
+            serialized_evaluation_keys (bytes): the serialized evaluation keys
 
         Returns:
-            cnp.PublicResult: the result of the model
+            bytes: the result of the model
         """
         assert_true(self.server is not None, "Model has not been loaded.")
 
-        deserialized_encrypted_quantized_data = self.server.client_specs.unserialize_public_args(
+        deserialized_encrypted_quantized_data = self.server.client_specs.deserialize_public_args(
             serialized_encrypted_quantized_data
         )
-        deserialized_evaluation_keys = cnp.EvaluationKeys.unserialize(serialized_evaluation_keys)
+        deserialized_evaluation_keys = fhe.EvaluationKeys.deserialize(serialized_evaluation_keys)
         result = self.server.run(
             deserialized_encrypted_quantized_data, deserialized_evaluation_keys
         )
         serialized_result = self.server.client_specs.serialize_public_result(result)
         return serialized_result
 
 
@@ -119,109 +160,106 @@
         """
 
         self.path_dir = path_dir
         self.model = model
 
         Path(self.path_dir).mkdir(parents=True, exist_ok=True)
 
-    def _clean_dict_types_for_json(self, d: dict) -> dict:
-        """Clean all values in the dict to be json serializable.
-
-        Args:
-            d (dict): the dict to clean
+    def _export_model_to_json(self) -> Path:
+        """Export the quantizers to a json file.
 
         Returns:
-            dict: the cleaned dict
+            Path: the path to the json file
         """
-        key_to_delete = []
-        for key, value in d.items():
-            if isinstance(value, list) and len(value) > 0 and isinstance(value[0], dict):
-                d[key] = [self._clean_dict_types_for_json(v) for v in value]
-            elif isinstance(value, dict):
-                d[key] = self._clean_dict_types_for_json(value)
-            elif isinstance(value, (numpy.generic, numpy.ndarray)):
-                d[key] = d[key].tolist()
-            elif isinstance(value, (UniformQuantizer)):
-                key_to_delete.append(key)
-        for key in key_to_delete:
-            d.pop(key)
-        return d
-
-    def _export_model_to_json(self):
-        """Export the quantizers to a json file."""
         serialized_processing = {
             "model_type": self.model.__class__.__name__,
             "model_post_processing_params": self.model.post_processing_params,
-            "input_quantizers": [],
-            "output_quantizers": [],
+            "input_quantizers": self.model.input_quantizers,
+            "output_quantizers": self.model.output_quantizers,
+            "cml_version": CML_VERSION,
         }
-        for quantizer in self.model.input_quantizers:
-            # The object __dict__ is not a copy and the values in the dict are the same instances
-            # as the original values. Modifying the __dict__ modifies the original values
-            quantizer_dict = deepcopy(quantizer.__dict__)
-            serialized_processing["input_quantizers"].append(quantizer_dict)
-
-        for quantizer in self.model.output_quantizers:
-            # The object __dict__ is not a copy and the values in the dict are the same instances
-            # as the original values. Modifying the __dict__ modifies the original values
-            quantizer_dict = deepcopy(quantizer.__dict__)
-            serialized_processing["output_quantizers"].append(quantizer_dict)
-
-        serialized_processing = self._clean_dict_types_for_json(serialized_processing)
-
-        # Add the version of the current CML library
-        serialized_processing["cml_version"] = CML_VERSION
-        with open(
-            Path(self.path_dir).joinpath("serialized_processing.json"), "w", encoding="utf-8"
-        ) as f:
-            json.dump(serialized_processing, f)
 
-    def save(self):
+        # Export the `is_fitted` attribute for built-in models
+        if hasattr(self.model, "is_fitted"):
+            serialized_processing["is_fitted"] = self.model.is_fitted
+
+        # Dump json
+        json_path = Path(self.path_dir).joinpath("serialized_processing.json")
+        with open(json_path, "w", encoding="utf-8") as file:
+            json.dump(serialized_processing, file, cls=CustomEncoder)
+        return json_path
+
+    def save(self, via_mlir: bool = False):
         """Export all needed artifacts for the client and server.
 
+        Arguments:
+            via_mlir (bool): serialize with `via_mlir` option from Concrete-Python.
+                For more details on the topic please refer to Concrete-Python's documentation.
+
         Raises:
             Exception: path_dir is not empty
         """
         # Check if the path_dir is empty with pathlib
         listdir = list(Path(self.path_dir).glob("**/*"))
         if len(listdir) > 0:
             raise Exception(
                 f"path_dir: {self.path_dir} is not empty."
                 "Please delete it before saving a new model."
             )
-        assert_true(
-            hasattr(self.model, "fhe_circuit"),
-            "The model must be compiled and have a fhe_circuit object",
-        )
+        self.model.check_model_is_compiled()
 
         # Model must be compiled with jit=False
         # In a jit model, everything is in memory so it is not serializable.
         assert_true(
             not self.model.fhe_circuit.configuration.jit,
             "The model must be compiled with the configuration option jit=False.",
         )
 
         # Export the quantizers
-        self._export_model_to_json()
+        json_path = self._export_model_to_json()
 
         # First save the circuit for the server
         path_circuit_server = Path(self.path_dir).joinpath("server.zip")
-        self.model.fhe_circuit.server.save(path_circuit_server)
+        self.model.fhe_circuit.server.save(path_circuit_server, via_mlir=via_mlir)
 
         # Save the circuit for the client
         path_circuit_client = Path(self.path_dir).joinpath("client.zip")
         self.model.fhe_circuit.client.save(path_circuit_client)
 
+        with zipfile.ZipFile(path_circuit_client, "a") as zip_file:
+            zip_file.write(filename=json_path, arcname="serialized_processing.json")
+
+        # Add versions
+        versions_path = Path(self.path_dir).joinpath("versions.json")
+        versions = {
+            package_name: version(package_name)
+            for package_name in ["concrete-ml", "concrete-python"]
+        }
+        versions[
+            "python"
+        ] = f"{sys.version_info.major}.{sys.version_info.minor}.{sys.version_info.micro}"
+
+        with open(versions_path, "w", encoding="utf-8") as file:
+            json.dump(fp=file, obj=versions)
+
+        with zipfile.ZipFile(path_circuit_server, "a") as zip_file:
+            zip_file.write(filename=versions_path, arcname="versions.json")
+
+        with zipfile.ZipFile(path_circuit_client, "a") as zip_file:
+            zip_file.write(filename=versions_path, arcname="versions.json")
+
+        json_path.unlink()
+
 
 class FHEModelClient:
     """Client API to encrypt and decrypt FHE data."""
 
-    client: cnp.Client
+    client: fhe.Client
 
-    def __init__(self, path_dir: str, key_dir: str = None):
+    def __init__(self, path_dir: str, key_dir: Optional[str] = None):
         """Initialize the FHE API.
 
         Args:
             path_dir (str): the path to the directory where the circuit is saved
             key_dir (str): the path to the directory where the keys are stored
         """
         self.path_dir = path_dir
@@ -232,119 +270,156 @@
             Path(path_dir).exists(), f"{path_dir} does not exist. Please specify a valid path."
         )
 
         # Load
         self.load()
 
     def load(self):  # pylint: disable=no-value-for-parameter
-        """Load the quantizers along with the FHE specs."""
-        self.client = cnp.Client.load(Path(self.path_dir).joinpath("client.zip"), self.key_dir)
+        """Load the quantizers along with the FHE specs.
+
+        Raises:
+            ValueError: if mismatch in versions between serialized file and runtime
+        """
+        self.client = fhe.Client.load(Path(self.path_dir).joinpath("client.zip"), self.key_dir)
 
         # Load the quantizers
-        with open(
-            Path(self.path_dir).joinpath("serialized_processing.json"), "r", encoding="utf-8"
-        ) as f:
-            serialized_processing = json.load(f)
+        with zipfile.ZipFile(Path(self.path_dir).joinpath("client.zip")) as client_zip:
+            with client_zip.open("serialized_processing.json", mode="r") as file:
+                serialized_processing = json.load(file)
+
+        # Load versions for checking
+        with zipfile.ZipFile(Path(self.path_dir).joinpath("client.zip")) as client_zip:
+            with client_zip.open("versions.json", mode="r") as file:
+                versions = json.load(file)
+
+        errors = []
+        packages_to_check = {"concrete-python"}
+        for package_name, package_version in versions.items():
+            if package_name not in packages_to_check:
+                continue
+            current_version = version(package_name)
+            if package_version != current_version:  # pragma: no cover
+                errors.append((package_name, package_version, current_version))
+        if errors:  # pragma: no cover
+            raise ValueError(
+                "Version mismatch for packages: \n"
+                + "\n".join(f"{error[0]}: {error[1]} != {error[2]}" for error in errors)
+            )
 
         # Make sure the version in serialized_model is the same as CML_VERSION
         assert_true(
             serialized_processing["cml_version"] == CML_VERSION,
             f"The version of Concrete ML library ({CML_VERSION}) is different "
             f"from the one used to save the model ({serialized_processing['cml_version']}). "
             "Please update to the proper Concrete ML version.",
         )
 
         # Create dict with available models along with their name
         model_dict = {model_type().__class__.__name__: model_type for model_type in AVAILABLE_MODEL}
 
         # Initialize the model
         self.model = model_dict[serialized_processing["model_type"]]()
-        self.model.input_quantizers = []
-        self.model.output_quantizers = []
-        for quantizer_dict in serialized_processing["input_quantizers"]:
-            self.model.input_quantizers.append(UniformQuantizer(**quantizer_dict))
-        for quantizer_dict in serialized_processing["output_quantizers"]:
-            self.model.output_quantizers.append(UniformQuantizer(**quantizer_dict))
+        self.model.input_quantizers = [
+            load_dict(elt) for elt in serialized_processing["input_quantizers"]
+        ]
+        self.model.output_quantizers = [
+            load_dict(elt) for elt in serialized_processing["output_quantizers"]
+        ]
+
+        # Load the `_is_fitted` private attribute for built-in models
+        if "is_fitted" in serialized_processing:
+            # This private access should be temporary as the Client-Server interface could benefit
+            # from built-in serialization load/dump methods
+            # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/3243
+            # pylint: disable-next=protected-access
+            self.model._is_fitted = serialized_processing["is_fitted"]
 
         # Load model parameters
+        # Add some checks on post-processing-params
+        # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/3131
         self.model.post_processing_params = serialized_processing["model_post_processing_params"]
 
     def generate_private_and_evaluation_keys(self, force=False):
         """Generate the private and evaluation keys.
 
         Args:
             force (bool): if True, regenerate the keys even if they already exist
         """
         self.client.keygen(force)
 
-    def get_serialized_evaluation_keys(self) -> cnp.EvaluationKeys:
+    def get_serialized_evaluation_keys(self) -> bytes:
         """Get the serialized evaluation keys.
 
         Returns:
-            cnp.EvaluationKeys: the evaluation keys
+            bytes: the evaluation keys
         """
         return self.client.evaluation_keys.serialize()
 
-    def quantize_encrypt_serialize(self, x: numpy.ndarray) -> cnp.PublicArguments:
+    def quantize_encrypt_serialize(self, x: numpy.ndarray) -> bytes:
         """Quantize, encrypt and serialize the values.
 
         Args:
             x (numpy.ndarray): the values to quantize, encrypt and serialize
 
         Returns:
-            cnp.PublicArguments: the quantized, encrypted and serialized values
+            bytes: the quantized, encrypted and serialized values
         """
         # Quantize the values
         quantized_x = self.model.quantize_input(x)
 
         # Encrypt the values
         enc_qx = self.client.encrypt(quantized_x)
 
         # Serialize the encrypted values to be sent to the server
         serialized_enc_qx = self.client.specs.serialize_public_args(enc_qx)
         return serialized_enc_qx
 
-    def deserialize_decrypt(
-        self, serialized_encrypted_quantized_result: cnp.PublicArguments
-    ) -> numpy.ndarray:
+    def deserialize_decrypt(self, serialized_encrypted_quantized_result: bytes) -> numpy.ndarray:
         """Deserialize and decrypt the values.
 
         Args:
-            serialized_encrypted_quantized_result (cnp.PublicArguments): the serialized, encrypted
+            serialized_encrypted_quantized_result (bytes): the serialized, encrypted
                 and quantized result
 
         Returns:
             numpy.ndarray: the decrypted and deserialized values
         """
         # Deserialize the encrypted values
-        deserialized_encrypted_quantized_result = self.client.specs.unserialize_public_result(
+        deserialized_encrypted_quantized_result = self.client.specs.deserialize_public_result(
             serialized_encrypted_quantized_result
         )
 
         # Decrypt the values
         deserialized_decrypted_quantized_result = self.client.decrypt(
             deserialized_encrypted_quantized_result
         )
+        assert isinstance(deserialized_decrypted_quantized_result, numpy.ndarray)
         return deserialized_decrypted_quantized_result
 
     def deserialize_decrypt_dequantize(
-        self, serialized_encrypted_quantized_result: cnp.PublicArguments
+        self, serialized_encrypted_quantized_result: bytes
     ) -> numpy.ndarray:
         """Deserialize, decrypt and dequantize the values.
 
         Args:
-            serialized_encrypted_quantized_result (cnp.PublicArguments): the serialized, encrypted
+            serialized_encrypted_quantized_result (bytes): the serialized, encrypted
                 and quantized result
 
         Returns:
             numpy.ndarray: the decrypted (dequantized) values
         """
         # Decrypt and deserialize the values
         deserialized_decrypted_quantized_result = self.deserialize_decrypt(
             serialized_encrypted_quantized_result
         )
 
-        # Dequantize the values and apply the model post processing
-        deserialized_decrypted_dequantized_result = self.model.post_processing(
+        # Dequantize the values
+        deserialized_decrypted_dequantized_result = self.model.dequantize_output(
             deserialized_decrypted_quantized_result
         )
+
+        # Apply post-processing the to dequantized values
+        deserialized_decrypted_dequantized_result = self.model.post_processing(
+            deserialized_decrypted_dequantized_result
+        )
+
         return deserialized_decrypted_dequantized_result
```

## concrete/ml/onnx/convert.py

```diff
@@ -42,15 +42,15 @@
 
     torch.onnx.export(
         torch_module,
         dummy_input,
         str(output_onnx_file_path),
         opset_version=OPSET_VERSION_FOR_ONNX_EXPORT,
     )
-    equivalent_onnx_model = onnx.load_model(output_onnx_file_path)
+    equivalent_onnx_model = onnx.load_model(str(output_onnx_file_path))
     checker.check_model(equivalent_onnx_model)
 
     # Remove the tempfile if we used one
     if use_tempfile:
         output_onnx_file_path.unlink()
 
     # The model was checked just above
```

## concrete/ml/onnx/onnx_impl_utils.py

```diff
@@ -1,14 +1,14 @@
 """Utility functions for onnx operator implementations."""
 
 from typing import Tuple, Union
 
 import numpy
-from concrete.numpy import ones as cnp_ones
-from concrete.onnx import conv as cnp_conv
+from concrete.fhe import conv as cnp_conv
+from concrete.fhe import ones as cnp_ones
 
 from ..common.debugging import assert_true
 
 
 def numpy_onnx_pad(
     x: numpy.ndarray,
     pads: Tuple[int, ...],
@@ -17,15 +17,15 @@
 ) -> numpy.ndarray:
     """Pad a tensor according to ONNX spec, using an optional custom pad value.
 
     Args:
         x (numpy.ndarray): input tensor to pad
         pads (List[int]): padding values according to ONNX spec
         pad_value (Optional[Union[float, int]]): value used to fill in padding, default 0
-        int_only (bool): set to True to generate integer only code with Concrete-Numpy
+        int_only (bool): set to True to generate integer only code with Concrete
 
     Returns:
         res(numpy.ndarray): the input tensor with padding applied
     """
 
     x_pad = x
     if numpy.any(numpy.asarray(pads) > 0):
@@ -43,15 +43,15 @@
         padded_shape = [x.shape[0], x.shape[1]]
         padded_shape += [x.shape[i + 2] + pads[i] + pads[ndim + i] for i in range(ndim)]
 
         # Initialize a padded version of the input, setting
         # the values on the edges to the input zero_point, which corresponds
         # to the real-axis 0
         if int_only:
-            # Work in integer Concrete-Numpy mode
+            # Work in integer Concrete mode
             x_pad = cnp_ones(tuple(padded_shape)) * numpy.int64(pad_value)
         else:
             # Floating point mode
             x_pad = numpy.ones(padded_shape, dtype=numpy.float32) * pad_value
 
         # Create the indices for slice assignment, copy all on batch size and channels dimension
         indices = [slice(None), slice(None)] + [
```

## concrete/ml/onnx/onnx_model_manipulations.py

```diff
@@ -44,16 +44,16 @@
             # If we find a constant that is used, then it is not a constant to remove anymore
             constants_to_remove.pop(graph_output_name)
 
     for node in constants_to_remove.values():
         onnx_model.graph.node.remove(node)
 
 
-# TODO: https://github.com/zama-ai/concrete-ml-internal/issues/410
-# Improve that algorithm which is O(N^2) for now
+# This algorithm needs to be improved, currently it runs in O(N^2)
+# FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/410
 def remove_identity_nodes(onnx_model: onnx.ModelProto):
     """Remove identity nodes from a model.
 
     Args:
         onnx_model (onnx.ModelProto): the model for which we want to remove Identity nodes.
     """
 
@@ -66,19 +66,14 @@
             identity_output = node.output[0]
             # We can only look at the end of the graph as nodes are in topological order
             # flake8 has this unresolved issue: https://github.com/PyCQA/pycodestyle/issues/373
             for next_nodes in onnx_model.graph.node[node_idx + 1 :]:  # noqa: E203
                 for input_idx, input_ in enumerate(next_nodes.input):
                     if input_ == identity_output:
                         next_nodes.input[input_idx] = identity_input
-
-            for output in onnx_model.graph.output:
-                if output.name == identity_output:
-                    output.name = identity_input
-
             onnx_model.graph.node.pop(node_idx)
         else:
             node_idx += 1
 
 
 def keep_following_outputs_discard_others(
     onnx_model: onnx.ModelProto, outputs_to_keep: Iterable[str]
@@ -161,28 +156,45 @@
             # Update the current node with the new Identity node
             onnx_model.graph.node[node_index].CopyFrom(new_node)
 
     # Remove Constant and Identity nodes from the graph
     simplify_onnx_model(onnx_model)
 
 
-def clean_graph_after_node_name(
-    onnx_model: onnx.ModelProto, node_name: str, fail_if_not_found: bool = True
+def clean_graph_at_node_op_type(
+    onnx_model: onnx.ModelProto, node_op_type: str, fail_if_not_found: bool = True
 ):
-    """Clean the graph of the onnx model by removing nodes after the given node name.
+    """Clean the graph of the onnx model by removing nodes at the given node type.
+
+    Note: the specified node_type is also removed.
 
     Args:
         onnx_model (onnx.ModelProto): The onnx model.
-        node_name (str): The node's name whose following nodes will be removed.
-        fail_if_not_found (bool): If true, abort if the node name is not found
+        node_op_type (str): The node's op_type whose following nodes will be removed.
+        fail_if_not_found (bool): If true, abort if the node op_type is not found
 
     Raises:
-        ValueError: if the node name is not found and if fail_if_not_found is set
-
+        ValueError: if fail_if_not_found is set
     """
+
+    target_node_list = [node for node in onnx_model.graph.node if node.op_type == node_op_type]
+    assert_true(
+        len(target_node_list) == 1,
+        "Multiple ReduceSum nodes found which is unexpected in tree-based models",
+    )
+
+    target_node = target_node_list[0]
+
+    # Get the input to ReduceSum where index 0 is the data
+    input_name = target_node.input[0]
+
+    # Find the node that has the input_name as output name
+    node_to_cut = next(node for node in onnx_model.graph.node if node.output[0] == input_name)
+    node_name = node_to_cut.name
+
     nodes_to_remove = []
     output_to_follow = "variable"
     op_reached = False
 
     # Find nodes to remove
     for node in onnx_model.graph.node:
```

## concrete/ml/onnx/onnx_utils.py

```diff
@@ -1,26 +1,215 @@
 """Utils to interpret an ONNX model with numpy."""
 # Utils to interpret an ONNX model with numpy.
 
 
-# Copyright 2018 Google LLC
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
+#                                  Apache License
+#                            Version 2.0, January 2004
+#                         http://www.apache.org/licenses/
+#    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 #
-#     https://www.apache.org/licenses/LICENSE-2.0
+#    1. Definitions.
 #
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+#       "License" shall mean the terms and conditions for use, reproduction,
+#       and distribution as defined by Sections 1 through 9 of this document.
 #
-# Modifications copyright (C) 2022 Zama:
+#       "Licensor" shall mean the copyright owner or entity authorized by
+#       the copyright owner that is granting the License.
+#
+#       "Legal Entity" shall mean the union of the acting entity and all
+#       other entities that control, are controlled by, or are under common
+#       control with that entity. For the purposes of this definition,
+#       "control" means (i) the power, direct or indirect, to cause the
+#       direction or management of such entity, whether by contract or
+#       otherwise, or (ii) ownership of fifty percent (50%) or more of the
+#       outstanding shares, or (iii) beneficial ownership of such entity.
+
+#       "You" (or "Your") shall mean an individual or Legal Entity
+#       exercising permissions granted by this License.
+
+#       "Source" form shall mean the preferred form for making modifications,
+#       including but not limited to software source code, documentation
+#       source, and configuration files.
+
+#       "Object" form shall mean any form resulting from mechanical
+#       transformation or translation of a Source form, including but
+#       not limited to compiled object code, generated documentation,
+#       and conversions to other media types.
+
+#       "Work" shall mean the work of authorship, whether in Source or
+#       Object form, made available under the License, as indicated by a
+#       copyright notice that is included in or attached to the work
+#       (an example is provided in the Appendix below).
+
+#       "Derivative Works" shall mean any work, whether in Source or Object
+#       form, that is based on (or derived from) the Work and for which the
+#       editorial revisions, annotations, elaborations, or other modifications
+#       represent, as a whole, an original work of authorship. For the purposes
+#       of this License, Derivative Works shall not include works that remain
+#       separable from, or merely link (or bind by name) to the interfaces of,
+#       the Work and Derivative Works thereof.
+
+#       "Contribution" shall mean any work of authorship, including
+#       the original version of the Work and any modifications or additions
+#       to that Work or Derivative Works thereof, that is intentionally
+#       submitted to Licensor for inclusion in the Work by the copyright owner
+#       or by an individual or Legal Entity authorized to submit on behalf of
+#       the copyright owner. For the purposes of this definition, "submitted"
+#       means any form of electronic, verbal, or written communication sent
+#       to the Licensor or its representatives, including but not limited to
+#       communication on electronic mailing lists, source code control systems,
+#       and issue tracking systems that are managed by, or on behalf of, the
+#       Licensor for the purpose of discussing and improving the Work, but
+#       excluding communication that is conspicuously marked or otherwise
+#       designated in writing by the copyright owner as "Not a Contribution."
+
+#       "Contributor" shall mean Licensor and any individual or Legal Entity
+#       on behalf of whom a Contribution has been received by Licensor and
+#       subsequently incorporated within the Work.
+
+#    2. Grant of Copyright License. Subject to the terms and conditions of
+#       this License, each Contributor hereby grants to You a perpetual,
+#       worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+#       copyright license to reproduce, prepare Derivative Works of,
+#       publicly display, publicly perform, sublicense, and distribute the
+#       Work and such Derivative Works in Source or Object form.
+
+#    3. Grant of Patent License. Subject to the terms and conditions of
+#       this License, each Contributor hereby grants to You a perpetual,
+#       worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+#       (except as stated in this section) patent license to make, have made,
+#       use, offer to sell, sell, import, and otherwise transfer the Work,
+#       where such license applies only to those patent claims licensable
+#       by such Contributor that are necessarily infringed by their
+#       Contribution(s) alone or by combination of their Contribution(s)
+#       with the Work to which such Contribution(s) was submitted. If You
+#       institute patent litigation against any entity (including a
+#       cross-claim or counterclaim in a lawsuit) alleging that the Work
+#       or a Contribution incorporated within the Work constitutes direct
+#       or contributory patent infringement, then any patent licenses
+#       granted to You under this License for that Work shall terminate
+#       as of the date such litigation is filed.
+
+#    4. Redistribution. You may reproduce and distribute copies of the
+#       Work or Derivative Works thereof in any medium, with or without
+#       modifications, and in Source or Object form, provided that You
+#       meet the following conditions:
+
+#       (a) You must give any other recipients of the Work or
+#           Derivative Works a copy of this License; and
+
+#       (b) You must cause any modified files to carry prominent notices
+#           stating that You changed the files; and
+
+#       (c) You must retain, in the Source form of any Derivative Works
+#           that You distribute, all copyright, patent, trademark, and
+#           attribution notices from the Source form of the Work,
+#           excluding those notices that do not pertain to any part of
+#           the Derivative Works; and
+
+#       (d) If the Work includes a "NOTICE" text file as part of its
+#           distribution, then any Derivative Works that You distribute must
+#           include a readable copy of the attribution notices contained
+#           within such NOTICE file, excluding those notices that do not
+#           pertain to any part of the Derivative Works, in at least one
+#           of the following places: within a NOTICE text file distributed
+#           as part of the Derivative Works; within the Source form or
+#           documentation, if provided along with the Derivative Works; or,
+#           within a display generated by the Derivative Works, if and
+#           wherever such third-party notices normally appear. The contents
+#           of the NOTICE file are for informational purposes only and
+#           do not modify the License. You may add Your own attribution
+#           notices within Derivative Works that You distribute, alongside
+#           or as an addendum to the NOTICE text from the Work, provided
+#           that such additional attribution notices cannot be construed
+#           as modifying the License.
+
+#       You may add Your own copyright statement to Your modifications and
+#       may provide additional or different license terms and conditions
+#       for use, reproduction, or distribution of Your modifications, or
+#       for any such Derivative Works as a whole, provided Your use,
+#       reproduction, and distribution of the Work otherwise complies with
+#       the conditions stated in this License.
+
+#    5. Submission of Contributions. Unless You explicitly state otherwise,
+#       any Contribution intentionally submitted for inclusion in the Work
+#       by You to the Licensor shall be under the terms and conditions of
+#       this License, without any additional terms or conditions.
+#       Notwithstanding the above, nothing herein shall supersede or modify
+#       the terms of any separate license agreement you may have executed
+#       with Licensor regarding such Contributions.
+
+#    6. Trademarks. This License does not grant permission to use the trade
+#       names, trademarks, service marks, or product names of the Licensor,
+#       except as required for reasonable and customary use in describing the
+#       origin of the Work and reproducing the content of the NOTICE file.
+
+#    7. Disclaimer of Warranty. Unless required by applicable law or
+#       agreed to in writing, Licensor provides the Work (and each
+#       Contributor provides its Contributions) on an "AS IS" BASIS,
+#       WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+#       implied, including, without limitation, any warranties or conditions
+#       of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+#       PARTICULAR PURPOSE. You are solely responsible for determining the
+#       appropriateness of using or redistributing the Work and assume any
+#       risks associated with Your exercise of permissions under this License.
+
+#    8. Limitation of Liability. In no event and under no legal theory,
+#       whether in tort (including negligence), contract, or otherwise,
+#       unless required by applicable law (such as deliberate and grossly
+#       negligent acts) or agreed to in writing, shall any Contributor be
+#       liable to You for damages, including any direct, indirect, special,
+#       incidental, or consequential damages of any character arising as a
+#       result of this License or out of the use or inability to use the
+#       Work (including but not limited to damages for loss of goodwill,
+#       work stoppage, computer failure or malfunction, or any and all
+#       other commercial damages or losses), even if such Contributor
+#       has been advised of the possibility of such damages.
+
+#    9. Accepting Warranty or Additional Liability. While redistributing
+#       the Work or Derivative Works thereof, You may choose to offer,
+#       and charge a fee for, acceptance of support, warranty, indemnity,
+#       or other liability obligations and/or rights consistent with this
+#       License. However, in accepting such obligations, You may act only
+#       on Your own behalf and on Your sole responsibility, not on behalf
+#       of any other Contributor, and only if You agree to indemnify,
+#       defend, and hold each Contributor harmless for any liability
+#       incurred by, or claims asserted against, such Contributor by reason
+#       of your accepting any such warranty or additional liability.
+
+#    END OF TERMS AND CONDITIONS
+
+#    APPENDIX: How to apply the Apache License to your work.
+
+#       To apply the Apache License to your work, attach the following
+#       boilerplate notice, with the fields enclosed by brackets "[]"
+#       replaced with your own identifying information. (Don't include
+#       the brackets!)  The text should be enclosed in the appropriate
+#       comment syntax for the file format. We also recommend that a
+#       file or class name and description of purpose be included on the
+#       same "printed page" as the copyright notice for easier
+#       identification within third-party archives.
+
+#    Copyright 2018 Google LLC
+
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+
+#        http://www.apache.org/licenses/LICENSE-2.0
+
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+
+#
+# Modifications copyright (C) 2022-2023 Zama:
 # - variable renaming
 # - streamlining of some functions
 # - mypy typing hints
 # - existing and new ops implementation in separate file
 
 # Original file:
 # https://github.com/google/jax/blob/f6d329b2d9b5f83c6a59e5739aa1ca8d4d1ffa1c/examples/onnx2xla.py
@@ -45,24 +234,26 @@
     numpy_batchnorm,
     numpy_brevitas_quant,
     numpy_cast,
     numpy_celu,
     numpy_clip,
     numpy_concatenate,
     numpy_constant,
+    numpy_constant_of_shape,
     numpy_conv,
     numpy_cos,
     numpy_cosh,
     numpy_div,
     numpy_elu,
     numpy_equal,
     numpy_erf,
     numpy_exp,
     numpy_flatten,
     numpy_floor,
+    numpy_gather,
     numpy_gemm,
     numpy_greater,
     numpy_greater_float,
     numpy_greater_or_equal,
     numpy_greater_or_equal_float,
     numpy_hardsigmoid,
     numpy_hardswish,
@@ -87,19 +278,22 @@
     numpy_pow,
     numpy_prelu,
     numpy_reduce_sum,
     numpy_relu,
     numpy_reshape,
     numpy_round,
     numpy_selu,
+    numpy_shape,
     numpy_sigmoid,
     numpy_sign,
     numpy_sin,
     numpy_sinh,
+    numpy_slice,
     numpy_softplus,
+    numpy_squeeze,
     numpy_sub,
     numpy_tan,
     numpy_tanh,
     numpy_thresholdedrelu,
     numpy_transpose,
     numpy_unsqueeze,
     numpy_where,
@@ -176,24 +370,26 @@
     "Floor": numpy_floor,
     "Max": numpy_max,
     "Min": numpy_min,
     "Neg": numpy_neg,
     "Sign": numpy_sign,
     "Concat": numpy_concatenate,
     "Unsqueeze": numpy_unsqueeze,
+    "Squeeze": numpy_squeeze,
+    "Slice": numpy_slice,
+    "Gather": numpy_gather,
+    "Shape": numpy_shape,
+    "ConstantOfShape": numpy_constant_of_shape,
 }
 
 
-# Creating the following dictionaries was introduced following the performance regression issues
-# observed in https://github.com/zama-ai/concrete-ml-internal/issues/1357.
 # Comparison operators from numpy return boolean values, which is a specific subtype of numpy
-# integer types. However, the problem lies in the fact that while this is the expected behavior for
-# tree-based models, QuantizedOps only handle float values in order to properly quantize. The
-# current solution therefore dissociates the numpy operators used in both cases.
-# FIXME: to remove once https://github.com/zama-ai/concrete-ml-internal/issues/1117 is done.
+# integer types. However, while this is the expected behavior for tree-based models, QuantizedOps
+# can only handle float values in order to properly quantize. The current solution therefore
+# dissociates the numpy operators used in both cases.
 
 # Comparison operators needed for QuantizedOps as they cast the boolean outputs into floats.
 ONNX_COMPARISON_OPS_TO_NUMPY_IMPL_FLOAT: Dict[str, Callable[..., Tuple[numpy.ndarray, ...]]] = {
     "Or": numpy_or_float,
     "Not": numpy_not_float,
     "Greater": numpy_greater_float,
     "GreaterOrEqual": numpy_greater_or_equal_float,
```

## concrete/ml/onnx/ops_impl.py

```diff
@@ -1,31 +1,35 @@
 """ONNX ops implementation in python + numpy."""
 
 # pylint: disable=too-many-lines
 from inspect import signature
-from typing import List, Optional, Sequence, Set, Tuple, Union
+from typing import Iterable, List, Optional, Sequence, Set, Tuple, Union
 
 import numpy
 import onnx
+import onnx.helper
 from brevitas.function import max_int, min_int
-from concrete.numpy import univariate
-from concrete.onnx import conv as cnp_conv
-from concrete.onnx import maxpool as cnp_maxpool
+from concrete.fhe import conv as cnp_conv
+from concrete.fhe import maxpool as cnp_maxpool
+from concrete.fhe import univariate
 from scipy import special
 from typing_extensions import SupportsIndex
 
 from ..common.debugging import assert_false, assert_true
 from .onnx_impl_utils import (
     compute_onnx_pool_padding,
     numpy_onnx_pad,
     onnx_avgpool_compute_norm_const,
 )
 
 
-# FIXME: to remove once https://github.com/zama-ai/concrete-ml-internal/issues/1117 is done.
+class RawOpOutput(numpy.ndarray):
+    """Type construct that marks an ndarray as a raw output of a quantized op."""
+
+
 # This function is only used for comparison operators that return boolean values by default.
 def cast_to_float(inputs):
     """Cast values to floating points.
 
     Args:
         inputs (Tuple[numpy.ndarray]): The values to consider.
 
@@ -41,74 +45,82 @@
     ONNX functions will take inputs which can be either quantized or float. Some functions
     only take quantized inputs, but some functions take both types. For mixed functions
     we need to tag the parameters that do not need quantization. Thus quantized ops
     can know which inputs are not QuantizedArray and we avoid unnecessary wrapping of float
     values as QuantizedArrays.
     """
 
-    def __init__(self, function, non_quant_params: Set[str]):
+    def __init__(self, function, non_quant_params: Set[str], output_is_raw: bool = False):
         """Create the mixed function and raw parameter list.
 
         Args:
             function (Any): function to be decorated
             non_quant_params: Set[str]: set of parameters that will not be quantized (stored
                 as numpy.ndarray)
+            output_is_raw (bool): indicates whether the op outputs a value that should
+                not be quantized
         """
 
         self.non_quant_params: Set[str] = non_quant_params
         bad_non_quant_params = set(non_quant_params).difference(set(signature(function).parameters))
         assert_true(
             len(bad_non_quant_params) == 0,
             f"ONNX function {function.__name__} tagged with invalid integer parameters: "
             ",".join(bad_non_quant_params),
         )
         self.function = function  # type: ignore
+        self.output_is_raw = output_is_raw
 
     def __call__(self, *args, **kwargs):
         """Call the wrapped numpy function.
 
         Args:
             args (tuple[Any]): function arguments
             kwargs (dict[str, Any]): function key value arguments
 
         Returns:
             result (Any): result of calling the wrapped function on the input arguments
         """
-        return self.function(*args, **kwargs)
+        result = self.function(*args, **kwargs)
+        if self.output_is_raw:
+            result = tuple(r.view(RawOpOutput) for r in result)
+        return result
 
     @property
     def __name__(self):
         """Return the wrapped function name.
 
         Returns:
             result (str): name of the wrapped function
         """
         return self.function.__name__
 
 
-def onnx_func_raw_args(*args):
+def onnx_func_raw_args(*args, output_is_raw: bool = False):
     """Decorate a numpy onnx function to flag the raw/non quantized inputs.
 
     Args:
         *args (tuple[Any]): function argument names
+        output_is_raw (bool): marks the function as returning raw
+            values that should not be quantized
 
     Returns:
         result (ONNXMixedFunction): wrapped numpy function with a list of mixed arguments
     """
 
     def decoration(function):
         """Construct the mixed function class.
 
         Args:
             function (Any): function to be decorated
 
         Returns:
             result (ONNXMixedFunction): wrapped numpy function with a list of mixed arguments
         """
-        return ONNXMixedFunction(function, set(args))
+        return ONNXMixedFunction(function, set(args), output_is_raw)
 
     return decoration
 
 
 def numpy_where_body(
     c: numpy.ndarray,
     t: numpy.ndarray,
@@ -124,18 +136,17 @@
         t (numpy.ndarray): True operand.
         f (numpy.ndarray): False operand.
 
     Returns:
         numpy.ndarray: numpy.where(c, t, f)
 
     """
-
-    # FIXME: can it be improved with a native numpy.where in Concrete Numpy?
-    # https://github.com/zama-ai/concrete-numpy-internal/issues/1429
-
+    # Use numpy.where (it is currently supported by CN) once we investigate why it outputs a
+    # a different dtype then the following workaround
+    # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/2738
     return c * t + (1.0 - c) * f
 
 
 def numpy_where(
     c: numpy.ndarray,
     t: numpy.ndarray,
     f: numpy.ndarray,
@@ -263,16 +274,15 @@
         transB (int): Whether B should be transposed. The type is kept as int as it's the
             type used by ONNX and it can easily be interpreted by python as a boolean.
             Defaults to 0.
 
     Returns:
         Tuple[numpy.ndarray]: The tuple containing the result tensor
     """
-    # If alpha and beta are integer, apply the int type for concrete-numpy
-    # to see they are integers (see issue #277)
+    # If alpha and beta are integer, apply the int type for Concrete to see they are integers
     processed_alpha = int(alpha) if round(alpha) == alpha else alpha
     processed_beta = int(beta) if round(beta) == beta else beta
 
     a_prime = numpy.transpose(a) if transA else a
     b_prime = numpy.transpose(b) if transB else b
     c_prime: Union[numpy.ndarray, float] = c if c is not None else 0
 
@@ -716,20 +726,28 @@
         a (numpy.ndarray): Input tensor
         b (numpy.ndarray): Input tensor
 
     Returns:
         Tuple[numpy.ndarray]: Output tensor
     """
 
-    # FIXME: remove this once https://github.com/zama-ai/concrete-ml-internal/issues/857 is
-    # explained
+    # Remove the where op once the following issue is explained
+    # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/857
     bp = numpy_where_body(b != 0, b, 1)
-    ans = numpy.divide(a, bp)
 
-    return (ans,)
+    # Check if processing non-encrypted constants.
+    # We handle non-encrypted constants differently because integer constants
+    # must use `floor_divide`
+    if isinstance(a, RawOpOutput) and numpy.issubdtype(a.dtype, numpy.integer):
+        return (numpy.floor_divide(a, bp),)
+
+    # This branch may be processing encrypted data or float clear constants that are initializers
+    # In FHE for integer values we want floating point behavior that produces TLUs without
+    # loss of precision.
+    return (numpy.divide(a, bp),)
 
 
 def numpy_mul(
     a: numpy.ndarray,
     b: numpy.ndarray,
 ) -> Tuple[numpy.ndarray]:
     """Compute mul in numpy according to ONNX spec.
@@ -777,15 +795,15 @@
         x (numpy.ndarray): Input tensor
 
     Returns:
         Tuple[numpy.ndarray]: Output tensor
     """
 
     # Epsilon is here to avoid problems with 0 or negative values, which may happen when Concrete
-    # Numpy creates the table (even if these problematic values would normally never be used)
+    # creates the table (even if these problematic values would normally never be used)
     epsilon = 10**-8
 
     return (numpy.log(numpy.maximum(x, epsilon)),)
 
 
 @onnx_func_raw_args("slope")
 def numpy_prelu(
@@ -896,15 +914,14 @@
     Returns:
         Tuple[numpy.ndarray]: Output tensor
     """
 
     return (numpy.logical_not(x),)
 
 
-# FIXME: to remove once https://github.com/zama-ai/concrete-ml-internal/issues/1117 is done.
 def numpy_not_float(
     x: numpy.ndarray,
 ) -> Tuple[numpy.ndarray]:
     """Compute not in numpy according to ONNX spec and cast outputs to floats.
 
     See https://github.com/onnx/onnx/blob/main/docs/Changelog.md#Not-1
 
@@ -933,15 +950,14 @@
     Returns:
         Tuple[numpy.ndarray]: Output tensor
     """
 
     return (numpy.greater(x, y),)
 
 
-# FIXME: to remove once https://github.com/zama-ai/concrete-ml-internal/issues/1117 is done.
 def numpy_greater_float(
     x: numpy.ndarray,
     y: numpy.ndarray,
 ) -> Tuple[numpy.ndarray]:
     """Compute greater in numpy according to ONNX spec and cast outputs to floats.
 
     See https://github.com/onnx/onnx/blob/main/docs/Changelog.md#Greater-13
@@ -972,15 +988,14 @@
     Returns:
         Tuple[numpy.ndarray]: Output tensor
     """
 
     return (numpy.greater_equal(x, y),)
 
 
-# FIXME: to remove once https://github.com/zama-ai/concrete-ml-internal/issues/1117 is done.
 def numpy_greater_or_equal_float(
     x: numpy.ndarray,
     y: numpy.ndarray,
 ) -> Tuple[numpy.ndarray]:
     """Compute greater or equal in numpy according to ONNX specs and cast outputs to floats.
 
     See https://github.com/onnx/onnx/blob/main/docs/Changelog.md#GreaterOrEqual-12
@@ -1011,15 +1026,14 @@
     Returns:
         Tuple[numpy.ndarray]: Output tensor
     """
 
     return (numpy.less(x, y),)
 
 
-# FIXME: to remove once https://github.com/zama-ai/concrete-ml-internal/issues/1117 is done.
 def numpy_less_float(
     x: numpy.ndarray,
     y: numpy.ndarray,
 ) -> Tuple[numpy.ndarray]:
     """Compute less in numpy according to ONNX spec and cast outputs to floats.
 
     See https://github.com/onnx/onnx/blob/main/docs/Changelog.md#Less-13
@@ -1050,15 +1064,14 @@
     Returns:
         Tuple[numpy.ndarray]: Output tensor
     """
 
     return (numpy.less_equal(x, y),)
 
 
-# FIXME: to remove once https://github.com/zama-ai/concrete-ml-internal/issues/1117 is done.
 def numpy_less_or_equal_float(
     x: numpy.ndarray,
     y: numpy.ndarray,
 ) -> Tuple[numpy.ndarray]:
     """Compute less or equal in numpy according to ONNX spec and cast outputs to floats.
 
     See https://github.com/onnx/onnx/blob/main/docs/Changelog.md#LessOrEqual-12
@@ -1087,15 +1100,15 @@
     Returns:
         Tuple[numpy.ndarray]: Output tensor
     """
 
     return (x,)
 
 
-@onnx_func_raw_args("newshape")
+@onnx_func_raw_args("newshape", "allowzero")
 def numpy_reshape(
     x: numpy.ndarray, newshape: numpy.ndarray, *, allowzero=0
 ) -> Tuple[numpy.ndarray]:
     """Compute reshape in numpy according to ONNX spec.
 
     See https://github.com/onnx/onnx/blob/main/docs/Changelog.md#Reshape-13
 
@@ -1120,16 +1133,15 @@
     Args:
         x (numpy.ndarray): Input tensor
         perm (numpy.ndarray): Permutation of the axes
 
     Returns:
         Tuple[numpy.ndarray]: Output tensor
     """
-    # FIXME: #931, remove the no-cover once #931 is done
-    return (numpy.transpose(x, axes=perm),)  # pragma: no cover
+    return (numpy.transpose(x, axes=perm),)
 
 
 @onnx_func_raw_args("b")
 def numpy_conv(
     x: numpy.ndarray,
     w: numpy.ndarray,
     b: Optional[numpy.ndarray] = None,
@@ -1163,15 +1175,15 @@
 
     """
 
     # Convert the inputs to tensors to compute conv using torch
     assert_true(len(kernel_shape) == 2, "The convolution operator currently supports only 2-d")
     assert_true(
         bool(numpy.all(numpy.asarray(dilations) == 1)),
-        "The convolution operator in Concrete Numpy does not support dilation",
+        "The convolution operator in Concrete does not support dilation",
     )
 
     weight_channels = x.shape[1]
     assert_true(
         w.shape[1] == weight_channels / group,
         f"Expected number of channels in weight to be {weight_channels / group} (C / group). Got "
         f"{w.shape[1]}.",
@@ -1324,15 +1336,15 @@
         ceil_mode=ceil_mode,
         storage_order=storage_order,
     )
 
     return (res,)
 
 
-@onnx_func_raw_args("pads")
+@onnx_func_raw_args("pads", "constant_value")
 def numpy_pad(
     data: numpy.ndarray,
     pads: numpy.ndarray,
     constant_value: Union[numpy.ndarray, None] = None,
     *,
     mode: str,
 ) -> Tuple[numpy.ndarray]:
@@ -1346,38 +1358,47 @@
         constant_value (float): Constant value to use for padding
         mode (str): padding mode: constant/edge/reflect
 
     Returns:
         res (numpy.ndarray): Padded tensor
     """
 
-    assert_true(bool(numpy.all(pads == 0)), "Padding operator supported only with all pads at zero")
     assert_true(mode == "constant", "Padding only supported with a constant pad value")
     assert_true(
         constant_value is None or constant_value == 0, "Pad only accepts a constant padding with 0s"
     )
 
-    return (data,)
+    # Pad the input if needed
+    x_pad = numpy_onnx_pad(data, tuple(pads))
+
+    return (x_pad,)
 
 
 def numpy_cast(data: numpy.ndarray, *, to: int) -> Tuple[numpy.ndarray]:
     """Execute ONNX cast in Numpy.
 
-    Supports only booleans for now, which are converted to integers.
+    For traced values during compilation, it supports only booleans, which are converted to float.
+    For raw values (used in constant folding or shape computations), any cast is allowed.
 
     See: https://github.com/onnx/onnx/blob/main/docs/Operators.md#Cast
 
     Args:
         data (numpy.ndarray): Input encrypted tensor
         to (int): integer value of the onnx.TensorProto DataType enum
 
     Returns:
         result (numpy.ndarray): a tensor with the required data type
     """
+    # For raw values, any cast is fine
+    if isinstance(data, RawOpOutput):
+        return (data.astype(onnx.helper.tensor_dtype_to_np_dtype(to)).view(RawOpOutput),)
+
     assert_true(to == onnx.TensorProto.BOOL)
+
+    # Will be used for traced values
     return (data.astype(numpy.float64),)
 
 
 def numpy_batchnorm(
     x: numpy.ndarray,
     scale: numpy.ndarray,
     bias: numpy.ndarray,
@@ -1480,15 +1501,14 @@
 
     Returns:
         Tuple[numpy.ndarray]: Output tensor
     """
     return (numpy.logical_or(a, b),)
 
 
-# FIXME: to remove once https://github.com/zama-ai/concrete-ml-internal/issues/1117 is done.
 def numpy_or_float(
     a: numpy.ndarray,
     b: numpy.ndarray,
 ) -> Tuple[numpy.ndarray]:
     """Compute or in numpy according to ONNX spec and cast outputs to floats.
 
     See https://github.com/onnx/onnx/blob/main/docs/Changelog.md#Or-7
@@ -1581,15 +1601,16 @@
     # Numpy's axis parameter only handles tuple of integers (or None) as input while ONNX's axes
     # parameter is an array (or None)
     axis = tuple(axes) if axes is not None else None
 
     # Numpy's keepdims parameter is a boolean while ONNX's one is an int (0 or 1). Even though
     # Python handles them equivalently, we need to manually convert it as mypy doesn't accept this
     # type difference
-    # FIXME #2050 : Find a way to make axis of type Union[SupportsIndex, Sequence[SupportsIndex]
+    # Find a way to make axis of type Union[SupportsIndex, Sequence[SupportsIndex]
+    # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/2050
     return (numpy.sum(a, axis=axis, keepdims=bool(keepdims)),)  # type: ignore
 
 
 @onnx_func_raw_args("scale", "zero_point", "bit_width")
 def numpy_brevitas_quant(
     x: numpy.ndarray,
     scale: float,
@@ -1730,22 +1751,192 @@
     Returns:
         Tuple[numpy.ndarray]: Output tensor.
     """
     return (numpy.concatenate(x, axis=axis),)
 
 
 @onnx_func_raw_args("axis")
-def numpy_unsqueeze(x: numpy.ndarray, axis: list) -> Tuple[numpy.ndarray]:
+def numpy_unsqueeze(x: numpy.ndarray, axis: Iterable) -> Tuple[numpy.ndarray]:
     """Apply the unsqueeze operator in numpy according to ONNX spec.
 
     See https://github.com/onnx/onnx/blob/main/docs/Changelog.md#unsqueeze-13
 
     Args:
         x (numpy.ndarray): Input tensor.
-        axis (list): List of the axis to unsqueeze.
+        axis (Iterable): Tuple of the axis to unsqueeze.
 
     Returns:
         Tuple[numpy.ndarray]: Output tensor.
     """
-    for ax in axis:
-        x = numpy.expand_dims(x, axis=ax)
+    for i, ax in enumerate(sorted(axis)):
+        # Add a dimension to x following the axis.
+        # The axis must be shifted by the number of dimensions already
+        # added to x (thus the ax + i).
+        x = numpy.expand_dims(x, axis=ax + i)
     return (x,)
+
+
+@onnx_func_raw_args("axis")
+def numpy_squeeze(x: numpy.ndarray, axis=None) -> Tuple[numpy.ndarray]:
+    """Apply the squeeze operator in numpy according to ONNX spec.
+
+    See https://github.com/onnx/onnx/blob/main/docs/Changelog.md#squeeze-13
+
+    Args:
+        x (numpy.ndarray): Input tensor.
+        axis: Tuple of the axis to squeeze.
+
+    Returns:
+        Tuple[numpy.ndarray]: Output tensor.
+    """
+    return (numpy.squeeze(x, axis=tuple(axis) if axis is not None else axis),)
+
+
+@onnx_func_raw_args(output_is_raw=True)
+def numpy_shape(x: numpy.ndarray) -> Tuple[numpy.ndarray]:
+    """Return the shape of the input tensor.
+
+    See https://github.com/onnx/onnx/blob/main/docs/Changelog.md#shape-13
+
+    Args:
+        x (numpy.ndarray): Input tensor
+
+    Returns:
+        Tuple[numpy.ndarray]: outputs an 1D int64 tensor (per ONNX spec)
+    """
+
+    # As this op is used in a graph to take the shape of an intermediary encrypted
+    # tensor, it marks its output as a raw output
+    return (numpy.asarray(x.shape, numpy.int64).view(RawOpOutput),)
+
+
+@onnx_func_raw_args("shape", "value", output_is_raw=True)
+def numpy_constant_of_shape(shape: numpy.ndarray, *, value=0.0) -> Tuple[numpy.ndarray]:
+    """Create a constant tensor with a specified shape.
+
+    See https://github.com/onnx/onnx/blob/main/docs/Operators.md#ConstantOfShape
+
+    Args:
+        shape (numpy.ndarray): the shape of the constant tensor
+        value (Optional[Any]): the constant value
+
+    Returns:
+        result(Tuple[numpy.ndarray]): the constant tensor
+    """
+
+    return (numpy.ones(shape, dtype=numpy.int64) * value,)
+
+
+@onnx_func_raw_args("starts", "ends", "steps", "axes")
+def numpy_slice(
+    x: numpy.ndarray,
+    starts: numpy.ndarray,
+    ends: numpy.ndarray,
+    axes: Optional[numpy.ndarray],
+    steps: Optional[numpy.ndarray],
+) -> Tuple[numpy.ndarray]:
+    """Slice the input according to ONNX spec.
+
+    See https://github.com/onnx/onnx/blob/main/docs/Changelog.md#slice-13
+
+    Args:
+        x (numpy.ndarray): input tensor to slice
+        starts (numpy.ndarray): the starting indices, one for each axis to slice
+        ends (numpy.ndarray): the ending indices, one for each axis to slice
+        axes (numpy.ndarray): the axis indices, default is all axes
+        steps (numpy.ndarray): the steps along each axis, defaults to 1
+
+    Returns:
+        result (Tuple[numpy.ndarray]): the slice(s) of the input tensor as a new tensor
+    """
+
+    slices = []
+    if steps is None:
+        steps = numpy.ones_like(starts)
+
+    if axes is None:
+        axes = numpy.arange(x.ndim)
+        assert_true(
+            starts.shape[0] == x.ndim and steps.shape[0] == x.ndim,
+            "The Starts and Ends parameter of Slice must have the same "
+            "number of elements as the number of axes of the input when the axes "
+            f"parameter is None. Got starts with {starts.shape[0]} elements, ends "
+            f"with {steps.shape[0]} elements, while the input has {x.ndim} dimensions.",
+        )
+    else:
+        # Adjust negative axes
+        axes = axes.copy()
+        axes[axes < 0] += x.ndim
+        assert_true(
+            steps.shape[0] == starts.shape[0]
+            and ends.shape[0] == starts.shape[0]
+            and axes.shape[0] == starts.shape[0],
+            "The Starts and Ends parameter of Slice must have the same "
+            "number of elements as the axes parameter. Got starts with "
+            f"{starts.shape[0]} elements, ends "
+            f"with {steps.shape[0]} elements, while the axes had {axes.shape[0]} dimensions.",
+        )
+
+    # All negative values in starts[i] and ends[i] have dims[axes[i]] added to them,
+    # where dims are the dimensions of input. Then start[axes[i]] is the adjusted starts[i]
+    # is clamped into the range [0, dims[axes[i]]] for positive stepping and
+    # [0, dims[axes[i]]-1] for negative stepping.
+
+    # The clamping for the adjusted ends[i] depends on the sign of steps[i] and must
+    # accommodate copying 0 through dims[axes[i]] elements,
+    # so for positive stepping end[axes[i]] is clamped to [0, dims[axes[i]]],
+    # while for negative stepping it is clamped to [-1, dims[axes[i]]-1].
+
+    starts = starts.copy()
+    ends = ends.copy()
+    for k in range(starts.size):
+        if starts[k] < 0:
+            starts[k] += x.shape[axes[k]]
+        if ends[k] < 0:
+            ends[k] += x.shape[axes[k]]
+
+        if steps[k] < 0:
+            starts[k] = numpy.clip(starts[k], -x.shape[axes[k]] - 1, -1)
+            ends[k] = numpy.clip(ends[k], -x.shape[axes[k]] - 1, -1)
+        else:
+            starts[k] = numpy.clip(starts[k], 0, x.shape[axes[k]] - 1)
+            ends[k] = numpy.clip(ends[k], 0, x.shape[axes[k]])
+
+    # Check there are no duplicates
+    assert_true(
+        len(numpy.unique(axes)) == len(axes), "Axes parameter to Slice contained duplicates"
+    )
+
+    # Initialize slices to take the whole input tensor
+    slices = [slice(0, int(x.shape[axis]), 1) for axis in range(x.ndim)]
+
+    for idx, axis in enumerate(axes):
+        slices[axis] = slice(int(starts[idx]), int(ends[idx]), int(steps[idx]))
+
+    return (x[tuple(slices)],)
+
+
+@onnx_func_raw_args("indices", "axis")
+def numpy_gather(
+    x: numpy.ndarray, indices: numpy.ndarray, *, axis: int = 0
+) -> Tuple[numpy.ndarray]:
+    """Gather indices according to ONNX spec.
+
+    Args:
+        x (numpy.ndarray): input tensor to slice
+        indices (numpy.ndarray): the indices at which to extract values
+        axis (int): the axis along which to extract values (defaults to 0)
+
+    Returns:
+        result (Tuple[numpy.ndarray]): the values gathered from the input tensor as a new tensor
+    """
+
+    slices: List[Union[slice, numpy.ndarray]] = []
+
+    for axis_iter in range(x.ndim):
+        # Support both negative and positive axis
+        if (axis >= 0 and axis_iter == axis) or (axis < 0 and axis_iter == x.ndim + axis):
+            slices.append(indices)
+        else:
+            slices.append(slice(0, x.shape[axis_iter]))
+
+    return (x[tuple(slices)],)
```

## concrete/ml/pytest/torch_models.py

```diff
@@ -1,14 +1,43 @@
 """Torch modules for our pytests."""
+
+# pylint: disable=too-many-lines
+from typing import Union
+
 import brevitas.nn as qnn
 import numpy
 import torch
+from brevitas.quant import Int8ActPerTensorFloat, Int8WeightPerTensorFloat
 from torch import nn
 from torch.nn.utils import prune
 
+# pylint: disable=too-many-lines
+
+
+class SimpleNet(torch.nn.Module):
+    """Fake torch model used to generate some onnx."""
+
+    def __init__(self) -> None:
+        super().__init__()
+        self.scale = 2.2
+        self.offset = 1.1
+
+    def forward(self, inputs):
+        """Forward function.
+
+        Arguments:
+            inputs: the inputs of the model.
+
+        Returns:
+            torch.Tensor: the result of the computation
+        """
+        res = (inputs * self.scale) + self.offset
+        res = torch.relu(inputs)
+        return res
+
 
 class FCSmall(nn.Module):
     """Torch model for the tests."""
 
     def __init__(self, input_output, activation_function):
         super().__init__()
         self.fc1 = nn.Linear(in_features=input_output, out_features=input_output)
@@ -162,27 +191,29 @@
         x = self.fc3(x)
         return x
 
 
 class CNNInvalid(nn.Module):
     """Torch CNN model for the tests."""
 
-    def __init__(self, activation_function, padding, groups, gather_slice):
+    def __init__(self, activation_function, groups):
         super().__init__()
 
+        padding = True
+
         self.activation_function = activation_function()
         self.flatten_function = lambda x: torch.flatten(x, 1)
         self.conv1 = nn.Conv2d(3, 6, 5)
         self.pool = nn.AvgPool2d(2, 2, padding=1) if padding else nn.AvgPool2d(2, 2)
         self.conv2 = nn.Conv2d(6, 16, 5, groups=2) if groups else nn.Conv2d(6, 16, 5)
         self.fc1 = nn.Linear(16 * (5 + padding * 1) * (5 + padding * 1), 120)
         self.fc2 = nn.Linear(120, 84)
         self.fc3 = nn.Linear(84, 10)
 
-        self.gather_slice = gather_slice
+        self.gather_slice = True
 
     def forward(self, x):
         """Forward pass.
 
         Args:
             x: the input of the NN
 
@@ -193,15 +224,16 @@
         x = self.pool(self.activation_function(self.conv2(x)))
         x = self.flatten_function(x)
         x = self.activation_function(self.fc1(x))
         x = self.activation_function(self.fc2(x))
         x = self.fc3(x)
         # Produce a Gather and Slice which are not supported
         if self.gather_slice:
-            return x[0, 0:-1:2]
+            x = x[0, 0:-1:2]
+        x = torch.mean(x)
         return x
 
 
 class CNNGrouped(nn.Module):
     """Torch CNN model with grouped convolution for compile torch tests."""
 
     def __init__(self, input_output, activation_function, groups):
@@ -282,14 +314,45 @@
 
         Returns:
             the output of the NN
         """
         return self.act(x + y)
 
 
+class MultiInputNNConfigurable(nn.Module):
+    """Torch model to test multiple inputs forward."""
+
+    layer1: nn.Module
+    layer2: nn.Module
+
+    def __init__(self, use_conv, use_qat, input_output, n_bits):  # pylint: disable=unused-argument
+        super().__init__()
+
+        if use_conv:
+            self.layer1 = nn.Conv2d(input_output[0], input_output[0], 1, 1, 0)
+            self.layer2 = nn.Conv2d(input_output[0], input_output[0], 1, 1, 0)
+        else:
+            self.layer1 = nn.Linear(input_output, input_output)
+            self.layer2 = nn.Linear(input_output, input_output)
+
+    def forward(self, x, y):
+        """Forward pass.
+
+        Args:
+            x: the first input of the NN
+            y: the second input of the NN
+
+        Returns:
+            the output of the NN
+        """
+        x = self.layer1(x)
+        y = self.layer2(y)
+        return self.layer1(x + y)
+
+
 class BranchingModule(nn.Module):
     """Torch model with some branching and skip connections."""
 
     # pylint: disable-next=unused-argument
     def __init__(self, input_output, activation_function):
         super().__init__()
 
@@ -414,38 +477,45 @@
         Returns:
             the output of the NN
         """
         x = self.act(self.fc1(x))
         results = []
         for module in self.ifc:
             results.append(module(x))
+
         # Use torch.stack which creates Unsqueeze operators for each module
         # and a final Concat operator.
-        results = torch.stack(results)
-        return results
+        return torch.stack(results)
 
 
 class MultiOpOnSingleInputConvNN(nn.Module):
     """Network that applies two quantized operations on a single input."""
 
-    def __init__(self):
+    def __init__(self, can_remove_input_tlu: bool):
         super().__init__()
+        self.can_remove_input_tlu = can_remove_input_tlu
         self.conv1 = nn.Conv2d(1, 8, 3)
         self.conv2 = nn.Conv2d(1, 8, 3)
 
     def forward(self, x):
         """Forward pass.
 
         Args:
             x: the input of the NN
 
         Returns:
             the output of the NN
         """
-        layer1_out = torch.relu(self.conv1(x))
+
+        # The quantizer for this network can be moved in the clear if the
+        # input is fed directly to two conv layers that have the same quantizer.
+        # To ensure the quantizer is performed in FHE, a univariate op is applied
+        # before _one_ of the convolutions
+        y = x if self.can_remove_input_tlu else torch.sigmoid(x)
+        layer1_out = torch.relu(self.conv1(y))
         layer2_out = torch.relu(self.conv2(x))
         return layer1_out + layer2_out
 
 
 class FCSeq(nn.Module):
     """Torch model that should generate MatMul->Add ONNX patterns.
 
@@ -818,40 +888,45 @@
         x = self.act(x)
         return x
 
 
 class SingleMixNet(nn.Module):
     """Torch model that with a single conv layer that produces the output, e.g. a blur filter."""
 
-    def __init__(self, use_conv, use_qat, inp_size, n_bits):  # pylint: disable=unused-argument
+    mixing_layer: Union[nn.Module, nn.Sequential]
+
+    def __init__(self, use_conv, use_qat, inp_size, n_bits):
         super().__init__()
 
         if use_conv:
             # Initialize a blur filter float weights
             np_weights = numpy.asarray([[[[1, 1, 1], [1, 4, 1], [1, 1, 1]]]])
 
             if use_qat:
                 self.mixing_layer = nn.Sequential(
                     qnn.QuantIdentity(bit_width=n_bits),
                     qnn.QuantConv2d(1, 1, 3, stride=1, bias=True, weight_bit_width=n_bits),
                 )
+                layer_obj = self.mixing_layer[1]
             else:
                 self.mixing_layer = nn.Conv2d(1, 1, 3, stride=1, bias=True)
+                layer_obj = self.mixing_layer
         else:
             # Initialize a linear layer with 1s
             np_weights = numpy.asarray([[1] * inp_size])
             if use_qat:
                 self.mixing_layer = nn.Sequential(
                     qnn.QuantIdentity(bit_width=n_bits),
                     qnn.QuantLinear(inp_size, inp_size, bias=True, weight_bit_width=n_bits),
                 )
+                layer_obj = self.mixing_layer[1]
             else:
                 self.mixing_layer = nn.Linear(inp_size, inp_size, bias=True)
+                layer_obj = self.mixing_layer
 
-        layer_obj = self.mixing_layer[1] if use_qat else self.mixing_layer
         layer_obj.weight.data = torch.from_numpy(np_weights).float()
         layer_obj.bias.data = torch.rand(size=(1,))
 
     def forward(self, x):
         """Execute the single convolution.
 
         Args:
@@ -860,14 +935,53 @@
         Returns:
             the output of the NN
         """
 
         return self.mixing_layer(x)
 
 
+class DoubleQuantQATMixNet(nn.Module):
+    """Torch model that with two different quantizers on the input.
+
+    Used to test that it keeps the input TLU.
+    """
+
+    def __init__(self, use_conv, use_qat, inp_size, n_bits):  # pylint: disable=unused-argument
+        super().__init__()
+
+        # A first quantizer
+        self.quant1 = qnn.QuantIdentity(bit_width=n_bits)
+        # A different quantizer
+        self.quant2 = qnn.QuantIdentity(bit_width=n_bits + 1)
+        self.quant3 = qnn.QuantIdentity(bit_width=n_bits)
+
+        if use_conv:
+            self.mixing_layer = qnn.QuantConv2d(
+                1, 1, 3, stride=1, bias=True, weight_bit_width=n_bits
+            )
+        else:
+            self.mixing_layer = qnn.QuantLinear(
+                inp_size, inp_size, bias=True, weight_bit_width=n_bits
+            )
+
+    def forward(self, x):
+        """Execute the single convolution.
+
+        Args:
+            x: the input of the NN
+
+        Returns:
+            the output of the NN
+        """
+
+        left_x1 = self.quant1(x)
+        right_x2 = self.quant2(x)
+        return self.mixing_layer(self.quant3(left_x1 + right_x2))
+
+
 class TorchSum(nn.Module):
     """Torch model to test the ReduceSum ONNX operator in a leveled circuit."""
 
     def __init__(self, dim=(0,), keepdim=True):
         """Initialize the module.
 
         Args:
@@ -910,7 +1024,368 @@
         """
         torch_sum = x.sum(dim=self.dim, keepdim=self.keepdim)
 
         # Add an additional operator that requires a TLU in order to force this circuit to
         # handle a PBS without actually changing the results
         torch_sum = torch_sum + torch_sum % 2 - torch_sum % 2
         return torch_sum
+
+
+class NetWithConstantsFoldedBeforeOps(nn.Module):
+    """Torch QAT model that does not quantize the inputs."""
+
+    def __init__(
+        self,
+        hparams: dict,
+        bits: int,
+        act_quant=Int8ActPerTensorFloat,
+        weight_quant=Int8WeightPerTensorFloat,
+    ):
+        super().__init__()
+        self.hparams = hparams
+        self.dense1 = qnn.QuantLinear(
+            hparams["n_feats"],
+            hparams["hidden_dim"],
+            weight_quant=weight_quant,
+            weight_bit_width=bits,
+            bias=True,
+        )
+        self.dp1 = qnn.QuantDropout(0.1)
+        self.act1 = qnn.QuantReLU(act_quant=act_quant, bit_width=bits)
+
+        self.dense2 = qnn.QuantLinear(
+            hparams["hidden_dim"],
+            1,
+            weight_bit_width=bits,
+            weight_quant=weight_quant,
+            bias=True,
+        )
+
+    def forward(self, x):
+        """Forward pass.
+
+        Args:
+            x (torch.tensor): The input of the model
+
+        Returns:
+            torch.tensor: Output of the network
+        """
+
+        # Note here that the input is not quantized, it is passed to the linear layer directly
+        x = self.dense1(x)
+        x = self.dp1(x)
+        x = self.act1(x)
+
+        x = self.dense2(x)
+        return x
+
+
+class ShapeOperationsNet(nn.Module):
+    """Torch QAT model that reshapes the input."""
+
+    def __init__(self, is_qat):
+        super().__init__()
+        self.is_qat = is_qat
+        if is_qat:
+            self.input_quant = qnn.QuantIdentity(bit_width=8)
+
+    def forward(self, x):
+        """Forward pass.
+
+        Args:
+            x (torch.tensor): The input of the model
+
+        Returns:
+            torch.tensor: Output of the network
+        """
+
+        def shufflenet_shuffle(x: torch.Tensor, groups: int) -> torch.Tensor:
+            """Shuffle the channels: split them into two groups and then recombine them.
+
+            In ShuffleNet, conv ops operate over the two branches, but here they are skipped
+            for simplicity.
+
+            Args:
+                x (torch.Tensor): the tensor that will be shuffled
+                groups (int): the number of groups of channels to
+
+            Returns:
+                torch.Tensor: the tensor containing the groups of channels of the input tensor
+            """
+
+            batchsize, num_channels, height, width = x.size()
+            channels_per_group = num_channels // groups
+
+            x = x.reshape(batchsize, groups, channels_per_group, height, width)
+            x = torch.transpose(x, 1, 2).contiguous()
+            x = x.reshape(batchsize, -1, height, width)
+
+            return x
+
+        if self.is_qat:
+            x = self.input_quant(x)
+        chunk1, chunk2 = x.chunk(2, dim=1)
+        out = torch.cat((chunk1, chunk2), dim=1)
+        return shufflenet_shuffle(out, 2)
+
+
+class PaddingNet(nn.Module):
+    """Torch QAT model that applies various padding patterns."""
+
+    def __init__(self):
+        super().__init__()
+
+        # Use a QAT network to allow the torch result to be the same as the CML result
+        self.input_quant = qnn.QuantIdentity(bit_width=8)
+
+    def forward(self, x):
+        """Forward pass.
+
+        Args:
+            x (torch.tensor): The input of the model
+
+        Returns:
+            torch.tensor: Output of the network
+        """
+
+        # Quantize input
+        x = self.input_quant(x)
+
+        # Torch pads starting from the last dimensions of the tensor moving forward, with
+        # potentially different padding at the start/end of the axes
+        # for example a 4d tensor NCHW, padded with [1, 2, 2, 3] is padded
+        # along the last 2 dimensions, with 1 cell to the left and 2 to the right (dimension 4: W)
+        # and 2 cells at the top and 3 at the bottom (dimension 3: H)
+        x = torch.nn.functional.pad(x, (3, 2))
+        x = torch.nn.functional.pad(x, (1, 2, 3, 4))
+
+        # Concrete ML only supports padding on the last two dimensions as this is the
+        # most common setting
+        x = torch.nn.functional.pad(x, (1, 1, 2, 2, 0, 0, 0, 0))
+        return x
+
+
+# pylint: disable=too-many-return-statements
+class QNNFashionMNIST(torch.nn.Module):
+    """A small quantized network with Brevitas for FashionMNIST classification."""
+
+    # pylint: disable=invalid-name
+    layers = [
+        # Layer 1
+        (
+            "Conv2d",
+            {"in_channels": 1, "out_channels": 12, "kernel_size": 2, "stride": 1, "padding": 0},
+        ),
+        ("ReLU",),
+        ("AvgPool2d", {"kernel_size": 2, "stride": 2, "padding": 0}),
+        ("BatchNorm2d", {"num_features": 12}),
+        ("Identity",),
+        # Layer 2
+        (
+            "Conv2d",
+            {"in_channels": 12, "out_channels": 16, "kernel_size": 3, "stride": 1, "padding": 0},
+        ),
+        ("ReLU",),
+        ("AvgPool2d", {"kernel_size": 2, "stride": 2, "padding": 0}),
+        ("BatchNorm2d", {"num_features": 16}),
+        ("Identity",),
+        # Layer 3
+        (
+            "Conv2d",
+            {"in_channels": 16, "out_channels": 20, "kernel_size": 2, "stride": 1, "padding": 0},
+        ),
+        ("ReLU",),
+        ("AvgPool2d", {"kernel_size": 2, "stride": 1, "padding": 0}),
+        ("BatchNorm2d", {"num_features": 20}),
+        # Layer 4
+        ("Identity",),
+        ("Flatten",),
+        ("Identity",),
+        # Layer 5
+        ("Linear", {"in_features": 20 * 3 * 3, "out_features": 100}),
+        ("ReLU",),
+        ("Dropout2d", {"p": 0.5}),
+        # Layer 6
+        ("Linear", {"in_features": 100, "out_features": 50}),
+        ("ReLU",),
+        # Layer 7
+        ("Linear", {"in_features": 50, "out_features": 10}),
+    ]
+
+    def __init__(
+        self,
+        n_bits,
+        quant_weight=Int8WeightPerTensorFloat,
+        act_quant=Int8ActPerTensorFloat,
+    ):
+        """Quantized Torch Model with Brevitas.
+
+        Args:
+            n_bits (int): Bit of quantization
+            quant_weight (brevitas.quant): Quantization protocol of weights
+            act_quant (brevitas.quant): Quantization protocol of activations.
+
+        """
+        super().__init__()
+
+        # pylint: disable=inconsistent-return-statements
+        def make_quant_layers(t):
+            if t[0] == "ReLU":
+                return qnn.QuantReLU(
+                    bit_width=n_bits, act_quant=act_quant, return_quant_tensor=True
+                )
+            if t[0] == "AvgPool2d":
+                return torch.nn.AvgPool2d(**t[1])
+            if t[0] == "Conv2d":
+                return qnn.QuantConv2d(
+                    **t[1],
+                    weight_bit_width=n_bits,
+                    quant_weight=quant_weight,
+                    return_quant_tensor=True,
+                )
+            if t[0] == "Linear":
+                return qnn.QuantLinear(
+                    **t[1],
+                    weight_quant=quant_weight,
+                    weight_bit_width=n_bits,
+                    bias=True,
+                    return_quant_tensor=True,
+                )
+
+            if t[0] == "Dropout2d":
+                return torch.nn.Dropout2d(**t[1])
+            if t[0] == "BatchNorm2d":
+                return torch.nn.BatchNorm2d(**t[1])
+            if t[0] == "Identity":
+                return qnn.QuantIdentity(
+                    bit_width=n_bits, act_quant=act_quant, return_quant_tensor=True
+                )
+            if t[0] == "Flatten":
+                return nn.Flatten()
+
+        # Convolutional layers
+        self.quant_input = qnn.QuantIdentity(
+            bit_width=n_bits, act_quant=act_quant, return_quant_tensor=True
+        )
+
+        # Fully connected linear layers
+        self.sequential = torch.nn.Sequential(*[make_quant_layers(t) for t in self.layers])
+
+    def forward(self, x):
+        """Forward pass.
+
+        Args:
+            x (torch.tensor): The input of the model.
+
+        Returns:
+            torch.tensor: Output of the network.
+        """
+        x = self.quant_input(x)
+        x = self.sequential(x)
+        return x.value
+
+
+class QuantCustomModel(nn.Module):
+    """A small quantized network with Brevitas, trained on make_classification."""
+
+    def __init__(
+        self,
+        input_shape: int,
+        output_shape: int,
+        hidden_shape: int = 100,
+        n_bits: int = 5,
+        act_quant=Int8ActPerTensorFloat,
+        weight_quant=Int8WeightPerTensorFloat,
+    ):
+        """Quantized Torch Model with Brevitas.
+
+        Args:
+            input_shape (int): Input size
+            output_shape (int): Output size
+            hidden_shape (int): Hidden size
+            n_bits (int): Bit of quantization
+            weight_quant (brevitas.quant): Quantization protocol of weights
+            act_quant (brevitas.quant): Quantization protocol of activations.
+
+        """
+        super().__init__()
+
+        self.quant_input = qnn.QuantIdentity(
+            bit_width=n_bits, act_quant=act_quant, return_quant_tensor=True
+        )
+        self.linear1 = qnn.QuantLinear(
+            in_features=input_shape,
+            out_features=hidden_shape,
+            weight_bit_width=n_bits,
+            weight_quant=weight_quant,
+            bias=True,
+            return_quant_tensor=True,
+        )
+
+        self.relu1 = qnn.QuantReLU(return_quant_tensor=True, bit_width=n_bits, act_quant=act_quant)
+        self.linear2 = qnn.QuantLinear(
+            in_features=hidden_shape,
+            out_features=hidden_shape,
+            weight_bit_width=n_bits,
+            weight_quant=weight_quant,
+            bias=True,
+            return_quant_tensor=True,
+        )
+
+        self.relu2 = qnn.QuantReLU(return_quant_tensor=True, bit_width=n_bits, act_quant=act_quant)
+
+        self.linear3 = qnn.QuantLinear(
+            in_features=hidden_shape,
+            out_features=output_shape,
+            weight_bit_width=n_bits,
+            weight_quant=weight_quant,
+            bias=True,
+            return_quant_tensor=True,
+        )
+
+    def forward(self, x):
+        """Forward pass.
+
+        Args:
+            x (torch.tensor): The input of the model.
+
+        Returns:
+            torch.tensor: Output of the network.
+        """
+        x = self.quant_input(x)
+        x = self.linear1(x)
+        x = self.relu1(x)
+        x = self.linear2(x)
+        x = self.relu2(x)
+        x = self.linear3(x)
+        return x.value
+
+
+class TorchCustomModel(nn.Module):
+    """A small network with Brevitas, trained on make_classification."""
+
+    def __init__(self, input_shape, hidden_shape, output_shape):
+        """Torch Model.
+
+        Args:
+            input_shape (int): Input size
+            output_shape (int): Output size
+            hidden_shape (int): Hidden size
+        """
+        super().__init__()
+        self.linear1 = nn.Linear(input_shape, hidden_shape)
+        self.linear2 = nn.Linear(hidden_shape, hidden_shape)
+        self.linear3 = nn.Linear(hidden_shape, output_shape)
+
+    def forward(self, x):
+        """Forward pass.
+
+        Args:
+            x (torch.tensor): The input of the model.
+
+        Returns:
+            torch.tensor: Output of the network.
+        """
+        x = torch.relu(self.linear1(x))
+        x = torch.relu(self.linear2(x))
+        x = self.linear3(x)
+        return x
```

## concrete/ml/pytest/utils.py

```diff
@@ -1,15 +1,19 @@
 """Common functions or lists for test files, which can't be put in fixtures."""
 from functools import partial
+from pathlib import Path
+from typing import Any, Dict, List, Optional, Union
 
 import numpy
 import pytest
+import torch
 from torch import nn
 
-from concrete.ml.sklearn import (
+from ..common.utils import get_model_class, get_model_name, is_model_class_in_a_list, is_pandas_type
+from ..sklearn import (
     DecisionTreeClassifier,
     DecisionTreeRegressor,
     ElasticNet,
     GammaRegressor,
     Lasso,
     LinearRegression,
     LinearSVC,
@@ -20,142 +24,270 @@
     PoissonRegressor,
     RandomForestClassifier,
     RandomForestRegressor,
     Ridge,
     TweedieRegressor,
     XGBClassifier,
     XGBRegressor,
+    get_sklearn_neural_net_models,
 )
 
-regressor_models = [
+_regressor_models = [
     XGBRegressor,
     GammaRegressor,
     LinearRegression,
     Lasso,
     Ridge,
     ElasticNet,
     LinearSVR,
     PoissonRegressor,
     TweedieRegressor,
+    partial(TweedieRegressor, link="auto", power=0.0),
+    partial(TweedieRegressor, link="auto", power=2.8),
+    partial(TweedieRegressor, link="log", power=1.0),
+    partial(TweedieRegressor, link="identity", power=0.0),
     DecisionTreeRegressor,
     RandomForestRegressor,
     partial(
         NeuralNetRegressor,
         module__n_layers=3,
         module__n_w_bits=2,
         module__n_a_bits=2,
         module__n_accum_bits=7,  # Let's stay with 7 bits for test exec time
         module__n_hidden_neurons_multiplier=1,
-        module__n_outputs=1,
-        module__input_dim=10,
         module__activation_function=nn.ReLU,
         max_epochs=10,
         verbose=0,
     ),
 ]
 
-classifier_models = [
+_classifier_models = [
     DecisionTreeClassifier,
     RandomForestClassifier,
     XGBClassifier,
     LinearSVC,
     LogisticRegression,
     partial(
         NeuralNetClassifier,
         module__n_layers=3,
-        module__n_w_bits=2,
-        module__n_a_bits=2,
-        module__n_accum_bits=7,  # Let's stay with 7 bits for test exec time.
-        module__n_outputs=2,
-        module__input_dim=10,
         module__activation_function=nn.ReLU,
         max_epochs=10,
         verbose=0,
     ),
 ]
 
 # Get the datasets. The data generation is seeded in load_data.
-classifiers = [
+_classifiers_and_datasets = [
     pytest.param(
         model,
         {
-            "dataset": "classification",
             "n_samples": 1000,
             "n_features": 10,
-            "n_classes": 2
-            if isinstance(model, partial) and "NeuralNet" in model.func.__name__
-            else n_classes,  # FIXME #2402, qnns do not have multiclass yet
+            "n_classes": n_classes,
             "n_informative": 10,
             "n_redundant": 0,
         },
-        id=model.__name__ if not isinstance(model, partial) else model.func.__name__,
+        id=get_model_name(model),
     )
-    for model in classifier_models
+    for model in _classifier_models
     for n_classes in [2, 4]
 ]
 
 # Get the datasets. The data generation is seeded in load_data.
 # Only LinearRegression supports multi targets
 # GammaRegressor, PoissonRegressor and TweedieRegressor only handle positive target values
-regressors = [
+_regressors_and_datasets = [
     pytest.param(
         model,
         {
-            "dataset": "regression",
-            "strictly_positive": model in [GammaRegressor, PoissonRegressor, TweedieRegressor],
             "n_samples": 200,
             "n_features": 10,
             "n_informative": 10,
             "n_targets": 2 if model == LinearRegression else 1,
             "noise": 0,
         },
-        id=model.__name__ if not isinstance(model, partial) else model.func.__name__,
+        id=get_model_name(model),
     )
-    for model in regressor_models
+    for model in _regressor_models
 ]
 
+# All scikit-learn models in Concrete ML
+sklearn_models_and_datasets = _classifiers_and_datasets + _regressors_and_datasets
+
+
+def get_random_extract_of_sklearn_models_and_datasets():
+    """Return a random sublist of sklearn_models_and_datasets.
+
+    The sublist contains exactly one model of each kind.
+
+    Returns:
+        the sublist
+
+    """
+    unique_model_classes = []
+    done = {}
+
+    for m in sklearn_models_and_datasets:
+        t = m.values
+        typ = get_model_class(t[0])
+
+        if typ not in done:
+            done[typ] = True
+            unique_model_classes.append(m)
+
+    # To avoid to make mistakes and return empty list
+    assert len(sklearn_models_and_datasets) == 28
+    assert len(unique_model_classes) == 18
+
+    return unique_model_classes
+
+
+def instantiate_model_generic(model_class, **parameters):
+    """Instantiate any Concrete ML model type.
+
+    Args:
+        model_class (class): The type of the model to instantiate
+        parameters (dict): Hyper-parameters for the model instantiation
+
+    Returns:
+        model_name (str): The type of the model as a string
+        model (object): The model instance
+    """
+
+    assert "n_bits" in parameters
+    n_bits = parameters["n_bits"]
+
+    # If the model is a QNN, set the model using appropriate bit-widths
+    if is_model_class_in_a_list(model_class, get_sklearn_neural_net_models()):
+        extra_kwargs = {}
+        if n_bits > 8:
+            extra_kwargs["module__n_w_bits"] = 3
+            extra_kwargs["module__n_a_bits"] = 3
+            extra_kwargs["module__n_accum_bits"] = 12
+        else:
+            extra_kwargs["module__n_w_bits"] = 2
+            extra_kwargs["module__n_a_bits"] = 2
+            extra_kwargs["module__n_accum_bits"] = 7
+
+        model = model_class(**extra_kwargs)
 
-def sanitize_test_and_train_datasets(model, x, y):
-    """Sanitize datasets depending on the model type.
+    # Else, set the model using n_bits
+    else:
+        model = model_class(n_bits=n_bits)
+
+    # Seed the model
+    model_params = model.get_params()
+    if "random_state" in model_params:
+        model_params["random_state"] = numpy.random.randint(0, 2**15)
+
+    model.set_params(**model_params)
+
+    return model
+
+
+def get_torchvision_dataset(
+    param: Dict,
+    train_set: bool,
+):
+    """Get train or testing data-set.
 
     Args:
-        model: the model
-        x: the first output of load_data, i.e., the inputs
-        y: the second output of load_data, i.e., the labels
+        param (Dict): Set of hyper-parameters to use based on the selected torchvision data-set.
+            It must contain: data-set transformations (torchvision.transforms.Compose), and the
+            data-set_size (Optional[int]).
+        train_set (bool): Use train data-set if True, else testing data-set
 
     Returns:
-        Tuple containing sanitized (model_params, x, y, x_train, y_train, x_test)
+        A torchvision datasets.
+    """
+
+    transform = param["train_transform"] if train_set else param["test_transform"]
+    dataset = param["dataset"](download=True, root="./data", train=train_set, transform=transform)
+
+    if param.get("dataset_size", None):
+        dataset = torch.utils.data.random_split(
+            dataset,
+            [param["dataset_size"], len(dataset) - param["dataset_size"]],
+        )[0]
+
+    return dataset
+
+
+def data_calibration_processing(data, n_sample: int, targets=None):
+    """Reduce size of the given dataset.
 
+    Args:
+        data: The input container to consider
+        n_sample (int): Number of samples to keep if the given data-set
+        targets: If `dataset` is a `torch.utils.data.Dataset`, it typically contains both the data
+            and the corresponding targets. In this case, `targets` must be set to `None`.
+            If `data` is instance of `torch.Tensor` or 'numpy.ndarray`, `targets` is expected.
+
+    Returns:
+        Tuple[numpy.ndarray, numpy.ndarray]: The input data and the target (respectively x and y).
+
+    Raises:
+        TypeError: If the 'data-set' does not match any expected type.
     """
+    assert n_sample >= 1, "`n_sample` must be greater than or equal to `1`"
+    n_sample = min(len(data), n_sample)
+
+    # Generates a random sample from a given 1-D array
+    random_sample = numpy.random.choice(len(data), n_sample, replace=False)
 
-    x_train = x[:-1]
-    y_train = y[:-1]
-    x_test = x[-1:]
-
-    if isinstance(model, partial):
-        if model.func in [NeuralNetClassifier, NeuralNetRegressor]:
-            model_params = model.keywords
-            # Change module__input_dim to be the same as the input dimension
-            model_params["module__input_dim"] = x_train.shape[1]
-            # qnns require float32 as input
-            x = x.astype(numpy.float32)
-            x_train = x_train.astype(numpy.float32)
-            x_test = x_test.astype(numpy.float32)
-
-            if model.func is NeuralNetRegressor:
-                # Reshape y_train and y_test if 1d (regression for neural nets)
-                if y_train.ndim == 1:
-                    y_train = y_train.reshape(-1, 1).astype(numpy.float32)
-    elif model in [XGBClassifier, RandomForestClassifier, XGBRegressor]:
-        model_params = {
-            "n_estimators": 5,
-            "max_depth": 2,
-            "random_state": numpy.random.randint(0, 2**15),
-        }
-    elif model is DecisionTreeClassifier:
-        model_params = {"max_depth": 2, "random_state": numpy.random.randint(0, 2**15)}
-    elif model in [LogisticRegression]:
-        model_params = {"random_state": numpy.random.randint(0, 2**15)}
+    if (
+        hasattr(data, "__getitem__") and hasattr(data, "__len__") and hasattr(data, "train")
+    ) or isinstance(data, torch.utils.data.dataset.Subset):
+        assert targets is None, "dataset includes inputs and targets"
+        splitted_dataset = list(zip(*data))
+        x, y = numpy.stack(splitted_dataset[0]), numpy.array(splitted_dataset[1])
+
+    elif targets is not None and is_pandas_type(data) and is_pandas_type(targets):
+        x = data.to_numpy()
+        y = targets.to_numpy()
+
+    elif (
+        targets is not None
+        and isinstance(targets, (List, numpy.ndarray, torch.Tensor))  # type: ignore[arg-type]
+        and isinstance(data, (numpy.ndarray, torch.Tensor))
+    ):
+        x = numpy.array(data)
+        y = numpy.array(targets)
     else:
-        model_params = {}
+        raise TypeError(
+            "Only numpy arrays, torch tensors and torchvision datasets are supported. "
+            f"Got `{type(data)}` as input type and `{type(targets)}` as target type"
+        )
+
+    x = x[random_sample]
+    y = y[random_sample]
+
+    return x, y
+
+
+def load_torch_model(
+    model_class: torch.nn.Module,
+    state_dict_or_path: Optional[Union[str, Path, Dict[str, Any]]],
+    params: Dict,
+    device: str = "cpu",
+) -> torch.nn.Module:
+    """Load an object saved with torch.save() from a file or dict.
+
+    Args:
+        model_class (torch.nn.Module): A Pytorch or Brevitas network.
+        state_dict_or_path (Optional[Union[str, Path, Dict[str, Any]]]): Path or state_dict
+        params (Dict): Model's parameters
+        device (str):  Device type.
+
+    Returns:
+        torch.nn.Module: A Pytorch or Brevitas network.
+    """
+    model = model_class(**params)
+
+    if state_dict_or_path is not None:
+        if isinstance(state_dict_or_path, (str, Path)):
+            state_dict = torch.load(state_dict_or_path, map_location=device)
+        else:
+            state_dict = state_dict_or_path
+        model.load_state_dict(state_dict)
 
-    return model_params, x, y, x_train, y_train, x_test
+    return model
```

## concrete/ml/quantization/base_quantized_op.py

```diff
@@ -2,24 +2,29 @@
 
 from copy import deepcopy
 from inspect import Parameter, _empty, signature
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Type, Union, cast
 
 import numpy
 
-from ..common.debugging import assert_true
+from concrete import fhe
+
+from ..common.debugging import assert_false, assert_true
+from ..common.utils import compute_bits_precision
 from ..onnx.onnx_utils import ONNX_OPS_TO_NUMPY_IMPL
-from ..onnx.ops_impl import ONNXMixedFunction
+from ..onnx.ops_impl import ONNXMixedFunction, RawOpOutput
 from .quantizers import (
     MinMaxQuantizationStats,
     QuantizationOptions,
     QuantizedArray,
     UniformQuantizationParameters,
 )
 
+ONNXOpInputOutputType = Union[numpy.ndarray, QuantizedArray, None]
+
 ALL_QUANTIZED_OPS: Set[Type] = set()
 
 ONNX_OPS_TO_QUANTIZED_IMPL: Dict[str, Type["QuantizedOp"]] = {}
 
 # This constant determines the number of bits for the quantization of input and output values
 # of an ML model. This is not necessarily the maximum bitwidth in the network, as Gemm/Conv ops
 # have output bitwidth that is related to their weights and inputs.
@@ -31,14 +36,18 @@
 
 
 class QuantizedOp:
     """Base class for quantized ONNX ops implemented in numpy.
 
     Args:
         n_bits_output (int): The number of bits to use for the quantization of the output
+        op_instance_name (str): The name that should be assigned to this operation, used
+            to retrieve it later or get debugging information about this op (bitwidth, value range,
+            integer intermediary values, op-specific error messages). Usually this name is the same
+            as the ONNX operation name for which this operation is constructed.
         int_input_names (Set[str]): The set of names of integer tensors that are inputs to this op
         constant_inputs (Optional[Union[Dict[str, Any], Dict[int, Any]]]): The constant tensors
             that are inputs to this op
         input_quant_opts (QuantizationOptions): Input quantizer options, determine the quantization
             that is applied to input tensors (that are not constants)
     """
 
@@ -66,35 +75,41 @@
     _input_idx_to_params_name: Dict[int, str] = {}
     _params_that_are_onnx_inputs: Set[str] = set()
     _params_that_are_onnx_var_inputs: Set[str] = set()
     _params_that_are_required_onnx_inputs: Set[str] = set()
     _has_attr: bool
     _inputs_not_quantized: Set[str] = set()
     quantize_inputs_with_model_outputs_precision: bool = False
-    op_instance_name: Optional[str] = None
+
+    # The ONNX name of this op instance (e.g. "Conv_9", "MatMul_5" etc.)
+    op_instance_name: str
 
     # Determines if this op computes a tensor that is a graph output, i.e. a tensor
     # that will be decrypted and dequantized in the clear
     produces_graph_output = False
 
-    # The ONNX name of this op instance (e.g. "Conv_9", "MatMul_5" etc.)
-    op_instance_name = None
+    # Determines if the op produces a raw output (not quantized). This can
+    # be a float or integer tensor that contains non-encrypted values
+    produces_raw_output = False
 
     error_tracker: Optional[List[int]] = None
-    debug_value_tracker: Optional[Dict[str, Any]] = None
+    debug_value_tracker: Optional[
+        Dict[str, Dict[Union[int, str], Optional[ONNXOpInputOutputType]]]
+    ] = None
 
     POSITIONAL_ARGUMENTS_KINDS = {
         Parameter.POSITIONAL_ONLY,
         Parameter.POSITIONAL_OR_KEYWORD,
     }
     VAR_POSITIONAL_ARGUMENTS_KINDS = {Parameter.VAR_POSITIONAL}
 
     def __init__(
         self,
         n_bits_output: int,
+        op_instance_name: str,
         int_input_names: Optional[Set[str]] = None,
         constant_inputs: Optional[Union[Dict[str, Any], Dict[int, Any]]] = None,
         input_quant_opts: Optional[QuantizationOptions] = None,
         **attrs,
     ) -> None:
         self.n_bits = n_bits_output
 
@@ -161,14 +176,18 @@
 
         self.attrs = dict(self._default_attrs, **deepcopy(attrs))
 
         # Only use QAT for layers that need it (that mix encrypted values: conv, dense, add, etc...)
         if self.can_fuse():
             self.input_quant_opts.is_qat = False
 
+        # Set the operation's name, which is used to identify this op in the CML op graph
+        # with respect to the ONNX graph (usually we keep use ONNX op name)
+        self.op_instance_name = op_instance_name
+
     @classmethod
     def op_type(cls):
         """Get the type of this operation.
 
         Returns:
             op_type (str): The type of this operation, in the ONNX referential
         """
@@ -198,35 +217,36 @@
             cls.impl = candidate_impl if candidate_impl is not None else cls.impl
 
         assert_true(cls.impl is not None, f"Missing 'impl' for class {cls.__name__}")
 
         cls._populate_op_input_infos()
         cls._has_attr = len(cls._authorized_attr_names) > 0
 
-    def __call__(self, *q_inputs: QuantizedArray) -> QuantizedArray:
+    def __call__(self, *q_inputs: ONNXOpInputOutputType) -> ONNXOpInputOutputType:
         """Process the forward pass of the quantized op according to the implementation.
 
         The calibrate method needs to be called with sample data before using this function.
 
         Args:
-            *q_inputs (QuantizedArray): Quantized inputs.
+            *q_inputs (ONNXOpInputOutputType): Quantized inputs.
 
         Returns:
-            QuantizedArray: Quantized output.
+            ONNXOpInputOutputType: Quantized output.
         """
 
         return self.q_impl(*q_inputs, **self.attrs)
 
     @classmethod
     def _populate_op_input_infos(cls):
         # for mypy
         assert cls.impl is not None
         if isinstance(cls.impl, ONNXMixedFunction):
             impl_signature = signature(cls.impl.function)
             cls._inputs_not_quantized = cls.impl.non_quant_params
+            cls.produces_raw_output = cls.impl.output_is_raw
         else:
             impl_signature = signature(cls.impl)
         impl_params = impl_signature.parameters
         cls._params_name_to_input_idx = {val: index for index, val in enumerate(impl_params)}
         cls._input_idx_to_params_name = dict(enumerate(impl_params))
         cls._params_that_are_onnx_inputs = {
             param.name
@@ -266,76 +286,66 @@
         """
 
         # Operation parameters have names and indices, we only support indices here
         assert_true(isinstance(input_name_or_idx, int))
         input_name = cls._input_idx_to_params_name[input_name_or_idx]
         return input_name not in cls._inputs_not_quantized
 
-    def q_impl(self, *q_inputs: QuantizedArray, **attrs) -> QuantizedArray:
+    def q_impl(
+        self,
+        *q_inputs: ONNXOpInputOutputType,
+        **attrs,
+    ) -> ONNXOpInputOutputType:
         """Execute the quantized forward.
 
         Args:
-            *q_inputs (QuantizedArray): Quantized inputs.
+            *q_inputs (ONNXOpInputOutputType): Quantized inputs.
             **attrs: the QuantizedOp attributes.
 
         Returns:
-            QuantizedArray: The returned quantized value.
+            ONNXOpInputOutputType: The returned quantized value.
         """
+
         # Here we need the float32 values from the QuantizedArrays. By default, when possible,
         # we want QuantizedOps to convert to TLUs. Ops that need to do quantized computation
         # will call _prepare_inputs_with_constants with quantize_actual_values=True
         prepared_inputs = self._prepare_inputs_with_constants(
             *q_inputs, calibrate=False, quantize_actual_values=False
         )
         f_outputs = self.call_impl(*prepared_inputs, **attrs)
-        return self.prepare_output(f_outputs)
 
-    def _prepare_inputs_with_constants(
-        self,
-        *inputs: Union[QuantizedArray, numpy.ndarray],
-        calibrate: bool,
-        quantize_actual_values: bool,
-    ):  # pylint: disable=too-many-branches
-        """Retrieve all the inputs of an operator in the computational graph.
+        # If the op takes only raw values as inputs it must be producing only raw outputs
+        # Operations such as Add/Mul can, in some settings, operate in this setting
+        # for example in subgraphs that manipulate shapes
+        if all(isinstance(q_input, RawOpOutput) for q_input in q_inputs):
+            return f_outputs.view(RawOpOutput)
 
-        This helper method will prepare a list of inputs to an operator. Inputs can be variables,
-        i.e. encrypted tensors, or constants (in the clear). Inputs to an operator are set-up in
-        the slots of a list, as the order of inputs is important.
+        return self.prepare_output(f_outputs)
 
-        Usually the input list is populated with QuantizedArrays. Operators that require the
-        original float (operators that only produce or contribute to TLUs) values will just read
-        out the .values of  these quantized arrays. Operators that do matrix multiplication will
-        read out the quantized integer values of the arrays.  The method can be called during
-        calibration, in which case the variable inputs are just float numpy tensors.
+    def _prepare_constants(
+        self, number_of_inputs: int, calibrate: bool, quantize_actual_values: bool
+    ) -> List[Optional[ONNXOpInputOutputType]]:
+        """Prepare a list of inputs of the quantized op, filling in the constants.
 
         Args:
-             *inputs (Union[QuantizedArray, numpy.ndarray]): A list of all variable inputs
+            number_of_inputs (int): The total number of inputs to fill in
             calibrate (bool): A flag specifying if the method is called during calibration
             quantize_actual_values (bool): If called by a quantized operator that does matrix
                 multiplication between encrypted and clear values, this method will apply
                 the quantization computation to the input, which will be fused in a (potentially
                 larger) TLU, with preceding floating point computations
 
         Returns:
             result (List): a list of inputs which are either QuantizedArray or numpy.arrays. If
-                quantize_actual_values==True then the quantization code is applied
+                quantize_actual_values==True then the constants are assumed to be quantized
         """
-        num_onnx_inputs = len(self._params_that_are_onnx_inputs)
-        num_required_onnx_inputs = len(self._params_that_are_required_onnx_inputs)
-        num_provided_constants = len(self.constant_inputs)
-        num_inputs = len(inputs)
-        is_param_variadic = len(self._params_that_are_onnx_var_inputs) > 0
 
-        prepared_inputs: List[Optional[Union[QuantizedArray, numpy.ndarray]]]
-        if is_param_variadic:
-            # prepared_inputs length can't be inferred from num_onnx_inputs with a var parameter
-            # use inputs instead
-            prepared_inputs = [None] * num_inputs
-        else:
-            prepared_inputs = [None] * num_onnx_inputs
+        prepared_inputs: List[Optional[ONNXOpInputOutputType]]
+
+        prepared_inputs = [None] * number_of_inputs
 
         # If calibrating (calibrate=True): inputs are numpy.ndarrays of float32
         # If used in the computation graph (calibrate=False): inputs are QuantizedArrays, of which
         # we use the float32 .values and optionally we quantized them to int
 
         # Constants are quantized during graph creation. If calibrating, pass through
         # the original float values. If running in the computation graph, if the quantized values
@@ -346,106 +356,182 @@
             # an input that **must** be quantized will be stored in a QuantizedArray, we need
             # to retrieve its .values to return the requested float values
 
             # In all other cases we return a QuantizedArray or numpy.array. QuantizedArrays
             # in this case are produced by other ops or inputs. numpy.arrays are produced
             # by initializers
             if calibrate or not quantize_actual_values:
-                if self.__class__.must_quantize_input(input_idx):
+                is_clear_value = isinstance(constant_val, RawOpOutput)
+
+                if not is_clear_value and self.__class__.must_quantize_input(input_idx):
                     prepared_inputs[input_idx] = constant_val.values
                 else:
                     prepared_inputs[input_idx] = constant_val
             else:
                 prepared_inputs[input_idx] = constant_val
 
+        return prepared_inputs
+
+    def _prepare_quantized_input(self, input_: QuantizedArray) -> QuantizedArray:
+        """Prepare a quantized encrypted input for a univariate or mixin operation.
+
+        Args:
+            input_ (QuantizedArray): the encrypted input
+
+        Returns:
+            result (QuantizedArray): the quantized input, either re-quantized to new quantization
+                options, or keeping the original quantization
+        """
+
+        # Here we want to trace the code that does quantization, to produce a TLU
+        # We use the op's input quantization options
+
+        quant_opts = QuantizationOptions(self.input_quant_opts.n_bits)
+        quant_opts.copy_opts(self.input_quant_opts)
+
+        assert_false(
+            self.can_fuse(),
+            f"The {self.__class__.__name__} operation is attempting "
+            "to quantize its inputs but is marked as fusable (can_fuse() return True). ",
+        )
+
+        # Now we quantize the input. For ops that require quantized inputs (which
+        # call this function with quantize_actual_values==True), this
+        # will produce numpy ops that will be fused to a TLU. Fusable ops will
+        # use the .values directly (see else branch below). We need the quantization
+        # stats to generate the quantization code, they cannot be computed on the fly.
+
+        # Conv/Matmul layers have quantization options initialized by the PTQ default,
+        # but when parsing the ONNX graph, some options can be overwritten. Thus
+        # when evaluating QAT layers we ignore one of these options to allow the
+        # override.
+        if quant_opts.is_equal(input_.quantizer.quant_options, ignore_sign_qat=True):
+            # Pass-through the input quantizer when the input is already quantized in
+            # the manner that this op requires: this makes the op use the qvalues directly,
+            # in q_impl and will avoid a TLU to re-quantize.
+            new_input = QuantizedArray(
+                quant_opts.n_bits,
+                input_.qvalues,
+                value_is_float=False,
+                options=input_.quantizer.quant_options,
+                stats=input_.quantizer.quant_stats,
+                params=input_.quantizer.quant_params,
+            )
+        else:
+            quant_params = None
+            if input_.quantizer.is_qat:
+                quant_params = input_.quantizer.quant_params
+
+            new_input = QuantizedArray(
+                quant_opts.n_bits,
+                input_.values,
+                options=quant_opts,
+                stats=input_.quantizer.quant_stats,
+                params=quant_params,
+            )
+
+        return new_input
+
+    def _prepare_inputs_with_constants(
+        self,
+        *inputs: ONNXOpInputOutputType,
+        calibrate: bool,
+        quantize_actual_values: bool,
+    ):
+        """Retrieve all the inputs of an operator in the computational graph.
+
+        This helper method will prepare a list of inputs to an operator. Inputs can be variables,
+        i.e. encrypted tensors, or constants (in the clear). Inputs to an operator are set-up in
+        the slots of a list, as the order of inputs is important.
+
+        Usually the input list is populated with QuantizedArrays. Operators that require the
+        original float (operators that only produce or contribute to TLUs) values will just read
+        out the .values of  these quantized arrays. Operators that do matrix multiplication will
+        read out the quantized integer values of the arrays.  The method can be called during
+        calibration, in which case the variable inputs are just float numpy tensors.
+
+        Args:
+             *inputs (ONNXOpInputOutputType): A list of all variable inputs
+            calibrate (bool): A flag specifying if the method is called during calibration
+            quantize_actual_values (bool): If called by a quantized operator that does matrix
+                multiplication between encrypted and clear values, this method will apply
+                the quantization computation to the input, which will be fused in a (potentially
+                larger) TLU, with preceding floating point computations
+
+        Returns:
+            result (List): a list of inputs which are either QuantizedArray or numpy.arrays. If
+                quantize_actual_values==True then the quantization code is applied
+        """
+        num_onnx_inputs = len(self._params_that_are_onnx_inputs)
+        num_required_onnx_inputs = len(self._params_that_are_required_onnx_inputs)
+        num_provided_constants = len(self.constant_inputs)
+        num_inputs = len(inputs)
+        is_param_variadic = len(self._params_that_are_onnx_var_inputs) > 0
+
         condition_inputs = (
             num_onnx_inputs >= (num_inputs) + num_provided_constants >= num_required_onnx_inputs
             if not is_param_variadic
             else True
         )
         assert_true(
             condition_inputs,
             f"This operator has {num_onnx_inputs} ONNX inputs, and {num_provided_constants} "
             "constants were already provided when instantiating the class. "
             f"Got a call with {num_inputs} inputs and constants while the call expects between "
             f"{num_required_onnx_inputs} and {num_onnx_inputs} inputs and constants.",
         )
 
+        prepared_inputs = self._prepare_constants(
+            num_inputs if is_param_variadic else num_onnx_inputs,
+            calibrate,
+            quantize_actual_values,
+        )
+
         # If calibrating, the function is called with numpy.ndarrays
         # If not calibrating, the function is called with QuantizedArray inputs
         # If quantized values are requested, we quantized the float32 values contained in the
         # QuantizedArrays, else we return the float32 values directly.
 
         curr_input_fill_idx = 0
         for input_idx, input_ in enumerate(inputs):
             while prepared_inputs[curr_input_fill_idx] is not None:
                 curr_input_fill_idx += 1
 
-            if calibrate:
+            # This is an integer scalar (e.g. tensor shape). This is not an encrypted
+            # value, it is not traced
+            is_clear_value = isinstance(input_, RawOpOutput)
+
+            if input_ is None:
+                # Do nothing if the input is not set, the underlying ops will handle the None
+                pass
+            elif calibrate or is_clear_value:
+                # This is used during calibration with numpy.ndarrays
+                # or then the input is raw (not quantized)
                 prepared_inputs[curr_input_fill_idx] = input_
             elif quantize_actual_values:
-                # Here we want to trace the code that does quantization, to produce a TLU
+                # This is used by mixing (conv/gemm) or value re-arranging ops (reshape)
                 input_ = cast(QuantizedArray, input_)
+                new_input = self._prepare_quantized_input(input_)
 
-                # We use the op's input quantization options
-                quant_opts = QuantizationOptions(self.input_quant_opts.n_bits)
-                quant_opts.copy_opts(self.input_quant_opts)
-
-                # And if this op is in a QAT enabled graph, we disable QAT if this op is fusable
-                # If the op can be fused, quantization will not be used, no need to run the QAT
-                # specific quantization process. This case is encountered for example for Add
-                # when the tensors that are added are produced from a single integer tensor
-                if self.can_fuse():
-                    quant_opts.is_qat = False
-
-                # Now we quantize the input. For ops that require quantized inputs (which
-                # call this function with quantize_actual_values==True), this
-                # will produce numpy ops that will be fused to a TLU. Fusable ops will
-                # use the .values directly (see else branch below). We need the quantization
-                # stats to generate the quantization code, they cannot be computed on the fly.
-
-                # Conv/Matmul layers have quantization options initialized by the PTQ default,
-                # but when parsing the ONNX graph, some options can be overwritten. Thus
-                # when evaluating QAT layers we ignore one of these options to allow the
-                # override.
-                if quant_opts.is_equal(input_.quantizer.quant_options, ignore_sign_qat=True):
-                    # Pass-through when the input is already quantized in
-                    # the manner that this op requires: use the qvalues directly,
-                    # they will then be used by this quantized op's q_impl
-                    new_input = QuantizedArray(
-                        quant_opts.n_bits,
-                        input_.qvalues,
-                        value_is_float=False,
-                        options=quant_opts,
-                        stats=input_.quantizer.quant_stats,
-                        params=input_.quantizer.quant_params,
-                    )
-                else:
-                    quant_params = None
-                    if input_.quantizer.is_qat:
-                        quant_params = input_.quantizer.quant_params
-
-                    new_input = QuantizedArray(
-                        quant_opts.n_bits,
-                        input_.values,
-                        options=quant_opts,
-                        stats=input_.quantizer.quant_stats,
-                        params=quant_params,
-                    )
-
+                # Check that the input quantizer is correct - that it can de-quantize
+                # values correctly. If it's not, it is added to the list of invalid tensors
+                # for which an error is raised
                 if (
-                    quant_opts.is_qat
+                    new_input.quantizer.is_qat
                     and not input_.quantizer.is_precomputed_qat
                     and self.error_tracker is not None
-                    and not new_input.quantizer.check_is_uniform_quantized(quant_opts)
+                    and not new_input.quantizer.check_is_uniform_quantized(
+                        new_input.quantizer.quant_options
+                    )
                 ):
                     self.error_tracker.append(input_idx)
 
                 prepared_inputs[curr_input_fill_idx] = new_input
             else:
+                # This is usually used for univariate ops that are fused into TLUs
                 input_ = cast(QuantizedArray, input_)
                 prepared_inputs[curr_input_fill_idx] = input_.values
 
             curr_input_fill_idx += 1
 
         if self.debug_value_tracker is not None:
             # For mypy
@@ -470,24 +556,26 @@
         """
 
         # Here we need the actual values of the constants, we need to pass through
         # the numpy.ndarrays in the computation graph
         prepared_inputs = self._prepare_inputs_with_constants(
             *inputs, calibrate=True, quantize_actual_values=False
         )
-        quantized_samples = QuantizedArray(
-            self.n_bits, self.call_impl(*prepared_inputs, **self.attrs)
-        )
+
+        raw_result = self.call_impl(*prepared_inputs, **self.attrs)
+        if isinstance(raw_result, RawOpOutput):
+            return raw_result
+
+        quantized_samples = QuantizedArray(self.n_bits, raw_result)
 
         self.output_quant_params = quantized_samples.quantizer.quant_params
         self.output_quant_stats = quantized_samples.quantizer.quant_stats
 
         return quantized_samples.values
 
-    # TODO: manage multiple inputs if it becomes necessary
     def prepare_output(self, qoutput_activation: numpy.ndarray) -> QuantizedArray:
         """Quantize the output of the activation function.
 
         The calibrate method needs to be called with sample data before using this function.
 
         Args:
             qoutput_activation (numpy.ndarray): Output of the activation function.
@@ -550,16 +638,15 @@
 
         This function shall be overloaded by inheriting classes to test self._int_input_names, to
         determine whether the operation can be fused to a TLU or not. For example an operation
         that takes inputs produced by a unique integer tensor can be fused to a TLU. Example:
         f(x) = x * (x + 1) can be fused. A function that does f(x) = x * (x @ w + 1) can't be fused.
 
         Returns:
-            bool: whether this instance of the QuantizedOp produces Concrete Numpy code
-                  that can be fused to TLUs
+            bool: whether this QuantizedOp instance produces Concrete code that can be fused to TLUs
         """
         return True
 
     def _get_output_quant_opts(self):
         """Return the output quantization options.
 
         This function computes the output quantization options based on the input quantizer
@@ -582,30 +669,39 @@
     This operation is not really operating as a quantized operation. It is useful when the
     computations get fused into a TLU, as in e.g. Act(x) = x || (x + 42)).
     """
 
     def __init__(
         self,
         n_bits_output: int,
+        op_instance_name: str,
         int_input_names: Optional[Set[str]] = None,
         constant_inputs: Optional[Union[Dict[str, Any], Dict[int, Any]]] = None,
         input_quant_opts: Optional[QuantizationOptions] = None,
         **attrs,
     ) -> None:
         # Disable mypy which is failing for mixins
         super().__init__(
-            n_bits_output, int_input_names, constant_inputs, input_quant_opts, **attrs
+            n_bits_output,
+            op_instance_name,
+            int_input_names,
+            constant_inputs,
+            input_quant_opts,
+            **attrs,
         )  # type: ignore
 
         # We do not support this type of operation between encrypted tensors, only between:
         # - encrypted tensors and float constants
         # - tensors that are produced by a unique integer tensor
         # If this operation is applied between two constants
         # it should be optimized out by the constant folding procedure
-        assert_true(self.can_fuse() or (constant_inputs is not None and len(constant_inputs) == 1))
+        assert_true(
+            self.can_fuse() or (constant_inputs is not None and len(constant_inputs) == 1),
+            "Do not support this type of operation between encrypted tensors",
+        )
 
     def can_fuse(self) -> bool:
         """Determine if this op can be fused.
 
         This operation can be fused and computed in float when a single integer tensor generates
         both the operands. For example in the formula: f(x) = x || (x + 1)  where x is an integer
         tensor.
@@ -622,14 +718,28 @@
 
 class QuantizedMixingOp(QuantizedOp, is_utility=True):
     """An operator that mixes (adds or multiplies) together encrypted inputs.
 
     Mixing operators cannot be fused to TLUs.
     """
 
+    lsbs_to_remove: Optional[int] = None
+    rounding_threshold_bits: Optional[int] = None
+
+    def __init__(self, *args, rounding_threshold_bits: Optional[int] = None, **kwargs) -> None:
+        """Initialize quantized ops parameters plus specific parameters.
+
+        Args:
+            rounding_threshold_bits (Optional[int]): Number of bits to round to.
+            *args: positional argument to pass to the parent class.
+            **kwargs: named argument to pass to the parent class.
+        """
+        self.rounding_threshold_bits = rounding_threshold_bits
+        super().__init__(*args, **kwargs)
+
     def can_fuse(self) -> bool:
         """Determine if this op can be fused.
 
         Mixing operations cannot be fused since it must be performed over integer tensors and it
         combines different encrypted elements of the input tensors. Mixing operations are Conv,
         MatMul, etc.
 
@@ -658,23 +768,61 @@
             QuantizedArray: the quantized array that will be passed to the QuantizedModule output.
         """
 
         out_opts = self._get_output_quant_opts()
         out_opts.is_signed = False
         out_opts.is_symmetric = False
 
-        out_params = UniformQuantizationParameters()
-        out_params.scale = scale
-        out_params.zero_point = zero_point
-
-        # Since we don't know the real bit-width of this numpy_q_out value,
+        # Since we don't know the real bit-width of these quantized values,
         # return a quantizer that has zero offset
-        out_params.offset = 0
+        out_params = UniformQuantizationParameters(
+            scale=scale,
+            zero_point=zero_point,
+            offset=0,
+        )
 
         return QuantizedArray(
             self.n_bits,
             q_values,
             value_is_float=False,
             options=self._get_output_quant_opts(),
             stats=self.output_quant_stats,
             params=out_params,
         )
+
+    def cnp_round(
+        self, x: Union[numpy.ndarray, fhe.tracing.Tracer], calibrate_rounding: bool
+    ) -> numpy.ndarray:
+        """Round the input array to the specified number of bits.
+
+        Args:
+            x (Union[numpy.ndarray, fhe.tracing.Tracer]): The input array to be rounded.
+            calibrate_rounding (bool): Whether to calibrate the rounding
+                (compute the lsbs_to_remove)
+
+        Returns:
+            numpy.ndarray: The rounded array.
+        """
+
+        # Rounding is applied only if specified by user
+        if self.rounding_threshold_bits is not None:
+            if calibrate_rounding:
+                assert_true(
+                    not isinstance(x, fhe.tracing.Tracer),
+                    "Can't compute lsbs_to_remove at compilation time.",
+                )
+                assert_true(
+                    self.lsbs_to_remove is None,
+                    "Rounding has already been calibrated.",
+                )
+
+                current_n_bits_accumulator = compute_bits_precision(x)
+                self.lsbs_to_remove = current_n_bits_accumulator - self.rounding_threshold_bits
+
+            # mypy
+            assert self.lsbs_to_remove is not None
+
+            # Apply rounding if needed
+            if self.lsbs_to_remove > 0:
+                x = fhe.round_bit_pattern(x, lsbs_to_remove=self.lsbs_to_remove)
+
+        return x
```

## concrete/ml/quantization/post_training.py

```diff
@@ -5,16 +5,23 @@
 
 import numpy
 import onnx
 from onnx import numpy_helper
 
 from ..common.debugging import assert_true
 from ..onnx.onnx_utils import ONNX_OPS_TO_NUMPY_IMPL, get_attribute, get_op_type
+from ..onnx.ops_impl import RawOpOutput
 from ..torch.numpy_module import NumpyModule
-from .base_quantized_op import DEFAULT_MODEL_BITS, ONNX_OPS_TO_QUANTIZED_IMPL, QuantizedOp
+from .base_quantized_op import (
+    DEFAULT_MODEL_BITS,
+    ONNX_OPS_TO_QUANTIZED_IMPL,
+    ONNXOpInputOutputType,
+    QuantizedMixingOp,
+    QuantizedOp,
+)
 from .quantized_module import QuantizedModule
 from .quantized_ops import QuantizedBrevitasQuant
 from .quantizers import QuantizationOptions, QuantizedArray, UniformQuantizer
 
 
 def get_n_bits_dict(n_bits: Union[int, Dict[str, int]]) -> Dict[str, int]:
     """Convert the n_bits parameter into a proper dictionary.
@@ -103,34 +110,37 @@
             When using a single integer for n_bits, its value is assigned to "op_inputs" and
             "op_weights" bits. The maximum between this value and a default value (5) is then
             assigned to the number of "model_inputs" "model_outputs". This default value is a
             compromise between model accuracy and runtime performance in FHE. "model_outputs" gives
             the precision of the final network's outputs, while "model_inputs" gives the precision
             of the network's inputs. "op_inputs" and "op_weights" both control the quantization for
             inputs and weights of all layers.
-        y_model (NumpyModule): Model in numpy.
-        is_signed (bool): Whether the weights of the layers can be signed. Currently, only the
-            weights can be signed.
+        numpy_model (NumpyModule): Model in numpy.
+        rounding_threshold_bits (int): if not None, every accumulators in the model are rounded down
+            to the given bits of precision
     """
 
     quant_ops_dict: Dict[str, Tuple[Tuple[str, ...], QuantizedOp]]
-    n_bits: Union[int, Dict]
-    quant_params: Dict[str, QuantizedArray]
+    n_bits: Dict[str, int]
+    quant_params: Dict[str, numpy.ndarray]
     numpy_model: NumpyModule
+    rounding_threshold_bits: Optional[int]
 
-    # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/2369
-    is_signed: bool
-
-    def __init__(self, n_bits: Union[int, Dict], numpy_model: NumpyModule, is_signed: bool = False):
+    def __init__(
+        self,
+        n_bits: Union[int, Dict],
+        numpy_model: NumpyModule,
+        rounding_threshold_bits: Optional[int] = None,
+    ):
         self.quant_ops_dict = {}
 
         self.n_bits = get_n_bits_dict(n_bits)
         self.quant_params = {}
         self.numpy_model = numpy_model
-        self.is_signed = is_signed
+        self.rounding_threshold_bits = rounding_threshold_bits
 
     @property
     def n_bits_model_outputs(self):
         """Get the number of bits to use for the quantization of the last layer's output.
 
         Returns:
             n_bits (int): number of bits for output quantization
@@ -166,15 +176,15 @@
 
     @abstractmethod
     def _process_layer(
         self,
         quantized_op: QuantizedOp,
         *calibration_data: numpy.ndarray,
         quantizers: List[Optional[UniformQuantizer]],
-    ) -> Tuple[numpy.ndarray, UniformQuantizer]:
+    ) -> Tuple[numpy.ndarray, Optional[UniformQuantizer]]:
         """Configure a graph operation according to model conversion mode.
 
         Args:
             quantized_op (QuantizedOp): Quantized graph operator instance
             *calibration_data (numpy.ndarray): tuple of network input tensors to be used for
                 calibration
             quantizers (List[Optional[UniformQuantizer]]): a list of quantizers that
@@ -188,15 +198,15 @@
 
     def _calibrate_layers_activation(
         self,
         calibrate_quantized: bool,
         quantized_op: QuantizedOp,
         *calibration_data: numpy.ndarray,
         quantizers: List[Optional[UniformQuantizer]],
-    ) -> Tuple[numpy.ndarray, UniformQuantizer]:
+    ) -> Tuple[numpy.ndarray, Optional[UniformQuantizer]]:
         """Calibrate the QuantizedOp with the previous layer's output calibration data.
 
         Args:
             calibrate_quantized (bool): determines if we use de-quantized values (True) or
                 raw values (False) during calibration.
             quantized_op (QuantizedOp): the quantized operator for the current layer.
             *calibration_data: numpy.ndarray: the previous layer's calibration data.
@@ -216,18 +226,23 @@
         if quantized_op.quantize_inputs_with_model_outputs_precision:
             n_bits = self.n_bits_model_outputs
         else:
             n_bits = self.n_bits_op_inputs
 
         # Create new calibration data (output of the previous layer)
         # Use the op's input options (thus behavior in calibration is the same as in compilation)
-        q_calibration_data: List[QuantizedArray] = list(
-            QuantizedArray(n_bits, data, True, options=quantized_op.input_quant_opts)
-            for data in calibration_data
-        )
+        q_calibration_data: List[ONNXOpInputOutputType] = []
+        for data in calibration_data:
+            is_clear_value = isinstance(data, RawOpOutput)
+            if is_clear_value or data is None:
+                q_calibration_data.append(data)
+            else:
+                q_calibration_data.append(
+                    QuantizedArray(n_bits, data, True, options=quantized_op.input_quant_opts)
+                )
 
         # Override, when necessary, the calibration data with data that is quantized with
         # layer quantizers that are overridden by the QAT graph quantizers
         for idx, data in enumerate(calibration_data):
             if quantizers[idx] is None:
                 continue
 
@@ -239,34 +254,61 @@
                 data,
                 True,
                 options=quantizer.quant_options,
                 stats=quantizer.quant_stats,
                 params=quantizer.quant_params,
             )
 
+        # Enable rounding calibration if used has set a rounding_threshold_bits
+        calibrate_attr = (
+            {"calibrate_rounding": True} if isinstance(quantized_op, QuantizedMixingOp) else {}
+        )
+
+        # Add calibrate_attr to list of attr for q_impl method
+        q_impl_attr = quantized_op.attrs.copy()
+        q_impl_attr.update(calibrate_attr)
+
         # Dequantize to have the value in clear and ready for next calibration
-        quant_result = quantized_op(*q_calibration_data)
+        quant_result = quantized_op.q_impl(*q_calibration_data, **q_impl_attr)
         if quantized_op.produces_graph_output:
+
+            assert isinstance(quant_result, QuantizedArray), (
+                "The PyTorch module can not return a raw value, "
+                "such as a clear constant or the shape of a tensor."
+            )
+
             assert quantized_op.output_quant_stats is not None
             assert quantized_op.output_quant_params is not None
             quantized_op.output_quant_stats.copy_stats(quant_result.quantizer.quant_stats)
             quantized_op.output_quant_params.copy_params(quant_result.quantizer.quant_params)
 
-        # For PTQ, the calibration is performed on quantized data
-        if calibrate_quantized:
-            return quant_result.dequant(), quant_result.quantizer
+        assert_true(
+            not quantized_op.produces_raw_output or isinstance(quant_result, RawOpOutput),
+            "QuantizedOps whose ONNX numpy implementation is marked as producing raw output"
+            " must return an instance of RawOpOutput. \n"
+            f" ** Offending Op: {quantized_op.__class__.__name__}",
+        )
+        # For PTQ, the calibration is performed on quantized data. But
+        # raw operation output (RawOpOutput) data should not be quantized
+        if calibrate_quantized and not isinstance(quant_result, RawOpOutput):
+            assert isinstance(quant_result, QuantizedArray)
+            return (
+                quant_result.dequant(),
+                quant_result.quantizer if isinstance(quant_result, QuantizedArray) else None,
+            )
 
         # For QAT, the calibration is performed on raw data, performing
         # calibration on quantized that would confound inferred QAT and PTQ.
-        return raw_result, quant_result.quantizer
+        return (
+            raw_result,
+            quant_result.quantizer if isinstance(quant_result, QuantizedArray) else None,
+        )
 
     @abstractmethod
-    def _process_initializer(
-        self, n_bits: int, values: Union[numpy.ndarray, QuantizedArray]
-    ) -> QuantizedArray:
+    def _process_initializer(self, n_bits: int, values: numpy.ndarray) -> QuantizedArray:
         """Transform a constant tensor according to the model conversion mode.
 
         The values supplied are floating point values that will be quantized.
 
         Arguments:
             n_bits (int): Number of bits to quantize the weight values
             values (numpy.ndarray): Float values that initialize this tensor
@@ -274,30 +316,27 @@
         Returns:
             QuantizedArray: a quantized tensor with integer values on n_bits bits
         """
 
     @abstractmethod
     def _get_input_quant_opts(
         self,
-        values: Tuple[Union[numpy.ndarray, QuantizedArray], ...],
+        values: Tuple[ONNXOpInputOutputType, ...],
         quantized_op_class: Type["QuantizedOp"],
     ) -> QuantizationOptions:
         """Construct a quantization options set for the input of a layer.
 
         Args:
-            values (Tuple[Union[numpy.ndarray, QuantizedArray], ...]): calibration data for this op
+            values (Tuple[ONNXOpInputOutputType, ...]): calibration data for this op
             quantized_op_class (Type["QuantizedOp"]): The quantized operator's class
 
         Returns:
             QuantizationOptions: quantization options set, specific to the network conversion method
         """
 
-    # TODO: https://github.com/zama-ai/concrete-ml-internal/issues/195
-    # probably could work by calling layer.quantize_params on each layer just before quantizing them
-    # layer to have weight quantization that manages all that by itself.
     def _quantize_params(self):
         """Transform all floating points initializers to integers."""
         graph: onnx.GraphProto = self.numpy_model.onnx_model.graph
         inits = graph.initializer
         self.quant_params.update(
             (
                 onnx_init.name,
@@ -321,22 +360,22 @@
         # pylint: disable=too-many-locals
 
         graph = self.numpy_model.onnx_model.graph
 
         # Get the list of output tensor names
         graph_output_names = [o.name for o in graph.output]
 
-        node_results: Dict[str, Union[numpy.ndarray, QuantizedArray]] = dict(
+        node_results: Dict[str, ONNXOpInputOutputType] = dict(
             {
                 graph_input.name: input_value
                 for graph_input, input_value in zip(graph.input, input_calibration_data)
             },
             **self.quant_params,
         )
-        node_override_quantizer: Dict[str, UniformQuantizer] = {}
+        node_override_quantizer: Dict[str, Optional[UniformQuantizer]] = {}
 
         constants: Set[str] = set(self.quant_params.keys())
 
         # We need to determine, for each op, whether it only performs univariate computations.
         # A univariate computation is one which depends on a single scalar integer encrypted input
         # which is only multiplied or added to constants or to itself, or a nonlinear function is
         # applied to it.
@@ -372,90 +411,94 @@
             attributes = {attribute.name: get_attribute(attribute) for attribute in node.attribute}
 
             # For now only single output nodes
             assert_true(len(node.output) == 1)
 
             output_name = node.output[0]
             if op_type == "Constant":
-
-                # FIXME: Do not handle constants with QuantizedArray, use numpy.ndarray
-                # let the ops quantize their own inputs
                 constant_values = ONNX_OPS_TO_NUMPY_IMPL["Constant"](**attributes)[0]
                 node_results[output_name] = constant_values
                 constants.add(output_name)
                 continue
 
             quantized_op_class = ONNX_OPS_TO_QUANTIZED_IMPL[op_type]
 
-            # All inputs
-            curr_inputs = {input_name: node_results[input_name] for input_name in node.input}
+            # Add rounding_threshold_bits to the attributes if available in quantized_op_class
+            if issubclass(quantized_op_class, QuantizedMixingOp):
+                attributes.update({"rounding_threshold_bits": self.rounding_threshold_bits})
+
+            # All inputs, allow optional constants (they become None)
+            curr_inputs = {
+                input_name: node_results.get(input_name, None) for input_name in node.input
+            }
 
             # Constant inputs
-            curr_cst_inputs: Dict[int, Union[QuantizedArray, numpy.ndarray]] = {}
+            curr_cst_inputs: Dict[int, ONNXOpInputOutputType] = {}
             for input_idx, (input_name, value) in enumerate(curr_inputs.items()):
                 if not (input_name in self.quant_params or input_name in constants):
                     continue
 
                 if quantized_op_class.must_quantize_input(input_idx):
                     if isinstance(value, QuantizedArray):
                         curr_cst_inputs[input_idx] = value
                     else:
                         # Initializers are ndarray or scalar
+                        assert value is not None
                         assert isinstance(value, numpy.ndarray) or numpy.isscalar(value)
                         curr_cst_inputs[input_idx] = self._process_initializer(
                             self.n_bits_op_weights, value
                         )
                 else:
                     # Initializers are ndarray or scalar
                     assert isinstance(value, numpy.ndarray) or numpy.isscalar(value)
                     curr_cst_inputs[input_idx] = value
 
             has_variable_inputs = (len(curr_inputs) - len(curr_cst_inputs)) > 0
 
+            variable_input_names = [
+                input_name for input_name in curr_inputs if input_name not in constants
+            ]
+            curr_calibration_data = tuple(
+                curr_inputs[input_name] for input_name in variable_input_names
+            )
+
+            # For mypy
+            assert_true(
+                all(val is None or isinstance(val, numpy.ndarray) for val in curr_calibration_data)
+            )
+            curr_calibration_data = cast(Tuple[numpy.ndarray], curr_calibration_data)
+
+            # Find the unique integer producers of the current's op output tensor
+            node_integer_inputs = set.union(
+                *[tensor_int_producers.get(input_node, set()) for input_node in node.input]
+            )
+
             # If we depend on a variable input use the quantized version of the operator
             if has_variable_inputs:
 
                 assert_true(
                     op_type in ONNX_OPS_TO_QUANTIZED_IMPL,
                     f"{op_type} can't be found in {ONNX_OPS_TO_QUANTIZED_IMPL}",
                 )
 
-                variable_input_names = [
-                    input_name for input_name in curr_inputs if input_name not in constants
-                ]
-                curr_calibration_data = tuple(
-                    curr_inputs[input_name] for input_name in variable_input_names
-                )
-
-                # For mypy
-                assert_true(all(isinstance(val, numpy.ndarray) for val in curr_calibration_data))
-                curr_calibration_data = cast(Tuple[numpy.ndarray], curr_calibration_data)
-
-                # Find the unique integer producers of the current's op output tensor
-                node_integer_inputs = set.union(
-                    *[tensor_int_producers.get(input_node, set()) for input_node in node.input]
-                )
-
                 # Note that the output of a quantized op could be a network output
                 # Thus the quantized op outputs are quantized to the network output bitwidth
                 quantized_op_instance = quantized_op_class(
                     self.n_bits_model_outputs,
+                    node.name,
                     node_integer_inputs,
                     curr_cst_inputs,
                     self._get_input_quant_opts(curr_calibration_data, quantized_op_class),
                     **attributes,
                 )
 
                 # Determine if this op computes a tensor that is a graph output, i.e. a tensor
                 # that will be decrypted and dequantized in the clear
                 quantized_op_instance.produces_graph_output = output_name in graph_output_names
 
-                # Set the operation name to be able to link errors to specific ops
-                quantized_op_instance.op_instance_name = node.name
-
                 # Store the output tensor's integer producers
                 tensor_int_producers[output_name] = set()
                 if not quantized_op_instance.can_fuse():
                     # This tensor is produced by a non fusable op
                     # Thus this tensor is marked as produced by itself
                     tensor_int_producers[output_name].add(output_name)
                 else:
@@ -488,37 +531,38 @@
                 # either numpy.array or QuantizedArray
                 real_cst_inputs = (
                     input.values if isinstance(input, QuantizedArray) else input
                     for input in curr_cst_inputs.values()
                 )
 
                 # The output of a constant folding op can be either QuantizedArray or numpy.ndarray
-                node_output: Tuple[Union[numpy.ndarray, QuantizedArray], ...] = ()
+                node_output: Tuple[ONNXOpInputOutputType, ...] = ()
 
                 if get_op_type(node) == QuantizedBrevitasQuant.op_type():
                     list_real_cst_inputs = list(real_cst_inputs)
                     quantizer = QuantizedBrevitasQuant(
                         self.n_bits_model_outputs,
+                        node.name,
                         node_integer_inputs,
                         {
                             1: list_real_cst_inputs[1],
                             2: list_real_cst_inputs[2],
                             3: list_real_cst_inputs[3],
                         },
                         self._get_input_quant_opts(curr_calibration_data, quantized_op_class),
                         **attributes,
                     )
                     # The values to quantize may be stored in a QuantizedArray (for initializers
-                    # and constants), but they can also be float (produced by some other folded
-                    # operation).
-                    constant_values_to_quantize = (
-                        curr_cst_inputs[0]
-                        if isinstance(curr_cst_inputs[0], QuantizedArray)
-                        else self._process_initializer(self.n_bits_op_weights, curr_cst_inputs[0])
-                    )
+                    # and constants)
+                    assert isinstance(
+                        curr_cst_inputs[0], QuantizedArray
+                    ), "Only QuantizedArray constant inputs of a Brevitas quantizer are supported"
+
+                    constant_values_to_quantize = curr_cst_inputs[0]
+
                     # QuantizedBrevitasQuant takes a single input
                     quantizer.calibrate(constant_values_to_quantize.values)
                     node_output = (quantizer(constant_values_to_quantize),)
                 else:
                     node_output = ONNX_OPS_TO_NUMPY_IMPL[op_type](*real_cst_inputs, **attributes)
                 num_output = len(node_output)
                 assert_true(
@@ -557,28 +601,28 @@
 
         self._process_input_quantizers(quantized_module, calibration_data)
 
         return quantized_module
 
     def _process_input_quantizers(
         self, quantized_module: QuantizedModule, calibration_data: Tuple[numpy.ndarray, ...]
-    ):
+    ):  # pylint: disable=too-many-branches
         """Determine the quantizers for a quantized module.
 
         Args:
             quantized_module (QuantizedModule): the quantized module containing the ops of the model
             calibration_data: calibration data for each input tensor
         """
 
         # Create several lists:
         # - a list of layers that use each input directly (i.e. have this input as an integer input)
         # - a list of quantizers that are applied to each input node
         # - a list of inputs that have TLUs, for which these TLUs cannot be removed
         layer_using_input: Dict[int, List[QuantizedOp]] = {}
-        quantizers_for_input: Dict[int, QuantizedBrevitasQuant] = {}
+        quantizers_for_input: Dict[int, List[QuantizedBrevitasQuant]] = {}
         inputs_not_optimizable: List[int] = []
 
         # Determine, for each input, whether it is used by a single non-fusable layer
         # and, optionally, if it is processed by a QAT quantizer in the process
 
         # If the input is used by a fusable op directly, or goes through a uniform QAT quantizer
         # then we can use the QAT quantizer's or fusable-op's quantizer in the clear, instead
@@ -597,54 +641,73 @@
                     # If this is a non-fusable op working on integers, store it
                     # If there is no QAT quantizer on this input, we'll use the op's
                     # input quantizer as the clear-input quantizer
                     layer_using_input[inp_idx].append(q_op)
                 elif isinstance(q_op, QuantizedBrevitasQuant):
                     # If this is a fusable op that is a QAT quantizer, store it
                     # We'll use this quantizer's parameters in the clear-input quantizer
-                    quantizers_for_input[inp_idx] = q_op
+                    if inp_idx not in quantizers_for_input:
+                        quantizers_for_input[inp_idx] = []
+                    quantizers_for_input[inp_idx].append(q_op)
                 else:
                     # If the input is processed by some other type of univariate layer
                     # we cannot optimize out the TLUs on this op by moving them in the clear
                     inputs_not_optimizable.append(inp_idx)
 
-            if len(layer_using_input[inp_idx]) > 1:
-                inputs_not_optimizable.append(inp_idx)
-
         # The input quantizers which we can extract from the graph
         # are:
         # - in quantizers_for_input : QAT quantizers applied directly to inputs
         # - in layer_using_input : quantizers taken from non-fusable ops
         # Now set the input quantizers based on the quantizers that can be extracted from the graph
         q_input_list = []
         for inp_idx, val in enumerate(calibration_data):
-            if inp_idx in inputs_not_optimizable:
+            # If multiple QAT Quantizers are applied to an input, it can not be optimized
+            # to remove the TLU and use a single quantizer in the clear
+            has_multiple_qat_quantizers = (
+                inp_idx in quantizers_for_input and len(quantizers_for_input[inp_idx]) > 1
+            )
+
+            if inp_idx in inputs_not_optimizable or has_multiple_qat_quantizers:
                 # If an input is not optimizable, use the "model_inputs" bits set by the user
                 q_input_list.append(
                     QuantizedArray(self.n_bits_model_inputs, val, is_signed=True).quantizer
                 )
             elif inp_idx in quantizers_for_input:
                 # If a QAT quantizer is applied to this input, use its output params that
                 # are determined from the ONNX file
-                opts = QuantizationOptions(quantizers_for_input[inp_idx].output_quant_opts.n_bits)
-                opts.copy_opts(quantizers_for_input[inp_idx].output_quant_opts)
+                quantizer = quantizers_for_input[inp_idx][0]
+                opts = QuantizationOptions(quantizer.output_quant_opts.n_bits)
+                opts.copy_opts(quantizer.output_quant_opts)
                 # Set the same options as those produced by a QuantizedBrevitasQuant op
                 q_input_list.append(
                     UniformQuantizer(
                         opts,
-                        quantizers_for_input[inp_idx].output_quant_stats,
-                        quantizers_for_input[inp_idx].output_quant_params,
+                        quantizer.output_quant_stats,
+                        quantizer.output_quant_params,
                     )
                 )
+
+                # Propagate the quantization options to non-fusable ops down the line,
+                # since these ops were initialized with a default n_bits - not necessarily
+                # the n_bits set in the QuantizedBrevitasQuant layer
+                for q_op in layer_using_input[inp_idx]:
+                    q_op.input_quant_opts.copy_opts(quantizer.output_quant_opts)
             else:
                 # If the input is injected directly into a non-fusable op (conv, etc...),
                 # use that op's quantization options (ensures matching options that allows
                 # the optimization to take place)
-                assert_true(len(layer_using_input[inp_idx]) == 1)
                 opts = layer_using_input[inp_idx][0].input_quant_opts
+                for layer in layer_using_input[inp_idx][1:]:
+                    opts_k = layer.input_quant_opts
+                    assert_true(
+                        opts.is_equal(opts_k),
+                        "Multiple quantizers "
+                        "applied to the same input must have the same quantization options",
+                    )
+
                 q_input_list.append(QuantizedArray(opts.n_bits, val, options=opts).quantizer)
 
         q_input = tuple(q_input_list)
         quantized_module.set_inputs_quantization_parameters(*q_input)
 
 
 class PostTrainingAffineQuantization(ONNXConverter):
@@ -660,27 +723,29 @@
                                         "model_outputs" keys with corresponding number of
                                         quantization bits for:
                                         - model_inputs : number of bits for model input
                                         - op_inputs : number of bits to quantize layer input values
                                         - op_weights: learned parameters or constants in the network
                                         - model_outputs: final model output quantization bits
         numpy_model (NumpyModule):      Model in numpy.
+        rounding_threshold_bits (int): if not None, every accumulators in the model are rounded down
+            to the given bits of precision
         is_signed:                      Whether the weights of the layers can be signed.
                                         Currently, only the weights can be signed.
 
     Returns:
         QuantizedModule: A quantized version of the numpy model.
     """
 
     def _process_layer(
         self,
         quantized_op: QuantizedOp,
         *calibration_data: numpy.ndarray,
         quantizers: List[Optional[UniformQuantizer]],
-    ) -> Tuple[numpy.ndarray, UniformQuantizer]:
+    ) -> Tuple[numpy.ndarray, Optional[UniformQuantizer]]:
         """Configure a graph operation by performing calibration for uniform quantization.
 
         Args:
             quantized_op (QuantizedOp): Quantized graph operator instance
             *calibration_data (numpy.ndarray): tuple of network input tensors to be used for
                 calibration
             quantizers (List[Optional[UniformQuantizer]]): a list of quantizers that
@@ -692,47 +757,51 @@
             numpy.ndarray: calibration data for the following operators
         """
 
         return self._calibrate_layers_activation(
             True, quantized_op, *calibration_data, quantizers=quantizers
         )
 
-    def _process_initializer(self, n_bits: int, values: Union[numpy.ndarray, QuantizedArray]):
+    def _process_initializer(self, n_bits: int, values: numpy.ndarray):
         """Quantize a network constant tensor (a weights tensor).
 
         The values supplied are floating point values that will be quantized.
 
         Arguments:
             n_bits (int): Number of bits to quantize the weight values
             values (numpy.ndarray): Float values that initialize this tensor
 
         Returns:
             QuantizedArray: a quantized tensor with integer values on n_bits bits
         """
+
+        if isinstance(values, numpy.ndarray) and numpy.issubdtype(values.dtype, numpy.integer):
+            return values.view(RawOpOutput)
+
         assert isinstance(values, (numpy.ndarray, float))
         is_signed = is_symmetric = self._check_distribution_is_symmetric_around_zero(values)
 
         return QuantizedArray(
             n_bits,
             values,
             is_signed=is_signed,
             is_symmetric=is_symmetric,
         )
 
     def _get_input_quant_opts(
         self,
-        values: Tuple[Union[numpy.ndarray, QuantizedArray], ...],
+        values: Tuple[ONNXOpInputOutputType, ...],
         quantized_op_class: Type["QuantizedOp"],
     ):
         """Construct a quantization options set for the input of a layer.
 
         Inputs and activations require signed quantization.
 
         Args:
-            values (Tuple[Union[numpy.ndarray, QuantizedArray], ...]): calibration data for this op
+            values (Tuple[ONNXOpInputOutputType, ...]): calibration data for this op
             quantized_op_class (Type["QuantizedOp"]): The quantized operator's class
 
         Returns:
             QuantizationOptions: quantization options set, specific to the network conversion method
         """
         is_signed = any(v.min() < 0 for v in values if isinstance(v, numpy.ndarray)) or any(
             v.values.min() < 0 for v in values if isinstance(v, QuantizedArray)
@@ -793,15 +862,15 @@
     """
 
     def _process_layer(
         self,
         quantized_op: QuantizedOp,
         *calibration_data: numpy.ndarray,
         quantizers: List[Optional[UniformQuantizer]],
-    ) -> Tuple[numpy.ndarray, UniformQuantizer]:
+    ) -> Tuple[numpy.ndarray, Optional[UniformQuantizer]]:
         """Configure a graph operation by calibrating it for Quantization Aware Training.
 
         Args:
             quantized_op (QuantizedOp): Quantized graph operator instance
             *calibration_data (numpy.ndarray): tuple of network input tensors to be used for
                 calibration
             quantizers (List[Optional[UniformQuantizer]]): a list of quantizers that
@@ -813,15 +882,15 @@
             numpy.ndarray: calibration data for the following operators
         """
 
         return self._calibrate_layers_activation(
             False, quantized_op, *calibration_data, quantizers=quantizers
         )
 
-    def _process_initializer(self, n_bits: int, values: Union[numpy.ndarray, QuantizedArray]):
+    def _process_initializer(self, n_bits: int, values: numpy.ndarray):
         """Process an already quantized weight tensor.
 
         The values supplied are in floating point, but are discrete, in the sense
         that the number of unique (possible) values is equal to 2**n_bits. These values,
         w_hat take the form w_hat = alpha * w_int, where w_int are integer values. Therefore, this
         function will retrieve the alpha and w_int that form w_hat which is passed here as `values`.
 
@@ -829,29 +898,44 @@
             n_bits (int): Number of bits that was used to quantize the weight values
             values (numpy.ndarray): Discrete float values that initialize this tensor
 
         Returns:
             QuantizedArray: a quantized tensor with integer values on n_bits bits and with alpha as
                 the scaling factor.
         """
-        assert isinstance(values, (numpy.ndarray, float))
+
+        # Assume that integer initializer op inputs are raw values that should not be quantized
+        # This allows to have patterns such as Add(shape(x)[0], 1). In this case the value `1`
+        # is the integer initializer and should not be quantized.
+        if isinstance(values, numpy.ndarray) and numpy.issubdtype(values.dtype, numpy.integer):
+            return values.view(RawOpOutput)
+
+        assert_true(
+            isinstance(values, float)
+            or (
+                isinstance(values, numpy.ndarray) and numpy.issubdtype(values.dtype, numpy.floating)
+            ),
+            f"ONNX initializers must be float if not marked as raw arguments, "
+            f"got {values.dtype if isinstance(values, numpy.ndarray) else type(values)} "
+            f"for initializer {values}",
+        )
         return QuantizedArray(n_bits, values, is_signed=True, is_symmetric=False, is_qat=True)
 
     def _get_input_quant_opts(
         self,
-        values: Tuple[Union[numpy.ndarray, QuantizedArray], ...],
+        values: Tuple[ONNXOpInputOutputType, ...],
         quantized_op_class: Type["QuantizedOp"],
     ):
         """Construct a quantization options set for the input of a layer of a QAT network.
 
         QAT networks require specific quantization for inputs to nodes that perform quantization
         (such as Gemm/Conv/Add).
 
         Args:
-            values (Tuple[Union[numpy.ndarray, QuantizedArray], ...]): calibration data for this op
+            values (Tuple[ONNXOpInputOutputType, ...]): calibration data for this op
             quantized_op_class (Type["QuantizedOp"]): The quantized operator's class
 
         Returns:
             QuantizationOptions: quantization options set, specific to the network conversion method
         """
 
         # Some operators need to quantize their inputs using model_outputs instead of op_inputs in
```

## concrete/ml/quantization/quantized_module.py

```diff
@@ -1,24 +1,31 @@
 """QuantizedModule API."""
 import copy
+import re
 from typing import Any, Dict, Generator, Iterable, List, Optional, Tuple, Union
 
 import numpy
-from concrete.numpy.compilation.artifacts import DebugArtifacts
-from concrete.numpy.compilation.circuit import Circuit
-from concrete.numpy.compilation.compiler import Compiler
-from concrete.numpy.compilation.configuration import Configuration
+from concrete.fhe.compilation.artifacts import DebugArtifacts
+from concrete.fhe.compilation.circuit import Circuit
+from concrete.fhe.compilation.compiler import Compiler
+from concrete.fhe.compilation.configuration import Configuration
 
 from ..common.debugging import assert_true
 from ..common.utils import (
+    SUPPORTED_FLOAT_TYPES,
+    SUPPORTED_INT_TYPES,
+    FheMode,
+    all_values_are_floats,
+    all_values_are_integers,
     check_there_is_no_p_error_options_in_configuration,
     generate_proxy_function,
     manage_parameters_for_pbs_errors,
+    to_tuple,
 )
-from .base_quantized_op import QuantizedOp
+from .base_quantized_op import ONNXOpInputOutputType, QuantizedOp
 from .quantizers import QuantizedArray, UniformQuantizer
 
 
 def _raise_qat_import_error(bad_qat_ops: List[Tuple[str, str]]):
     """Raise a descriptive error if any invalid ops are present in the ONNX graph.
 
     Args:
@@ -39,50 +46,63 @@
             )
         )
         + "\n\nCould not determine a unique scale for the quantization! "
         "Please check the ONNX graph of this model."
     )
 
 
-def _get_inputset_generator(
-    q_inputs: Tuple[numpy.ndarray, ...], input_quantizers: List[UniformQuantizer]
-) -> Generator:
+def _get_inputset_generator(q_inputs: Union[numpy.ndarray, Tuple[numpy.ndarray, ...]]) -> Generator:
     """Create an input set generator with proper dimensions.
 
     Args:
-        q_inputs (numpy.ndarray): The quantized inputs
-        input_quantizers (List[UniformQuantizer]): The input quantizers used on the input set
+        q_inputs (Union[numpy.ndarray, Tuple[numpy.ndarray, ...]]): The quantized inputs.
 
     Returns:
         Generator: The input set generator with proper dimensions.
     """
-    if len(input_quantizers) > 1:
+    q_inputs = to_tuple(q_inputs)
+
+    assert len(q_inputs) > 0, "Inputset cannot be empty"
+
+    if len(q_inputs) > 1:
         return (
             tuple(numpy.expand_dims(q_input[idx], 0) for q_input in q_inputs)
             for idx in range(q_inputs[0].shape[0])
         )
-    return (numpy.expand_dims(arr, 0) for arr in q_inputs[0])
+
+    # Else, there's only a single input (q_inputs, )
+    return (numpy.expand_dims(q_input, 0) for q_input in q_inputs[0])
 
 
 class QuantizedModule:
     """Inference for a quantized model."""
 
     ordered_module_input_names: Tuple[str, ...]
     ordered_module_output_names: Tuple[str, ...]
     quant_layers_dict: Dict[str, Tuple[Tuple[str, ...], QuantizedOp]]
     input_quantizers: List[UniformQuantizer]
     output_quantizers: List[UniformQuantizer]
-    forward_fhe: Union[None, Circuit]
+    fhe_circuit: Union[None, Circuit]
 
     def __init__(
         self,
         ordered_module_input_names: Iterable[str] = None,
         ordered_module_output_names: Iterable[str] = None,
         quant_layers_dict: Dict[str, Tuple[Tuple[str, ...], QuantizedOp]] = None,
     ):
+        # Set base attributes for API consistency. This could be avoided if an abstract base class
+        # is created for both Concrete ML models and QuantizedModule
+        # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/2899
+        self.fhe_circuit = None
+        self._is_compiled = False
+        self.input_quantizers = []
+        self.output_quantizers = []
+        self._onnx_model = None
+        self._post_processing_params: Dict[str, Any] = {}
+
         # If any of the arguments are not provided, skip the init
         if not all([ordered_module_input_names, ordered_module_output_names, quant_layers_dict]):
             return
 
         # for mypy
         assert isinstance(ordered_module_input_names, Iterable)
         assert isinstance(ordered_module_output_names, Iterable)
@@ -95,48 +115,36 @@
             (num_outputs) == 1,
             f"{QuantizedModule.__class__.__name__} only supports a single output for now, "
             f"got {num_outputs}",
         )
 
         assert quant_layers_dict is not None
         self.quant_layers_dict = copy.deepcopy(quant_layers_dict)
-        self._is_compiled = False
-        self.forward_fhe = None
-        self.input_quantizers = []
         self.output_quantizers = self._set_output_quantizers()
-        self._onnx_model = None
-        self._post_processing_params: Dict[str, Any] = {}
 
     @property
     def is_compiled(self) -> bool:
-        """Return the compiled status of the module.
+        """Indicate if the model is compiled.
 
         Returns:
-            bool: the compiled status of the module.
+            bool: If the model is compiled.
         """
         return self._is_compiled
 
-    @property
-    def fhe_circuit(self) -> Circuit:
-        """Get the FHE circuit.
-
-        Returns:
-            Circuit: the FHE circuit
-        """
-        return self.forward_fhe
-
-    @fhe_circuit.setter
-    def fhe_circuit(self, fhe_circuit: Circuit):
-        """Set the FHE circuit.
+    def check_model_is_compiled(self):
+        """Check if the quantized module is compiled.
 
-        Args:
-            fhe_circuit (Circuit): the FHE circuit
+        Raises:
+            AttributeError: If the quantized module is not compiled.
         """
-        self.forward_fhe = fhe_circuit
-        self._is_compiled = True
+        if not self.is_compiled:
+            raise AttributeError(
+                "The quantized module is not compiled. Please run compile(...) first before "
+                "executing it in FHE."
+            )
 
     @property
     def post_processing_params(self) -> Dict[str, Any]:
         """Get the post-processing parameters.
 
         Returns:
             Dict[str, Any]: the post-processing parameters
@@ -148,24 +156,28 @@
         """Set the post-processing parameters.
 
         Args:
             post_processing_params (dict): the post-processing parameters
         """
         self._post_processing_params = post_processing_params
 
-    def post_processing(self, qvalues: numpy.ndarray) -> numpy.ndarray:
-        """Post-processing of the quantized output.
+    # pylint: disable-next=no-self-use
+    def post_processing(self, values: numpy.ndarray) -> numpy.ndarray:
+        """Apply post-processing to the dequantized values.
+
+        For quantized modules, there is no post-processing step but the method is kept to make the
+        API consistent for the client-server API.
 
         Args:
-            qvalues (numpy.ndarray): numpy.ndarray containing the quantized input values.
+            values (numpy.ndarray): The dequantized values to post-process.
 
         Returns:
-            (numpy.ndarray): Predictions of the quantized model
+            numpy.ndarray: The post-processed values.
         """
-        return self.dequantize_output(qvalues)
+        return values
 
     def _set_output_quantizers(self) -> List[UniformQuantizer]:
         """Get the output quantizers.
 
         Returns:
             List[UniformQuantizer]: List of output quantizers.
         """
@@ -197,95 +209,162 @@
         return self._onnx_model
 
     @onnx_model.setter
     def onnx_model(self, value):
         self._onnx_model = value
 
     def __call__(self, *x: numpy.ndarray):
+        """Define the QuantizedModule's call method.
+
+        This method is a forward method executed in the clear.
+
+        Args:
+            *x (numpy.ndarray): Input float values to consider.
+
+        Returns:
+            numpy.ndarray: Predictions of the quantized model, in floating points.
+        """
         return self.forward(*x)
 
     def forward(
-        self, *qvalues: numpy.ndarray, debug: bool = False
-    ) -> Union[numpy.ndarray, Tuple[numpy.ndarray, Dict[str, numpy.ndarray]]]:
-        """Forward pass with numpy function only.
+        self,
+        *x: numpy.ndarray,
+        fhe: Union[FheMode, str] = FheMode.DISABLE,
+        debug: bool = False,
+    ) -> Union[numpy.ndarray, Tuple[numpy.ndarray, Optional[Dict[Any, Any]]]]:
+        """Forward pass with numpy function only on floating points.
+
+        This method executes the forward pass in the clear, with simulation or in FHE. Input values
+        are expected to be floating points, as the method handles the quantization step. The
+        returned values are floating points as well.
 
         Args:
-            *qvalues (numpy.ndarray): numpy.array containing the quantized values.
+            *x (numpy.ndarray): Input float values to consider.
+            fhe (Union[FheMode, str]): The mode to use for prediction. Can be FheMode.DISABLE for
+                Concrete ML python inference, FheMode.SIMULATE for FHE simulation and
+                FheMode.EXECUTE for actual FHE execution. Can also be the string representation of
+                any of these values. Default to FheMode.DISABLE.
             debug (bool): In debug mode, returns quantized intermediary values of the computation.
-                          This is useful when a model's intermediary values in Concrete-ML need
-                          to be compared with the intermediary values obtained in pytorch/onnx.
-                          When set, the second return value is a dictionary containing ONNX
-                          operation names as keys and, as values, their input QuantizedArray or
-                          ndarray. The use can thus extract the quantized or float values of
-                          quantized inputs.
+                This is useful when a model's intermediary values in Concrete ML need to be
+                compared with the intermediary values obtained in pytorch/onnx. When set, the
+                second return value is a dictionary containing ONNX operation names as keys and,
+                as values, their input QuantizedArray or ndarray. The use can thus extract the
+                quantized or float values of quantized inputs. This feature is only available in
+                FheMode.DISABLE mode. Default to False.
 
         Returns:
-            (numpy.ndarray): Predictions of the quantized model
-        """
-        # Make sure that the input is quantized
-        invalid_inputs = tuple(
-            (idx, qvalue)
-            for idx, qvalue in enumerate(qvalues)
-            if not issubclass(qvalue.dtype.type, numpy.integer)
+            numpy.ndarray: Predictions of the quantized model, in floating points.
+        """
+        assert_true(
+            FheMode.is_valid(fhe),
+            "`fhe` mode is not supported. Expected one of 'disable' (resp. FheMode.DISABLE), "
+            "'simulate' (resp. FheMode.SIMULATE) or 'execute' (resp. FheMode.EXECUTE). Got "
+            f"{fhe}",
         )
+
+        # Make sure that the inputs are floating points
         assert_true(
-            len(invalid_inputs) == 0,
-            f"Inputs: {', '.join(f'#{val[0]} ({val[1].dtype})' for val in invalid_inputs)} are not "
-            "integer types. Make sure you quantize your input before calling forward.",
-            ValueError,
+            all_values_are_floats(*x),
+            "Input values are expected to be floating points of dtype "
+            f"{SUPPORTED_FLOAT_TYPES}. Do not quantize the inputs manually as it is handled "
+            "within this method.",
+            TypeError,
         )
 
-        if debug:
-            debug_value_tracker: Dict[str, Any] = {}
+        # Quantized the input values
+        q_x = to_tuple(self.quantize_input(*x))
+
+        if debug and fhe == "disable":
+            debug_value_tracker: Optional[
+                Dict[str, Dict[Union[int, str], Optional[ONNXOpInputOutputType]]]
+            ] = {}
             for (_, layer) in self.quant_layers_dict.values():
                 layer.debug_value_tracker = debug_value_tracker
-            result = self._forward(*qvalues)
+            result = self.quantized_forward(*q_x, fhe="disable")
             for (_, layer) in self.quant_layers_dict.values():
                 layer.debug_value_tracker = None
             return result, debug_value_tracker
 
-        return self._forward(*qvalues)
+        q_y_pred = self.quantized_forward(*q_x, fhe=fhe)
 
-    def _forward(self, *qvalues: numpy.ndarray) -> numpy.ndarray:
+        # Dequantize the output predicted values
+        y_pred = self.dequantize_output(q_y_pred)
+
+        return y_pred
+
+    def quantized_forward(
+        self, *q_x: numpy.ndarray, fhe: Union[FheMode, str] = FheMode.DISABLE
+    ) -> numpy.ndarray:
         """Forward function for the FHE circuit.
 
         Args:
-            *qvalues (numpy.ndarray): numpy.array containing the quantized values.
+            *q_x (numpy.ndarray): Input integer values to consider.
+            fhe (Union[FheMode, str]): The mode to use for prediction. Can be FheMode.DISABLE for
+                Concrete ML python inference, FheMode.SIMULATE for FHE simulation and
+                FheMode.EXECUTE for actual FHE execution. Can also be the string representation of
+                any of these values. Default to FheMode.DISABLE.
 
         Returns:
-            (numpy.ndarray): Predictions of the quantized model
+            (numpy.ndarray): Predictions of the quantized model, with integer values.
 
         """
-
-        n_qinputs = len(self.input_quantizers)
-        n_qvalues = len(qvalues) == n_qinputs
+        # Make sure that the inputs are integers
         assert_true(
-            n_qvalues,
-            f"Got {n_qvalues} inputs, expected {n_qinputs}",
+            all_values_are_integers(*q_x),
+            f"Input values are expected to be integers of dtype {SUPPORTED_INT_TYPES}. "
+            "Please quantize the inputs manually as it is not handled within this method.",
             TypeError,
         )
 
+        n_inputs = len(self.input_quantizers)
+        n_values = len(q_x)
+        assert_true(
+            n_values == n_inputs,
+            f"Got {n_values} inputs, expected {n_inputs}. Either the quantized module has not been "
+            "properly initialized or the input data has been changed since its initialization.",
+            ValueError,
+        )
+
+        if fhe == "disable":
+            return self._clear_forward(*q_x)
+
+        simulate = fhe == "simulate"
+        return self._fhe_forward(*q_x, simulate=simulate)
+
+    def _clear_forward(self, *q_x: numpy.ndarray) -> numpy.ndarray:
+        """Forward function for the FHE circuit executed in the clear.
+
+        Args:
+            *q_x (numpy.ndarray): Input integer values to consider.
+
+        Returns:
+            (numpy.ndarray): Predictions of the quantized model, with integer values.
+
+        """
+
         q_inputs = [
             QuantizedArray(
                 self.input_quantizers[idx].n_bits,
-                qvalues[idx],
+                q_x[idx],
                 value_is_float=False,
                 options=self.input_quantizers[idx].quant_options,
                 stats=self.input_quantizers[idx].quant_stats,
                 params=self.input_quantizers[idx].quant_params,
             )
             for idx in range(len(self.input_quantizers))
         ]
 
         # Init layer_results with the inputs
-        layer_results = dict(zip(self.ordered_module_input_names, q_inputs))
+        layer_results: Dict[str, ONNXOpInputOutputType] = dict(
+            zip(self.ordered_module_input_names, q_inputs)
+        )
 
         bad_qat_ops: List[Tuple[str, str]] = []
         for output_name, (input_names, layer) in self.quant_layers_dict.items():
-            inputs = (layer_results[input_name] for input_name in input_names)
+            inputs = (layer_results.get(input_name, None) for input_name in input_names)
 
             error_tracker: List[int] = []
             layer.error_tracker = error_tracker
             output = layer(*inputs)
             layer.error_tracker = None
 
             if len(error_tracker) > 0:
@@ -295,160 +374,251 @@
                     bad_qat_ops.append((input_names[input_idx], layer.__class__.op_type()))
 
             layer_results[output_name] = output
 
         if len(bad_qat_ops) > 0:
             _raise_qat_import_error(bad_qat_ops)
 
-        outputs = tuple(
+        output_quantized_arrays = tuple(
             layer_results[output_name] for output_name in self.ordered_module_output_names
         )
 
-        assert_true(len(outputs) == 1)
+        assert_true(len(output_quantized_arrays) == 1)
+
+        # The output of a graph must be a QuantizedArray
+        assert isinstance(output_quantized_arrays[0], QuantizedArray)
 
-        return outputs[0].qvalues
+        return output_quantized_arrays[0].qvalues
 
-    def forward_and_dequant(self, *q_x: numpy.ndarray) -> numpy.ndarray:
-        """Forward pass with numpy function only plus dequantization.
+    def _fhe_forward(self, *q_x: numpy.ndarray, simulate: bool = True) -> numpy.ndarray:
+        """Forward function executed in FHE or with simulation.
 
         Args:
-            *q_x (numpy.ndarray): numpy.ndarray containing the quantized input values. Requires the
-                input dtype to be int64.
+            *q_x (numpy.ndarray): Input integer values to consider.
+            simulate (bool): Whether the function should be run in FHE or in simulation mode.
+                Default to True.
 
         Returns:
-            (numpy.ndarray): Predictions of the quantized model
+            (numpy.ndarray): Predictions of the quantized model, with integer values.
+
         """
-        q_out = self.forward(*q_x)
-        return self.dequantize_output(q_out)  # type: ignore
 
-    def quantize_input(
-        self, *values: numpy.ndarray
-    ) -> Union[numpy.ndarray, Tuple[numpy.ndarray, ...]]:
+        # Make sure that the module is compiled
+        assert_true(
+            self.fhe_circuit is not None,
+            "The quantized module is not compiled. Please run compile(...) first before "
+            "executing it in FHE.",
+        )
+
+        # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/2888
+        # Check if rounding is being executed in FHE, which is not currently optimized
+        # Assert that there are rounding nodes in the circuit graph
+        rounding_nodes = self.fhe_circuit.graph.query_nodes(  # type: ignore[union-attr]
+            operation_filter="round_bit_pattern"
+        )
+
+        assert_true(
+            not rounding_nodes or simulate,
+            "Rounding is not currently optimized for execution in FHE. "
+            "Only simulation is allowed with a rounding operator.",
+        )
+
+        results_cnp_circuit_list = []
+        for i in range(q_x[0].shape[0]):
+
+            # Extract the i th example from every element in the tuple q_x
+            q_input = tuple(q_x[input][[i]] for input in range(len(q_x)))
+
+            # For mypy
+            assert self.fhe_circuit is not None
+
+            # Execute the forward pass in FHE or with simulation
+            q_result = (
+                self.fhe_circuit.simulate(*q_input)
+                if simulate
+                else self.fhe_circuit.encrypt_run_decrypt(*q_input)
+            )
+            results_cnp_circuit_list.append(q_result)
+
+        results_cnp_circuit = numpy.concatenate(results_cnp_circuit_list, axis=0)
+
+        return results_cnp_circuit
+
+    def quantize_input(self, *x: numpy.ndarray) -> Union[numpy.ndarray, Tuple[numpy.ndarray, ...]]:
         """Take the inputs in fp32 and quantize it using the learned quantization parameters.
 
         Args:
-            *values (numpy.ndarray): Floating point values.
+            x (numpy.ndarray): Floating point x.
 
         Returns:
-            Union[numpy.ndarray, Tuple[numpy.ndarray, ...]]: Quantized (numpy.int64) values.
+            Union[numpy.ndarray, Tuple[numpy.ndarray, ...]]: Quantized (numpy.int64) x.
         """
-        n_qinputs = len(self.input_quantizers)
-        n_values = len(values) == n_qinputs
+        n_inputs = len(self.input_quantizers)
+        n_values = len(x)
         assert_true(
-            n_values,
-            f"Got {n_values} inputs, expected {n_qinputs}",
-            TypeError,
+            n_values == n_inputs,
+            f"Got {n_values} inputs, expected {n_inputs}. Either the quantized module has not been "
+            "properly initialized or the input data has been changed since its initialization.",
+            ValueError,
         )
 
-        qvalues = tuple(self.input_quantizers[idx].quant(values[idx]) for idx in range(len(values)))
+        q_x = tuple(self.input_quantizers[idx].quant(x[idx]) for idx in range(len(x)))
+
+        assert numpy.array(q_x).dtype == numpy.int64, "Inputs were not quantized to int64 x"
 
-        return qvalues[0] if len(qvalues) == 1 else qvalues
+        return q_x[0] if len(q_x) == 1 else q_x
 
-    def dequantize_output(self, qvalues: numpy.ndarray) -> numpy.ndarray:
+    def dequantize_output(self, q_y_preds: numpy.ndarray) -> numpy.ndarray:
         """Take the last layer q_out and use its dequant function.
 
         Args:
-            qvalues (numpy.ndarray): Quantized values of the last layer.
+            q_y_preds (numpy.ndarray): Quantized output values of the last layer.
 
         Returns:
-            numpy.ndarray: Dequantized values of the last layer.
+            numpy.ndarray: Dequantized output values of the last layer.
         """
-        real_values = tuple(
-            output_quantizer.dequant(qvalues) for output_quantizer in self.output_quantizers
+        y_preds = tuple(
+            output_quantizer.dequant(q_y_preds) for output_quantizer in self.output_quantizers
         )
 
-        assert_true(len(real_values) == 1)
+        assert_true(len(y_preds) == 1)
 
-        return real_values[0]
+        return y_preds[0]
 
     def set_inputs_quantization_parameters(self, *input_q_params: UniformQuantizer):
         """Set the quantization parameters for the module's inputs.
 
         Args:
             *input_q_params (UniformQuantizer): The quantizer(s) for the module.
         """
         n_inputs = len(self.ordered_module_input_names)
         n_values = len(input_q_params)
         assert_true(
             n_values == n_inputs,
-            f"Got {n_values} inputs, expected {n_inputs}",
-            TypeError,
+            f"Got {n_values} inputs, expected {n_inputs}. Either the quantized module has not been "
+            "properly initialized or the input data has been changed since its initialization.",
+            ValueError,
         )
 
         self.input_quantizers.clear()
         self.input_quantizers.extend(copy.deepcopy(q_params) for q_params in input_q_params)
 
     def compile(
         self,
-        q_inputs: Union[Tuple[numpy.ndarray, ...], numpy.ndarray],
+        inputs: Union[Tuple[numpy.ndarray, ...], numpy.ndarray],
         configuration: Optional[Configuration] = None,
-        compilation_artifacts: Optional[DebugArtifacts] = None,
+        artifacts: Optional[DebugArtifacts] = None,
         show_mlir: bool = False,
-        use_virtual_lib: bool = False,
         p_error: Optional[float] = None,
         global_p_error: Optional[float] = None,
-        verbose_compilation: bool = False,
+        verbose: bool = False,
     ) -> Circuit:
-        """Compile the forward function of the module.
+        """Compile the module's forward function.
 
         Args:
-            q_inputs (Union[Tuple[numpy.ndarray, ...], numpy.ndarray]): Needed for tracing and
-                building the boundaries.
-            configuration (Optional[Configuration]): Configuration object to use during compilation
-            compilation_artifacts (Optional[DebugArtifacts]): Artifacts object to fill during
-            show_mlir (bool): if set, the MLIR produced by the converter and which is
-                going to be sent to the compiler backend is shown on the screen, e.g., for debugging
-                or demo. Defaults to False.
-            use_virtual_lib (bool): set to use the so called virtual lib simulating FHE computation.
-                Defaults to False.
-            p_error (Optional[float]): probability of error of a single PBS.
-            global_p_error (Optional[float]): probability of error of the full circuit. Not
-                simulated by the VL, i.e., taken as 0
-            verbose_compilation (bool): whether to show compilation information
-
-        Returns:
-            Circuit: the compiled Circuit.
-        """
-
-        if not isinstance(q_inputs, tuple):
-            q_inputs = (q_inputs,)
-        else:
-            ref_len = q_inputs[0].shape[0]
-            assert_true(
-                all(q_input.shape[0] == ref_len for q_input in q_inputs),
-                "Mismatched dataset lengths",
-            )
+            inputs (numpy.ndarray): A representative set of input values used for building
+                cryptographic parameters.
+            configuration (Optional[Configuration]): Options to use for compilation. Default
+                to None.
+            artifacts (Optional[DebugArtifacts]): Artifacts information about the
+                compilation process to store for debugging.
+            show_mlir (bool): Indicate if the MLIR graph should be printed during compilation.
+            p_error (Optional[float]): Probability of error of a single PBS. A p_error value cannot
+                be given if a global_p_error value is already set. Default to None, which sets this
+                error to a default value.
+            global_p_error (Optional[float]): Probability of error of the full circuit. A
+                global_p_error value cannot be given if a p_error value is already set. This feature
+                is not supported during simulation, meaning the probability is
+                currently set to 0. Default to None, which sets this
+                error to a default value.
+            verbose (bool): Indicate if compilation information should be printed
+                during compilation. Default to False.
+
+        Returns:
+            Circuit: The compiled Circuit.
+        """
+        inputs = to_tuple(inputs)
 
-        # concrete-numpy does not support variable *args-style functions, so compile a proxy
+        ref_len = inputs[0].shape[0]
+        assert_true(
+            all(input.shape[0] == ref_len for input in inputs),
+            "Mismatched dataset lengths",
+        )
+
+        assert not numpy.any([numpy.issubdtype(input.dtype, numpy.integer) for input in inputs]), (
+            "Inputs used for compiling a QuantizedModule should only be floating points and not"
+            "already-quantized values."
+        )
+
+        # Concrete does not support variable *args-style functions, so compile a proxy
         # function dynamically with a suitable number of arguments
         forward_proxy, orig_args_to_proxy_func_args = generate_proxy_function(
-            self._forward, self.ordered_module_input_names
+            self._clear_forward, self.ordered_module_input_names
         )
 
         compiler = Compiler(
             forward_proxy,
             {arg_name: "encrypted" for arg_name in orig_args_to_proxy_func_args.values()},
         )
 
-        inputset = _get_inputset_generator(q_inputs, self.input_quantizers)
+        # Quantize the inputs
+        q_inputs = self.quantize_input(*inputs)
+
+        # Generate the inputset with proper dimensions
+        inputset = _get_inputset_generator(q_inputs)
 
         # Don't let the user shoot in her foot, by having p_error or global_p_error set in both
         # configuration and in direct arguments
         check_there_is_no_p_error_options_in_configuration(configuration)
 
         # Find the right way to set parameters for compiler, depending on the way we want to default
         p_error, global_p_error = manage_parameters_for_pbs_errors(p_error, global_p_error)
 
-        self.forward_fhe = compiler.compile(
+        self.fhe_circuit = compiler.compile(
             inputset,
-            configuration,
-            compilation_artifacts,
+            configuration=configuration,
+            artifacts=artifacts,
             show_mlir=show_mlir,
-            virtual=use_virtual_lib,
             p_error=p_error,
             global_p_error=global_p_error,
-            verbose=verbose_compilation,
+            verbose=verbose,
         )
 
         self._is_compiled = True
 
-        return self.forward_fhe
+        return self.fhe_circuit
+
+    def bitwidth_and_range_report(
+        self,
+    ) -> Optional[Dict[str, Dict[str, Union[Tuple[int, ...], int]]]]:
+        """Report the ranges and bitwidths for layers that mix encrypted integer values.
+
+        Returns:
+            op_names_to_report (Dict): a dictionary with operation names as keys. For each
+                operation, (e.g. conv/gemm/add/avgpool ops), a range and a bitwidth are returned.
+                The range contains the min/max values encountered when computing the operation and
+                the bitwidth gives the number of bits needed to represent this range.
+        """
+
+        if self.fhe_circuit is None:
+            return None
+
+        op_names_to_report: Dict[str, Dict[str, Union[Tuple[int, ...], int]]] = {}
+        for (_, op_inst) in self.quant_layers_dict.values():
+            # Get the value range of this tag and all its subtags
+            # The potential tags for this op start with the op instance name
+            # and are, sometimes, followed by a subtag starting with a period:
+            # ex: abc, abc.cde, abc.cde.fgh
+            # so first craft a regex to match all such tags.
+            pattern = re.compile(re.escape(op_inst.op_instance_name) + "(\\..*)?")
+            value_range = self.fhe_circuit.graph.integer_range(pattern)
+            bitwidth = self.fhe_circuit.graph.maximum_integer_bit_width(pattern)
+
+            # Only store the range and bit-width if there are valid ones,
+            # as some ops (fusable ones) do not have tags
+            if value_range is not None and bitwidth >= 0:
+                op_names_to_report[op_inst.op_instance_name] = {
+                    "range": value_range,
+                    "bitwidth": bitwidth,
+                }
+
+        return op_names_to_report
```

## concrete/ml/quantization/quantized_ops.py

```diff
@@ -1,27 +1,35 @@
 """Quantized versions of the ONNX operators for post training quantization."""
 
 # pylint: disable=too-many-lines
 
-# FIXME: #1018
+# This file is too long and should be splitted
+# FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/1018
 
 from typing import Any, Dict, Optional, Sequence, Set, Union
 
 import numpy
-from concrete.onnx import conv as cnp_conv
-from concrete.onnx import maxpool as cnp_maxpool
+from concrete.fhe import conv as cnp_conv
+from concrete.fhe import maxpool as cnp_maxpool
+from concrete.fhe import tag
 from typing_extensions import SupportsIndex
 
 from ..common.debugging import assert_false, assert_true
 from ..onnx.onnx_impl_utils import (
     compute_onnx_pool_padding,
     numpy_onnx_pad,
     onnx_avgpool_compute_norm_const,
 )
-from .base_quantized_op import QuantizedMixingOp, QuantizedOp, QuantizedOpUnivariateOfEncrypted
+from ..onnx.ops_impl import RawOpOutput
+from .base_quantized_op import (
+    ONNXOpInputOutputType,
+    QuantizedMixingOp,
+    QuantizedOp,
+    QuantizedOpUnivariateOfEncrypted,
+)
 from .quantizers import QuantizationOptions, QuantizedArray, UniformQuantizationParameters
 
 
 def _check_op_input_zero_point(zero_point: Any, op_name: Optional[str]):
     """Check that an operation's quantized input zero-point is a single value.
 
     Args:
@@ -121,20 +129,28 @@
     """Quantized Gemm op."""
 
     _impl_for_op_named: str = "Gemm"
 
     def __init__(
         self,
         n_bits_output: int,
+        op_instance_name: str,
         int_input_names: Set[str] = None,
         constant_inputs: Optional[Union[Dict[str, Any], Dict[int, Any]]] = None,
         input_quant_opts: QuantizationOptions = None,
         **attrs,
     ) -> None:
-        super().__init__(n_bits_output, int_input_names, constant_inputs, input_quant_opts, **attrs)
+        super().__init__(
+            n_bits_output,
+            op_instance_name,
+            int_input_names,
+            constant_inputs,
+            input_quant_opts,
+            **attrs,
+        )
 
         alpha = self.attrs.get("alpha", 1)
         beta = self.attrs.get("beta", 1)
 
         assert_true(
             alpha == 1 and beta in [0, 1],
             f"{self.__class__.__name__} currently only supports alpha == 1 and beta in [0, 1].\n"
@@ -145,17 +161,18 @@
             1 in self.constant_inputs,
             f"{self.__class__.__name__} currently only supports quantizing "
             f"{self._impl_for_op_named} if weights are provided as the 'b' constant input.",
         )
 
     def q_impl(
         self,
-        *q_inputs: QuantizedArray,
+        *q_inputs: ONNXOpInputOutputType,
+        calibrate_rounding: bool = False,
         **attrs,
-    ) -> QuantizedArray:
+    ) -> ONNXOpInputOutputType:
 
         alpha = self.attrs.get("alpha", 1)
         beta = self.attrs.get("beta", 1)
 
         # If alpha != 1 or beta not in [0, 1], this function must be modified
         assert_true(alpha == 1)
         assert_true(beta in [0, 1])
@@ -171,15 +188,18 @@
         )
 
         # Using snake case here to please the python format, the original attrs don't have the '_'
         # Use default false so we also support MatMul impl, MatMul does not have these flags
         transpose_inputs = attrs.get("transA", False)
         transpose_w = attrs.get("transB", False)
 
-        input_q_values = numpy.transpose(q_input.qvalues) if transpose_inputs else q_input.qvalues
+        with tag(self.op_instance_name + ".input"):
+            input_q_values = (
+                numpy.transpose(q_input.qvalues) if transpose_inputs else q_input.qvalues
+            )
         weights_q_values = numpy.transpose(q_weights.qvalues) if transpose_w else q_weights.qvalues
 
         # For mypy
         assert self.output_quant_params is not None
         assert self.output_quant_params.scale is not None
         assert self.output_quant_params.zero_point is not None
 
@@ -195,30 +215,37 @@
 
         # Here we follow Eq.7 in https://arxiv.org/abs/1712.05877 to split the core computation
         # from the zero points and scales.
 
         p = weights_q_values.shape[0]
 
         # Core matmul operation in full integers with a shape change (INTEGERS)
-        matmul = input_q_values @ weights_q_values
+        with tag(self.op_instance_name + ".matmul"):
+            matmul = input_q_values @ weights_q_values
 
         # If the weights have symmetric quantization, their zero point will be 0
         # The following check avoids the computation of the sum of the inputs, which may have
         # large bitwidth, in the case where it would be multiplied by zero
         if q_weights.quantizer.zero_point != 0:
             # Sum operation in full integers resulting in large integers (INTEGERS)
-            sum_input = -q_weights.quantizer.zero_point * numpy.sum(
-                input_q_values, axis=1, keepdims=True
-            )
-
-            # Last part that has to be done in integer
-            numpy_q_out = matmul + sum_input
+            with tag(self.op_instance_name + ".matmul_inputsum"):
+                sum_input = -q_weights.quantizer.zero_point * numpy.sum(
+                    input_q_values, axis=1, keepdims=True
+                )
+
+            with tag(self.op_instance_name + ".matmul_add_inputsum"):
+                # Last part that has to be done in integer
+                numpy_q_out = matmul + sum_input
         else:
             numpy_q_out = matmul
 
+        if self.debug_value_tracker is not None:
+            # pylint: disable-next=unsubscriptable-object
+            self.debug_value_tracker[self.op_instance_name]["output"] = numpy_q_out  # type: ignore
+
         # sum_weights is a constant
         sum_weights = q_input.quantizer.zero_point * numpy.sum(
             weights_q_values, axis=0, keepdims=True
         )
 
         final_term = p * q_input.quantizer.zero_point * q_weights.quantizer.zero_point
 
@@ -234,35 +261,34 @@
             out_zp: Union[int, numpy.ndarray] = sum_weights - final_term
             if q_bias is not None:
                 # Make mypy happy
                 assert q_bias is not None
                 # Reshape the biases to broadcast them to each neuron
                 out_zp = out_zp + q_bias / (-m_matmul)
 
-            # FIXME: remove when CNP fixes the return type of cnp_conv in non-tracing mode
-            # https://github.com/zama-ai/concrete-numpy-internal/issues/1739
-            if isinstance(numpy_q_out, numpy.ndarray):
-                numpy_q_out = numpy_q_out.astype(numpy.int64)
-
             # We identify terms in the above equation to determine what
             # the scale/zero-point of the in-the-clear quantizer should be
             # to properly dequantize numpy_q_out
             return self.make_output_quant_parameters(numpy_q_out, m_matmul, out_zp)
 
+        with tag(self.op_instance_name + ".matmul_rounding"):
+            # Apply Concrete rounding (if relevant)
+            numpy_q_out = self.cnp_round(numpy_q_out, calibrate_rounding)
+
         # Quantization scales and zero points (FLOATS involved)
         # This is going to be compiled with a PBS (along with the following activation function)
         numpy_q_out = numpy_q_out.astype(numpy.float64) + final_term - sum_weights
 
         numpy_q_out = m_matmul * numpy_q_out
 
         if q_bias is not None:
             # The bias is handled as a float and will be fused
             numpy_q_out = numpy_q_out + q_bias
 
-        # Return the float values, so that CN can fuse any following float operations
+        # Return the float values, so that Concrete can fuse any following float operations
         # We also keep track of the scaling factor and zero-point, since these will be
         # applied by the following layers.
         return QuantizedArray(
             self.n_bits,
             numpy_q_out,
             value_is_float=True,
             options=self._get_output_quant_opts(),
@@ -284,17 +310,24 @@
     """
 
     _impl_for_op_named: str = "Add"
     b_sign: int = 1
 
     def q_impl(
         self,
-        *q_inputs: QuantizedArray,
+        *q_inputs: ONNXOpInputOutputType,
         **attrs,
-    ) -> QuantizedArray:
+    ) -> ONNXOpInputOutputType:
+
+        # If operating over all raw inputs, just perform the op in the clear
+        if all(isinstance(q_input, RawOpOutput) for q_input in q_inputs):
+            prepared_inputs = self._prepare_inputs_with_constants(
+                *q_inputs, calibrate=False, quantize_actual_values=False
+            )
+            return self.call_impl(*prepared_inputs, **attrs).view(RawOpOutput)
 
         # For mypy
         assert self.output_quant_params is not None
         assert self.output_quant_params.scale is not None
         assert self.output_quant_params.zero_point is not None
 
         # Optimize computation when adding constants, or tensors obtained from a unique integer
@@ -421,130 +454,167 @@
 
 
 class QuantizedIdentity(QuantizedOp):
     """Quantized Identity op."""
 
     _impl_for_op_named: str = "Identity"
 
-    def q_impl(self, *q_inputs: QuantizedArray, **attrs) -> QuantizedArray:
+    def q_impl(
+        self,
+        *q_inputs: ONNXOpInputOutputType,
+        **attrs,
+    ) -> ONNXOpInputOutputType:
         assert_true(len(q_inputs) == 1, "Identity does not work with multiple QuantizedArray")
+
+        # This op takes only encrypted inputs in the form of QuantizedArray
+        assert isinstance(q_inputs[0], QuantizedArray)
+
         self.output_quant_params = q_inputs[0].quantizer.quant_params
         return super().q_impl(*q_inputs, **attrs)
 
 
 class QuantizedReshape(QuantizedOp):
     """Quantized Reshape op."""
 
     _impl_for_op_named: str = "Reshape"
     quantize_inputs_with_model_outputs_precision = True
 
-    def q_impl(self, *q_inputs: QuantizedArray, **attrs) -> QuantizedArray:
+    def q_impl(
+        self,
+        *q_inputs: ONNXOpInputOutputType,
+        **attrs,
+    ) -> ONNXOpInputOutputType:
         """Reshape the input integer encrypted tensor.
 
         Args:
             q_inputs: an encrypted integer tensor at index 0 and one constant shape at index 1
             attrs: additional optional reshape options
 
         Returns:
             result (QuantizedArray): reshaped encrypted integer tensor
         """
 
-        # FIXME: Currently reshape quantizes the inputs, but this is unnecessary if the reshape
-        # operation could be fused into a Gemm/Add/Conv that follows it. We should reshape
-        # here only if the reshaped result is returned directly from the FHE program.
-        # See https://github.com/zama-ai/concrete-ml-internal/issues/527
         prepared_inputs = self._prepare_inputs_with_constants(
             *q_inputs, calibrate=False, quantize_actual_values=True
         )
 
+        # This op takes only encrypted inputs in the form of QuantizedArray
+        assert isinstance(q_inputs[0], QuantizedArray)
+
         newshape = prepared_inputs[1]
         assert_true(numpy.issubdtype(newshape.dtype, numpy.integer))
 
         # Return a new quantized array with the same quantization parameters
         return QuantizedArray(
             q_inputs[0].quantizer.n_bits,
             self.call_impl(prepared_inputs[0].qvalues, newshape, **attrs),
             value_is_float=False,
-            options=self._get_output_quant_opts(),
+            options=prepared_inputs[0].quantizer.quant_options,
             stats=prepared_inputs[0].quantizer.quant_stats,
             params=prepared_inputs[0].quantizer.quant_params,
         )
 
+    def can_fuse(self) -> bool:
+        """Determine if this op can be fused.
+
+        Max Pooling operation can not be fused since it must be performed over integer tensors and
+        it combines different elements of the input tensors.
+
+        Returns:
+            bool: False, this operation can not be fused as it adds different encrypted integers
+        """
+        return False
+
 
 class QuantizedConv(QuantizedMixingOp):
     """Quantized Conv op."""
 
     _impl_for_op_named: str = "Conv"
 
     def __init__(
         self,
         n_bits_output: int,
+        op_instance_name: str,
         int_input_names: Set[str] = None,
         constant_inputs: Optional[Union[Dict[str, Any], Dict[int, Any]]] = None,
         input_quant_opts: QuantizationOptions = None,
         **attrs,
     ) -> None:
         """Construct the quantized convolution operator and retrieve parameters.
 
         Args:
             n_bits_output: number of bits for the quantization of the outputs of this operator
+            op_instance_name (str): The name that should be assigned to this operation, used
+                to retrieve it later or get debugging information about this op (bitwidth, value
+                range, integer intermediary values, op-specific error messages). Usually this name
+                is the same as the ONNX operation name for which this operation is constructed.
             int_input_names: names of integer tensors that are taken as input for this operation
             constant_inputs: the weights and activations
             input_quant_opts: options for the input quantizer
             attrs: convolution options
                 dilations (Tuple[int]): dilation of the kernel. Default to 1 on all dimensions.
                 group (int): number of convolution groups. Default to 1.
                 kernel_shape (Tuple[int]): shape of the kernel. Should have 2 elements for 2d conv
                 pads (Tuple[int]): padding in ONNX format (begin, end) on each axis
                 strides (Tuple[int]): stride of the convolution on each axis
         """
 
-        super().__init__(n_bits_output, int_input_names, constant_inputs, input_quant_opts, **attrs)
+        super().__init__(
+            n_bits_output,
+            op_instance_name,
+            int_input_names,
+            constant_inputs,
+            input_quant_opts,
+            **attrs,
+        )
 
         # Get the ONNX parameters
         self.group = attrs.get("group", 1)
         self.kernel_shape = attrs.get("kernel_shape", None)
         self.pads = attrs.get("pads", tuple([0] * 2 * (len(self.kernel_shape) - 2)))
         self.dilations = attrs.get("dilations", tuple([1] * len(self.kernel_shape)))
         self.strides = attrs.get("strides", tuple([1] * len(self.kernel_shape)))
 
         # Validate the parameters
         assert_true(
-            len(self.kernel_shape) == 2, "The convolution operator currently supports only 2d"
+            len(self.kernel_shape) == 2,
+            "The convolution operator currently supports only 2d",
         )
         assert_true(
             len(self.kernel_shape) == len(self.strides),
             "The convolution operator requires the number of strides to "
             "be the same as the number of kernel dimensions",
         )
         assert_true(
             bool(numpy.all(numpy.asarray(self.dilations) == 1)),
-            "The convolution operator in Concrete Numpy does not suppport dilation",
+            "The convolution operator in Concrete does not suppport dilation",
         )
         assert_true(
             len(self.pads) == 2 * len(self.kernel_shape),
             "The convolution operator in Concrete ML requires padding to be specified as "
             " (pad_left_dim1, pad_right_dim1, pad_left_dim2, pad_right_dim2, ...), following ONNX"
             " standard",
         )
 
     def q_impl(
         self,
-        *q_inputs: QuantizedArray,
+        *q_inputs: ONNXOpInputOutputType,
+        calibrate_rounding: bool = False,
         **attrs,
-    ) -> QuantizedArray:
+    ) -> ONNXOpInputOutputType:
         """Compute the quantized convolution between two quantized tensors.
 
         Allows an optional quantized bias.
 
         Args:
             q_inputs: input tuple, contains
                 x (numpy.ndarray): input data. Shape is N x C x H x W for 2d
                 w (numpy.ndarray): weights tensor. Shape is (O x I x Kh x Kw) for 2d
                 b (numpy.ndarray, Optional): bias tensor, Shape is (O,)
+            calibrate_rounding (bool): Whether to calibrate rounding
             attrs: convolution options handled in constructor
 
         Returns:
             res (QuantizedArray): result of the quantized integer convolution
         """
 
         # For mypy
@@ -594,50 +664,59 @@
         # which in turn follows Eq.7 in https://arxiv.org/abs/1712.05877
         # to split the core computation from the zero points and scales.
 
         # Compute the first encrypted term that convolves weights and inputs
         # Force padding to 0 as padding needs to use a custom padding initializer
         # and is thus manually performed in the code above
         fake_pads = [0] * len(self.pads)
-        conv_wx = cnp_conv(
-            q_input_pad,
-            q_weights.qvalues,
-            bias=None,
-            pads=fake_pads,
-            strides=self.strides,
-            dilations=self.dilations,
-            group=self.group,
-        )
+
+        with tag(self.op_instance_name + ".conv"):
+            conv_wx = cnp_conv(
+                q_input_pad,
+                q_weights.qvalues,
+                bias=None,
+                pads=fake_pads,
+                strides=self.strides,
+                dilations=self.dilations,
+                group=self.group,
+            )
 
         # The total number of elements that are convolved by the application of a single kernel
         n_weights = numpy.prod(q_weights.qvalues.shape[1:])
 
         # If the weights have symmetric quantization, their zero point will be 0
         # The following check avoids the computation of the sum of the inputs, which may have
         # large bitwidth, in the case where it would be multiplied by zero
         if q_weights.quantizer.zero_point != 0:
             # Compute the sum of the inputs (second encrypted term)
             assert_true(
                 isinstance(q_weights.quantizer.zero_point, (int, numpy.int_)),
                 f"Zero point of weights tensor in {self.op_type} "
                 f"op {self.op_instance_name} must be integer",
             )
-            zw_conv_1x = -q_weights.quantizer.zero_point * cnp_conv(
-                q_input_pad,
-                q_weights_1,
-                bias=None,
-                pads=[0, 0, 0, 0],
-                strides=self.strides,
-                dilations=self.dilations,
-                group=self.group,
-            )
-            numpy_q_out = conv_wx + zw_conv_1x
+            with tag(self.op_instance_name + ".conv_inputsum"):
+                zw_conv_1x = -q_weights.quantizer.zero_point * cnp_conv(
+                    q_input_pad,
+                    q_weights_1,
+                    bias=None,
+                    pads=[0, 0, 0, 0],
+                    strides=self.strides,
+                    dilations=self.dilations,
+                    group=self.group,
+                )
+
+            with tag(self.op_instance_name + ".conv_add_inputsum"):
+                numpy_q_out = conv_wx + zw_conv_1x
         else:
             numpy_q_out = conv_wx
 
+        if self.debug_value_tracker is not None:
+            # pylint: disable-next=unsubscriptable-object
+            self.debug_value_tracker[self.op_instance_name]["output"] = numpy_q_out
+
         # Compute the third term, the sum of the weights which is a constant
         sum_weights = q_input.quantizer.zero_point * numpy.sum(
             q_weights.qvalues, axis=(1, 2, 3), keepdims=True
         ).transpose(1, 0, 2, 3)
 
         # Compute the forth term which is a constant
         final_term = n_weights * q_input.quantizer.zero_point * q_weights.quantizer.zero_point
@@ -661,24 +740,23 @@
             #   q_out = multisum terms involving inputs
             #   zp_out = -(multisum terms involving weights + bias / (S_x * S_w))
             out_zp: Union[int, numpy.ndarray] = sum_weights - final_term
             if q_bias is not None:
                 # Reshape the biases to broadcast them to each channel
                 out_zp = out_zp - q_bias.reshape((1, -1, 1, 1)) / m_matmul
 
-            # FIXME: remove when CNP fixes the return type of cnp_conv in non-tracing mode
-            # https://github.com/zama-ai/concrete-numpy-internal/issues/1739
-            if isinstance(numpy_q_out, numpy.ndarray):
-                numpy_q_out = numpy_q_out.astype(numpy.int64)
-
             # We identify terms in the above equation to determine what
             # the scale/zero-point of the in-the-clear quantizer should be
             # to properly dequantize numpy_q_out
             return self.make_output_quant_parameters(numpy_q_out, m_matmul, out_zp)
 
+        with tag(self.op_instance_name + ".conv_rounding"):
+            # Apply Concrete rounding (if relevant)
+            numpy_q_out = self.cnp_round(numpy_q_out, calibrate_rounding)
+
         # Now compute the whole sum (sum of the four terms)
         numpy_q_out = numpy_q_out.astype(numpy.float64) + final_term - sum_weights
 
         # Rescale from scale=scale_inputs x scale_outputs to output scale
         numpy_q_out = m_matmul * numpy_q_out
 
         if q_bias is not None:
@@ -703,32 +781,41 @@
 
     _impl_for_op_named: str = "AveragePool"
 
     # Since this op takes a single input, we can set int_input_names to a single default id
     def __init__(
         self,
         n_bits_output: int,
+        op_instance_name: str,
         int_input_names: Set[str] = None,
         constant_inputs: Optional[Union[Dict[str, Any], Dict[int, Any]]] = None,
         input_quant_opts: QuantizationOptions = None,
         **attrs,
     ) -> None:
 
-        super().__init__(n_bits_output, int_input_names, constant_inputs, input_quant_opts, **attrs)
+        super().__init__(
+            n_bits_output,
+            op_instance_name,
+            int_input_names,
+            constant_inputs,
+            input_quant_opts,
+            **attrs,
+        )
 
         # Get the ONNX parameters
         self.ceil_mode = attrs.get("ceil_mode", None)
         self.kernel_shape = attrs.get("kernel_shape", None)
         self.pads = attrs.get("pads", tuple([0] * 2 * (len(self.kernel_shape) - 2)))
         self.dilations = attrs.get("dilations", tuple([1] * len(self.kernel_shape)))
         self.strides = attrs.get("strides", tuple([1] * len(self.kernel_shape)))
 
         # Validate the parameters
         assert_true(
-            len(self.kernel_shape) == 2, "The Average Pool operator currently supports only 2d"
+            len(self.kernel_shape) == 2,
+            "The Average Pool operator currently supports only 2d",
         )
         assert_true(
             len(self.kernel_shape) == len(self.strides),
             "The Average Pool operator requires the number of strides to "
             "be the same as the number of kernel dimensions",
         )
         assert_true(
@@ -739,17 +826,18 @@
         )
 
         self.kernel: Union[numpy.ndarray, None] = None
         self.norm_const: Union[float, None] = None
 
     def q_impl(
         self,
-        *q_inputs: QuantizedArray,
+        *q_inputs: ONNXOpInputOutputType,
+        calibrate_rounding: bool = False,
         **attrs,
-    ) -> QuantizedArray:
+    ) -> ONNXOpInputOutputType:
 
         # Retrieve the quantized inputs
         prepared_inputs = self._prepare_inputs_with_constants(
             *q_inputs, calibrate=False, quantize_actual_values=True
         )
         q_input: QuantizedArray = prepared_inputs[0]
 
@@ -758,15 +846,19 @@
             (n_in_channels, n_in_channels, self.kernel_shape[0], self.kernel_shape[1]),
             dtype=numpy.int64,
         )
         for i in range(n_in_channels):
             kernel[i, i, ::] = 1
 
         norm_const = 1.0 / onnx_avgpool_compute_norm_const(
-            q_input.qvalues.shape, self.kernel_shape, self.pads, self.strides, self.ceil_mode
+            q_input.qvalues.shape,
+            self.kernel_shape,
+            self.pads,
+            self.strides,
+            self.ceil_mode,
         )
 
         # for mypy: The Quantized ops can only run on QuantizedArray that have quantization
         # parameters (i.e. were fully constructed). This should always be the case, except
         # during the UniformQuantizer initialization when the zero_point can exist as None
         assert q_input.quantizer.zero_point is not None
 
@@ -794,19 +886,28 @@
             # for output layers
             q_input_pad_ceil = numpy_onnx_pad(q_input.qvalues, pool_pads_ceil, 0, True)
 
             # Copy the PyTorch style padded input to the larger 0 padded tensor
             q_input_pad_ceil[:, :, 0 : q_input_pad.shape[2], 0 : q_input_pad.shape[3]] = q_input_pad
             q_input_pad = q_input_pad_ceil
 
-        # Remark that here, we are _not_ using Concrete-Numpy pad, since it would pad with
+        # Remark that here, we are _not_ using Concrete pad, since it would pad with
         # 0's while we want to pad with zero-point's. So, instead, he have done the padding
         # on our side, with q_input_pad
         fake_pads = [0] * len(self.pads)
-        sum_result = cnp_conv(q_input_pad, kernel, None, fake_pads, self.strides)
+        with tag(self.op_instance_name + ".avgpool"):
+            sum_result = cnp_conv(q_input_pad, kernel, None, fake_pads, self.strides)
+
+        with tag(self.op_instance_name + ".avgpool_rounding"):
+            # Apply Concrete rounding (if relevant)
+            sum_result = self.cnp_round(sum_result, calibrate_rounding)
+
+        if self.debug_value_tracker is not None:
+            # pylint: disable-next=unsubscriptable-object
+            self.debug_value_tracker[self.op_instance_name]["output"] = sum_result
 
         result = (
             sum_result.astype(numpy.float64) * norm_const - q_input.quantizer.zero_point
         ) * q_input.quantizer.scale
 
         return QuantizedArray(
             self.n_bits,
@@ -823,81 +924,95 @@
 
     _impl_for_op_named: str = "MaxPool"
 
     # Since this op takes a single input, we can set int_input_names to a single default id
     def __init__(
         self,
         n_bits_output: int,
+        op_instance_name: str,
         int_input_names: Set[str] = None,
         constant_inputs: Optional[Union[Dict[str, Any], Dict[int, Any]]] = None,
         input_quant_opts: QuantizationOptions = None,
         **attrs,
     ) -> None:
 
-        super().__init__(n_bits_output, int_input_names, constant_inputs, input_quant_opts, **attrs)
+        super().__init__(
+            n_bits_output,
+            op_instance_name,
+            int_input_names,
+            constant_inputs,
+            input_quant_opts,
+            **attrs,
+        )
 
         # Get the ONNX parameters
         self.auto_pad = attrs.get("auto_pad", "NOTSET")
         self.ceil_mode = attrs.get("ceil_mode", 0)
         self.kernel_shape = attrs.get("kernel_shape", None)
         self.storage_order = attrs.get("storage_order", 0)
         self.pads = attrs.get("pads", tuple([0] * 2 * (len(self.kernel_shape) - 2)))
         self.dilations = attrs.get("dilations", tuple([1] * len(self.kernel_shape)))
         self.strides = attrs.get("strides", tuple([1] * len(self.kernel_shape)))
 
         # Validate the parameters
-        assert_true(
-            self.ceil_mode == 0, "Only ceil_mode = 0 is supported by Concrete Numpy for now"
-        )
+        assert_true(self.ceil_mode == 0, "Only ceil_mode = 0 is supported by Concrete for now")
 
         # Validate the parameters
-        assert_true(len(self.kernel_shape) == 2, "The Max Pool operator currently supports only 2d")
+        assert_true(
+            len(self.kernel_shape) == 2,
+            "The Max Pool operator currently supports only 2d",
+        )
         assert_true(
             len(self.kernel_shape) == len(self.strides),
             "The Max Pool operator requires the number of strides to "
             "be the same as the number of kernel dimensions",
         )
         assert_true(
             len(self.pads) == 2 * len(self.kernel_shape),
             "The Max Pool operator in Concrete ML requires padding to be specified as "
             " (pad_left_dim1, pad_right_dim1, pad_left_dim2, pad_right_dim2, ...), following ONNX"
             " standard",
         )
 
     def q_impl(
         self,
-        *q_inputs: QuantizedArray,
+        *q_inputs: ONNXOpInputOutputType,
         **attrs,
-    ) -> QuantizedArray:
+    ) -> ONNXOpInputOutputType:
 
         # Retrieve the quantized inputs
         prepared_inputs = self._prepare_inputs_with_constants(
             *q_inputs, calibrate=False, quantize_actual_values=True
         )
         q_input: QuantizedArray = prepared_inputs[0]
 
         # for mypy: The Quantized ops can only run on QuantizedArray that have quantization
         # parameters (i.e. were fully constructed). This should always be the case, except
         # during the UniformQuantizer initialization when the zero_point can exist as None
         assert q_input.quantizer.zero_point is not None
 
         assert_true(
-            self.ceil_mode == 0, "Only ceil_mode = 0 is supported by Concrete Numpy for now"
+            self.ceil_mode == 0,
+            "Only ceil_mode = 0 is supported by Concrete for now",
         )
 
         # Simple padding for PyTorch style
         pool_pads = compute_onnx_pool_padding(
-            q_input.qvalues.shape, self.kernel_shape, self.pads, self.strides, self.ceil_mode
+            q_input.qvalues.shape,
+            self.kernel_shape,
+            self.pads,
+            self.strides,
+            self.ceil_mode,
         )
 
         q_input_pad = numpy_onnx_pad(
             q_input.qvalues, pool_pads, q_input.quantizer.zero_point, int_only=True
         )
 
-        # Remark that here, we are _not_ using Concrete-Numpy pad, since it would pad with
+        # Remark that here, we are _not_ using Concrete pad, since it would pad with
         # 0's while we want to pad with zero-point's. So, instead, he have done the padding
         # on our side, with q_input_pad
         fake_pads = [0] * len(self.pads)
         sum_result = cnp_maxpool(
             q_input_pad,
             kernel_shape=self.kernel_shape,
             strides=self.strides,
@@ -937,31 +1052,76 @@
     """Quantized Padding op."""
 
     _impl_for_op_named: str = "Pad"
 
     def __init__(
         self,
         n_bits_output: int,
+        op_instance_name: str,
         int_input_names: Set[str] = None,
         constant_inputs: Optional[Union[Dict[str, Any], Dict[int, Any]]] = None,
         input_quant_opts: QuantizationOptions = None,
         **attrs,
     ) -> None:
 
-        super().__init__(n_bits_output, int_input_names, constant_inputs, input_quant_opts, **attrs)
+        super().__init__(
+            n_bits_output,
+            op_instance_name,
+            int_input_names,
+            constant_inputs,
+            input_quant_opts,
+            **attrs,
+        )
 
         # Get the ONNX parameters
         self.mode = attrs.get("mode", None)
         assert_true(
-            self.mode == "constant", "Padding operator only supports padding with a constant"
+            self.mode == "constant",
+            "Padding operator only supports padding with a constant",
+        )
+
+    def q_impl(
+        self,
+        *q_inputs: ONNXOpInputOutputType,
+        calibrate_rounding: bool = False,  # pylint: disable=unused-argument
+        **attrs,
+    ) -> ONNXOpInputOutputType:
+        # Retrieve the quantized inputs
+        prepared_inputs = self._prepare_inputs_with_constants(
+            *q_inputs, calibrate=False, quantize_actual_values=True
         )
+        q_input: QuantizedArray = prepared_inputs[0]
+        pads = prepared_inputs[1]
 
         assert_true(
-            self.constant_inputs is None or bool(numpy.all(self.constant_inputs[1] == 0)),
-            "Padding operator supported only with all pads at zero",
+            all(pads[i] == 0 and pads[4 + i] == 0 for i in range(0, 2)),
+            "Concrete ML only supports padding along the width & height dimensions, padding"
+            f" requested was {pads}",
+        )
+
+        assert_true(pads.size % 2 == 0)  # must be a multiple of 2
+        assert_true(pads.size in [4, 8], "Only supporting pads of size 4 or 8.")
+        if pads.size == 8:
+            pads = numpy.asarray([pads[2], pads[3], pads[6], pads[7]])
+
+        assert_true(pads.size == 4, "Not currently supporting padding of 3D tensors")
+
+        pad_value = 0 if prepared_inputs[2] is None else prepared_inputs[2]
+        assert_true(pad_value == 0, "Concrete ML only supports padding with constant zero values")
+
+        assert q_input.quantizer.zero_point is not None
+        q_input_pad = numpy_onnx_pad(q_input.qvalues, pads, q_input.quantizer.zero_point, True)
+
+        return QuantizedArray(
+            q_input.quantizer.n_bits,
+            q_input_pad,
+            value_is_float=False,
+            options=q_input.quantizer.quant_options,
+            stats=q_input.quantizer.quant_stats,
+            params=q_input.quantizer.quant_params,
         )
 
     def can_fuse(self) -> bool:
         """Determine if this op can be fused.
 
         Pad operation cannot be fused since it must be performed over integer tensors.
 
@@ -979,20 +1139,28 @@
 
     _impl_for_op_named: str = "Where"
 
     # This op takes a single variable input, so we can set int_input_names to a default id
     def __init__(
         self,
         n_bits_output: int,
+        op_instance_name: str,
         int_input_names: Set[str] = None,
         constant_inputs: Optional[Union[Dict[str, Any], Dict[int, Any]]] = None,
         input_quant_opts: QuantizationOptions = None,
         **attrs,
     ) -> None:
-        super().__init__(n_bits_output, int_input_names, constant_inputs, input_quant_opts, **attrs)
+        super().__init__(
+            n_bits_output,
+            op_instance_name,
+            int_input_names,
+            constant_inputs,
+            input_quant_opts,
+            **attrs,
+        )
 
         # Remember that there are examples of where with more than 1 variable which are going to be
         # well managed, thanks to fusing:
         # Act(x) = (x < 3) ? x + 42 : x ^ 42 would perfectly fuse
         # But for this kind of example, we have int_input_names = {'x'} since they all depend only
         # on x
         assert_true(
@@ -1020,20 +1188,28 @@
 
     _impl_for_op_named: str = "Greater"
 
     # Since this op takes a single variable input, we can set int_input_names to a single default id
     def __init__(
         self,
         n_bits_output: int,
+        op_instance_name: str,
         int_input_names: Set[str] = None,
         constant_inputs: Optional[Union[Dict[str, Any], Dict[int, Any]]] = None,
         input_quant_opts: QuantizationOptions = None,
         **attrs,
     ) -> None:
-        super().__init__(n_bits_output, int_input_names, constant_inputs, input_quant_opts, **attrs)
+        super().__init__(
+            n_bits_output,
+            op_instance_name,
+            int_input_names,
+            constant_inputs,
+            input_quant_opts,
+            **attrs,
+        )
 
         # We do not support testing a > b where a,b are encrypted
         # only comparing to a constant is supported
         assert_true(constant_inputs is not None and len(constant_inputs) >= 1)
 
 
 class QuantizedGreaterOrEqual(QuantizedOp):
@@ -1044,20 +1220,28 @@
 
     _impl_for_op_named: str = "GreaterOrEqual"
 
     # Since this op takes a single variable input, we can set int_input_names to a single default id
     def __init__(
         self,
         n_bits_output: int,
+        op_instance_name: str,
         int_input_names: Set[str] = None,
         constant_inputs: Optional[Union[Dict[str, Any], Dict[int, Any]]] = None,
         input_quant_opts: QuantizationOptions = None,
         **attrs,
     ) -> None:
-        super().__init__(n_bits_output, int_input_names, constant_inputs, input_quant_opts, **attrs)
+        super().__init__(
+            n_bits_output,
+            op_instance_name,
+            int_input_names,
+            constant_inputs,
+            input_quant_opts,
+            **attrs,
+        )
 
         # We do not support testing a >= b where a,b are encrypted
         # only comparing to a constant is supported
         assert_true(constant_inputs is not None and len(constant_inputs) >= 1)
 
 
 class QuantizedLess(QuantizedOp):
@@ -1068,20 +1252,28 @@
 
     _impl_for_op_named: str = "Less"
 
     # Since this op takes a single variable input, we can set int_input_names to a single default id
     def __init__(
         self,
         n_bits_output: int,
+        op_instance_name: str,
         int_input_names: Set[str] = None,
         constant_inputs: Optional[Union[Dict[str, Any], Dict[int, Any]]] = None,
         input_quant_opts: QuantizationOptions = None,
         **attrs,
     ) -> None:
-        super().__init__(n_bits_output, int_input_names, constant_inputs, input_quant_opts, **attrs)
+        super().__init__(
+            n_bits_output,
+            op_instance_name,
+            int_input_names,
+            constant_inputs,
+            input_quant_opts,
+            **attrs,
+        )
 
         # We do not support testing a < b where a,b are encrypted
         # only comparing to a constant is supported
         assert_true(constant_inputs is not None and len(constant_inputs) >= 1)
 
 
 class QuantizedLessOrEqual(QuantizedOp):
@@ -1092,20 +1284,28 @@
 
     _impl_for_op_named: str = "LessOrEqual"
 
     # Since this op takes a single variable input, we can set int_input_names to a single default id
     def __init__(
         self,
         n_bits_output: int,
+        op_instance_name: str,
         int_input_names: Set[str] = None,
         constant_inputs: Optional[Union[Dict[str, Any], Dict[int, Any]]] = None,
         input_quant_opts: QuantizationOptions = None,
         **attrs,
     ) -> None:
-        super().__init__(n_bits_output, int_input_names, constant_inputs, input_quant_opts, **attrs)
+        super().__init__(
+            n_bits_output,
+            op_instance_name,
+            int_input_names,
+            constant_inputs,
+            input_quant_opts,
+            **attrs,
+        )
 
         # We do not support testing a <= b where a,b are encrypted
         # only comparing to a constant is supported
         assert_true(constant_inputs is not None and len(constant_inputs) >= 1)
 
 
 class QuantizedOr(QuantizedOpUnivariateOfEncrypted, QuantizedOp):
@@ -1156,33 +1356,36 @@
 
 class QuantizedFlatten(QuantizedOp):
     """Quantized flatten for encrypted inputs."""
 
     _impl_for_op_named: str = "Flatten"
     quantize_inputs_with_model_outputs_precision = True
 
-    def q_impl(self, *q_inputs: QuantizedArray, **attrs) -> QuantizedArray:
+    def q_impl(
+        self,
+        *q_inputs: ONNXOpInputOutputType,
+        **attrs,
+    ) -> ONNXOpInputOutputType:
         """Flatten the input integer encrypted tensor.
 
         Args:
             q_inputs: an encrypted integer tensor at index 0
             attrs: contains axis attribute
 
         Returns:
             result (QuantizedArray): reshaped encrypted integer tensor
         """
 
-        # FIXME: Currently reshape quantizes the inputs, but this is unnecessary if the reshape
-        # operation could be fused into a Gemm/Add/Conv that follows it. We should reshape
-        # here only if the reshaped result is returned directly from the FHE program.
-        # See https://github.com/zama-ai/concrete-ml-internal/issues/527
         prepared_inputs = self._prepare_inputs_with_constants(
             *q_inputs, calibrate=False, quantize_actual_values=True
         )
 
+        # This op takes only encrypted inputs in the form of QuantizedArray
+        assert isinstance(q_inputs[0], QuantizedArray)
+
         assert_true(len(q_inputs) == 1, "Flatten operator only takes a single input")
 
         axis = attrs["axis"]
         newshape: Sequence[SupportsIndex]
         newshape = (
             *q_inputs[0].qvalues.shape[0:axis],
             numpy.prod(q_inputs[0].qvalues.shape[axis:]),
@@ -1214,23 +1417,28 @@
     """ReduceSum with encrypted input."""
 
     _impl_for_op_named: str = "ReduceSum"
 
     def __init__(
         self,
         n_bits_output: int,
+        op_instance_name: str,
         int_input_names: Set[str] = None,
         constant_inputs: Optional[Union[Dict[str, Any], Dict[int, Any]]] = None,
         input_quant_opts: Optional[QuantizationOptions] = None,
         **attrs,
     ) -> None:
         """Construct the quantized ReduceSum operator and retrieve parameters.
 
         Args:
             n_bits_output (int): Number of bits for the operator's quantization of outputs.
+            op_instance_name (str): The name that should be assigned to this operation, used
+                to retrieve it later or get debugging information about this op (bitwidth, value
+                range, integer intermediary values, op-specific error messages). Usually this name
+                is the same as the ONNX operation name for which this operation is constructed.
             int_input_names (Optional[Set[str]]): Names of input integer tensors. Default to None.
             constant_inputs (Optional[Dict]): Input constant tensor.
                 axes (Optional[numpy.ndarray]): Array of integers along which to reduce.
                     The default is to reduce over all the dimensions of the input tensor if
                     'noop_with_empty_axes' is false, else act as an Identity op when
                     'noop_with_empty_axes' is true. Accepted range is [-r, r-1] where
                     r = rank(data). Default to None.
@@ -1240,15 +1448,22 @@
                 keepdims (int): Keep the reduced dimension or not, 1 means keeping the
                     input dimension, 0 will reduce it along the given axis. Default to 1.
                 noop_with_empty_axes (int): Defines behavior if 'axes' is empty or set to None.
                     Default behavior with 0 is to reduce all axes. When axes is empty and this
                     attribute is set to true 1, input tensor will not be reduced, and the output
                     tensor would be equivalent to input tensor. Default to 0.
         """
-        super().__init__(n_bits_output, int_input_names, constant_inputs, input_quant_opts, **attrs)
+        super().__init__(
+            n_bits_output,
+            op_instance_name,
+            int_input_names,
+            constant_inputs,
+            input_quant_opts,
+            **attrs,
+        )
 
         # Retrieve and set the ONNX parameters
         # Numpy's keepdims parameter is a boolean while ONNX's one is an int (0 or 1). Even though
         # Python handles them equivalently, we need to manually convert it as mypy doesn't accept
         # this type difference
         self.keepdims = bool(attrs.get("keepdims", 1))
         self.noop_with_empty_axes = attrs.get("noop_with_empty_axes", 0)
@@ -1273,15 +1488,19 @@
         )
 
         self.output_quant_params = quantized_samples.quantizer.quant_params
         self.output_quant_stats = quantized_samples.quantizer.quant_stats
 
         return quantized_samples.values
 
-    def q_impl(self, *q_inputs: QuantizedArray, **attrs) -> QuantizedArray:
+    def q_impl(
+        self,
+        *q_inputs: ONNXOpInputOutputType,
+        **attrs,
+    ) -> ONNXOpInputOutputType:
         """Sum the encrypted tensor's values along the given axes.
 
         Args:
             q_inputs (QuantizedArray): An encrypted integer tensor at index 0.
             attrs (Dict): Options are handled in constructor.
 
         Returns:
@@ -1326,15 +1545,15 @@
             params=self.output_quant_params,
         )
 
         return sum_qarray
 
     def _prepare_inputs_with_constants(
         self,
-        *inputs: Union[QuantizedArray, numpy.ndarray],
+        *inputs: ONNXOpInputOutputType,
         calibrate: bool,
         quantize_actual_values: bool,
     ):
         """Retrieve all the inputs of an operator in the computational graph.
 
         This helper method will prepare a list of inputs to an operator. Inputs can be variables,
         i.e. encrypted tensors, or constants (in the clear). Inputs to an operator are set-up in
@@ -1343,15 +1562,15 @@
         Usually the input list is populated with QuantizedArrays. Operators that require the
         original float (operators that only produce or contribute to TLUs) values will just read
         out the .values of  these quantized arrays. Operators that do matrix multiplication will
         read out the quantized integer values of the arrays.  The method can be called during
         calibration, in which case the variable inputs are just float numpy tensors.
 
         Args:
-             *inputs (Union[QuantizedArray, numpy.ndarray]): A list of all variable inputs
+             *inputs (ONNXOpInputOutputType): A list of all variable inputs
             calibrate (bool): A flag specifying if the method is called during calibration
             quantize_actual_values (bool): If called by a quantized operator that does matrix
                 multiplication between encrypted and clear values, this method will apply
                 the quantization computation to the input, which will be fused in a (potentially
                 larger) TLU, with preceding floating point computations
 
         Returns:
@@ -1408,48 +1627,60 @@
     _impl_for_op_named: str = "Not"
 
 
 class QuantizedBrevitasQuant(QuantizedOp):
     """Brevitas uniform quantization with encrypted input."""
 
     _impl_for_op_named: str = "onnx.brevitas.Quant"
-    # FIXME: Note that this should be reset when the correctness test that finds
+    # Note that this should be reset when the correctness test that finds
     # all mismatches between CML and Brevitas is fixed
-    # https://github.com/zama-ai/concrete-ml-internal/issues/2373
+    # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/2373
     quantize_inputs_with_model_outputs_precision = True
     output_quant_opts: QuantizationOptions
 
     def __init__(
         self,
         n_bits_output: int,
+        op_instance_name: str,
         int_input_names: Set[str] = None,
         constant_inputs: Optional[Union[Dict[str, Any], Dict[int, Any]]] = None,
         input_quant_opts: Optional[QuantizationOptions] = None,
         **attrs,
     ) -> None:
         """Construct the Brevitas quantization operator.
 
         Args:
             n_bits_output (int): Number of bits for the operator's quantization of outputs.
                 Not used, will be overridden by the bit_width in ONNX
+            op_instance_name (str): The name that should be assigned to this operation, used
+                to retrieve it later or get debugging information about this op (bitwidth, value
+                range, integer intermediary values, op-specific error messages). Usually this name
+                is the same as the ONNX operation name for which this operation is constructed.
             int_input_names (Optional[Set[str]]): Names of input integer tensors. Default to None.
             constant_inputs (Optional[Dict]): Input constant tensor.
                 scale (float): Quantizer scale
                 zero_point (float): Quantizer zero-point
                 bit_width (int): Number of bits of the integer representation
             input_quant_opts (Optional[QuantizationOptions]): Options for the input quantizer.
                 Default to None.
             attrs (dict):
                 rounding_mode (str): Rounding mode (default and only accepted option is "ROUND")
                 signed (int): Whether this op quantizes to signed integers (default 1),
                 narrow (int): Whether this op quantizes to a narrow range of integers
                     e.g. [-2**n_bits-1 .. 2**n_bits-1] (default 0),
         """
 
-        super().__init__(n_bits_output, int_input_names, constant_inputs, input_quant_opts, **attrs)
+        super().__init__(
+            n_bits_output,
+            op_instance_name,
+            int_input_names,
+            constant_inputs,
+            input_quant_opts,
+            **attrs,
+        )
 
         def check_float(v, err_msg):
             assert_true(
                 isinstance(v, float)
                 or (isinstance(v, numpy.ndarray) and numpy.issubdtype(v.dtype, numpy.floating)),
                 err_msg,
             )
@@ -1520,53 +1751,60 @@
 
         result = super().calibrate(*inputs)
 
         # Override the output quantization params with
         # those stored in the ONNX model. This allows the quantized module to
         # pass these parameters to the module's input quantizer
 
-        # for mypy: this is set by the base class calibration
-        assert self.output_quant_params is not None
-
-        self.output_quant_params = UniformQuantizationParameters()
-        self.output_quant_params.scale = numpy.float64(self.constant_inputs[1])
-        self.output_quant_params.zero_point = int(self.constant_inputs[2])
-
         n_bits = int(self.constant_inputs[3])
-        self.output_quant_params.offset = 2 ** (n_bits - 1) if self.is_signed else 0
+
+        self.output_quant_params = UniformQuantizationParameters(
+            scale=numpy.float64(self.constant_inputs[1]),
+            zero_point=int(self.constant_inputs[2]),
+            offset=2 ** (n_bits - 1) if self.is_signed else 0,
+        )
 
         return result
 
-    def q_impl(self, *q_inputs: QuantizedArray, **attrs) -> QuantizedArray:
+    def q_impl(
+        self,
+        *q_inputs: ONNXOpInputOutputType,
+        **attrs,
+    ) -> ONNXOpInputOutputType:
         """Quantize values.
 
         Args:
-            q_inputs: an encrypted integer tensor at index 0 and one constant shape at index 1
-            attrs: additional optional reshape options
+            q_inputs: an encrypted integer tensor at index 0,
+                      scale, zero_point, n_bits at indices 1,2,3
+            attrs: additional optional attributes
 
         Returns:
             result (QuantizedArray): reshaped encrypted integer tensor
         """
 
         prepared_inputs = self._prepare_inputs_with_constants(
             *q_inputs, calibrate=False, quantize_actual_values=False
         )
 
+        # This op takes only encrypted inputs in the form of QuantizedArray
+        assert isinstance(q_inputs[0], QuantizedArray)
+
         # Impose the number of bits that this op quantizes its inputs, to the value that
         # was provided by Brevitas. This number of bits is normally
         # different from the op's n_bits. The op will usually have an output number of bits
         # that is suitable for network output, as the op could be the last op in the graph
 
         # Thus, we enforce the QAT number of bits on this op's output
         n_bits = int(prepared_inputs[3])
 
         assert len(q_inputs) >= 1
 
         assert_true(
-            self.output_quant_params is not None, "You need to calibrate this op before using it"
+            self.output_quant_params is not None,
+            "You need to calibrate this op before using it",
         )
 
         # For mypy
         assert self.output_quant_params is not None
         assert self.output_quant_params.scale is not None
         assert self.output_quant_params.zero_point is not None
 
@@ -1591,50 +1829,64 @@
         )
         return res
 
 
 class QuantizedTranspose(QuantizedOp):
     """Transpose operator for quantized inputs.
 
-    This operator performs quantization, transposes the encrypted data, then
-    dequantizes again.
+    This operator performs quantization and transposes the encrypted data.
+    When the inputs are pre-computed QAT the input is only quantized if needed.
     """
 
     _impl_for_op_named: str = "Transpose"
     quantize_inputs_with_model_outputs_precision = True
 
-    def q_impl(self, *q_inputs: QuantizedArray, **attrs) -> QuantizedArray:
-        """Reshape the input integer encrypted tensor.
+    def q_impl(
+        self,
+        *q_inputs: ONNXOpInputOutputType,
+        **attrs,
+    ) -> ONNXOpInputOutputType:
+        """Transpose the input integer encrypted tensor.
 
         Args:
             q_inputs: an encrypted integer tensor at index 0 and one constant shape at index 1
             attrs: additional optional reshape options
 
         Returns:
-            result (QuantizedArray): reshaped encrypted integer tensor
+            result (QuantizedArray): transposed encrypted integer tensor
         """
 
-        # FIXME: Currently Transpose quantizes the inputs, but this is unnecessary if the reshape
-        # operation could be fused into a Gemm/Add/Conv that follows it. We should transpose
-        # here only if the transpose result is returned directly from the FHE program.
-        # See https://github.com/zama-ai/concrete-ml-internal/issues/527
         prepared_inputs = self._prepare_inputs_with_constants(
             *q_inputs, calibrate=False, quantize_actual_values=True
         )
 
+        # This op takes only encrypted inputs in the form of QuantizedArray
+        assert isinstance(q_inputs[0], QuantizedArray)
+
         # Return a new quantized array with the same quantization parameters
         return QuantizedArray(
             q_inputs[0].quantizer.n_bits,
             self.call_impl(prepared_inputs[0].qvalues, **attrs),
             value_is_float=False,
-            options=self._get_output_quant_opts(),
+            options=prepared_inputs[0].quantizer.quant_options,
             stats=prepared_inputs[0].quantizer.quant_stats,
             params=prepared_inputs[0].quantizer.quant_params,
         )
 
+    def can_fuse(self) -> bool:
+        """Determine if this op can be fused.
+
+        Transpose can not be fused since it must be performed over integer tensors as
+        it moves around different elements of these input tensors.
+
+        Returns:
+            bool: False, this operation can not be fused as it copies encrypted integers
+        """
+        return False
+
 
 class QuantizedFloor(QuantizedOp):
     """Quantized Floor op."""
 
     _impl_for_op_named: str = "Floor"
 
 
@@ -1664,84 +1916,300 @@
 
 class QuantizedUnsqueeze(QuantizedOp):
     """Unsqueeze operator."""
 
     _impl_for_op_named: str = "Unsqueeze"
     quantize_inputs_with_model_outputs_precision = True
 
-    def q_impl(self, *q_inputs: QuantizedArray, **attrs) -> QuantizedArray:
+    def q_impl(
+        self,
+        *q_inputs: ONNXOpInputOutputType,
+        **attrs,
+    ) -> ONNXOpInputOutputType:
         """Unsqueeze the input tensors on a given axis.
 
         Args:
-            q_inputs: an encrypted integer tensor
+            q_inputs: an encrypted integer tensor at index 0, axes at index 1
             attrs: additional optional unsqueeze options
 
         Returns:
             result (QuantizedArray): unsqueezed encrypted integer tensor
         """
 
-        # FIXME: Currently Unsqueeze quantizes the inputs, but this is unnecessary if the reshape
-        # operation could be fused into a Gemm/Add/Conv that follows it. We should concatenate
-        # here only if the concatenated result is returned directly from the FHE program.
-        # See https://github.com/zama-ai/concrete-ml-internal/issues/527
         prepared_inputs = self._prepare_inputs_with_constants(
             *q_inputs, calibrate=False, quantize_actual_values=True
         )
 
+        # This op takes only encrypted inputs in the form of QuantizedArray
+        assert isinstance(q_inputs[0], QuantizedArray)
+
         axes = prepared_inputs[1]
-        assert_true(isinstance(axes, list))
 
         # Return a new quantized array with the same quantization parameters
         return QuantizedArray(
             q_inputs[0].quantizer.n_bits,
             self.call_impl(prepared_inputs[0].qvalues, axes, **attrs),
             value_is_float=False,
             options=self._get_output_quant_opts(),
             stats=prepared_inputs[0].quantizer.quant_stats,
             params=prepared_inputs[0].quantizer.quant_params,
         )
 
+    def can_fuse(self) -> bool:
+        """Determine if this op can be fused.
+
+        Unsqueeze can not be fused since it must be performed over integer tensors as
+        it reshapes an encrypted tensor.
+
+        Returns:
+            bool: False, this operation can not be fused as it operates on encrypted tensors
+        """
+        return False
+
 
 class QuantizedConcat(QuantizedOp):
     """Concatenate operator."""
 
     _impl_for_op_named: str = "Concat"
     quantize_inputs_with_model_outputs_precision = True
 
-    def q_impl(self, *q_inputs: QuantizedArray, **attrs) -> QuantizedArray:
-        """Concatenate the input tensors on a giver axis.
+    def q_impl(
+        self,
+        *q_inputs: ONNXOpInputOutputType,
+        **attrs,
+    ) -> ONNXOpInputOutputType:
+        """Concatenate the input tensors on a given axis.
 
         Args:
             q_inputs: an encrypted integer tensor
             attrs: additional optional concatenate options
 
         Returns:
             result (QuantizedArray): concatenated encrypted integer tensor
         """
 
-        # FIXME: Currently Concatenate quantizes the inputs, but this is unnecessary if the reshape
-        # operation could be fused into a Gemm/Add/Conv that follows it. We should concatenate
-        # here only if the concatenated result is returned directly from the FHE program.
-        # See https://github.com/zama-ai/concrete-ml-internal/issues/527
         prepared_inputs = self._prepare_inputs_with_constants(
             *q_inputs, calibrate=False, quantize_actual_values=True
         )
 
+        # This op takes only encrypted inputs in the form of QuantizedArray
+        assert isinstance(q_inputs[0], QuantizedArray)
+
         # The input tensors must have the same quantization parameters to be concatenated.
         scales = [x.quantizer.scale for x in prepared_inputs]
         zero_points = [x.quantizer.zero_point for x in prepared_inputs]
         assert_true(
             all(x == scales[0] for x in scales) and all(x == zero_points[0] for x in zero_points),
             "All inputs must have the same scale and zero_point to be concatenated.",
         )
+        assert_true(
+            all(
+                prep_input.quantizer.quant_options.is_equal(
+                    prepared_inputs[0].quantizer.quant_options
+                )
+                for prep_input in prepared_inputs[1:]
+            )
+        )
 
         tensors_to_concat = [prepared_input.qvalues for prepared_input in prepared_inputs]
 
         # Return a new quantized array with the same quantization parameters
         return QuantizedArray(
             q_inputs[0].quantizer.n_bits,
             self.call_impl(*tensors_to_concat, **attrs),
             value_is_float=False,
+            options=prepared_inputs[0].quantizer.quant_options,
+            stats=prepared_inputs[0].quantizer.quant_stats,
+            params=prepared_inputs[0].quantizer.quant_params,
+        )
+
+    def can_fuse(self) -> bool:
+        """Determine if this op can be fused.
+
+        Concatenation can not be fused since it must be performed over integer tensors as
+        it copies encrypted integers from one tensor to another.
+
+        Returns:
+            bool: False, this operation can not be fused as it copies encrypted integers
+        """
+        return False
+
+
+class QuantizedSqueeze(QuantizedOp):
+    """Squeeze operator."""
+
+    _impl_for_op_named: str = "Squeeze"
+    quantize_inputs_with_model_outputs_precision = True
+
+    def q_impl(
+        self,
+        *q_inputs: ONNXOpInputOutputType,
+        **attrs,
+    ) -> ONNXOpInputOutputType:
+        """Squeeze the input tensors on a given axis.
+
+        Args:
+            q_inputs: an encrypted integer tensor at index 0, axes at index 1
+            attrs: additional optional squeeze options
+
+        Returns:
+            result (QuantizedArray): squeezed encrypted integer tensor
+        """
+
+        prepared_inputs = self._prepare_inputs_with_constants(
+            *q_inputs, calibrate=False, quantize_actual_values=True
+        )
+
+        # This op takes only encrypted inputs in the form of QuantizedArray
+        assert isinstance(q_inputs[0], QuantizedArray)
+
+        axes = prepared_inputs[1]
+
+        # Return a new quantized array with the same quantization parameters
+        return QuantizedArray(
+            q_inputs[0].quantizer.n_bits,
+            self.call_impl(prepared_inputs[0].qvalues, axes, **attrs),
+            value_is_float=False,
             options=self._get_output_quant_opts(),
             stats=prepared_inputs[0].quantizer.quant_stats,
             params=prepared_inputs[0].quantizer.quant_params,
         )
+
+    def can_fuse(self) -> bool:
+        """Determine if this op can be fused.
+
+        Squeeze can not be fused since it must be performed over integer tensors as
+        it reshapes encrypted tensors.
+
+        Returns:
+            bool: False, this operation can not be fused as it reshapes encrypted tensors
+        """
+        return False
+
+
+class ONNXShape(QuantizedOp):
+    """Shape operator."""
+
+    _impl_for_op_named: str = "Shape"
+
+    def q_impl(
+        self,
+        *q_inputs: ONNXOpInputOutputType,
+        **attrs,
+    ) -> ONNXOpInputOutputType:
+        # This op takes only encrypted inputs in the form of QuantizedArray
+        assert isinstance(q_inputs[0], QuantizedArray)
+
+        return numpy.asarray(q_inputs[0].qvalues.shape, numpy.int64).view(RawOpOutput)
+
+    def can_fuse(self) -> bool:
+        """Determine if this op can be fused.
+
+        This operation returns the shape of the tensor and thus can not be fused into a
+        univariate TLU.
+
+        Returns:
+            bool: False, this operation can not be fused
+        """
+        return False
+
+
+class ONNXConstantOfShape(QuantizedOp):
+    """ConstantOfShape operator."""
+
+    _impl_for_op_named: str = "ConstantOfShape"
+
+    def can_fuse(self) -> bool:
+        """Determine if this op can be fused.
+
+        This operation returns a new encrypted tensor and thus can
+        not be fused.
+
+        Returns:
+            bool: False, this operation can not be fused
+        """
+        return False
+
+
+class ONNXGather(QuantizedOp):
+    """Gather operator.
+
+    Returns values at requested indices from the input tensor.
+    """
+
+    _impl_for_op_named: str = "Gather"
+
+    def q_impl(
+        self,
+        *q_inputs: ONNXOpInputOutputType,
+        **attrs,
+    ) -> ONNXOpInputOutputType:
+        prepared_inputs = self._prepare_inputs_with_constants(
+            *q_inputs, calibrate=False, quantize_actual_values=True
+        )
+
+        # The first parameter can be either an encrypted tensor or a shape (int64 array)
+        if isinstance(prepared_inputs[0], QuantizedArray):
+            inputs = (prepared_inputs[0].qvalues, *prepared_inputs[1:])
+            return QuantizedArray(
+                prepared_inputs[0].quantizer.n_bits,
+                self.call_impl(*inputs, **attrs),
+                value_is_float=False,
+                options=prepared_inputs[0].quantizer.quant_options,
+                stats=prepared_inputs[0].quantizer.quant_stats,
+                params=prepared_inputs[0].quantizer.quant_params,
+            )
+
+        assert_true(isinstance(prepared_inputs[0], numpy.ndarray))
+        return self.call_impl(*prepared_inputs, **attrs)
+
+    def can_fuse(self) -> bool:
+        """Determine if this op can be fused.
+
+        This operation returns values from a tensor and thus can not be fused into a
+        univariate TLU.
+
+        Returns:
+            bool: False, this operation can not be fused
+        """
+        return False
+
+
+class ONNXSlice(QuantizedOp):
+    """Slice operator."""
+
+    _impl_for_op_named: str = "Slice"
+
+    def q_impl(
+        self,
+        *q_inputs: ONNXOpInputOutputType,
+        **attrs,
+    ) -> ONNXOpInputOutputType:
+        prepared_inputs = self._prepare_inputs_with_constants(
+            *q_inputs, calibrate=False, quantize_actual_values=True
+        )
+
+        assert_true(
+            isinstance(prepared_inputs[0], QuantizedArray),
+            "Slice currently only supports QuantizedArray inputs (encrypted inputs)",
+        )
+
+        inputs = (prepared_inputs[0].qvalues, *prepared_inputs[1:])
+        return QuantizedArray(
+            prepared_inputs[0].quantizer.n_bits,
+            self.call_impl(*inputs, **attrs),
+            value_is_float=False,
+            options=prepared_inputs[0].quantizer.quant_options,
+            stats=prepared_inputs[0].quantizer.quant_stats,
+            params=prepared_inputs[0].quantizer.quant_params,
+        )
+
+    def can_fuse(self) -> bool:
+        """Determine if this op can be fused.
+
+        This operation returns values from a tensor and thus can not be fused into a
+        univariate TLU.
+
+        Returns:
+            bool: False, this operation can not be fused
+        """
+        return False
```

## concrete/ml/quantization/quantizers.py

```diff
@@ -1,15 +1,19 @@
 """Quantization utilities for a numpy array/tensor."""
+# pylint: disable=too-many-lines
+from __future__ import annotations
 
+import json
 from copy import deepcopy
-from typing import Optional, Union, get_type_hints
+from typing import IO, Any, Dict, Optional, Union, get_type_hints
 
 import numpy
 
 from ..common.debugging import assert_true
+from ..common.serialization.encoder import CustomEncoder
 
 STABILITY_CONST = 10**-6
 
 
 def fill_from_kwargs(obj, klass, **kwargs):
     """Fill a parameter set structure from kwargs parameters.
 
@@ -92,26 +96,107 @@
     is_narrow: bool = False
 
     # Determines whether the values handled by the quantizer were produced by a custom
     # quantization layer that has pre-computed scale and zero-point (i.e. ONNX brevitas quant layer)
     is_precomputed_qat: bool = False
 
     def __init__(
-        self, n_bits, is_signed: bool = False, is_symmetric: bool = False, is_qat: bool = False
-    ) -> None:
+        self, n_bits: int, is_signed: bool = False, is_symmetric: bool = False, is_qat: bool = False
+    ):
         self.n_bits = n_bits
         self.is_signed = is_signed
         self.is_symmetric = is_symmetric
         self.is_qat = is_qat
 
         # QAT quantization is not symmetric
-        assert_true(not self.is_qat or (self.is_qat and not self.is_symmetric))
+        assert_true(not self.is_qat or not self.is_symmetric)
 
         # Symmetric quantization is signed
-        assert_true(not self.is_symmetric or (self.is_signed and self.is_symmetric))
+        assert_true(not self.is_symmetric or self.is_signed)
+
+    def dump_dict(self) -> Dict:
+        """Dump itelf to a dict.
+
+        Returns:
+            metadata (Dict): dict of serialized object
+        """
+        metadata: Dict[str, Any] = {}
+        metadata["cml_dumped_class_name"] = str(type(self).__name__)
+        metadata["n_bits"] = self.n_bits
+        metadata["is_signed"] = self.is_signed
+        metadata["is_symmetric"] = self.is_symmetric
+        metadata["is_qat"] = self.is_qat
+        metadata["is_narrow"] = self.is_narrow
+        metadata["is_precomputed_qat"] = self.is_precomputed_qat
+        return metadata
+
+    def dumps(self) -> str:
+        """Dump itelf to a string.
+
+        Returns:
+            metadata (str): string of serialized object
+        """
+
+        return json.dumps(self.dump_dict(), cls=CustomEncoder)
+
+    def dump(self, file: IO[str]):
+        """Dump itelf to a file.
+
+        Args:
+            file (IO[str]): file of where to dump.
+        """
+        metadata = self.dump_dict()
+        json.dump(metadata, file, cls=CustomEncoder)
+
+    # Loading
+    @staticmethod
+    def load_dict(metadata: Dict):
+        """Load itelf from a string.
+
+        Args:
+            metadata (Dict): dict of serialized object
+
+        Returns:
+            QuantizationOptions: the loaded object
+        """
+        to_return = QuantizationOptions(
+            n_bits=metadata["n_bits"],
+            is_symmetric=metadata["is_symmetric"],
+            is_signed=metadata["is_signed"],
+            is_qat=metadata["is_qat"],
+        )
+        for attr_name in ["is_narrow", "is_precomputed_qat"]:
+            setattr(to_return, attr_name, metadata[attr_name])
+        return to_return
+
+    @staticmethod
+    def load(file: IO[str]) -> QuantizationOptions:
+        """Load itelf from a file.
+
+        Args:
+            file (IO[str]): file of serialized object
+
+        Returns:
+            QuantizationOptions: the loaded object
+        """
+        metadata = json.load(file)
+        return QuantizationOptions.load_dict(metadata=metadata)
+
+    @staticmethod
+    def loads(metadata: str) -> QuantizationOptions:
+        """Load itelf from a string.
+
+        Args:
+            metadata (str): serialized object
+
+        Returns:
+            QuantizationOptions: the loaded object
+        """
+        _metadata: Dict = json.loads(metadata)
+        return QuantizationOptions.load_dict(metadata=_metadata)
 
     def copy_opts(self, opts):
         """Copy the options from a different structure.
 
         Args:
             opts (QuantizationOptions): structure to copy parameters from.
         """
@@ -163,14 +248,100 @@
     from the calibration set.
     """
 
     rmax: Optional[float] = None
     rmin: Optional[float] = None
     uvalues: Optional[numpy.ndarray] = None
 
+    def __init__(
+        self,
+        rmax: Optional[float] = None,
+        rmin: Optional[float] = None,
+        uvalues: Optional[numpy.ndarray] = None,
+    ):
+        self.rmax = rmax
+        self.rmin = rmin
+        self.uvalues = uvalues
+
+    def dump_dict(self) -> Dict:
+        """Dump itelf to a dict.
+
+        Returns:
+            metadata (Dict): dict of serialized object
+        """
+        metadata: Dict[str, Any] = {}
+        metadata["cml_dumped_class_name"] = str(type(self).__name__)
+        metadata["rmax"] = self.rmax
+        metadata["rmin"] = self.rmin
+        metadata["uvalues"] = self.uvalues
+        return metadata
+
+    def dumps(self) -> str:
+        """Dump itelf to a string.
+
+        Returns:
+            metadata (str): string of serialized object
+        """
+
+        return json.dumps(self.dump_dict(), cls=CustomEncoder)
+
+    def dump(self, file: IO[str]):
+        """Dump itelf to a file.
+
+        Args:
+            file (IO[str]): file of where to dump.
+        """
+        metadata = self.dump_dict()
+        json.dump(metadata, file, cls=CustomEncoder)
+
+    # Loading
+    @staticmethod
+    def load_dict(metadata: Dict):
+        """Load itelf from a string.
+
+        Args:
+            metadata (Dict): dict of serialized object
+
+        Returns:
+            QuantizationOptions: the loaded object
+        """
+        to_return = MinMaxQuantizationStats(
+            rmax=metadata["rmax"],
+            rmin=metadata["rmin"],
+            uvalues=numpy.array(metadata["uvalues"]),
+        )
+
+        return to_return
+
+    @staticmethod
+    def load(file: IO[str]) -> MinMaxQuantizationStats:
+        """Load itelf from a file.
+
+        Args:
+            file (IO[str]): file of serialized object
+
+        Returns:
+            MinMaxQuantizationStats: the loaded object
+        """
+        metadata = json.load(file)
+        return MinMaxQuantizationStats.load_dict(metadata=metadata)
+
+    @staticmethod
+    def loads(metadata: str) -> MinMaxQuantizationStats:
+        """Load itelf from a string.
+
+        Args:
+            metadata (str): serialized object
+
+        Returns:
+            MinMaxQuantizationStats: the loaded object
+        """
+        _metadata: Dict = json.loads(metadata)
+        return MinMaxQuantizationStats.load_dict(metadata=_metadata)
+
     def compute_quantization_stats(self, values: numpy.ndarray) -> None:
         """Compute the calibration set quantization statistics.
 
         Args:
             values (numpy.ndarray): Calibration set on which to compute statistics.
         """
 
@@ -247,14 +418,99 @@
     The parameters are computed from quantization options and quantization statistics.
     """
 
     scale: Optional[numpy.float64] = None
     zero_point: Optional[Union[int, float, numpy.ndarray]] = None
     offset: Optional[int] = None
 
+    def __init__(
+        self,
+        scale: Optional[numpy.float64] = None,
+        zero_point: Optional[Union[int, float, numpy.ndarray]] = None,
+        offset: Optional[int] = None,
+    ):
+        self.scale = scale
+        self.zero_point = zero_point
+        self.offset = offset
+
+    def dump_dict(self) -> Dict:
+        """Dump itelf to a dict.
+
+        Returns:
+            metadata (Dict): dict of serialized object
+        """
+        metadata: Dict[str, Any] = {}
+        metadata["cml_dumped_class_name"] = type(self).__name__
+        metadata["scale"] = self.scale
+        metadata["zero_point"] = self.zero_point
+        metadata["offset"] = self.offset
+        return metadata
+
+    def dumps(self) -> str:
+        """Dump itelf to a string.
+
+        Returns:
+            metadata (str): string of serialized object
+        """
+
+        return json.dumps(self.dump_dict(), cls=CustomEncoder)
+
+    def dump(self, file: IO[str]):
+        """Dump itelf to a file.
+
+        Args:
+            file (IO[str]): file of where to dump.
+        """
+        metadata = self.dump_dict()
+        json.dump(metadata, file, cls=CustomEncoder)
+
+    # Loading
+    @staticmethod
+    def load_dict(metadata: Dict) -> UniformQuantizationParameters:
+        """Load itelf from a string.
+
+        Args:
+            metadata (Dict): dict of serialized object
+
+        Returns:
+            UniformQuantizationParameters: the loaded object
+        """
+        to_return = UniformQuantizationParameters(
+            scale=metadata["scale"],
+            zero_point=metadata["zero_point"],
+            offset=metadata["offset"],
+        )
+        return to_return
+
+    @staticmethod
+    def load(file: IO[str]) -> UniformQuantizationParameters:
+        """Load itelf from a file.
+
+        Args:
+            file (IO[str]): file of serialized object
+
+        Returns:
+            UniformQuantizationParameters: the loaded object
+        """
+        metadata = json.load(file)
+        return UniformQuantizationParameters.load_dict(metadata=metadata)
+
+    @staticmethod
+    def loads(metadata: str) -> UniformQuantizationParameters:
+        """Load itelf from a string.
+
+        Args:
+            metadata (str): serialized object
+
+        Returns:
+            UniformQuantizationParameters: the loaded object
+        """
+        _metadata: Dict = json.loads(metadata)
+        return UniformQuantizationParameters.load_dict(metadata=_metadata)
+
     def copy_params(self, params) -> None:
         """Copy the parameters from a different structure.
 
         Args:
             params (UniformQuantizationParameters): parameter structure to copy
         """
 
@@ -343,18 +599,14 @@
                 # and will issue an error if the network is not well quantized during training
                 if (
                     options.is_qat
                     and not options.is_precomputed_qat
                     and stats.uvalues is not None
                     and stats.check_is_uniform_quantized(options)
                 ):
-
-                    # FIXME: this crashes when a model is poorly trained
-                    # the code crashes later on without this check
-                    # https://github.com/zama-ai/concrete-ml-internal/issues/1620
                     assert_true(
                         len(stats.uvalues) > 1,
                         "A single unique value was detected in a tensor of "
                         "quantized values in a QAT import.\n"
                         "Please check the stability thresholds.\n"
                         "This can occur with a badly trained model.",
                     )
@@ -372,64 +624,61 @@
                     self.zero_point = 0
                 else:
                     # for mypy
                     assert self.offset is not None
 
                     self.zero_point = numpy.round(
                         (
+                            # Pylint does not see that offset is not None here
+                            # pylint: disable-next=invalid-unary-operand-type
                             stats.rmax * (-self.offset)
                             - (stats.rmin * (2**options.n_bits - 1 - self.offset))
                         )
                         / (stats.rmax - stats.rmin)
                     ).astype(numpy.int64)
 
 
-# FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/1434
 # Change UniformQuantizer inheritance from UniformQuantizationParameters to composition.
+# FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/1434
 class UniformQuantizer(UniformQuantizationParameters, QuantizationOptions, MinMaxQuantizationStats):
     """Uniform quantizer.
 
     Contains all information necessary for uniform quantization and provides
     quantization/dequantization functionality on numpy arrays.
 
     Args:
         options (QuantizationOptions): Quantization options set
         stats (Optional[MinMaxQuantizationStats]): Quantization batch statistics set
         params (Optional[UniformQuantizationParameters]): Quantization parameters set
             (scale, zero-point)
     """
 
-    def __init__(  # pylint: disable=super-init-not-called
+    # pylint: disable-next=super-init-not-called
+    def __init__(
         self,
-        options: QuantizationOptions = None,
+        options: Optional[QuantizationOptions] = None,
         stats: Optional[MinMaxQuantizationStats] = None,
         params: Optional[UniformQuantizationParameters] = None,
-        **kwargs,
+        no_clipping: bool = False,
     ):
         if options is not None:
             self.copy_opts(options)
 
         if stats is not None:
             self.copy_stats(stats)
 
         if params is not None:
             self.copy_params(params)
 
-        if kwargs:
-            self.options, kwargs = fill_from_kwargs(self, QuantizationOptions, **kwargs)
-            self.stats, kwargs = fill_from_kwargs(self, MinMaxQuantizationStats, **kwargs)
-            self.params, kwargs = fill_from_kwargs(self, UniformQuantizationParameters, **kwargs)
+        self.no_clipping = no_clipping
 
         # Force scale to be a float64
         if self.scale is not None:
             self.scale = numpy.float64(self.scale)
 
-        # All kwargs should belong to one of the parameter sets, anything else is unsupported
-        assert_true(len(kwargs) == 0, f"Unexpected kwargs: {kwargs}")
-
     def quant(self, values: numpy.ndarray) -> numpy.ndarray:
         """Quantize values.
 
         Args:
             values (numpy.ndarray): float values to quantize
 
         Returns:
@@ -439,53 +688,135 @@
         # for mypy
         assert self.zero_point is not None
         assert self.offset is not None
         assert self.scale is not None
 
         qvalues = numpy.rint(values / self.scale + self.zero_point)
 
-        # Offset is either 2^(n-1) or 0, but for narrow range
-        # the values should be clipped to [2^(n-1)+1, .. 2^(n-1)-1], so we add
-        # one to the minimum value for narrow range
-        min_value = -self.offset
-        if self.is_narrow:
-            min_value += 1
-
         # Clipping can be performed for PTQ and for precomputed (for now only Brevitas) QAT
         # (where quantizer parameters are available in ONNX layers).
         # For Custom QAT, with inferred parameters the type of quantization (signed/narrow)
         # can not be inferred and thus clipping can not be performed reliably
-        if not self.is_qat or self.is_precomputed_qat:
+        # It is possible to disable this clipping step for specific cases such as quantizing values
+        # within fully-leveled circuits (where not bounds are needed)
+        if (not self.is_qat or self.is_precomputed_qat) and not self.no_clipping:
+            # Offset is either 2^(n-1) or 0, but for narrow range
+            # the values should be clipped to [2^(n-1)+1, .. 2^(n-1)-1], so we add
+            # one to the minimum value for narrow range
+            # Pylint does not see that offset is not None here
+            # pylint: disable-next=invalid-unary-operand-type
+            min_value = -self.offset
+            if self.is_narrow:
+                min_value += 1
+
             qvalues = qvalues.clip(min_value, 2 ** (self.n_bits) - 1 - self.offset)
 
         return qvalues.astype(numpy.int64)
 
-    def dequant(self, qvalues: numpy.ndarray) -> numpy.ndarray:
+    def dequant(self, qvalues: numpy.ndarray) -> Union[Any, numpy.ndarray]:
         """Dequantize values.
 
         Args:
             qvalues (numpy.ndarray): integer values to dequantize
 
         Returns:
-            numpy.ndarray: Dequantized float values.
+            Union[Any, numpy.ndarray]: Dequantized float values.
         """
 
         # for mypy
         assert self.zero_point is not None
         assert self.scale is not None
 
         assert_true(
-            isinstance(self.scale, numpy.float64)
+            isinstance(self.scale, (numpy.floating, float))
             or (isinstance(self.scale, numpy.ndarray) and self.scale.dtype is numpy.float64),
-            "Scale is a "
-            + str(type(self.scale))
+            "Scale is a of type "
+            + type(self.scale).__name__
             + ((" " + str(self.scale.dtype)) if isinstance(self.scale, numpy.ndarray) else ""),
         )
 
-        return self.scale * (qvalues - numpy.asarray(self.zero_point, dtype=numpy.float64))
+        ans = self.scale * (qvalues - numpy.asarray(self.zero_point, dtype=numpy.float64))
+
+        return ans
+
+    def dump_dict(self) -> Dict:
+        """Dump itelf to a dict.
+
+        Returns:
+            metadata (Dict): dict of serialized object
+        """
+        metadata: Dict[str, Any] = {}
+        metadata["cml_dumped_class_name"] = str(type(self).__name__)
+
+        for attribute in ["zero_point", "scale", "offset", "n_bits"]:
+            if hasattr(self, attribute):
+                metadata[attribute] = getattr(self, attribute)
+        return metadata
+
+    def dumps(self) -> str:
+        """Dump itelf to a string.
+
+        Returns:
+            metadata (str): string of serialized object
+        """
+        metadata = self.dump_dict()
+        return json.dumps(metadata, cls=CustomEncoder)
+
+    def dump(self, file: IO[str]) -> None:
+        """Dump itelf to a file.
+
+        Args:
+            file (IO[str]): file of where to dump.
+        """
+        metadata = self.dump_dict()
+        json.dump(metadata, file, cls=CustomEncoder)
+
+    # Loading
+    @staticmethod
+    def load_dict(metadata: Dict) -> UniformQuantizer:
+        """Load itelf from a string.
+
+        Args:
+            metadata (Dict): dict of serialized object
+
+        Returns:
+            UniformQuantizer: the loaded object
+        """
+        obj = UniformQuantizer()
+
+        for attribute in ["zero_point", "scale", "offset", "n_bits"]:
+            if attribute in metadata:
+                setattr(obj, attribute, metadata[attribute])
+        return obj
+
+    @staticmethod
+    def load(file: IO[str]) -> UniformQuantizer:
+        """Load itelf from a file.
+
+        Args:
+            file (IO[str]): file of serialized object
+
+        Returns:
+            UniformQuantizer: the loaded object
+        """
+        metadata = json.load(file)
+        return UniformQuantizer.load_dict(metadata=metadata)
+
+    @staticmethod
+    def loads(metadata: str) -> UniformQuantizer:
+        """Load itelf from a string.
+
+        Args:
+            metadata (str): serialized object
+
+        Returns:
+            UniformQuantizer: the loaded object
+        """
+        _metadata: Dict = json.loads(metadata)
+        return UniformQuantizer.load_dict(metadata=_metadata)
 
 
 class QuantizedArray:
     """Abstraction of quantized array.
 
     Contains float values and their quantized integer counter-parts. Quantization is performed
     by the quantizer member object. Float and int values are kept in sync. Having both types
@@ -516,25 +847,26 @@
     qvalues: numpy.ndarray
 
     def __init__(
         self,
         n_bits,
         values: Optional[numpy.ndarray],
         value_is_float: bool = True,
-        options: QuantizationOptions = None,
+        options: Optional[QuantizationOptions] = None,
         stats: Optional[MinMaxQuantizationStats] = None,
         params: Optional[UniformQuantizationParameters] = None,
         **kwargs,
     ):
         # If no options were passed, create a default options structure with the required n_bits
         options = deepcopy(options) if options is not None else QuantizationOptions(n_bits)
 
         # Override the options number of bits if an options structure was provided
         # with the number of bits specified by the caller.
         options.n_bits = n_bits
+        self.n_bits = n_bits
 
         options, kwargs = fill_from_kwargs(options, QuantizationOptions, **kwargs)
         stats, kwargs = fill_from_kwargs(stats, MinMaxQuantizationStats, **kwargs)
         params, kwargs = fill_from_kwargs(params, UniformQuantizationParameters, **kwargs)
 
         # All kwargs should belong to one of the parameter sets, anything else is unsupported
         if len(kwargs) > 0:
@@ -571,16 +903,14 @@
             if isinstance(values, numpy.ndarray):
                 assert_true(
                     numpy.issubdtype(values.dtype, numpy.floating),
                     "Values must be float if value_is_float is set to True, "
                     f"got {values.dtype}: {values}",
                 )
 
-            # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/303
-            # To be seen what should be done in the long run (refactor of this class or Tracers)
             self.values = deepcopy(values) if isinstance(values, numpy.ndarray) else values
 
             # If no stats are provided, compute them.
             # Note that this cannot be done during tracing
             if stats is None:
                 self.quantizer.compute_quantization_stats(values)
 
@@ -604,16 +934,14 @@
                 assert_true(
                     numpy.issubdtype(values.dtype, numpy.integer)
                     or numpy.issubdtype(values.dtype, numpy.unsignedinteger),
                     f"Can't create a QuantizedArray from {values.dtype} values "
                     "when int/uint was required",
                 )
 
-            # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/303
-            # To be seen what should be done in the long run (refactor of this class or Tracers)
             self.qvalues = deepcopy(values) if isinstance(values, numpy.ndarray) else values
 
             # Populate self.values
             self.dequant()
 
     def __call__(self) -> Optional[numpy.ndarray]:
         return self.qvalues
@@ -623,31 +951,27 @@
 
         Args:
             values (numpy.ndarray): Values to replace self.values
 
         Returns:
             qvalues (numpy.ndarray): Corresponding qvalues
         """
-        # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/303
-        # To be seen what should be done in the long run (refactor of this class or Tracers)
         self.values = deepcopy(values) if isinstance(values, numpy.ndarray) else values
         self.quant()
         return self.qvalues
 
     def update_quantized_values(self, qvalues: numpy.ndarray) -> numpy.ndarray:
         """Update qvalues to get their corresponding values using the related quantized parameters.
 
         Args:
             qvalues (numpy.ndarray): Values to replace self.qvalues
 
         Returns:
             values (numpy.ndarray): Corresponding values
         """
-        # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/303
-        # To be seen what should be done in the long run (refactor of this class or Tracers)
         self.qvalues = deepcopy(qvalues) if isinstance(qvalues, numpy.ndarray) else qvalues
         self.dequant()
         return self.values
 
     def quant(self) -> Optional[numpy.ndarray]:
         """Quantize self.values.
 
@@ -660,15 +984,93 @@
 
     def dequant(self) -> numpy.ndarray:
         """Dequantize self.qvalues.
 
         Returns:
             numpy.ndarray: Dequantized values.
         """
-        # TODO: https://github.com/zama-ai/concrete-numpy-internal/issues/721
-        # remove this + (-x) when the above issue is done
         self.values = self.quantizer.dequant(self.qvalues)
         assert_true(
             not isinstance(self.values, numpy.ndarray) or self.values.dtype == numpy.float64,
             "Dequantized values must be float64",
         )
         return self.values
+
+    def dump_dict(self) -> Dict:
+        """Dump itelf to a dict.
+
+        Returns:
+            metadata (Dict): dict of serialized object
+        """
+        metadata: Dict[str, Any] = {}
+        metadata["cml_dumped_class_name"] = str(type(self).__name__)
+        metadata["STABILITY_CONST"] = self.STABILITY_CONST
+        metadata["quantizer"] = self.quantizer
+        metadata["n_bits"] = self.n_bits
+        metadata["values"] = self.values
+        metadata["qvalues"] = self.qvalues
+        metadata["values"] = self.values
+        return metadata
+
+    def dumps(self) -> str:
+        """Dump itelf to a string.
+
+        Returns:
+            metadata (str): string of serialized object
+        """
+        metadata = self.dump_dict()
+        return json.dumps(metadata, cls=CustomEncoder)
+
+    def dump(self, file: IO[str]) -> None:
+        """Dump itelf to a file.
+
+        Args:
+            file (IO[str]): file of where to dump.
+        """
+        metadata = self.dump_dict()
+        json.dump(metadata, file, cls=CustomEncoder)
+
+    # Loading
+    @staticmethod
+    def load_dict(metadata: Dict) -> QuantizedArray:
+        """Load itelf from a string.
+
+        Args:
+            metadata (Dict): dict of serialized object
+
+        Returns:
+            QuantizedArray: the loaded object
+        """
+        obj = QuantizedArray(n_bits=metadata["n_bits"], values=metadata["values"])
+        # pylint: disable-next=invalid-name
+        obj.STABILITY_CONST = metadata["STABILITY_CONST"]
+        obj.quantizer = metadata["quantizer"]
+        obj.values = metadata["values"]
+        obj.qvalues = metadata["qvalues"]
+
+        return obj
+
+    @staticmethod
+    def load(file: IO[str]) -> QuantizedArray:
+        """Load itelf from a file.
+
+        Args:
+            file (IO[str]): file of serialized object
+
+        Returns:
+            QuantizedArray: the loaded object
+        """
+        metadata = json.load(file)
+        return QuantizedArray.load_dict(metadata=metadata)
+
+    @staticmethod
+    def loads(metadata: str) -> QuantizedArray:
+        """Load itelf from a string.
+
+        Args:
+            metadata (str): serialized object
+
+        Returns:
+            QuantizedArray: the loaded object
+        """
+        _metadata: Dict = json.loads(metadata)
+        return QuantizedArray.load_dict(metadata=_metadata)
```

## concrete/ml/sklearn/__init__.py

```diff
@@ -1,8 +1,119 @@
 """Import sklearn models."""
+from ..common.debugging.custom_assert import assert_true
+from ..common.utils import is_classifier_or_partial_classifier, is_regressor_or_partial_regressor
+from .base import _ALL_SKLEARN_MODELS, _LINEAR_MODELS, _NEURALNET_MODELS, _TREE_MODELS
 from .glm import GammaRegressor, PoissonRegressor, TweedieRegressor
 from .linear_model import ElasticNet, Lasso, LinearRegression, LogisticRegression, Ridge
 from .qnn import NeuralNetClassifier, NeuralNetRegressor
 from .rf import RandomForestClassifier, RandomForestRegressor
 from .svm import LinearSVC, LinearSVR
 from .tree import DecisionTreeClassifier, DecisionTreeRegressor
 from .xgb import XGBClassifier, XGBRegressor
+
+
+def get_sklearn_models():
+    """Return the list of available models in Concrete ML.
+
+    Returns:
+        the lists of models in Concrete ML
+    """
+
+    # Import anything in sklearn, just to force the import, to populate _ALL_SKLEARN_MODELS list
+    # pylint: disable-next=unused-import, import-outside-toplevel, cyclic-import, redefined-outer-name  # noqa: E501
+    from .linear_model import LinearRegression  # noqa: F401, F811
+
+    # We return sorted lists such that it is ordered, to avoid notably issues when it is used
+    # in @pytest.mark.parametrize
+    ans = {
+        "all": sorted(list(_ALL_SKLEARN_MODELS), key=lambda m: m.__name__),
+        "linear": sorted(list(_LINEAR_MODELS), key=lambda m: m.__name__),
+        "tree": sorted(list(_TREE_MODELS), key=lambda m: m.__name__),
+        "neural_net": sorted(list(_NEURALNET_MODELS), key=lambda m: m.__name__),
+    }
+    return ans
+
+
+def _filter_models(prelist, classifier: bool, regressor: bool, str_in_class_name: str = None):
+    """Return the models which are in prelist and follow (classifier, regressor) conditions.
+
+    Args:
+        prelist: list of models
+        classifier (bool): whether you want classifiers or not
+        regressor (bool): whether you want regressors or not
+        str_in_class_name (str): if not None, only return models with this as a substring in the
+            class name
+
+    Returns:
+        the sublist which fulfills the (classifier, regressor, str_in_class_name) conditions.
+
+    """
+    assert_true(classifier or regressor, "Please set at least one option")
+
+    answer = []
+
+    if classifier:
+        answer += [m for m in prelist if is_classifier_or_partial_classifier(m)]
+
+    if regressor:
+        answer += [m for m in prelist if is_regressor_or_partial_regressor(m)]
+
+    if str_in_class_name is not None:
+        answer = [m for m in answer if str_in_class_name in m.__name__]
+
+    # We return a sorted list such that it is ordered, to avoid notably issues when it is used
+    # in @pytest.mark.parametrize
+    return sorted(answer, key=lambda m: m.__name__)
+
+
+def get_sklearn_linear_models(
+    classifier: bool = True, regressor: bool = True, str_in_class_name: str = None
+):
+    """Return the list of available linear models in Concrete ML.
+
+    Args:
+        classifier (bool): whether you want classifiers or not
+        regressor (bool): whether you want regressors or not
+        str_in_class_name (str): if not None, only return models with this as a substring in the
+            class name
+
+    Returns:
+        the lists of linear models in Concrete ML
+    """
+    prelist = get_sklearn_models()["linear"]
+    return _filter_models(prelist, classifier, regressor, str_in_class_name)
+
+
+def get_sklearn_tree_models(
+    classifier: bool = True, regressor: bool = True, str_in_class_name: str = None
+):
+    """Return the list of available tree models in Concrete ML.
+
+    Args:
+        classifier (bool): whether you want classifiers or not
+        regressor (bool): whether you want regressors or not
+        str_in_class_name (str): if not None, only return models with this as a substring in the
+            class name
+
+    Returns:
+        the lists of tree models in Concrete ML
+    """
+    prelist = get_sklearn_models()["tree"]
+    return _filter_models(prelist, classifier, regressor, str_in_class_name)
+
+
+def get_sklearn_neural_net_models(
+    classifier: bool = True, regressor: bool = True, str_in_class_name: str = None
+):
+    """Return the list of available neural net models in Concrete ML.
+
+    Args:
+        classifier (bool): whether you want classifiers or not
+        regressor (bool): whether you want regressors or not
+        str_in_class_name (str): if not None, only return models with this as a substring in the
+            class name
+
+    Returns:
+        the lists of neural net models in Concrete ML
+    """
+    prelist = get_sklearn_models()["neural_net"]
+    return _filter_models(prelist, classifier, regressor, str_in_class_name)
```

## concrete/ml/sklearn/base.py

```diff
@@ -1,530 +1,964 @@
-"""Module that contains base classes for our libraries estimators."""
-import copy
-import functools
+"""Base classes for all estimators."""
+from __future__ import annotations
+
+import json
 import tempfile
 
-# https://github.com/zama-ai/concrete-ml-internal/issues/942
-# Refactoring base.py. This file is more than 1000 lines.
-# We use names like X and q_X
+# Disable pylint as some names like X and q_X are used, following Scikit-Learn's standard. The file
+# is also more than 1000 lines long.
 # pylint: disable=too-many-lines,invalid-name
 import warnings
-from abc import abstractmethod
+from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Type, Union
+from typing import IO, Any, Callable, Dict, List, Optional, Set, Type, Union
 
 import brevitas.nn as qnn
 import numpy
 import onnx
 import sklearn
 import torch
 from brevitas.export.onnx.qonnx.manager import QONNXManager as BrevitasONNXManager
-from concrete.numpy.compilation.artifacts import DebugArtifacts
-from concrete.numpy.compilation.circuit import Circuit
-from concrete.numpy.compilation.compiler import Compiler
-from concrete.numpy.compilation.configuration import Configuration
-from concrete.numpy.dtypes.integer import Integer
-
-from concrete.ml.quantization.quantized_module import QuantizedModule, _get_inputset_generator
-from concrete.ml.quantization.quantizers import QuantizationOptions, UniformQuantizer
+from concrete.fhe.compilation.artifacts import DebugArtifacts
+from concrete.fhe.compilation.circuit import Circuit
+from concrete.fhe.compilation.compiler import Compiler
+from concrete.fhe.compilation.configuration import Configuration
+from concrete.fhe.dtypes.integer import Integer
+from sklearn.base import clone
+from skorch.net import NeuralNet as SkorchNeuralNet
 
-from ..common.check_inputs import check_array_and_assert, check_X_y_and_assert
+from ..common.check_inputs import check_array_and_assert, check_X_y_and_assert_multi_output
 from ..common.debugging.custom_assert import assert_true
+from ..common.serialization.encoder import CustomEncoder
 from ..common.utils import (
+    FheMode,
     check_there_is_no_p_error_options_in_configuration,
     generate_proxy_function,
     manage_parameters_for_pbs_errors,
 )
 from ..onnx.convert import OPSET_VERSION_FOR_ONNX_EXPORT
 from ..onnx.onnx_model_manipulations import clean_graph_after_node_op_type, remove_node_types
 
 # The sigmoid and softmax functions are already defined in the ONNX module and thus are imported
 # here in order to avoid duplicating them.
 from ..onnx.ops_impl import numpy_sigmoid, numpy_softmax
 from ..quantization import PostTrainingQATImporter, QuantizedArray, get_n_bits_dict
+from ..quantization.quantized_module import QuantizedModule, _get_inputset_generator
+from ..quantization.quantizers import (
+    QuantizationOptions,
+    UniformQuantizationParameters,
+    UniformQuantizer,
+)
 from ..torch import NumpyModule
-from .protocols import Quantizer
-from .tree_to_numpy import Task, tree_to_numpy
+from .qnn_module import SparseQuantNeuralNetwork
+from .tree_to_numpy import tree_to_numpy
 
 # Disable pylint to import hummingbird while ignoring the warnings
 # pylint: disable=wrong-import-position,wrong-import-order
 # Silence hummingbird warnings
 warnings.filterwarnings("ignore")
 from hummingbird.ml import convert as hb_convert  # noqa: E402
 
-# pylint: enable=wrong-import-position,wrong-import-order
-
 _ALL_SKLEARN_MODELS: Set[Type] = set()
 _LINEAR_MODELS: Set[Type] = set()
 _TREE_MODELS: Set[Type] = set()
 _NEURALNET_MODELS: Set[Type] = set()
 
+# Define the supported types for both the input data and the target values. Since the Pandas
+# library is currently only a dev dependencies, we cannot import it. We therefore need to use type
+# strings and the `name-defined` mypy error to do so.
+Data = Union[
+    numpy.ndarray,
+    torch.Tensor,
+    "pandas.DataFrame",  # type: ignore[name-defined] # noqa: F821
+    List,
+]
+Target = Union[
+    numpy.ndarray,
+    torch.Tensor,
+    "pandas.DataFrame",  # type: ignore[name-defined] # noqa: F821
+    "pandas.Series",  # type: ignore[name-defined] # noqa: F821
+    List,
+]
+
+# Define QNN's attribute that will be auto-generated when fitting
+QNN_AUTO_KWARGS = ["module__n_outputs", "module__input_dim"]
+
+
+# pylint: disable=too-many-public-methods
+class BaseEstimator:
+    """Base class for all estimators in Concrete ML.
+
+    This class does not inherit from sklearn.base.BaseEstimator as it creates some conflicts
+    with Skorch in QuantizedTorchEstimatorMixin's subclasses (more specifically, the `get_params`
+    method is not properly inherited).
+
+    Attributes:
+        _is_a_public_cml_model (bool): Private attribute indicating if the class is a public model
+            (as opposed to base or mixin classes).
+    """
 
-class QuantizedTorchEstimatorMixin:
-    """Mixin that provides quantization for a torch module and follows the Estimator API.
+    #: Base float estimator class to consider for the model. Is set for each subclasses.
+    sklearn_model_class: Type
 
-    This class should be mixed in with another that provides the full Estimator API. This class
-    only provides modifiers for .fit() (with quantization) and .predict() (optionally in FHE)
-    """
+    _is_a_public_cml_model: bool = False
 
-    post_processing_params: Dict[str, Any] = {}
-    _is_a_public_cml_model = False
+    def __init__(self):
+        """Initialize the base class with common attributes used in all estimators.
 
-    def __init_subclass__(cls):
-        for klass in cls.__mro__:
+        An underscore "_" is appended to attributes that were created while fitting the model. This
+        is done in order to follow Scikit-Learn's standard format. More information available
+        in their documentation:
+        https://scikit-learn.org/stable/developers/develop.html#:~:text=Estimated%20Attributes%C2%B6
+        """
+        #: The equivalent fitted float model. Is None if the model is not fitted.
+        self.sklearn_model: Optional[sklearn.base.BaseEstimator] = None
+
+        #: The list of quantizers, which contain all information necessary for applying uniform
+        #: quantization to inputs and provide quantization/dequantization functionalities. Is empty
+        #: if the model is not fitted
+        self.input_quantizers: List[UniformQuantizer] = []
 
-            # pylint: disable-next=protected-access
-            if hasattr(klass, "_is_a_public_cml_model") and klass._is_a_public_cml_model:
-                _NEURALNET_MODELS.add(cls)
-                _ALL_SKLEARN_MODELS.add(cls)
+        #: The list of quantizers, which contain all information necessary for applying uniform
+        #: quantization to outputs and provide quantization/dequantization functionalities. Is
+        #: empty if the model is not fitted
+        self.output_quantizers: List[UniformQuantizer] = []
 
-    def __init__(
-        self,
-    ):
-        # The quantized module variable appends "_" so that it is not registered as a sklearn
-        # parameter. Only training parameters should register, to enable easy cloning of untrained
-        # estimator
-        self.quantized_module_ = None
-        self._onnx_model_ = None
+        #: The parameters needed for post-processing the outputs.
+        #: Can be empty if no post-processing operations are needed for the associated model
+        #: This attribute is typically used for serving models
+        self.post_processing_params: Dict[str, Any] = {}
+
+        #: Indicate if the model is fitted.
+        self._is_fitted: bool = False
+
+        #: Indicate if the model is compiled.
+        self._is_compiled: bool = False
+
+        self.fhe_circuit_: Optional[Circuit] = None
+        self.onnx_model_: Optional[onnx.ModelProto] = None
 
     @property
-    @abstractmethod
-    def base_estimator_type(self):
-        """Get the sklearn estimator that should be trained by the child class."""
+    def onnx_model(self) -> Optional[onnx.ModelProto]:
+        """Get the ONNX model.
 
-    def get_params_for_benchmark(self):
-        """Get the parameters to instantiate the sklearn estimator trained by the child class.
+        Is None if the model is not fitted.
 
         Returns:
-            params (dict): dictionary with parameters that will initialize a new Estimator
+            onnx.ModelProto: The ONNX model.
         """
-        return self.get_params()
+        assert isinstance(self.onnx_model_, onnx.ModelProto) or self.onnx_model_ is None
+        return self.onnx_model_
 
     @property
-    def input_quantizers(self) -> List[Quantizer]:
-        """Get the input quantizers.
+    def fhe_circuit(self) -> Optional[Circuit]:
+        """Get the FHE circuit.
+
+        The FHE circuit combines computational graph, mlir, client and server into a single object.
+        More information available in Concrete documentation:
+        https://docs.zama.ai/concrete/developer/terminology_and_structure#terminology
+        Is None if the model is not fitted.
 
         Returns:
-            List[Quantizer]: the input quantizers
+            Circuit: The FHE circuit.
         """
-        return self.quantized_module_.input_quantizers
+        assert isinstance(self.fhe_circuit_, Circuit) or self.fhe_circuit_ is None
+        return self.fhe_circuit_
 
-    @input_quantizers.setter
-    def input_quantizers(self, value: List[Quantizer]):
-        """Set the input quantizers.
+    @fhe_circuit.setter
+    def fhe_circuit(self, value: Circuit) -> None:
+        """Set the FHE circuit.
 
         Args:
-            value (List[Quantizer]): the input quantizers
+            value (Circuit): The FHE circuit to set.
         """
-        self.quantized_module_ = QuantizedModule()
-        self.quantized_module_.input_quantizers = value
+        self.fhe_circuit_ = value
 
-    @property
-    @abstractmethod
-    def base_module_to_compile(self):
-        """Get the Torch module that should be compiled to FHE."""
+    def _sklearn_model_is_not_fitted_error_message(self) -> str:
+        return (
+            f"The underlying model (class: {self.sklearn_model_class}) is not fitted and thus "
+            "cannot be quantized."
+        )  # pragma: no cover
 
     @property
-    @abstractmethod
-    def n_bits_quant(self):
-        """Get the number of quantization bits."""
+    def is_fitted(self) -> bool:
+        """Indicate if the model is fitted.
 
-    @property
-    def onnx_model(self):
-        """Get the ONNX model.
+        Returns:
+            bool: If the model is fitted.
+        """
+        return self._is_fitted
 
-        .. # noqa: DAR201
+    def _is_not_fitted_error_message(self) -> str:
+        return (
+            f"The {self.__class__.__name__} model is not fitted. "
+            "Please run fit(...) on proper arguments first."
+        )
 
-        Returns:
-           _onnx_model_ (onnx.ModelProto): the ONNX model
+    def check_model_is_fitted(self) -> None:
+        """Check if the model is fitted.
+
+        Raises:
+            AttributeError: If the model is not fitted.
         """
-        return self._onnx_model_
+        if not self.is_fitted:
+            raise AttributeError(self._is_not_fitted_error_message())
 
     @property
-    def quantize_input(self) -> Callable:
-        """Get the input quantization function.
+    def is_compiled(self) -> bool:
+        """Indicate if the model is compiled.
 
         Returns:
-            Callable : function that quantizes the input
+            bool: If the model is compiled.
         """
-        assert self.quantized_module_ is not None
-        return self.quantized_module_.quantize_input
+        return self._is_compiled
 
-    @property
-    def fhe_circuit(self) -> Circuit:
-        """Get the FHE circuit.
+    def _is_not_compiled_error_message(self) -> str:
+        return (
+            f"The {self.__class__.__name__} model is not compiled. "
+            "Please run compile(...) first before executing the prediction in FHE."
+        )
 
-        Returns:
-            Circuit: the FHE circuit
+    def check_model_is_compiled(self) -> None:
+        """Check if the model is compiled.
+
+        Raises:
+            AttributeError: If the model is not compiled.
         """
-        return self.quantized_module_.fhe_circuit
+        if not self.is_compiled:
+            raise AttributeError(self._is_not_compiled_error_message())
 
-    @fhe_circuit.setter
-    def fhe_circuit(self, value: Circuit):
-        """Set the FHE circuit.
+    def get_sklearn_params(self, deep: bool = True) -> dict:
+        """Get parameters for this estimator.
+
+        This method is used to instantiate a Scikit-Learn model using the Concrete ML model's
+        parameters. It does not override Scikit-Learn's existing `get_params` method in order to
+        not break its implementation of `set_params`.
 
         Args:
-            value (Circuit): the FHE circuit
+            deep (bool): If True, will return the parameters for this estimator and contained
+                subobjects that are estimators. Default to True.
+
+        Returns:
+            params (dict): Parameter names mapped to their values.
         """
-        self.quantized_module_.fhe_circuit = value
+        # Here, the `get_params` method is the `BaseEstimator.get_params` method from Scikit-Learn,
+        # which will become available once a subclass inherits from it. We therefore disable both
+        # pylint and mypy as this behavior is expected
+        # pylint: disable-next=no-member
+        # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/3373
+        params = super().get_params(deep=deep)  # type: ignore[misc]
 
-    @property
-    def output_quantizers(self) -> List[QuantizedArray]:
-        """Get the input quantizers.
+        # Remove the n_bits parameters as this attribute is added by Concrete ML
+        params.pop("n_bits", None)
+
+        return params
+
+    def _set_post_processing_params(self) -> None:
+        """Set parameters used in post-processing."""
+        self.post_processing_params = {}
+
+    def _fit_sklearn_model(self, X: Data, y: Target, **fit_parameters):
+        """Fit the model's Scikit-Learn equivalent estimator.
+
+        Args:
+            X (Data): The training data, as a Numpy array, Torch tensor, Pandas DataFrame or List.
+            y (Target): The target data, as a Numpy array, Torch tensor, Pandas DataFrame, Pandas
+                Series or List.
+            **fit_parameters: Keyword arguments to pass to the Scikit-Learn estimator's fit method.
 
         Returns:
-            List[QuantizedArray]: the input quantizers
+            The fitted Scikit-Learn estimator.
         """
-        return self.quantized_module_.output_quantizers
 
-    @output_quantizers.setter
-    def output_quantizers(self, value: List[QuantizedArray]):
-        """Set the input quantizers.
+        # Initialize the underlying Scikit-learn model if it has not already been done or if
+        # `warm_start` is set to False (for neural networks)
+        # This model should be directly initialized in the model's __init__ method instead
+        # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/3373
+        if self.sklearn_model is None or not getattr(self, "warm_start", False):
+            # Retrieve the init parameters
+            params = self.get_sklearn_params()
+
+            self.sklearn_model = self.sklearn_model_class(**params)
+
+        # Fit the Scikit-Learn model
+        self.sklearn_model.fit(X, y, **fit_parameters)
+
+        return self.sklearn_model
+
+    @abstractmethod
+    def fit(self, X: Data, y: Target, **fit_parameters):
+        """Fit the estimator.
+
+        This method trains a Scikit-Learn estimator, computes its ONNX graph and defines the
+        quantization parameters needed for proper FHE inference.
 
         Args:
-            value (List[QuantizedArray]): the input quantizers
+            X (Data): The training data, as a Numpy array, Torch tensor, Pandas DataFrame or List.
+            y (Target): The target data, as a Numpy array, Torch tensor, Pandas DataFrame, Pandas
+                Series or List.
+            **fit_parameters: Keyword arguments to pass to the float estimator's fit method.
+
+        Returns:
+            The fitted estimator.
         """
-        self.quantized_module_.output_quantizers = value
 
-    def post_processing(self, y_preds: numpy.ndarray) -> numpy.ndarray:
-        """Post-processing the output.
+    # Several attributes and methods are called in `fit_benchmark` but will only be accessible
+    # in subclasses, we therefore need to disable pylint and mypy from checking these no-member
+    # issues
+    # pylint: disable=no-member
+    def fit_benchmark(
+        self,
+        X: Data,
+        y: Target,
+        random_state: Optional[int] = None,
+        **fit_parameters,
+    ):
+        """Fit both the Concrete ML and its equivalent float estimators.
 
         Args:
-            y_preds (numpy.ndarray): the output to post-process
+            X (Data): The training data, as a Numpy array, Torch tensor, Pandas DataFrame or List.
+            y (Target): The target data, as a Numpy array, Torch tensor, Pandas DataFrame, Pandas
+                Series or List.
+            random_state (Optional[int]): The random state to use when fitting. Defaults to None.
+            **fit_parameters: Keyword arguments to pass to the float estimator's fit method.
 
-        Raises:
-            ValueError: if unknown post-processing function
+        Returns:
+            The Concrete ML and float equivalent fitted estimators.
+        """
+
+        # Retrieve sklearn's init parameters
+        params = self.get_sklearn_params()
+
+        # Make sure the random_state is set or both algorithms will diverge
+        # due to randomness in the training.
+        if "random_state" in params:
+            if random_state is not None:
+                params["random_state"] = random_state
+            elif getattr(self, "random_state", None) is not None:
+                # Disable mypy attribute definition errors as it does not seem to see that we make
+                # sure this attribute actually exists before calling it
+                params["random_state"] = self.random_state  # type: ignore[attr-defined]
+            else:
+                params["random_state"] = numpy.random.randint(0, 2**15)
+
+        # Initialize the Scikit-Learn model
+        sklearn_model = self.sklearn_model_class(**params)
+
+        # Train the Scikit-Learn model
+        sklearn_model.fit(X, y, **fit_parameters)
+
+        # Update the Concrete ML model's parameters
+        # Disable mypy attribute definition errors as this attribute is expected to be
+        # initialized once the model inherits from Skorch
+        self.set_params(n_bits=self.n_bits, **params)  # type: ignore[attr-defined]
+
+        # Train the Concrete ML model
+        self.fit(X, y, **fit_parameters)
+
+        return self, sklearn_model
+
+    # pylint: enable=no-member
+
+    @abstractmethod
+    def quantize_input(self, X: numpy.ndarray) -> numpy.ndarray:
+        """Quantize the input.
+
+        This step ensures that the fit method has been called.
+
+        Args:
+            X (numpy.ndarray): The input values to quantize.
 
         Returns:
-            numpy.ndarray: the post-processed output
+            numpy.ndarray: The quantized input values.
         """
-        y_preds = self.quantized_module_.dequantize_output(y_preds)
 
-        if self.post_processing_params["post_processing_function_name"] == "softmax":
-            # Get dim argument
-            dim = self.post_processing_params["post_processing_function_keywords"]["dim"]
+    @abstractmethod
+    def dequantize_output(self, q_y_preds: numpy.ndarray) -> numpy.ndarray:
+        """Dequantize the output.
 
-            # Apply softmax to the output
-            y_preds = numpy_softmax(y_preds, axis=dim)[0]
+        This step ensures that the fit method has been called.
 
-        elif "sigmoid" in self.post_processing_params["post_processing_function_name"]:
-            # Transform in a 2d array where [p, 1-p] is the output
-            y_preds = numpy.concatenate((y_preds, 1 - y_preds), axis=1)  # pragma: no cover
+        Args:
+            q_y_preds (numpy.ndarray): The quantized output values to dequantize.
 
-        elif self.post_processing_params["post_processing_function_name"] == "_identity":
-            pass
+        Returns:
+            numpy.ndarray: The dequantized output values.
+        """
 
-        else:
-            raise ValueError(
-                "Unknown post-processing function "
-                f"{self.post_processing_params['post_processing_function_name']}"
-            )  # pragma: no cover
+    @abstractmethod
+    def _get_module_to_compile(self) -> Union[Compiler, QuantizedModule]:
+        """Retrieve the module instance to compile.
 
-        # To match torch softmax we need to cast to float32
-        return y_preds.astype(numpy.float32)
+        Returns:
+            Union[Compiler, QuantizedModule]: The module instance to compile.
+        """
 
     def compile(
         self,
-        X: numpy.ndarray,
+        X: Data,
         configuration: Optional[Configuration] = None,
-        compilation_artifacts: Optional[DebugArtifacts] = None,
+        artifacts: Optional[DebugArtifacts] = None,
         show_mlir: bool = False,
-        use_virtual_lib: bool = False,
         p_error: Optional[float] = None,
         global_p_error: Optional[float] = None,
-        verbose_compilation: bool = False,
+        verbose: bool = False,
     ) -> Circuit:
         """Compile the model.
 
         Args:
-            X (numpy.ndarray): the dequantized dataset
-            configuration (Optional[Configuration]): the options for
-                compilation
-            compilation_artifacts (Optional[DebugArtifacts]): artifacts object to fill
-                during compilation
-            show_mlir (bool): whether or not to show MLIR during the compilation
-            use_virtual_lib (bool): whether to compile using the virtual library that allows higher
-                bitwidths
-            p_error (Optional[float]): probability of error of a single PBS
-            global_p_error (Optional[float]): probability of error of the full circuit. Not
-                simulated by the VL, i.e., taken as 0
-            verbose_compilation (bool): whether to show compilation information
+            X (Data): A representative set of input values used for building cryptographic
+                parameters, as a Numpy array, Torch tensor, Pandas DataFrame or List. This is
+                usually the training data set or s sub-set of it.
+            configuration (Optional[Configuration]): Options to use for compilation. Default
+                to None.
+            artifacts (Optional[DebugArtifacts]): Artifacts information about the compilation
+                process to store for debugging. Default to None.
+            show_mlir (bool): Indicate if the MLIR graph should be printed during compilation.
+                Default to False.
+            p_error (Optional[float]): Probability of error of a single PBS. A p_error value cannot
+                be given if a global_p_error value is already set. Default to None, which sets this
+                error to a default value.
+            global_p_error (Optional[float]): Probability of error of the full circuit. A
+                global_p_error value cannot be given if a p_error value is already set. This feature
+                is not supported during the FHE simulation mode, meaning the probability is
+                currently set to 0. Default to None, which sets this error to a default value.
+            verbose (bool): Indicate if compilation information should be printed
+                during compilation. Default to False.
 
         Returns:
-            Circuit: the compiled Circuit.
-
-        Raises:
-            ValueError: if called before the model is trained
+            Circuit: The compiled Circuit.
         """
-        if self.quantized_module_ is None:
-            raise ValueError(
-                "The classifier needs to be calibrated before compilation,"
-                " please call .fit() first!"
-            )
+        # Reset for double compile
+        self._is_compiled = False
 
-        # Quantize the compilation input set using the quantization parameters computed in .fit()
-        quantized_numpy_inputset = self.quantized_module_.quantize_input(X)
+        # Check that the model is correctly fitted
+        self.check_model_is_fitted()
 
-        # Don't let the user shoot in her foot, by having p_error or global_p_error set in both
-        # configuration and in direct arguments
+        # Cast pandas, list or torch to numpy
+        X = check_array_and_assert(X)
+
+        # p_error or global_p_error should not be set in both the configuration and direct arguments
         check_there_is_no_p_error_options_in_configuration(configuration)
 
-        # Call the compilation backend to produce the FHE inference circuit
-        circuit = self.quantized_module_.compile(
-            quantized_numpy_inputset,
+        # Find the right way to set parameters for compiler, depending on the way we want to default
+        p_error, global_p_error = manage_parameters_for_pbs_errors(p_error, global_p_error)
+
+        # Quantize the inputs
+        q_X = self.quantize_input(X)
+
+        # Generate the compilation inputset with proper dimensions
+        inputset = _get_inputset_generator(q_X)
+
+        # Retrieve the compiler instance
+        module_to_compile = self._get_module_to_compile()
+
+        # Compiling using a QuantizedModule requires different steps and should not be done here
+        assert isinstance(module_to_compile, Compiler), (
+            "Wrong module to compile. Expected to be of type `Compiler` but got "
+            f"{type(module_to_compile)}."
+        )
+
+        self.fhe_circuit = module_to_compile.compile(
+            inputset,
             configuration=configuration,
-            compilation_artifacts=compilation_artifacts,
+            artifacts=artifacts,
             show_mlir=show_mlir,
-            use_virtual_lib=use_virtual_lib,
             p_error=p_error,
             global_p_error=global_p_error,
-            verbose_compilation=verbose_compilation,
+            verbose=verbose,
         )
 
-        succ = list(circuit.graph.graph.successors(circuit.graph.input_nodes[0]))
+        self._is_compiled = True
+
+        assert isinstance(self.fhe_circuit, Circuit)
+        return self.fhe_circuit
+
+    @abstractmethod
+    def _inference(self, q_X: numpy.ndarray) -> numpy.ndarray:
+        """Inference function to consider when executing in the clear.
+
+        Args:
+            q_X (numpy.ndarray): The quantized input values.
+
+        Returns:
+            numpy.ndarray: The quantized predicted values.
+        """
+
+    def predict(self, X: Data, fhe: Union[FheMode, str] = FheMode.DISABLE) -> numpy.ndarray:
+        """Predict values for X, in FHE or in the clear.
+
+        Args:
+            X (Data): The input values to predict, as a Numpy array, Torch tensor, Pandas DataFrame
+                or List.
+            fhe (Union[FheMode, str]): The mode to use for prediction.
+                Can be FheMode.DISABLE for Concrete ML python inference,
+                FheMode.SIMULATE for FHE simulation and FheMode.EXECUTE for actual FHE execution.
+                Can also be the string representation of any of these values.
+                Default to FheMode.DISABLE.
+
+        Returns:
+            np.ndarray: The predicted values for X.
+        """
         assert_true(
-            not any(s.converted_to_table_lookup for s in succ),
-            "The compiled circuit"
-            " applies lookup tables on input nodes, please check the underlying nn.Module.",
+            FheMode.is_valid(fhe),
+            "`fhe` mode is not supported. Expected one of 'disable' (resp. FheMode.DISABLE), "
+            "'simulate' (resp. FheMode.SIMULATE) or 'execute' (resp. FheMode.EXECUTE). Got "
+            f"{fhe}",
+            ValueError,
         )
 
-        return circuit
+        # Check that the model is properly fitted
+        self.check_model_is_fitted()
 
-    def fit(self, X, y, **fit_params):
-        """Initialize and fit the module.
+        # Ensure inputs are 2D
+        if isinstance(X, (numpy.ndarray, torch.Tensor)) and X.ndim == 1:
+            X = X.reshape((1, -1))
 
-        If the module was already initialized, by calling fit, the
-        module will be re-initialized (unless ``warm_start`` is True). In addition to the
-        torch training step, this method performs quantization of the trained torch model.
+        # Check that X's type and shape are supported
+        X = check_array_and_assert(X)
+
+        # Quantize the input
+        q_X = self.quantize_input(X)
+
+        # If the inference is executed in FHE or simulation mode
+        if fhe in ["simulate", "execute"]:
+            # Check that the model is properly compiled
+            self.check_model_is_compiled()
+
+            q_y_pred_list = []
+            for q_X_i in q_X:
+                # Expected encrypt_run_decrypt output shape is (1, n_features) while q_X_i
+                # is of shape (n_features,)
+                q_X_i = numpy.expand_dims(q_X_i, 0)
+
+                # Disable mypy's union attribute error as we already check that fhe_circuit is not
+                # None using check_model_is_compiled
+                q_y_pred_i = (
+                    self.fhe_circuit.simulate(q_X_i)  # type: ignore[union-attr]
+                    if fhe == "simulate"
+                    else self.fhe_circuit.encrypt_run_decrypt(q_X_i)  # type: ignore[union-attr]
+                )
+                q_y_pred_list.append(q_y_pred_i[0])
+
+            q_y_pred = numpy.array(q_y_pred_list)
+
+        # Else, the prediction is simulated in the clear
+        else:
+            q_y_pred = self._inference(q_X)
+
+        # Dequantize the predicted values in the clear
+        y_pred = self.dequantize_output(q_y_pred)
+
+        return y_pred
+
+    # pylint: disable-next=no-self-use
+    def post_processing(self, y_preds: numpy.ndarray) -> numpy.ndarray:
+        """Apply post-processing to the dequantized predictions.
+
+        This post-processing step can include operations such as applying the sigmoid or softmax
+        function for classifiers, or summing an ensemble's outputs. These steps are done in the
+        clear because of current technical constraints. They most likely will be integrated in the
+        FHE computations in the future.
+
+        For some simple models such a linear regression, there is no post-processing step but the
+        method is kept to make the API consistent for the client-server API. Other models might
+        need to use attributes stored in `post_processing_params`.
 
         Args:
-            X : training data
-                By default, you should be able to pass:
-                * numpy arrays
-                * torch tensors
-                * pandas DataFrame or Series
-            y (numpy.ndarray): labels associated with training data
-            **fit_params: additional parameters that can be used during training, these are passed
-                to the torch training interface
+            y_preds (numpy.ndarray): The dequantized predictions to post-process.
 
         Returns:
-            self: the trained quantized estimator
+            numpy.ndarray: The post-processed predictions.
         """
-        # Reset the quantized module since quantization is lost during refit
-        # This will make the .infer() function call into the Torch nn.Module
-        # Instead of the quantized module
-        self.quantized_module_ = None
-        X, y = check_X_y_and_assert(X, y, multi_output=len(y.shape) > 1)
+        return y_preds
 
-        # Call skorch fit that will train the network
-        super().fit(X, y, **fit_params)
+    @abstractmethod
+    def dump_dict(self) -> Dict[str, Any]:
+        """Dump the object as a dict.
 
-        # Export the brevitas model to ONNX
-        output_onnx_file_path = Path(tempfile.mkstemp(suffix=".onnx")[1])
+        Returns:
+            Dict[str, Any]: a dict representing the object
+        """
 
-        BrevitasONNXManager.export(
-            self.base_module_to_compile,
-            input_shape=X[[0], ::].shape,
-            export_path=str(output_onnx_file_path),
-            keep_initializers_as_inputs=False,
-            opset_version=OPSET_VERSION_FOR_ONNX_EXPORT,
-        )
+    def dumps(self) -> str:
+        """Dump itelf to a string.
 
-        onnx_model = onnx.load(output_onnx_file_path)
+        Returns:
+            metadata (str): string of serialized object
+        """
+        metadata: Dict[str, Any] = self.dump_dict()
+        return json.dumps(metadata, cls=CustomEncoder)
 
-        output_onnx_file_path.unlink()
+    def dump(self, file: IO[str]) -> None:
+        """Dump itelf to a file.
 
-        # Create corresponding numpy model
-        numpy_model = NumpyModule(onnx_model, torch.tensor(X[[0], ::]))
+        Args:
+            file (IO[str]): file of where to dump.
+        """
+        metadata: Dict[str, Any] = self.dump_dict()
+        json.dump(metadata, file, cls=CustomEncoder)
 
-        self._onnx_model_ = numpy_model.onnx_model
+    @classmethod
+    @abstractmethod
+    def load_dict(cls, metadata: Dict[str, Any]) -> BaseEstimator:
+        """Load itelf from a dict.
 
-        # Set the quantization bits for import
+        Args:
+            metadata (Dict[str, Any]): dict of metadata of the object
 
-        # Note that the ONNXConverter will use a default value for network input bits
-        # Furthermore, Brevitas ONNX contains bitwidths in the ONNX file
-        # which override the bitwidth that we pass here
+        Returns:
+            BaseEstimator: the loaded object
+        """
 
-        # Thus, this parameter, set by the inheriting classes, such as NeuralNetClassifier
-        # is only used to check consistency during import (onnx file vs import)
-        n_bits = self.n_bits_quant
+    @classmethod
+    def load(cls, file: IO[str]) -> BaseEstimator:
+        """Load itelf from a file.
 
-        # Import the quantization aware trained model
-        qat_model = PostTrainingQATImporter(n_bits, numpy_model, is_signed=True)
+        Args:
+            file (IO[str]): file of serialized object
 
-        self.quantized_module_ = qat_model.quantize_module(X)
+        Returns:
+            BaseEstimator: the loaded object
+        """
+        metadata: Dict[str, Any] = json.load(file)
+        return cls.load_dict(metadata=metadata)
 
-        # Set post-processing params
-        self._update_post_processing_params()
-        return self
+    @classmethod
+    def loads(cls, metadata: str) -> BaseEstimator:
+        """Load itelf from a string.
 
-    def _update_post_processing_params(self):
-        """Update the post-processing parameters."""
-        params = self._get_predict_nonlinearity()  # type: ignore
-        if isinstance(params, functools.partial):
-            post_processing_function_name = params.func.__name__
-            post_processing_function_keywords = params.keywords
-        else:
-            post_processing_function_name = params.__name__
-            post_processing_function_keywords = {}
-        post_processing_params: Dict[str, Any] = {}
-        post_processing_params["post_processing_function_name"] = post_processing_function_name
-        post_processing_params[
-            "post_processing_function_keywords"
-        ] = post_processing_function_keywords
-        self.post_processing_params = post_processing_params
+        Args:
+            metadata (str): serialized object
+
+        Returns:
+            BaseEstimator: the loaded object
+        """
+        _metadata: Dict = json.loads(metadata)
+        return cls.load_dict(metadata=_metadata)
+
+
+# This class only is an equivalent of BaseEstimator applied to classifiers, therefore not all
+# methods are implemented and we need to disable pylint from checking that
+# pylint: disable-next=abstract-method
+class BaseClassifier(BaseEstimator):
+    """Base class for linear and tree-based classifiers in Concrete ML.
+
+    This class inherits from BaseEstimator and modifies some of its methods in order to align them
+    with classifier behaviors. This notably include applying a sigmoid/softmax post-processing to
+    the predicted values as well as handling a mapping of classes in case they are not ordered.
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        #: The classifier's different target classes. Is None if the model is not fitted.
+        self.target_classes_: Optional[numpy.ndarray] = None
+
+        #: The classifier's number of different target classes. Is None if the model is not fitted.
+        self.n_classes_: Optional[int] = None
+
+    def _set_post_processing_params(self):
+        super()._set_post_processing_params()
+        self.post_processing_params.update({"n_classes_": self.n_classes_})
+
+    def fit(self, X: Data, y: Target, **fit_parameters):
+        X, y = check_X_y_and_assert_multi_output(X, y)
 
-    # Disable pylint here because we add an additional argument to .predict,
-    # with respect to the base class .predict method.
-    # pylint: disable=arguments-differ
-    def predict(self, X, execute_in_fhe=False):
-        """Predict on user provided data.
+        # Retrieve the different target classes
+        classes = numpy.unique(y)
+        self.target_classes_ = classes
 
-        Predicts using the quantized clear or FHE classifier
+        # Compute the number of target classes
+        self.n_classes_ = len(classes)
+
+        # Make sure y contains at least two classes
+        assert_true(self.n_classes_ > 1, "You must provide at least 2 classes in y.")
+
+        # Change to composition in order to avoid diamond inheritance and indirect super() calls
+        # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/3249
+        return super().fit(X, y, **fit_parameters)  # type: ignore[safe-super]
+
+    def predict_proba(self, X: Data, fhe: Union[FheMode, str] = FheMode.DISABLE) -> numpy.ndarray:
+        """Predict class probabilities.
 
         Args:
-            X : input data, a numpy array of raw values (non quantized)
-            execute_in_fhe : whether to execute the inference in FHE or in the clear
+            X (Data): The input values to predict, as a Numpy array, Torch tensor, Pandas DataFrame
+                or List.
+            fhe (Union[FheMode, str]): The mode to use for prediction.
+                Can be FheMode.DISABLE for Concrete ML python inference,
+                FheMode.SIMULATE for FHE simulation and FheMode.EXECUTE for actual FHE execution.
+                Can also be the string representation of any of these values.
+                Default to FheMode.DISABLE.
 
         Returns:
-            y_pred : numpy ndarray with predictions
+            numpy.ndarray: The predicted class probabilities.
+        """
+        return super().predict(X, fhe=fhe)
+
+    def predict(self, X: Data, fhe: Union[FheMode, str] = FheMode.DISABLE) -> numpy.ndarray:
+        # Compute the predicted probabilities
+        y_proba = self.predict_proba(X, fhe=fhe)
+
+        # Retrieve the class with the highest probability
+        y_preds = numpy.argmax(y_proba, axis=1)
+
+        assert self.target_classes_ is not None, self._is_not_fitted_error_message()
+
+        return self.target_classes_[y_preds]
+
+    def post_processing(self, y_preds: numpy.ndarray) -> numpy.ndarray:
+        y_preds = super().post_processing(y_preds)
+
+        # Retrieve the number of target classes
+        n_classes_ = self.post_processing_params["n_classes_"]
+
+        # If the predictions only has one dimension (i.e. binary classification problem), apply the
+        # sigmoid operator
+        if n_classes_ == 2:
+            y_preds = numpy_sigmoid(y_preds)[0]
+
+            # If the prediction array is 1D (which happens with some models such as XGBCLassifier
+            # models), transform the output into a 2D array [1-p, p], with p the initial
+            # output probabilities
+            if y_preds.ndim == 1 or y_preds.shape[1] == 1:
+                y_preds = numpy.concatenate((1 - y_preds, y_preds), axis=1)
+
+        # Else, apply the softmax operator
+        else:
+            y_preds = numpy_softmax(y_preds)[0]
+
+        return y_preds
+
+
+# QNNs do not support serialization yet
+# FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/3134
+# pylint: disable-next=abstract-method
+class QuantizedTorchEstimatorMixin(BaseEstimator):
+    """Mixin that provides quantization for a torch module and follows the Estimator API."""
 
+    def __init_subclass__(cls):
+        for klass in cls.__mro__:
+            # pylint: disable-next=protected-access
+            if getattr(klass, "_is_a_public_cml_model", False):
+                _NEURALNET_MODELS.add(cls)
+                _ALL_SKLEARN_MODELS.add(cls)
+
+    def __init__(self):
+        #: The quantized module used to store the quantized parameters. Is empty if the model is
+        #: not fitted.
+        self.quantized_module_ = QuantizedModule()
+
+        #: The input dimension in the underlying model
+        self.module__input_dim: Optional[int] = None
+
+        #: The number of outputs in the underlying model
+        self.module__n_outputs: Optional[int] = None
+
+        super().__init__()
+
+    @property
+    def base_module(self) -> SparseQuantNeuralNetwork:
+        """Get the Torch module.
+
+        Returns:
+            SparseQuantNeuralNetwork: The fitted underlying module.
         """
-        # By default, just return the result of predict_proba
-        # which for linear models with no non-linearity applied simply returns
-        # the decision function value
-        return self.predict_proba(X, execute_in_fhe=execute_in_fhe)
+        assert self.sklearn_model is not None, self._sklearn_model_is_not_fitted_error_message()
 
-    def predict_proba(self, X, execute_in_fhe=False):
-        """Predict on user provided data, returning probabilities.
+        return self.sklearn_model.module_
 
-        Predicts using the quantized clear or FHE classifier
+    @property
+    def input_quantizers(self) -> List[UniformQuantizer]:
+        """Get the input quantizers.
 
-        Args:
-            X : input data, a numpy array of raw values (non quantized)
-            execute_in_fhe : whether to execute the inference in FHE or in the clear
+        Returns:
+            List[UniformQuantizer]: The input quantizers.
+        """
+        return self.quantized_module_.input_quantizers
+
+    @input_quantizers.setter
+    def input_quantizers(self, value: List[UniformQuantizer]) -> None:
+        self.quantized_module_.input_quantizers = value
+
+    @property
+    def output_quantizers(self) -> List[UniformQuantizer]:
+        """Get the output quantizers.
 
         Returns:
-            y_pred : numpy ndarray with probabilities (if applicable)
+            List[UniformQuantizer]: The output quantizers.
+        """
+        return self.quantized_module_.output_quantizers
 
-        Raises:
-            ValueError: if the estimator was not yet trained or compiled
+    @output_quantizers.setter
+    def output_quantizers(self, value: List[UniformQuantizer]) -> None:
+        self.quantized_module_.output_quantizers = value
+
+    @property
+    def fhe_circuit(self) -> Circuit:
+        return self.quantized_module_.fhe_circuit
+
+    @fhe_circuit.setter
+    def fhe_circuit(self, value: Circuit) -> None:
+        self.quantized_module_.fhe_circuit = value
+
+    def get_params(self, deep: bool = True) -> dict:
+        """Get parameters for this estimator.
+
+        This method is overloaded in order to make sure that auto-computed parameters are not
+        considered when cloning the model (e.g during a GridSearchCV call).
+
+        Args:
+            deep (bool): If True, will return the parameters for this estimator and
+                contained subobjects that are estimators.
+
+        Returns:
+            params (dict): Parameter names mapped to their values.
         """
-        if execute_in_fhe:
-            if self.quantized_module_ is None:
-                raise ValueError(
-                    "The classifier needs to be calibrated before compilation,"
-                    " please call .fit() first!"
-                )
-            if not self.quantized_module_.is_compiled:
-                raise ValueError(
-                    "The classifier is not yet compiled to FHE, please call .compile() first"
-                )
+        # Retrieve the Skorch estimator's init parameters
+        # Here, the `get_params` method is the `NeuralNet.get_params` method from Skorch, which
+        # will become available once a subclass inherits from it. We therefore disable both pylint
+        # and mypy as this behavior is expected
+        # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/3373
+        # pylint: disable-next=no-member
+        params = super().get_params(deep)  # type: ignore[misc]
 
-            # Run over each element of X individually and aggregate predictions in a vector
-            if X.ndim == 1:
-                X = X.reshape((1, -1))
-            X = check_array_and_assert(X)
-            y_pred = None
-            for idx, x in enumerate(X):
-                q_x = self.quantized_module_.quantize_input(x).reshape(1, -1)
-                q_pred = self.quantized_module_.forward_fhe.encrypt_run_decrypt(q_x)
-                if y_pred is None:
-                    assert_true(
-                        isinstance(q_pred, numpy.ndarray),
-                        f"bad type {q_pred}, expected np.ndarray",
-                    )
-                    # pylint is lost: Instance of 'tuple' has no 'size' member (no-member)
-                    # because it doesn't understand the Union in encrypt_run_decrypt
-                    # pylint: disable=no-member
-                    y_pred = numpy.zeros((X.shape[0], q_pred.size), numpy.float32)
-                    # pylint: enable=no-member
-                y_pred[idx, :] = q_pred
-            y_pred = self.post_processing(y_pred)
-            return y_pred
-
-        # For prediction in the clear we call the super class which, in turn,
-        # will end up calling .infer of this class
-        return super().predict_proba(X).astype(numpy.float32)
+        # Remove `module` since it is automatically set to SparseQuantNeuralNetImpl. Therefore,
+        # we don't need to pass module again when cloning this estimator
+        params.pop("module", None)
 
-    # pylint: enable=arguments-differ
+        # Remove the parameters that are auto-computed by `fit` as well
+        for kwarg in QNN_AUTO_KWARGS:
+            params.pop(kwarg, None)
 
-    def fit_benchmark(self, X: numpy.ndarray, y: numpy.ndarray, *args, **kwargs) -> Tuple[Any, Any]:
-        """Fit the quantized estimator as well as its equivalent float estimator.
+        return params
 
-        This function returns both the quantized estimator (itself) as well as its non-quantized
-        (float) equivalent, which are both trained separately. This is useful in order
-        to compare performances between quantized and fp32 versions.
+    def get_sklearn_params(self, deep: bool = True) -> Dict:
+        # Retrieve the Skorch estimator's init parameters
+        # Here, the `get_params` method is the `NeuralNet.get_params` method from Skorch, which
+        # will become available once a subclass inherits from it. We therefore disable both pylint
+        # and mypy as this behavior is expected
+        # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/3373
+        # pylint: disable-next=no-member
+        params = super().get_params(deep=deep)  # type: ignore[misc]
+
+        # Set the quantized module to SparseQuantNeuralNetwork
+        params["module"] = SparseQuantNeuralNetwork
+
+        return params
+
+    def _fit_sklearn_model(self, X: Data, y: Target, **fit_parameters):
+        super()._fit_sklearn_model(X, y, **fit_parameters)
+
+        # Make pruning permanent by removing weights associated to pruned neurons
+        self.base_module.make_pruning_permanent()
+
+    def fit(self, X: Data, y: Target, **fit_parameters):
+        """Fit he estimator.
+
+        If the module was already initialized, the module will be re-initialized unless
+        `warm_start` is set to True. In addition to the torch training step, this method performs
+        quantization of the trained Torch model using Quantization Aware Training (QAT).
+
+        Values of dtype float64 are not supported and will be casted to float32.
 
         Args:
-            X : The training data
-                By default, you should be able to pass:
-                * numpy arrays
-                * torch tensors
-                * pandas DataFrame or Series
-            y (numpy.ndarray): The labels associated with the training data
-            *args: The arguments to pass to the sklearn linear model.
-            **kwargs: The keyword arguments to pass to the sklearn linear model.
+            X (Data): The training data, as a Numpy array, Torch tensor, Pandas DataFrame or List.
+            y (Target): The target data,  as a Numpy array, Torch tensor, Pandas DataFrame, Pandas
+                Series or List.
+            **fit_parameters: Keyword arguments to pass to Skorch's fit method.
 
         Returns:
-            self: The trained quantized estimator
-            fp32_model: The trained float equivalent estimator
+            The fitted estimator.
         """
-        # Fit the quantized estimator
-        self.fit(X, y, *args, **kwargs)
+        # Reset for double fit
+        self._is_fitted = False
 
-        # Retrieve the Skorch estimator's training parameters
-        # Following sklearn.base.clone's documentation, parameters are obtained with get_params()
-        # and then need to be copied using copy.deepcopy before passing them to the constructor
-        # Following sklearn.base.clone's documentation: "Clone does a deep copy of the model in an
-        # estimator without actually copying  attached data. It returns a new estimator with the
-        # same parameters that has not been fitted on any data."
-        # See: https://scikit-learn.org/stable/modules/generated/sklearn.base.clone.html
-        # We therefore obtained the parameters with get_params(), copy them using copy.deepcopy
-        # and then pass them to the constructor.
-        estimator_parameters = self.get_params_for_benchmark()
-
-        # The `module` parameter needs to be removed as we need to rebuild it separately
-        # This key is only present for NeuralNetClassifiers that don't fix the module type,
-        # otherwise, it may have already been removed (e.g. by FixedTypeSkorchNeuralNet)
-        estimator_parameters.pop("module", None)
-
-        # Copy the estimator's training parameters
-        for name, param in estimator_parameters.items():
-            estimator_parameters[name] = copy.deepcopy(param)
+        # Reset the quantized module since quantization is lost during refit
+        # This will make the .infer() function call into the Torch nn.Module
+        # Instead of the quantized module
+        self.quantized_module_ = QuantizedModule()
 
-        # Retrieve the estimator's float equivalent module
-        float_module = self._get_equivalent_float_module()
+        X, y = check_X_y_and_assert_multi_output(X, y)
 
-        # Instantiate the float estimator
-        skorch_estimator_type = self.base_estimator_type
-        float_estimator = skorch_estimator_type(float_module, **estimator_parameters)
+        # A helper for users so they don't need to import torch directly
+        args_to_convert_to_tensor = ["criterion__weight"]
+        for arg_name in args_to_convert_to_tensor:
+            if hasattr(self, arg_name):
+                attr_value = getattr(self, arg_name)
+                # The parameter could be a list, numpy.ndarray or tensor
+                if isinstance(attr_value, list):
+                    attr_value = numpy.asarray(attr_value, numpy.float32)
+
+                if isinstance(attr_value, numpy.ndarray):
+                    setattr(self, arg_name, torch.from_numpy(attr_value).float())
+
+                assert_true(
+                    isinstance(getattr(self, arg_name), torch.Tensor),
+                    f"Parameter `{arg_name}` must be a numpy.ndarray, list or torch.Tensor",
+                )
 
-        # Fit the float estimator
-        float_estimator.fit(X, y, *args, **kwargs)
+        # Fit the model by using Skorch's fit
+        self._fit_sklearn_model(X, y, **fit_parameters)
 
-        return self, float_estimator
+        # Export the brevitas model to ONNX
+        output_onnx_file_path = Path(tempfile.mkstemp(suffix=".onnx")[1])
+
+        BrevitasONNXManager.export(
+            self.base_module,
+            input_shape=X[[0], ::].shape,
+            export_path=str(output_onnx_file_path),
+            keep_initializers_as_inputs=False,
+            opset_version=OPSET_VERSION_FOR_ONNX_EXPORT,
+        )
+
+        onnx_model = onnx.load(str(output_onnx_file_path))
 
-    def _get_equivalent_float_module(self):
+        output_onnx_file_path.unlink()
+
+        # Create corresponding numpy model
+        numpy_model = NumpyModule(onnx_model, torch.tensor(X[[0], ::]))
+
+        self.onnx_model_ = numpy_model.onnx_model
+
+        # Set the quantization bits for import
+        # Note that the ONNXConverter will use a default value for network input bits
+        # Furthermore, Brevitas ONNX contains bitwidths in the ONNX file
+        # which override the bitwidth that we pass here
+        # Thus, this parameter is only used to check consistency during import (onnx file vs import)
+        n_bits = self.base_module.n_a_bits
+
+        # Import the quantization aware trained model
+        qat_model = PostTrainingQATImporter(n_bits, numpy_model)
+
+        self.quantized_module_ = qat_model.quantize_module(X)
+
+        # Set post-processing params
+        self._set_post_processing_params()
+
+        self._is_fitted = True
+
+        return self
+
+    def _get_equivalent_float_module(self) -> torch.nn.Sequential:
         """Build a topologically equivalent Torch module that can be used on floating points.
 
         Returns:
-            float_module (nn.Sequential): The equivalent float module.
+            float_module (torch.nn.Sequential): The equivalent float module.
         """
         # Instantiate a new sequential module
         float_module = torch.nn.Sequential()
 
         layer_index = -1
 
         # Iterate over the model's sub-modules
-        for module in self.base_module_to_compile.features:
+        for module in self.base_module.features:
 
             # If the module is not a QuantIdentity, it's either a QuantLinear or an activation
             if not isinstance(module, qnn.QuantIdentity):
-
                 # If the module is a QuantLinear, replace it with a Linear module
                 if isinstance(module, qnn.QuantLinear):
                     layer_index += 1
 
                     linear_name = f"fc{layer_index}"
                     linear_layer = torch.nn.Linear(
                         module.in_features,
@@ -538,585 +972,461 @@
                 # added as well
                 else:
                     activation_name = f"act{layer_index}"
                     float_module.add_module(activation_name, module)
 
         return float_module
 
-
-class BaseTreeEstimatorMixin(sklearn.base.BaseEstimator):
-    """Mixin class for tree-based estimators.
-
-    A place to share methods that are used on all tree-based estimators.
-    """
-
-    n_bits: int
-    input_quantizers: List[UniformQuantizer]
-    output_quantizers: List[UniformQuantizer]
-    init_args: Dict[str, Any]
-    random_state: Optional[Union[numpy.random.RandomState, int]] = None  # pylint: disable=no-member
-    sklearn_alg: Callable[..., sklearn.base.BaseEstimator]
-    sklearn_model: sklearn.base.BaseEstimator
-    _tensor_tree_predict: Optional[Callable]
-    framework: str
-    fhe_circuit: Optional[Circuit] = None
-    _onnx_model_: Optional[onnx.ModelProto] = None
-    _is_a_public_cml_model: bool = False
-
-    def __init_subclass__(cls):
-        for klass in cls.__mro__:
-            # pylint: disable-next=protected-access
-            if hasattr(klass, "_is_a_public_cml_model") and klass._is_a_public_cml_model:
-                _TREE_MODELS.add(cls)
-                _ALL_SKLEARN_MODELS.add(cls)
-
-    def __init__(self, n_bits: int):
-        """Initialize the TreeBasedEstimatorMixin.
-
-        Args:
-            n_bits (int): number of bits used for quantization
-        """
-        self.n_bits = n_bits
-        self.input_quantizers = []
-        self.output_quantizers = []
-        self.fhe_circuit = None
-        self._onnx_model_ = None
-        self.post_processing_params: Dict[str, Any] = {}
-
-    @property
-    def onnx_model(self) -> onnx.ModelProto:
-        """Get the ONNX model.
-
-        .. # noqa: DAR201
+    def _get_equivalent_float_estimator(self) -> SkorchNeuralNet:
+        """Initialize a topologically equivalent estimator that can be used on floating points.
 
         Returns:
-           onnx.ModelProto: the ONNX model
+            float_estimator (SkorchNeuralNet): An instance of the equivalent float estimator.
         """
-        return self._onnx_model_
+        # Retrieve the Skorch estimator's init parameters
+        sklearn_params = self.get_params()
 
-    def quantize_input(self, X: numpy.ndarray):
-        """Quantize the input.
+        # Retrieve all parameters related to the module
+        module_param_names = [name for name in sklearn_params if "module__" in name]
 
-        Args:
-            X (numpy.ndarray): the input
+        # Remove all parameters related to the module
+        for name in module_param_names:
+            sklearn_params.pop(name, None)
 
-        Returns:
-            the quantized input
-        """
-        qX = numpy.zeros_like(X)
-        # Quantize using the learned quantization parameters for each feature
-        for i, q_x_ in enumerate(self.input_quantizers):
-            qX[:, i] = q_x_.quant(X[:, i])
-        return qX.astype(numpy.int64)
+        # Retrieve the estimator's float topological equivalent module
+        float_module = self._get_equivalent_float_module()
 
-    def dequantize_output(self, y_preds: numpy.ndarray):
-        """Dequantize the integer predictions.
+        # Instantiate the float estimator
+        float_estimator = self.sklearn_model_class(float_module, **sklearn_params)
 
-        Args:
-            y_preds (numpy.ndarray): the predictions
+        return float_estimator
 
-        Returns:
-            the dequantized predictions
-        """
-        # mypy
-        assert self.output_quantizers is not None
-        y_preds = self.output_quantizers[0].dequant(y_preds)
-        return y_preds
+    def fit_benchmark(
+        self, X: Data, y: Target, random_state: Optional[int] = None, **fit_parameters
+    ):
+        """Fit the quantized estimator as well as its equivalent float estimator.
 
-    def _update_post_processing_params(self):
-        """Update the post processing parameters."""
-        self.post_processing_params = {}
+        This function returns both the quantized estimator (itself) as well as its non-quantized
+        (float) equivalent, which are both trained separately. This method differs from the
+        BaseEstimator's `fit_benchmark` method as QNNs use QAT instead of PTQ. Hence, here, the
+        float model is topologically equivalent as we have less control over the influence of QAT
+        over the weights.
 
-    def fit_benchmark(
-        self,
-        X: numpy.ndarray,
-        y: numpy.ndarray,
-        *args,
-        random_state: Optional[int] = None,
-        **kwargs,
-    ) -> Tuple[Any, Any]:
-        """Fit the sklearn tree-based model and the FHE tree-based model.
+        Values of dtype float64 are not supported and will be casted to float32.
 
         Args:
-            X (numpy.ndarray): The input data.
-            y (numpy.ndarray): The target data.
-            random_state (Optional[Union[int, numpy.random.RandomState, None]]):
-                The random state. Defaults to None.
-            *args: args for super().fit
-            **kwargs: kwargs for super().fit
+            X (Data): The training data, as a Numpy array, Torch tensor, Pandas DataFrame or List.
+            y (Target): The target data,  as a Numpy array, Torch tensor, Pandas DataFrame Pandas
+                Series or List.
+            random_state (Optional[int]): The random state to use when fitting. However, Skorch
+                does not handle such a parameter and setting it will have no effect. Defaults
+                to None.
+            **fit_parameters: Keyword arguments to pass to Skorch's fit method.
 
         Returns:
-            Tuple[ConcreteEstimators, SklearnEstimators]:
-                                                The FHE and sklearn tree-based models.
+            The Concrete ML and equivalent Skorch fitted estimators.
         """
 
-        params = self.get_params()  # type: ignore
-        params.pop("n_bits", None)
+        assert (
+            random_state is None
+        ), "Neural Network models do not support random_state as a parameter when fitting."
 
-        # Make sure the random_state is set or both algorithms will diverge
-        # due to randomness in the training.
-        if random_state is not None:
-            params["random_state"] = random_state
-        elif self.random_state is not None:
-            params["random_state"] = self.random_state
-        else:
-            params["random_state"] = numpy.random.randint(0, 2**15)
+        # Fit the quantized estimator
+        self.fit(X, y, **fit_parameters)
 
-        # Train the sklearn model without X quantized
-        sklearn_model = self.sklearn_alg(**params)
-        sklearn_model.fit(X, y, *args, **kwargs)
-
-        # Train the FHE model
-        self.set_params(n_bits=self.n_bits, **params)
-        self.fit(X, y, *args, **kwargs)
-        return self, sklearn_model
+        # Instantiate the equivalent float estimator
+        float_estimator = self._get_equivalent_float_estimator()
 
-    def _execute_in_fhe(self, qX: numpy.ndarray) -> numpy.ndarray:
-        """Execute the FHE inference on the input data.
+        # Fit the float equivalent estimator
+        float_estimator.fit(X, y, **fit_parameters)
 
-        Args:
-            qX (numpy.ndarray): the input data quantized
+        return self, float_estimator
 
-        Returns:
-            numpy.ndarray: the prediction as ordinals
-        """
-        # Check that self.fhe_tree is not None
-        # mypy
-        assert self.fhe_circuit is not None, (
-            f"You must call {self.compile.__name__} "
-            f"before calling {self.predict.__name__} with execute_in_fhe=True."
-        )
-        # mypy
-        assert self.fhe_circuit is not None
+    def quantize_input(self, X: numpy.ndarray) -> numpy.ndarray:
+        self.check_model_is_fitted()
+        q_X = self.quantized_module_.quantize_input(X)
+
+        assert numpy.array(q_X).dtype == numpy.int64, "Inputs were not quantized to int64 values"
+        assert isinstance(q_X, numpy.ndarray)
+        return q_X
 
-        y_preds = []
-        for qX_i in qX:
-            # expected x shape is (n_features, n_samples)
-            qX_i = numpy.expand_dims(qX_i, 0)
-            fhe_pred = self.fhe_circuit.encrypt_run_decrypt(qX_i)
-            y_preds.append(fhe_pred)
-        y_preds_array = numpy.concatenate(y_preds, axis=-1)
+    def dequantize_output(self, q_y_preds: numpy.ndarray) -> numpy.ndarray:
+        self.check_model_is_fitted()
+        return self.quantized_module_.dequantize_output(q_y_preds)
 
-        return y_preds_array
+    def _get_module_to_compile(self) -> Union[Compiler, QuantizedModule]:
+        return self.quantized_module_
 
     def compile(
         self,
-        X: numpy.ndarray,
+        X: Data,
         configuration: Optional[Configuration] = None,
-        compilation_artifacts: Optional[DebugArtifacts] = None,
+        artifacts: Optional[DebugArtifacts] = None,
         show_mlir: bool = False,
-        use_virtual_lib: bool = False,
         p_error: Optional[float] = None,
         global_p_error: Optional[float] = None,
-        verbose_compilation: bool = False,
+        verbose: bool = False,
     ) -> Circuit:
-        """Compile the model.
+        # Reset for double compile
+        self._is_compiled = False
 
-        Args:
-            X (numpy.ndarray): the dequantized dataset
-            configuration (Optional[Configuration]): the options for
-                compilation
-            compilation_artifacts (Optional[DebugArtifacts]): artifacts object to fill
-                during compilation
-            show_mlir (bool): whether or not to show MLIR during the compilation
-            use_virtual_lib (bool): set to True to use the so called virtual lib
-                simulating FHE computation. Defaults to False
-            p_error (Optional[float]): probability of error of a single PBS
-            global_p_error (Optional[float]): probability of error of the full circuit. Not
-                simulated by the VL, i.e., taken as 0
-            verbose_compilation (bool): whether to show compilation information
-
-        Returns:
-            Circuit: the compiled Circuit.
+        # Check that the model is correctly fitted
+        self.check_model_is_fitted()
 
-        """
-        # Make sure that self.tree_predict is not None
-        assert_true(
-            self._tensor_tree_predict is not None, "You must fit the model before compiling it."
-        )
-
-        # mypy bug fix
-        assert self._tensor_tree_predict is not None
-        _tensor_tree_predict_proxy, parameters_mapping = generate_proxy_function(
-            self._tensor_tree_predict, ["inputs"]
-        )
-
-        X = self.quantize_input(X)
-        compiler = Compiler(
-            _tensor_tree_predict_proxy,
-            {parameters_mapping["inputs"]: "encrypted"},
-        )
-
-        # Don't let the user shoot in her foot, by having p_error or global_p_error set in both
-        # configuration and in direct arguments
-        check_there_is_no_p_error_options_in_configuration(configuration)
+        # Cast pandas, list or torch to numpy
+        X = check_array_and_assert(X)
 
-        # Find the right way to set parameters for compiler, depending on the way we want to default
-        p_error, global_p_error = manage_parameters_for_pbs_errors(p_error, global_p_error)
+        # Retrieve the module instance to compile
+        module_to_compile = self._get_module_to_compile()
 
-        self.fhe_circuit = compiler.compile(
-            (sample.reshape(1, sample.shape[0]) for sample in X),
+        # Compile the QuantizedModule
+        module_to_compile.compile(
+            X,
             configuration=configuration,
-            artifacts=compilation_artifacts,
+            artifacts=artifacts,
             show_mlir=show_mlir,
-            virtual=use_virtual_lib,
             p_error=p_error,
             global_p_error=global_p_error,
-            verbose=verbose_compilation,
+            verbose=verbose,
         )
-        # mypy
-        assert self.fhe_circuit is not None
-        output_graph = self.fhe_circuit.graph.ordered_outputs()
-        assert_true(
-            len(output_graph) == 1,
-            "graph has too many outputs",
-        )
-        dtype_output = output_graph[0].output.dtype
+
+        # Make sure that no avoidable TLUs are found in the built-in model
+        succ = list(self.fhe_circuit.graph.graph.successors(self.fhe_circuit.graph.input_nodes[0]))
         assert_true(
-            isinstance(dtype_output, Integer),
-            f"output is {dtype_output} but an Integer is expected.",
+            not any(s.converted_to_table_lookup for s in succ),
+            "The compiled circuit currently applies some lookup tables on input nodes but this "
+            "should be avoided. Please check the underlying nn.Module.",
         )
 
-        return self.fhe_circuit
-
+        self._is_compiled = True
 
-class BaseTreeRegressorMixin(BaseTreeEstimatorMixin, sklearn.base.RegressorMixin):
-    """Mixin class for tree-based regressors.
+        return self.fhe_circuit
 
-    A place to share methods that are used on all tree-based regressors.
-    """
+    def _inference(self, q_X: numpy.ndarray) -> numpy.ndarray:
+        self.check_model_is_fitted()
 
-    _is_a_public_cml_model: bool = False
+        return self.quantized_module_.quantized_forward(q_X)
 
-    def __init_subclass__(cls):
-        for klass in cls.__mro__:
-            # pylint: disable-next=protected-access
-            if hasattr(klass, "_is_a_public_cml_model") and klass._is_a_public_cml_model:
-                _TREE_MODELS.add(cls)
-                _ALL_SKLEARN_MODELS.add(cls)
+    def post_processing(self, y_preds: numpy.ndarray) -> numpy.ndarray:
+        # Cast the predictions to float32 in order to match Torch's softmax outputs
+        return y_preds.astype(numpy.float32)
 
-    def fit(self, X, y: numpy.ndarray, **kwargs) -> Any:
-        """Fit the tree-based estimator.
+    def prune(self, X: Data, y: Target, n_prune_neurons_percentage: float, **fit_params):
+        """Prune a copy of this Neural Network model.
 
-        Args:
-            X : training data
-                By default, you should be able to pass:
-                * numpy arrays
-                * torch tensors
-                * pandas DataFrame or Series
-            y (numpy.ndarray): The target data.
-            **kwargs: args for super().fit
+        This can be used when the number of neurons on the hidden layers is too high. For example,
+        when creating a Neural Network model with `n_hidden_neurons_multiplier` high (3-4), it
+        can be used to speed up the model inference in FHE. Many times, up to 50% of
+        neurons can be pruned without losing accuracy, when using this function to fine-tune
+        an already trained model with good accuracy. This method should be used
+        once good accuracy is obtained.
+
+        Args:
+            X (Data): The training data, as a Numpy array, Torch tensor, Pandas DataFrame or List.
+            y (Target): The target data,  as a Numpy array, Torch tensor, Pandas DataFrame Pandas
+                Series or List.
+            n_prune_neurons_percentage (float): The percentage of neurons to remove. A value of
+                0 (resp. 1.0) means no (resp. all) neurons will be removed.
+            fit_params: Additional parameters to pass to the underlying nn.Module's forward method.
 
         Returns:
-            Any: The fitted model.
+            A new pruned copy of the Neural Network model.
+
+        Raises:
+            ValueError: If the model has not been trained or has already been pruned.
         """
-        X, y = check_X_y_and_assert(X, y, multi_output=len(y.shape) > 1)
+        self.check_model_is_fitted()
 
-        # mypy
-        assert self.n_bits is not None
+        if self.base_module.n_prune_neurons_percentage > 0.0:
+            raise ValueError(
+                "Cannot apply structured pruning optimization to an already pruned model"
+            )
 
-        qX = numpy.zeros_like(X)
-        self.input_quantizers = []
+        if n_prune_neurons_percentage >= 1.0 or n_prune_neurons_percentage < 0:
+            raise ValueError(
+                f"Valid values for `n_prune_neurons_percentage` are in the [0..1) range, but "
+                f"{n_prune_neurons_percentage} was given."
+            )
 
-        # Quantization of each feature in X
-        for i in range(X.shape[1]):
-            q_x_ = QuantizedArray(n_bits=self.n_bits, values=X[:, i]).quantizer
-            self.input_quantizers.append(q_x_)
-            qX[:, i] = q_x_.quant(X[:, i])
+        pruned_model = clone(self)
 
-        # Initialize the sklearn model
-        params = self.get_params()
-        params.pop("n_bits", None)
+        # Copy the input/output dims, as they are kept constant. These
+        # are usually computed by .fit, but here we want to manually instantiate the model
+        # before .fit() in order to fine-tune the original model
+        pruned_model.module__input_dim = self.module__input_dim
+        pruned_model.module__n_outputs = self.module__n_outputs
 
-        self.sklearn_model = self.sklearn_alg(**params)
+        # Create .module_ if the .module is a class (not an instance)
+        pruned_model.sklearn_model.initialize()
 
-        self.sklearn_model.fit(qX, y, **kwargs)
-        self._update_post_processing_params()
+        # Deactivate the default pruning
+        pruned_model.base_module.make_pruning_permanent()
 
-        # Tree ensemble inference to numpy
-        self._tensor_tree_predict, self.output_quantizers, self._onnx_model_ = tree_to_numpy(
-            self.sklearn_model,
-            qX[:1],
-            framework=self.framework,
-            output_n_bits=self.n_bits,
-            task=Task.REGRESSION,
-        )
-        return self
+        # Load the original model
+        pruned_model.base_module.load_state_dict(self.base_module.state_dict())
 
-    def post_processing(self, y_preds: numpy.ndarray) -> numpy.ndarray:
-        """Apply post-processing to the predictions.
+        # Set the new pruning amount
+        pruned_model.base_module.n_prune_neurons_percentage = n_prune_neurons_percentage
 
-        Args:
-            y_preds (numpy.ndarray): The predictions.
+        # Enable pruning again, this time with structured pruning
+        pruned_model.base_module.enable_pruning()
 
-        Returns:
-            numpy.ndarray: The post-processed predictions.
-        """
-        y_preds = self.dequantize_output(y_preds)
+        # The .module_ was initialized manually, prevent .fit (for both Skorch and Concrete ML)
+        # from creating a new one
+        # Setting both attributes could be avoided by initializing `sklearn_model` in __init__
+        # # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/3373
+        pruned_model.warm_start = True
+        pruned_model.sklearn_model.warm_start = True
 
-        # Sum all tree outputs.
-        # FIXME Remove this once #451 is done :
-        # https://github.com/zama-ai/concrete-ml-internal/issues/451
-        y_preds = numpy.sum(y_preds, axis=0)
-        assert_true(y_preds.ndim == 2, "y_preds should be a 2D array")
+        # Now, fine-tune the original module with structured pruning
+        pruned_model.fit(X, y, **fit_params)
 
-        # FIXME transpose workaround see #931
-        # https://github.com/zama-ai/concrete-ml-internal/issues/931
-        y_preds = numpy.transpose(y_preds)
-        return y_preds
+        return pruned_model
 
-    def predict(self, X: numpy.ndarray, execute_in_fhe: bool = False) -> numpy.ndarray:
-        """Predict the probability.
 
-        Args:
-            X (numpy.ndarray): The input data.
-            execute_in_fhe (bool): Whether to execute in FHE. Defaults to False.
-
-        Returns:
-            numpy.ndarray: The predicted probabilities.
-        """
-
-        X = check_array_and_assert(X)
-
-        # mypy
-        assert self._tensor_tree_predict is not None
-        qX = self.quantize_input(X)
-        if execute_in_fhe:
-            y_preds = self._execute_in_fhe(qX)
-        else:
-            y_preds = self._tensor_tree_predict(qX)[0]
-        y_preds = self.post_processing(y_preds)
-        return y_preds
-
-
-class BaseTreeClassifierMixin(BaseTreeEstimatorMixin, sklearn.base.ClassifierMixin):
-    """Mixin class for tree-based classifiers.
+class BaseTreeEstimatorMixin(BaseEstimator, sklearn.base.BaseEstimator, ABC):
+    """Mixin class for tree-based estimators.
 
-    A place to share methods that are used on all tree-based classifiers.
+    This class inherits from sklearn.base.BaseEstimator in order to have access to Scikit-Learn's
+    `get_params` and `set_params` methods.
     """
 
-    classes_: numpy.ndarray
-    n_classes_: int
-    class_mapping_: Optional[Dict[int, int]]
+    #: Model's base framework used, either 'xgboost' or 'sklearn'. Is set for each subclasses.
+    framework: str
 
-    def fit(self, X, y: numpy.ndarray, **kwargs) -> Any:
-        """Fit the tree-based estimator.
+    def __init_subclass__(cls):
+        for klass in cls.__mro__:
+            # pylint: disable-next=protected-access
+            if getattr(klass, "_is_a_public_cml_model", False):
+                _TREE_MODELS.add(cls)
+                _ALL_SKLEARN_MODELS.add(cls)
 
-        Args:
-            X : training data
-                By default, you should be able to pass:
-                * numpy arrays
-                * torch tensors
-                * pandas DataFrame or Series
-            y (numpy.ndarray): The target data.
-            **kwargs: args for super().fit
+    def __init__(self, n_bits: int):
+        """Initialize the TreeBasedEstimatorMixin.
 
-        Returns:
-            Any: The fitted model.
+        Args:
+            n_bits (int): The number of bits used for quantization.
         """
-        X, y = check_X_y_and_assert(X, y, multi_output=len(y.shape) > 1)
-
-        self.classes_ = numpy.unique(y)
+        self.n_bits: int = n_bits
 
-        # Register the number of classes
-        self.n_classes_ = len(self.classes_)
+        #: The model's inference function. Is None if the model is not fitted.
+        self._tree_inference: Optional[Callable] = None
 
-        # Make sure y contains at least two classes.
-        assert_true(self.n_classes_ > 1, "You must provide at least 2 classes in y.")
+        BaseEstimator.__init__(self)
 
-        self.class_mapping_ = None
-        if not numpy.array_equal(numpy.arange(len(self.classes_)), self.classes_):
-            self.class_mapping_ = dict(enumerate(self.classes_))
+    def fit(self, X: Data, y: Target, **fit_parameters):
+        # Reset for double fit
+        self._is_fitted = False
 
-        # mypy
-        assert self.n_bits is not None
+        X, y = check_X_y_and_assert_multi_output(X, y)
 
-        qX = numpy.zeros_like(X)
+        q_X = numpy.zeros_like(X)
         self.input_quantizers = []
 
         # Quantization of each feature in X
         for i in range(X.shape[1]):
-            q_x_ = QuantizedArray(n_bits=self.n_bits, values=X[:, i]).quantizer
-            self.input_quantizers.append(q_x_)
-            qX[:, i] = q_x_.quant(X[:, i])
+            input_quantizer = QuantizedArray(n_bits=self.n_bits, values=X[:, i]).quantizer
+            self.input_quantizers.append(input_quantizer)
+            q_X[:, i] = input_quantizer.quant(X[:, i])
 
-        # Initialize the sklearn model
-        params = self.get_params()
-        params.pop("n_bits", None)
+        # Fit the Scikit-Learn model
+        self._fit_sklearn_model(q_X, y, **fit_parameters)
 
-        self.sklearn_model = self.sklearn_alg(**params)
+        # Set post-processing parameters
+        self._set_post_processing_params()
 
-        self.sklearn_model.fit(qX, y, **kwargs)
-        self._update_post_processing_params()
+        # Check that the underlying sklearn model has been set and fit
+        assert self.sklearn_model is not None, self._sklearn_model_is_not_fitted_error_message()
 
-        # Tree ensemble inference to numpy
-        self._tensor_tree_predict, self.output_quantizers, self._onnx_model_ = tree_to_numpy(
+        # Convert the tree inference with Numpy operators
+        self._tree_inference, self.output_quantizers, self.onnx_model_ = tree_to_numpy(
             self.sklearn_model,
-            qX[:1],
+            q_X[:1],
             framework=self.framework,
             output_n_bits=self.n_bits,
-            task=Task.CLASSIFICATION,
         )
+
+        self._is_fitted = True
+
         return self
 
-    def predict(self, X: numpy.ndarray, execute_in_fhe: bool = False) -> numpy.ndarray:
-        """Predict the class with highest probability.
+    def quantize_input(self, X: numpy.ndarray) -> numpy.ndarray:
+        self.check_model_is_fitted()
 
-        Args:
-            X (numpy.ndarray): The input data.
-            execute_in_fhe (bool): Whether to execute in FHE. Defaults to False.
+        q_X = numpy.zeros_like(X, dtype=numpy.int64)
 
-        Returns:
-            numpy.ndarray: The predicted target values.
-        """
-        X = check_array_and_assert(X)
+        # Quantize using the learned quantization parameters for each feature
+        for i, input_quantizer in enumerate(self.input_quantizers):
+            q_X[:, i] = input_quantizer.quant(X[:, i])
 
-        y_preds = self.predict_proba(X, execute_in_fhe=execute_in_fhe)
-        y_preds = numpy.argmax(y_preds, axis=1)
-        if self.class_mapping_ is not None:
-            y_preds = numpy.array([self.class_mapping_[y_pred] for y_pred in y_preds])
-        return y_preds
+        assert q_X.dtype == numpy.int64, "Inputs were not quantized to int64 values"
+        return q_X
 
-    def predict_proba(self, X: numpy.ndarray, execute_in_fhe: bool = False) -> numpy.ndarray:
-        """Predict the probability.
+    def dequantize_output(self, q_y_preds: numpy.ndarray) -> numpy.ndarray:
+        self.check_model_is_fitted()
 
-        Args:
-            X (numpy.ndarray): The input data.
-            execute_in_fhe (bool): Whether to execute in FHE. Defaults to False.
+        q_y_preds = self.output_quantizers[0].dequant(q_y_preds)
+        return q_y_preds
 
-        Returns:
-            numpy.ndarray: The predicted probabilities.
-        """
-        X = check_array_and_assert(X)
+    def _get_module_to_compile(self) -> Union[Compiler, QuantizedModule]:
+        assert self._tree_inference is not None, self._is_not_fitted_error_message()
 
-        # mypy
-        assert self._tensor_tree_predict is not None
-        qX = self.quantize_input(X)
-        if execute_in_fhe:
-            y_preds = self._execute_in_fhe(qX)
-        else:
-            y_preds = self._tensor_tree_predict(qX)[0]
-        y_preds = self.post_processing(y_preds)
-        return y_preds
+        # Generate the proxy function to compile
+        _tree_inference_proxy, parameters_mapping = generate_proxy_function(
+            self._tree_inference, ["inputs"]
+        )
 
-    def post_processing(self, y_preds: numpy.ndarray) -> numpy.ndarray:
-        """Apply post-processing to the predictions.
+        # Create the compiler instance
+        compiler = Compiler(
+            _tree_inference_proxy,
+            {parameters_mapping["inputs"]: "encrypted"},
+        )
 
-        Args:
-            y_preds (numpy.ndarray): The predictions.
+        return compiler
 
-        Returns:
-            numpy.ndarray: The post-processed predictions.
-        """
-        y_preds = self.dequantize_output(y_preds)
+    def compile(self, *args, **kwargs) -> Circuit:
+        BaseEstimator.compile(self, *args, **kwargs)
 
-        # Sum all tree outputs.
-        # FIXME Remove this once #451 is done :
-        # https://github.com/zama-ai/concrete-ml-internal/issues/451
-        y_preds = numpy.sum(y_preds, axis=0)
-        assert_true(y_preds.ndim == 2, "y_preds should be a 2D array")
+        # Check that the graph only has a single output
+        # Ignore mypy issue as `self.fhe_circuit` is set in the super
+        output_graph = self.fhe_circuit.graph.ordered_outputs()  # type: ignore[union-attr]
+        assert_true(
+            len(output_graph) == 1,
+            "graph has too many outputs",
+        )
+
+        # Check that the output is an integer
+        dtype_output = output_graph[0].output.dtype
+        assert_true(
+            isinstance(dtype_output, Integer),
+            f"output is {dtype_output} but an Integer is expected.",
+        )
+        assert self.fhe_circuit is not None
+        return self.fhe_circuit
+
+    def _inference(self, q_X: numpy.ndarray) -> numpy.ndarray:
+        assert self._tree_inference is not None, self._is_not_fitted_error_message()
+
+        return self._tree_inference(q_X)[0]
+
+    def predict(self, X: Data, fhe: Union[FheMode, str] = FheMode.DISABLE) -> numpy.ndarray:
+        y_pred = BaseEstimator.predict(self, X, fhe=fhe)
+        y_pred = self.post_processing(y_pred)
+        return y_pred
+
+    def post_processing(self, y_preds: numpy.ndarray) -> numpy.ndarray:
+        # Sum all tree outputs
+        # Remove the sum once we handle multi-precision circuits
+        # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/451
+        y_preds = numpy.sum(y_preds, axis=-1)
 
-        # FIXME transpose workaround see #931
-        # https://github.com/zama-ai/concrete-ml-internal/issues/931
-        y_preds = numpy.transpose(y_preds)
+        assert_true(y_preds.ndim == 2, "y_preds should be a 2D array")
         return y_preds
 
 
-# pylint: disable=invalid-name,too-many-instance-attributes
-class SklearnLinearModelMixin(sklearn.base.BaseEstimator):
-    """A Mixin class for sklearn linear models with FHE."""
+class BaseTreeRegressorMixin(BaseTreeEstimatorMixin, sklearn.base.RegressorMixin, ABC):
+    """Mixin class for tree-based regressors.
 
-    sklearn_alg: Callable[..., sklearn.base.BaseEstimator]
-    random_state: Optional[Union[numpy.random.RandomState, int]] = None  # pylint: disable=no-member
+    This class is used to create a tree-based regressor class that inherits from
+    sklearn.base.RegressorMixin, which essentially gives access to Scikit-Learn's `score` method
+    for regressors.
+    """
 
-    _is_a_public_cml_model: bool = False
+
+class BaseTreeClassifierMixin(
+    BaseClassifier, BaseTreeEstimatorMixin, sklearn.base.ClassifierMixin, ABC
+):
+    """Mixin class for tree-based classifiers.
+
+    This class is used to create a tree-based classifier class that inherits from
+    sklearn.base.ClassifierMixin, which essentially gives access to Scikit-Learn's `score` method
+    for classifiers.
+
+    Additionally, this class adjusts some of the tree-based base class's methods in order to make
+    them compliant with classification workflows.
+    """
+
+
+# pylint: disable=invalid-name,too-many-instance-attributes
+class SklearnLinearModelMixin(BaseEstimator, sklearn.base.BaseEstimator, ABC):
+    """A Mixin class for sklearn linear models with FHE.
+
+    This class inherits from sklearn.base.BaseEstimator in order to have access to Scikit-Learn's
+    `get_params` and `set_params` methods.
+    """
 
     def __init_subclass__(cls):
         for klass in cls.__mro__:
             # pylint: disable-next=protected-access
-            if hasattr(klass, "_is_a_public_cml_model") and klass._is_a_public_cml_model:
+            if getattr(klass, "_is_a_public_cml_model", False):
                 _LINEAR_MODELS.add(cls)
                 _ALL_SKLEARN_MODELS.add(cls)
 
-    def __init__(self, *args, n_bits: Union[int, Dict[str, int]] = 8, **kwargs):
+    def __init__(self, n_bits: Union[int, Dict[str, int]] = 8):
         """Initialize the FHE linear model.
 
         Args:
             n_bits (int, Dict[str, int]): Number of bits to quantize the model. If an int is passed
                 for n_bits, the value will be used for quantizing inputs and weights. If a dict is
                 passed, then it should contain "op_inputs" and "op_weights" as keys with
                 corresponding number of quantization bits so that:
                     - op_inputs : number of bits to quantize the input values
                     - op_weights: number of bits to quantize the learned parameters
                 Default to 8.
-            *args: The arguments to pass to the sklearn linear model.
-            **kwargs: The keyword arguments to pass to the sklearn linear model.
         """
-        super().__init__(*args, **kwargs)
         self.n_bits: Union[int, Dict[str, int]] = n_bits
-        self.post_processing_params: Dict[str, Any] = {}
-        self.fhe_circuit: Optional[Circuit] = None
-        self.input_quantizers: List[UniformQuantizer] = []
-        self.output_quantizers: List[UniformQuantizer] = []
-        self.weight_quantizers: List[UniformQuantizer] = []
-        self.onnx_model: onnx.ModelProto = None
-        self._output_scale: Optional[numpy.float64] = None
-        self._output_zero_point: Optional[int] = None
+
+        #: The quantizer to use for quantizing the model's weights
+        self._weight_quantizer: Optional[UniformQuantizer] = None
+
+        #: The model's quantized weights
         self._q_weights: Optional[numpy.ndarray] = None
+
+        #: The model's quantized bias
         self._q_bias: Optional[numpy.ndarray] = None
 
-    def fit(self, X, y: numpy.ndarray, *args, **kwargs) -> Any:
-        """Fit the FHE linear model.
+        BaseEstimator.__init__(self)
 
-        Args:
-            X : Training data
-                By default, you should be able to pass:
-                * numpy arrays
-                * torch tensors
-                * pandas DataFrame or Series
-            y (numpy.ndarray): The target data.
-            *args: The arguments to pass to the sklearn linear model.
-            **kwargs: The keyword arguments to pass to the sklearn linear model.
+    def _set_onnx_model(self, test_input: numpy.ndarray) -> None:
+        """Retrieve the model's ONNX graph using Hummingbird conversion.
 
-        Returns:
-            Any
+        Args:
+            test_input (numpy.ndarray): An input data used to trace the model execution.
         """
-        # Copy X
-        X = copy.deepcopy(X)
+        # Check that the underlying sklearn model has been set and fit
+        assert self.sklearn_model is not None, self._sklearn_model_is_not_fitted_error_message()
 
-        # LinearRegression handles multi-labels data
-        X, y = check_X_y_and_assert(X, y, multi_output=len(y.shape) > 1)
+        self.onnx_model_ = hb_convert(
+            self.sklearn_model,
+            backend="onnx",
+            test_input=test_input,
+            extra_config={"onnx_target_opset": OPSET_VERSION_FOR_ONNX_EXPORT},
+        ).model
 
-        # Retrieve sklearn's init parameters and remove the ones specific to Concrete-ML
-        params = self.get_params()  # type: ignore
-        params.pop("n_bits", None)
+        self._clean_graph()
+
+    def _clean_graph(self) -> None:
+        """Clean the ONNX graph from undesired nodes."""
+        assert self.onnx_model_ is not None, self._is_not_fitted_error_message()
+
+        # Remove cast operators as they are not needed
+        remove_node_types(onnx_model=self.onnx_model_, op_types_to_remove=["Cast"])
+
+    def fit(self, X: Data, y: Target, **fit_parameters):
+        # Reset for double fit
+        self._is_fitted = False
 
-        # Initialize the sklearn model
-        self.sklearn_model = self.sklearn_alg(**params)
+        # LinearRegression handles multi-labels data
+        X, y = check_X_y_and_assert_multi_output(X, y)
 
-        # Fit the sklearn model
-        self.sklearn_model.fit(X, y, *args, **kwargs)
+        # Fit the Scikit-Learn model
+        self._fit_sklearn_model(X, y, **fit_parameters)
 
-        # FIXME: Remove this when #1610 is done
-        # This workaround makes linear regressors be able to fit with fit_intercept set to False.
-        if not self.fit_intercept:
-            self.sklearn_model.intercept_ = numpy.array(self.sklearn_model.intercept_)
-
-        # These models are not natively supported by Hummingbird
-        # The trick is to hide their type to Hummingbird
-        # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/1473
-        # Open PR to hummingbird to add support
-        if self.sklearn_alg in {
-            sklearn.linear_model.Lasso,
-            sklearn.linear_model.Ridge,
-            sklearn.linear_model.ElasticNet,
-        }:
-            self.sklearn_model.__class__ = sklearn.linear_model.LinearRegression
-            self.n_jobs = None
-            self.sklearn_model.n_jobs = None
+        # Check that the underlying sklearn model has been set and fit
+        assert self.sklearn_model is not None, self._sklearn_model_is_not_fitted_error_message()
 
         # Retrieve the ONNX graph
         self._set_onnx_model(X)
 
         # Convert the n_bits attribute into a proper dictionary
         n_bits = get_n_bits_dict(self.n_bits)
 
@@ -1138,541 +1448,148 @@
         q_weights = QuantizedArray(
             n_bits=n_bits["op_weights"],
             values=numpy.expand_dims(weights, axis=1) if len(weights.shape) == 1 else weights,
             options=weight_options,
         )
         self._q_weights = q_weights.qvalues
         weight_quantizer = q_weights.quantizer
-        self.weight_quantizers.append(weight_quantizer)
+        self._weight_quantizer = weight_quantizer
 
         # mypy
         assert input_quantizer.scale is not None
         assert weight_quantizer.scale is not None
 
-        # Retrieve the scale and zero-point of the matmul's outputs, following the same steps from
+        # Compute the scale and zero-point of the matmul's outputs, following the same steps from
         # the QuantizedGemm operator, which are based on equations detailed in
         # https://arxiv.org/abs/1712.05877
-        self._output_scale = input_quantizer.scale * weight_quantizer.scale
-        self._output_zero_point = input_quantizer.zero_point * (
-            numpy.sum(self._q_weights, axis=0, keepdims=True)
-            - X.shape[1] * weight_quantizer.zero_point
+        output_quant_params = UniformQuantizationParameters(
+            scale=input_quantizer.scale * weight_quantizer.scale,
+            zero_point=input_quantizer.zero_point
+            * (
+                numpy.sum(self._q_weights, axis=0, keepdims=True)
+                - X.shape[1] * weight_quantizer.zero_point
+            ),
+            offset=0,
         )
 
-        # Updating post-processing parameters
-        self._update_post_processing_params()
+        output_quantizer = UniformQuantizer(params=output_quant_params, no_clipping=True)
 
         # Quantize the bias using the matmul's scale and zero-point, such that
         # q_bias = round((1/S)*bias + Z)
-        # Contrary to the QuantizedGemm operator which handles the bias term as a floating point
-        # (and thus fusing it with following TLUs), we need to quantize the bias term so that it
-        # matches the same range of values as the matmul's outputs.
-        self._q_bias = numpy.round(
-            self.sklearn_model.intercept_ / self._output_scale + self._output_zero_point
-        ).astype(numpy.int64)
-
-        return self
-
-    def fit_benchmark(
-        self,
-        X: numpy.ndarray,
-        y: numpy.ndarray,
-        *args,
-        random_state: Optional[int] = None,
-        **kwargs,
-    ) -> Tuple[Any, Any]:
-        """Fit the sklearn linear model and the FHE linear model.
-
-        Args:
-            X (numpy.ndarray): The input data.
-            y (numpy.ndarray): The target data.
-            random_state (Optional[Union[int, numpy.random.RandomState, None]]):
-                The random state. Defaults to None.
-            *args: The arguments to pass to the sklearn linear model.
-                or not (False). Default to False.
-            *args: Arguments for super().fit
-            **kwargs: Keyword arguments for super().fit
-
-        Returns:
-            Tuple[SklearnLinearModelMixin, sklearn.linear_model.LinearRegression]:
-                The FHE and sklearn LinearRegression.
-        """
+        self._q_bias = output_quantizer.quant(self.sklearn_model.intercept_)
 
-        # Retrieve sklearn's init parameters and remove the ones specific to Concrete-ML
-        params = self.get_params()  # type: ignore
-        params.pop("n_bits", None)
-
-        # Make sure the random_state is set or both algorithms will diverge
-        # due to randomness in the training.
-        if "random_state" in params:
-            if random_state is not None:
-                params["random_state"] = random_state
-            elif self.random_state is not None:
-                params["random_state"] = self.random_state
-            else:
-                params["random_state"] = numpy.random.randint(0, 2**15)
+        # Since the matmul and the bias both use the same scale and zero-points, we obtain that
+        # y = S*(q_y - 2*Z) when dequantizing the values. We therefore need to multiply the initial
+        # output zero_point by 2
+        assert output_quantizer.zero_point is not None
+        output_quantizer.zero_point *= 2
+        self.output_quantizers.append(output_quantizer)
 
-        # Train the sklearn model without X quantized
-        sklearn_model = self.sklearn_alg(**params)
-        sklearn_model.fit(X, y, *args, **kwargs)
+        # Updating post-processing parameters
+        self._set_post_processing_params()
 
-        # Train the FHE model
-        self.set_params(n_bits=self.n_bits, **params)
+        self._is_fitted = True
 
-        self.fit(X, y, *args, **kwargs)
+        return self
 
-        return self, sklearn_model
+    def quantize_input(self, X: numpy.ndarray) -> numpy.ndarray:
+        self.check_model_is_fitted()
+        q_X = self.input_quantizers[0].quant(X)
 
-    def compile(
-        self,
-        X: numpy.ndarray,
-        configuration: Optional[Configuration] = None,
-        compilation_artifacts: Optional[DebugArtifacts] = None,
-        show_mlir: bool = False,
-        use_virtual_lib: bool = False,
-        p_error: Optional[float] = None,
-        global_p_error: Optional[float] = None,
-        verbose_compilation: bool = False,
-    ) -> Circuit:
-        """Compile the FHE linear model.
+        assert q_X.dtype == numpy.int64, "Inputs were not quantized to int64 values"
+        return q_X
 
-        Args:
-            X (numpy.ndarray): The input data.
-            configuration (Optional[Configuration]): Configuration object
-                to use during compilation
-            compilation_artifacts (Optional[DebugArtifacts]): Artifacts object to fill during
-                compilation
-            show_mlir (bool): If set, the MLIR produced by the converter and which is
-                going to be sent to the compiler backend is shown on the screen, e.g., for debugging
-                or demo. Defaults to False.
-            use_virtual_lib (bool): Whether to compile using the virtual library that allows higher
-                bitwidths with simulated FHE computation. Defaults to False
-            p_error (Optional[float]): Probability of error of a single PBS
-            global_p_error (Optional[float]): probability of error of the full circuit. Not
-                simulated by the VL, i.e., taken as 0
-            verbose_compilation (bool): whether to show compilation information
+    def dequantize_output(self, q_y_preds: numpy.ndarray) -> numpy.ndarray:
+        self.check_model_is_fitted()
 
-        Returns:
-            Circuit: The compiled Circuit.
+        # Dequantize the output values
+        y_preds = self.output_quantizers[0].dequant(q_y_preds)
 
-        """
+        return y_preds
 
+    def _get_module_to_compile(self) -> Union[Compiler, QuantizedModule]:
+        # Define the inference function to compile.
+        # This function can neither be a class method nor a static one because self we want to avoid
+        # having self as a parameter while still being able to access some of its attribute
         def inference_to_compile(q_X: numpy.ndarray) -> numpy.ndarray:
             """Compile the circuit in FHE using only the inputs as parameters.
 
             Args:
                 q_X (numpy.ndarray): The quantized input data
 
             Returns:
                 numpy.ndarray: The circuit's outputs.
             """
-            # mypy
-            assert (
-                self.weight_quantizers and self._q_weights is not None and self._q_bias is not None
-            ), "The model is not fitted. Please run fit(...) on proper arguments first."
-
-            return self._inference(
-                q_X, self._q_weights, self._q_bias, self.weight_quantizers[0].zero_point
-            )
-
-        # mypy
-        assert (
-            self.input_quantizers
-        ), "The model is not fitted. Please run fit(...) on proper arguments first."
+            return self._inference(q_X)
 
-        # Quantize the inputs
-        q_X = self.input_quantizers[0].quant(X)
-
-        # Make the input set an generator yielding values with proper dimensions
-        inputset = _get_inputset_generator((q_X,), self.input_quantizers)
-
-        # Instantiate the compiler on the linear regression's inference
+        # Create the compiler instance
         compiler = Compiler(inference_to_compile, {"q_X": "encrypted"})
 
-        # Don't let the user shoot in her foot, by having p_error or global_p_error set in both
-        # configuration and in direct arguments
-        check_there_is_no_p_error_options_in_configuration(configuration)
-
-        # Find the right way to set parameters for compiler, depending on the way we want to default
-        p_error, global_p_error = manage_parameters_for_pbs_errors(p_error, global_p_error)
-
-        # Compile on the input set
-        self.fhe_circuit = compiler.compile(
-            inputset,
-            configuration=configuration,
-            artifacts=compilation_artifacts,
-            show_mlir=show_mlir,
-            virtual=use_virtual_lib,
-            p_error=p_error,
-            global_p_error=global_p_error,
-            verbose=verbose_compilation,
-        )
-
-        return self.fhe_circuit
-
-    def predict(self, X: numpy.ndarray, execute_in_fhe: bool = False) -> numpy.ndarray:
-        """Predict on user data.
+        return compiler
 
-        Predict on user data using either the quantized clear model,
-        implemented with tensors, or, if execute_in_fhe is set, using the compiled FHE circuit
+    def _inference(self, q_X: numpy.ndarray) -> numpy.ndarray:
+        assert self._weight_quantizer is not None, self._is_not_fitted_error_message()
 
-        Args:
-            X (numpy.ndarray): The input data
-            execute_in_fhe (bool): Whether to execute the inference in FHE
-
-        Returns:
-            numpy.ndarray: The prediction as ordinals
-        """
-
-        X = check_array_and_assert(X)
-
-        # mypy
-        # The model is fitted if and only if the model's input quantizer is initialized
-        assert (
-            self.input_quantizers
-        ), "The model is not fitted. Please run fit(...) on proper arguments first."
-
-        # Quantize the inputs
-        q_X = self.quantize_input(X)
-
-        # If the predictions are executed in FHE, we call the circuit on each sample
-        if execute_in_fhe:
-
-            # mypy
-            # Make sure the model is compiled
-            assert (
-                self.fhe_circuit is not None
-            ), "The model is not compiled. Please run compile(...) first."
-
-            q_y_preds_list = []
-            for q_X_i in q_X:
-                q_y_pred_i = self.fhe_circuit.encrypt_run_decrypt(q_X_i.reshape(1, q_X_i.shape[0]))
-                q_y_preds_list.append(q_y_pred_i[0])
-
-            q_y_preds = numpy.array(q_y_preds_list)
-
-        # If the predictions are not executed in FHE, we only need to call the inference
-        else:
-            # mypy
-            assert (
-                self.weight_quantizers and self._q_weights is not None and self._q_bias is not None
-            ), "The model is not fitted. Please run fit(...) on proper arguments first."
-
-            q_y_preds = self._inference(
-                q_X, self._q_weights, self._q_bias, self.weight_quantizers[0].zero_point
-            )
-
-        # Dequantize the outputs
-        y_preds = self.dequantize_output(q_y_preds)
-
-        return y_preds
-
-    def quantize_input(self, X: numpy.ndarray):
-        """Quantize the input.
-
-        Args:
-            X (numpy.ndarray): The input to quantize
-
-        Returns:
-            numpy.ndarray: The quantized input
-        """
-        return self.input_quantizers[0].quant(X)
-
-    def dequantize_output(self, q_y_preds: numpy.ndarray) -> numpy.ndarray:
-        """Dequantize the output.
-
-        Args:
-            q_y_preds (numpy.ndarray): The quantized output to dequantize
-
-        Returns:
-            numpy.ndarray: The dequantized output
-        """
-        # Retrieve the post-processing parameters
-        output_scale = self.post_processing_params["output_scale"]
-        output_zero_point = self.post_processing_params["output_zero_point"]
-
-        assert (
-            output_scale is not None and output_zero_point is not None
-        ), "The model is not fitted. Please run fit(...) on proper arguments first."
-
-        # Dequantize the output.
-        # Since the matmul and the bias both use the same scale and zero-points, we obtain that
-        # y = S*(q_y - 2*Z)
-        y_preds = output_scale * (q_y_preds - 2 * output_zero_point)
-        return y_preds
-
-    def post_processing(self, y_preds: numpy.ndarray) -> numpy.ndarray:
-        """Post-processing the quantized output.
-
-        For linear models, post-processing only considers a dequantization step.
-
-        Args:
-            y_preds (numpy.ndarray): The quantized outputs to post-process
-
-        Returns:
-            numpy.ndarray: The post-processed output
-        """
-        return self.dequantize_output(y_preds)
-
-    def _set_onnx_model(self, test_input: numpy.ndarray):
-        """Retrieve the model's ONNX graph using Hummingbird conversion.
-
-        Args:
-            test_input (numpy.ndarray): An input data used to trace the model execution.
-        """
-
-        assert_true(
-            self.sklearn_model is not None,
-            "The model is not fitted. Please run fit(...) on proper arguments first.",
-        )
-
-        self.onnx_model = hb_convert(
-            self.sklearn_model,
-            backend="onnx",
-            test_input=test_input,
-            extra_config={"onnx_target_opset": OPSET_VERSION_FOR_ONNX_EXPORT},
-        ).model
-
-        self.clean_graph()
-
-    def clean_graph(self):
-        """Clean the graph of the onnx model.
-
-        This will remove the Cast node in the model's onnx.graph since they have no use in
-        quantized or FHE models.
-        """
-        remove_node_types(onnx_model=self.onnx_model, op_types_to_remove=["Cast"])
-
-    def _update_post_processing_params(self):
-        """Update the post processing parameters."""
-
-        assert (
-            self._output_scale is not None and self._output_zero_point is not None
-        ), "The model is not fitted. Please run fit(...) on proper arguments first."
-
-        self.post_processing_params = {
-            "output_scale": self._output_scale,
-            "output_zero_point": self._output_zero_point,
-        }
-
-    @staticmethod
-    def _inference(
-        q_x: numpy.ndarray,
-        q_weights: numpy.ndarray,
-        q_bias: numpy.ndarray,
-        weight_zp: numpy.ndarray,
-    ) -> numpy.ndarray:
-        """Execute a linear inference.
-
-        Args:
-            q_x (numpy.ndarray): The quantized input data
-            q_weights (numpy.ndarray): The quantized weights
-            q_bias (numpy.ndarray): The quantized bias
-            weight_zp (int): Zero-point use for quantizing the weights
-
-        Returns:
-            numpy.ndarray: The predicted values.
-        """
         # Quantizing weights and inputs makes an additional term appear in the inference function
-        y_pred = q_x @ q_weights - weight_zp * numpy.sum(q_x, axis=1, keepdims=True)
-        y_pred += q_bias
+        y_pred = q_X @ self._q_weights - self._weight_quantizer.zero_point * numpy.sum(
+            q_X, axis=1, keepdims=True
+        )
+        y_pred += self._q_bias
         return y_pred
 
 
-class SklearnLinearClassifierMixin(SklearnLinearModelMixin):
-    """A Mixin class for sklearn linear classifiers with FHE."""
-
-    def post_processing(self, y_preds: numpy.ndarray, already_dequantized: bool = False):
-        """Post-processing the predictions.
-
-        This step may include a dequantization of the inputs if not done previously, in particular
-        within the client-server workflow.
-
-        Args:
-            y_preds (numpy.ndarray): The predictions to post-process.
-            already_dequantized (bool): Whether the inputs were already dequantized or not. Default
-                to False.
-
-        Returns:
-            numpy.ndarray: The post-processed predictions.
-        """
-
-        # If y_preds were already dequantized previously, there is no need to do so once again.
-        # This step is necessary for the client-server workflow as the post_processing method
-        # is directly called on the quantized outputs, contrary to the base class' predict method.
-        if not already_dequantized:
-            y_preds = self.dequantize_output(y_preds)
-
-        # If the predictions only has one dimension (i.e. binary classification problem), apply the
-        # sigmoid operator
-        if y_preds.shape[1] == 1:
-            y_preds = numpy_sigmoid(y_preds)[0]
-
-            # Transform in a 2d array where [1-p, p] is the output as scikit-learn only outputs 1
-            # value when considering 2 classes
-            y_preds = numpy.concatenate((1 - y_preds, y_preds), axis=1)
-
-        # Else, apply the softmax operator
-        else:
-            y_preds = numpy_softmax(y_preds)[0]
-
-        return y_preds
+class SklearnLinearRegressorMixin(SklearnLinearModelMixin, sklearn.base.RegressorMixin, ABC):
+    """A Mixin class for sklearn linear regressors with FHE.
 
-    def decision_function(self, X: numpy.ndarray, execute_in_fhe: bool = False) -> numpy.ndarray:
-        """Predict confidence scores for samples.
+    This class is used to create a linear regressor class that inherits from
+    sklearn.base.RegressorMixin, which essentially gives access to Scikit-Learn's `score` method
+    for regressors.
+    """
 
-        Args:
-            X (numpy.ndarray): Samples to predict.
-            execute_in_fhe (bool): If True, the inference will be executed in FHE. Default to False.
 
-        Returns:
-            numpy.ndarray: Confidence scores for samples.
-        """
-        y_preds = super().predict(X, execute_in_fhe=execute_in_fhe)
-        return y_preds
+class SklearnLinearClassifierMixin(
+    BaseClassifier, SklearnLinearModelMixin, sklearn.base.ClassifierMixin, ABC
+):
+    """A Mixin class for sklearn linear classifiers with FHE.
 
-    def predict_proba(self, X: numpy.ndarray, execute_in_fhe: bool = False) -> numpy.ndarray:
-        """Predict class probabilities for samples.
+    This class is used to create a linear classifier class that inherits from
+    sklearn.base.ClassifierMixin, which essentially gives access to Scikit-Learn's `score` method
+    for classifiers.
 
-        Args:
-            X (numpy.ndarray): Samples to predict.
-            execute_in_fhe (bool): If True, the inference will be executed in FHE. Default to False.
+    Additionally, this class adjusts some of the tree-based base class's methods in order to make
+    them compliant with classification workflows.
+    """
 
-        Returns:
-            numpy.ndarray: Class probabilities for samples.
-        """
-        y_preds = self.decision_function(X, execute_in_fhe=execute_in_fhe)
-        y_preds = self.post_processing(y_preds, already_dequantized=True)
-        return y_preds
+    def _clean_graph(self) -> None:
+        assert self.onnx_model_ is not None, self._is_not_fitted_error_message()
 
-    def predict(self, X: numpy.ndarray, execute_in_fhe: bool = False) -> numpy.ndarray:
-        """Predict on user data.
+        # Remove any operators following gemm, as they will be done in the clear
+        assert self.onnx_model_ is not None
+        clean_graph_after_node_op_type(self.onnx_model_, node_op_type="Gemm")
+        SklearnLinearModelMixin._clean_graph(self)
 
-        Predict on user data using either the quantized clear model, implemented with tensors, or,
-        if execute_in_fhe is set, using the compiled FHE circuit.
+    def decision_function(
+        self, X: Data, fhe: Union[FheMode, str] = FheMode.DISABLE
+    ) -> numpy.ndarray:
+        """Predict confidence scores.
 
         Args:
-            X (numpy.ndarray): Samples to predict.
-            execute_in_fhe (bool): If True, the inference will be executed in FHE. Default to False.
+            X (Data): The input values to predict, as a Numpy array, Torch tensor, Pandas DataFrame
+                or List.
+            fhe (Union[FheMode, str]): The mode to use for prediction.
+                Can be FheMode.DISABLE for Concrete ML python inference,
+                FheMode.SIMULATE for FHE simulation and FheMode.EXECUTE for actual FHE execution.
+                Can also be the string representation of any of these values.
+                Default to FheMode.DISABLE.
 
         Returns:
-            numpy.ndarray: The prediction as ordinals.
+            numpy.ndarray: The predicted confidence scores.
         """
-        y_preds = self.predict_proba(X, execute_in_fhe=execute_in_fhe)
-        y_preds = numpy.argmax(y_preds, axis=1)
+        # Here, we want to use SklearnLinearModelMixin's `predict` method as confidence scores are
+        # the dot product's output values, without any post-processing
+        y_preds = SklearnLinearModelMixin.predict(self, X, fhe=fhe)
         return y_preds
 
-    def clean_graph(self):
-        """Clean the graph of the onnx model.
-
-        Any operators following gemm, including the sigmoid, softmax and argmax operators, are
-        removed from the graph. They will be executed in clear in the post-processing method.
-        """
-        clean_graph_after_node_op_type(self.onnx_model, node_op_type="Gemm")
-        super().clean_graph()
-
-
-def get_sklearn_models():
-    """Return the list of available models in Concrete-ML.
-
-    Returns:
-        the lists of models in Concrete-ML
-    """
-
-    # Import anything in sklearn, just to force the import, to populate _ALL_SKLEARN_MODELS list
-    # pylint: disable=unused-import, import-outside-toplevel, cyclic-import
-    from ..sklearn import LinearRegression  # noqa: F401
-
-    # We return sorted lists such that it is ordered, to avoid notably issues when it is used
-    # in @pytest.mark.parametrize
-    ans = {
-        "all": sorted(list(_ALL_SKLEARN_MODELS), key=lambda m: m.__name__),
-        "linear": sorted(list(_LINEAR_MODELS), key=lambda m: m.__name__),
-        "tree": sorted(list(_TREE_MODELS), key=lambda m: m.__name__),
-        "neural_net": sorted(list(_NEURALNET_MODELS), key=lambda m: m.__name__),
-    }
-    return ans
-
-
-def _filter_models(prelist, classifier: bool, regressor: bool, str_in_class_name: str = None):
-    """Return the models which are in prelist and follow (classifier, regressor) conditions.
-
-    Args:
-        prelist: list of models
-        classifier (bool): whether you want classifiers or not
-        regressor (bool): whether you want regressors or not
-        str_in_class_name (str): if not None, only return models with this as a substring in the
-            class name
-
-    Returns:
-        the sublist which fulfills the (classifier, regressor, str_in_class_name) conditions.
-
-    """
-    assert_true(classifier or regressor, "Please set at least one option")
-
-    answer = []
-
-    if classifier:
-        answer += [m for m in prelist if sklearn.base.is_classifier(m)]
-
-    if regressor:
-        answer += [m for m in prelist if sklearn.base.is_regressor(m)]
-
-    if str_in_class_name is not None:
-        answer = [m for m in answer if str_in_class_name in m.__name__]
-
-    # We return a sorted list such that it is ordered, to avoid notably issues when it is used
-    # in @pytest.mark.parametrize
-    return sorted(answer, key=lambda m: m.__name__)
-
-
-def get_sklearn_linear_models(
-    classifier: bool = True, regressor: bool = True, str_in_class_name: str = None
-):
-    """Return the list of available linear models in Concrete-ML.
-
-    Args:
-        classifier (bool): whether you want classifiers or not
-        regressor (bool): whether you want regressors or not
-        str_in_class_name (str): if not None, only return models with this as a substring in the
-            class name
-
-    Returns:
-        the lists of linear models in Concrete-ML
-    """
-    prelist = get_sklearn_models()["linear"]
-    return _filter_models(prelist, classifier, regressor, str_in_class_name)
-
-
-def get_sklearn_tree_models(
-    classifier: bool = True, regressor: bool = True, str_in_class_name: str = None
-):
-    """Return the list of available tree models in Concrete-ML.
-
-    Args:
-        classifier (bool): whether you want classifiers or not
-        regressor (bool): whether you want regressors or not
-        str_in_class_name (str): if not None, only return models with this as a substring in the
-            class name
-
-    Returns:
-        the lists of tree models in Concrete-ML
-    """
-    prelist = get_sklearn_models()["tree"]
-    return _filter_models(prelist, classifier, regressor, str_in_class_name)
-
-
-def get_sklearn_neural_net_models(
-    classifier: bool = True, regressor: bool = True, str_in_class_name: str = None
-):
-    """Return the list of available neural net models in Concrete-ML.
-
-    Args:
-        classifier (bool): whether you want classifiers or not
-        regressor (bool): whether you want regressors or not
-        str_in_class_name (str): if not None, only return models with this as a substring in the
-            class name
-
-    Returns:
-        the lists of neural net models in Concrete-ML
-    """
-    prelist = get_sklearn_models()["neural_net"]
-    return _filter_models(prelist, classifier, regressor, str_in_class_name)
+    def predict_proba(self, X: Data, fhe: Union[FheMode, str] = FheMode.DISABLE) -> numpy.ndarray:
+        y_logits = self.decision_function(X, fhe=fhe)
+        y_proba = self.post_processing(y_logits)
+        return y_proba
```

## concrete/ml/sklearn/glm.py

```diff
@@ -1,25 +1,28 @@
 """Implement sklearn's Generalized Linear Models (GLM)."""
 from __future__ import annotations
 
 from abc import abstractmethod
-from typing import Union
+from typing import Any, Dict, Union
 
 import numpy
-import sklearn
-import torch
+from sklearn.linear_model import GammaRegressor as SklearnGammaRegressor
+from sklearn.linear_model import PoissonRegressor as SklearnPoissonRegressor
+from sklearn.linear_model import TweedieRegressor as SklearnTweedieRegressor
 
+from .. import TRUSTED_SKOPS, USE_SKOPS, loads_sklearn
 from ..common.debugging.custom_assert import assert_true
-from ..torch.numpy_module import NumpyModule
-from .base import SklearnLinearModelMixin
-from .torch_modules import _LinearTorchModel
+from ..common.utils import FheMode
+from ..onnx.onnx_model_manipulations import clean_graph_after_node_op_type
+from ..quantization.quantizers import UniformQuantizer
+from .base import Data, SklearnLinearRegressorMixin
 
 
 # pylint: disable-next=too-many-instance-attributes
-class _GeneralizedLinearRegressor(SklearnLinearModelMixin, sklearn.base.RegressorMixin):
+class _GeneralizedLinearRegressor(SklearnLinearRegressorMixin):
     """Regression via a penalized Generalized Linear Model (GLM) with FHE.
 
     Parameters:
         n_bits (int, Dict[str, int]): Number of bits to quantize the model. If an int is passed
             for n_bits, the value will be used for quantizing inputs and weights. If a dict is
             passed, then it should contain "op_inputs" and "op_weights" as keys with
             corresponding number of quantization bits so that:
@@ -36,103 +39,117 @@
         fit_intercept: bool = True,
         solver: str = "lbfgs",
         max_iter: int = 100,
         tol: float = 1e-4,
         warm_start: bool = False,
         verbose: int = 0,
     ):
-        self.n_bits = n_bits
+        # Call SklearnLinearModelMixin's __init__ method
+        super().__init__(n_bits=n_bits)
+
         self.alpha = alpha
         self.fit_intercept = fit_intercept
         self.solver = solver
         self.max_iter = max_iter
         self.tol = tol
         self.warm_start = warm_start
         self.verbose = verbose
-        self._onnx_model_ = None
-        super().__init__(n_bits=n_bits)
 
-    def post_processing(
-        self, y_preds: numpy.ndarray, already_dequantized: bool = False
-    ) -> numpy.ndarray:
-        """Post-processing the predictions.
+    def _clean_graph(self) -> None:
+        assert self.onnx_model_ is not None, self._is_not_fitted_error_message()
 
-        Args:
-            y_preds (numpy.ndarray): The predictions to post-process.
-            already_dequantized (bool): Whether the inputs were already dequantized or not. Default
-                to False.
-
-        Returns:
-            numpy.ndarray: The post-processed predictions.
-        """
-        # If y_preds were already dequantized previously, there is no need to do so once again.
-        # This step is necessary for the client-server workflow as the post_processing method
-        # is directly called on the quantized outputs, contrary to the base class' predict method.
-        if not already_dequantized:
-            y_preds = self.dequantize_output(y_preds)
+        # Remove any operators following gemm, as they will be done in the clear in post-processing
+        # In particular, this includes the exponential operator
+        clean_graph_after_node_op_type(self.onnx_model_, node_op_type="Gemm")
+        super()._clean_graph()
 
+    def post_processing(self, y_preds: numpy.ndarray) -> numpy.ndarray:
         return self._inverse_link(y_preds)
 
-    def predict(self, X: numpy.ndarray, execute_in_fhe: bool = False) -> numpy.ndarray:
-        """Predict on user data.
-
-        Predict on user data using either the quantized clear model, implemented with tensors, or,
-        if execute_in_fhe is set, using the compiled FHE circuit.
+    def predict(self, X: Data, fhe: Union[FheMode, str] = FheMode.DISABLE) -> numpy.ndarray:
+        # Call SklearnLinearModelMixin's predict method
+        y_preds = super().predict(X, fhe=fhe)
 
-        Args:
-            X (numpy.ndarray): The input data.
-            execute_in_fhe (bool): Whether to execute the inference in FHE. Default to False.
-
-        Returns:
-            numpy.ndarray: The model's predictions.
-        """
-        y_preds = super().predict(X, execute_in_fhe=execute_in_fhe)
-        y_preds = self.post_processing(y_preds, already_dequantized=True)
+        y_preds = self.post_processing(y_preds)
         return y_preds
 
-    # FIXME: #2080 Remove this method when Hummingbird releases its next update as they will make
-    # converting GLMs available
-    def _set_onnx_model(self, test_input: numpy.ndarray):
-        """Retrieve the model's ONNX graph using Hummingbird conversion.
+    @abstractmethod
+    def _inverse_link(self, y_preds: numpy.ndarray) -> numpy.ndarray:
+        """Apply the link function's inverse on the inputs.
 
         Args:
-            test_input (numpy.ndarray): An input data used to trace the model execution.
+            y_preds (numpy.ndarray): The input data.
         """
 
-        assert_true(
-            self.sklearn_model is not None,
-            "The model is not fitted. Please run fit(...) on proper arguments first.",
-        )
+    def dump_dict(self) -> Dict:
+        assert self._weight_quantizer is not None, self._is_not_fitted_error_message()
 
-        # Initialize the Torch model. Using a small Torch model that reproduces the proper
-        # inference is necessary for GLMs. Indeed, the Hummingbird library does not support these
-        # models and thus cannot be used to convert them into an ONNX form. Additionally, a
-        # NumpyModule accepts a Torch module as an input, making the rest of the structure still
-        # usable.
-        torch_model = _LinearTorchModel(
-            weight=self.sklearn_model.coef_,
-            bias=self.sklearn_model.intercept_ if self.fit_intercept else None,
+        metadata: Dict[str, Any] = {}
+        metadata["cml_dumped_class_name"] = str(type(self).__name__)
+        metadata["n_bits"] = self.n_bits
+        metadata["sklearn_model"] = self.sklearn_model
+        metadata["sklearn_model_class"] = self.sklearn_model_class
+        metadata["post_processing_params"] = self.post_processing_params
+        metadata["fhe_circuit"] = self.fhe_circuit
+        metadata["_is_fitted"] = self._is_fitted
+        metadata["_is_compiled"] = self._is_compiled
+        metadata["input_quantizers"] = [elt.dumps() for elt in self.input_quantizers]
+        metadata["_weight_quantizer"] = self._weight_quantizer.dumps()
+        metadata["output_quantizers"] = [elt.dumps() for elt in self.output_quantizers]
+        metadata["onnx_model_"] = self.onnx_model_
+        metadata["_q_weights"] = self._q_weights
+        metadata["_q_bias"] = self._q_bias
+
+        metadata["alpha"] = self.alpha
+        metadata["fit_intercept"] = self.fit_intercept
+        metadata["solver"] = self.solver
+        metadata["max_iter"] = self.max_iter
+        metadata["tol"] = self.tol
+        metadata["warm_start"] = self.warm_start
+        metadata["verbose"] = self.verbose
+
+        return metadata
+
+    @classmethod
+    def load_dict(cls, metadata: Dict):
+        obj = cls(n_bits=metadata["n_bits"])
+
+        obj.input_quantizers = [UniformQuantizer.loads(elt) for elt in metadata["input_quantizers"]]
+        obj._weight_quantizer = UniformQuantizer.loads(metadata["_weight_quantizer"])
+        obj.output_quantizers = [
+            UniformQuantizer.loads(elt) for elt in metadata["output_quantizers"]
+        ]
+
+        # Load the underlying fitted model
+        loads_sklearn_kwargs = {}
+        if USE_SKOPS:
+            loads_sklearn_kwargs["trusted"] = TRUSTED_SKOPS
+        obj.sklearn_model = loads_sklearn(
+            bytes.fromhex(metadata["sklearn_model"]), **loads_sklearn_kwargs
         )
 
-        # Create a NumpyModule from the Torch model
-        numpy_module = NumpyModule(
-            torch_model,
-            dummy_input=torch.from_numpy(test_input[0]),
-        )
+        obj.post_processing_params = metadata["post_processing_params"]
 
-        # Retrieve the ONNX graph
-        self.onnx_model = numpy_module.onnx_model
+        obj.fhe_circuit = metadata["fhe_circuit"]
+        obj.onnx_model_ = metadata["onnx_model_"]
+        obj._is_fitted = metadata["_is_fitted"]
+        obj._is_compiled = metadata["_is_compiled"]
+        obj._q_weights = metadata["_q_weights"]
+        obj._q_bias = metadata["_q_bias"]
+
+        obj.n_bits = metadata["n_bits"]
+        obj.alpha = metadata["alpha"]
+        obj.fit_intercept = metadata["fit_intercept"]
+        obj.solver = metadata["solver"]
+        obj.max_iter = metadata["max_iter"]
+        obj.tol = metadata["tol"]
+        obj.warm_start = metadata["warm_start"]
+        obj.verbose = metadata["verbose"]
 
-    @abstractmethod
-    def _inverse_link(self, y_preds):
-        """Apply the link function's inverse on the inputs.
-
-        Args:
-            y_preds (numpy.ndarray): The input data.
-        """
+        return obj
 
 
 class PoissonRegressor(_GeneralizedLinearRegressor):
     """A Poisson regression model with FHE.
 
     Parameters:
         n_bits (int, Dict[str, int]): Number of bits to quantize the model. If an int is passed
@@ -143,17 +160,15 @@
             - op_weights: number of bits to quantize the learned parameters
             Default to 8.
 
     For more details on PoissonRegressor please refer to the scikit-learn documentation:
     https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.PoissonRegressor.html
     """
 
-    sklearn_alg = sklearn.linear_model.PoissonRegressor
-
-    # pylint: disable-next=protected-access
+    sklearn_model_class = SklearnPoissonRegressor
     _is_a_public_cml_model = True
 
     def __init__(
         self,
         *,
         n_bits: Union[int, dict] = 8,
         alpha: float = 1.0,
@@ -169,25 +184,15 @@
             fit_intercept=fit_intercept,
             max_iter=max_iter,
             tol=tol,
             warm_start=warm_start,
             verbose=verbose,
         )
 
-    def _inverse_link(self, y_preds) -> numpy.ndarray:
-        """Apply the link function's inverse on the inputs.
-
-        PoissonRegressor uses the exponential function.
-
-        Args:
-            y_preds (numpy.ndarray): The input data.
-
-        Returns:
-            The model's final predictions.
-        """
+    def _inverse_link(self, y_preds: numpy.ndarray) -> numpy.ndarray:
         return numpy.exp(y_preds)
 
 
 class GammaRegressor(_GeneralizedLinearRegressor):
     """A Gamma regression model with FHE.
 
     Parameters:
@@ -199,17 +204,15 @@
             - op_weights: number of bits to quantize the learned parameters
             Default to 8.
 
     For more details on GammaRegressor please refer to the scikit-learn documentation:
     https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.GammaRegressor.html
     """
 
-    sklearn_alg = sklearn.linear_model.GammaRegressor
-
-    # pylint: disable-next=protected-access
+    sklearn_model_class = SklearnGammaRegressor
     _is_a_public_cml_model = True
 
     def __init__(
         self,
         *,
         n_bits: Union[int, dict] = 8,
         alpha: float = 1.0,
@@ -225,28 +228,19 @@
             fit_intercept=fit_intercept,
             max_iter=max_iter,
             tol=tol,
             warm_start=warm_start,
             verbose=verbose,
         )
 
-    def _inverse_link(self, y_preds) -> numpy.ndarray:
-        """Apply the link function's inverse on the inputs.
-
-        GammaRegressor uses the exponential function.
-
-        Args:
-            y_preds (numpy.ndarray): The input data.
-
-        Returns:
-            The model's final predictions.
-        """
+    def _inverse_link(self, y_preds: numpy.ndarray) -> numpy.ndarray:
         return numpy.exp(y_preds)
 
 
+# pylint: disable-next=too-many-instance-attributes
 class TweedieRegressor(_GeneralizedLinearRegressor):
     """A Tweedie regression model with FHE.
 
     Parameters:
         n_bits (int, Dict[str, int]): Number of bits to quantize the model. If an int is passed
             for n_bits, the value will be used for quantizing inputs and weights. If a dict is
             passed, then it should contain "op_inputs" and "op_weights" as keys with
@@ -255,17 +249,15 @@
             - op_weights: number of bits to quantize the learned parameters
             Default to 8.
 
     For more details on TweedieRegressor please refer to the scikit-learn documentation:
     https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.TweedieRegressor.html
     """
 
-    sklearn_alg = sklearn.linear_model.TweedieRegressor
-
-    # pylint: disable-next=protected-access
+    sklearn_model_class = SklearnTweedieRegressor
     _is_a_public_cml_model = True
 
     def __init__(
         self,
         *,
         n_bits: Union[int, dict] = 8,
         power: float = 0.0,
@@ -291,32 +283,88 @@
             link in ["auto", "log", "identity"],
             f"link must be an element of ['auto', 'identity', 'log'], got '{link}'",
         )
 
         self.power = power
         self.link = link
 
-    def _inverse_link(self, y_preds) -> numpy.ndarray:
-        """Apply the link function's inverse on the inputs.
-
-        TweedieRegressor uses either the identity or the exponential function.
-
-        Args:
-            y_preds (numpy.ndarray): The input data.
+    def _set_post_processing_params(self):
+        super()._set_post_processing_params()
+        self.post_processing_params.update(
+            {
+                "link": self.link,
+                "power": self.power,
+            }
+        )
 
-        Returns:
-            The model's final predictions.
-        """
+    def _inverse_link(self, y_preds: numpy.ndarray) -> numpy.ndarray:
+        self.check_model_is_fitted()
 
-        if self.link == "auto":
+        if self.post_processing_params["link"] == "auto":
 
             # Identity link
-            if self.power <= 0:
+            if self.post_processing_params["power"] <= 0:
                 return y_preds
 
             # Log link
             return numpy.exp(y_preds)
 
-        if self.link == "log":
+        if self.post_processing_params["link"] == "log":
             return numpy.exp(y_preds)
 
         return y_preds
+
+    def dump_dict(self) -> Dict:
+        assert self._weight_quantizer is not None, self._is_not_fitted_error_message()
+
+        metadata: Dict[str, Any] = {}
+        metadata["cml_dumped_class_name"] = str(type(self).__name__)
+        metadata["n_bits"] = self.n_bits
+        metadata["sklearn_model"] = self.sklearn_model
+        metadata["sklearn_model_class"] = self.sklearn_model_class
+        metadata["post_processing_params"] = self.post_processing_params
+        metadata["fhe_circuit"] = self.fhe_circuit
+        metadata["_is_fitted"] = self._is_fitted
+        metadata["_is_compiled"] = self._is_compiled
+        metadata["input_quantizers"] = [elt.dumps() for elt in self.input_quantizers]
+        metadata["_weight_quantizer"] = self._weight_quantizer.dumps()
+        metadata["output_quantizers"] = [elt.dumps() for elt in self.output_quantizers]
+        metadata["onnx_model_"] = self.onnx_model_
+        metadata["_q_weights"] = self._q_weights
+        metadata["_q_bias"] = self._q_bias
+
+        metadata["power"] = self.power
+        metadata["link"] = self.link
+
+        return metadata
+
+    @classmethod
+    def load_dict(cls, metadata: Dict):
+        obj = cls(n_bits=metadata["n_bits"])
+
+        obj.input_quantizers = [UniformQuantizer.loads(elt) for elt in metadata["input_quantizers"]]
+        obj._weight_quantizer = UniformQuantizer.loads(metadata["_weight_quantizer"])
+        obj.output_quantizers = [
+            UniformQuantizer.loads(elt) for elt in metadata["output_quantizers"]
+        ]
+
+        # Load the underlying fitted model
+        loads_sklearn_kwargs = {}
+        if USE_SKOPS:
+            loads_sklearn_kwargs["trusted"] = TRUSTED_SKOPS
+        obj.sklearn_model = loads_sklearn(
+            bytes.fromhex(metadata["sklearn_model"]), **loads_sklearn_kwargs
+        )
+
+        obj.post_processing_params = metadata["post_processing_params"]
+
+        obj.fhe_circuit = metadata["fhe_circuit"]
+        obj.onnx_model_ = metadata["onnx_model_"]
+        obj._is_fitted = metadata["_is_fitted"]
+        obj._is_compiled = metadata["_is_compiled"]
+        obj._q_weights = metadata["_q_weights"]
+        obj._q_bias = metadata["_q_bias"]
+
+        obj.power = metadata["power"]
+        obj.link = metadata["link"]
+
+        return obj
```

## concrete/ml/sklearn/linear_model.py

```diff
@@ -1,16 +1,21 @@
 """Implement sklearn linear model."""
+from typing import Any, Dict
+
+import numpy
 import sklearn
 import sklearn.linear_model
 
-from .base import SklearnLinearClassifierMixin, SklearnLinearModelMixin
+from .. import TRUSTED_SKOPS, USE_SKOPS, loads_sklearn
+from ..quantization.quantizers import UniformQuantizer
+from .base import SklearnLinearClassifierMixin, SklearnLinearRegressorMixin
 
 
 # pylint: disable=invalid-name,too-many-instance-attributes
-class LinearRegression(SklearnLinearModelMixin, sklearn.base.RegressorMixin):
+class LinearRegression(SklearnLinearRegressorMixin):
     """A linear regression model with FHE.
 
     Parameters:
         n_bits (int, Dict[str, int]): Number of bits to quantize the model. If an int is passed
             for n_bits, the value will be used for quantizing inputs and weights. If a dict is
             passed, then it should contain "op_inputs" and "op_weights" as keys with
             corresponding number of quantization bits so that:
@@ -18,39 +23,104 @@
             - op_weights: number of bits to quantize the learned parameters
             Default to 8.
 
     For more details on LinearRegression please refer to the scikit-learn documentation:
     https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html
     """
 
-    sklearn_alg = sklearn.linear_model.LinearRegression
+    sklearn_model_class = sklearn.linear_model.LinearRegression
 
     _is_a_public_cml_model = True
 
     def __init__(
         self,
         n_bits=8,
         fit_intercept=True,
         normalize="deprecated",
         copy_X=True,
         n_jobs=None,
         positive=False,
     ):
-        # FIXME: Figure out how to add scikit-learn documentation into our object #893
-        self.n_bits = n_bits
+        # Call SklearnLinearModelMixin's __init__ method
+        super().__init__(n_bits=n_bits)
+
         self.fit_intercept = fit_intercept
         self.normalize = normalize
         self.copy_X = copy_X
         self.n_jobs = n_jobs
         self.positive = positive
-        self._onnx_model_ = None
-        super().__init__(n_bits=n_bits)
 
+    def dump_dict(self) -> Dict[str, Any]:
+        assert self._weight_quantizer is not None, self._is_not_fitted_error_message()
+
+        metadata: Dict[str, Any] = {}
 
-class ElasticNet(SklearnLinearModelMixin, sklearn.base.RegressorMixin):
+        metadata["post_processing_params"] = self.post_processing_params
+        metadata["cml_dumped_class_name"] = type(self).__name__
+
+        # Linear
+        metadata["n_bits"] = self.n_bits
+        metadata["sklearn_model"] = self.sklearn_model
+        metadata["sklearn_model_class"] = self.sklearn_model_class
+        metadata["fhe_circuit"] = self.fhe_circuit
+        metadata["_is_fitted"] = self._is_fitted
+        metadata["_is_compiled"] = self._is_compiled
+        metadata["input_quantizers"] = [elt.dumps() for elt in self.input_quantizers]
+        metadata["_weight_quantizer"] = self._weight_quantizer.dumps()
+        metadata["output_quantizers"] = [elt.dumps() for elt in self.output_quantizers]
+        metadata["onnx_model_"] = self.onnx_model_
+        metadata["_q_weights"] = self._q_weights
+        metadata["_q_bias"] = self._q_bias
+
+        metadata["fit_intercept"] = self.fit_intercept
+        metadata["normalize"] = self.normalize
+        metadata["copy_X"] = self.copy_X
+        metadata["n_jobs"] = self.n_jobs
+        metadata["positive"] = self.positive
+
+        return metadata
+
+    @classmethod
+    def load_dict(cls, metadata: Dict):
+        obj = LinearRegression()
+        obj.post_processing_params = metadata["post_processing_params"]
+
+        # Load the underlying fitted model
+        loads_sklearn_kwargs = {}
+        if USE_SKOPS:
+            loads_sklearn_kwargs["trusted"] = TRUSTED_SKOPS
+        obj.sklearn_model = loads_sklearn(
+            bytes.fromhex(metadata["sklearn_model"]), **loads_sklearn_kwargs
+        )
+
+        # Linear
+        obj.n_bits = metadata["n_bits"]
+        obj.sklearn_model_class = metadata["sklearn_model_class"]
+        obj.fhe_circuit = metadata["fhe_circuit"]
+        obj.input_quantizers = [UniformQuantizer.loads(elt) for elt in metadata["input_quantizers"]]
+        obj.output_quantizers = [
+            UniformQuantizer.loads(elt) for elt in metadata["output_quantizers"]
+        ]
+        obj._weight_quantizer = UniformQuantizer.loads(metadata["_weight_quantizer"])
+        obj.onnx_model_ = metadata["onnx_model_"]
+        obj._is_fitted = metadata["_is_fitted"]
+        obj._is_compiled = metadata["_is_compiled"]
+        obj._q_weights = metadata["_q_weights"]
+        obj._q_bias = metadata["_q_bias"]
+
+        # Custom
+        obj.fit_intercept = metadata["fit_intercept"]
+        obj.normalize = metadata["normalize"]
+        obj.copy_X = metadata["copy_X"]
+        obj.n_jobs = metadata["n_jobs"]
+        obj.positive = metadata["positive"]
+        return obj
+
+
+class ElasticNet(SklearnLinearRegressorMixin):
     """An ElasticNet regression model with FHE.
 
     Parameters:
         n_bits (int, Dict[str, int]): Number of bits to quantize the model. If an int is passed
             for n_bits, the value will be used for quantizing inputs and weights. If a dict is
             passed, then it should contain "op_inputs" and "op_weights" as keys with
             corresponding number of quantization bits so that:
@@ -58,15 +128,15 @@
             - op_weights: number of bits to quantize the learned parameters
             Default to 8.
 
     For more details on ElasticNet please refer to the scikit-learn documentation:
     https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.ElasticNet.html
     """
 
-    sklearn_alg = sklearn.linear_model.ElasticNet
+    sklearn_model_class = sklearn.linear_model.ElasticNet
     _is_a_public_cml_model = True
 
     # pylint: disable-next=too-many-arguments
     def __init__(
         self,
         n_bits=8,
         alpha=1.0,
@@ -78,33 +148,112 @@
         copy_X=True,
         tol=0.0001,
         warm_start=False,
         positive=False,
         random_state=None,
         selection="cyclic",
     ):
-        # FIXME: Figure out how to add scikit-learn documentation into our object #893
-        self.n_bits = n_bits
+        # Call SklearnLinearModelMixin's __init__ method
+        super().__init__(n_bits=n_bits)
+
         self.alpha = alpha
         self.l1_ratio = l1_ratio
         self.fit_intercept = fit_intercept
         self.normalize = normalize
         self.copy_X = copy_X
         self.positive = positive
-        self._onnx_model_ = None
         self.precompute = precompute
         self.max_iter = max_iter
         self.tol = tol
         self.warm_start = warm_start
         self.random_state = random_state
         self.selection = selection
-        super().__init__(n_bits=n_bits)
 
+    def dump_dict(self) -> Dict[str, Any]:
+        assert self._weight_quantizer is not None, self._is_not_fitted_error_message()
+
+        metadata: Dict[str, Any] = {}
+
+        metadata["post_processing_params"] = self.post_processing_params
+        metadata["cml_dumped_class_name"] = type(self).__name__
+
+        # Linear
+        metadata["n_bits"] = self.n_bits
+        metadata["sklearn_model"] = self.sklearn_model
+        metadata["sklearn_model_class"] = self.sklearn_model_class
+        metadata["fhe_circuit"] = self.fhe_circuit
+        metadata["_is_fitted"] = self._is_fitted
+        metadata["_is_compiled"] = self._is_compiled
+        metadata["input_quantizers"] = [elt.dumps() for elt in self.input_quantizers]
+        metadata["_weight_quantizer"] = self._weight_quantizer.dumps()
+        metadata["output_quantizers"] = [elt.dumps() for elt in self.output_quantizers]
+        metadata["onnx_model_"] = self.onnx_model_
+        metadata["_q_weights"] = self._q_weights
+        metadata["_q_bias"] = self._q_bias
+
+        metadata["alpha"] = self.alpha
+        metadata["l1_ratio"] = self.l1_ratio
+        metadata["fit_intercept"] = self.fit_intercept
+        metadata["normalize"] = self.normalize
+        metadata["copy_X"] = self.copy_X
+        metadata["positive"] = self.positive
+        metadata["precompute"] = self.precompute
+        metadata["max_iter"] = self.max_iter
+        metadata["tol"] = self.tol
+        metadata["warm_start"] = self.warm_start
+        metadata["random_state"] = self.random_state
+        metadata["selection"] = self.selection
+
+        return metadata
+
+    @classmethod
+    def load_dict(cls, metadata: Dict):
+        obj = ElasticNet()
+        obj.post_processing_params = metadata["post_processing_params"]
+
+        # Load the underlying fitted model
+        loads_sklearn_kwargs = {}
+        if USE_SKOPS:
+            loads_sklearn_kwargs["trusted"] = TRUSTED_SKOPS
+        obj.sklearn_model = loads_sklearn(
+            bytes.fromhex(metadata["sklearn_model"]), **loads_sklearn_kwargs
+        )
+
+        # Linear
+        obj.n_bits = metadata["n_bits"]
+        obj.sklearn_model_class = metadata["sklearn_model_class"]
+        obj.fhe_circuit = metadata["fhe_circuit"]
+        obj.input_quantizers = [UniformQuantizer.loads(elt) for elt in metadata["input_quantizers"]]
+        obj.output_quantizers = [
+            UniformQuantizer.loads(elt) for elt in metadata["output_quantizers"]
+        ]
+        obj._weight_quantizer = UniformQuantizer.loads(metadata["_weight_quantizer"])
+        obj.onnx_model_ = metadata["onnx_model_"]
+        obj._is_fitted = metadata["_is_fitted"]
+        obj._is_compiled = metadata["_is_compiled"]
+        obj._q_weights = metadata["_q_weights"]
+        obj._q_bias = metadata["_q_bias"]
+
+        obj.alpha = metadata["alpha"]
+        obj.l1_ratio = metadata["l1_ratio"]
+        obj.fit_intercept = metadata["fit_intercept"]
+        obj.normalize = metadata["normalize"]
+        obj.copy_X = metadata["copy_X"]
+        obj.positive = metadata["positive"]
+        obj.precompute = metadata["precompute"]
+        obj.max_iter = metadata["max_iter"]
+        obj.tol = metadata["tol"]
+        obj.warm_start = metadata["warm_start"]
+        obj.random_state = metadata["random_state"]
+        obj.selection = metadata["selection"]
+
+        return obj
 
-class Lasso(SklearnLinearModelMixin, sklearn.base.RegressorMixin):
+
+class Lasso(SklearnLinearRegressorMixin):
     """A Lasso regression model with FHE.
 
     Parameters:
         n_bits (int, Dict[str, int]): Number of bits to quantize the model. If an int is passed
             for n_bits, the value will be used for quantizing inputs and weights. If a dict is
             passed, then it should contain "op_inputs" and "op_weights" as keys with
             corresponding number of quantization bits so that:
@@ -112,15 +261,15 @@
             - op_weights: number of bits to quantize the learned parameters
             Default to 8.
 
     For more details on Lasso please refer to the scikit-learn documentation:
     https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.Lasso.html
     """
 
-    sklearn_alg = sklearn.linear_model.Lasso
+    sklearn_model_class = sklearn.linear_model.Lasso
     _is_a_public_cml_model = True
 
     # pylint: disable-next=too-many-arguments
     def __init__(
         self,
         n_bits=8,
         alpha: float = 1.0,
@@ -131,32 +280,109 @@
         max_iter=1000,
         tol=0.0001,
         warm_start=False,
         positive=False,
         random_state=None,
         selection="cyclic",
     ):
-        # FIXME: Figure out how to add scikit-learn documentation into our object #893
-        self.n_bits = n_bits
+        # Call SklearnLinearModelMixin's __init__ method
+        super().__init__(n_bits=n_bits)
+
         self.alpha = alpha
         self.fit_intercept = fit_intercept
         self.normalize = normalize
         self.copy_X = copy_X
         self.positive = positive
-        self._onnx_model_ = None
         self.max_iter = max_iter
         self.warm_start = warm_start
         self.selection = selection
         self.tol = tol
         self.precompute = precompute
         self.random_state = random_state
-        super().__init__(n_bits=n_bits)
 
+    def dump_dict(self) -> Dict[str, Any]:
+        assert self._weight_quantizer is not None, self._is_not_fitted_error_message()
+
+        metadata: Dict[str, Any] = {}
 
-class Ridge(SklearnLinearModelMixin, sklearn.base.RegressorMixin):
+        metadata["post_processing_params"] = self.post_processing_params
+        metadata["cml_dumped_class_name"] = type(self).__name__
+
+        # Linear
+        metadata["n_bits"] = self.n_bits
+        metadata["sklearn_model"] = self.sklearn_model
+        metadata["sklearn_model_class"] = self.sklearn_model_class
+        metadata["fhe_circuit"] = self.fhe_circuit
+        metadata["_is_fitted"] = self._is_fitted
+        metadata["_is_compiled"] = self._is_compiled
+        metadata["input_quantizers"] = [elt.dumps() for elt in self.input_quantizers]
+        metadata["_weight_quantizer"] = self._weight_quantizer.dumps()
+        metadata["output_quantizers"] = [elt.dumps() for elt in self.output_quantizers]
+        metadata["onnx_model_"] = self.onnx_model_
+        metadata["_q_weights"] = self._q_weights
+        metadata["_q_bias"] = self._q_bias
+
+        metadata["alpha"] = self.alpha
+        metadata["fit_intercept"] = self.fit_intercept
+        metadata["normalize"] = self.normalize
+        metadata["copy_X"] = self.copy_X
+        metadata["positive"] = self.positive
+        metadata["max_iter"] = self.max_iter
+        metadata["warm_start"] = self.warm_start
+        metadata["selection"] = self.selection
+        metadata["tol"] = self.tol
+        metadata["precompute"] = self.precompute
+        metadata["random_state"] = self.random_state
+
+        return metadata
+
+    @classmethod
+    def load_dict(cls, metadata: Dict):
+        obj = Lasso()
+        obj.post_processing_params = metadata["post_processing_params"]
+
+        # Load the underlying fitted model
+        loads_sklearn_kwargs = {}
+        if USE_SKOPS:
+            loads_sklearn_kwargs["trusted"] = TRUSTED_SKOPS
+        obj.sklearn_model = loads_sklearn(
+            bytes.fromhex(metadata["sklearn_model"]), **loads_sklearn_kwargs
+        )
+
+        # Linear
+        obj.n_bits = metadata["n_bits"]
+        obj.sklearn_model_class = metadata["sklearn_model_class"]
+        obj.fhe_circuit = metadata["fhe_circuit"]
+        obj.input_quantizers = [UniformQuantizer.loads(elt) for elt in metadata["input_quantizers"]]
+        obj.output_quantizers = [
+            UniformQuantizer.loads(elt) for elt in metadata["output_quantizers"]
+        ]
+        obj._weight_quantizer = UniformQuantizer.loads(metadata["_weight_quantizer"])
+        obj.onnx_model_ = metadata["onnx_model_"]
+        obj._is_fitted = metadata["_is_fitted"]
+        obj._is_compiled = metadata["_is_compiled"]
+        obj._q_weights = metadata["_q_weights"]
+        obj._q_bias = metadata["_q_bias"]
+
+        obj.alpha = metadata["alpha"]
+        obj.fit_intercept = metadata["fit_intercept"]
+        obj.normalize = metadata["normalize"]
+        obj.copy_X = metadata["copy_X"]
+        obj.positive = metadata["positive"]
+        obj.max_iter = metadata["max_iter"]
+        obj.warm_start = metadata["warm_start"]
+        obj.selection = metadata["selection"]
+        obj.tol = metadata["tol"]
+        obj.precompute = metadata["precompute"]
+        obj.random_state = metadata["random_state"]
+
+        return obj
+
+
+class Ridge(SklearnLinearRegressorMixin):
     """A Ridge regression model with FHE.
 
     Parameters:
         n_bits (int, Dict[str, int]): Number of bits to quantize the model. If an int is passed
             for n_bits, the value will be used for quantizing inputs and weights. If a dict is
             passed, then it should contain "op_inputs" and "op_weights" as keys with
             corresponding number of quantization bits so that:
@@ -164,15 +390,15 @@
             - op_weights: number of bits to quantize the learned parameters
             Default to 8.
 
     For more details on Ridge please refer to the scikit-learn documentation:
     https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.Ridge.html
     """
 
-    sklearn_alg = sklearn.linear_model.Ridge
+    sklearn_model_class = sklearn.linear_model.Ridge
     _is_a_public_cml_model = True
 
     # pylint: disable-next=too-many-arguments
     def __init__(
         self,
         n_bits=8,
         alpha: float = 1.0,
@@ -181,30 +407,102 @@
         copy_X=True,
         max_iter=None,
         tol=0.001,
         solver="auto",
         positive=False,
         random_state=None,
     ):
-        # FIXME: Figure out how to add scikit-learn documentation into our object #893
-        self.n_bits = n_bits
+        # Call SklearnLinearModelMixin's __init__ method
+        super().__init__(n_bits=n_bits)
+
         self.alpha = alpha
         self.fit_intercept = fit_intercept
         self.normalize = normalize
         self.copy_X = copy_X
         self.positive = positive
         self.max_iter = max_iter
         self.tol = tol
         self.solver = solver
         self.random_state = random_state
-        self._onnx_model_ = None
-        super().__init__(n_bits=n_bits)
 
+    def dump_dict(self) -> Dict[str, Any]:
+        assert self._weight_quantizer is not None, self._is_not_fitted_error_message()
+
+        metadata: Dict[str, Any] = {}
+
+        metadata["post_processing_params"] = self.post_processing_params
+        metadata["cml_dumped_class_name"] = type(self).__name__
+
+        # Linear
+        metadata["n_bits"] = self.n_bits
+        metadata["sklearn_model"] = self.sklearn_model
+        metadata["sklearn_model_class"] = self.sklearn_model_class
+        metadata["fhe_circuit"] = self.fhe_circuit
+        metadata["_is_fitted"] = self._is_fitted
+        metadata["_is_compiled"] = self._is_compiled
+        metadata["input_quantizers"] = [elt.dumps() for elt in self.input_quantizers]
+        metadata["_weight_quantizer"] = self._weight_quantizer.dumps()
+        metadata["output_quantizers"] = [elt.dumps() for elt in self.output_quantizers]
+        metadata["onnx_model_"] = self.onnx_model_
+        metadata["_q_weights"] = self._q_weights
+        metadata["_q_bias"] = self._q_bias
+
+        metadata["alpha"] = self.alpha
+        metadata["fit_intercept"] = self.fit_intercept
+        metadata["normalize"] = self.normalize
+        metadata["copy_X"] = self.copy_X
+        metadata["positive"] = self.positive
+        metadata["max_iter"] = self.max_iter
+        metadata["tol"] = self.tol
+        metadata["solver"] = self.solver
+        metadata["random_state"] = self.random_state
+
+        return metadata
+
+    @classmethod
+    def load_dict(cls, metadata: Dict):
+        obj = Ridge()
+        obj.post_processing_params = metadata["post_processing_params"]
+
+        # Load the underlying fitted model
+        loads_sklearn_kwargs = {}
+        if USE_SKOPS:
+            loads_sklearn_kwargs["trusted"] = TRUSTED_SKOPS
+        obj.sklearn_model = loads_sklearn(
+            bytes.fromhex(metadata["sklearn_model"]), **loads_sklearn_kwargs
+        )
+
+        # Linear
+        obj.n_bits = metadata["n_bits"]
+        obj.sklearn_model_class = metadata["sklearn_model_class"]
+        obj.fhe_circuit = metadata["fhe_circuit"]
+        obj.input_quantizers = [UniformQuantizer.loads(elt) for elt in metadata["input_quantizers"]]
+        obj.output_quantizers = [
+            UniformQuantizer.loads(elt) for elt in metadata["output_quantizers"]
+        ]
+        obj._weight_quantizer = UniformQuantizer.loads(metadata["_weight_quantizer"])
+        obj.onnx_model_ = metadata["onnx_model_"]
+        obj._is_fitted = metadata["_is_fitted"]
+        obj._is_compiled = metadata["_is_compiled"]
+        obj._q_weights = metadata["_q_weights"]
+        obj._q_bias = metadata["_q_bias"]
+
+        obj.alpha = metadata["alpha"]
+        obj.fit_intercept = metadata["fit_intercept"]
+        obj.normalize = metadata["normalize"]
+        obj.copy_X = metadata["copy_X"]
+        obj.positive = metadata["positive"]
+        obj.max_iter = metadata["max_iter"]
+        obj.tol = metadata["tol"]
+        obj.solver = metadata["solver"]
+        obj.random_state = metadata["random_state"]
+        return obj
 
-class LogisticRegression(SklearnLinearClassifierMixin, sklearn.base.ClassifierMixin):
+
+class LogisticRegression(SklearnLinearClassifierMixin):
     """A logistic regression model with FHE.
 
     Parameters:
         n_bits (int, Dict[str, int]): Number of bits to quantize the model. If an int is passed
             for n_bits, the value will be used for quantizing inputs and weights. If a dict is
             passed, then it should contain "op_inputs" and "op_weights" as keys with
             corresponding number of quantization bits so that:
@@ -212,15 +510,15 @@
             - op_weights: number of bits to quantize the learned parameters
             Default to 8.
 
     For more details on LogisticRegression please refer to the scikit-learn documentation:
     https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html
     """
 
-    sklearn_alg = sklearn.linear_model.LogisticRegression
+    sklearn_model_class = sklearn.linear_model.LogisticRegression
     _is_a_public_cml_model = True
 
     # pylint: disable-next=too-many-arguments
     def __init__(
         self,
         n_bits=8,
         penalty="l2",
@@ -235,15 +533,17 @@
         max_iter=100,
         multi_class="auto",
         verbose=0,
         warm_start=False,
         n_jobs=None,
         l1_ratio=None,
     ):
-        # FIXME: Figure out how to add scikit-learn documentation into our object #893
+        # Call BaseClassifier's __init__ method
+        super().__init__(n_bits=n_bits)
+
         self.penalty = penalty
         self.dual = dual
         self.tol = tol
         self.C = C
         self.fit_intercept = fit_intercept
         self.intercept_scaling = intercept_scaling
         self.class_weight = class_weight
@@ -251,12 +551,106 @@
         self.solver = solver
         self.max_iter = max_iter
         self.multi_class = multi_class
         self.verbose = verbose
         self.warm_start = warm_start
         self.n_jobs = n_jobs
         self.l1_ratio = l1_ratio
-        self._onnx_model_ = None
-        super().__init__(n_bits=n_bits)
+
+    def dump_dict(self) -> Dict[str, Any]:
+        assert self._weight_quantizer is not None, self._is_not_fitted_error_message()
+
+        metadata: Dict[str, Any] = {}
+
+        metadata["post_processing_params"] = self.post_processing_params
+        metadata["cml_dumped_class_name"] = type(self).__name__
+
+        # Classifier
+        metadata["classes_"] = self.target_classes_
+        metadata["n_classes_"] = self.n_classes_
+        metadata["cml_dumped_class_name"] = type(self).__name__
+
+        # Linear
+        metadata["n_bits"] = self.n_bits
+        metadata["sklearn_model"] = self.sklearn_model
+        metadata["sklearn_model_class"] = self.sklearn_model_class
+        metadata["fhe_circuit"] = self.fhe_circuit
+        metadata["_is_fitted"] = self._is_fitted
+        metadata["_is_compiled"] = self._is_compiled
+        metadata["input_quantizers"] = [elt.dumps() for elt in self.input_quantizers]
+        metadata["_weight_quantizer"] = self._weight_quantizer.dumps()
+        metadata["output_quantizers"] = [elt.dumps() for elt in self.output_quantizers]
+        metadata["onnx_model_"] = self.onnx_model_
+        metadata["_q_weights"] = self._q_weights
+        metadata["_q_bias"] = self._q_bias
+
+        # Specific
+        metadata["penalty"] = self.penalty
+        metadata["dual"] = self.dual
+        metadata["tol"] = self.tol
+        metadata["C"] = self.C
+        metadata["fit_intercept"] = self.fit_intercept
+        metadata["intercept_scaling"] = self.intercept_scaling
+        metadata["class_weight"] = self.class_weight
+        metadata["random_state"] = self.random_state
+        metadata["solver"] = self.solver
+        metadata["max_iter"] = self.max_iter
+        metadata["multi_class"] = self.multi_class
+        metadata["verbose"] = self.verbose
+        metadata["warm_start"] = self.warm_start
+        metadata["n_jobs"] = self.n_jobs
+        metadata["l1_ratio"] = self.l1_ratio
+
+        return metadata
+
+    @classmethod
+    def load_dict(cls, metadata: Dict):
+        obj = LogisticRegression()
+        obj.post_processing_params = metadata["post_processing_params"]
+
+        # Load the underlying fitted model
+        loads_sklearn_kwargs = {}
+        if USE_SKOPS:
+            loads_sklearn_kwargs["trusted"] = TRUSTED_SKOPS
+        obj.sklearn_model = loads_sklearn(
+            bytes.fromhex(metadata["sklearn_model"]), **loads_sklearn_kwargs
+        )
+
+        # Classifier
+        obj.target_classes_ = numpy.array(metadata["classes_"])
+        obj.n_classes_ = metadata["n_classes_"]
+
+        # Linear
+        obj.n_bits = metadata["n_bits"]
+        obj.sklearn_model_class = metadata["sklearn_model_class"]
+        obj.fhe_circuit = metadata["fhe_circuit"]
+        obj.input_quantizers = [UniformQuantizer.loads(elt) for elt in metadata["input_quantizers"]]
+        obj.output_quantizers = [
+            UniformQuantizer.loads(elt) for elt in metadata["output_quantizers"]
+        ]
+        obj._weight_quantizer = UniformQuantizer.loads(metadata["_weight_quantizer"])
+        obj.onnx_model_ = metadata["onnx_model_"]
+        obj._is_fitted = metadata["_is_fitted"]
+        obj._is_compiled = metadata["_is_compiled"]
+        obj._q_weights = metadata["_q_weights"]
+        obj._q_bias = metadata["_q_bias"]
+
+        obj.penalty = metadata["penalty"]
+        obj.dual = metadata["dual"]
+        obj.tol = metadata["tol"]
+        obj.C = metadata["C"]
+        obj.fit_intercept = metadata["fit_intercept"]
+        obj.intercept_scaling = metadata["intercept_scaling"]
+        obj.class_weight = metadata["class_weight"]
+        obj.random_state = metadata["random_state"]
+        obj.solver = metadata["solver"]
+        obj.max_iter = metadata["max_iter"]
+        obj.multi_class = metadata["multi_class"]
+        obj.verbose = metadata["verbose"]
+        obj.warm_start = metadata["warm_start"]
+        obj.n_jobs = metadata["n_jobs"]
+        obj.l1_ratio = metadata["l1_ratio"]
+
+        return obj
 
 
 # pylint: enable=too-many-instance-attributes,invalid-name
```

## concrete/ml/sklearn/qnn.py

```diff
@@ -1,511 +1,303 @@
-"""Scikit-learn interface for concrete quantized neural networks."""
+"""Scikit-learn interface for fully-connected quantized neural networks."""
 
 # Disable pylint invalid name since scikit learn uses "X" as variable name for data
 # pylint: disable=invalid-name
 
-from abc import abstractmethod
+from typing import Any, Dict, Union
 
-import brevitas.nn as qnn
 import numpy
 import torch
-import torch.nn.utils.prune as pruning
-from skorch.classifier import NeuralNetClassifier as SKNeuralNetClassifier
-from skorch.regressor import NeuralNetRegressor as SKNeuralNetRegressor
-from torch import nn
-
-from ..common.utils import MAX_BITWIDTH_BACKWARD_COMPATIBLE
-from .base import QuantizedTorchEstimatorMixin
-
-
-class SparseQuantNeuralNetImpl(nn.Module):
-    """Sparse Quantized Neural Network classifier.
-
-    This class implements an MLP that is compatible with FHE constraints. The weights and
-    activations are quantized to low bitwidth and pruning is used to ensure accumulators do not
-    surpass an user-provided accumulator bit-width. The number of classes and number of layers
-    are specified by the user, as well as the breadth of the network
-    """
-
-    def __init__(
-        self,
-        input_dim,
-        n_layers,
-        n_outputs,
-        n_hidden_neurons_multiplier=4,
-        n_w_bits=3,
-        n_a_bits=3,
-        n_accum_bits=MAX_BITWIDTH_BACKWARD_COMPATIBLE,
-        activation_function=nn.ReLU,
-        quant_narrow=False,
-        quant_signed=True,
-    ):  # pylint: disable=too-many-arguments
-        """Sparse Quantized Neural Network constructor.
-
-        Args:
-            input_dim: Number of dimensions of the input data
-            n_layers: Number of linear layers for this network
-            n_outputs: Number of output classes or regression targets
-            n_w_bits: Number of weight bits
-            n_a_bits: Number of activation and input bits
-            n_accum_bits: Maximal allowed bitwidth of intermediate accumulators
-            n_hidden_neurons_multiplier: A factor that is multiplied by the maximal number of
-                active (non-zero weight) neurons for every layer. The maximal number of neurons in
-                the worst case scenario is:
-                                                                      2^n_max-1
-                       max_active_neurons(n_max, n_w, n_a) = floor(---------------------)
-                                                                   (2^n_w-1)*(2^n_a-1) )
-                The worst case scenario for the bitwidth of the accumulator is when all weights and
-                activations are maximum simultaneously. We set, for each layer, the total number of
-                neurons to be:
-                 n_hidden_neurons_multiplier * max_active_neurons(n_accum_bits, n_w_bits, n_a_bits)
-                Through experiments, for typical distributions of weights and activations,
-                the default value for n_hidden_neurons_multiplier, 4, is safe to avoid overflow.
-            activation_function: a torch class that is used to construct activation functions in
-                the network (e.g. torch.ReLU, torch.SELU, torch.Sigmoid, etc)
-            quant_narrow : whether this network should use narrow range quantized integer values
-            quant_signed : whether to use signed quantized integer values
-
-        Raises:
-            ValueError: if the parameters have invalid values or the computed accumulator bitwidth
-                        is zero
-        """
-
-        super().__init__()
-
-        self.features = nn.Sequential()
-        in_features = input_dim
-
-        if input_dim <= 0:
-            raise ValueError(
-                f"Invalid number of input dimensions: {input_dim}, input_dim must be greater than 0"
-            )
-
-        if n_layers <= 0:
-            raise ValueError(
-                f"Invalid number of layers: {n_layers}, at least one intermediary layers is needed"
-            )
-
-        if n_outputs < 1:
-            raise ValueError(
-                f"Invalid number of outputs: {n_outputs}, n_outputs should be larger than one"
-            )
-
-        if n_w_bits <= 0 or n_a_bits <= 0:
-            raise ValueError("The weight & activation quantization bitwidth cannot be less than 1")
-
-        for idx in range(n_layers):
-            out_features = (
-                n_outputs if idx == n_layers - 1 else input_dim * n_hidden_neurons_multiplier
-            )
-
-            quant_name = f"quant{idx}"
-            quantizer = qnn.QuantIdentity(
-                bit_width=n_a_bits,
-                return_quant_tensor=True,
-                narrow_range=quant_narrow,
-                signed=quant_signed,
-            )
-
-            layer_name = f"fc{idx}"
-            layer = qnn.QuantLinear(
-                in_features,
-                out_features,
-                True,
-                weight_bit_width=n_w_bits,
-                bias_quant=None,
-                weight_narrow_range=quant_narrow,
-                narrow_range=quant_narrow,
-                signed=quant_signed,
-            )
-
-            self.features.add_module(quant_name, quantizer)
-            self.features.add_module(layer_name, layer)
-
-            if idx < n_layers - 1:
-                self.features.add_module(f"act{idx}", activation_function())
+from skorch.classifier import NeuralNetClassifier as SkorchNeuralNetClassifier
+from skorch.dataset import Dataset, ValidSplit
+from skorch.regressor import NeuralNetRegressor as SkorchNeuralNetRegressor
+from torch.utils.data import DataLoader
 
-            in_features = out_features
+from ..common.debugging import assert_true
+from ..common.utils import FheMode, check_dtype_and_cast
+from .base import QNN_AUTO_KWARGS, BaseClassifier, Data, QuantizedTorchEstimatorMixin, Target
 
-        self.n_w_bits = n_w_bits
-        self.n_a_bits = n_a_bits
-        self.n_accum_bits = n_accum_bits
+# Define the QNN's support float and int dtypes
+QNN_FLOAT_DTYPE = numpy.float32
+QNN_INT_DTYPE = numpy.int64
 
-        self.pruned_layers = set()
 
-        self.enable_pruning()
+def _check_qnn_kwargs(input_kwargs: Dict[str, Any]) -> None:
+    """Check that a QNN model is not constructed with automatically computed parameters.
 
-    def max_active_neurons(self):
-        """Compute the maximum number of active (non-zero weight) neurons.
+    Args:
+        input_kwargs (dict): The keyword arguments to check.
 
-        The computation is done using the quantization parameters passed to the constructor.
-        Warning: With the current quantization algorithm (asymmetric) the value returned by this
-        function is not guaranteed to ensure FHE compatibility. For some weight distributions,
-        weights that are 0 (which are pruned weights) will not be quantized to 0.
-        Therefore the total number of active quantized neurons will not be equal to
-        max_active_neurons.
-
-        Returns:
-            n (int): maximum number of active neurons
-        """
+    Raises:
+        ValueError: If the automatically computed parameters are present in the keyword arguments.
+    """
 
-        return int(
-            numpy.floor(
-                (2**self.n_accum_bits - 1) / (2**self.n_w_bits - 1) / (2**self.n_a_bits - 1)
-            )
+    if "n_bits" in input_kwargs:
+        raise ValueError(
+            "Setting `n_bits` in Quantized Neural Networks is not possible. Instead, initialize "
+            "the model using `module__n_w_bits`, `module__n_a_bits` and `module__n_accum_bits` "
+            "keyword arguments."
         )
 
-    def make_pruning_permanent(self):
-        """Make the learned pruning permanent in the network."""
-        max_neuron_connections = self.max_active_neurons()
-
-        # Iterate over all layers that have weights (Linear ones)
-        for layer in self.features:
-            if not isinstance(layer, nn.Linear):
-                continue
-
-            s = layer.weight.shape
-            # If this is a layer that should be pruned and is currently being pruned,
-            # Make the pruning permanent
-            if s[0] > max_neuron_connections and layer in self.pruned_layers:
-                pruning.remove(layer, "weight")
-                self.pruned_layers.remove(layer)
-
-    def enable_pruning(self):
-        """Enable pruning in the network. Pruning must be made permanent to recover pruned weights.
-
-        Raises:
-            ValueError: if the quantization parameters are invalid
-        """
-        max_neuron_connections = self.max_active_neurons()
+    if "module" in input_kwargs:
+        raise ValueError(
+            "Setting `module` manually is forbidden. The module is set automatically when "
+            "initializing the instance."
+        )
 
-        if max_neuron_connections == 0:
+    for auto_kwarg in QNN_AUTO_KWARGS:
+        if auto_kwarg in input_kwargs:
             raise ValueError(
-                "The maximum accumulator bitwidth is too low "
-                "for the quantization parameters requested. No neurons would be created in the "
-                "requested configuration"
+                f" Setting `{auto_kwarg}` manually is forbidden. The number of inputs and outputs "
+                "of the neural network are determined automatically in .fit, based on the data-set."
             )
 
-        # Iterate over all layers that have weights (Linear ones)
-        for layer in self.features:
-            if not isinstance(layer, nn.Linear) and not isinstance(layer, qnn.QuantLinear):
-                continue
-
-            s = layer.weight.shape
-            # To satisfy accumulator bitwidth constraints each dot-product between an input line and
-            # weight column must not exceed n_accum_bits bits. We thus prune the layer to have
-            # at most max_neuron_connections non-zero weights
-            if s[0] > max_neuron_connections and layer not in self.pruned_layers:
-                pruning.l1_unstructured(layer, "weight", (s[0] - max_neuron_connections) * s[1])
-                self.pruned_layers.add(layer)
-
-    def forward(self, x):
-        """Forward pass.
-
-        Args:
-            x (torch.Tensor): network input
-
-        Returns:
-            x (torch.Tensor): network prediction
-        """
-        return self.features(x)
-
-    def on_train_end(self):
-        """Call back when training is finished, can be useful to remove training hooks."""
-        self.make_pruning_permanent()
-
-
-class QuantizedSkorchEstimatorMixin(QuantizedTorchEstimatorMixin):
-    """Mixin class that adds quantization features to Skorch NN estimators."""
-
-    @property
-    @abstractmethod
-    def base_estimator_type(self):
-        """Get the sklearn estimator that should be trained by the child class."""
-
-    def infer(self, x, **fit_params):
-        """Perform a single inference step on a batch of data.
-
-        This method is specific to Skorch estimators.
-
-        Args:
-            x (torch.Tensor): A batch of the input data, produced by a Dataset
-            **fit_params (dict) : Additional parameters passed to the ``forward`` method of
-                the module and to the ``self.train_split`` call.
-
-        Returns:
-            A torch tensor with the inference results for each item in the input
-        """
-
-        # During training we infer the same as in the base class
-        # Note that this supports more data types for x than we support in quantized mode
-        if self.quantized_module_ is None:
-            return super().infer(x, **fit_params)
-
-        # Get a numpy array from the tensor to do quantization
-        x = x.detach().cpu().numpy()
-
-        # Once we finished the data type checks, quantize the input and perform quantized inference
-        q_x = self.quantized_module_.quantize_input(x)
-        q_out = self.quantized_module_(q_x)
-
-        # Cast back to a tensor to keep a consistent API (tensor in, tensor out)
-        return torch.tensor(self.quantized_module_.dequantize_output(q_out))
-
-    @property
-    def base_module_to_compile(self):
-        """Get the module that should be compiled to FHE. In our case this is a torch nn.Module.
-
-        Returns:
-            module (nn.Module): the instantiated torch module
-        """
-        return self.module_
-
-    @property
-    def n_bits_quant(self):
-        """Return the number of quantization bits.
-
-        This is stored by the torch.nn.module instance and thus cannot be retrieved until this
-        instance is created.
-
-        Returns:
-            n_bits (int): the number of bits to quantize the network
-
-        Raises:
-            ValueError: with skorch estimators, the `module_` is not instantiated until .fit() is
-                called. Thus this estimator needs to be .fit() before we get the quantization number
-                of bits. If it is not trained we raise an exception
-        """
-
-        module_attr = getattr(self, "module_", None)
-        if module_attr is None:
-            raise ValueError("NN Classifier must be trained before getting the number of bits")
-        return self.module_.n_a_bits
-
-    def get_params_for_benchmark(self):
-        """Get parameters for benchmark when cloning a skorch wrapped NN.
-
-        We must remove all parameters related to the module. Skorch takes either a class or a
-        class instance for the `module` parameter. We want to pass our trained model, a class
-        instance. But for this to work, we need to remove all module related constructor params.
-        If not, skorch will instantiate a new class instance of the same type as the passed module
-        see skorch net.py NeuralNet::initialize_instance
-
-        Returns:
-            params (dict): parameters to create an equivalent fp32 sklearn estimator for benchmark
-        """
-        new_object_params = super().get_params_for_benchmark()
-        module_params = [name for name in new_object_params.keys() if "module__" in name]
-        for name in module_params:
-            new_object_params.pop(name)
-        return new_object_params
-
-    # pylint: disable=unused-argument
-    def on_train_end(self, net, X=None, y=None, **kwargs):
-        """Call back when training is finished by the skorch wrapper.
-
-        Check if the underlying neural net has a callback for this event and, if so, call it.
-
-        Args:
-            net: estimator for which training has ended (equal to self)
-            X: data
-            y: targets
-            kwargs: other arguments
-        """
-        train_end_callback = getattr(self.module_, "on_train_end", None)
-        if callable(train_end_callback):
-            train_end_callback()
-
-
-class FixedTypeSkorchNeuralNet:
-    """A mixin with a helpful modification to a skorch estimator that fixes the module type."""
-
-    def get_params(self, deep=True, **kwargs):
-        """Get parameters for this estimator.
-
-        Args:
-            deep (bool): If True, will return the parameters for this estimator and
-                contained subobjects that are estimators.
-            **kwargs: any additional parameters to pass to the sklearn BaseEstimator class
-
-        Returns:
-            params : dict, Parameter names mapped to their values.
-        """
-        # Known but with pylint when mixin is mixed with a class in a different file
-        # pylint: disable=no-member
-        params = super().get_params(deep, **kwargs)
-        # pylint: enable=no-member
-
-        # Remove the module key since our NN skorch class imposes SparseQuantNeuralNetImpl as
-        # the NN model type. Therefore, when cloning this estimator we don't need to pass
-        # module again, it's passed by this class's constructor
-        params.pop("module")
-        return params
-
-
-class NeuralNetClassifier(
-    FixedTypeSkorchNeuralNet,
-    QuantizedSkorchEstimatorMixin,
-    SKNeuralNetClassifier,
-):
-    """Scikit-learn interface for quantized FHE compatible neural networks.
-
-    This class wraps a quantized NN implemented using our Torch tools as a scikit-learn Estimator.
-    It uses the skorch package to handle training and scikit-learn compatibility,
-    and adds quantization and compilation functionality. The neural network implemented by this
-    class is a multi layer fully connected network trained with Quantization Aware Training (QAT).
-
-    The datatypes that are allowed for prediction by this wrapper are more restricted than
-    standard scikit-learn estimators as this class needs to predict in FHE and network inference
-    executor is the NumpyModule.
+
+# QNNs do not support serialization yet
+# FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/3134
+# pylint: disable-next=too-many-instance-attributes, abstract-method
+class NeuralNetRegressor(QuantizedTorchEstimatorMixin, SkorchNeuralNetRegressor):
+    """A Fully-Connected Neural Network regressor with FHE.
+
+    This class wraps a quantized neural network implemented using Torch tools as a Scikit-Learn
+    estimator. The Skorch package allows to handle training and Scikit-Learn compatibility,
+    and adds quantization as well as compilation functionalities. The neural network implemented
+    by this class is a multi layer fully connected network trained with Quantization Aware Training
+    (QAT).
+
+    Inputs and targets that are float64 will be casted to float32 before training as Torch does not
+    handle float64 types properly. Thus should not have a significant impact on the model's
+    performances. An error is raised if these values are not floating points.
     """
 
-    # pylint: disable-next=protected-access
+    sklearn_model_class = SkorchNeuralNetRegressor
     _is_a_public_cml_model = True
 
-    # FIXME: make this class accept a generic NN and not impose our SparseQuantNeuralNetImpl
-    # see https://github.com/zama-ai/concrete-ml-internal/issues/327
+    # pylint: disable=too-many-arguments
     def __init__(
         self,
-        *args,
-        criterion=torch.nn.CrossEntropyLoss,
-        classes=None,
+        criterion=torch.nn.MSELoss,
         optimizer=torch.optim.Adam,
+        lr=0.01,
+        max_epochs=10,
+        batch_size=128,
+        iterator_train=DataLoader,
+        iterator_valid=DataLoader,
+        dataset=Dataset,
+        train_split=None,
+        callbacks=None,
+        predict_nonlinearity="auto",
+        warm_start=False,
+        verbose=1,
+        device="cpu",
         **kwargs,
     ):
-        # It basically just sets quantized_module_ and _onnx_model_ to None
-        # It calls the init of QuantizedSkorchEstimatorMixin
+        # Call QuantizedTorchEstimatorMixin's __init__ method
         super().__init__()
 
-        # If no parameters are passed just returns
-        # Used to load the model class from json
-        if len(args) == 0 and len(kwargs) == 0:
-            return
-        # A helper for users so they don't need to import torch directly
-        args_to_convert_to_tensor = ["criterion__weight"]
-        for arg_name in args_to_convert_to_tensor:
-            if arg_name in kwargs and isinstance(kwargs[arg_name], numpy.ndarray):
-                kwargs[arg_name] = torch.from_numpy(kwargs[arg_name]).float()
-
-        n_classes = kwargs["module__n_outputs"]
-        if n_classes < 2:
-            raise ValueError(
-                f"Invalid number of classes: {str(n_classes)}, "
-                "n_outputs should be larger than one"
-            )
-
-        kwargs.pop("n_bits", None)
-
-        # Note that our default optimizer is Adam which was found to be more stable when pruning
-        SKNeuralNetClassifier.__init__(
-            self,
-            SparseQuantNeuralNetImpl,
-            *args,
-            criterion=criterion,
-            classes=classes,
-            optimizer=optimizer,
-            **kwargs,
+        self.criterion = criterion
+        self.optimizer = optimizer
+        self.lr = lr
+        self.max_epochs = max_epochs
+        self.batch_size = batch_size
+        self.iterator_train = iterator_train
+        self.iterator_valid = iterator_valid
+        self.dataset = dataset
+        self.train_split = ValidSplit(5) if train_split is None else train_split
+        self.callbacks = callbacks
+        self.predict_nonlinearity = predict_nonlinearity
+        self.warm_start = warm_start
+        self.verbose = verbose
+        self.device = device
+
+        _check_qnn_kwargs(kwargs)
+
+        history = kwargs.pop("history", None)
+        initialized = kwargs.pop("initialized_", False)
+        virtual_params = kwargs.pop("virtual_params_", {})
+
+        self._kwargs = kwargs
+        vars(self).update(kwargs)
+
+        self.history_ = history
+        self.initialized_ = initialized
+        self.virtual_params_ = virtual_params
+
+    def fit(self, X: Data, y: Target, *args, **kwargs):
+        # Check that inputs and targets are float32. If they are float64, they will be casted to
+        # float32 as this should not have a great impact on the model's performances. Else, an error
+        # is raised.
+        X = check_dtype_and_cast(X, "float32", error_information="Neural Network regressor input")
+        y = check_dtype_and_cast(y, "float32", error_information="Neural Network regressor target")
+
+        # The number of outputs for regressions is the number of regression targets
+        # We use y.shape which works for all supported datatype (including numpy array, pandas
+        # dataframe and torch tensor).
+        self.module__n_outputs = y.shape[1] if y.ndim == 2 else 1
+
+        # Set the number of input dimensions to use
+        self.module__input_dim = X.shape[1]
+
+        # Call QuantizedTorchEstimatorMixin's fit method
+        return super().fit(X, y, *args, **kwargs)
+
+    def fit_benchmark(self, X: Data, y: Target, *args, **kwargs):
+        # Check that inputs and targets are float32. If they are float64, they will be casted to
+        # float32 as this should not have a great impact on the model's performances. Else, an error
+        # is raised.
+        X = check_dtype_and_cast(X, "float32", error_information="Neural Network regressor input")
+        y = check_dtype_and_cast(y, "float32", error_information="Neural Network regressor target")
+
+        # Call QuantizedTorchEstimatorMixin's fit_benchmark method
+        return super().fit_benchmark(X, y, *args, **kwargs)
+
+    # Skorch provides a predict_proba method for neural network regressors while Scikit-Learn does
+    # not. We decided to follow Scikit-Learn's API as we build most of our tools on this library.
+    # However, our models are still directly inheriting from Skorch's classes, which makes this
+    # method accessible by anyone, without having any FHE implementation. As this could create some
+    # confusion, a NotImplementedError is raised. This issue could be fixed by making these classes
+    # not inherit from Skorch.
+    # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/3373
+    def predict_proba(self, X: Data, fhe: Union[FheMode, str] = FheMode.DISABLE) -> numpy.ndarray:
+        raise NotImplementedError(
+            "The `predict_proba` method is not implemented for neural network regressors. Please "
+            "call `predict` instead."
         )
 
-    @property
-    def base_estimator_type(self):
-        return SKNeuralNetClassifier
-
-    # Disable pylint here because we add an additional argument to .predict,
-    # with respect to the base class .predict method.
-    # pylint: disable=arguments-differ
-    def predict(self, X, execute_in_fhe=False):
-        """Predict on user provided data.
-
-        Predicts using the quantized clear or FHE classifier
-
-        Args:
-            X : input data, a numpy array of raw values (non quantized)
-            execute_in_fhe : whether to execute the inference in FHE or in the clear
-
-        Returns:
-            y_pred : numpy ndarray with predictions
-
-        """
-
-        # We just need to do argmax on the predicted probabilities
-        return self.predict_proba(X, execute_in_fhe=execute_in_fhe).argmax(axis=1)
-
-    def fit(self, X, y, **fit_params):
-        # We probably can't handle all cases since per Skorch documentation they handle:
-        #  * numpy arrays
-        #  * torch tensors
-        #  * pandas DataFrame or Series
-        #  * scipy sparse CSR matrices
-        #  * a dictionary of the former three
-        #  * a list/tuple of the former three
-        #  * a Dataset
-        # which is a bit much since they don't necessarily have the same interfaces to handle types
-        if isinstance(X, numpy.ndarray) and (X.dtype != numpy.float32):
-            X = X.astype(numpy.float32)
-        if isinstance(y, numpy.ndarray) and (y.dtype != numpy.int64):
-            y = y.astype(numpy.int64)
-        return super().fit(X, y, **fit_params)
-
-
-class NeuralNetRegressor(
-    FixedTypeSkorchNeuralNet, QuantizedSkorchEstimatorMixin, SKNeuralNetRegressor
-):
-    """Scikit-learn interface for quantized FHE compatible neural networks.
-
-    This class wraps a quantized NN implemented using our Torch tools as a scikit-learn Estimator.
-    It uses the skorch package to handle training and scikit-learn compatibility,
-    and adds quantization and compilation functionality. The neural network implemented by this
-    class is a multi layer fully connected network trained with Quantization Aware Training (QAT).
-
-    The datatypes that are allowed for prediction by this wrapper are more restricted than
-    standard scikit-learn estimators as this class needs to predict in FHE and network inference
-    executor is the NumpyModule.
+    def predict(self, X: Data, fhe: Union[FheMode, str] = FheMode.DISABLE) -> numpy.ndarray:
+        # Check that inputs are float32. If they are float64, they will be casted to float32 as
+        # this should not have a great impact on the model's performances. Else, an error is raised.
+        X = check_dtype_and_cast(X, "float32", error_information="Neural Network regressor input")
+
+        # Call BaseEstimator's predict method and cast values to float32
+        y_preds = super().predict(X, fhe=fhe)
+        y_preds = self.post_processing(y_preds)
+        return y_preds
+
+
+# QNNs do not support serialization yet
+# FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/3134
+# pylint: disable-next=too-many-instance-attributes, abstract-method
+class NeuralNetClassifier(BaseClassifier, QuantizedTorchEstimatorMixin, SkorchNeuralNetClassifier):
+    """A Fully-Connected Neural Network classifier with FHE.
+
+    This class wraps a quantized neural network implemented using Torch tools as a Scikit-Learn
+    estimator. The Skorch package allows to handle training and Scikit-Learn compatibility,
+    and adds quantization as well as compilation functionalities. The neural network implemented
+    by this class is a multi layer fully connected network trained with Quantization Aware Training
+    (QAT).
+
+    Inputs that are float64 will be casted to float32 before training as Torch does not
+    handle float64 types properly. Thus should not have a significant impact on the model's
+    performances. If the targets are integers of lower bitwidth, they will be safely casted to
+    int64. Else, an error is raised.
     """
 
-    # pylint: disable-next=protected-access
+    sklearn_model_class = SkorchNeuralNetClassifier
     _is_a_public_cml_model = True
 
-    # FIXME: make this class accept a generic NN and not impose our SparseQuantNeuralNetImpl
-    # see https://github.com/zama-ai/concrete-ml-internal/issues/327
+    # pylint: disable=too-many-arguments
     def __init__(
         self,
-        *args,
+        criterion=torch.nn.CrossEntropyLoss,
         optimizer=torch.optim.Adam,
+        classes=None,
+        lr=0.01,
+        max_epochs=10,
+        batch_size=128,
+        iterator_train=DataLoader,
+        iterator_valid=DataLoader,
+        dataset=Dataset,
+        train_split=None,
+        callbacks=None,
+        predict_nonlinearity="auto",
+        warm_start=False,
+        verbose=1,
+        device="cpu",
         **kwargs,
     ):
+        # Call BaseClassifier's __init__ method
         super().__init__()
-        # If no parameters are passed just return
-        # Used to load the model class from json
-        if len(args) == 0 and len(kwargs) == 0:
-            return
-
-        kwargs.pop("n_bits", None)
-
-        # Note that our default optimizer is Adam which was found to be more stable when pruning
-        SKNeuralNetRegressor.__init__(
-            self,
-            SparseQuantNeuralNetImpl,
-            *args,
-            optimizer=optimizer,
-            **kwargs,
+
+        self.criterion = criterion
+        self.optimizer = optimizer
+        self.classes = classes
+        self.lr = lr
+        self.max_epochs = max_epochs
+        self.batch_size = batch_size
+        self.iterator_train = iterator_train
+        self.iterator_valid = iterator_valid
+        self.dataset = dataset
+        self.train_split = ValidSplit(5, stratified=True) if train_split is None else train_split
+        self.callbacks = callbacks
+        self.predict_nonlinearity = predict_nonlinearity
+        self.warm_start = warm_start
+        self.verbose = verbose
+        self.device = device
+
+        _check_qnn_kwargs(kwargs)
+
+        history = kwargs.pop("history", None)
+        initialized = kwargs.pop("initialized_", False)
+        virtual_params = kwargs.pop("virtual_params_", {})
+
+        self._kwargs = kwargs
+        vars(self).update(kwargs)
+
+        self.history_ = history
+        self.initialized_ = initialized
+        self.virtual_params_ = virtual_params
+
+    def fit(self, X: Data, y: Target, *args, **kwargs):
+        # Check that inputs are float32 and targets are int64. If inputs are float64, they will be
+        # casted to float32 as this should not have a great impact on the model's performances. If
+        # the targets are integers of lower bitwidth, they will be safely casted to int64. Else, an
+        # error is raised.
+        X = check_dtype_and_cast(X, "float32", error_information="Neural Network classifier input")
+        y = check_dtype_and_cast(y, "int64", error_information="Neural Network classifier target")
+
+        classes, y = numpy.unique(y, return_inverse=True)
+
+        # Check that at least two classes are given
+        n_classes = len(classes)
+        assert_true(
+            n_classes >= 2,
+            f"Invalid number of classes: {str(n_classes)}, " "n_outputs should be larger than one",
         )
 
-    @property
-    def base_estimator_type(self):
-        return SKNeuralNetRegressor
-
-    def fit(self, X, y, **fit_params):
-        # We probably can't handle all cases since per Skorch documentation they handle:
-        #  * numpy arrays
-        #  * torch tensors
-        #  * pandas DataFrame or Series
-        #  * scipy sparse CSR matrices
-        #  * a dictionary of the former three
-        #  * a list/tuple of the former three
-        #  * a Dataset
-        # which is a bit much since they don't necessarily have the same interfaces to handle types
-        if isinstance(X, numpy.ndarray) and (X.dtype != numpy.float32):
-            X = X.astype(numpy.float32)
-        if isinstance(y, numpy.ndarray) and (y.dtype != numpy.float32):
-            y = y.astype(numpy.float32)
-        return super().fit(X, y, **fit_params)
+        # Set the number of outputs of the nn.Module to the number of classes
+        self.module__n_outputs = n_classes
+
+        # Set the number of input dimensions to use
+        self.module__input_dim = X.shape[1]
+
+        # Call BaseClassifier's fit method
+        return super().fit(X, y, *args, **kwargs)
+
+    def fit_benchmark(self, X: Data, y: Target, *args, **kwargs):
+        # Check that inputs are float32 and targets are int64. If inputs are float64, they will be
+        # casted to float32 as this should not have a great impact on the model's performances. If
+        # the targets are integers of lower bitwidth, they will be safely casted to int64. Else, an
+        # error is raised.
+        X = check_dtype_and_cast(X, "float32", error_information="Neural Network classifier input")
+        y = check_dtype_and_cast(y, "int64", error_information="Neural Network classifier target")
+
+        # Call QuantizedTorchEstimatorMixin's fit_benchmark method
+        return super().fit_benchmark(X, y, *args, **kwargs)
+
+    def predict_proba(self, X: Data, fhe: Union[FheMode, str] = FheMode.DISABLE) -> numpy.ndarray:
+        # Check that inputs are float32. If they are, they will be casted to float32 as this
+        # should not have a great impact on the model's performances. Else, an error is raised.
+        X = check_dtype_and_cast(X, "float32", error_information="Neural Network classifier input")
+
+        # Call BaseClassifier's predict_proba method, apply the sigmoid and cast values to float32
+        y_logits = super().predict_proba(X, fhe=fhe)
+        y_proba = self.post_processing(y_logits)
+        return y_proba
+
+    def predict(self, X: Data, fhe: Union[FheMode, str] = FheMode.DISABLE) -> numpy.ndarray:
+        # Check that inputs are float32. If they are float64, they will be casted to float32 as
+        # this should not have a great impact on the model's performances. Else, an error is raised.
+        X = check_dtype_and_cast(X, "float32", error_information="Neural Network classifier input")
+
+        # Call BaseClassifier's predict method
+        return super().predict(X, fhe=fhe)
```

## concrete/ml/sklearn/rf.py

```diff
@@ -1,32 +1,29 @@
-"""Implements RandomForest models."""
-from typing import Any, Callable, List, Optional
+"""Implement RandomForest models."""
+from typing import Any, Dict
 
-import sklearn.ensemble
-
-from ..quantization import QuantizedArray
-from .base import BaseTreeClassifierMixin, BaseTreeRegressorMixin
+import numpy
+from sklearn.ensemble import RandomForestClassifier as SklearnRandomForestClassifier
+from sklearn.ensemble import RandomForestRegressor as SklearnRandomForestRegressor
+
+from .. import TRUSTED_SKOPS, USE_SKOPS, loads_sklearn
+from ..quantization.quantizers import UniformQuantizer
+from ..sklearn.tree_to_numpy import tree_to_numpy
+from .base import BaseTreeClassifierMixin, BaseTreeEstimatorMixin, BaseTreeRegressorMixin
 
 
 # pylint: disable=too-many-instance-attributes
 class RandomForestClassifier(BaseTreeClassifierMixin):
     """Implements the RandomForest classifier."""
 
-    sklearn_alg = sklearn.ensemble.RandomForestClassifier
-    q_x_byfeatures: List[QuantizedArray]
-    n_bits: int
-    q_y: QuantizedArray
-    _tensor_tree_predict: Optional[Callable]
-    sklearn_model: Any
-    framework: str = "sklearn"
-
+    sklearn_model_class = SklearnRandomForestClassifier
+    framework = "sklearn"
     _is_a_public_cml_model = True
 
-    # pylint: disable=too-many-arguments,protected-access
-
+    # pylint: disable-next=too-many-arguments
     def __init__(
         self,
         n_bits: int = 6,
         n_estimators=20,
         criterion="gini",
         max_depth=4,
         min_samples_split=2,
@@ -45,17 +42,17 @@
         ccp_alpha=0.0,
         max_samples=None,
     ):
         """Initialize the RandomForestClassifier.
 
         # noqa: DAR101
         """
+        # Call BaseClassifier's __init__ method
+        super().__init__(n_bits=n_bits)
 
-        # FIXME #893
-        BaseTreeClassifierMixin.__init__(self, n_bits=n_bits)
         self.n_estimators = n_estimators
         self.bootstrap = bootstrap
         self.oob_score = oob_score
         self.n_jobs = n_jobs
         self.random_state = random_state
         self.verbose = verbose
         self.warm_start = warm_start
@@ -67,30 +64,126 @@
         self.min_samples_leaf = min_samples_leaf
         self.min_weight_fraction_leaf = min_weight_fraction_leaf
         self.max_features = max_features
         self.max_leaf_nodes = max_leaf_nodes
         self.min_impurity_decrease = min_impurity_decrease
         self.ccp_alpha = ccp_alpha
 
+    def post_processing(self, y_preds: numpy.ndarray) -> numpy.ndarray:
+        # Here, we want to use BaseTreeEstimatorMixin's `post-processing` method as
+        # RandomForestClassifier models directly computes probabilities and therefore don't require
+        # to apply a sigmoid or softmax in post-processing
+        return BaseTreeEstimatorMixin.post_processing(self, y_preds)
+
+    def dump_dict(self) -> Dict[str, Any]:
+        metadata: Dict[str, Any] = {}
+
+        metadata["post_processing_params"] = self.post_processing_params
+        metadata["cml_dumped_class_name"] = str(type(self).__name__)
+        metadata["n_bits"] = self.n_bits
+        metadata["input_quantizers"] = [elt.dumps() for elt in self.input_quantizers]
+        metadata["output_quantizers"] = [elt.dumps() for elt in self.output_quantizers]
+        metadata["sklearn_model_class"] = self.sklearn_model_class
+        metadata["sklearn_model"] = self.sklearn_model
+        metadata["onnx_model_"] = self.onnx_model_
+        metadata["_is_fitted"] = self._is_fitted
+        metadata["_is_compiled"] = self._is_compiled
+        metadata["framework"] = self.framework
+
+        # Classifier
+        metadata["classes_"] = self.target_classes_
+        metadata["n_classes_"] = self.n_classes_
+
+        metadata["n_estimators"] = self.n_estimators
+        metadata["bootstrap"] = self.bootstrap
+        metadata["oob_score"] = self.oob_score
+        metadata["n_jobs"] = self.n_jobs
+        metadata["random_state"] = self.random_state
+        metadata["verbose"] = self.verbose
+        metadata["warm_start"] = self.warm_start
+        metadata["class_weight"] = self.class_weight
+        metadata["max_samples"] = self.max_samples
+        metadata["criterion"] = self.criterion
+        metadata["max_depth"] = self.max_depth
+        metadata["min_samples_split"] = self.min_samples_split
+        metadata["min_samples_leaf"] = self.min_samples_leaf
+        metadata["min_weight_fraction_leaf"] = self.min_weight_fraction_leaf
+        metadata["max_features"] = self.max_features
+        metadata["max_leaf_nodes"] = self.max_leaf_nodes
+        metadata["min_impurity_decrease"] = self.min_impurity_decrease
+        metadata["ccp_alpha"] = self.ccp_alpha
+
+        return metadata
+
+    @classmethod
+    def load_dict(cls, metadata: Dict):
+        obj = RandomForestClassifier(n_bits=metadata["n_bits"])
+
+        # Tree
+        obj.input_quantizers = [UniformQuantizer.loads(elt) for elt in metadata["input_quantizers"]]
+        obj.output_quantizers = [
+            UniformQuantizer.loads(elt) for elt in metadata["output_quantizers"]
+        ]
+
+        # Load the underlying fitted model
+        loads_sklearn_kwargs = {}
+        if USE_SKOPS:
+            loads_sklearn_kwargs["trusted"] = TRUSTED_SKOPS
+        obj.sklearn_model = loads_sklearn(
+            bytes.fromhex(metadata["sklearn_model"]), **loads_sklearn_kwargs
+        )
+
+        obj.framework = metadata["framework"]
+
+        obj._tree_inference, obj.output_quantizers, obj.onnx_model_ = tree_to_numpy(
+            obj.sklearn_model,
+            numpy.zeros((len(obj.input_quantizers),))[None, ...],
+            framework=obj.framework,
+            output_n_bits=obj.n_bits,
+        )
+
+        obj.post_processing_params = metadata["post_processing_params"]
+        obj._is_fitted = metadata["_is_fitted"]
+        obj._is_compiled = metadata["_is_compiled"]
+
+        # Classifier
+        obj.target_classes_ = numpy.array(metadata["classes_"])
+        obj.n_classes_ = metadata["n_classes_"]
+
+        obj.n_estimators = metadata["n_estimators"]
+        obj.bootstrap = metadata["bootstrap"]
+        obj.oob_score = metadata["oob_score"]
+        obj.n_jobs = metadata["n_jobs"]
+        obj.random_state = metadata["random_state"]
+        obj.verbose = metadata["verbose"]
+        obj.warm_start = metadata["warm_start"]
+        obj.class_weight = metadata["class_weight"]
+        obj.max_samples = metadata["max_samples"]
+        obj.criterion = metadata["criterion"]
+        obj.max_depth = metadata["max_depth"]
+        obj.min_samples_split = metadata["min_samples_split"]
+        obj.min_samples_leaf = metadata["min_samples_leaf"]
+        obj.min_weight_fraction_leaf = metadata["min_weight_fraction_leaf"]
+        obj.max_features = metadata["max_features"]
+        obj.max_leaf_nodes = metadata["max_leaf_nodes"]
+        obj.min_impurity_decrease = metadata["min_impurity_decrease"]
+        obj.ccp_alpha = metadata["ccp_alpha"]
+
+        return obj
+
 
 # pylint: disable=too-many-instance-attributes
 class RandomForestRegressor(BaseTreeRegressorMixin):
     """Implements the RandomForest regressor."""
 
-    sklearn_alg = sklearn.ensemble.RandomForestRegressor
-    q_x_byfeatures: List[QuantizedArray]
-    n_bits: int
-    q_y: QuantizedArray
-    _tensor_tree_predict: Optional[Callable]
-    sklearn_model: Any
-    framework: str = "sklearn"
+    sklearn_model_class = SklearnRandomForestRegressor
+    framework = "sklearn"
     _is_a_public_cml_model = True
 
-    # pylint: disable=too-many-arguments,protected-access
-
+    # pylint: disable-next=too-many-arguments
     def __init__(
         self,
         n_bits: int = 6,
         n_estimators=20,
         criterion="squared_error",
         max_depth=4,
         min_samples_split=2,
@@ -108,17 +201,17 @@
         ccp_alpha=0.0,
         max_samples=None,
     ):
         """Initialize the RandomForestRegressor.
 
         # noqa: DAR101
         """
+        # Call BaseTreeEstimatorMixin's __init__ method
+        super().__init__(n_bits=n_bits)
 
-        # FIXME #893
-        BaseTreeRegressorMixin.__init__(self, n_bits=n_bits)
         self.n_estimators = n_estimators
         self.bootstrap = bootstrap
         self.oob_score = oob_score
         self.n_jobs = n_jobs
         self.random_state = random_state
         self.verbose = verbose
         self.warm_start = warm_start
@@ -128,7 +221,93 @@
         self.min_samples_split = min_samples_split
         self.min_samples_leaf = min_samples_leaf
         self.min_weight_fraction_leaf = min_weight_fraction_leaf
         self.max_features = max_features
         self.max_leaf_nodes = max_leaf_nodes
         self.min_impurity_decrease = min_impurity_decrease
         self.ccp_alpha = ccp_alpha
+
+    def dump_dict(self) -> Dict[str, Any]:
+        metadata: Dict[str, Any] = {}
+
+        metadata["post_processing_params"] = self.post_processing_params
+        metadata["cml_dumped_class_name"] = str(type(self).__name__)
+        metadata["n_bits"] = self.n_bits
+        metadata["input_quantizers"] = [elt.dumps() for elt in self.input_quantizers]
+        metadata["output_quantizers"] = [elt.dumps() for elt in self.output_quantizers]
+        metadata["sklearn_model_class"] = self.sklearn_model_class
+        metadata["sklearn_model"] = self.sklearn_model
+        metadata["onnx_model_"] = self.onnx_model_
+        metadata["_is_fitted"] = self._is_fitted
+        metadata["_is_compiled"] = self._is_compiled
+        metadata["framework"] = self.framework
+
+        metadata["n_estimators"] = self.n_estimators
+        metadata["bootstrap"] = self.bootstrap
+        metadata["oob_score"] = self.oob_score
+        metadata["n_jobs"] = self.n_jobs
+        metadata["random_state"] = self.random_state
+        metadata["verbose"] = self.verbose
+        metadata["warm_start"] = self.warm_start
+        metadata["max_samples"] = self.max_samples
+        metadata["criterion"] = self.criterion
+        metadata["max_depth"] = self.max_depth
+        metadata["min_samples_split"] = self.min_samples_split
+        metadata["min_samples_leaf"] = self.min_samples_leaf
+        metadata["min_weight_fraction_leaf"] = self.min_weight_fraction_leaf
+        metadata["max_features"] = self.max_features
+        metadata["max_leaf_nodes"] = self.max_leaf_nodes
+        metadata["min_impurity_decrease"] = self.min_impurity_decrease
+        metadata["ccp_alpha"] = self.ccp_alpha
+
+        return metadata
+
+    @classmethod
+    def load_dict(cls, metadata: Dict):
+        obj = RandomForestRegressor(n_bits=metadata["n_bits"])
+
+        # Tree
+        obj.input_quantizers = [UniformQuantizer.loads(elt) for elt in metadata["input_quantizers"]]
+        obj.output_quantizers = [
+            UniformQuantizer.loads(elt) for elt in metadata["output_quantizers"]
+        ]
+
+        # Load the underlying fitted model
+        loads_sklearn_kwargs = {}
+        if USE_SKOPS:
+            loads_sklearn_kwargs["trusted"] = TRUSTED_SKOPS
+        obj.sklearn_model = loads_sklearn(
+            bytes.fromhex(metadata["sklearn_model"]), **loads_sklearn_kwargs
+        )
+
+        obj.framework = metadata["framework"]
+
+        obj._tree_inference, obj.output_quantizers, obj.onnx_model_ = tree_to_numpy(
+            obj.sklearn_model,
+            numpy.zeros((len(obj.input_quantizers),))[None, ...],
+            framework=obj.framework,
+            output_n_bits=obj.n_bits,
+        )
+
+        obj.post_processing_params = metadata["post_processing_params"]
+        obj._is_fitted = metadata["_is_fitted"]
+        obj._is_compiled = metadata["_is_compiled"]
+
+        obj.n_estimators = metadata["n_estimators"]
+        obj.bootstrap = metadata["bootstrap"]
+        obj.oob_score = metadata["oob_score"]
+        obj.n_jobs = metadata["n_jobs"]
+        obj.random_state = metadata["random_state"]
+        obj.verbose = metadata["verbose"]
+        obj.warm_start = metadata["warm_start"]
+        obj.max_samples = metadata["max_samples"]
+        obj.criterion = metadata["criterion"]
+        obj.max_depth = metadata["max_depth"]
+        obj.min_samples_split = metadata["min_samples_split"]
+        obj.min_samples_leaf = metadata["min_samples_leaf"]
+        obj.min_weight_fraction_leaf = metadata["min_weight_fraction_leaf"]
+        obj.max_features = metadata["max_features"]
+        obj.max_leaf_nodes = metadata["max_leaf_nodes"]
+        obj.min_impurity_decrease = metadata["min_impurity_decrease"]
+        obj.ccp_alpha = metadata["ccp_alpha"]
+
+        return obj
```

## concrete/ml/sklearn/svm.py

```diff
@@ -1,15 +1,20 @@
 """Implement Support Vector Machine."""
+from typing import Any, Dict
+
+import numpy
 import sklearn.linear_model
 
-from .base import SklearnLinearClassifierMixin, SklearnLinearModelMixin
+from .. import TRUSTED_SKOPS, USE_SKOPS, loads_sklearn
+from ..quantization.quantizers import UniformQuantizer
+from .base import SklearnLinearClassifierMixin, SklearnLinearRegressorMixin
 
 
 # pylint: disable=invalid-name,too-many-instance-attributes
-class LinearSVR(SklearnLinearModelMixin, sklearn.base.RegressorMixin):
+class LinearSVR(SklearnLinearRegressorMixin):
     """A Regression Support Vector Machine (SVM).
 
     Parameters:
         n_bits (int, Dict[str, int]): Number of bits to quantize the model. If an int is passed
             for n_bits, the value will be used for quantizing inputs and weights. If a dict is
             passed, then it should contain "op_inputs" and "op_weights" as keys with
             corresponding number of quantization bits so that:
@@ -17,15 +22,15 @@
             - op_weights: number of bits to quantize the learned parameters
             Default to 8.
 
     For more details on LinearSVR please refer to the scikit-learn documentation:
     https://scikit-learn.org/stable/modules/generated/sklearn.svm.LinearSVR.html
     """
 
-    sklearn_alg = sklearn.svm.LinearSVR
+    sklearn_model_class = sklearn.svm.LinearSVR
     _is_a_public_cml_model = True
 
     # pylint: disable-next=too-many-arguments
     def __init__(
         self,
         n_bits=8,
         epsilon=0.0,
@@ -35,31 +40,106 @@
         fit_intercept=True,
         intercept_scaling=1.0,
         dual=True,
         verbose=0,
         random_state=None,
         max_iter=1000,
     ):
-        # FIXME: Figure out how to add scikit-learn documentation into our object #893
+        # Call SklearnLinearModelMixin's __init__ method
+        super().__init__(n_bits=n_bits)
+
         self.epsilon = epsilon
         self.tol = tol
         self.C = C
         self.loss = loss
         self.fit_intercept = fit_intercept
         self.intercept_scaling = intercept_scaling
         self.dual = dual
         self.verbose = verbose
         self.random_state = random_state
         self.max_iter = max_iter
-        self.n_bits = n_bits
-        self._onnx = None
-        super().__init__(n_bits=n_bits)
+
+    def dump_dict(self) -> Dict[str, Any]:
+        assert self._weight_quantizer is not None, self._is_not_fitted_error_message()
+
+        metadata: Dict[str, Any] = {}
+
+        metadata["post_processing_params"] = self.post_processing_params
+        metadata["cml_dumped_class_name"] = type(self).__name__
+
+        # Linear
+        metadata["n_bits"] = self.n_bits
+        metadata["sklearn_model"] = self.sklearn_model
+        metadata["sklearn_model_class"] = self.sklearn_model_class
+        metadata["fhe_circuit"] = self.fhe_circuit
+        metadata["input_quantizers"] = [elt.dumps() for elt in self.input_quantizers]
+        metadata["_weight_quantizer"] = self._weight_quantizer.dumps()
+        metadata["output_quantizers"] = [elt.dumps() for elt in self.output_quantizers]
+        metadata["onnx_model_"] = self.onnx_model_
+        metadata["_is_fitted"] = self._is_fitted
+        metadata["_is_compiled"] = self._is_compiled
+        metadata["_q_weights"] = self._q_weights
+        metadata["_q_bias"] = self._q_bias
+
+        metadata["epsilon"] = self.epsilon
+        metadata["tol"] = self.tol
+        metadata["C"] = self.C
+        metadata["loss"] = self.loss
+        metadata["fit_intercept"] = self.fit_intercept
+        metadata["intercept_scaling"] = self.intercept_scaling
+        metadata["dual"] = self.dual
+        metadata["verbose"] = self.verbose
+        metadata["random_state"] = self.random_state
+        metadata["max_iter"] = self.max_iter
+
+        return metadata
+
+    @classmethod
+    def load_dict(cls, metadata: Dict):
+        obj = LinearSVR()
+        obj.post_processing_params = metadata["post_processing_params"]
+
+        # Load the underlying fitted model
+        loads_sklearn_kwargs = {}
+        if USE_SKOPS:
+            loads_sklearn_kwargs["trusted"] = TRUSTED_SKOPS
+        obj.sklearn_model = loads_sklearn(
+            bytes.fromhex(metadata["sklearn_model"]), **loads_sklearn_kwargs
+        )
+
+        # Linear
+        obj.n_bits = metadata["n_bits"]
+        obj.sklearn_model_class = metadata["sklearn_model_class"]
+        obj.fhe_circuit = metadata["fhe_circuit"]
+        obj.input_quantizers = [UniformQuantizer.loads(elt) for elt in metadata["input_quantizers"]]
+        obj.output_quantizers = [
+            UniformQuantizer.loads(elt) for elt in metadata["output_quantizers"]
+        ]
+        obj._weight_quantizer = UniformQuantizer.loads(metadata["_weight_quantizer"])
+        obj.onnx_model_ = metadata["onnx_model_"]
+        obj._is_fitted = metadata["_is_fitted"]
+        obj._is_compiled = metadata["_is_compiled"]
+        obj._q_weights = metadata["_q_weights"]
+        obj._q_bias = metadata["_q_bias"]
+
+        obj.epsilon = metadata["epsilon"]
+        obj.tol = metadata["tol"]
+        obj.C = metadata["C"]
+        obj.loss = metadata["loss"]
+        obj.fit_intercept = metadata["fit_intercept"]
+        obj.intercept_scaling = metadata["intercept_scaling"]
+        obj.dual = metadata["dual"]
+        obj.verbose = metadata["verbose"]
+        obj.random_state = metadata["random_state"]
+        obj.max_iter = metadata["max_iter"]
+
+        return obj
 
 
-class LinearSVC(SklearnLinearClassifierMixin, sklearn.base.ClassifierMixin):
+class LinearSVC(SklearnLinearClassifierMixin):
     """A Classification Support Vector Machine (SVM).
 
     Parameters:
         n_bits (int, Dict[str, int]): Number of bits to quantize the model. If an int is passed
             for n_bits, the value will be used for quantizing inputs and weights. If a dict is
             passed, then it should contain "op_inputs" and "op_weights" as keys with
             corresponding number of quantization bits so that:
@@ -67,15 +147,15 @@
             - op_weights: number of bits to quantize the learned parameters
             Default to 8.
 
     For more details on LinearSVC please refer to the scikit-learn documentation:
     https://scikit-learn.org/stable/modules/generated/sklearn.svm.LinearSVC.html
     """
 
-    sklearn_alg = sklearn.svm.LinearSVC
+    sklearn_model_class = sklearn.svm.LinearSVC
     _is_a_public_cml_model = True
 
     # pylint: disable-next=too-many-arguments
     def __init__(
         self,
         n_bits=8,
         penalty="l2",
@@ -88,25 +168,114 @@
         fit_intercept=True,
         intercept_scaling=1,
         class_weight=None,
         verbose=0,
         random_state=None,
         max_iter=1000,
     ):
+        # Call BaseClassifier's __init__ method
+        super().__init__(n_bits=n_bits)
+
         self.penalty = penalty
         self.loss = loss
         self.dual = dual
         self.tol = tol
         self.C = C
         self.multi_class = multi_class
         self.fit_intercept = fit_intercept
         self.intercept_scaling = intercept_scaling
         self.class_weight = class_weight
         self.verbose = verbose
         self.random_state = random_state
         self.max_iter = max_iter
-        self.n_bits = n_bits
-        self._onnx = None
-        super().__init__(n_bits=n_bits)
+
+    def dump_dict(self) -> Dict[str, Any]:
+        assert self._weight_quantizer is not None, self._is_not_fitted_error_message()
+
+        metadata: Dict[str, Any] = {}
+
+        metadata["post_processing_params"] = self.post_processing_params
+        metadata["cml_dumped_class_name"] = type(self).__name__
+
+        # Classifier
+        metadata["classes_"] = self.target_classes_
+        metadata["n_classes_"] = self.n_classes_
+        metadata["cml_dumped_class_name"] = type(self).__name__
+
+        # Linear
+        metadata["n_bits"] = self.n_bits
+        metadata["sklearn_model"] = self.sklearn_model
+        metadata["sklearn_model_class"] = self.sklearn_model_class
+        metadata["fhe_circuit"] = self.fhe_circuit
+        metadata["input_quantizers"] = [elt.dumps() for elt in self.input_quantizers]
+        metadata["_weight_quantizer"] = self._weight_quantizer.dumps()
+        metadata["output_quantizers"] = [elt.dumps() for elt in self.output_quantizers]
+        metadata["onnx_model_"] = self.onnx_model_
+        metadata["_is_fitted"] = self._is_fitted
+        metadata["_is_compiled"] = self._is_compiled
+        metadata["_q_weights"] = self._q_weights
+        metadata["_q_bias"] = self._q_bias
+
+        metadata["penalty"] = self.penalty
+        metadata["loss"] = self.loss
+        metadata["dual"] = self.dual
+        metadata["tol"] = self.tol
+        metadata["C"] = self.C
+        metadata["multi_class"] = self.multi_class
+        metadata["fit_intercept"] = self.fit_intercept
+        metadata["intercept_scaling"] = self.intercept_scaling
+        metadata["class_weight"] = self.class_weight
+        metadata["verbose"] = self.verbose
+        metadata["random_state"] = self.random_state
+        metadata["max_iter"] = self.max_iter
+
+        return metadata
+
+    @classmethod
+    def load_dict(cls, metadata: Dict):
+        obj = LinearSVC()
+        obj.post_processing_params = metadata["post_processing_params"]
+
+        # Load the underlying fitted model
+        loads_sklearn_kwargs = {}
+        if USE_SKOPS:
+            loads_sklearn_kwargs["trusted"] = TRUSTED_SKOPS
+        obj.sklearn_model = loads_sklearn(
+            bytes.fromhex(metadata["sklearn_model"]), **loads_sklearn_kwargs
+        )
+
+        # Classifier
+        obj.target_classes_ = numpy.array(metadata["classes_"])
+        obj.n_classes_ = metadata["n_classes_"]
+
+        # Linear
+        obj.n_bits = metadata["n_bits"]
+        obj.sklearn_model_class = metadata["sklearn_model_class"]
+        obj.fhe_circuit = metadata["fhe_circuit"]
+        obj.input_quantizers = [UniformQuantizer.loads(elt) for elt in metadata["input_quantizers"]]
+        obj.output_quantizers = [
+            UniformQuantizer.loads(elt) for elt in metadata["output_quantizers"]
+        ]
+        obj._weight_quantizer = UniformQuantizer.loads(metadata["_weight_quantizer"])
+        obj.onnx_model_ = metadata["onnx_model_"]
+        obj._is_fitted = metadata["_is_fitted"]
+        obj._is_compiled = metadata["_is_compiled"]
+        obj._q_weights = metadata["_q_weights"]
+        obj._q_bias = metadata["_q_bias"]
+
+        obj.penalty = metadata["penalty"]
+        obj.loss = metadata["loss"]
+        obj.dual = metadata["dual"]
+        obj.tol = metadata["tol"]
+        obj.C = metadata["C"]
+        obj.multi_class = metadata["multi_class"]
+        obj.fit_intercept = metadata["fit_intercept"]
+        obj.intercept_scaling = metadata["intercept_scaling"]
+        obj.class_weight = metadata["class_weight"]
+        obj.verbose = metadata["verbose"]
+        obj.random_state = metadata["random_state"]
+        obj.max_iter = metadata["max_iter"]
+
+        return obj
 
 
 # pylint: enable=invalid-name,too-many-instance-attributes
```

## concrete/ml/sklearn/tree.py

```diff
@@ -1,31 +1,26 @@
-"""Implement the sklearn tree models."""
-from typing import Callable, Optional
+"""Implement DecisionTree models."""
+from typing import Any, Dict
 
-import sklearn
-from concrete.numpy.compilation.circuit import Circuit
-
-from ..quantization.quantizers import QuantizedArray
-from .base import BaseTreeClassifierMixin, BaseTreeRegressorMixin
+import numpy
+from sklearn.tree import DecisionTreeClassifier as SklearnDecisionTreeClassifier
+from sklearn.tree import DecisionTreeRegressor as SklearnDecisionTreeRegressor
+
+from .. import TRUSTED_SKOPS, USE_SKOPS, loads_sklearn
+from ..quantization.quantizers import UniformQuantizer
+from ..sklearn.tree_to_numpy import tree_to_numpy
+from .base import BaseTreeClassifierMixin, BaseTreeEstimatorMixin, BaseTreeRegressorMixin
 
 
 # pylint: disable-next=too-many-instance-attributes
 class DecisionTreeClassifier(BaseTreeClassifierMixin):
     """Implements the sklearn DecisionTreeClassifier."""
 
-    sklearn_alg = sklearn.tree.DecisionTreeClassifier
-    q_x_byfeatures: list
-    fhe_tree: Circuit
-    _tensor_tree_predict: Optional[Callable]
-    q_y: QuantizedArray
-    class_mapping_: Optional[dict]
-    n_classes_: int
-    framework: str = "sklearn"
-
-    # pylint: disable-next=protected-access
+    sklearn_model_class = SklearnDecisionTreeClassifier
+    framework = "sklearn"
     _is_a_public_cml_model = True
 
     # pylint: disable-next=too-many-arguments
     def __init__(
         self,
         criterion="gini",
         splitter="best",
@@ -42,47 +37,127 @@
         n_bits: int = 6,
     ):
         """Initialize the DecisionTreeClassifier.
 
         # noqa: DAR101
 
         """
+        # Call BaseClassifier's __init__ method
+        super().__init__(n_bits=n_bits)
 
         self.criterion = criterion
         self.splitter = splitter
         self.max_depth = max_depth
         self.min_samples_split = min_samples_split
         self.min_samples_leaf = min_samples_leaf
         self.min_weight_fraction_leaf = min_weight_fraction_leaf
         self.max_features = max_features
         self.max_leaf_nodes = max_leaf_nodes
         self.class_weight = class_weight
         self.random_state = random_state
         self.min_impurity_decrease = min_impurity_decrease
         self.ccp_alpha = ccp_alpha
 
-        BaseTreeClassifierMixin.__init__(self, n_bits=n_bits)
-        self.q_x_byfeatures = []
-        self.n_bits = n_bits
-        self.fhe_tree = None
-        self.class_mapping_ = None
+    def post_processing(self, y_preds: numpy.ndarray) -> numpy.ndarray:
+        # Here, we want to use BaseTreeEstimatorMixin's `post-processing` method as
+        # DecisionTreeClassifier models directly computes probabilities and therefore don't require
+        # to apply a sigmoid or softmax in post-processing
+        return BaseTreeEstimatorMixin.post_processing(self, y_preds)
+
+    def dump_dict(self) -> Dict[str, Any]:
+        metadata: Dict[str, Any] = {}
+
+        metadata["post_processing_params"] = self.post_processing_params
+        metadata["cml_dumped_class_name"] = str(type(self).__name__)
+        metadata["n_bits"] = self.n_bits
+        metadata["input_quantizers"] = [elt.dumps() for elt in self.input_quantizers]
+        metadata["output_quantizers"] = [elt.dumps() for elt in self.output_quantizers]
+        metadata["sklearn_model_class"] = self.sklearn_model_class
+        metadata["sklearn_model"] = self.sklearn_model
+        metadata["onnx_model_"] = self.onnx_model_
+        metadata["_is_fitted"] = self._is_fitted
+        metadata["_is_compiled"] = self._is_compiled
+        metadata["framework"] = self.framework
+
+        # Classifier
+        metadata["classes_"] = self.target_classes_
+        metadata["n_classes_"] = self.n_classes_
+
+        metadata["criterion"] = self.criterion
+        metadata["splitter"] = self.splitter
+        metadata["max_depth"] = self.max_depth
+        metadata["min_samples_split"] = self.min_samples_split
+        metadata["min_samples_leaf"] = self.min_samples_leaf
+        metadata["min_weight_fraction_leaf"] = self.min_weight_fraction_leaf
+        metadata["max_features"] = self.max_features
+        metadata["max_leaf_nodes"] = self.max_leaf_nodes
+        metadata["class_weight"] = self.class_weight
+        metadata["random_state"] = self.random_state
+        metadata["min_impurity_decrease"] = self.min_impurity_decrease
+        metadata["ccp_alpha"] = self.ccp_alpha
+
+        return metadata
+
+    @classmethod
+    def load_dict(cls, metadata: Dict):
+        obj = cls(n_bits=metadata["n_bits"])
+
+        # Tree
+        obj.input_quantizers = [UniformQuantizer.loads(elt) for elt in metadata["input_quantizers"]]
+        obj.output_quantizers = [
+            UniformQuantizer.loads(elt) for elt in metadata["output_quantizers"]
+        ]
+
+        # Load the underlying fitted model
+        loads_sklearn_kwargs = {}
+        if USE_SKOPS:
+            loads_sklearn_kwargs["trusted"] = TRUSTED_SKOPS
+        obj.sklearn_model = loads_sklearn(
+            bytes.fromhex(metadata["sklearn_model"]), **loads_sklearn_kwargs
+        )
+
+        obj.framework = metadata["framework"]
+
+        obj._tree_inference, obj.output_quantizers, obj.onnx_model_ = tree_to_numpy(
+            obj.sklearn_model,
+            numpy.zeros((len(obj.input_quantizers),))[None, ...],
+            framework=obj.framework,
+            output_n_bits=obj.n_bits,
+        )
+
+        obj.post_processing_params = metadata["post_processing_params"]
+        obj._is_fitted = metadata["_is_fitted"]
+        obj._is_compiled = metadata["_is_compiled"]
+
+        # Classifier
+        obj.target_classes_ = numpy.array(metadata["classes_"])
+        obj.n_classes_ = metadata["n_classes_"]
+
+        obj.criterion = metadata["criterion"]
+        obj.splitter = metadata["splitter"]
+        obj.max_depth = metadata["max_depth"]
+        obj.min_samples_split = metadata["min_samples_split"]
+        obj.min_samples_leaf = metadata["min_samples_leaf"]
+        obj.min_weight_fraction_leaf = metadata["min_weight_fraction_leaf"]
+        obj.max_features = metadata["max_features"]
+        obj.max_leaf_nodes = metadata["max_leaf_nodes"]
+        obj.class_weight = metadata["class_weight"]
+        obj.random_state = metadata["random_state"]
+        obj.min_impurity_decrease = metadata["min_impurity_decrease"]
+        obj.ccp_alpha = metadata["ccp_alpha"]
+
+        return obj
 
 
 # pylint: disable-next=too-many-instance-attributes
 class DecisionTreeRegressor(BaseTreeRegressorMixin):
     """Implements the sklearn DecisionTreeClassifier."""
 
-    sklearn_alg = sklearn.tree.DecisionTreeRegressor
-    q_x_byfeatures: list
-    fhe_tree: Circuit
-    _tensor_tree_predict: Optional[Callable]
-    q_y: QuantizedArray
-    framework: str = "sklearn"
-
-    # pylint: disable-next=protected-access
+    sklearn_model_class = SklearnDecisionTreeRegressor
+    framework = "sklearn"
     _is_a_public_cml_model = True
 
     # pylint: disable-next=too-many-arguments
     def __init__(
         self,
         criterion="squared_error",
         splitter="best",
@@ -98,25 +173,95 @@
         n_bits: int = 6,
     ):
         """Initialize the DecisionTreeRegressor.
 
         # noqa: DAR101
 
         """
+        # Call BaseTreeEstimatorMixin's __init__ method
+        super().__init__(n_bits=n_bits)
 
         self.criterion = criterion
         self.splitter = splitter
         self.max_depth = max_depth
         self.min_samples_split = min_samples_split
         self.min_samples_leaf = min_samples_leaf
         self.min_weight_fraction_leaf = min_weight_fraction_leaf
         self.max_features = max_features
         self.max_leaf_nodes = max_leaf_nodes
         self.random_state = random_state
         self.min_impurity_decrease = min_impurity_decrease
         self.ccp_alpha = ccp_alpha
 
-        BaseTreeRegressorMixin.__init__(self, n_bits=n_bits)
-        self.q_x_byfeatures = []
-        self.n_bits = n_bits
-        self.fhe_tree = None
-        self.class_mapping_ = None
+    def dump_dict(self) -> Dict[str, Any]:
+        metadata: Dict[str, Any] = {}
+
+        metadata["post_processing_params"] = self.post_processing_params
+        metadata["cml_dumped_class_name"] = str(type(self).__name__)
+        metadata["n_bits"] = self.n_bits
+        metadata["input_quantizers"] = [elt.dumps() for elt in self.input_quantizers]
+        metadata["output_quantizers"] = [elt.dumps() for elt in self.output_quantizers]
+        metadata["sklearn_model_class"] = self.sklearn_model_class
+        metadata["sklearn_model"] = self.sklearn_model
+        metadata["onnx_model_"] = self.onnx_model_
+        metadata["_is_fitted"] = self._is_fitted
+        metadata["_is_compiled"] = self._is_compiled
+        metadata["framework"] = self.framework
+
+        metadata["criterion"] = self.criterion
+        metadata["splitter"] = self.splitter
+        metadata["max_depth"] = self.max_depth
+        metadata["min_samples_split"] = self.min_samples_split
+        metadata["min_samples_leaf"] = self.min_samples_leaf
+        metadata["min_weight_fraction_leaf"] = self.min_weight_fraction_leaf
+        metadata["max_features"] = self.max_features
+        metadata["max_leaf_nodes"] = self.max_leaf_nodes
+        metadata["random_state"] = self.random_state
+        metadata["min_impurity_decrease"] = self.min_impurity_decrease
+        metadata["ccp_alpha"] = self.ccp_alpha
+
+        return metadata
+
+    @classmethod
+    def load_dict(cls, metadata: Dict):
+        obj = cls(n_bits=metadata["n_bits"])
+
+        # Tree
+        obj.input_quantizers = [UniformQuantizer.loads(elt) for elt in metadata["input_quantizers"]]
+        obj.output_quantizers = [
+            UniformQuantizer.loads(elt) for elt in metadata["output_quantizers"]
+        ]
+
+        # Load the underlying fitted model
+        loads_sklearn_kwargs = {}
+        if USE_SKOPS:
+            loads_sklearn_kwargs["trusted"] = TRUSTED_SKOPS
+        obj.sklearn_model = loads_sklearn(
+            bytes.fromhex(metadata["sklearn_model"]), **loads_sklearn_kwargs
+        )
+
+        obj.framework = metadata["framework"]
+
+        obj._tree_inference, obj.output_quantizers, obj.onnx_model_ = tree_to_numpy(
+            obj.sklearn_model,
+            numpy.zeros((len(obj.input_quantizers),))[None, ...],
+            framework=obj.framework,
+            output_n_bits=obj.n_bits,
+        )
+
+        obj.post_processing_params = metadata["post_processing_params"]
+        obj._is_fitted = metadata["_is_fitted"]
+        obj._is_compiled = metadata["_is_compiled"]
+
+        obj.criterion = metadata["criterion"]
+        obj.splitter = metadata["splitter"]
+        obj.max_depth = metadata["max_depth"]
+        obj.min_samples_split = metadata["min_samples_split"]
+        obj.min_samples_leaf = metadata["min_samples_leaf"]
+        obj.min_weight_fraction_leaf = metadata["min_weight_fraction_leaf"]
+        obj.max_features = metadata["max_features"]
+        obj.max_leaf_nodes = metadata["max_leaf_nodes"]
+        obj.random_state = metadata["random_state"]
+        obj.min_impurity_decrease = metadata["min_impurity_decrease"]
+        obj.ccp_alpha = metadata["ccp_alpha"]
+
+        return obj
```

## concrete/ml/sklearn/tree_to_numpy.py

```diff
@@ -1,77 +1,49 @@
 """Implements the conversion of a tree model to a numpy function."""
 import warnings
-from enum import Enum
-from typing import Callable, List, Optional, Tuple
+from typing import Callable, List, Tuple
 
 import numpy
 import onnx
 from onnx import numpy_helper
 
 from ..common.debugging.custom_assert import assert_true
-from ..common.utils import MAX_BITWIDTH_BACKWARD_COMPATIBLE, get_onnx_opset_version
-from ..onnx.convert import OPSET_VERSION_FOR_ONNX_EXPORT, get_equivalent_numpy_forward
-from ..onnx.onnx_model_manipulations import (
-    clean_graph_after_node_name,
-    keep_following_outputs_discard_others,
-    remove_node_types,
+from ..common.utils import (
+    MAX_BITWIDTH_BACKWARD_COMPATIBLE,
+    get_onnx_opset_version,
+    is_regressor_or_partial_regressor,
 )
+from ..onnx.convert import OPSET_VERSION_FOR_ONNX_EXPORT, get_equivalent_numpy_forward
+from ..onnx.onnx_model_manipulations import clean_graph_at_node_op_type, remove_node_types
 from ..quantization import QuantizedArray
 from ..quantization.quantizers import UniformQuantizer
 
 # pylint: disable=wrong-import-position,wrong-import-order
 
 # Silence hummingbird warnings
 warnings.filterwarnings("ignore")
 from hummingbird.ml import convert as hb_convert  # noqa: E402
 
 # pylint: enable=wrong-import-position,wrong-import-order
 
 # pylint: disable=too-many-branches
 
 
-class Task(Enum):
-    """Task enumerate."""
-
-    CLASSIFICATION = "classification"
-    REGRESSION = "regression"
-
-
-EXPECTED_NUMBER_OF_OUTPUTS_PER_TASK = {Task.CLASSIFICATION: 2, Task.REGRESSION: 1}
-
-
-def tree_to_numpy(
-    model: onnx.ModelProto,
-    x: numpy.ndarray,
-    framework: str,
-    task: Task,
-    output_n_bits: Optional[int] = MAX_BITWIDTH_BACKWARD_COMPATIBLE,
-) -> Tuple[Callable, List[UniformQuantizer], onnx.ModelProto]:
-    """Convert the tree inference to a numpy functions using Hummingbird.
+def get_onnx_model(model: Callable, x: numpy.ndarray, framework: str) -> onnx.ModelProto:
+    """Create ONNX model with Hummingbird convert method.
 
     Args:
-        model (onnx.ModelProto): The model to convert.
-        x (numpy.ndarray): The input data.
-        framework (str): The framework from which the onnx_model is generated.
+        model (Callable): The tree model to convert.
+        x (numpy.ndarray): Dataset used to trace the tree inference and convert the model to ONNX.
+        framework (str): The framework from which the ONNX model is generated.
             (options: 'xgboost', 'sklearn')
-        task (Task): The task the model is solving
-        output_n_bits (int): The number of bits of the output.
 
     Returns:
-        Tuple[Callable, List[QuantizedArray], onnx.ModelProto]: A tuple with a function that takes a
-            numpy array and returns a numpy array, QuantizedArray object to quantize and dequantize
-            the output of the tree, and the ONNX model.
+        onnx.ModelProto: The ONNX model.
     """
-    # mypy
-    assert output_n_bits is not None
-
-    assert_true(
-        framework in ["xgboost", "sklearn"],
-        f"framework={framework} is not supported. It must be either 'xgboost' or 'sklearn'",
-    )
 
     # Silence hummingbird warnings
     warnings.filterwarnings("ignore")
 
     extra_config = {
         "tree_implementation": "gemm",
         "onnx_target_opset": OPSET_VERSION_FOR_ONNX_EXPORT,
@@ -81,120 +53,244 @@
 
     onnx_model = hb_convert(
         model,
         backend="onnx",
         test_input=x,
         extra_config=extra_config,
     ).model
+    return onnx_model
+
+
+def workaround_squeeze_node_xgboost(onnx_model: onnx.ModelProto):
+    """Workaround to fix torch issue that does not export the proper axis in the ONNX squeeze node.
+
+    FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/2778
+    The squeeze ops does not have the proper dimensions.
+    remove the following workaround when the issue is fixed
+    Add the axis attribute to the Squeeze node
+
+    Args:
+        onnx_model (onnx.ModelProto): The ONNX model.
+    """
+    target_node_id_list = [
+        i for i, node in enumerate(onnx_model.graph.node) if node.op_type == "Squeeze"
+    ]
+    assert_true(
+        len(target_node_id_list) == 1,
+        "Multiple Squeeze node found which is unexpected in tree-based models",
+    )
+    axes_input_name = "axes_squeeze"
+    axes_input = onnx.helper.make_tensor(axes_input_name, onnx.TensorProto.INT64, [1], (1,))
+
+    onnx_model.graph.initializer.append(axes_input)
+    onnx_model.graph.node[target_node_id_list[0]].input.insert(1, axes_input_name)
+
+
+def add_transpose_after_last_node(onnx_model: onnx.ModelProto):
+    """Add transpose after last node.
+
+    Args:
+        onnx_model (onnx.ModelProto): The ONNX model.
+    """
+    # Get the output node
+    output_node = onnx_model.graph.output[0]
+
+    # Create the node with perm attribute equal to (2, 1, 0)
+    transpose_node = onnx.helper.make_node(
+        "Transpose",
+        inputs=[output_node.name],
+        outputs=["transposed_output"],
+        perm=[2, 1, 0],
+    )
+
+    onnx_model.graph.node.append(transpose_node)
+    onnx_model.graph.output[0].name = "transposed_output"
+
+
+def preprocess_tree_predictions(
+    init_tensor: numpy.ndarray,
+    output_n_bits: int,
+) -> QuantizedArray:
+    """Apply post-processing from the graph.
+
+    Args:
+        init_tensor (numpy.ndarray): Model parameters to be pre-processed.
+        output_n_bits (int): The number of bits of the output.
+
+    Returns:
+        QuantizedArray: Quantizer for the tree predictions.
+    """
+
+    # Quantize probabilities and store QuantizedArray
+    # IMPORTANT: we must use symmetric signed quantization such that
+    # 0 in clear == 0 in quantized.
+
+    quant_args = {}
+
+    # If we have negative values, use a symmetric quantization
+    # in order to have a zero zero-point
+    if numpy.min(init_tensor) < 0:
+        is_signed = is_symmetric = True
+
+    # To ensure the zero-point is 0 we force the
+    # range of the quantizer to [0..max(init_tensor)]
+    else:
+        is_signed = is_symmetric = False
+        quant_args["rmax"] = numpy.max(init_tensor)
+        quant_args["rmin"] = 0
+        quant_args["uvalues"] = []
+
+    q_y = QuantizedArray(
+        n_bits=output_n_bits,
+        values=init_tensor,
+        is_signed=is_signed,
+        is_symmetric=is_symmetric,
+        **quant_args,
+    )
+    # Make sure the zero_point is 0 to prevent errors in Hummingbird's GEMM approach.
+    # Asymmetric quantization may cause the zero_point to be non-zero
+    # which leads to incorrect results.
+    assert_true(
+        q_y.quantizer.zero_point == 0,
+        "Zero point is not 0. Symmetric signed quantization must work.",
+    )
+    return q_y
 
-    # Make sure the onnx version returned by hummingbird is OPSET_VERSION_FOR_ONNX_EXPORT
+
+def tree_onnx_graph_preprocessing(
+    onnx_model: onnx.ModelProto, framework: str, expected_number_of_outputs: int
+):
+    """Apply pre-precessing onto the ONNX graph.
+
+    Args:
+        onnx_model (onnx.ModelProto): The ONNX model.
+        framework (str): The framework from which the ONNX model is generated.
+            (options: 'xgboost', 'sklearn')
+        expected_number_of_outputs (int): The expected number of outputs in the ONNX model.
+    """
+    # Make sure the ONNX version returned by hummingbird is OPSET_VERSION_FOR_ONNX_EXPORT
     onnx_version = get_onnx_opset_version(onnx_model)
     assert_true(
         onnx_version == OPSET_VERSION_FOR_ONNX_EXPORT,
-        f"The onnx version returned by Hummingbird is {onnx_version} "
+        f"The ONNX version returned by Hummingbird is {onnx_version} "
         f"instead of {OPSET_VERSION_FOR_ONNX_EXPORT}",
     )
 
-    # The tree returned by hummingbird has two outputs which is not supported currently by the
-    # compiler (as it only returns one output). Here we explicitly only keep the output named
-    # "variable", which after inspecting the hummingbird code is considered the canonical
-    # output. This was causing issues as the virtual lib (correctly) returned both outputs which
-    # the predict method did not expect as it was only getting one output from the compiler
-    # engine.
-    # The output we keep is the output giving the actual classes out, the other one is the
-    # one-hot encoded vectors to indicate which class is predicted.
-    # This is fine for now as we remove the argmax operator.
-
-    # Check we do have the correct number of output for the given task
-    expected_number_of_outputs = EXPECTED_NUMBER_OF_OUTPUTS_PER_TASK[task]
+    # Check we do have the correct number of ONNX output.
+    # Hummingbird returns two outputs for classification (predict and predict_proba)
+    # while a single output for regression (predict)
     assert_true(
         len(onnx_model.graph.output) == expected_number_of_outputs,
         on_error_msg=f"{len(onnx_model.graph.output)} != 2",
     )
 
-    # If the framework used is XGBoost, remove all the ONNX graph's nodes that follow the last
-    # MatMul operator
+    # Cut the graph at the ReduceSum node as large sum are not yet supported.
+    # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/451
+    clean_graph_at_node_op_type(onnx_model, "ReduceSum")
+
     if framework == "xgboost":
-        # Find Reshape node after last MatMul node
-        # (last MatMul node takes an input with "weight_3" in the name)
-        node_cut_id = ""
-        for node in onnx_model.graph.node:
-            if node_cut_id != "" and node.op_type == "Reshape" and node_cut_id in node.input:
-                node_name_to_cut = node.name
-                break
+        # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/2778
+        # The squeeze ops does not have the proper dimensions.
+        # remove the following workaround when the issue is fixed
+        # Add the axis attribute to the Squeeze node
+        workaround_squeeze_node_xgboost(onnx_model)
+    else:
+        # Add a transpose node after the last node.
+        # Sklearn models apply the reduce sum before the transpose.
+        # To have equivalent output between xgboost in sklearn,
+        # apply the transpose before returning the output.
+        add_transpose_after_last_node(onnx_model)
+
+    # Cast nodes are not necessary so remove them.
+    op_type_to_remove = ["Cast"]
+    remove_node_types(onnx_model, op_type_to_remove)
 
-            if len(node.input) > 0 and "weight_3" in node.input[0] and node.op_type == "MatMul":
-                node_cut_id = node.output[0]
 
-        clean_graph_after_node_name(onnx_model=onnx_model, node_name=node_name_to_cut)
+def tree_values_preprocessing(
+    onnx_model: onnx.ModelProto,
+    framework: str,
+    output_n_bits: int,
+) -> QuantizedArray:
+    """Pre-process tree values.
 
-    # Else, keep track of the last output
-    else:
-        keep_following_outputs_discard_others(onnx_model, ("variable",))
+    Args:
+        onnx_model (onnx.ModelProto): The ONNX model.
+        framework (str): The framework from which the ONNX model is generated.
+            (options: 'xgboost', 'sklearn')
+        output_n_bits (int): The number of bits of the output.
 
-    # TODO remove Transpose from the list when #931 is done
-    # TODO remove Gather from the list when #345 is done
-    op_type_to_remove = ["Transpose", "ArgMax", "ReduceSum", "Cast", "Gather"]
-    remove_node_types(onnx_model, op_type_to_remove)
+    Returns:
+        QuantizedArray: Quantizer for the tree predictions.
+    """
 
-    # Modify onnx graph to fit in FHE
+    # Modify ONNX graph to fit in FHE
     for i, initializer in enumerate(onnx_model.graph.initializer):
         # All constants in our tree should be integers.
         # Tree thresholds can be rounded up or down (depending on the tree implementation)
         # while the final probabilities/regression values must be quantized.
+        # We extract the value stored in each initializer node into the init_tensor.
         init_tensor = numpy_helper.to_array(initializer)
         if "weight_3" in initializer.name:
-            # This is the prediction tensor.
-            # Quantize probabilities and store QuantizedArray
-            # IMPORTANT: we must use symmetric signed quantization such that
-            # 0 in clear == 0 in quantized.
-
-            quant_args = {}
-            if numpy.min(init_tensor) < 0:
-                # If we have negative values, use a symmetric quantization
-                # in order to have a zero zero-point
-
-                is_signed = is_symmetric = True
-            else:
-                # To ensure the zero-point is 0 we force the
-                # range of the quantizer to [0..max(init_tensor)]
-
-                is_signed = is_symmetric = False
-                quant_args["rmax"] = numpy.max(init_tensor)
-                quant_args["rmin"] = 0
-                quant_args["uvalues"] = []
-
-            q_y = QuantizedArray(
-                n_bits=output_n_bits,
-                values=init_tensor,
-                is_signed=is_signed,
-                is_symmetric=is_symmetric,
-                **quant_args,
-            )
-            # Make sure the zero_point is 0.
-            # This is important for the final summation to work.
-            # The problem comes from the GEMM approach in Hummingbird where the default value of
-            # rows in the matrix that selects the correct output in each tree is set to True when
-            # the node does not exist in the tree. So the same value as a selected node.
-            # For Hummingbird, this is not a problem as the values for nodes that do not exist
-            # are set to 0.
-            # Here, if we use asymmetric quantization, there is a risk that the zero_point is
-            # not 0. The matmul will then select values != 0 and sum them.
-            # The resulting value will be different from the expected terminal node value.
-            assert_true(
-                q_y.quantizer.zero_point == 0,
-                "Zero point is not 0. Symmetric signed quantization must work.",
-            )
+            # weight_3 is the prediction tensor, apply the required pre-processing
+            q_y = preprocess_tree_predictions(init_tensor, output_n_bits)
+
+            # Get the preprocessed tree predictions to replace the current (non-quantized)
+            # values in the onnx_model.
             init_tensor = q_y.qvalues
         else:
             if framework == "xgboost":
                 # xgboost uses "<" operator thus we must round up.
                 init_tensor = numpy.ceil(init_tensor)
             elif framework == "sklearn":
                 # sklearn trees use ">" operator thus we must round down.
                 init_tensor = numpy.floor(init_tensor)
-        new_initializer = numpy_helper.from_array(init_tensor.astype(int), initializer.name)
+        new_initializer = numpy_helper.from_array(init_tensor.astype(numpy.int64), initializer.name)
         onnx_model.graph.initializer[i].CopyFrom(new_initializer)
+    return q_y
+
+
+# pylint: disable=too-many-locals
+def tree_to_numpy(
+    model: Callable,
+    x: numpy.ndarray,
+    framework: str,
+    output_n_bits: int = MAX_BITWIDTH_BACKWARD_COMPATIBLE,
+) -> Tuple[Callable, List[UniformQuantizer], onnx.ModelProto]:
+    """Convert the tree inference to a numpy functions using Hummingbird.
+
+    Args:
+        model (Callable): The tree model to convert.
+        x (numpy.ndarray): The input data.
+        framework (str): The framework from which the ONNX model is generated.
+            (options: 'xgboost', 'sklearn')
+        output_n_bits (int): The number of bits of the output. Default to 8.
+
+    Returns:
+        Tuple[Callable, List[QuantizedArray], onnx.ModelProto]: A tuple with a function that takes a
+            numpy array and returns a numpy array, QuantizedArray object to quantize and dequantize
+            the output of the tree, and the ONNX model.
+    """
+    # mypy
+    assert output_n_bits is not None
+
+    assert_true(
+        framework in ["xgboost", "sklearn"],
+        f"framework={framework} is not supported. It must be either 'xgboost' or 'sklearn'",
+    )
+
+    onnx_model = get_onnx_model(model, x, framework)
+
+    # Get the expected number of ONNX outputs in the sklearn model.
+    expected_number_of_outputs = 1 if is_regressor_or_partial_regressor(model) else 2
+
+    # ONNX graph pre-processing to make the model FHE friendly
+    # i.e. delete irrelevant nodes and cut the graph before the final ensemble sum)
+    tree_onnx_graph_preprocessing(onnx_model, framework, expected_number_of_outputs)
+
+    # Tree values pre-processing
+    # i.e. mainly predictions quantization
+    # but also rounding the threshold such that they are now integers
+    q_y = tree_values_preprocessing(onnx_model, framework, output_n_bits)
 
-    _tensor_tree_predict = get_equivalent_numpy_forward(onnx_model)
+    _tree_inference = get_equivalent_numpy_forward(onnx_model)
 
-    return (_tensor_tree_predict, [q_y.quantizer], onnx_model)
+    return (_tree_inference, [q_y.quantizer], onnx_model)
```

## concrete/ml/sklearn/xgb.py

```diff
@@ -1,40 +1,33 @@
 """Implements XGBoost models."""
 import platform
 import warnings
-from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy
 import xgboost.sklearn
 
-from concrete.ml.quantization.quantizers import UniformQuantizer
-
+from .. import TRUSTED_SKOPS, USE_SKOPS, loads_sklearn
 from ..common.debugging.custom_assert import assert_true
-
-# The sigmoid and softmax functions are already defined in the ONNX module and thus are imported
-# here in order to avoid duplicating them.
-from ..onnx.ops_impl import numpy_sigmoid, numpy_softmax
-from ..quantization import QuantizedArray
+from ..quantization.quantizers import UniformQuantizer
+from ..sklearn.tree_to_numpy import tree_to_numpy
 from .base import BaseTreeClassifierMixin, BaseTreeRegressorMixin
 
 
 # Disabling invalid-name to use uppercase X
 # pylint: disable=invalid-name,too-many-instance-attributes
 class XGBClassifier(BaseTreeClassifierMixin):
-    """Implements the XGBoost classifier."""
+    """Implements the XGBoost classifier.
 
-    sklearn_alg = xgboost.sklearn.XGBClassifier
-    q_x_byfeatures: List[QuantizedArray]
-    n_bits: int
-    output_quantizers: List[UniformQuantizer]
-    _tensor_tree_predict: Optional[Callable]
-    n_classes_: int
-    sklearn_model: Any
-    framework: str = "xgboost"
+    See https://xgboost.readthedocs.io/en/stable/python/python_api.html#module-xgboost.sklearn
+    for more information about the parameters used.
+    """
 
+    sklearn_model_class = xgboost.sklearn.XGBClassifier
+    framework = "xgboost"
     _is_a_public_cml_model = True
 
     # pylint: disable=too-many-arguments,too-many-locals
     def __init__(
         self,
         n_bits: int = 6,
         max_depth: Optional[int] = 3,
@@ -61,38 +54,38 @@
         interaction_constraints: Optional[Union[str, List[Tuple[str]]]] = None,
         importance_type: Optional[str] = None,
         gpu_id: Optional[int] = None,
         validate_parameters: Optional[bool] = None,
         predictor: Optional[str] = None,
         enable_categorical: bool = False,
         use_label_encoder: bool = False,
-        random_state: Optional[
-            Union[numpy.random.RandomState, int]  # pylint: disable=no-member
-        ] = None,
+        random_state: Optional[int] = None,
         verbosity: Optional[int] = None,
     ):
-        # See https://xgboost.readthedocs.io/en/stable/python/python_api.html#module-xgboost.sklearn
-        # for more information about the parameters used.
-
-        # base_score != 0.5 or None seems to not pass our tests (see #474)
+        # base_score != 0.5 or None does not seem to not pass our tests
+        # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/474
         assert_true(
             base_score in [0.5, None],
             f"Currently, only 0.5 or None are supported for base_score. Got {base_score}",
         )
 
-        # FIXME: see https://github.com/zama-ai/concrete-ml-internal/issues/503, there is currently
+        # See https://github.com/zama-ai/concrete-ml-internal/issues/503, there is currently
         # an issue with n_jobs != 1 on macOS
-        # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/506, remove this workaround
-        # once https://github.com/zama-ai/concrete-ml-internal/issues/503 is fixed
+        #
+        # When it gets fixed, we'll remove this workaround
+        # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/2747
         if platform.system() == "Darwin":
             if n_jobs != 1:  # pragma: no cover
-                warnings.warn("forcing n_jobs = 1 on mac for segfault issue")  # pragma: no cover
+                warnings.warn(
+                    "forcing n_jobs = 1 on mac for segfault issue", stacklevel=3
+                )  # pragma: no cover
                 n_jobs = 1  # pragma: no cover
 
-        BaseTreeClassifierMixin.__init__(self, n_bits=n_bits)
+        # Call BaseClassifier's __init__ method
+        super().__init__(n_bits=n_bits)
 
         self.max_depth = max_depth
         self.learning_rate = learning_rate
         self.n_estimators = n_estimators
         self.objective = objective
         self.booster = booster
         self.tree_method = tree_method
@@ -116,83 +109,146 @@
         self.gpu_id = gpu_id
         self.validate_parameters = validate_parameters
         self.predictor = predictor
         self.enable_categorical = enable_categorical
         self.use_label_encoder = use_label_encoder
         self.random_state = random_state
         self.verbosity = verbosity
-        self.post_processing_params: Dict[str, Any] = {}
-
-    def _update_post_processing_params(self):
-        """Update the post processing params."""
-        self.post_processing_params = {
-            "n_classes_": self.n_classes_,
-            "n_estimators": self.n_estimators,
-        }
-
-    def post_processing(self, y_preds: numpy.ndarray) -> numpy.ndarray:
-        """Apply post-processing to the predictions.
-
-        Args:
-            y_preds (numpy.ndarray): The predictions.
-
-        Returns:
-            numpy.ndarray: The post-processed predictions.
-        """
-        assert self.output_quantizers is not None
-
-        # Update post-processing params with their current values
-        self.__dict__.update(self.post_processing_params)
 
-        y_preds = self.output_quantizers[0].dequant(y_preds)
+    def dump_dict(self) -> Dict[str, Any]:
+        metadata: Dict[str, Any] = {}
 
-        # Apply transpose
-        y_preds = numpy.transpose(y_preds, axes=(2, 1, 0))
-
-        # XGBoost returns a shape (n_examples, n_classes, n_trees) when self.n_classes_ >= 3
-        # otherwise it returns a shape (n_examples, 1, n_trees)
-
-        # Reshape to (-1, n_classes, n_trees)
-        # No need to reshape if n_classes = 2
-        if self.n_classes_ > 2:
-            y_preds = y_preds.reshape((-1, self.n_classes_, self.n_estimators))  # type: ignore
-
-        # Sum all tree outputs.
-        y_preds = numpy.sum(y_preds, axis=2)
-        assert_true(y_preds.ndim == 2, "y_preds should be a 2D array")
-
-        # If this binary classification problem
-        if self.n_classes_ == 2:
-            # Apply sigmoid
-            y_preds = numpy_sigmoid(y_preds)[0]
+        metadata["cml_dumped_class_name"] = str(type(self).__name__)
+        metadata["n_bits"] = self.n_bits
+        metadata["input_quantizers"] = [elt.dumps() for elt in self.input_quantizers]
+        metadata["output_quantizers"] = [elt.dumps() for elt in self.output_quantizers]
+        metadata["sklearn_model_class"] = self.sklearn_model_class
+        metadata["sklearn_model"] = self.sklearn_model
+        metadata["onnx_model_"] = self.onnx_model_
+        metadata["_is_fitted"] = self._is_fitted
+        metadata["_is_compiled"] = self._is_compiled
+        metadata["framework"] = self.framework
+
+        # Classifier
+        metadata["classes_"] = self.target_classes_
+        metadata["n_classes_"] = self.n_classes_
+
+        metadata["max_depth"] = self.max_depth
+        metadata["learning_rate"] = self.learning_rate
+        metadata["n_estimators"] = self.n_estimators
+        metadata["objective"] = self.objective
+        metadata["booster"] = self.booster
+        metadata["tree_method"] = self.tree_method
+        metadata["n_jobs"] = self.n_jobs
+        metadata["gamma"] = self.gamma
+        metadata["min_child_weight"] = self.min_child_weight
+        metadata["max_delta_step"] = self.max_delta_step
+        metadata["subsample"] = self.subsample
+        metadata["colsample_bytree"] = self.colsample_bytree
+        metadata["colsample_bylevel"] = self.colsample_bylevel
+        metadata["colsample_bynode"] = self.colsample_bynode
+        metadata["reg_alpha"] = self.reg_alpha
+        metadata["reg_lambda"] = self.reg_lambda
+        metadata["scale_pos_weight"] = self.scale_pos_weight
+        metadata["base_score"] = self.base_score
+        metadata["missing"] = self.missing
+        metadata["num_parallel_tree"] = self.num_parallel_tree
+        metadata["monotone_constraints"] = self.monotone_constraints
+        metadata["interaction_constraints"] = self.interaction_constraints
+        metadata["importance_type"] = self.importance_type
+        metadata["gpu_id"] = self.gpu_id
+        metadata["validate_parameters"] = self.validate_parameters
+        metadata["predictor"] = self.predictor
+        metadata["enable_categorical"] = self.enable_categorical
+        metadata["use_label_encoder"] = self.use_label_encoder
+        metadata["random_state"] = self.random_state
+        metadata["verbosity"] = self.verbosity
+        metadata["post_processing_params"] = self.post_processing_params
+
+        return metadata
+
+    @classmethod
+    def load_dict(cls, metadata: Dict):
+        obj = XGBClassifier(n_bits=metadata["n_bits"])
+
+        # Tree
+        obj.input_quantizers = [UniformQuantizer.loads(elt) for elt in metadata["input_quantizers"]]
+        obj.output_quantizers = [
+            UniformQuantizer.loads(elt) for elt in metadata["output_quantizers"]
+        ]
+
+        # Load the underlying fitted model
+        loads_sklearn_kwargs = {}
+        if USE_SKOPS:
+            loads_sklearn_kwargs["trusted"] = TRUSTED_SKOPS
+        obj.sklearn_model = loads_sklearn(
+            bytes.fromhex(metadata["sklearn_model"]), **loads_sklearn_kwargs
+        )
 
-            # Transform in a 2d array where [1-p, p] is the output as XGBoost only outputs 1 value
-            # when considering 2 classes
-            y_preds = numpy.concatenate((1 - y_preds, y_preds), axis=1)
+        obj.framework = metadata["framework"]
+        obj._is_fitted = metadata["_is_fitted"]
+        obj._is_compiled = metadata["_is_compiled"]
+
+        obj._tree_inference, obj.output_quantizers, obj.onnx_model_ = tree_to_numpy(
+            obj.sklearn_model,
+            numpy.zeros((len(obj.input_quantizers),))[None, ...],
+            framework=obj.framework,
+            output_n_bits=obj.n_bits,
+        )
 
-        # Else, it's a multi-class classification problem
-        else:
-            # Apply softmax
-            y_preds = numpy_softmax(y_preds)[0]
+        # Classifier
+        obj.target_classes_ = numpy.array(metadata["classes_"])
+        obj.n_classes_ = metadata["n_classes_"]
+
+        obj.max_depth = metadata["max_depth"]
+        obj.learning_rate = metadata["learning_rate"]
+        obj.n_estimators = metadata["n_estimators"]
+        obj.objective = metadata["objective"]
+        obj.booster = metadata["booster"]
+        obj.tree_method = metadata["tree_method"]
+        obj.n_jobs = metadata["n_jobs"]
+        obj.gamma = metadata["gamma"]
+        obj.min_child_weight = metadata["min_child_weight"]
+        obj.max_delta_step = metadata["max_delta_step"]
+        obj.subsample = metadata["subsample"]
+        obj.colsample_bytree = metadata["colsample_bytree"]
+        obj.colsample_bylevel = metadata["colsample_bylevel"]
+        obj.colsample_bynode = metadata["colsample_bynode"]
+        obj.reg_alpha = metadata["reg_alpha"]
+        obj.reg_lambda = metadata["reg_lambda"]
+        obj.scale_pos_weight = metadata["scale_pos_weight"]
+        obj.base_score = metadata["base_score"]
+        obj.missing = metadata["missing"]
+        obj.num_parallel_tree = metadata["num_parallel_tree"]
+        obj.monotone_constraints = metadata["monotone_constraints"]
+        obj.interaction_constraints = metadata["interaction_constraints"]
+        obj.importance_type = metadata["importance_type"]
+        obj.gpu_id = metadata["gpu_id"]
+        obj.validate_parameters = metadata["validate_parameters"]
+        obj.predictor = metadata["predictor"]
+        obj.enable_categorical = metadata["enable_categorical"]
+        obj.use_label_encoder = metadata["use_label_encoder"]
+        obj.random_state = metadata["random_state"]
+        obj.verbosity = metadata["verbosity"]
+        obj.post_processing_params = metadata["post_processing_params"]
 
-        return y_preds
+        return obj
 
 
 # Disabling invalid-name to use uppercase X
 # pylint: disable=invalid-name,too-many-instance-attributes
 class XGBRegressor(BaseTreeRegressorMixin):
-    """Implements the XGBoost regressor."""
+    """Implements the XGBoost regressor.
+
+    See https://xgboost.readthedocs.io/en/stable/python/python_api.html#module-xgboost.sklearn
+    for more information about the parameters used.
+    """
 
-    sklearn_alg = xgboost.sklearn.XGBRegressor
-    q_x_byfeatures: List[QuantizedArray]
-    n_bits: int
-    output_quantizers: List[UniformQuantizer]
-    _tensor_tree_predict: Optional[Callable]
-    sklearn_model: Any
-    framework: str = "xgboost"
+    sklearn_model_class = xgboost.sklearn.XGBRegressor
+    framework = "xgboost"
     _is_a_public_cml_model = True
 
     # pylint: disable=too-many-arguments,too-many-locals
     def __init__(
         self,
         n_bits: int = 6,
         max_depth: Optional[int] = 3,
@@ -219,38 +275,38 @@
         interaction_constraints: Optional[Union[str, List[Tuple[str]]]] = None,
         importance_type: Optional[str] = None,
         gpu_id: Optional[int] = None,
         validate_parameters: Optional[bool] = None,
         predictor: Optional[str] = None,
         enable_categorical: bool = False,
         use_label_encoder: bool = False,
-        random_state: Optional[
-            Union[numpy.random.RandomState, int]  # pylint: disable=no-member
-        ] = None,
+        random_state: Optional[int] = None,
         verbosity: Optional[int] = None,
     ):
-        # See https://xgboost.readthedocs.io/en/stable/python/python_api.html#module-xgboost.sklearn
-        # for more information about the parameters used.
-
-        # base_score != 0.5 or None seems to not pass our tests (see #474)
+        # base_score != 0.5 or None does not seem to not pass our tests
+        # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/474
         assert_true(
             base_score in [0.5, None],
             f"Currently, only 0.5 or None are supported for base_score. Got {base_score}",
         )
 
-        # FIXME: see https://github.com/zama-ai/concrete-ml-internal/issues/503, there is currently
+        # See https://github.com/zama-ai/concrete-ml-internal/issues/503, there is currently
         # an issue with n_jobs != 1 on macOS
-        # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/506, remove this workaround
-        # once https://github.com/zama-ai/concrete-ml-internal/issues/503 is fixed
+        #
+        # When it gets fixed, we'll remove this workaround
+        # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/2747
         if platform.system() == "Darwin":
             if n_jobs != 1:  # pragma: no cover
-                warnings.warn("forcing n_jobs = 1 on mac for segfault issue")  # pragma: no cover
+                warnings.warn(
+                    "forcing n_jobs = 1 on mac for segfault issue", stacklevel=3
+                )  # pragma: no cover
                 n_jobs = 1  # pragma: no cover
 
-        BaseTreeRegressorMixin.__init__(self, n_bits=n_bits)
+        # Call BaseTreeEstimatorMixin's __init__ method
+        super().__init__(n_bits=n_bits)
 
         self.max_depth = max_depth
         self.learning_rate = learning_rate
         self.n_estimators = n_estimators
         self.objective = objective
         self.booster = booster
         self.tree_method = tree_method
@@ -274,67 +330,134 @@
         self.gpu_id = gpu_id
         self.validate_parameters = validate_parameters
         self.predictor = predictor
         self.enable_categorical = enable_categorical
         self.use_label_encoder = use_label_encoder
         self.random_state = random_state
         self.verbosity = verbosity
-        self.post_processing_params: Dict[str, Any] = {}
-
-    def _update_post_processing_params(self):
-        """Update the post processing params."""
-        self.post_processing_params = {
-            "n_estimators": self.n_estimators,
-        }
-
-    def post_processing(self, y_preds: numpy.ndarray) -> numpy.ndarray:
-        """Apply post-processing to the predictions.
-
-        Args:
-            y_preds (numpy.ndarray): The predictions.
-
-        Returns:
-            numpy.ndarray: The post-processed predictions.
-        """
-        assert self.output_quantizers is not None
-
-        # Update post-processing params with their current values
-        self.__dict__.update(self.post_processing_params)
-
-        y_preds = self.output_quantizers[0].dequant(y_preds)
-
-        # Apply transpose
-        y_preds = numpy.transpose(y_preds, axes=(2, 1, 0))
 
-        # XGBoost returns a shape (n_examples, n_classes, n_trees) when self.n_classes_ >= 3
-        # otherwise it returns a shape (n_examples, 1, n_trees)
+    def fit(self, X, y, *args, **kwargs) -> Any:
 
-        # Sum all tree outputs.
-        y_preds = numpy.sum(y_preds, axis=2)
-        assert_true(y_preds.ndim == 2, "y_preds should be a 2D array")
+        # HummingBird and XGBoost don't properly manage multi-outputs cases
+        # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/1856
 
-        return y_preds
+        assert_true(
+            (isinstance(y, list) and (not isinstance(y[0], list) or (len(y[0]) == 1)))
+            or (not isinstance(y, list) and (len(y.shape) == 1 or y.shape[1] == 1)),
+            "XGBRegressor doesn't support multi-output cases.",
+        )
 
-    def fit(self, X, y, **kwargs) -> Any:
-        """Fit the tree-based estimator.
+        # Call BaseTreeEstimatorMixin's fit method
+        super().fit(X, y, *args, **kwargs)
+        return self
 
-        Args:
-            X : training data
-                By default, you should be able to pass:
-                * numpy arrays
-                * torch tensors
-                * pandas DataFrame or Series
-            y (numpy.ndarray): The target data.
-            **kwargs: args for super().fit
+    def dump_dict(self) -> Dict[str, Any]:
+        metadata: Dict[str, Any] = {}
 
-        Returns:
-            Any: The fitted model.
-        """
+        metadata["cml_dumped_class_name"] = str(type(self).__name__)
+        metadata["n_bits"] = self.n_bits
+        metadata["input_quantizers"] = [elt.dumps() for elt in self.input_quantizers]
+        metadata["output_quantizers"] = [elt.dumps() for elt in self.output_quantizers]
+        metadata["sklearn_model_class"] = self.sklearn_model_class
+        metadata["sklearn_model"] = self.sklearn_model
+        metadata["onnx_model_"] = self.onnx_model_
+        metadata["_is_fitted"] = self._is_fitted
+        metadata["_is_compiled"] = self._is_compiled
+        metadata["framework"] = self.framework
+
+        # Specific
+        metadata["max_depth"] = self.max_depth
+        metadata["learning_rate"] = self.learning_rate
+        metadata["n_estimators"] = self.n_estimators
+        metadata["objective"] = self.objective
+        metadata["booster"] = self.booster
+        metadata["tree_method"] = self.tree_method
+        metadata["n_jobs"] = self.n_jobs
+        metadata["gamma"] = self.gamma
+        metadata["min_child_weight"] = self.min_child_weight
+        metadata["max_delta_step"] = self.max_delta_step
+        metadata["subsample"] = self.subsample
+        metadata["colsample_bytree"] = self.colsample_bytree
+        metadata["colsample_bylevel"] = self.colsample_bylevel
+        metadata["colsample_bynode"] = self.colsample_bynode
+        metadata["reg_alpha"] = self.reg_alpha
+        metadata["reg_lambda"] = self.reg_lambda
+        metadata["scale_pos_weight"] = self.scale_pos_weight
+        metadata["base_score"] = self.base_score
+        metadata["missing"] = self.missing
+        metadata["num_parallel_tree"] = self.num_parallel_tree
+        metadata["monotone_constraints"] = self.monotone_constraints
+        metadata["interaction_constraints"] = self.interaction_constraints
+        metadata["importance_type"] = self.importance_type
+        metadata["gpu_id"] = self.gpu_id
+        metadata["validate_parameters"] = self.validate_parameters
+        metadata["predictor"] = self.predictor
+        metadata["enable_categorical"] = self.enable_categorical
+        metadata["use_label_encoder"] = self.use_label_encoder
+        metadata["random_state"] = self.random_state
+        metadata["verbosity"] = self.verbosity
+        metadata["post_processing_params"] = self.post_processing_params
+
+        return metadata
+
+    @classmethod
+    def load_dict(cls, metadata: Dict):
+        obj = XGBRegressor(n_bits=metadata["n_bits"])
+
+        # Tree
+        obj.input_quantizers = [UniformQuantizer.loads(elt) for elt in metadata["input_quantizers"]]
+        obj.output_quantizers = [
+            UniformQuantizer.loads(elt) for elt in metadata["output_quantizers"]
+        ]
+
+        # Load the underlying fitted model
+        loads_sklearn_kwargs = {}
+        if USE_SKOPS:
+            loads_sklearn_kwargs["trusted"] = TRUSTED_SKOPS
+        obj.sklearn_model = loads_sklearn(
+            bytes.fromhex(metadata["sklearn_model"]), **loads_sklearn_kwargs
+        )
 
-        # HummingBird doesn't manage correctly n_targets > 1
-        assert_true(
-            len(y.shape) == 1 or y.shape[1] == 1, "n_targets = 1 is the only supported case"
+        obj.framework = metadata["framework"]
+        obj._is_fitted = metadata["_is_fitted"]
+        obj._is_compiled = metadata["_is_compiled"]
+
+        obj._tree_inference, obj.output_quantizers, obj.onnx_model_ = tree_to_numpy(
+            obj.sklearn_model,
+            numpy.zeros((len(obj.input_quantizers),))[None, ...],
+            framework=obj.framework,
+            output_n_bits=obj.n_bits,
         )
 
-        # Call super's fit that will train the network
-        super().fit(X, y, **kwargs)
-        return self
+        obj.max_depth = metadata["max_depth"]
+        obj.learning_rate = metadata["learning_rate"]
+        obj.n_estimators = metadata["n_estimators"]
+        obj.objective = metadata["objective"]
+        obj.booster = metadata["booster"]
+        obj.tree_method = metadata["tree_method"]
+        obj.n_jobs = metadata["n_jobs"]
+        obj.gamma = metadata["gamma"]
+        obj.min_child_weight = metadata["min_child_weight"]
+        obj.max_delta_step = metadata["max_delta_step"]
+        obj.subsample = metadata["subsample"]
+        obj.colsample_bytree = metadata["colsample_bytree"]
+        obj.colsample_bylevel = metadata["colsample_bylevel"]
+        obj.colsample_bynode = metadata["colsample_bynode"]
+        obj.reg_alpha = metadata["reg_alpha"]
+        obj.reg_lambda = metadata["reg_lambda"]
+        obj.scale_pos_weight = metadata["scale_pos_weight"]
+        obj.base_score = metadata["base_score"]
+        obj.missing = metadata["missing"]
+        obj.num_parallel_tree = metadata["num_parallel_tree"]
+        obj.monotone_constraints = metadata["monotone_constraints"]
+        obj.interaction_constraints = metadata["interaction_constraints"]
+        obj.importance_type = metadata["importance_type"]
+        obj.gpu_id = metadata["gpu_id"]
+        obj.validate_parameters = metadata["validate_parameters"]
+        obj.predictor = metadata["predictor"]
+        obj.enable_categorical = metadata["enable_categorical"]
+        obj.use_label_encoder = metadata["use_label_encoder"]
+        obj.random_state = metadata["random_state"]
+        obj.verbosity = metadata["verbosity"]
+        obj.post_processing_params = metadata["post_processing_params"]
+
+        return obj
```

## concrete/ml/torch/compile.py

```diff
@@ -4,23 +4,26 @@
 from pathlib import Path
 from typing import Optional, Tuple, Union
 
 import numpy
 import onnx
 import torch
 from brevitas.export.onnx.qonnx.manager import QONNXManager as BrevitasONNXManager
-from concrete.numpy.compilation.artifacts import DebugArtifacts
-from concrete.numpy.compilation.configuration import Configuration
+from brevitas.nn.quant_layer import QuantInputOutputLayer as QNNMixingLayer
+from brevitas.nn.quant_layer import QuantNonLinearActLayer as QNNUnivariateLayer
+from concrete.fhe.compilation.artifacts import DebugArtifacts
+from concrete.fhe.compilation.configuration import Configuration
 
-from ..common.debugging import assert_true
+from ..common.debugging import assert_false, assert_true
 from ..common.utils import (
     MAX_BITWIDTH_BACKWARD_COMPATIBLE,
     check_there_is_no_p_error_options_in_configuration,
     get_onnx_opset_version,
     manage_parameters_for_pbs_errors,
+    to_tuple,
 )
 from ..onnx.convert import OPSET_VERSION_FOR_ONNX_EXPORT
 from ..onnx.onnx_utils import remove_initializer_from_input
 from ..quantization import PostTrainingAffineQuantization, PostTrainingQATImporter, QuantizedModule
 from . import NumpyModule
 
 Tensor = Union[torch.Tensor, numpy.ndarray]
@@ -48,200 +51,207 @@
 
 # pylint: disable-next=too-many-arguments
 def _compile_torch_or_onnx_model(
     model: Union[torch.nn.Module, onnx.ModelProto],
     torch_inputset: Dataset,
     import_qat: bool = False,
     configuration: Optional[Configuration] = None,
-    compilation_artifacts: Optional[DebugArtifacts] = None,
+    artifacts: Optional[DebugArtifacts] = None,
     show_mlir: bool = False,
     n_bits=MAX_BITWIDTH_BACKWARD_COMPATIBLE,
-    use_virtual_lib: bool = False,
+    rounding_threshold_bits: Optional[int] = None,
     p_error: Optional[float] = None,
     global_p_error: Optional[float] = None,
-    verbose_compilation: bool = False,
+    verbose: bool = False,
 ) -> QuantizedModule:
     """Compile a torch module or ONNX into a FHE equivalent.
 
     Take a model in torch or ONNX, turn it to numpy, quantize its inputs / weights / outputs and
-    finally compile it with Concrete-Numpy
+    finally compile it with Concrete
 
     Args:
         model (Union[torch.nn.Module, onnx.ModelProto]): the model to quantize, either in torch or
             in ONNX
         torch_inputset (Dataset): the calibration inputset, can contain either torch
-            tensors or numpy.ndarray.
+            tensors or numpy.ndarray
         import_qat (bool): Flag to signal that the network being imported contains quantizers in
-            in its computation graph and that Concrete ML should not requantize it.
-        configuration (Configuration): Configuration object to use
-            during compilation
-        compilation_artifacts (DebugArtifacts): Artifacts object to fill
-            during compilation
+            in its computation graph and that Concrete ML should not requantize it
+        configuration (Configuration): Configuration object to use during compilation
+        artifacts (DebugArtifacts): Artifacts object to fill during compilation
         show_mlir (bool): if set, the MLIR produced by the converter and which is going
-            to be sent to the compiler backend is shown on the screen, e.g., for debugging or demo
+            to be sent to the compiler backend is shown on the screen, e.g. for debugging or demo
         n_bits: the number of bits for the quantization
-        use_virtual_lib (bool): set to use the so called virtual lib simulating FHE computation.
-            Defaults to False
+        rounding_threshold_bits (int): if not None, every accumulators in the model are rounded down
+            to the given bits of precision
         p_error (Optional[float]): probability of error of a single PBS
-        global_p_error (Optional[float]): probability of error of the full circuit. Not simulated
-            by the VL, i.e., taken as 0
-        verbose_compilation (bool): whether to show compilation information
+        global_p_error (Optional[float]): probability of error of the full circuit. In FHE
+            simulation `global_p_error` is set to 0
+        verbose (bool): whether to show compilation information
 
     Returns:
         QuantizedModule: The resulting compiled QuantizedModule.
     """
 
-    inputset_as_numpy_tuple = (
-        tuple(convert_torch_tensor_or_numpy_array_to_numpy_array(val) for val in torch_inputset)
-        if isinstance(torch_inputset, tuple)
-        else (convert_torch_tensor_or_numpy_array_to_numpy_array(torch_inputset),)
+    inputset_as_numpy_tuple = tuple(
+        convert_torch_tensor_or_numpy_array_to_numpy_array(val) for val in to_tuple(torch_inputset)
     )
 
     # Tracing needs to be done with the batch size of 1 since we compile our models to FHE with
     # this batch size. The input set contains many examples, to determine a representative bitwidth,
     # but for tracing we only take a single one. We need the ONNX tracing batch size to match
     # the batch size during FHE inference which can only be 1 for the moment.
-    # FIXME: if it's possible to use batch size > 1 in FHE, update this function
-    # see https://github.com/zama-ai/concrete-ml-internal/issues/758
+    # Use batch size > 1 in FHE once it is available
+    # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/758
     dummy_input_for_tracing = tuple(
         torch.from_numpy(val[[0], ::]).float() for val in inputset_as_numpy_tuple
     )
 
     # Create corresponding numpy model
     numpy_model = NumpyModule(model, dummy_input_for_tracing)
     onnx_model = numpy_model.onnx_model
 
     # Quantize with post-training static method, to have a model with integer weights
-    post_training_quant: Union[PostTrainingAffineQuantization, PostTrainingQATImporter]
-    if import_qat:
-        post_training_quant = PostTrainingQATImporter(n_bits, numpy_model, is_signed=True)
-    else:
-        post_training_quant = PostTrainingAffineQuantization(n_bits, numpy_model, is_signed=True)
-    quantized_module = post_training_quant.quantize_module(*inputset_as_numpy_tuple)
+    post_training = PostTrainingQATImporter if import_qat else PostTrainingAffineQuantization
+    post_training_quant = post_training(n_bits, numpy_model, rounding_threshold_bits)
 
-    quantized_numpy_inputset = quantized_module.quantize_input(*inputset_as_numpy_tuple)
+    quantized_module = post_training_quant.quantize_module(*inputset_as_numpy_tuple)
 
     # Don't let the user shoot in her foot, by having p_error or global_p_error set in both
     # configuration and in direct arguments
     check_there_is_no_p_error_options_in_configuration(configuration)
 
     # Find the right way to set parameters for compiler, depending on the way we want to default
     p_error, global_p_error = manage_parameters_for_pbs_errors(p_error, global_p_error)
 
     quantized_module.compile(
-        quantized_numpy_inputset,
+        inputset_as_numpy_tuple,
         configuration,
-        compilation_artifacts,
+        artifacts,
         show_mlir=show_mlir,
-        use_virtual_lib=use_virtual_lib,
         p_error=p_error,
         global_p_error=global_p_error,
-        verbose_compilation=verbose_compilation,
+        verbose=verbose,
     )
 
     quantized_module.onnx_model = onnx_model
 
     return quantized_module
 
 
 # pylint: disable-next=too-many-arguments
 def compile_torch_model(
     torch_model: torch.nn.Module,
     torch_inputset: Dataset,
     import_qat: bool = False,
     configuration: Optional[Configuration] = None,
-    compilation_artifacts: Optional[DebugArtifacts] = None,
+    artifacts: Optional[DebugArtifacts] = None,
     show_mlir: bool = False,
     n_bits=MAX_BITWIDTH_BACKWARD_COMPATIBLE,
-    use_virtual_lib: bool = False,
+    rounding_threshold_bits: Optional[int] = None,
     p_error: Optional[float] = None,
     global_p_error: Optional[float] = None,
-    verbose_compilation: bool = False,
+    verbose: bool = False,
 ) -> QuantizedModule:
     """Compile a torch module into a FHE equivalent.
 
     Take a model in torch, turn it to numpy, quantize its inputs / weights / outputs and finally
-    compile it with Concrete-Numpy
+    compile it with Concrete
 
     Args:
         torch_model (torch.nn.Module): the model to quantize
         torch_inputset (Dataset): the calibration inputset, can contain either torch
             tensors or numpy.ndarray.
         import_qat (bool): Set to True to import a network that contains quantizers and was
             trained using quantization aware training
         configuration (Configuration): Configuration object to use
             during compilation
-        compilation_artifacts (DebugArtifacts): Artifacts object to fill
+        artifacts (DebugArtifacts): Artifacts object to fill
             during compilation
         show_mlir (bool): if set, the MLIR produced by the converter and which is going
             to be sent to the compiler backend is shown on the screen, e.g., for debugging or demo
         n_bits: the number of bits for the quantization
-        use_virtual_lib (bool): set to use the so called virtual lib simulating FHE computation.
-            Defaults to False
+        rounding_threshold_bits (int): if not None, every accumulators in the model are rounded down
+            to the given bits of precision
         p_error (Optional[float]): probability of error of a single PBS
-        global_p_error (Optional[float]): probability of error of the full circuit. Not simulated
-            by the VL, i.e., taken as 0
-        verbose_compilation (bool): whether to show compilation information
+        global_p_error (Optional[float]): probability of error of the full circuit. In FHE
+            simulation `global_p_error` is set to 0
+        verbose (bool): whether to show compilation information
 
     Returns:
         QuantizedModule: The resulting compiled QuantizedModule.
     """
+    assert_true(
+        isinstance(torch_model, torch.nn.Module),
+        "The compile_torch_model function must be called on a torch.nn.Module",
+    )
+
+    has_any_qnn_layers = any(
+        isinstance(layer, (QNNMixingLayer, QNNUnivariateLayer)) for layer in torch_model.modules()
+    )
+
+    assert_false(
+        has_any_qnn_layers,
+        "The compile_torch_model was called on a torch.nn.Module that contains "
+        "Brevitas quantized layers. These models must be imported "
+        "using compile_brevitas_qat_model instead.",
+    )
+
     return _compile_torch_or_onnx_model(
         torch_model,
         torch_inputset,
         import_qat,
         configuration=configuration,
-        compilation_artifacts=compilation_artifacts,
+        artifacts=artifacts,
         show_mlir=show_mlir,
         n_bits=n_bits,
-        use_virtual_lib=use_virtual_lib,
+        rounding_threshold_bits=rounding_threshold_bits,
         p_error=p_error,
         global_p_error=global_p_error,
-        verbose_compilation=verbose_compilation,
+        verbose=verbose,
     )
 
 
 # pylint: disable-next=too-many-arguments
 def compile_onnx_model(
     onnx_model: onnx.ModelProto,
     torch_inputset: Dataset,
     import_qat: bool = False,
     configuration: Optional[Configuration] = None,
-    compilation_artifacts: Optional[DebugArtifacts] = None,
+    artifacts: Optional[DebugArtifacts] = None,
     show_mlir: bool = False,
     n_bits=MAX_BITWIDTH_BACKWARD_COMPATIBLE,
-    use_virtual_lib: bool = False,
+    rounding_threshold_bits: Optional[int] = None,
     p_error: Optional[float] = None,
     global_p_error: Optional[float] = None,
-    verbose_compilation: bool = False,
+    verbose: bool = False,
 ) -> QuantizedModule:
     """Compile a torch module into a FHE equivalent.
 
     Take a model in torch, turn it to numpy, quantize its inputs / weights / outputs and finally
-    compile it with Concrete-Numpy
+    compile it with Concrete-Python
 
     Args:
         onnx_model (onnx.ModelProto): the model to quantize
         torch_inputset (Dataset): the calibration inputset, can contain either torch
             tensors or numpy.ndarray.
         import_qat (bool): Flag to signal that the network being imported contains quantizers in
             in its computation graph and that Concrete ML should not requantize it.
         configuration (Configuration): Configuration object to use
             during compilation
-        compilation_artifacts (DebugArtifacts): Artifacts object to fill
+        artifacts (DebugArtifacts): Artifacts object to fill
             during compilation
         show_mlir (bool): if set, the MLIR produced by the converter and which is going
             to be sent to the compiler backend is shown on the screen, e.g., for debugging or demo
         n_bits: the number of bits for the quantization
-        use_virtual_lib (bool): set to use the so called virtual lib simulating FHE computation.
-            Defaults to False.
+        rounding_threshold_bits (int): if not None, every accumulators in the model are rounded down
+            to the given bits of precision
         p_error (Optional[float]): probability of error of a single PBS
-        global_p_error (Optional[float]): probability of error of the full circuit. Not simulated
-            by the VL, i.e., taken as 0
-        verbose_compilation (bool): whether to show compilation information
+        global_p_error (Optional[float]): probability of error of the full circuit. In FHE
+            simulation `global_p_error` is set to 0
+        verbose (bool): whether to show compilation information
 
     Returns:
         QuantizedModule: The resulting compiled QuantizedModule.
     """
 
     onnx_model_opset_version = get_onnx_opset_version(onnx_model)
     assert_true(
@@ -251,84 +261,103 @@
     )
 
     return _compile_torch_or_onnx_model(
         onnx_model,
         torch_inputset,
         import_qat,
         configuration=configuration,
-        compilation_artifacts=compilation_artifacts,
+        artifacts=artifacts,
         show_mlir=show_mlir,
         n_bits=n_bits,
-        use_virtual_lib=use_virtual_lib,
+        rounding_threshold_bits=rounding_threshold_bits,
         p_error=p_error,
         global_p_error=global_p_error,
-        verbose_compilation=verbose_compilation,
+        verbose=verbose,
     )
 
 
 # pylint: disable-next=too-many-arguments
 def compile_brevitas_qat_model(
     torch_model: torch.nn.Module,
     torch_inputset: Dataset,
-    n_bits: Union[int, dict],
+    n_bits: Optional[Union[int, dict]] = None,
     configuration: Optional[Configuration] = None,
-    compilation_artifacts: Optional[DebugArtifacts] = None,
+    artifacts: Optional[DebugArtifacts] = None,
     show_mlir: bool = False,
-    use_virtual_lib: bool = False,
+    rounding_threshold_bits: Optional[int] = None,
     p_error: Optional[float] = None,
     global_p_error: Optional[float] = None,
     output_onnx_file: Union[Path, str] = None,
-    verbose_compilation: bool = False,
+    verbose: bool = False,
 ) -> QuantizedModule:
     """Compile a Brevitas Quantization Aware Training model.
 
     The torch_model parameter is a subclass of torch.nn.Module that uses quantized
     operations from brevitas.qnn. The model is trained before calling this function. This
     function compiles the trained model to FHE.
 
     Args:
         torch_model (torch.nn.Module): the model to quantize
         torch_inputset (Dataset): the calibration inputset, can contain either torch
             tensors or numpy.ndarray.
-        n_bits (Union[int,dict]): the number of bits for the quantization
+        n_bits (Optional[Union[int, dict]): the number of bits for the quantization. By default,
+            for most models, a value of None should be given, which instructs Concrete ML to use the
+            bit-widths configured using Brevitas quantization options. For some networks, that
+            perform a non-linear operation on an input on an output, if None is given, a default
+            value of 8 bits is used for the input/output quantization. For such models the user can
+            also specify a dictionary with model_inputs/model_outputs keys to override
+            the 8-bit default or a single integer for both values.
         configuration (Configuration): Configuration object to use
             during compilation
-        compilation_artifacts (DebugArtifacts): Artifacts object to fill
+        artifacts (DebugArtifacts): Artifacts object to fill
             during compilation
         show_mlir (bool): if set, the MLIR produced by the converter and which is going
             to be sent to the compiler backend is shown on the screen, e.g., for debugging or demo
-        use_virtual_lib (bool): set to use the so called virtual lib simulating FHE computation,
-            defaults to False.
+        rounding_threshold_bits (int): if not None, every accumulators in the model are rounded down
+            to the given bits of precision
         p_error (Optional[float]): probability of error of a single PBS
-        global_p_error (Optional[float]): probability of error of the full circuit. Not simulated
-            by the VL, i.e., taken as 0
+        global_p_error (Optional[float]): probability of error of the full circuit. In FHE
+            simulation `global_p_error` is set to 0
         output_onnx_file (str): temporary file to store ONNX model. If None a temporary file
             is generated
-        verbose_compilation (bool): whether to show compilation information
+        verbose (bool): whether to show compilation information
 
     Returns:
         QuantizedModule: The resulting compiled QuantizedModule.
     """
 
-    inputset_as_numpy_tuple = (
-        tuple(convert_torch_tensor_or_numpy_array_to_numpy_array(val) for val in torch_inputset)
-        if isinstance(torch_inputset, tuple)
-        else (convert_torch_tensor_or_numpy_array_to_numpy_array(torch_inputset),)
+    inputset_as_numpy_tuple = tuple(
+        convert_torch_tensor_or_numpy_array_to_numpy_array(val) for val in to_tuple(torch_inputset)
     )
 
     dummy_input_for_tracing = tuple(
         torch.from_numpy(val[[0], ::]).float() for val in inputset_as_numpy_tuple
     )
 
     output_onnx_file_path = Path(
         tempfile.mkstemp(suffix=".onnx")[1] if output_onnx_file is None else output_onnx_file
     )
 
     use_tempfile: bool = output_onnx_file is None
 
+    assert_true(
+        isinstance(torch_model, torch.nn.Module),
+        "The compile_brevitas_qat_model function must be called on a torch.nn.Module",
+    )
+
+    has_any_qnn_layers = any(
+        isinstance(layer, (QNNMixingLayer, QNNUnivariateLayer)) for layer in torch_model.modules()
+    )
+
+    assert_true(
+        has_any_qnn_layers,
+        "The compile_brevitas_qat_model was called on a torch.nn.Module that contains "
+        "no Brevitas quantized layers, consider using compile_torch_model instead",
+    )
+
     # Brevitas to ONNX
     exporter = BrevitasONNXManager()
     # Here we add a "eliminate_nop_pad" optimization step for onnxoptimizer
     # https://github.com/onnx/optimizer/blob/master/onnxoptimizer/passes/eliminate_nop_pad.h#L5
     # It deletes 0-values padding.
     # This is needed because AvgPool2d adds a 0-Pad operation that then breaks the compilation
     # A list of steps that can be added can be found in the following link
@@ -341,27 +370,59 @@
         input_shape=dummy_input_for_tracing[0].shape,
         export_path=str(output_onnx_file_path),
         keep_initializers_as_inputs=False,
         opset_version=OPSET_VERSION_FOR_ONNX_EXPORT,
     )
     onnx_model = remove_initializer_from_input(onnx_model)
 
+    if n_bits is None:
+        n_bits = {
+            "model_inputs": 8,
+            "op_weights": 8,
+            "op_inputs": 8,
+            "model_outputs": 8,
+        }
+    elif isinstance(n_bits, int):
+        n_bits = {
+            "model_inputs": n_bits,
+            "op_weights": n_bits,
+            "op_inputs": n_bits,
+            "model_outputs": n_bits,
+        }
+    elif isinstance(n_bits, dict):
+        assert_true(
+            isinstance(n_bits, dict) and set(n_bits.keys()) == {"model_inputs", "model_outputs"},
+            "When importing a Brevitas QAT network, n_bits can only contain the following keys: "
+            '"model_inputs", "model_outputs"',
+        )
+
+        n_bits = {
+            "model_inputs": n_bits["model_inputs"],
+            "op_weights": n_bits["model_inputs"],
+            "op_inputs": n_bits["model_inputs"],
+            "model_outputs": n_bits["model_outputs"],
+        }
+    assert_true(
+        n_bits is None or isinstance(n_bits, (int, dict)),
+        "The n_bits parameter must be either a dictionary, an integer or None",
+    )
+
     # Compile using the ONNX conversion flow, in QAT mode
-    q_module_vl = compile_onnx_model(
+    q_module = compile_onnx_model(
         onnx_model,
         torch_inputset,
         n_bits=n_bits,
         import_qat=True,
-        compilation_artifacts=compilation_artifacts,
+        artifacts=artifacts,
         show_mlir=show_mlir,
-        use_virtual_lib=use_virtual_lib,
+        rounding_threshold_bits=rounding_threshold_bits,
         configuration=configuration,
         p_error=p_error,
         global_p_error=global_p_error,
-        verbose_compilation=verbose_compilation,
+        verbose=verbose,
     )
 
     # Remove the tempfile if we used one
     if use_tempfile:
         output_onnx_file_path.unlink()
 
-    return q_module_vl
+    return q_module
```

## concrete/ml/version.py

```diff
@@ -1,3 +1,3 @@
 """File to manage the version of the package."""
 # Auto-generated by "make set_version" do not modify
-__version__ = "0.6.1"
+__version__ = "1.0.0"
```

## Comparing `concrete_ml-0.6.1.dist-info/LICENSE` & `concrete_ml-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `concrete_ml-0.6.1.dist-info/RECORD` & `concrete_ml-1.0.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,55 @@
 concrete/__init__.py,sha256=MXQ2ILkTW4ziKnd7dVxTEVOpHe8clGF34EXxmBCF_pk,284
-concrete/ml/__init__.py,sha256=htzTyO9HYHXRqKiUO0PLiYat1jwU4Z1xcc0NDWw9mK8,50
+concrete/ml/__init__.py,sha256=MkPEAQmtmfFHFJWlw1gMaVr07GLjPuIBv85lNFSp0aI,1722
 concrete/ml/common/__init__.py,sha256=dXaklwVfEYsMLqyH_YFOjGuxnyzoZuApIm8dKLefybw,95
-concrete/ml/common/check_inputs.py,sha256=FArVR452U0OHgbGxkOPk_RLqDNSJTzk-nclqVhMJ8NU,1574
+concrete/ml/common/check_inputs.py,sha256=wj_oyESYWHemVsPRBC25OQc8a2pX2j7fYGpw8lCeKUA,2519
 concrete/ml/common/debugging/__init__.py,sha256=_eh1MBBmnk2o1M4YGbH0Cbr_cEPjFOVz5wsp080HonE,101
 concrete/ml/common/debugging/custom_assert.py,sha256=qrTn_5Nu2hxsrPB-9bM_6NFTOQ9MakFaomT9XuHXpKU,2377
-concrete/ml/common/utils.py,sha256=LIAUy2j38TGzqz7jRpqHj6rbMhLbAP_-QRjYpSIW2KE,6116
+concrete/ml/common/serialization/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+concrete/ml/common/serialization/dumpers.py,sha256=YQge8j1daH-zCeC6mwYkkOrQERd7oyrwiFIM9hhqtyM,1310
+concrete/ml/common/serialization/encoder.py,sha256=TsZ4_FnfWpgk87CpeQDCyqANGmsJ3OlEKmWXBG9fiJk,2018
+concrete/ml/common/serialization/loaders.py,sha256=eCiLRIsTljMQsuzTLYj7wxjdhb4eyub3E-kFDV8ufCo,2856
+concrete/ml/common/utils.py,sha256=BWwck2DQk-6fVYw2mJ6bO9BPYnASm5RUP25Zh_sfGbA,17216
+concrete/ml/deployment/Dockerfile.server,sha256=TbSoyy195L9ttQnEf4YJ70yMuphZRHZvGep1GI4kRlM,235
 concrete/ml/deployment/__init__.py,sha256=jgaPZMSlsJy1KF45EI92rQ7e2CKEpmLdaWcwwFEPeZ8,121
-concrete/ml/deployment/fhe_client_server.py,sha256=LFXvyB7c4ODWX1Dsmv2L4tB4M1KBqey04HJcXjMEhTk,12249
+concrete/ml/deployment/deploy_to_aws.py,sha256=Cpc5Rg7VR73zMxd1IAmLD3j8ClpNsCIL71Qn_GJm6i8,17568
+concrete/ml/deployment/deploy_to_docker.py,sha256=jqKy9sIFwa-xLCOQAqe9olGYQ5iLt48sUx_4x5rvKIg,3800
+concrete/ml/deployment/fhe_client_server.py,sha256=9w32jHS9PB0D9lanfWO7eSpXU1wF4J5pE9ZOdRuuiuE,15080
+concrete/ml/deployment/server.py,sha256=vb2X9aLE0kfb4fiZikokxNVE-MnBtcVWabtF3ENCYzM,4321
+concrete/ml/deployment/server_requirements.txt,sha256=gyd07Mp8qZPWhuz7QI1kgYS3JbjcPbZK4cL9RDOR_x8,33
+concrete/ml/deployment/utils.py,sha256=yQbGiq2vBaEX2hoZ36z1q4I7KfFACoTaSROGo--Jcps,3285
 concrete/ml/onnx/__init__.py,sha256=LiK0TOCAo7c5-TBk4zcO3PEQmdASN0NgLDYIYUXl464,19
-concrete/ml/onnx/convert.py,sha256=S-BXPAeD5WREhLuDP51-w-hlPIEOnlfBployHGtd7Oc,3467
-concrete/ml/onnx/onnx_impl_utils.py,sha256=lfd4x4-cVYH4_Jo2BbHQQX9syoZrQUvkwazt-VnE6-s,9416
-concrete/ml/onnx/onnx_model_manipulations.py,sha256=1oRzkiDyv0rnSjxRmBDflIhg3_P3XW6wXrLxzx4qUNU,9227
-concrete/ml/onnx/onnx_utils.py,sha256=ZORsZxhXVbcxuofTQ9v_kuteRGrk_OsUBfTRTLoK4yA,9115
-concrete/ml/onnx/ops_impl.py,sha256=du9a4-qZ5-M8bpoGMMTYJMu8DQaGcD6OK1M6hLTtBbY,50990
+concrete/ml/onnx/convert.py,sha256=LC1YtDL_miK0QKYXzwYwLyBt1PTOXqk247BPS714EnA,3472
+concrete/ml/onnx/onnx_impl_utils.py,sha256=1KVD5LkzGt1AKJF0x5qIa2_idQacpws-cW30LWhLO_Y,9401
+concrete/ml/onnx/onnx_model_manipulations.py,sha256=qbWOR40TJy-CoD6p4Cc9xIgu9BGo0xoVrtqty3MXZSc,9684
+concrete/ml/onnx/onnx_utils.py,sha256=V39Fip97h4F85PlhiQduQPFnNizpGjyGyCHFYOHPon8,20192
+concrete/ml/onnx/ops_impl.py,sha256=YYMyuLg2T9C3V3PGMBgbpRV_sOccA-g1-RnyaNAutIs,58040
 concrete/ml/pytest/__init__.py,sha256=5Zk0w3T-MYPF3485ir5kZ1dP7x_VoMIreDMKnJuyBCo,101
-concrete/ml/pytest/torch_models.py,sha256=9ViZiw6WflONwNNrQ7jy5N-vcdGu7V-ZJYKb5n-M3AQ,27539
-concrete/ml/pytest/utils.py,sha256=5cfh9LhWbAWb2miDFEoMznAMjt4_8sc8r2BoOVNqGrk,4767
+concrete/ml/pytest/torch_models.py,sha256=L43QyEEu63vPTYRGdkt-gyLFpt2p8-31D_Ct-dNCE0c,42028
+concrete/ml/pytest/utils.py,sha256=RsOLNe9Ha2kBjk_vTXfM7_VHu_Emu1mYQnoVxF117Tg,8787
 concrete/ml/quantization/__init__.py,sha256=AMEpmLBppr9jRyHOaz9X6dND-u6urnDnkW06X_80JWQ,1081
-concrete/ml/quantization/base_quantized_op.py,sha256=7IrT_-1YcnwgVPuLmYYs7LQNQsY1jJFtlL3RoMUp32s,29563
-concrete/ml/quantization/post_training.py,sha256=4kOnhNNo0FnASbzuhss1rt1-hNlw0cM4dLoW8vHhAGQ,40067
-concrete/ml/quantization/quantized_module.py,sha256=MrfWxLDtOPpnQVSdKag-nRVTSCsz_oynwRN3j4nItvs,16579
-concrete/ml/quantization/quantized_ops.py,sha256=wPNORJFq58OSdrXh1aLKNtvYG1nZQv_vcn8SbJP6lWk,67819
-concrete/ml/quantization/quantizers.py,sha256=M3H_9LS7AAxHC0Dlw_FVTsfpJY79zjqDf0m3RWg-M5o,26653
-concrete/ml/sklearn/__init__.py,sha256=lDOoOLrdHYvSSpEF2rf6N53p04CosKKqUL8J9XBDv1M,452
-concrete/ml/sklearn/base.py,sha256=6oP2bDALlMPRIRQ-fEzzXpWb3686759Zop9OdeleGo4,63178
-concrete/ml/sklearn/glm.py,sha256=XG3db3J9AEb1uuAHyn_-3TGL58v8cwjlS-HrmhNkHlc,10913
-concrete/ml/sklearn/linear_model.py,sha256=Zbhv3Izp7liPOlEAQKWCqNoR2fYhoZZC-J0_9z255Ac,9283
-concrete/ml/sklearn/protocols.py,sha256=6ZGFCQq8b9G7ps5Pi0-y8FITJD2uL-1TJwlAC4uZGTI,6926
-concrete/ml/sklearn/qnn.py,sha256=5bRCEGCLUbI_5_7-urQ2hK7rvhbIt4yWdQY85iQiaPM,20369
-concrete/ml/sklearn/rf.py,sha256=xgF0qaFR2oo1GHIJNY8md1Muc5FnxKsuUw9DARscF6s,4043
-concrete/ml/sklearn/svm.py,sha256=lNBU98bKwSg1JDAnflCgSnXb_o3MzQ-Ov-j-s1LvcdI,3813
-concrete/ml/sklearn/torch_modules.py,sha256=_hKSOND1kzIJuu2otjF1ewPjRBJHLwLXjWGnLvAzDKA,1393
-concrete/ml/sklearn/tree.py,sha256=R5PjBwYGZ5uiJX4iTFCgj1du0-jeixwIoKmRdQKzoqQ,3676
-concrete/ml/sklearn/tree_to_numpy.py,sha256=yRNaMnwGOIJzXQnlcnK9B5dFBaLrjmxmPnHQdDBfGRk,8292
-concrete/ml/sklearn/xgb.py,sha256=oaYMTYvyEAFtxFqVuJ1H12is_4nRJ5DgAGwZDbK0WSs,13273
+concrete/ml/quantization/base_quantized_op.py,sha256=Od8BimxvZC6MMdX15laqwUAh0JZ1O7quCewWT6i0aXs,35250
+concrete/ml/quantization/post_training.py,sha256=A6W2K-m4RA_Usx6EfuOluqE3OPO_oVMIMScflFQrp5o,43507
+concrete/ml/quantization/quantized_module.py,sha256=PzkKfuZNoGxKLjD8OzWgcl64Qt2860ziYdbMBMWu2Q4,24344
+concrete/ml/quantization/quantized_ops.py,sha256=7PGQTAQpnZcztL8vyXkkqoIZb_PY_u8KS4Lns2d8Aq0,80967
+concrete/ml/quantization/quantizers.py,sha256=dKngjgtunqBZzZwCPg-qneW69Pgr9ufpCIqcuxurwHo,37503
+concrete/ml/search_parameters/__init__.py,sha256=-TGfmte3AvAn2ajLxLd-FCbru6_Ml9DiKeG7ooR819Q,77
+concrete/ml/search_parameters/p_error_search.py,sha256=rQe56M66QmZKiUfk1bRVxTYRKDSC2u5XhfG3mx4lC2s,21176
+concrete/ml/sklearn/__init__.py,sha256=PPR2RuegE_0-OOA9QhYyZ75lxm7rZiAWI4MqeQwRoCo,4679
+concrete/ml/sklearn/base.py,sha256=je41FdKhLGT3wyqmaeCyKgVh5CbVhtm-utXj4sF73Uk,62686
+concrete/ml/sklearn/glm.py,sha256=xca19CFi-QhSTNm9I3anlK7PxEqDx2e1Z9MXw_NKJF8,13633
+concrete/ml/sklearn/linear_model.py,sha256=kQOGeIZjXUUmpSvxCWe-XKd02iY5MuXebvakEWJScvA,25212
+concrete/ml/sklearn/qnn.py,sha256=-VIkCtZO89uTjrNBY4fgcarIqnrqqPZ8OSRB2Nt6B4A,13339
+concrete/ml/sklearn/qnn_module.py,sha256=5jxigI42-aCG0_ko1u6aV6RXOjBhSD9afSorvD-V-n4,12567
+concrete/ml/sklearn/rf.py,sha256=QSqXnHua77SLFX5crYe5s-XWsmz4AR06QTWSC7uuIOU,12243
+concrete/ml/sklearn/svm.py,sha256=bmfwiJcb28LzPbfiaGiNeHtEug8tzmoBHes_ee4cNgs,10614
+concrete/ml/sklearn/tree.py,sha256=1d2uOLER4HfVWb3tr3nHMEyFTQdpaoq2bjrSPkSHDD8,10394
+concrete/ml/sklearn/tree_to_numpy.py,sha256=PMK6VQskkZhW6YzhtCTl2pcg1BvZc5QpHdKY2KfnGw0,10920
+concrete/ml/sklearn/xgb.py,sha256=cHq7HyONowCiS-rCTh1TX_b-v0Ns7Vec0xm4DmB0GT4,20074
 concrete/ml/torch/__init__.py,sha256=aUQ25-hJdirZCa20KqaVMrt2PnpnSXBCVw7QvLQ_BoQ,83
-concrete/ml/torch/compile.py,sha256=1FuXcQ25o5Yb-DfhsEW1wq63SR3rrGRSKWaeb36hh30,15356
+concrete/ml/torch/compile.py,sha256=gwWBFuNdkQocDupvpw-l9LT6XKSEWS7ZS6ju8oshc_o,17532
 concrete/ml/torch/numpy_module.py,sha256=PKJmuGL0Q7nzfXsbwz9Mr1J-w5MDGkpzRnZY86TylOI,3174
-concrete/ml/version.py,sha256=QBgqykT3FqU5DWZpMXOhnE9hlSTVMR1uGOm7O3Gomyc,124
-concrete_ml-0.6.1.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-concrete_ml-0.6.1.dist-info/LICENSE,sha256=Q2TUW9iqL5JOnEcNTstSvNPYRnF-iQi24FUla8oUEwE,1546
-concrete_ml-0.6.1.dist-info/METADATA,sha256=RN5o2__HFbVOTur2cCg9ree4nagz1aGztCZBbdCVbqI,2307
-concrete_ml-0.6.1.dist-info/RECORD,,
+concrete/ml/version.py,sha256=SQu4i6SxaSjblZS1KOTjixyzzbdHd9y4oE9gZ0CY6nY,124
+concrete_ml-1.0.0.dist-info/LICENSE,sha256=Q2TUW9iqL5JOnEcNTstSvNPYRnF-iQi24FUla8oUEwE,1546
+concrete_ml-1.0.0.dist-info/WHEEL,sha256=vxFmldFsRN_Hx10GDvsdv1wroKq8r5Lzvjp6GZ4OO8c,88
+concrete_ml-1.0.0.dist-info/METADATA,sha256=UU16LiaRSne7CAAWzLY7wN1pBxb1vdNXtTZ489KT928,11662
+concrete_ml-1.0.0.dist-info/RECORD,,
```

