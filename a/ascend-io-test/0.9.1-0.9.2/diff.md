# Comparing `tmp/ascend_io_test-0.9.1.tar.gz` & `tmp/ascend_io_test-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascend_io_test-0.9.1.tar", max compression
+gzip compressed data, was "ascend_io_test-0.9.2.tar", max compression
```

## Comparing `ascend_io_test-0.9.1.tar` & `ascend_io_test-0.9.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-03-23 14:32:28.635111 ascend_io_test-0.9.1/LICENSE
--rw-r--r--   0        0        0     4263 2023-03-23 14:32:28.635111 ascend_io_test-0.9.1/README.rst
--rw-r--r--   0        0        0       59 2023-03-23 14:32:28.635111 ascend_io_test-0.9.1/ascend_io_test/framework/__init__.py
--rw-r--r--   0        0        0     4973 2023-03-23 14:32:28.635111 ascend_io_test-0.9.1/ascend_io_test/framework/ascend_pyspark_transform.py
--rw-r--r--   0        0        0     1722 2023-03-23 14:32:28.635111 ascend_io_test-0.9.1/ascend_io_test/framework/ascend_python_bytestream_read_connector.py
--rw-r--r--   0        0        0     3758 2023-03-23 14:32:28.635111 ascend_io_test-0.9.1/ascend_io_test/framework/ascend_python_read_connector.py
--rw-r--r--   0        0        0     1091 2023-03-23 14:32:28.635111 ascend_io_test-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     5172 1970-01-01 00:00:00.000000 ascend_io_test-0.9.1/setup.py
--rw-r--r--   0        0        0     5548 1970-01-01 00:00:00.000000 ascend_io_test-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-13 16:30:12.319238 ascend_io_test-0.9.2/LICENSE
+-rw-r--r--   0        0        0     4263 2023-04-13 16:30:12.319238 ascend_io_test-0.9.2/README.rst
+-rw-r--r--   0        0        0       59 2023-04-13 16:30:12.319238 ascend_io_test-0.9.2/ascend_io_test/framework/__init__.py
+-rw-r--r--   0        0        0     4973 2023-04-13 16:30:12.319238 ascend_io_test-0.9.2/ascend_io_test/framework/ascend_pyspark_transform.py
+-rw-r--r--   0        0        0     1722 2023-04-13 16:30:12.319238 ascend_io_test-0.9.2/ascend_io_test/framework/ascend_python_bytestream_read_connector.py
+-rw-r--r--   0        0        0     4560 2023-04-13 16:30:12.319238 ascend_io_test-0.9.2/ascend_io_test/framework/ascend_python_read_connector.py
+-rw-r--r--   0        0        0     1091 2023-04-13 16:30:12.319238 ascend_io_test-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     5172 1970-01-01 00:00:00.000000 ascend_io_test-0.9.2/setup.py
+-rw-r--r--   0        0        0     5548 1970-01-01 00:00:00.000000 ascend_io_test-0.9.2/PKG-INFO
```

### Comparing `ascend_io_test-0.9.1/LICENSE` & `ascend_io_test-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ascend_io_test-0.9.1/README.rst` & `ascend_io_test-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `ascend_io_test-0.9.1/ascend_io_test/framework/ascend_pyspark_transform.py` & `ascend_io_test-0.9.2/ascend_io_test/framework/ascend_pyspark_transform.py`

 * *Files identical despite different names*

### Comparing `ascend_io_test-0.9.1/ascend_io_test/framework/ascend_python_bytestream_read_connector.py` & `ascend_io_test-0.9.2/ascend_io_test/framework/ascend_python_bytestream_read_connector.py`

 * *Files identical despite different names*

### Comparing `ascend_io_test-0.9.1/ascend_io_test/framework/ascend_python_read_connector.py` & `ascend_io_test-0.9.2/ascend_io_test/framework/ascend_python_read_connector.py`

 * *Files 20% similar despite different names*

