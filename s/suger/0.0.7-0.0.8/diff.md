# Comparing `tmp/suger-0.0.7.tar.gz` & `tmp/suger-0.0.8.tar.gz`

## Comparing `suger-0.0.7.tar` & `suger-0.0.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 suger-0.0.7/setup.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 suger-0.0.7/upload.sh
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 suger-0.0.7/suger/__init__.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 suger-0.0.7/suger/common/CsvUtils.py
--rw-r--r--   0        0        0     8254 2020-02-02 00:00:00.000000 suger-0.0.7/suger/common/FileCompareUtils.py
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 suger-0.0.7/suger/common/FileUtils.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 suger-0.0.7/suger/common/JsonUtils.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 suger-0.0.7/suger/common/ObjectUtils.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 suger-0.0.7/suger/common/SSH.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 suger-0.0.7/suger/common/StringUtils.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 suger-0.0.7/suger/common/TerminalUtils.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 suger-0.0.7/suger/common/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.0.7/suger/decorator/__init__.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 suger-0.0.7/suger/decorator/csv_decorator.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 suger-0.0.7/suger/decorator/string_decorator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 suger-0.0.7/tests/test_CsvUtils.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 suger-0.0.7/tests/test_FileCompareUtils.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 suger-0.0.7/tests/test_FileUtils.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 suger-0.0.7/tests/test_JsonUtils.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 suger-0.0.7/tests/test_ObjectUtils.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 suger-0.0.7/tests/test_SSH.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 suger-0.0.7/tests/test_TerminalUtils.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 suger-0.0.7/tests/test_csv_decorator.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 suger-0.0.7/tests/test_string_decorator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.0.7/tests/decorator/__init__.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 suger-0.0.7/.gitignore
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 suger-0.0.7/LICENSE
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 suger-0.0.7/README.md
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 suger-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 suger-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 suger-0.0.8/setup.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 suger-0.0.8/upload.sh
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 suger-0.0.8/suger/__init__.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 suger-0.0.8/suger/common/CsvUtils.py
+-rw-r--r--   0        0        0     9253 2020-02-02 00:00:00.000000 suger-0.0.8/suger/common/FileCompareUtils.py
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 suger-0.0.8/suger/common/FileUtils.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 suger-0.0.8/suger/common/JsonUtils.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 suger-0.0.8/suger/common/ObjectUtils.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 suger-0.0.8/suger/common/SSH.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 suger-0.0.8/suger/common/StringUtils.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 suger-0.0.8/suger/common/TerminalUtils.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 suger-0.0.8/suger/common/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.0.8/suger/decorator/__init__.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 suger-0.0.8/suger/decorator/csv_decorator.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 suger-0.0.8/suger/decorator/string_decorator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 suger-0.0.8/tests/test_CsvUtils.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 suger-0.0.8/tests/test_FileCompareUtils.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 suger-0.0.8/tests/test_FileUtils.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 suger-0.0.8/tests/test_JsonUtils.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 suger-0.0.8/tests/test_ObjectUtils.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 suger-0.0.8/tests/test_SSH.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 suger-0.0.8/tests/test_TerminalUtils.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 suger-0.0.8/tests/test_csv_decorator.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 suger-0.0.8/tests/test_string_decorator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.0.8/tests/decorator/__init__.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 suger-0.0.8/.gitignore
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 suger-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 suger-0.0.8/README.md
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 suger-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 suger-0.0.8/PKG-INFO
```

### Comparing `suger-0.0.7/suger/common/CsvUtils.py` & `suger-0.0.8/suger/common/CsvUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.0.7/suger/common/FileCompareUtils.py` & `suger-0.0.8/suger/common/FileCompareUtils.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,51 +3,69 @@
 import string
 import time
 from typing import List
 
 from suger.common import StringUtils, FileUtils
 from suger.common.CsvUtils import CsvUtils
 
-
 #
 DEFAULT_FILE_VERSION_OUTPUT_PATH = 'file_use_metadata.csv'
 # 对比结果
-DEFAULT_COMPARE_FILE_OUTPUT_PATH = 'FileCompareUtils_compare_results.txt'
+DEFAULT_COMPARE_FILE_OUTPUT_PATH = 'FileCompareUtils_compare_results.output'
 
 
 class FileCompareUtils:
 
     @staticmethod
     def writeCompareFileVersionInfo(result_output_file=DEFAULT_COMPARE_FILE_OUTPUT_PATH,
+                                    isSplitOutput=True,
                                     input_scan_directory: string = './',
                                     isNeedMd5: bool = True,
                                     history_data_file_full_path: string = DEFAULT_FILE_VERSION_OUTPUT_PATH,
                                     ):
         same_changed_objs, only_in_list1_objs, only_in_list2_objs \
