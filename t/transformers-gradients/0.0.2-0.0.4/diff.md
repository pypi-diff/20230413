# Comparing `tmp/transformers_gradients-0.0.2.tar.gz` & `tmp/transformers_gradients-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformers_gradients-0.0.2.tar", last modified: Wed Apr 12 23:03:23 2023, max compression
+gzip compressed data, was "transformers_gradients-0.0.4.tar", last modified: Thu Apr 13 08:05:24 2023, max compression
```

## Comparing `transformers_gradients-0.0.2.tar` & `transformers_gradients-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      173 2023-04-12 23:03:09.626808 transformers_gradients-0.0.2/Readme.md
--rw-r--r--   0        0        0     4429 2023-04-12 23:03:09.626808 transformers_gradients-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      357 2023-04-12 23:03:09.626808 transformers_gradients-0.0.2/src/transformers_gradients/__init__.py
--rw-r--r--   0        0        0     5231 2023-04-12 23:03:09.626808 transformers_gradients-0.0.2/src/transformers_gradients/config.py
--rw-r--r--   0        0        0       64 2023-04-12 23:03:09.626808 transformers_gradients-0.0.2/src/transformers_gradients/py.typed
--rw-r--r--   0        0        0        0 2023-04-12 23:03:09.626808 transformers_gradients-0.0.2/src/transformers_gradients/text_classification/__init__.py
--rw-r--r--   0        0        0    18647 2023-04-12 23:03:09.626808 transformers_gradients-0.0.2/src/transformers_gradients/text_classification/explanation_func.py
--rw-r--r--   0        0        0     2714 2023-04-12 23:03:09.626808 transformers_gradients-0.0.2/src/transformers_gradients/text_classification/explanation_func.pyi
--rw-r--r--   0        0        0     1171 2023-04-12 23:03:09.626808 transformers_gradients-0.0.2/src/transformers_gradients/types.py
--rw-r--r--   0        0        0     1507 2023-04-12 23:03:09.626808 transformers_gradients-0.0.2/src/transformers_gradients/util.py
--rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 transformers_gradients-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    48301 2023-04-13 08:05:16.689063 transformers_gradients-0.0.4/Readme.md
+-rw-r--r--   0        0        0     4429 2023-04-13 08:05:16.689063 transformers_gradients-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      357 2023-04-13 08:05:16.689063 transformers_gradients-0.0.4/src/transformers_gradients/__init__.py
+-rw-r--r--   0        0        0     5241 2023-04-13 08:05:16.689063 transformers_gradients-0.0.4/src/transformers_gradients/config.py
+-rw-r--r--   0        0        0     7351 2023-04-13 08:05:16.689063 transformers_gradients-0.0.4/src/transformers_gradients/plotting.py
+-rw-r--r--   0        0        0       64 2023-04-13 08:05:16.689063 transformers_gradients-0.0.4/src/transformers_gradients/py.typed
+-rw-r--r--   0        0        0        0 2023-04-13 08:05:16.689063 transformers_gradients-0.0.4/src/transformers_gradients/text_classification/__init__.py
+-rw-r--r--   0        0        0    18474 2023-04-13 08:05:16.689063 transformers_gradients-0.0.4/src/transformers_gradients/text_classification/explanation_func.py
+-rw-r--r--   0        0        0     2610 2023-04-13 08:05:16.689063 transformers_gradients-0.0.4/src/transformers_gradients/text_classification/explanation_func.pyi
+-rw-r--r--   0        0        0     1179 2023-04-13 08:05:16.689063 transformers_gradients-0.0.4/src/transformers_gradients/types.py
+-rw-r--r--   0        0        0     1273 2023-04-13 08:05:16.689063 transformers_gradients-0.0.4/src/transformers_gradients/util.py
+-rw-r--r--   0        0        0    49559 1970-01-01 00:00:00.000000 transformers_gradients-0.0.4/PKG-INFO
```

### Comparing `transformers_gradients-0.0.2/pyproject.toml` & `transformers_gradients-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "transformers_gradients"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "0.0.2"  # Required
+version = "0.0.4"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Gradient-based XAI methods for TensorFlow transformers."  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `transformers_gradients-0.0.2/src/transformers_gradients/config.py` & `transformers_gradients-0.0.4/src/transformers_gradients/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         Function to apply noise, default=multiplication.
     seed:
         PRNG seed used for noise generating distributions.
     """
 
     n: int = 10
     mean: float = 1.0
-    std: float = 0.2
+    std: float = 0.0055
     explain_fn: Union[ExplainFn, str] = "IntGrad"
     noise_fn: ApplyNoiseFn = tf.function(
         reduce_retracing=True, jit_compile=is_xla_compatible_platform()
     )(lambda a, b: a * b)
 
 
 class SmoothGradConfing(NamedTuple):
@@ -71,15 +71,15 @@
         Function to apply noise, default=multiplication.
     seed:
         PRNG seed used for noise generating distributions.
     """
 
     n: int = 10
     mean: float = 1.0
