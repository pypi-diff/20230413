# Comparing `tmp/transformers_gradients-0.0.4.tar.gz` & `tmp/transformers_gradients-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformers_gradients-0.0.4.tar", last modified: Thu Apr 13 08:05:24 2023, max compression
+gzip compressed data, was "transformers_gradients-0.0.5.tar", last modified: Thu Apr 13 10:07:10 2023, max compression
```

## Comparing `transformers_gradients-0.0.4.tar` & `transformers_gradients-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    48301 2023-04-13 08:05:16.689063 transformers_gradients-0.0.4/Readme.md
--rw-r--r--   0        0        0     4429 2023-04-13 08:05:16.689063 transformers_gradients-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      357 2023-04-13 08:05:16.689063 transformers_gradients-0.0.4/src/transformers_gradients/__init__.py
--rw-r--r--   0        0        0     5241 2023-04-13 08:05:16.689063 transformers_gradients-0.0.4/src/transformers_gradients/config.py
--rw-r--r--   0        0        0     7351 2023-04-13 08:05:16.689063 transformers_gradients-0.0.4/src/transformers_gradients/plotting.py
--rw-r--r--   0        0        0       64 2023-04-13 08:05:16.689063 transformers_gradients-0.0.4/src/transformers_gradients/py.typed
--rw-r--r--   0        0        0        0 2023-04-13 08:05:16.689063 transformers_gradients-0.0.4/src/transformers_gradients/text_classification/__init__.py
--rw-r--r--   0        0        0    18474 2023-04-13 08:05:16.689063 transformers_gradients-0.0.4/src/transformers_gradients/text_classification/explanation_func.py
--rw-r--r--   0        0        0     2610 2023-04-13 08:05:16.689063 transformers_gradients-0.0.4/src/transformers_gradients/text_classification/explanation_func.pyi
--rw-r--r--   0        0        0     1179 2023-04-13 08:05:16.689063 transformers_gradients-0.0.4/src/transformers_gradients/types.py
--rw-r--r--   0        0        0     1273 2023-04-13 08:05:16.689063 transformers_gradients-0.0.4/src/transformers_gradients/util.py
--rw-r--r--   0        0        0    49559 1970-01-01 00:00:00.000000 transformers_gradients-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    48165 2023-04-13 10:07:02.676687 transformers_gradients-0.0.5/Readme.md
+-rw-r--r--   0        0        0     4429 2023-04-13 10:07:02.676687 transformers_gradients-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      357 2023-04-13 10:07:02.676687 transformers_gradients-0.0.5/src/transformers_gradients/__init__.py
+-rw-r--r--   0        0        0     5241 2023-04-13 10:07:02.676687 transformers_gradients-0.0.5/src/transformers_gradients/config.py
+-rw-r--r--   0        0        0     7351 2023-04-13 10:07:02.676687 transformers_gradients-0.0.5/src/transformers_gradients/plotting.py
+-rw-r--r--   0        0        0       64 2023-04-13 10:07:02.676687 transformers_gradients-0.0.5/src/transformers_gradients/py.typed
+-rw-r--r--   0        0        0        0 2023-04-13 10:07:02.676687 transformers_gradients-0.0.5/src/transformers_gradients/text_classification/__init__.py
+-rw-r--r--   0        0        0    18482 2023-04-13 10:07:02.676687 transformers_gradients-0.0.5/src/transformers_gradients/text_classification/explanation_func.py
+-rw-r--r--   0        0        0     2610 2023-04-13 10:07:02.676687 transformers_gradients-0.0.5/src/transformers_gradients/text_classification/explanation_func.pyi
+-rw-r--r--   0        0        0     1179 2023-04-13 10:07:02.676687 transformers_gradients-0.0.5/src/transformers_gradients/types.py
+-rw-r--r--   0        0        0     1273 2023-04-13 10:07:02.676687 transformers_gradients-0.0.5/src/transformers_gradients/util.py
+-rw-r--r--   0        0        0    49423 1970-01-01 00:00:00.000000 transformers_gradients-0.0.5/PKG-INFO
```

### Comparing `transformers_gradients-0.0.4/Readme.md` & `transformers_gradients-0.0.5/Readme.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,46 +2,46 @@
 
 like GradientXInput, pun intended.
 
 Collection of gradient-based XAI methods for TensorFlow models from HuggingFace Hub.
 
 Work in Progress!!!
 
