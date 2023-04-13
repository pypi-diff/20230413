# Comparing `tmp/arcaflow_plugin_sdk-0.8.0.tar.gz` & `tmp/arcaflow_plugin_sdk-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcaflow_plugin_sdk-0.8.0.tar", last modified: Mon Oct 17 15:10:44 2022, max compression
+gzip compressed data, was "arcaflow_plugin_sdk-0.9.0.tar", last modified: Tue Oct 18 11:24:39 2022, max compression
```

## Comparing `arcaflow_plugin_sdk-0.8.0.tar` & `arcaflow_plugin_sdk-0.9.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 15:10:44.873569 arcaflow_plugin_sdk-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)    10174 2022-10-17 15:08:22.000000 arcaflow_plugin_sdk-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3269 2022-10-17 15:10:44.873569 arcaflow_plugin_sdk-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2738 2022-10-17 15:08:22.000000 arcaflow_plugin_sdk-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      750 2022-10-17 15:10:32.000000 arcaflow_plugin_sdk-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-10-17 15:10:44.873569 arcaflow_plugin_sdk-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 15:10:44.861568 arcaflow_plugin_sdk-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 15:10:44.869568 arcaflow_plugin_sdk-0.8.0/src/arcaflow_plugin_sdk/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 15:08:22.000000 arcaflow_plugin_sdk-0.8.0/src/arcaflow_plugin_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6152 2022-10-17 15:08:22.000000 arcaflow_plugin_sdk-0.8.0/src/arcaflow_plugin_sdk/_http.py
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-10-17 15:08:22.000000 arcaflow_plugin_sdk-0.8.0/src/arcaflow_plugin_sdk/annotations.py
--rw-r--r--   0 runner    (1001) docker     (121)     5051 2022-10-17 15:08:22.000000 arcaflow_plugin_sdk-0.8.0/src/arcaflow_plugin_sdk/atp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1398 2022-10-17 15:08:22.000000 arcaflow_plugin_sdk-0.8.0/src/arcaflow_plugin_sdk/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (121)    12542 2022-10-17 15:08:22.000000 arcaflow_plugin_sdk-0.8.0/src/arcaflow_plugin_sdk/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)   202072 2022-10-17 15:08:22.000000 arcaflow_plugin_sdk-0.8.0/src/arcaflow_plugin_sdk/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     2104 2022-10-17 15:08:22.000000 arcaflow_plugin_sdk-0.8.0/src/arcaflow_plugin_sdk/serialization.py
--rw-r--r--   0 runner    (1001) docker     (121)     3024 2022-10-17 15:08:22.000000 arcaflow_plugin_sdk-0.8.0/src/arcaflow_plugin_sdk/test_atp.py
--rw-r--r--   0 runner    (1001) docker     (121)     6163 2022-10-17 15:08:22.000000 arcaflow_plugin_sdk-0.8.0/src/arcaflow_plugin_sdk/test_jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-10-17 15:08:22.000000 arcaflow_plugin_sdk-0.8.0/src/arcaflow_plugin_sdk/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)    48796 2022-10-17 15:08:22.000000 arcaflow_plugin_sdk-0.8.0/src/arcaflow_plugin_sdk/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-10-17 15:08:22.000000 arcaflow_plugin_sdk-0.8.0/src/arcaflow_plugin_sdk/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 15:10:44.873569 arcaflow_plugin_sdk-0.8.0/src/arcaflow_plugin_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3269 2022-10-17 15:10:44.000000 arcaflow_plugin_sdk-0.8.0/src/arcaflow_plugin_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      757 2022-10-17 15:10:44.000000 arcaflow_plugin_sdk-0.8.0/src/arcaflow_plugin_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-17 15:10:44.000000 arcaflow_plugin_sdk-0.8.0/src/arcaflow_plugin_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-10-17 15:10:44.000000 arcaflow_plugin_sdk-0.8.0/src/arcaflow_plugin_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-10-17 15:10:44.000000 arcaflow_plugin_sdk-0.8.0/src/arcaflow_plugin_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 11:24:39.153885 arcaflow_plugin_sdk-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    10174 2022-10-18 11:21:36.000000 arcaflow_plugin_sdk-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3269 2022-10-18 11:24:39.153885 arcaflow_plugin_sdk-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2738 2022-10-18 11:21:36.000000 arcaflow_plugin_sdk-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      750 2022-10-18 11:24:21.000000 arcaflow_plugin_sdk-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2022-10-18 11:24:39.157884 arcaflow_plugin_sdk-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 11:24:39.141884 arcaflow_plugin_sdk-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 11:24:39.153885 arcaflow_plugin_sdk-0.9.0/src/arcaflow_plugin_sdk/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-18 11:21:36.000000 arcaflow_plugin_sdk-0.9.0/src/arcaflow_plugin_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6152 2022-10-18 11:21:36.000000 arcaflow_plugin_sdk-0.9.0/src/arcaflow_plugin_sdk/_http.py
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2022-10-18 11:21:36.000000 arcaflow_plugin_sdk-0.9.0/src/arcaflow_plugin_sdk/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5195 2022-10-18 11:21:36.000000 arcaflow_plugin_sdk-0.9.0/src/arcaflow_plugin_sdk/atp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1398 2022-10-18 11:21:36.000000 arcaflow_plugin_sdk-0.9.0/src/arcaflow_plugin_sdk/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12542 2022-10-18 11:21:36.000000 arcaflow_plugin_sdk-0.9.0/src/arcaflow_plugin_sdk/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)   202072 2022-10-18 11:21:37.000000 arcaflow_plugin_sdk-0.9.0/src/arcaflow_plugin_sdk/schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2104 2022-10-18 11:21:37.000000 arcaflow_plugin_sdk-0.9.0/src/arcaflow_plugin_sdk/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3058 2022-10-18 11:21:37.000000 arcaflow_plugin_sdk-0.9.0/src/arcaflow_plugin_sdk/test_atp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6163 2022-10-18 11:21:37.000000 arcaflow_plugin_sdk-0.9.0/src/arcaflow_plugin_sdk/test_jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-10-18 11:21:37.000000 arcaflow_plugin_sdk-0.9.0/src/arcaflow_plugin_sdk/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)    48796 2022-10-18 11:21:37.000000 arcaflow_plugin_sdk-0.9.0/src/arcaflow_plugin_sdk/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)      202 2022-10-18 11:21:37.000000 arcaflow_plugin_sdk-0.9.0/src/arcaflow_plugin_sdk/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 11:24:39.153885 arcaflow_plugin_sdk-0.9.0/src/arcaflow_plugin_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3269 2022-10-18 11:24:39.000000 arcaflow_plugin_sdk-0.9.0/src/arcaflow_plugin_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      757 2022-10-18 11:24:39.000000 arcaflow_plugin_sdk-0.9.0/src/arcaflow_plugin_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-18 11:24:39.000000 arcaflow_plugin_sdk-0.9.0/src/arcaflow_plugin_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-10-18 11:24:39.000000 arcaflow_plugin_sdk-0.9.0/src/arcaflow_plugin_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-10-18 11:24:39.000000 arcaflow_plugin_sdk-0.9.0/src/arcaflow_plugin_sdk.egg-info/top_level.txt
```

### Comparing `arcaflow_plugin_sdk-0.8.0/LICENSE` & `arcaflow_plugin_sdk-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arcaflow_plugin_sdk-0.8.0/PKG-INFO` & `arcaflow_plugin_sdk-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcaflow_plugin_sdk
-Version: 0.8.0
+Version: 0.9.0
 Summary: Plugin SDK for the Arcaflow workflow engine
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/arcalot/arcaflow-python-sdk
 Project-URL: Bug Tracker, https://github.com/arcalot/arcaflow-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `arcaflow_plugin_sdk-0.8.0/README.md` & `arcaflow_plugin_sdk-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `arcaflow_plugin_sdk-0.8.0/pyproject.toml` & `arcaflow_plugin_sdk-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "arcaflow_plugin_sdk"
 # Do not change, the version is automatically updated in CI.
