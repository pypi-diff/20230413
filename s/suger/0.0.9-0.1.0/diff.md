# Comparing `tmp/suger-0.0.9.tar.gz` & `tmp/suger-0.1.0.tar.gz`

## Comparing `suger-0.0.9.tar` & `suger-0.1.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 suger-0.0.9/setup.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 suger-0.0.9/upload.sh
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 suger-0.0.9/suger/__init__.py
--rw-r--r--   0        0        0     9260 2020-02-02 00:00:00.000000 suger-0.0.9/suger/common/FileCompareUtils.py
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 suger-0.0.9/suger/common/FileUtils.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 suger-0.0.9/suger/common/ObjectUtils.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 suger-0.0.9/suger/common/StringUtils.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 suger-0.0.9/suger/common/__init__.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 suger-0.0.9/suger/data_operator/CsvUtils.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 suger-0.0.9/suger/data_operator/ExcelUtils.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 suger-0.0.9/suger/data_operator/JsonUtils.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 suger-0.0.9/suger/data_operator/XmlUtils.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 suger-0.0.9/suger/data_operator/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.0.9/suger/decorator/__init__.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 suger-0.0.9/suger/decorator/csv_decorator.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 suger-0.0.9/suger/decorator/string_decorator.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 suger-0.0.9/suger/terminal/SSH.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 suger-0.0.9/suger/terminal/TerminalUtils.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 suger-0.0.9/suger/terminal/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.0.9/tests/__init__.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 suger-0.0.9/tests/test_CsvUtils.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 suger-0.0.9/tests/test_ExcelUtils.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 suger-0.0.9/tests/test_FileCompareUtils.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 suger-0.0.9/tests/test_FileUtils.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 suger-0.0.9/tests/test_JsonUtils.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 suger-0.0.9/tests/test_ObjectUtils.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 suger-0.0.9/tests/test_SSH.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 suger-0.0.9/tests/test_TerminalUtils.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 suger-0.0.9/tests/test_XmlUtils.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 suger-0.0.9/tests/test_csv_decorator.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 suger-0.0.9/tests/test_string_decorator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.0.9/tests/decorator/__init__.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 suger-0.0.9/.gitignore
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 suger-0.0.9/LICENSE
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 suger-0.0.9/README.md
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 suger-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 suger-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 suger-0.1.0/setup.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 suger-0.1.0/upload.sh
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 suger-0.1.0/suger/__init__.py
+-rw-r--r--   0        0        0     9260 2020-02-02 00:00:00.000000 suger-0.1.0/suger/common/FileCompareUtils.py
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 suger-0.1.0/suger/common/FileUtils.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 suger-0.1.0/suger/common/ObjectUtils.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 suger-0.1.0/suger/common/StringUtils.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 suger-0.1.0/suger/common/__init__.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 suger-0.1.0/suger/data_operator/CsvUtils.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 suger-0.1.0/suger/data_operator/ExcelUtils.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 suger-0.1.0/suger/data_operator/JsonUtils.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 suger-0.1.0/suger/data_operator/XmlUtils.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 suger-0.1.0/suger/data_operator/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.1.0/suger/decorator/__init__.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 suger-0.1.0/suger/decorator/csv_decorator.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 suger-0.1.0/suger/decorator/string_decorator.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 suger-0.1.0/suger/terminal/SSH.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 suger-0.1.0/suger/terminal/TerminalUtils.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 suger-0.1.0/suger/terminal/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 suger-0.1.0/tests/test_CsvUtils.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 suger-0.1.0/tests/test_ExcelUtils.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 suger-0.1.0/tests/test_FileCompareUtils.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 suger-0.1.0/tests/test_FileUtils.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 suger-0.1.0/tests/test_JsonUtils.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 suger-0.1.0/tests/test_ObjectUtils.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 suger-0.1.0/tests/test_SSH.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 suger-0.1.0/tests/test_TerminalUtils.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 suger-0.1.0/tests/test_XmlUtils.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 suger-0.1.0/tests/test_csv_decorator.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 suger-0.1.0/tests/test_string_decorator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.1.0/tests/decorator/__init__.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 suger-0.1.0/.gitignore
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 suger-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 suger-0.1.0/README.md
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 suger-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 suger-0.1.0/PKG-INFO
```

### Comparing `suger-0.0.9/suger/common/FileCompareUtils.py` & `suger-0.1.0/suger/common/FileCompareUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.0.9/suger/common/FileUtils.py` & `suger-0.1.0/suger/common/FileUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.0.9/suger/common/ObjectUtils.py` & `suger-0.1.0/suger/common/ObjectUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.0.9/suger/common/StringUtils.py` & `suger-0.1.0/suger/common/StringUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.0.9/suger/data_operator/CsvUtils.py` & `suger-0.1.0/suger/data_operator/CsvUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.0.9/suger/data_operator/ExcelUtils.py` & `suger-0.1.0/suger/data_operator/ExcelUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.0.9/suger/data_operator/JsonUtils.py` & `suger-0.1.0/suger/data_operator/JsonUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.0.9/suger/data_operator/XmlUtils.py` & `suger-0.1.0/suger/data_operator/XmlUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.0.9/suger/decorator/csv_decorator.py` & `suger-0.1.0/suger/decorator/csv_decorator.py`

 * *Files identical despite different names*

### Comparing `suger-0.0.9/suger/terminal/SSH.py` & `suger-0.1.0/suger/terminal/SSH.py`

 * *Files identical despite different names*

### Comparing `suger-0.0.9/suger/terminal/TerminalUtils.py` & `suger-0.1.0/suger/terminal/TerminalUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.0.9/tests/test_CsvUtils.py` & `suger-0.1.0/tests/test_CsvUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.0.9/tests/test_JsonUtils.py` & `suger-0.1.0/tests/test_JsonUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.0.9/LICENSE` & `suger-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `suger-0.0.9/pyproject.toml` & `suger-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "suger"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
     { name = "SolarisNeko", email = "1417015340@qq.com" },
 ]
 
 description = "suger is a sugar. use python in @decorator/@Annotation like other languages~"
 readme = "README.md"
```

