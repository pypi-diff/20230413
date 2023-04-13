# Comparing `tmp/ats_case-0.4.2.tar.gz` & `tmp/ats_case-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.4.2.tar", last modified: Wed Apr 12 01:19:10 2023, max compression
+gzip compressed data, was "ats_case-0.4.3.tar", last modified: Thu Apr 13 02:22:15 2023, max compression
```

## Comparing `ats_case-0.4.2.tar` & `ats_case-0.4.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 01:19:10.180730 ats_case-0.4.2/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.4.2/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-04-12 01:19:10.169760 ats_case-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 01:19:09.204342 ats_case-0.4.2/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.4.2/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 01:19:09.929402 ats_case-0.4.2/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.4.2/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    17147 2023-04-12 01:02:29.000000 ats_case-0.4.2/ats_case/case/command.py
--rw-rw-rw-   0        0        0    10103 2023-04-07 01:41:51.000000 ats_case-0.4.2/ats_case/case/context.py
--rw-rw-rw-   0        0        0     5143 2023-04-12 01:07:14.000000 ats_case-0.4.2/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5437 2023-04-12 01:16:48.000000 ats_case-0.4.2/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-04-12 01:19:10.045093 ats_case-0.4.2/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.4.2/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      381 2023-04-10 07:20:19.000000 ats_case-0.4.2/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      628 2023-04-11 03:13:44.000000 ats_case-0.4.2/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-04-12 01:19:10.092965 ats_case-0.4.2/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.4.2/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.4.2/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     2586 2023-04-12 01:16:48.000000 ats_case-0.4.2/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-04-12 01:19:10.143829 ats_case-0.4.2/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.4.2/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2089 2023-04-12 01:03:34.000000 ats_case-0.4.2/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-04-12 01:19:09.389847 ats_case-0.4.2/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-04-12 01:19:08.000000 ats_case-0.4.2/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-04-12 01:19:08.000000 ats_case-0.4.2/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 01:19:08.000000 ats_case-0.4.2/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-04-12 01:19:08.000000 ats_case-0.4.2/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-12 01:19:08.000000 ats_case-0.4.2/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 01:19:10.180730 ats_case-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0      916 2023-04-12 01:19:03.000000 ats_case-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:22:15.707571 ats_case-0.4.3/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.4.3/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.4.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-04-13 02:22:15.704976 ats_case-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 02:22:15.293085 ats_case-0.4.3/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.4.3/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:22:15.508533 ats_case-0.4.3/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.4.3/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    16964 2023-04-13 02:21:54.000000 ats_case-0.4.3/ats_case/case/command.py
+-rw-rw-rw-   0        0        0    10103 2023-04-07 01:41:51.000000 ats_case-0.4.3/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     5143 2023-04-12 01:07:14.000000 ats_case-0.4.3/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5437 2023-04-12 01:16:48.000000 ats_case-0.4.3/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:22:15.573135 ats_case-0.4.3/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.4.3/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      381 2023-04-10 07:20:19.000000 ats_case-0.4.3/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      628 2023-04-11 03:13:44.000000 ats_case-0.4.3/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:22:15.637332 ats_case-0.4.3/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.4.3/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.4.3/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     2586 2023-04-12 01:16:48.000000 ats_case-0.4.3/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-04-13 02:22:15.693851 ats_case-0.4.3/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.4.3/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2089 2023-04-12 01:03:34.000000 ats_case-0.4.3/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-04-13 02:22:15.393919 ats_case-0.4.3/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-04-13 02:22:14.000000 ats_case-0.4.3/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-04-13 02:22:14.000000 ats_case-0.4.3/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 02:22:14.000000 ats_case-0.4.3/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-04-13 02:22:14.000000 ats_case-0.4.3/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-13 02:22:14.000000 ats_case-0.4.3/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 02:22:15.707571 ats_case-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      935 2023-04-13 02:21:54.000000 ats_case-0.4.3/setup.py
```

### Comparing `ats_case-0.4.2/PKG-INFO` & `ats_case-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.4.2
+Version: 0.4.3
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.4.2/README.md` & `ats_case-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.2/ats_case/case/command.py` & `ats_case-0.4.3/ats_case/case/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import time
 
 from ats_base.common import func
 from ats_base.log.logger import logger
