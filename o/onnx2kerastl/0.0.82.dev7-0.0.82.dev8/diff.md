# Comparing `tmp/onnx2kerastl-0.0.82.dev7.tar.gz` & `tmp/onnx2kerastl-0.0.82.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx2kerastl-0.0.82.dev7.tar", max compression
+gzip compressed data, was "onnx2kerastl-0.0.82.dev8.tar", max compression
```

## Comparing `onnx2kerastl-0.0.82.dev7.tar` & `onnx2kerastl-0.0.82.dev8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1067 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev7/LICENSE
--rw-r--r--   0        0        0       66 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev7/onnx2kerastl/__init__.py
--rw-r--r--   0        0        0     8121 2023-04-03 08:32:59.779031 onnx2kerastl-0.0.82.dev7/onnx2kerastl/activation_layers.py
--rw-r--r--   0        0        0     1127 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev7/onnx2kerastl/caffe2_layers.py
--rw-r--r--   0        0        0      780 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev7/onnx2kerastl/constant_layers.py
--rw-r--r--   0        0        0    13188 2023-04-03 08:32:59.779031 onnx2kerastl-0.0.82.dev7/onnx2kerastl/converter.py
--rw-r--r--   0        0        0    11246 2023-04-03 08:32:59.779031 onnx2kerastl-0.0.82.dev7/onnx2kerastl/convolution_layers.py
--rw-r--r--   0        0        0      584 2023-04-04 08:56:02.330516 onnx2kerastl-0.0.82.dev7/onnx2kerastl/customonnxlayer/__init__.py
--rw-r--r--   0        0        0      236 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev7/onnx2kerastl/customonnxlayer/onnxabs.py
--rw-r--r--   0        0        0      236 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev7/onnx2kerastl/customonnxlayer/onnxerf.py
--rw-r--r--   0        0        0      606 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev7/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py
--rw-r--r--   0        0        0     1472 2023-04-10 08:16:31.705202 onnx2kerastl-0.0.82.dev7/onnx2kerastl/customonnxlayer/onnxlstm.py
--rw-r--r--   0        0        0      605 2022-09-29 08:59:30.260148 onnx2kerastl-0.0.82.dev7/onnx2kerastl/customonnxlayer/onnxreducemean.py
--rw-r--r--   0        0        0      238 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev7/onnx2kerastl/customonnxlayer/onnxsqrt.py
--rw-r--r--   0        0        0     9300 2023-04-03 08:32:59.783031 onnx2kerastl-0.0.82.dev7/onnx2kerastl/elementwise_layers.py
--rw-r--r--   0        0        0      179 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev7/onnx2kerastl/exceptions.py
--rw-r--r--   0        0        0     3693 2023-04-03 08:32:59.783031 onnx2kerastl-0.0.82.dev7/onnx2kerastl/layers.py
--rw-r--r--   0        0        0     2301 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev7/onnx2kerastl/linear_layers.py
--rw-r--r--   0        0        0     3779 2023-04-10 08:16:31.709202 onnx2kerastl-0.0.82.dev7/onnx2kerastl/ltsm_layers.py
--rw-r--r--   0        0        0      368 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev7/onnx2kerastl/main.py
--rw-r--r--   0        0        0     5328 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev7/onnx2kerastl/normalization_layers.py
--rw-r--r--   0        0        0    15397 2023-04-03 08:32:59.783031 onnx2kerastl-0.0.82.dev7/onnx2kerastl/operation_layers.py
--rw-r--r--   0        0        0     2940 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev7/onnx2kerastl/padding_layers.py
--rw-r--r--   0        0        0     7464 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev7/onnx2kerastl/pooling_layers.py
--rw-r--r--   0        0        0    17567 2023-04-10 08:16:31.709202 onnx2kerastl-0.0.82.dev7/onnx2kerastl/reshape_layers.py
--rw-r--r--   0        0        0     1655 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev7/onnx2kerastl/upsampling_layers.py
--rw-r--r--   0        0        0     4415 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev7/onnx2kerastl/utils.py
--rw-r--r--   0        0        0     1035 2023-04-10 08:17:15.892249 onnx2kerastl-0.0.82.dev7/pyproject.toml
--rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 onnx2kerastl-0.0.82.dev7/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev8/LICENSE
+-rw-r--r--   0        0        0       66 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev8/onnx2kerastl/__init__.py
+-rw-r--r--   0        0        0     8121 2023-04-03 08:32:59.779031 onnx2kerastl-0.0.82.dev8/onnx2kerastl/activation_layers.py
+-rw-r--r--   0        0        0     1127 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev8/onnx2kerastl/caffe2_layers.py
+-rw-r--r--   0        0        0      780 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev8/onnx2kerastl/constant_layers.py
+-rw-r--r--   0        0        0    13188 2023-04-03 08:32:59.779031 onnx2kerastl-0.0.82.dev8/onnx2kerastl/converter.py
+-rw-r--r--   0        0        0    11246 2023-04-03 08:32:59.779031 onnx2kerastl-0.0.82.dev8/onnx2kerastl/convolution_layers.py
+-rw-r--r--   0        0        0      584 2023-04-04 08:56:02.330516 onnx2kerastl-0.0.82.dev8/onnx2kerastl/customonnxlayer/__init__.py
+-rw-r--r--   0        0        0      236 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev8/onnx2kerastl/customonnxlayer/onnxabs.py
+-rw-r--r--   0        0        0      236 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev8/onnx2kerastl/customonnxlayer/onnxerf.py
+-rw-r--r--   0        0        0      606 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev8/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py
+-rw-r--r--   0        0        0     1730 2023-04-13 13:17:22.638560 onnx2kerastl-0.0.82.dev8/onnx2kerastl/customonnxlayer/onnxlstm.py
+-rw-r--r--   0        0        0      605 2022-09-29 08:59:30.260148 onnx2kerastl-0.0.82.dev8/onnx2kerastl/customonnxlayer/onnxreducemean.py
+-rw-r--r--   0        0        0      238 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev8/onnx2kerastl/customonnxlayer/onnxsqrt.py
+-rw-r--r--   0        0        0     9300 2023-04-03 08:32:59.783031 onnx2kerastl-0.0.82.dev8/onnx2kerastl/elementwise_layers.py
+-rw-r--r--   0        0        0      179 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev8/onnx2kerastl/exceptions.py
+-rw-r--r--   0        0        0     3693 2023-04-03 08:32:59.783031 onnx2kerastl-0.0.82.dev8/onnx2kerastl/layers.py
+-rw-r--r--   0        0        0     2301 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev8/onnx2kerastl/linear_layers.py
+-rw-r--r--   0        0        0     3791 2023-04-13 13:17:22.654560 onnx2kerastl-0.0.82.dev8/onnx2kerastl/ltsm_layers.py
+-rw-r--r--   0        0        0      368 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.82.dev8/onnx2kerastl/main.py
+-rw-r--r--   0        0        0     5328 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev8/onnx2kerastl/normalization_layers.py
+-rw-r--r--   0        0        0    15397 2023-04-03 08:32:59.783031 onnx2kerastl-0.0.82.dev8/onnx2kerastl/operation_layers.py
+-rw-r--r--   0        0        0     2940 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev8/onnx2kerastl/padding_layers.py
+-rw-r--r--   0        0        0     7464 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev8/onnx2kerastl/pooling_layers.py
+-rw-r--r--   0        0        0    17567 2023-04-13 13:17:22.642560 onnx2kerastl-0.0.82.dev8/onnx2kerastl/reshape_layers.py
+-rw-r--r--   0        0        0     1655 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev8/onnx2kerastl/upsampling_layers.py
+-rw-r--r--   0        0        0     4415 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.82.dev8/onnx2kerastl/utils.py
+-rw-r--r--   0        0        0     1035 2023-04-13 13:23:53.671617 onnx2kerastl-0.0.82.dev8/pyproject.toml
+-rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 onnx2kerastl-0.0.82.dev8/PKG-INFO
```

### Comparing `onnx2kerastl-0.0.82.dev7/LICENSE` & `onnx2kerastl-0.0.82.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev7/onnx2kerastl/activation_layers.py` & `onnx2kerastl-0.0.82.dev8/onnx2kerastl/activation_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev7/onnx2kerastl/caffe2_layers.py` & `onnx2kerastl-0.0.82.dev8/onnx2kerastl/caffe2_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev7/onnx2kerastl/constant_layers.py` & `onnx2kerastl-0.0.82.dev8/onnx2kerastl/constant_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev7/onnx2kerastl/converter.py` & `onnx2kerastl-0.0.82.dev8/onnx2kerastl/converter.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev7/onnx2kerastl/convolution_layers.py` & `onnx2kerastl-0.0.82.dev8/onnx2kerastl/convolution_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev7/onnx2kerastl/customonnxlayer/__init__.py` & `onnx2kerastl-0.0.82.dev8/onnx2kerastl/customonnxlayer/__init__.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev7/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py` & `onnx2kerastl-0.0.82.dev8/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev7/onnx2kerastl/customonnxlayer/onnxlstm.py` & `onnx2kerastl-0.0.82.dev8/onnx2kerastl/customonnxlayer/onnxlstm.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,16 +16,20 @@
         super().__init__(**kwargs)
         self.lstm_layer = tf.keras.layers.LSTM(units, return_sequences=return_sequences,
                                                return_state=return_lstm_state)
         self.return_lstm_state = return_lstm_state
         self.return_sequences = return_sequences
         self.units = units
 