-            = FileCompareUtils.compareFileVersion(input_scan_directory
-                                                  , isNeedMd5
-                                                  , history_data_file_full_path)
-
-        FileUtils.writeStringToFile(result_output_file, '[is deleted]\n')
-        FileUtils.writeStringToFile(result_output_file, CsvUtils.serialize(only_in_list1_objs), isAppend=True)
-        FileUtils.writeStringToFile(result_output_file, '\n---\n', isAppend=True)
-        FileUtils.writeStringToFile(result_output_file, '[is changed]\n', isAppend=True)
-        FileUtils.writeStringToFile(result_output_file, CsvUtils.serialize(same_changed_objs), isAppend=True)
-        FileUtils.writeStringToFile(result_output_file, '\n---\n', isAppend=True)
-        FileUtils.writeStringToFile(result_output_file, '[is created]\n', isAppend=True)
-        FileUtils.writeStringToFile(result_output_file, CsvUtils.serialize(only_in_list2_objs), isAppend=True)
+            = FileCompareUtils.compareFileVersion(filterFileName=result_output_file,
+                                                  input_scan_directory=input_scan_directory,
+                                                  isNeedMd5=isNeedMd5,
+                                                  history_data_file_full_path=history_data_file_full_path,
+                                                  )
+
+        isDeleteFile = result_output_file + '.deleted'
+        isChangedFile = result_output_file + '.changed'
+        isCreatedFile = result_output_file + '.created'
+
+        if not isSplitOutput:
+            FileUtils.writeStringToFile(result_output_file, '[is deleted]\n')
+            FileUtils.writeStringToFile(result_output_file, CsvUtils.serialize(only_in_list1_objs), isAppend=True)
+            FileUtils.writeStringToFile(result_output_file, '\n---\n', isAppend=True)
+            FileUtils.writeStringToFile(result_output_file, '[is changed]\n', isAppend=True)
+            FileUtils.writeStringToFile(result_output_file, CsvUtils.serialize(same_changed_objs), isAppend=True)
+            FileUtils.writeStringToFile(result_output_file, '\n---\n', isAppend=True)
+            FileUtils.writeStringToFile(result_output_file, '[is created]\n', isAppend=True)
+            FileUtils.writeStringToFile(result_output_file, CsvUtils.serialize(only_in_list2_objs), isAppend=True)
+            return;
+
+        FileUtils.writeStringToFile(isDeleteFile, CsvUtils.serialize(only_in_list1_objs))
+
+        FileUtils.writeStringToFile(isChangedFile, CsvUtils.serialize(same_changed_objs))
+
+        FileUtils.writeStringToFile(isCreatedFile, CsvUtils.serialize(only_in_list2_objs))
 
     @staticmethod
-    def compareFileVersion(input_scan_directory: string = './',
+    def compareFileVersion(filterFileName: string,
+                           input_scan_directory: string = './',
                            isNeedMd5: bool = True,
                            history_data_file_full_path: string = DEFAULT_FILE_VERSION_OUTPUT_PATH,
                            ):
-        newDtoList, output_file_name = FileCompareUtils.getFileVersionInfo(input_scan_directory,
-                                                                           isNeedMd5,
-                                                                           history_data_file_full_path)
+        originalNewDtoList, output_file_name = FileCompareUtils.getFileVersionInfo(input_scan_directory,
+                                                                                   isNeedMd5,
+                                                                                   history_data_file_full_path)
+
+        # filter output file name
+        newDtoList = [dto for dto in originalNewDtoList if filterFileName not in dto.fullpath]
 
         old_csv_str = FileUtils.readFileToString(history_data_file_full_path)
         oldDtoList = CsvUtils.deserialize(old_csv_str, FileCompareDto)
 
         same_changed_objs, only_in_list1_objs, only_in_list2_objs \
             = FileCompareUtils.compare_dto_lists(oldDtoList, newDtoList, FileCompareDto.PK_FIELD)
```

### Comparing `suger-0.0.7/suger/common/FileUtils.py` & `suger-0.0.8/suger/common/FileUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.0.7/suger/common/JsonUtils.py` & `suger-0.0.8/suger/common/JsonUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.0.7/suger/common/ObjectUtils.py` & `suger-0.0.8/suger/common/ObjectUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.0.7/suger/common/SSH.py` & `suger-0.0.8/suger/common/SSH.py`

 * *Files identical despite different names*

### Comparing `suger-0.0.7/suger/common/StringUtils.py` & `suger-0.0.8/suger/common/StringUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.0.7/suger/decorator/csv_decorator.py` & `suger-0.0.8/suger/decorator/csv_decorator.py`

 * *Files identical despite different names*

### Comparing `suger-0.0.7/tests/test_CsvUtils.py` & `suger-0.0.8/tests/test_CsvUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.0.7/tests/test_JsonUtils.py` & `suger-0.0.8/tests/test_JsonUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.0.7/LICENSE` & `suger-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `suger-0.0.7/README.md` & `suger-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `suger-0.0.7/pyproject.toml` & `suger-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "suger"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
     { name = "SolarisNeko", email = "1417015340@qq.com" },
 ]
 
 description = "suger is a sugar. use python in @decorator/@Annotation like other languages~"
 readme = "README.md"
```

### Comparing `suger-0.0.7/PKG-INFO` & `suger-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suger
-Version: 0.0.7
+Version: 0.0.8
 Summary: suger is a sugar. use python in @decorator/@Annotation like other languages~
 Project-URL: Homepage, https://github.com/SolarisNeko/python-suger
 Project-URL: Bug Tracker, https://github.com/SolarisNeko/python-suger/issues
 Author-email: SolarisNeko <1417015340@qq.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

