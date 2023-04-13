# Comparing `tmp/keras_generators-1.2.6-py3-none-any.whl.zip` & `tmp/keras_generators-1.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 28550 bytes, number of entries: 16
+Zip file size: 27904 bytes, number of entries: 16
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-08 16:27 examples/__init__.py
--rw-rw-rw-  2.0 fat     6233 b- defN 23-Mar-08 16:27 examples/predict_stock_price.py
+-rw-rw-rw-  2.0 fat     6233 b- defN 23-Apr-13 14:38 examples/predict_stock_price.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-08 16:27 keras_generators/__init__.py
 -rw-rw-rw-  2.0 fat     7068 b- defN 23-Mar-08 16:27 keras_generators/callbacks.py
--rw-rw-rw-  2.0 fat     2637 b- defN 23-Mar-08 16:27 keras_generators/common.py
+-rw-rw-rw-  2.0 fat      520 b- defN 23-Apr-13 14:20 keras_generators/common.py
 -rw-rw-rw-  2.0 fat    10842 b- defN 23-Mar-08 16:27 keras_generators/encoders.py
 -rw-rw-rw-  2.0 fat    33395 b- defN 23-Mar-08 16:27 keras_generators/generators.py
 -rw-rw-rw-  2.0 fat     4139 b- defN 23-Mar-08 19:39 keras_generators/splitters.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-08 16:27 keras_generators/model_abstractions/__init__.py
 -rw-rw-rw-  2.0 fat     7224 b- defN 23-Mar-08 20:48 keras_generators/model_abstractions/model_object.py
--rw-rw-rw-  2.0 fat     3271 b- defN 23-Mar-08 16:27 keras_generators/model_abstractions/model_params.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Mar-08 20:49 keras_generators-1.2.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     9777 b- defN 23-Mar-08 20:49 keras_generators-1.2.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-08 20:49 keras_generators-1.2.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       26 b- defN 23-Mar-08 20:49 keras_generators-1.2.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1422 b- defN 23-Mar-08 20:49 keras_generators-1.2.6.dist-info/RECORD
-16 files, 97684 bytes uncompressed, 26164 bytes compressed:  73.2%
+-rw-rw-rw-  2.0 fat     3188 b- defN 23-Apr-13 14:19 keras_generators/model_abstractions/model_params.py
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Apr-13 14:41 keras_generators-1.3.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     9891 b- defN 23-Apr-13 14:41 keras_generators-1.3.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-13 14:41 keras_generators-1.3.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       26 b- defN 23-Apr-13 14:41 keras_generators-1.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1421 b- defN 23-Apr-13 14:41 keras_generators-1.3.0.dist-info/RECORD
+16 files, 95597 bytes uncompressed, 25518 bytes compressed:  73.3%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: keras_generators/model_abstractions/model_object.py
 Comment: 
 
 Filename: keras_generators/model_abstractions/model_params.py
 Comment: 
 
-Filename: keras_generators-1.2.6.dist-info/LICENSE
+Filename: keras_generators-1.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: keras_generators-1.2.6.dist-info/METADATA
+Filename: keras_generators-1.3.0.dist-info/METADATA
 Comment: 
 
-Filename: keras_generators-1.2.6.dist-info/WHEEL
+Filename: keras_generators-1.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: keras_generators-1.2.6.dist-info/top_level.txt
+Filename: keras_generators-1.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: keras_generators-1.2.6.dist-info/RECORD
+Filename: keras_generators-1.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## keras_generators/common.py