-<div>
-    <style>
-        .container {
-            line-height: 1.4;
-            text-align: center;
-            margin: 10px 10px 10px 10px;
-            color: black;
-            background: white;
-        }
-        p {
-            font-size: 16px;
-        }
-        .highlight-container, .highlight {
-            position: relative;
-            border-radius: 10% 10% 10% 10%;
-        }
-        .highlight-container {
-            display: inline-block;
-        }
-        .highlight-container:before {
-            content: " ";
-            display: block;
-            height: 90%;
-            width: 100%;
-            margin-left: -3px;
-            margin-right: -3px;
-            position: absolute;
-            top: -1px;
-            left: -1px;
-            padding: 10px 3px 3px 10px;
-        }
-    </style>
+
+<style>
+    .container {
+        line-height: 1.4;
+        text-align: center;
+        margin: 10px 10px 10px 10px;
+        color: black;
+        background: white;
+    }
+    p {
+        font-size: 16px;
+    }
+    .highlight-container, .highlight {
+        position: relative;
+        border-radius: 10% 10% 10% 10%;
+    }
+    .highlight-container {
+        display: inline-block;
+    }
+    .highlight-container:before {
+        content: " ";
+        display: block;
+        height: 90%;
+        width: 100%;
+        margin-left: -3px;
+        margin-right: -3px;
+        position: absolute;
+        top: -1px;
+        left: -1px;
+        padding: 10px 3px 3px 10px;
+    }
+</style>
 <div class="container">
     <p> Gradient Norm <br>
         <span class="highlight-container" style="background:rgb(255.0,0.0,0.0);">
             <span class="highlight"> [CLS] </span>
         </span>
         <span class="highlight-container" style="background:rgb(255.0,190.44862365722656,190.44862365722656);">
             <span class="highlight"> like </span>
@@ -896,8 +896,7 @@
             <span class="highlight"> ##graphy </span>
         </span>
         <span class="highlight-container" style="background:rgb(255.0,0.0,0.0);">
             <span class="highlight"> [SEP] </span>
         </span>
     </p>
 </div>
-</div>
```

### Comparing `transformers_gradients-0.0.4/pyproject.toml` & `transformers_gradients-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "transformers_gradients"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "0.0.4"  # Required
+version = "0.0.5"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Gradient-based XAI methods for TensorFlow transformers."  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `transformers_gradients-0.0.4/src/transformers_gradients/config.py` & `transformers_gradients-0.0.5/src/transformers_gradients/config.py`

 * *Files identical despite different names*

### Comparing `transformers_gradients-0.0.4/src/transformers_gradients/plotting.py` & `transformers_gradients-0.0.5/src/transformers_gradients/plotting.py`

 * *Files identical despite different names*

### Comparing `transformers_gradients-0.0.4/src/transformers_gradients/text_classification/explanation_func.py` & `transformers_gradients-0.0.5/src/transformers_gradients/text_classification/explanation_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     Returns
     -------
     a_batch:
         List of tuples, where 1st element is tokens and 2nd is the scores assigned to the tokens.
 
     """
 
-    @cached_tf_function
+    # @cached_tf_function
     def grad_norm_fn(xx_batch, yy_batch, **kwargs):
         with tf.GradientTape() as tape:
             tape.watch(xx_batch)
             logits = model(
                 None, inputs_embeds=xx_batch, training=False, **kwargs
             ).logits
             logits_for_label = logits_for_labels(logits, yy_batch)
@@ -142,15 +142,15 @@
     Returns
     -------
     a_batch:
         List of tuples, where 1st element is tokens and 2nd is the scores assigned to the tokens.
 
     """
 
-    @cached_tf_function
+    # @cached_tf_function
     def grad_x_input_fn(xx_batch, yy_batch, **kwargs):
         with tf.GradientTape() as tape:
             tape.watch(xx_batch)
             logits = model(
                 None, inputs_embeds=xx_batch, training=False, **kwargs
             ).logits
             logits_for_label = logits_for_labels(logits, yy_batch)
@@ -247,15 +247,15 @@
     y_batch: tf.Tensor,
     config: SmoothGradConfing | None = None,
     **kwargs,
 ) -> tf.Tensor:
     config = value_or_default(config, lambda: SmoothGradConfing())
     explain_fn = resolve_baseline_explain_fn(config.explain_fn)
 
-    @cached_tf_function
+    # @cached_tf_function
     def smooth_grad_fn(xx_batch, yy_batch, n, mean, std, **kwargs):
         explanations_array = tf.TensorArray(
             xx_batch.dtype,
             size=n,
             clear_after_read=True,
             colocate_with_first_write_call=True,
         )
