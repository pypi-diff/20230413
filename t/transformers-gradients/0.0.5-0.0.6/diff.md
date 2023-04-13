# Comparing `tmp/transformers_gradients-0.0.5.tar.gz` & `tmp/transformers_gradients-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformers_gradients-0.0.5.tar", last modified: Thu Apr 13 10:07:10 2023, max compression
+gzip compressed data, was "transformers_gradients-0.0.6.tar", last modified: Thu Apr 13 18:05:24 2023, max compression
```

## Comparing `transformers_gradients-0.0.5.tar` & `transformers_gradients-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    48165 2023-04-13 10:07:02.676687 transformers_gradients-0.0.5/Readme.md
--rw-r--r--   0        0        0     4429 2023-04-13 10:07:02.676687 transformers_gradients-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      357 2023-04-13 10:07:02.676687 transformers_gradients-0.0.5/src/transformers_gradients/__init__.py
--rw-r--r--   0        0        0     5241 2023-04-13 10:07:02.676687 transformers_gradients-0.0.5/src/transformers_gradients/config.py
--rw-r--r--   0        0        0     7351 2023-04-13 10:07:02.676687 transformers_gradients-0.0.5/src/transformers_gradients/plotting.py
--rw-r--r--   0        0        0       64 2023-04-13 10:07:02.676687 transformers_gradients-0.0.5/src/transformers_gradients/py.typed
--rw-r--r--   0        0        0        0 2023-04-13 10:07:02.676687 transformers_gradients-0.0.5/src/transformers_gradients/text_classification/__init__.py
--rw-r--r--   0        0        0    18482 2023-04-13 10:07:02.676687 transformers_gradients-0.0.5/src/transformers_gradients/text_classification/explanation_func.py
--rw-r--r--   0        0        0     2610 2023-04-13 10:07:02.676687 transformers_gradients-0.0.5/src/transformers_gradients/text_classification/explanation_func.pyi
--rw-r--r--   0        0        0     1179 2023-04-13 10:07:02.676687 transformers_gradients-0.0.5/src/transformers_gradients/types.py
--rw-r--r--   0        0        0     1273 2023-04-13 10:07:02.676687 transformers_gradients-0.0.5/src/transformers_gradients/util.py
--rw-r--r--   0        0        0    49423 1970-01-01 00:00:00.000000 transformers_gradients-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    48165 2023-04-13 18:05:13.636379 transformers_gradients-0.0.6/Readme.md
+-rw-r--r--   0        0        0     4429 2023-04-13 18:05:13.636379 transformers_gradients-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      357 2023-04-13 18:05:13.640379 transformers_gradients-0.0.6/src/transformers_gradients/__init__.py
+-rw-r--r--   0        0        0     5241 2023-04-13 18:05:13.640379 transformers_gradients-0.0.6/src/transformers_gradients/config.py
+-rw-r--r--   0        0        0     7351 2023-04-13 18:05:13.640379 transformers_gradients-0.0.6/src/transformers_gradients/plotting.py
+-rw-r--r--   0        0        0       64 2023-04-13 18:05:13.640379 transformers_gradients-0.0.6/src/transformers_gradients/py.typed
+-rw-r--r--   0        0        0        0 2023-04-13 18:05:13.640379 transformers_gradients-0.0.6/src/transformers_gradients/text_classification/__init__.py
+-rw-r--r--   0        0        0    17328 2023-04-13 18:05:13.640379 transformers_gradients-0.0.6/src/transformers_gradients/text_classification/explanation_func.py
+-rw-r--r--   0        0        0     2610 2023-04-13 18:05:13.640379 transformers_gradients-0.0.6/src/transformers_gradients/text_classification/explanation_func.pyi
+-rw-r--r--   0        0        0     1179 2023-04-13 18:05:13.640379 transformers_gradients-0.0.6/src/transformers_gradients/types.py
+-rw-r--r--   0        0        0     1059 2023-04-13 18:05:13.640379 transformers_gradients-0.0.6/src/transformers_gradients/util.py
+-rw-r--r--   0        0        0    49423 1970-01-01 00:00:00.000000 transformers_gradients-0.0.6/PKG-INFO
```

### Comparing `transformers_gradients-0.0.5/Readme.md` & `transformers_gradients-0.0.6/Readme.md`

 * *Files identical despite different names*

### Comparing `transformers_gradients-0.0.5/pyproject.toml` & `transformers_gradients-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "transformers_gradients"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "0.0.5"  # Required
+version = "0.0.6"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Gradient-based XAI methods for TensorFlow transformers."  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `transformers_gradients-0.0.5/src/transformers_gradients/config.py` & `transformers_gradients-0.0.6/src/transformers_gradients/config.py`

 * *Files identical despite different names*

