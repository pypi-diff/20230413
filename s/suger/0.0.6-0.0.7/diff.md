# Comparing `tmp/suger-0.0.6.tar.gz` & `tmp/suger-0.0.7.tar.gz`

## Comparing `suger-0.0.6.tar` & `suger-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,31 @@
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 suger-0.0.6/upload.sh
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 suger-0.0.6/suger/__init__.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 suger-0.0.6/suger/common/FileUtils.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 suger-0.0.6/suger/common/ObjectUtils.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 suger-0.0.6/suger/common/StringUtils.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 suger-0.0.6/suger/common/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.0.6/suger/decorator/__init__.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 suger-0.0.6/suger/decorator/csv_decorator.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 suger-0.0.6/suger/decorator/string_decorator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 suger-0.0.6/tests/test_FileUtils.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 suger-0.0.6/tests/test_ObjectUtils.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 suger-0.0.6/tests/test_csv_decorator.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 suger-0.0.6/tests/test_string_decorator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.0.6/tests/decorator/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 suger-0.0.6/.gitignore
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 suger-0.0.6/LICENSE
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 suger-0.0.6/README.md
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 suger-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 suger-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 suger-0.0.7/setup.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 suger-0.0.7/upload.sh
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 suger-0.0.7/suger/__init__.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 suger-0.0.7/suger/common/CsvUtils.py
+-rw-r--r--   0        0        0     8254 2020-02-02 00:00:00.000000 suger-0.0.7/suger/common/FileCompareUtils.py
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 suger-0.0.7/suger/common/FileUtils.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 suger-0.0.7/suger/common/JsonUtils.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 suger-0.0.7/suger/common/ObjectUtils.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 suger-0.0.7/suger/common/SSH.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 suger-0.0.7/suger/common/StringUtils.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 suger-0.0.7/suger/common/TerminalUtils.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 suger-0.0.7/suger/common/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.0.7/suger/decorator/__init__.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 suger-0.0.7/suger/decorator/csv_decorator.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 suger-0.0.7/suger/decorator/string_decorator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 suger-0.0.7/tests/test_CsvUtils.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 suger-0.0.7/tests/test_FileCompareUtils.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 suger-0.0.7/tests/test_FileUtils.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 suger-0.0.7/tests/test_JsonUtils.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 suger-0.0.7/tests/test_ObjectUtils.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 suger-0.0.7/tests/test_SSH.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 suger-0.0.7/tests/test_TerminalUtils.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 suger-0.0.7/tests/test_csv_decorator.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 suger-0.0.7/tests/test_string_decorator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 suger-0.0.7/tests/decorator/__init__.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 suger-0.0.7/.gitignore
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 suger-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 suger-0.0.7/README.md
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 suger-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 suger-0.0.7/PKG-INFO
```

### Comparing `suger-0.0.6/suger/common/FileUtils.py` & `suger-0.0.7/suger/common/FileUtils.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,29 +4,33 @@
 from suger.common.StringUtils import StringUtils
 
 
 # @author SolarisNeko
 class FileUtils:
 
     @staticmethod
+    def getFullPath(your_path):
+        return os.path.abspath(your_path)
+
+    @staticmethod
     def scanDir(dirPath, suffix=""):
         """
         递归扫描指定目录下指定后缀的所有文件名。
         """
         fileNames = []
         for root, dirs, files in os.walk(dirPath):
             for name in files:
                 if (StringUtils.isNotBlank(suffix)):
                     if name.endswith(suffix):
                         fileNames.append(os.path.join(root, name))
                         continue
                     else:
                         continue
                 fileNames.append(os.path.join(root, name))
-        return fileNames
+        return list(map(FileUtils.getFullPath, fileNames))
 
     @staticmethod
     def deleteQuietly(fileOrDir):
         """
         尝试删除文件或目录，如果删除失败则不报错。
         """
         try:
@@ -53,13 +57,28 @@
         """
         读取文件内容并返回字符串。
         """
         with open(file, "r", encoding=encoding) as f:
             return f.read()
 
     @staticmethod
-    def writeStringToFile(file, data, encoding="utf-8"):
+    def writeStringToFile(file, data, encoding="utf-8", isAppend: bool = False):
+        if (isAppend):
+            with open(file, "a", encoding=encoding) as f:
+                f.write(data)
+            return
+
         """
         将字符串写入文件。
         """
         with open(file, "w", encoding=encoding) as f:
             f.write(data)
+
+    @classmethod
+    def isNotFileExists(cls, path):
+        return not FileUtils.isFileExists(path)
+
+    @classmethod
+    def isFileExists(cls, path):
+        if os.path.exists(path):
+            return True
+        return False
```

### Comparing `suger-0.0.6/suger/common/StringUtils.py` & `suger-0.0.7/suger/common/StringUtils.py`

 * *Files identical despite different names*

### Comparing `suger-0.0.6/suger/decorator/csv_decorator.py` & `suger-0.0.7/suger/decorator/csv_decorator.py`

 * *Files identical despite different names*

### Comparing `suger-0.0.6/LICENSE` & `suger-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `suger-0.0.6/pyproject.toml` & `suger-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "suger"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
     { name = "SolarisNeko", email = "1417015340@qq.com" },
 ]
 
 description = "suger is a sugar. use python in @decorator/@Annotation like other languages~"
 readme = "README.md"
```

### Comparing `suger-0.0.6/PKG-INFO` & `suger-0.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suger
-Version: 0.0.6
+Version: 0.0.7
 Summary: suger is a sugar. use python in @decorator/@Annotation like other languages~
 Project-URL: Homepage, https://github.com/SolarisNeko/python-suger
 Project-URL: Bug Tracker, https://github.com/SolarisNeko/python-suger/issues
 Author-email: SolarisNeko <1417015340@qq.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,30 +36,32 @@
 
 # How to use 如何使用
 ## install 安装依赖
 ```shell
 pip install suger
 ```
 
-## @string | __str__
+
+## decorator 装饰器/注解
+### @string | __str__
 ```python
 @string
 class MockData:
     def __init__(self, age):
         self.age = age
 
 
 data = MockData(18)
 
 # Output = "MockData(age=18)"
 print(data)
 
 ```
 
-## @csv | CSV 
+### @csv | CSV 
 ```python
 @csv
 class MockData:
     def __init__(self, name, age):
         self.name = name
         self.age = age
         self.emptyTips = ''
@@ -78,14 +80,43 @@
 
 # 示例中，有个字段为空
 # neko,18,
 # name,age,emptyTips
 
 ```
 
+## 工具
+### FileUtils 文件工具
+```python
+
+from suger.common import FileUtils
+
+# 递归扫描, png 格式
+fileArray = FileUtils.scanDir('C:/Users/suger/Documents/WeChat Files', 'png')
+print(fileArray)
+
+```
+
+
+### ObjectUtils 对象工具
+```python
+from suger.common import ObjectUtils
+
+# true
+ObjectUtils.isNull(None)
+
+#  true
+data = {}
+ObjectUtils.isNotNull(data)
+
+
+
+```
+
+
 
 # my project init
 ```shell
 git init
 
  git remote add github https://github.com/SolarisNeko/neko233-python-suger.git
  git remote add origin https://gitee.com/SolarisNeko/neko233-python-suger.git
```