-version = "0.8.0"
+version = "0.9.0"
 authors = [
 ]
 description = "Plugin SDK for the Arcaflow workflow engine"
 readme = "README.md"
 license = { text="Apache-2.0" }
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `arcaflow_plugin_sdk-0.8.0/src/arcaflow_plugin_sdk/_http.py` & `arcaflow_plugin_sdk-0.9.0/src/arcaflow_plugin_sdk/_http.py`

 * *Files identical despite different names*

### Comparing `arcaflow_plugin_sdk-0.8.0/src/arcaflow_plugin_sdk/atp.py` & `arcaflow_plugin_sdk-0.9.0/src/arcaflow_plugin_sdk/atp.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,17 @@
         return 1
 
     signal.signal(signal.SIGTERM, _handle_exit)
     try:
         decoder = cbor2.decoder.CBORDecoder(stdin)
         encoder = cbor2.encoder.CBOREncoder(stdout)
 
+        # Decode empty "start output" message.
+        decoder.decode()
+
         start = HelloMessage(1, s)
         serialized_message = _HELLO_MESSAGE_SCHEMA.serialize(start)
         encoder.encode(serialized_message)
         stdout.flush()
 
         message = decoder.decode()
     except SystemExit:
@@ -132,14 +135,17 @@
         stdout: io.FileIO,
     ):
         self.stdin = stdin
         self.stdout = stdout
         self.decoder = cbor2.decoder.CBORDecoder(stdout)
         self.encoder = cbor2.encoder.CBOREncoder(stdin)
 