```diff
@@ -1,75 +1,14 @@
 #!/usr/bin/env python
 # Author: ASU --<andrei.suiu@gmail.com>
 
-import json
 from json import JSONEncoder
-from typing import Any, Callable, Optional, cast
 
 import numpy as np
-from pydantic import BaseModel, Extra
-from tsx import TS
-
-
-class TSJSONEncoder(json.JSONEncoder):
-    def encode(self, o: Any) -> str:
-        if isinstance(o, dict):
-            new_o = o.copy()
-            for k in new_o:
-                if isinstance(new_o[k], TS):
-                    new_o[k] = new_o[k].as_iso
-            return super().encode(new_o)
-        return super().encode(o)
-
-
-class SerializableStruct(BaseModel):
-    def json(
-            self,
-            *,
-            include=None,
-            exclude=None,
-            by_alias: bool = False,
-            skip_defaults: bool = None,
-            exclude_unset: bool = False,
-            exclude_defaults: bool = False,
-            exclude_none: bool = False,
-            encoder: Optional[Callable[[Any], Any]] = None,
-            **dumps_kwargs: Any,
-    ) -> str:
-        """
-        Generate a JSON representation of the model, `include` and `exclude` arguments as per `dict()`.
-
-        `encoder` is an optional function to supply as `default` to json.dumps(), other arguments as per `json.dumps()`.
-        """
-        if skip_defaults is not None:
-            exclude_unset = skip_defaults
-        encoder = cast(Callable[[Any], Any], encoder or self.__json_encoder__)
-        data = self.dict(
-            include=include,
-            exclude=exclude,
-            by_alias=by_alias,
-            exclude_unset=exclude_unset,
-            exclude_defaults=exclude_defaults,
-            exclude_none=exclude_none,
-        )
-        if self.__custom_root_type__:
-            # below is a hardcoding workaround instead of original utils.ROOT_KEY as Pydantic doesn't have it on Unix
-            data = data["__root__"]
-
-        return self.__config__.json_dumps(data, default=encoder, cls=TSJSONEncoder, **dumps_kwargs)
-
-    class Config:
-        arbitrary_types_allowed = True
-
-
-class SerializableImmutableStruct(SerializableStruct):
-    class Config:
-        allow_mutation = False
-        arbitrary_types_allowed = True
-        extra = Extra.forbid
+from pydantic import Extra
 
 
 class NumpyArrayEncoder(JSONEncoder):
     def default(self, obj):
         if isinstance(obj, np.ndarray):
             return obj.tolist()
         return JSONEncoder.default(self, obj)
```

## keras_generators/model_abstractions/model_params.py

```diff
@@ -1,21 +1,20 @@
 #!/usr/bin/env python
 # Author: ASU --<andrei.suiu@gmail.com>
 
 import json
 from pathlib import Path
 from typing import Optional, List
 
-from pydantic import constr, conint, PositiveInt, confloat, Extra
+from pydantic import constr, conint, PositiveInt, confloat
+from pyxtension.models import ImmutableExtModel
 from typing_extensions import Literal
 
-from ..common import SerializableImmutableStruct
 
-
-class ModelParams(SerializableImmutableStruct):
+class ModelParams(ImmutableExtModel):
     """
     This class is a base class used to encode the parameters of a model.
     It's easy serializable and deserializable to/from a file.
     It's immutable, and versioned. It won't deserialize an instance of a class with a different version.
     Feel free to extend this class and add more hyper-parameters and architecture parameters for your model like:
         - number of Dense layers
         - type of RNN layer (LSTM, GRU or RNN)
@@ -42,20 +41,17 @@
 
     loss: Literal['mse'] = 'mse'
     metrics: List[Literal['mse']] = ['mse']
 
     input_name: str = "input"  # Name of the main input layer
     target_name: str = "target"  # Name of the main target layer
 
-    class Config:
-        extra = Extra.forbid
-
     def get_config(self):
         """Returns the config dictionary for a `ModelParams` instance."""
-        return {"data": json.dumps(self.dict())}
+        return {"data": self.json()}
 
     def __repr__(self) -> str:
         str_repr = self.__repr_str__(",\n")
         return f"{self.__repr_name__()}({str_repr})"
 
     @property
     def out_dim(self):
```