-from ats_base.service import app, pro, em, udm, mm
+from ats_base.service import app, pro, em, udm
 
 from ats_case.case.context import Context
 from ats_case.common.enum import ProClazz, OperationClazz
 from ats_case.common.error import APIError, ClientReturnError
 
 """
     常用操作命令
@@ -226,14 +226,15 @@
         logger.info('~ @PRO-DECODE-> protocol:{} frame:{}'.format(self._protocol, self._frame))
         data = pro.decode(func.to_dict(protocol=self._protocol.name, frame=self._frame, session_key=context.session.basename))
         logger.info('~ @PRO-DECODE<- protocol:{} parse:{}'.format(self._protocol, data))
 
         self._handle_framing(context, data)
 
         self._parse = data.get('parse').get('link_data').get('mission').get('result')
+        self._flush(context)
         return self._parse
 
     def _handle_framing(self, context: Context, data: dict, index=0):
         try:
             next_frame = data['parse']['next_frame']
         except:
             next_frame = None
@@ -256,41 +257,36 @@
                                                                          , parameter=self._parameter,
                                                                          result=self._parse)})
 
     def acv(self, context: Context):
         result = str(self._parse)
         if self._func is not None:
             if type(self._func_parameter) is not dict:
-                self._func_parameter = {}
-            self._func_parameter['result'] = self._parse
-            self._func_parameter = _replace(context, self._func_parameter)
+                self._func_parameter = _replace(context, self._func_parameter)
             try:
-                self._func_parameter['expect_result'] = context.runtime.steps[context.runtime.step - 1]
+                expect_result = context.runtime.steps[context.runtime.step - 1]
             except:
-                pass
+                expect_result = None
+            data = func.to_dict(result=self._parse, expect_result=expect_result, parameter=self._func_parameter)
 
             logger.info('~ @ACD-> module:{} function:{} parameter:{}'.format(
                 self._func_module, self._func, self._func_parameter))
             result = udm.acv(module='meter.{}'.format(self._func_module), function=self._func
-                             , data=self._func_parameter, url=context.acd_url)
+                             , data=data, url=context.acd_url)
             logger.info('~ @ACD<- module:{} function:{} result:{}'.format(self._func_module, self._func, result))
 
         return result
 
     def exec(self, context: Context):
         self.encode(context)
         result = send(context,
                       todo={'meter:comm': {'channel': {'type': 'RS485', 'baudrate': 9600}, 'frame': self._frame}})
-
         self._frame = result.get('result')
-        
         self.decode(context)
 
-        self._flush(context)
-
         send(context, todo={'app:show': {'msg': self.acv(context)}})
 
 
 """
     加密机篇
 """
 
@@ -300,15 +296,14 @@
 
 
 class Encryptor(object):
     def __init__(self, protocol):
         self._protocol = ProClazz(protocol)
         self._operation = None
         self._parameter = None
-        self._func_parameter = {}
         self._result = None
 
     def operation(self, op: str):
         self._operation = op
         return self
 
     def parameter(self, param=None):
@@ -332,22 +327,20 @@
 
     def _flush(self, context: Context):
         context.runtime.steps.update({context.runtime.step: func.to_dict(obj='em', op=self._operation
                                                                          , parameter=self._parameter,
                                                                          result=self._result)})
 
     def acv(self, context: Context):
-        # self._func_parameter['basename'] = context.session.basename
-        # self._func_parameter['parameter'] = self._parameter
-        self._func_parameter['result'] = self._result
+        data = func.to_dict(result=self._result)
 
         logger.info('~ @ACD-> module:{} function:{} parameter:{}'.format(
             self._protocol.name, self._operation, self._parameter))
         result = udm.acv(module='em.{}'.format(self._protocol.name), function=self._operation
-                         , data=self._func_parameter, url=context.acd_url)
+                         , data=data, url=context.acd_url)
         logger.info('~ @ACD<- module:{} function:{} result:{}'.format(self._protocol.name, self._operation, result))
 
         return result
 
     def exec(self, context: Context):
         self.handle(context)
         send(context, todo={'app:show': {'msg': self.acv(context)}})
@@ -403,32 +396,34 @@
         if self._function is not None and len(self._function) > 0:
             self._built_in(context)
 
     def decode(self, context: Context):
         logger.info('~ @BENCH<- manufacture:{} operation:{} result:{}'.format(self._manufacture,
                                                                               self._operation, self._result))
 
-        self._result = {'result': self._result.get('result')}
+        self._result = self._result.get('result')
         self._flush(context)
 
     def _built_in(self, context: Context):
         logger.info('~ @BUILTIN-> module:{} parameter:{}'.format('bench', self._parameter))
         for op, d in self._function.items():
             v_data = udm.built_in(module='bench', function=op, data=func.to_dict(
                 param=d, iabc=context.meter.iabc, voltage=context.meter.rated_voltage,
                 current=context.meter.rated_current, index=self._exec_times), url=context.acd_url)
             self._parameter = _replace_bench1(self._parameter, v_data)
 
         logger.info('~ @BUILTIN<- module:{} parameter:{}'.format('bench', self._parameter))
 
     def acv(self, context: Context):
+        data = func.to_dict(result=self._result)
+
         logger.info('~ @ACD-> module:{} function:{} parameter:{}'.format(
             'bench', self._operation, self._result))
         result = udm.acv(module='bench.{}'.format(self._manufacture), function=self._operation
-                         , data=self._result, url=context.acd_url)
+                         , data=data, url=context.acd_url)
         logger.info('~ @ACD<- module:{} function:{} result:{}'.format('bench', self._operation, result))
 
         return result
 
     def _flush(self, context: Context):
         context.runtime.steps.update({context.runtime.step: func.to_dict(obj='bench', op=self._operation
                                                                          , parameter=self._parameter,
```

### Comparing `ats_case-0.4.2/ats_case/case/context.py` & `ats_case-0.4.3/ats_case/case/context.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.2/ats_case/case/executor.py` & `ats_case-0.4.3/ats_case/case/executor.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.2/ats_case/case/translator.py` & `ats_case-0.4.3/ats_case/case/translator.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.2/ats_case/common/error.py` & `ats_case-0.4.3/ats_case/common/error.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.2/ats_case/manage/core.py` & `ats_case-0.4.3/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.2/ats_case/manage/start.py` & `ats_case-0.4.3/ats_case/manage/start.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.2/ats_case/template/testcase_v1.tmp` & `ats_case-0.4.3/ats_case/template/testcase_v1.tmp`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.2/ats_case.egg-info/PKG-INFO` & `ats_case-0.4.3/ats_case.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.4.2
+Version: 0.4.3
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.4.2/ats_case.egg-info/SOURCES.txt` & `ats_case-0.4.3/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.2/setup.py` & `ats_case-0.4.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.4.2",
+    version="0.4.3",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
@@ -19,12 +19,12 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=setuptools.find_packages(),
     python_requires=">=3.9",
-    install_requires=["pytest", "psutil", "ats-base"],
+    install_requires=["pytest", "pytest-ordering", "psutil", "ats-base"],
     package_data={
         '': ['*.tmp'],
     },
 )
```