```diff
@@ -62,14 +62,16 @@
       patches = []
     self.credentials = credentials
     self.module = module
     self.name = name
     self.def_context = _get_method(module, 'context')
     self.def_list_objects = _get_method(module, 'list_objects')
     self.def_read_bytes = _get_method(module, 'read_bytes')
+    self.def_read_spark_dataframe = _get_method(module, 'read_spark_dataframe')
+    self.def_read_pandas_dataframe = _get_method(module, 'read_pandas_dataframe')
     self.patches = patches
 
     # inject pytest fixtures if they were applied to the global method
     caller_globals = inspect.stack()[1][0].f_globals
     caller_globals['context_result'] = _result_fixture('function', None)
     caller_globals['list_objects_result'] = _result_fixture('function', None)
     caller_globals['read_bytes_result'] = _result_fixture('function', None)
@@ -88,15 +90,26 @@
       # TODO: implement some meaningful metadata
       if self.name:
         context_result['name'] = self.name
       list_objects_result = [o for o in self.def_list_objects(context_result, {})]
 
       read_bytes_result = []
       for result in list_objects_result:
-        read_bytes_result = list(b for b in self.def_read_bytes(context_result, MetadataSupport(**result).to_dict()))
+        if self.def_read_bytes:
+          assert not self.def_read_spark_dataframe
+          assert not self.def_read_pandas_dataframe
+          read_bytes_result = (list(b for b in self.def_read_bytes(context_result, MetadataSupport(**result).to_dict())))
+        elif self.def_read_spark_dataframe:
+          assert not self.def_read_bytes
+          assert not self.def_read_pandas_dataframe
+          read_bytes_result = self.def_read_spark_dataframe(context_result, MetadataSupport(**result).to_dict())
+        elif self.def_read_pandas_dataframe:
+          assert not self.def_read_bytes
+          assert not self.def_read_spark_dataframe
+          read_bytes_result = self.def_read_pandas_dataframe(context_result, MetadataSupport(**result).to_dict())
 
       logging.debug('read connector interface calls complete')
       # write the data back to the test method for assertion
       full_args = inspect.getfullargspec(func)
       if 'context_result' in full_args.args:
         kwargs['context_result'] = context_result
       if 'list_objects_result' in full_args.args:
```

### Comparing `ascend_io_test-0.9.1/pyproject.toml` & `ascend_io_test-0.9.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ascend-io-test"
-version = "0.9.1"
+version = "0.9.2"
 description = "The Ascend Python Test Framework"
 license = "Apache-2.0"
 authors = ["Ascend.io Engineering <support@ascend.io>"]
 maintainers = ["Ascend.io Engineering <support@ascend.io>"]
 readme = "README.rst"
 homepage = "https://www.ascend.io"
 documentation = "https://developer.ascend.io"