-    def call(self, inputs, **kwargs):
-        res = self.lstm_layer(inputs, **kwargs)
+    def call(self, inputs, initial_h_state=None, initial_c_state=None, **kwargs):
+        if initial_h_state is not None and initial_c_state is not None:
+            initial_states = [initial_h_state, initial_c_state]
+        else:
+            initial_states = None
+        res = self.lstm_layer(inputs, initial_state=initial_states, **kwargs)
         if self.return_lstm_state:
             lstm_tensor, h_out, c_out = res
             lstm_flat = tf.keras.layers.Flatten()(lstm_tensor)
             h_flat = tf.keras.layers.Flatten()(h_out)
             c_flat = tf.keras.layers.Flatten()(c_out)
             concat_output = tf.keras.layers.Concatenate()([lstm_flat, h_flat, c_flat])
             return concat_output
```

### Comparing `onnx2kerastl-0.0.82.dev7/onnx2kerastl/customonnxlayer/onnxreducemean.py` & `onnx2kerastl-0.0.82.dev8/onnx2kerastl/customonnxlayer/onnxreducemean.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev7/onnx2kerastl/elementwise_layers.py` & `onnx2kerastl-0.0.82.dev8/onnx2kerastl/elementwise_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev7/onnx2kerastl/layers.py` & `onnx2kerastl-0.0.82.dev8/onnx2kerastl/layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev7/onnx2kerastl/linear_layers.py` & `onnx2kerastl-0.0.82.dev8/onnx2kerastl/linear_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev7/onnx2kerastl/ltsm_layers.py` & `onnx2kerastl-0.0.82.dev8/onnx2kerastl/ltsm_layers.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,16 @@
     weights_b = ensure_numpy_type(layers[node.input[3]])[0]
 
     initial_h_state = tf.cast(tf.squeeze(ensure_tf_type(layers[node.input[5]]), axis=1), input_tensor.dtype)
     initial_c_state = tf.cast(tf.squeeze(ensure_tf_type(layers[node.input[6]]), axis=1), input_tensor.dtype)
 
     tf.keras.backend.set_image_data_format("channels_last")
     hidden_size = params['hidden_size']