-    std: float = 0.2
+    std: float = 0.0055
     explain_fn: Union[ExplainFn, str] = "IntGrad"
     noise_fn: ApplyNoiseFn = tf.function(
         reduce_retracing=True, jit_compile=is_xla_compatible_platform()
     )(lambda a, b: a * b)
 
 
 class NoiseGradPlusPlusConfig(NamedTuple):
@@ -106,16 +106,16 @@
         PRNG seed used for noise generating distributions.
     """
 
     n: int = 10
     m: int = 10
     mean: float = 1.0
     sg_mean: float = 0.0
-    std: float = 0.2
-    sg_std: float = 0.4
+    std: float = 0.0055
+    sg_std: float = 0.05
     explain_fn: Union[ExplainFn, str] = "IntGrad"
     noise_fn: ApplyNoiseFn = tf.function(
         reduce_retracing=True, jit_compile=is_xla_compatible_platform()
     )(lambda a, b: a * b)
 
 
 def update_config(**kwargs):
```

### Comparing `transformers_gradients-0.0.2/src/transformers_gradients/text_classification/explanation_func.py` & `transformers_gradients-0.0.4/src/transformers_gradients/text_classification/explanation_func.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 from __future__ import annotations
 
 import gc
 from functools import wraps, partial
 from operator import itemgetter
+from typing import List
 
 import tensorflow as tf
 import tensorflow_probability as tfp
 from tensorflow_probability.python.distributions.normal import Normal
 from transformers import TFPreTrainedModel, PreTrainedTokenizerBase
 
 from transformers_gradients.config import (
     IntGradConfig,
     NoiseGradPlusPlusConfig,
     NoiseGradConfig,
     SmoothGradConfing,
     resolve_baseline_explain_fn,
 )
-from transformers_gradients.types import (
-    Explanation,
-)
 from transformers_gradients.util import (
     value_or_default,
     is_xla_compatible_platform,
     get_input_ids,
     as_tensor,
-    map_dict,
+    cached_tf_function,
 )
 
 
 def plain_text_hook(func):
     @wraps(func)
     def wrapper(
         model: TFPreTrainedModel,
-        x_batch: list[str] | tf.Tensor,
+        x_batch: List[str] | tf.Tensor,
         y_batch: tf.Tensor,
         tokenizer: PreTrainedTokenizerBase | None = None,
         **kwargs,
     ):
         if isinstance(x_batch[0], str):
             input_ids, predict_kwargs = get_input_ids(tokenizer, x_batch)
             embeddings = model.get_input_embeddings()(input_ids)
@@ -50,15 +48,14 @@
         else:
             return func(model, as_tensor(x_batch), as_tensor(y_batch), **kwargs)
 
     return wrapper
 
 
 @plain_text_hook
-@tf.function(reduce_retracing=True, jit_compile=is_xla_compatible_platform())
 def gradient_norm(
     model: TFPreTrainedModel,
     x_batch: tf.Tensor,
     y_batch: tf.Tensor,
     **kwargs,
 ) -> tf.Tensor:
     """
@@ -90,27 +87,27 @@
     Returns
     -------
     a_batch:
         List of tuples, where 1st element is tokens and 2nd is the scores assigned to the tokens.
 
     """
 
-    @tf.function(reduce_retracing=True, jit_compile=is_xla_compatible_platform())
+    @cached_tf_function
     def grad_norm_fn(xx_batch, yy_batch, **kwargs):
         with tf.GradientTape() as tape:
             tape.watch(xx_batch)
             logits = model(
                 None, inputs_embeds=xx_batch, training=False, **kwargs
             ).logits
             logits_for_label = logits_for_labels(logits, yy_batch)
 
         grads = tape.gradient(logits_for_label, xx_batch)
         return tf.linalg.norm(grads, axis=-1)
 
-    return grad_norm_fn(x_batch, y_batch, **kwargs)
+    return grad_norm_fn(x_batch, y_batch, **tf.nest.map_structure(as_tensor, kwargs))
 
 
 @plain_text_hook
 def gradient_x_input(
     model: TFPreTrainedModel,
     x_batch: tf.Tensor,
     y_batch: tf.Tensor,
@@ -145,26 +142,26 @@
     Returns
     -------
     a_batch:
         List of tuples, where 1st element is tokens and 2nd is the scores assigned to the tokens.
 
     """
 