```

### Comparing `ascend_io_test-0.9.1/setup.py` & `ascend_io_test-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pyspark>=3.3.1,<4.0.0', 'pytest-mock>=3.10.0,<4.0.0', 'pytest>=7.2.1,<8.0.0']
 
 setup_kwargs = {
     'name': 'ascend-io-test',
-    'version': '0.9.1',
+    'version': '0.9.2',
     'description': 'The Ascend Python Test Framework',
     'long_description': '========================\nAscend.io Test Framework\n========================\n\nThis package helps developers who are writing custom python for Ascend.io automated pipelines by providing a local\ntesting framework. Local testing speeds the development of python pipeline code. The local framework exercises the\ncode as if the code was running directly in the platform while giving you access to patching and mocking frameworks.\n\nDocumentation, including examples, is located in our `Ascend Developer Hub <https://developer.ascend.io>`_.\n\nHere is a basic python transformation test case example. The python code under test is located in a file\nwith the name ``my_python_transform.py`` and imported with the name ``my_python_transform``. Other variables,\nimports, and code are omitted for brevity::\n\n    @AscendPySparkTransform(spark=spark_session,\n                            module=my_python_transform,\n                            schema=input_schema,\n                            data=[(123, \'NORMAL\', today, today + datetime.timedelta(days=1))],\n                            credentials=test_creds,\n                            discover_schema=True,\n                            patches=[patch(\'requests.post\', return_value=Mock(status_code=200,\n                                                                              text=\'{"internalReportIds":"REPORT_A"}\')),\n                                     patch(\'requests.get\', return_value=Mock(status_code=200,\n                                                                             text=\'{"status":"SUCCESS", "downloadLink": "https://test.my.download"}\')),\n                                     patch(\'pandas.read_csv\', return_value=build_mock_csv()),\n                                     ], )\n    def test_normal_loading_process_single_record(input_dataframe, transform_result: DataFrame, mock_results: List[Mock]):\n      """Check that a normal call does the work properly.\n            Assert values are correct.\n            Assert mock services are called."""\n      assert input_dataframe\n      assert transform_result\n      assert transform_result.count() == 3\n      dataset = transform_result.collect()\n      # check field mapping\n      assert dataset[0][\'CUSTOMER_ID\'] == \'101\'\n      assert dataset[1][\'CUSTOMER_ID\'] == \'102\'\n      assert dataset[2][\'CUSTOMER_ID\'] == \'103\'\n      assert dataset[0][\'YOUR_NAME\'] == "customerName.one"\n      assert dataset[0][\'THE_OBJECTIVE\'] == "customerBudget.one"\n      assert dataset[0][\'AD_ID\'] == "tempId.one"\n      assert dataset[0][\'AD_NAME\'] == "myName.one"\n      assert dataset[0][\'GEO_LOC\'] == "geo_location.one"\n      assert dataset[0][\'ORDER_ID\'] == "orderId.test"\n      assert dataset[0][\'ORDER_NAME\'] == "orderName.test"\n      assert dataset[0][\'DT\'] == "__time.one"\n      assert dataset[0][\'AUDIO_IMPRESSIONS\'] == 1\n      assert transform_result.columns.__contains__(\'RUN_ID\')\n      assert transform_result.columns.__contains__(\'REPORT_START_DT\')\n      assert transform_result.columns.__contains__(\'REPORT_END_DT\')\n      assert transform_result.columns.__contains__(\'record_number\')\n      # check mocks were properly called\n      mock_results[0].assert_called_once()\n      mock_results[1].assert_called_once_with(f"https://custom.io/v1/async-query/REPORT_A",\n                                              headers={\'agency\': \'12\', \'x-api-key\': \'key\', \'Content-Type\': \'application/json\'})\n      mock_results[2].assert_called_once_with("https://test.my.download", header=0, skip_blank_lines=True)\n\n\nDecorators are available for all types of Ascend python implementation strategies. Testing scenarios are only limited\nby your creativity and desire to produce high quality code.\n\nDownload your pipelines using the `Ascend CLI <https://pypi.org/project/ascend-io-cli/>`_ like this::\n\n    ascend download data-flow MY_DATASERVICE MY_DATA_FLOW\n\nWrite some tests. When your test cases are complete, pushing the code to the platform is simple with\nthe `CLI <https://pypi.org/project/ascend-io-cli/>`_. For example::\n\n    ascend apply data-flow MY_DATASERVICE MY_DATA_FLOW\n\n\n---------------\nRead the Docs\n---------------\n* `Ascend Developer Hub <https://developer.ascend.io>`_\n* `Ascend.io <https://www.ascend.io>`_\n* `Ascend CLI <https://pypi.org/project/ascend-io-cli/>`_\n',
     'author': 'Ascend.io Engineering',
     'author_email': 'support@ascend.io',
     'maintainer': 'Ascend.io Engineering',
     'maintainer_email': 'support@ascend.io',
     'url': 'https://www.ascend.io',
```

### Comparing `ascend_io_test-0.9.1/PKG-INFO` & `ascend_io_test-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascend-io-test
-Version: 0.9.1
+Version: 0.9.2
 Summary: The Ascend Python Test Framework
 Home-page: https://www.ascend.io
 License: Apache-2.0
 Keywords: ascend,pipeline,data,automation,platform
 Author: Ascend.io Engineering
 Author-email: support@ascend.io
 Maintainer: Ascend.io Engineering
```