@@ -434,15 +434,15 @@
 def _integrated_gradients_batched(
     model: TFPreTrainedModel,
     x_batch: tf.Tensor,
     y_batch: tf.Tensor,
     num_steps: tf.Tensor,
     **kwargs,
 ) -> tf.Tensor:
-    @cached_tf_function
+    # @cached_tf_function
     def int_grad_fn(xx_batch, yy_batch, nnum_steps, **kwargs):
         shape = tf.shape(xx_batch)
         batch_size = shape[0]
 
         interpolated_embeddings = tf.reshape(
             tf.cast(xx_batch, dtype=tf.float32),
             [-1, shape[2], shape[3]],
```

### Comparing `transformers_gradients-0.0.4/src/transformers_gradients/text_classification/explanation_func.pyi` & `transformers_gradients-0.0.5/src/transformers_gradients/text_classification/explanation_func.pyi`

 * *Files identical despite different names*

### Comparing `transformers_gradients-0.0.4/src/transformers_gradients/types.py` & `transformers_gradients-0.0.5/src/transformers_gradients/types.py`

 * *Files identical despite different names*

### Comparing `transformers_gradients-0.0.4/src/transformers_gradients/util.py` & `transformers_gradients-0.0.5/src/transformers_gradients/util.py`

 * *Files identical despite different names*

### Comparing `transformers_gradients-0.0.4/PKG-INFO` & `transformers_gradients-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformers_gradients
-Version: 0.0.4
+Version: 0.0.5
 Summary: Gradient-based XAI methods for TensorFlow transformers.
 Keywords: explainable ai,xai,machine learning,deep learning
 Author-email: Artem Sereda <artem.sereda@campus.tu-berlin.de>
 Maintainer-email: Artem Sereda <artem.sereda@campus.tu-berlin.de>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
@@ -30,46 +30,46 @@
 
 like GradientXInput, pun intended.
 
 Collection of gradient-based XAI methods for TensorFlow models from HuggingFace Hub.
 
 Work in Progress!!!
 
-<div>
-    <style>
-        .container {
-            line-height: 1.4;
-            text-align: center;
-            margin: 10px 10px 10px 10px;
-            color: black;
-            background: white;
-        }
-        p {
-            font-size: 16px;
-        }
-        .highlight-container, .highlight {
-            position: relative;
-            border-radius: 10% 10% 10% 10%;
-        }
-        .highlight-container {
-            display: inline-block;
-        }
-        .highlight-container:before {
-            content: " ";
-            display: block;
-            height: 90%;
-            width: 100%;
-            margin-left: -3px;
-            margin-right: -3px;
-            position: absolute;
-            top: -1px;
-            left: -1px;
-            padding: 10px 3px 3px 10px;
-        }
-    </style>
+
+<style>
+    .container {
+        line-height: 1.4;
+        text-align: center;
+        margin: 10px 10px 10px 10px;
+        color: black;
+        background: white;
+    }
+    p {
+        font-size: 16px;
+    }
+    .highlight-container, .highlight {
+        position: relative;
+        border-radius: 10% 10% 10% 10%;
+    }
+    .highlight-container {
+        display: inline-block;
+    }
+    .highlight-container:before {
+        content: " ";
+        display: block;
+        height: 90%;
+        width: 100%;
+        margin-left: -3px;
+        margin-right: -3px;
+        position: absolute;
+        top: -1px;
+        left: -1px;
+        padding: 10px 3px 3px 10px;
+    }
+</style>
 <div class="container">
     <p> Gradient Norm <br>
         <span class="highlight-container" style="background:rgb(255.0,0.0,0.0);">
             <span class="highlight"> [CLS] </span>
         </span>
         <span class="highlight-container" style="background:rgb(255.0,190.44862365722656,190.44862365722656);">
             <span class="highlight"> like </span>
@@ -924,9 +924,8 @@
             <span class="highlight"> ##graphy </span>
         </span>
         <span class="highlight-container" style="background:rgb(255.0,0.0,0.0);">
             <span class="highlight"> [SEP] </span>
         </span>
     </p>
 </div>
-</div>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: transformers_gradients Version: 0.0.4 Summary:
+Metadata-Version: 2.1 Name: transformers_gradients Version: 0.0.5 Summary:
 Gradient-based XAI methods for TensorFlow transformers. Keywords: explainable
 ai,xai,machine learning,deep learning Author-email: Artem Sereda
 sereda@campus.tu-berlin.de> Maintainer-email: Artem Sereda
 sereda@campus.tu-berlin.de> Requires-Python: >=3.8 Description-Content-Type:
 text/markdown Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Education Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
```