-    @tf.function(reduce_retracing=True, jit_compile=is_xla_compatible_platform())
+    @cached_tf_function
     def grad_x_input_fn(xx_batch, yy_batch, **kwargs):
         with tf.GradientTape() as tape:
             tape.watch(xx_batch)
             logits = model(
                 None, inputs_embeds=xx_batch, training=False, **kwargs
             ).logits
             logits_for_label = logits_for_labels(logits, yy_batch)
         grads = tape.gradient(logits_for_label, xx_batch)
         return tf.math.reduce_sum(xx_batch * grads, axis=-1)
 
-    return grad_x_input_fn(x_batch, y_batch, **kwargs)
+    return grad_x_input_fn(x_batch, y_batch, **tf.nest.map_structure(as_tensor, kwargs))
 
 
 @plain_text_hook
 def integrated_gradients(
     model: TFPreTrainedModel,
     x_batch: tf.Tensor,
     y_batch: tf.Tensor,
@@ -213,50 +210,52 @@
     >>> unk_token_embedding = model.embedding_lookup([model.tokenizer.unk_token_id])[0, 0]
     >>> unknown_token_baseline_function = tf.function(lambda x: unk_token_embedding)
     >>> config = IntGradConfig(baseline_fn=unknown_token_baseline_function)
     >>> integrated_gradients(..., ..., ..., config=config)
 
     """
     config = value_or_default(config, lambda: IntGradConfig())
-    interpolated_embeddings = tf.vectorized_map(
+    # tf.vectorized_map(
+    interpolated_embeddings = tf.map_fn(
         lambda i: interpolate_inputs(
             config.baseline_fn(i), i, tf.constant(config.num_steps)
         ),
         x_batch,
     )
+    kwargs = tf.nest.map_structure(as_tensor, kwargs)
 
     if config.batch_interpolated_inputs:
         return _integrated_gradients_batched(
             model,
             interpolated_embeddings,
             y_batch,
             tf.constant(config.num_steps),
-            **kwargs,
+            **tf.nest.map_structure(as_tensor, kwargs),
         )
     else:
         return _integrated_gradients_iterative(
             model,
             interpolated_embeddings,
             y_batch,
             **kwargs,
         )
 
 
 @plain_text_hook
-# @tf.function(reduce_retracing=True, jit_compile=is_xla_compatible_platform())
 def smooth_grad(
     model: TFPreTrainedModel,
     x_batch: tf.Tensor,
     y_batch: tf.Tensor,
     config: SmoothGradConfing | None = None,
     **kwargs,
-) -> list[Explanation] | tf.Tensor:
+) -> tf.Tensor:
     config = value_or_default(config, lambda: SmoothGradConfing())
     explain_fn = resolve_baseline_explain_fn(config.explain_fn)
 
+    @cached_tf_function
     def smooth_grad_fn(xx_batch, yy_batch, n, mean, std, **kwargs):
         explanations_array = tf.TensorArray(
             xx_batch.dtype,
             size=n,
             clear_after_read=True,
             colocate_with_first_write_call=True,
         )
@@ -278,26 +277,26 @@
 
     return smooth_grad_fn(
         x_batch,
         y_batch,
         tf.constant(config.n),
         tf.constant(config.mean),
         tf.constant(config.std),
-        **kwargs,
+        **tf.nest.map_structure(as_tensor, kwargs),
     )
 
 
 @plain_text_hook
 def noise_grad(
     model: TFPreTrainedModel,
-    x_batch: list[str] | tf.Tensor,
+    x_batch: tf.Tensor,
     y_batch: tf.Tensor,
     config: NoiseGradConfig | None = None,
     **kwargs,
-) -> list[Explanation] | tf.Tensor:
+) -> tf.Tensor:
     """
     NoiseGrad++ is a state-of-the-art gradient based XAI method, which enhances baseline explanation function
     by adding stochasticity to model's weights. The implementation is based
     on https://github.com/understandable-machine-intelligence-lab/NoiseGrad/blob/master/src/noisegrad.py#L80.
 
     Parameters
     ----------
@@ -373,15 +372,15 @@
 @plain_text_hook
 def noise_grad_plus_plus(
     model: TFPreTrainedModel,
     x_batch: tf.Tensor,
     y_batch: tf.Tensor,
     config: NoiseGradPlusPlusConfig | None = None,
     **kwargs,
-) -> list[Explanation] | tf.Tensor:
+) -> tf.Tensor:
     """
     NoiseGrad++ is a state-of-the-art gradient based XAI method, which enhances baseline explanation function
     by adding stochasticity to model's weights and model's inputs. The implementation is based
     on https://github.com/understandable-machine-intelligence-lab/NoiseGrad/blob/master/src/noisegrad.py#L80.
 
     Parameters
     ----------
@@ -428,23 +427,22 @@
     )
     return noise_grad(model, x_batch, y_batch, config=ng_config, **kwargs)
 
 
 # ----------------------- IntGrad ------------------------
 
 
-@tf.function(reduce_retracing=True, jit_compile=is_xla_compatible_platform())
 def _integrated_gradients_batched(
     model: TFPreTrainedModel,
     x_batch: tf.Tensor,
     y_batch: tf.Tensor,
-    num_steps: int,
+    num_steps: tf.Tensor,
     **kwargs,
-):
-    @tf.function(reduce_retracing=True, jit_compile=is_xla_compatible_platform())
+) -> tf.Tensor:
+    @cached_tf_function
     def int_grad_fn(xx_batch, yy_batch, nnum_steps, **kwargs):
         shape = tf.shape(xx_batch)
         batch_size = shape[0]
 
         interpolated_embeddings = tf.reshape(
             tf.cast(xx_batch, dtype=tf.float32),
             [-1, shape[2], shape[3]],
@@ -474,15 +472,17 @@
         grads = tape.gradient(logits_for_label, interpolated_embeddings)
         grads_shape = tf.shape(grads)
         grads = tf.reshape(
             grads, [batch_size, nnum_steps + 1, grads_shape[1], grads_shape[2]]
         )
         return tf.linalg.norm(tfp.math.trapz(grads, axis=1), axis=-1)
 
-    return int_grad_fn(x_batch, y_batch, num_steps, **kwargs)
+    return int_grad_fn(
+        x_batch, y_batch, num_steps, **tf.nest.map_structure(as_tensor, kwargs)
+    )
 
 
 def _integrated_gradients_iterative(
     model: TFPreTrainedModel,
     x_batch: tf.Tensor,
     y_batch: tf.Tensor,
     **kwargs,
@@ -497,17 +497,19 @@
 
     def pseudo_interpolate(x, embeds):
         return tf.broadcast_to(x, (tf.shape(embeds)[0], *x.shape))
 
     for i in tf.range(batch_size):
         interpolated_embeddings = x_batch[i]
 
+        kwargs_i = tf.nest.map_structure(itemgetter(i), kwargs)
+
         interpolated_kwargs = tf.nest.map_structure(
-            lambda x: pseudo_interpolate(x, interpolated_embeddings),
-            map_dict(kwargs, itemgetter(i)),
+            partial(pseudo_interpolate, embeds=interpolated_embeddings),
+            kwargs_i,
         )
         with tf.GradientTape() as tape:
             tape.watch(interpolated_embeddings)
             logits = model(
                 None,
                 inputs_embeds=interpolated_embeddings,
                 training=False,
@@ -540,15 +542,15 @@
         [1, 0],
     )
     return tf.gather_nd(logits, indexes)
 
 
 @tf.function(reduce_retracing=True, jit_compile=is_xla_compatible_platform())
 def interpolate_inputs(
-    baseline: tf.Tensor, target: tf.Tensor, num_steps: tf.Tensor
+    baseline: tf.Tensor, target: tf.Tensor, num_steps: int
 ) -> tf.Tensor:
     """Gets num_step linearly interpolated inputs from baseline to target."""
     delta = target - baseline
     scales = tf.linspace(0, 1, num_steps + 1)[:, tf.newaxis, tf.newaxis]
     scales = tf.cast(scales, dtype=delta.dtype)
     shape = tf.convert_to_tensor(
         [num_steps + 1, tf.shape(delta)[0], tf.shape(delta)[1]]
```

### Comparing `transformers_gradients-0.0.2/src/transformers_gradients/text_classification/explanation_func.pyi` & `transformers_gradients-0.0.4/src/transformers_gradients/text_classification/explanation_func.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,102 +1,101 @@
-from typing import overload, List, Optional
+from __future__ import annotations
+
+from typing import overload, List
 
 import tensorflow as tf
 from transformers import TFPreTrainedModel, PreTrainedTokenizerBase
 
-from transformers_gradients.types import Explanation
 from transformers_gradients.config import (
     IntGradConfig,
     NoiseGradConfig,
     NoiseGradPlusPlusConfig,
     SmoothGradConfing,
 )
+from transformers_gradients.types import Explanation
 
-def gradient_norm(model, x_batch, y_batch, *args, **kwargs): ...
 @overload
 def gradient_norm(
     model: TFPreTrainedModel,
-    x_batch: list[str],
+    x_batch: List[str],
     y_batch: tf.Tensor,
     tokenizer: PreTrainedTokenizerBase,
-) -> list[Explanation]: ...
+) -> List[Explanation]: ...
 @overload
 def gradient_norm(
     model: TFPreTrainedModel, x_batch: tf.Tensor, y_batch: tf.Tensor, **kwargs
 ) -> tf.Tensor: ...
-def gradient_x_input(
-    model,
-    x_batch,
-    y_batch,
-    tokenizer,
-): ...
 @overload
 def gradient_x_input(
     model: TFPreTrainedModel,
-    x_batch: list[str],
+    x_batch: List[str],
     y_batch: tf.Tensor,
     tokenizer: PreTrainedTokenizerBase,
 ) -> tf.Tensor: ...
 @overload
 def gradient_x_input(
     model: TFPreTrainedModel, x_batch: tf.Tensor, y_batch: tf.Tensor, **kwargs
 ) -> tf.Tensor: ...
+@overload
 def integrated_gradients(
     model: TFPreTrainedModel,
     x_batch: List[str],
     y_batch: tf.Tensor,
     tokenizer: PreTrainedTokenizerBase,
-    config: Optional[IntGradConfig] = None,
+    config: IntGradConfig | None = None,
 ) -> List[Explanation]: ...
 @overload
 def integrated_gradients(
     model: TFPreTrainedModel,
     x_batch: tf.Tensor,
     y_batch: tf.Tensor,
-    config: Optional[IntGradConfig] = None,
+    config: IntGradConfig | None = None,
     **kwargs,
 ) -> tf.Tensor: ...
+@overload
 def smooth_grad(
     model: TFPreTrainedModel,
     x_batch: List[str],
     y_batch: tf.Tensor,
     tokenizer: PreTrainedTokenizerBase,
-    config: Optional[SmoothGradConfing] = None,
+    config: SmoothGradConfing | None = None,
 ) -> List[Explanation]: ...
 @overload
 def smooth_grad(
     model: TFPreTrainedModel,
     x_batch: tf.Tensor,
     y_batch: tf.Tensor,
-    config: Optional[SmoothGradConfing] = None,
+    config: SmoothGradConfing | None = None,
     **kwargs,
 ) -> tf.Tensor: ...
+@overload
 def noise_grad(
     model: TFPreTrainedModel,
     x_batch: List[str],
     y_batch: tf.Tensor,
     tokenizer: PreTrainedTokenizerBase,
-    config: Optional[NoiseGradConfig] = None,
+    config: NoiseGradConfig | None = None,
 ) -> List[Explanation]: ...
 @overload
 def noise_grad(
     model: TFPreTrainedModel,
     x_batch: tf.Tensor,
     y_batch: tf.Tensor,
-    config: Optional[NoiseGradConfig] = None,
+    config: NoiseGradConfig | None = None,
     **kwargs,
 ) -> tf.Tensor: ...
+@overload
 def noise_grad_plus_plus(
     model: TFPreTrainedModel,
     x_batch: List[str],
     y_batch: tf.Tensor,
     tokenizer: PreTrainedTokenizerBase,
-    config: Optional[NoiseGradPlusPlusConfig] = None,
+    config: NoiseGradPlusPlusConfig | None = None,
 ) -> List[Explanation]: ...
 @overload
 def noise_grad_plus_plus(
     model: TFPreTrainedModel,
     x_batch: tf.Tensor,
     y_batch: tf.Tensor,
-    config: Optional[NoiseGradPlusPlusConfig] = None,
+    config: NoiseGradPlusPlusConfig | None = None,
     **kwargs,
 ) -> List[Explanation]: ...
```

### Comparing `transformers_gradients-0.0.2/src/transformers_gradients/types.py` & `transformers_gradients-0.0.4/src/transformers_gradients/types.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 from __future__ import annotations
 
-from typing import (
-    Callable,
-    Protocol,
-    overload,
-    runtime_checkable,
-)
+from typing import Callable, Protocol, overload, runtime_checkable, Tuple, List
 
 import tensorflow as tf
 from transformers import TFPreTrainedModel, PreTrainedTokenizerBase
 
 BaselineFn = Callable[[tf.Tensor], tf.Tensor]
-Explanation = tuple[list[str], tf.Tensor]
+Explanation = Tuple[List[str], tf.Tensor]
 ApplyNoiseFn = Callable[[tf.Tensor, tf.Tensor], tf.Tensor]
 
 
 @runtime_checkable
 class ExplainFn(Protocol):
     @overload
     def __call__(
@@ -29,25 +24,25 @@
     ) -> tf.Tensor:
         ...
 
     @overload
     def __call__(
         self,
         model: TFPreTrainedModel,
-        x_batch: list[str],
+        x_batch: List[str],
         y_batch: tf.Tensor,
         tokenizer: PreTrainedTokenizerBase,
         *args,
         **kwargs,
-    ) -> list[Explanation]:
+    ) -> List[Explanation]:
         ...
 
-    def __call__(
+    def __call__(  # type: ignore
         self,
         model: TFPreTrainedModel,
-        x_batch: list[str] | tf.Tensor,
+        x_batch: List[str] | tf.Tensor,
         y_batch: tf.Tensor,
         tokenizer: PreTrainedTokenizerBase | None,
         *args,
         **kwargs,
-    ) -> list[Explanation] | tf.Tensor:
+    ) -> List[Explanation] | tf.Tensor:
         ...
```

### Comparing `transformers_gradients-0.0.2/src/transformers_gradients/util.py` & `transformers_gradients-0.0.4/src/transformers_gradients/util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
 import platform
-from typing import TypeVar, Callable, Dict, NamedTuple
+from typing import TypeVar, Callable, Dict, List, Tuple
 
 import tensorflow as tf
+from cachetools import cached
 from transformers import PreTrainedTokenizerBase
 
 T = TypeVar("T")
-R = TypeVar("R")
 
 
 def get_input_ids(
-    tokenizer: PreTrainedTokenizerBase, x_batch: list[str]
-) -> tuple[tf.Tensor, dict[str, tf.Tensor]]:
+    tokenizer: PreTrainedTokenizerBase, x_batch: List[str]
+) -> Tuple[tf.Tensor, Dict[str, tf.Tensor]]:
     """Do batch encode, unpack input ids and other forward-pass kwargs."""
     encoded_input = tokenizer(x_batch, padding="longest", return_tensors="tf").data
     return encoded_input.pop("input_ids"), encoded_input
 
 
 def value_or_default(value: T | None, default_factory: Callable[[], T]) -> T:
     if value is not None:
@@ -26,25 +26,19 @@
 
 
 def is_xla_compatible_platform() -> bool:
     """Determine if host is xla-compatible."""
     return not (platform.system() == "Darwin" and "arm" in platform.processor().lower())
 
 
-@tf.function(reduce_retracing=True, jit_compile=is_xla_compatible_platform())
 def as_tensor(arr) -> tf.Tensor:
-    if isinstance(arr, (tf.Tensor, NamedTuple, Callable)):
+    if isinstance(arr, (tf.Tensor, Callable)):  # type: ignore
         return arr
     else:
         return tf.convert_to_tensor(arr)
 
 
-def map_dict(
-    dictionary: Dict[str, T],
-    value_mapper: Callable[[T], R],
-    key_mapper: Callable[[str], str] = lambda x: x,
-) -> Dict[str, R]:
-    """Applies func to values in dict. Additionally, if provided can also map keys."""
-    result = {}
-    for k, v in dictionary.items():
-        result[key_mapper(k)] = value_mapper(v)
-    return result
+@cached(key=lambda f: f.__name__, cache={})
+def cached_tf_function(func):
+    return tf.function(
+        func, reduce_retracing=True, jit_compile=is_xla_compatible_platform()
+    )
```