### Comparing `transformers_gradients-0.0.5/src/transformers_gradients/plotting.py` & `transformers_gradients-0.0.6/src/transformers_gradients/plotting.py`

 * *Files identical despite different names*

### Comparing `transformers_gradients-0.0.5/src/transformers_gradients/text_classification/explanation_func.py` & `transformers_gradients-0.0.6/src/transformers_gradients/text_classification/explanation_func.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     resolve_baseline_explain_fn,
 )
 from transformers_gradients.util import (
     value_or_default,
     is_xla_compatible_platform,
     get_input_ids,
     as_tensor,
-    cached_tf_function,
 )
 
 
 def plain_text_hook(func):
     @wraps(func)
     def wrapper(
         model: TFPreTrainedModel,
@@ -86,28 +85,21 @@
 
     Returns
     -------
     a_batch:
         List of tuples, where 1st element is tokens and 2nd is the scores assigned to the tokens.
 
     """
+    with tf.GradientTape() as tape:
+        tape.watch(x_batch)
+        logits = model(None, inputs_embeds=x_batch, training=False, **kwargs).logits
+        logits_for_label = logits_for_labels(logits, y_batch)
 
-    # @cached_tf_function
-    def grad_norm_fn(xx_batch, yy_batch, **kwargs):
-        with tf.GradientTape() as tape:
-            tape.watch(xx_batch)
-            logits = model(
-                None, inputs_embeds=xx_batch, training=False, **kwargs
-            ).logits
-            logits_for_label = logits_for_labels(logits, yy_batch)
-
-        grads = tape.gradient(logits_for_label, xx_batch)
-        return tf.linalg.norm(grads, axis=-1)
-
-    return grad_norm_fn(x_batch, y_batch, **tf.nest.map_structure(as_tensor, kwargs))
+    grads = tape.gradient(logits_for_label, x_batch)
+    return tf.linalg.norm(grads, axis=-1)
 
 
 @plain_text_hook
 def gradient_x_input(
     model: TFPreTrainedModel,
     x_batch: tf.Tensor,
     y_batch: tf.Tensor,
@@ -141,27 +133,20 @@
 
     Returns
     -------
     a_batch:
         List of tuples, where 1st element is tokens and 2nd is the scores assigned to the tokens.
 
     """
-
-    # @cached_tf_function
-    def grad_x_input_fn(xx_batch, yy_batch, **kwargs):
-        with tf.GradientTape() as tape:
-            tape.watch(xx_batch)
-            logits = model(
-                None, inputs_embeds=xx_batch, training=False, **kwargs
-            ).logits
-            logits_for_label = logits_for_labels(logits, yy_batch)
-        grads = tape.gradient(logits_for_label, xx_batch)
-        return tf.math.reduce_sum(xx_batch * grads, axis=-1)
-
-    return grad_x_input_fn(x_batch, y_batch, **tf.nest.map_structure(as_tensor, kwargs))
+    with tf.GradientTape() as tape:
+        tape.watch(x_batch)
+        logits = model(None, inputs_embeds=x_batch, training=False, **kwargs).logits
+        logits_for_label = logits_for_labels(logits, y_batch)
+    grads = tape.gradient(logits_for_label, x_batch)
+    return tf.math.reduce_sum(x_batch * grads, axis=-1)
 
 
 @plain_text_hook
 def integrated_gradients(
     model: TFPreTrainedModel,
     x_batch: tf.Tensor,
     y_batch: tf.Tensor,
@@ -210,15 +195,14 @@
     >>> unk_token_embedding = model.embedding_lookup([model.tokenizer.unk_token_id])[0, 0]
     >>> unknown_token_baseline_function = tf.function(lambda x: unk_token_embedding)
     >>> config = IntGradConfig(baseline_fn=unknown_token_baseline_function)
     >>> integrated_gradients(..., ..., ..., config=config)
 
     """
     config = value_or_default(config, lambda: IntGradConfig())
-    # tf.vectorized_map(
     interpolated_embeddings = tf.map_fn(
         lambda i: interpolate_inputs(
             config.baseline_fn(i), i, tf.constant(config.num_steps)
         ),
         x_batch,
     )
     kwargs = tf.nest.map_structure(as_tensor, kwargs)
@@ -247,46 +231,35 @@
     y_batch: tf.Tensor,
     config: SmoothGradConfing | None = None,
     **kwargs,
 ) -> tf.Tensor:
     config = value_or_default(config, lambda: SmoothGradConfing())
     explain_fn = resolve_baseline_explain_fn(config.explain_fn)
 
-    # @cached_tf_function
-    def smooth_grad_fn(xx_batch, yy_batch, n, mean, std, **kwargs):
-        explanations_array = tf.TensorArray(
-            xx_batch.dtype,
-            size=n,
-            clear_after_read=True,
-            colocate_with_first_write_call=True,
-        )
+    explanations_array = tf.TensorArray(
+        x_batch.dtype,
+        size=config.n,
+        clear_after_read=True,
+        colocate_with_first_write_call=True,
+    )
+
+    noise_dist = Normal(config.mean, config.std)
 
-        noise_dist = Normal(mean, std)
+    def noise_fn(x):
+        noise = noise_dist.sample(tf.shape(x))
+        return config.noise_fn(x, noise)
 
-        def noise_fn(x):
-            noise = noise_dist.sample(tf.shape(x))
-            return config.noise_fn(x, noise)
-
-        for n in tf.range(n):
-            noisy_x = noise_fn(xx_batch)
-            explanation = explain_fn(model, noisy_x, yy_batch, **kwargs)
-            explanations_array = explanations_array.write(n, explanation)
-
-        scores = tf.reduce_mean(explanations_array.stack(), axis=0)
-        explanations_array.close()
-        return scores
+    for n in tf.range(config.n):
+        noisy_x = noise_fn(x_batch)
+        explanation = explain_fn(model, noisy_x, y_batch, **kwargs)
+        explanations_array = explanations_array.write(n, explanation)
 
-    return smooth_grad_fn(
-        x_batch,
-        y_batch,
-        tf.constant(config.n),
-        tf.constant(config.mean),
-        tf.constant(config.std),
-        **tf.nest.map_structure(as_tensor, kwargs),
-    )
+    scores = tf.reduce_mean(explanations_array.stack(), axis=0)
+    explanations_array.close()
+    return scores
 
 
 @plain_text_hook
 def noise_grad(
     model: TFPreTrainedModel,
     x_batch: tf.Tensor,
     y_batch: tf.Tensor,
@@ -434,55 +407,49 @@
 def _integrated_gradients_batched(
     model: TFPreTrainedModel,
     x_batch: tf.Tensor,
     y_batch: tf.Tensor,
     num_steps: tf.Tensor,
     **kwargs,
 ) -> tf.Tensor:
-    # @cached_tf_function
-    def int_grad_fn(xx_batch, yy_batch, nnum_steps, **kwargs):
-        shape = tf.shape(xx_batch)
-        batch_size = shape[0]
-
-        interpolated_embeddings = tf.reshape(
-            tf.cast(xx_batch, dtype=tf.float32),
-            [-1, shape[2], shape[3]],
-        )
+    shape = tf.shape(x_batch)
+    batch_size = shape[0]
 
-        def pseudo_interpolate(x):
-            og_shape = tf.convert_to_tensor(tf.shape(x))
-            new_shape = tf.concat([[nnum_steps + 1], og_shape], axis=0)
-            x = tf.broadcast_to(x, new_shape)
-            flat_shape = tf.concat([tf.constant([-1]), og_shape[1:]], axis=0)
-            x = tf.reshape(x, flat_shape)
-            return x
-
-        interpolated_kwargs = tf.nest.map_structure(pseudo_interpolate, kwargs)
-        interpolated_y_batch = pseudo_interpolate(yy_batch)
-
-        with tf.GradientTape() as tape:
-            tape.watch(interpolated_embeddings)
-            logits = model(
-                None,
-                inputs_embeds=interpolated_embeddings,
-                training=False,
-                **interpolated_kwargs,
-            ).logits
-            logits_for_label = logits_for_labels(logits, interpolated_y_batch)
-
-        grads = tape.gradient(logits_for_label, interpolated_embeddings)
-        grads_shape = tf.shape(grads)
-        grads = tf.reshape(
-            grads, [batch_size, nnum_steps + 1, grads_shape[1], grads_shape[2]]
-        )
-        return tf.linalg.norm(tfp.math.trapz(grads, axis=1), axis=-1)
+    interpolated_embeddings = tf.reshape(
+        tf.cast(x_batch, dtype=tf.float32),
+        [-1, shape[2], shape[3]],
+    )
 
-    return int_grad_fn(
-        x_batch, y_batch, num_steps, **tf.nest.map_structure(as_tensor, kwargs)
+    def pseudo_interpolate(x):
+        og_shape = tf.convert_to_tensor(tf.shape(x))
+        new_shape = tf.concat([[num_steps + 1], og_shape], axis=0)
+        x = tf.broadcast_to(x, new_shape)
+        flat_shape = tf.concat([tf.constant([-1]), og_shape[1:]], axis=0)
+        x = tf.reshape(x, flat_shape)
+        return x
+
+    interpolated_kwargs = tf.nest.map_structure(pseudo_interpolate, kwargs)
+    interpolated_y_batch = pseudo_interpolate(y_batch)
+
+    with tf.GradientTape() as tape:
+        tape.watch(interpolated_embeddings)
+        logits = model(
+            None,
+            inputs_embeds=interpolated_embeddings,
+            training=False,
+            **interpolated_kwargs,
+        ).logits
+        logits_for_label = logits_for_labels(logits, interpolated_y_batch)
+
+    grads = tape.gradient(logits_for_label, interpolated_embeddings)
+    grads_shape = tf.shape(grads)
+    grads = tf.reshape(
+        grads, [batch_size, num_steps + 1, grads_shape[1], grads_shape[2]]
     )
+    return tf.linalg.norm(tfp.math.trapz(grads, axis=1), axis=-1)
 
 
 def _integrated_gradients_iterative(
     model: TFPreTrainedModel,
     x_batch: tf.Tensor,
     y_batch: tf.Tensor,
     **kwargs,
@@ -492,15 +459,16 @@
         x_batch.dtype,
         size=batch_size,
         clear_after_read=True,
         colocate_with_first_write_call=True,
     )
 
     def pseudo_interpolate(x, embeds):
-        return tf.broadcast_to(x, (tf.shape(embeds)[0], *x.shape))
+        x_shape = tf.shape(x)
+        return tf.broadcast_to(x, (tf.shape(embeds)[0], *x_shape))
 
     for i in tf.range(batch_size):
         interpolated_embeddings = x_batch[i]
 
         kwargs_i = tf.nest.map_structure(itemgetter(i), kwargs)
 
         interpolated_kwargs = tf.nest.map_structure(
```

### Comparing `transformers_gradients-0.0.5/src/transformers_gradients/text_classification/explanation_func.pyi` & `transformers_gradients-0.0.6/src/transformers_gradients/text_classification/explanation_func.pyi`

 * *Files identical despite different names*

### Comparing `transformers_gradients-0.0.5/src/transformers_gradients/types.py` & `transformers_gradients-0.0.6/src/transformers_gradients/types.py`

 * *Files identical despite different names*

### Comparing `transformers_gradients-0.0.5/src/transformers_gradients/util.py` & `transformers_gradients-0.0.6/src/transformers_gradients/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 import platform
 from typing import TypeVar, Callable, Dict, List, Tuple
 
 import tensorflow as tf
-from cachetools import cached
 from transformers import PreTrainedTokenizerBase
 
 T = TypeVar("T")
 
 
 def get_input_ids(
     tokenizer: PreTrainedTokenizerBase, x_batch: List[str]
@@ -31,14 +30,7 @@
 
 
 def as_tensor(arr) -> tf.Tensor:
     if isinstance(arr, (tf.Tensor, Callable)):  # type: ignore
         return arr
     else:
         return tf.convert_to_tensor(arr)
-
-
-@cached(key=lambda f: f.__name__, cache={})
-def cached_tf_function(func):
-    return tf.function(
-        func, reduce_retracing=True, jit_compile=is_xla_compatible_platform()
-    )
```

### Comparing `transformers_gradients-0.0.5/PKG-INFO` & `transformers_gradients-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformers_gradients
-Version: 0.0.5
+Version: 0.0.6
 Summary: Gradient-based XAI methods for TensorFlow transformers.
 Keywords: explainable ai,xai,machine learning,deep learning
 Author-email: Artem Sereda <artem.sereda@campus.tu-berlin.de>
 Maintainer-email: Artem Sereda <artem.sereda@campus.tu-berlin.de>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: transformers_gradients Version: 0.0.5 Summary:
+Metadata-Version: 2.1 Name: transformers_gradients Version: 0.0.6 Summary:
 Gradient-based XAI methods for TensorFlow transformers. Keywords: explainable
 ai,xai,machine learning,deep learning Author-email: Artem Sereda
 sereda@campus.tu-berlin.de> Maintainer-email: Artem Sereda
 sereda@campus.tu-berlin.de> Requires-Python: >=3.8 Description-Content-Type:
 text/markdown Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Education Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
```

