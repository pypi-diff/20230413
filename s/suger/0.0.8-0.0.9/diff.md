# Comparing `tmp/suger-0.0.8.tar.gz` & `tmp/suger-0.0.9.tar.gz`

## Comparing `suger-0.0.8.tar` & `suger-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,37 @@
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 suger-0.0.8/setup.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 suger-0.0.8/upload.sh
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 suger-0.0.8/suger/__init__.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 suger-0.0.8/suger/common/CsvUtils.py
--rw-r--r--   0        0        0     9253 2020-02-02 00:00:00.000000 suger-0.0.8/suger/common/FileCompareUtils.py
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 suger-0.0.8/suger/common/FileUtils.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 suger-0.0.8/suger/common/JsonUtils.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 suger-0.0.8/suger/common/ObjectUtils.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 suger-0.0.8/suger/common/SSH.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 suger-0.0.8/suger/common/StringUtils.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 suger-0.0.8/suger/common/TerminalUtils.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 suger-0.0.8/suger/common/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.0.8/suger/decorator/__init__.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 suger-0.0.8/suger/decorator/csv_decorator.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 suger-0.0.8/suger/decorator/string_decorator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 suger-0.0.8/tests/test_CsvUtils.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 suger-0.0.8/tests/test_FileCompareUtils.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 suger-0.0.8/tests/test_FileUtils.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 suger-0.0.8/tests/test_JsonUtils.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 suger-0.0.8/tests/test_ObjectUtils.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 suger-0.0.8/tests/test_SSH.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 suger-0.0.8/tests/test_TerminalUtils.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 suger-0.0.8/tests/test_csv_decorator.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 suger-0.0.8/tests/test_string_decorator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.0.8/tests/decorator/__init__.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 suger-0.0.8/.gitignore
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 suger-0.0.8/LICENSE
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 suger-0.0.8/README.md
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 suger-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 suger-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 suger-0.0.9/setup.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 suger-0.0.9/upload.sh
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 suger-0.0.9/suger/__init__.py
+-rw-r--r--   0        0        0     9260 2020-02-02 00:00:00.000000 suger-0.0.9/suger/common/FileCompareUtils.py
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 suger-0.0.9/suger/common/FileUtils.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 suger-0.0.9/suger/common/ObjectUtils.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 suger-0.0.9/suger/common/StringUtils.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 suger-0.0.9/suger/common/__init__.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 suger-0.0.9/suger/data_operator/CsvUtils.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 suger-0.0.9/suger/data_operator/ExcelUtils.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 suger-0.0.9/suger/data_operator/JsonUtils.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 suger-0.0.9/suger/data_operator/XmlUtils.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 suger-0.0.9/suger/data_operator/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.0.9/suger/decorator/__init__.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 suger-0.0.9/suger/decorator/csv_decorator.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 suger-0.0.9/suger/decorator/string_decorator.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 suger-0.0.9/suger/terminal/SSH.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 suger-0.0.9/suger/terminal/TerminalUtils.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 suger-0.0.9/suger/terminal/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 suger-0.0.9/tests/test_CsvUtils.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 suger-0.0.9/tests/test_ExcelUtils.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 suger-0.0.9/tests/test_FileCompareUtils.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 suger-0.0.9/tests/test_FileUtils.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 suger-0.0.9/tests/test_JsonUtils.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 suger-0.0.9/tests/test_ObjectUtils.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 suger-0.0.9/tests/test_SSH.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 suger-0.0.9/tests/test_TerminalUtils.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 suger-0.0.9/tests/test_XmlUtils.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 suger-0.0.9/tests/test_csv_decorator.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 suger-0.0.9/tests/test_string_decorator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.0.9/tests/decorator/__init__.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 suger-0.0.9/.gitignore
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 suger-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 suger-0.0.9/README.md
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 suger-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 suger-0.0.9/PKG-INFO
```

### Comparing `suger-0.0.8/suger/common/CsvUtils.py` & `suger-0.0.9/suger/data_operator/CsvUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.0.8/suger/common/FileCompareUtils.py` & `suger-0.0.9/suger/common/FileCompareUtils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import hashlib
 import os
 import string
 import time
 from typing import List
 
 from suger.common import StringUtils, FileUtils
-from suger.common.CsvUtils import CsvUtils
+from suger.data_operator.CsvUtils import CsvUtils
 
 #
 DEFAULT_FILE_VERSION_OUTPUT_PATH = 'file_use_metadata.csv'
 # 对比结果
 DEFAULT_COMPARE_FILE_OUTPUT_PATH = 'FileCompareUtils_compare_results.output'
```

### Comparing `suger-0.0.8/suger/common/FileUtils.py` & `suger-0.0.9/suger/common/FileUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.0.8/suger/common/JsonUtils.py` & `suger-0.0.9/suger/data_operator/JsonUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.0.8/suger/common/ObjectUtils.py` & `suger-0.0.9/suger/common/ObjectUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.0.8/suger/common/SSH.py` & `suger-0.0.9/suger/terminal/SSH.py`

 * *Files identical despite different names*

### Comparing `suger-0.0.8/suger/common/StringUtils.py` & `suger-0.0.9/suger/common/StringUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.0.8/suger/common/TerminalUtils.py` & `suger-0.0.9/suger/terminal/TerminalUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.0.8/suger/decorator/csv_decorator.py` & `suger-0.0.9/suger/decorator/csv_decorator.py`

 * *Files identical despite different names*

### Comparing `suger-0.0.8/tests/test_CsvUtils.py` & `suger-0.0.9/tests/test_CsvUtils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from unittest import TestCase
 
-from suger.common.CsvUtils import CsvUtils
+from suger.data_operator.CsvUtils import CsvUtils
 
 
 class TestCsvUtils(TestCase):
     def test_serialize(self):
         person1 = Person("Alice", 25)
         person2 = Person("Bob", 30)
         persons = [person1, person2]
```

### Comparing `suger-0.0.8/tests/test_JsonUtils.py` & `suger-0.0.9/tests/test_JsonUtils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from unittest import TestCase
 
-from suger.common import JsonUtils
+from suger.data_operator import JsonUtils
 
 
 class TestJsonUtils(TestCase):
     def test_serialize(self):
         user = User('neko233')
         json = JsonUtils.serialize(user)
         print(json)
```

### Comparing `suger-0.0.8/LICENSE` & `suger-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `suger-0.0.8/README.md` & `suger-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `suger-0.0.8/pyproject.toml` & `suger-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "suger"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     { name = "SolarisNeko", email = "1417015340@qq.com" },
 ]
 
 description = "suger is a sugar. use python in @decorator/@Annotation like other languages~"
 readme = "README.md"
```

### Comparing `suger-0.0.8/PKG-INFO` & `suger-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suger
-Version: 0.0.8
+Version: 0.0.9
 Summary: suger is a sugar. use python in @decorator/@Annotation like other languages~
 Project-URL: Homepage, https://github.com/SolarisNeko/python-suger
 Project-URL: Bug Tracker, https://github.com/SolarisNeko/python-suger/issues
 Author-email: SolarisNeko <1417015340@qq.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