## Comparing `keras_generators-1.2.6.dist-info/LICENSE` & `keras_generators-1.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `keras_generators-1.2.6.dist-info/METADATA` & `keras_generators-1.3.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-generators
-Version: 1.2.6
+Version: 1.3.0
 Summary: Multi-dimensional/Multi-input/Multi-output Data preprocessing and Batch Generators for Keras models
 Home-page: https://github.com/asuiu/keras-generators
 Author: Andrei Suiu
 Author-email: andrei.suiu@gmail.com
 License: Apache License 2.0
 Keywords: ML,DataGenerators,Keras,tensorflow
 Classifier: Intended Audience :: Developers
@@ -17,20 +17,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: packaging
-Requires-Dist: tensorflow (>=2.8.0)
-Requires-Dist: scikit-learn (>=0.22.2)
 Requires-Dist: numpy (>=1.20)
+Requires-Dist: pip (>=22.1.2)
 Requires-Dist: pydantic (>=1.10.2)
-Requires-Dist: tsx (>=0.0.4)
+Requires-Dist: scikit-learn (>=0.22.2)
+Requires-Dist: setuptools (>=63.4.1)
+Requires-Dist: tensorflow (>=2.8.0)
+Requires-Dist: tsx (>=0.1.1)
+Requires-Dist: wheel (>=0.37.1)
+Requires-Dist: pyxtension (>=1.15.0)
 Provides-Extra: tests
 
 # keras-generators
 
 Multi-dimensional/Multi-input/Multi-output Data preprocessing and Batch Generators for Tensorflow models
 
 ## Installation
```

## Comparing `keras_generators-1.2.6.dist-info/RECORD` & `keras_generators-1.3.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 examples/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 examples/predict_stock_price.py,sha256=OLhlvKkctYf12kGk7QgxSWKVWM61EI6r0NzXwSKOuAY,6233
 keras_generators/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 keras_generators/callbacks.py,sha256=fGCSRg13d7oPutoXVnSA2R72ri9kGcZnj47LdNCCcvs,7068
-keras_generators/common.py,sha256=jEUsw52tSCGSZqA4iOifdHk1RrVpxbo_p1-BPmhaKnE,2637
+keras_generators/common.py,sha256=sFcCpVV8dJBrWG3Ry9MhpNZC0l-MZAMBdUBJNwlZYs4,520
 keras_generators/encoders.py,sha256=WwviJAdT_mYwjSIn9wqzt3-DEjLNl7jbliKC2jjlYik,10842
 keras_generators/generators.py,sha256=FxGsroItR3HehAMv9f8FYzPLwsoj5lpF15GigNROnrY,33395
 keras_generators/splitters.py,sha256=O7AKehcoPiQNjv1kuZWOoax-yvnjTFPuOkwLjox-qMw,4139
 keras_generators/model_abstractions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 keras_generators/model_abstractions/model_object.py,sha256=k5aBRhSseV0gzTyDYpMvjvN_wH5lPFLKQF4Nis0rUsM,7224
-keras_generators/model_abstractions/model_params.py,sha256=HOJatwbb_25aoV4hYpDQWGe06itOdl4QaRwxafF-9vs,3271
-keras_generators-1.2.6.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-keras_generators-1.2.6.dist-info/METADATA,sha256=5pjmKfuuicInl-hDsE7pe56jBwnbJ4gaLr07owEW2QY,9777
-keras_generators-1.2.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-keras_generators-1.2.6.dist-info/top_level.txt,sha256=6h3qtPKTpHlh7dFVHfOuDDRxVzXpjgb3hL-O3LMXK2w,26
-keras_generators-1.2.6.dist-info/RECORD,,
+keras_generators/model_abstractions/model_params.py,sha256=-Dr1zxdO4NaJ9ibYq0IsQg3n79AJyiGv4aaPma67__E,3188
+keras_generators-1.3.0.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+keras_generators-1.3.0.dist-info/METADATA,sha256=Tv6LZ1hYPWPP3N6rgD6w4s6BDfY1vxHC5tU8_EaPGwo,9891
+keras_generators-1.3.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+keras_generators-1.3.0.dist-info/top_level.txt,sha256=6h3qtPKTpHlh7dFVHfOuDDRxVzXpjgb3hL-O3LMXK2w,26
+keras_generators-1.3.0.dist-info/RECORD,,
```