+    def start_output(self) -> None:
+        self.encoder.encode(None)
+
     def read_hello(self) -> HelloMessage:
         """
         This function reads the intial "Hello" message from the plugin.
         """
         message = self.decoder.decode()
         return _HELLO_MESSAGE_SCHEMA.unserialize(message)
```

### Comparing `arcaflow_plugin_sdk-0.8.0/src/arcaflow_plugin_sdk/jsonschema.py` & `arcaflow_plugin_sdk-0.9.0/src/arcaflow_plugin_sdk/jsonschema.py`

 * *Files identical despite different names*

### Comparing `arcaflow_plugin_sdk-0.8.0/src/arcaflow_plugin_sdk/plugin.py` & `arcaflow_plugin_sdk-0.9.0/src/arcaflow_plugin_sdk/plugin.py`

 * *Files identical despite different names*

### Comparing `arcaflow_plugin_sdk-0.8.0/src/arcaflow_plugin_sdk/schema.py` & `arcaflow_plugin_sdk-0.9.0/src/arcaflow_plugin_sdk/schema.py`

 * *Files identical despite different names*

### Comparing `arcaflow_plugin_sdk-0.8.0/src/arcaflow_plugin_sdk/serialization.py` & `arcaflow_plugin_sdk-0.9.0/src/arcaflow_plugin_sdk/serialization.py`

 * *Files identical despite different names*

### Comparing `arcaflow_plugin_sdk-0.8.0/src/arcaflow_plugin_sdk/test_atp.py` & `arcaflow_plugin_sdk-0.9.0/src/arcaflow_plugin_sdk/test_atp.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,15 @@
             self.fail("Plugin exited with non-zero status: {}".format(exit_status))
 
     def test_full_workflow(self):
         pid, stdin_writer, stdout_reader = self._execute_plugin()
 
         try:
             client = atp.PluginClient(stdin_writer.buffer.raw, stdout_reader.buffer.raw)
+            client.start_output()
             hello_message = client.read_hello()
             self.assertEqual(1, hello_message.version)
 
             self.assertEqual(
                 schema.SCHEMA_SCHEMA.serialize(test_schema),
                 schema.SCHEMA_SCHEMA.serialize(hello_message.schema)
             )
```

### Comparing `arcaflow_plugin_sdk-0.8.0/src/arcaflow_plugin_sdk/test_jsonschema.py` & `arcaflow_plugin_sdk-0.9.0/src/arcaflow_plugin_sdk/test_jsonschema.py`

 * *Files identical despite different names*

### Comparing `arcaflow_plugin_sdk-0.8.0/src/arcaflow_plugin_sdk/test_plugin.py` & `arcaflow_plugin_sdk-0.9.0/src/arcaflow_plugin_sdk/test_plugin.py`

 * *Files identical despite different names*

### Comparing `arcaflow_plugin_sdk-0.8.0/src/arcaflow_plugin_sdk/test_schema.py` & `arcaflow_plugin_sdk-0.9.0/src/arcaflow_plugin_sdk/test_schema.py`

 * *Files identical despite different names*

### Comparing `arcaflow_plugin_sdk-0.8.0/src/arcaflow_plugin_sdk.egg-info/PKG-INFO` & `arcaflow_plugin_sdk-0.9.0/src/arcaflow_plugin_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcaflow-plugin-sdk
-Version: 0.8.0
+Version: 0.9.0
 Summary: Plugin SDK for the Arcaflow workflow engine
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/arcalot/arcaflow-python-sdk
 Project-URL: Bug Tracker, https://github.com/arcalot/arcaflow-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `arcaflow_plugin_sdk-0.8.0/src/arcaflow_plugin_sdk.egg-info/SOURCES.txt` & `arcaflow_plugin_sdk-0.9.0/src/arcaflow_plugin_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