-    res = OnnxLSTM(hidden_size, return_sequences=True, return_lstm_state=should_return_state)(input_tensor, initial_state=[initial_h_state, initial_c_state])
+    lstm_layer = OnnxLSTM(hidden_size, return_sequences=True, return_lstm_state=should_return_state)
+    res = lstm_layer(input_tensor, initial_h_state, initial_c_state)
     # prepare the keras lstm weights from the onnx inputs:
     w1 = np.concatenate([weights_w[0:hidden_size, :], weights_w[2 * hidden_size:3 * hidden_size, :],
                          weights_w[3 * hidden_size:4 * hidden_size, :],
                          weights_w[hidden_size:2 * hidden_size, :]]).transpose()
     w2 = np.concatenate([weights_r[0:hidden_size, :], weights_r[2 * hidden_size:3 * hidden_size, :],
                          weights_r[3 * hidden_size:4 * hidden_size, :],
                          weights_r[hidden_size:2 * hidden_size, :]]).transpose()
```

### Comparing `onnx2kerastl-0.0.82.dev7/onnx2kerastl/normalization_layers.py` & `onnx2kerastl-0.0.82.dev8/onnx2kerastl/normalization_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev7/onnx2kerastl/operation_layers.py` & `onnx2kerastl-0.0.82.dev8/onnx2kerastl/operation_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev7/onnx2kerastl/padding_layers.py` & `onnx2kerastl-0.0.82.dev8/onnx2kerastl/padding_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev7/onnx2kerastl/pooling_layers.py` & `onnx2kerastl-0.0.82.dev8/onnx2kerastl/pooling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev7/onnx2kerastl/reshape_layers.py` & `onnx2kerastl-0.0.82.dev8/onnx2kerastl/reshape_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev7/onnx2kerastl/upsampling_layers.py` & `onnx2kerastl-0.0.82.dev8/onnx2kerastl/upsampling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev7/onnx2kerastl/utils.py` & `onnx2kerastl-0.0.82.dev8/onnx2kerastl/utils.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.82.dev7/pyproject.toml` & `onnx2kerastl-0.0.82.dev8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "onnx2kerastl"
-version = "0.0.82.dev7"
+version = "0.0.82.dev8"
 description = ""
 authors = ["dorhar <doron.harnoy@tensorleap.ai>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 tensorflow = {version = "2.11.0", markers = "platform_machine  == 'x86_64'"}
```

### Comparing `onnx2kerastl-0.0.82.dev7/PKG-INFO` & `onnx2kerastl-0.0.82.dev8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx2kerastl
-Version: 0.0.82.dev7
+Version: 0.0.82.dev8
 Summary: 
 License: MIT
 Author: dorhar
 Author-email: doron.harnoy@tensorleap.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

