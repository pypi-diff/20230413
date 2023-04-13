# Comparing `tmp/legal_documents_cn-0.0.7.tar.gz` & `tmp/legal_documents_cn-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legal_documents_cn-0.0.7.tar", last modified: Mon Feb 20 13:25:33 2023, max compression
+gzip compressed data, was "legal_documents_cn-0.0.8.tar", last modified: Tue Feb 21 06:31:42 2023, max compression
```

## Comparing `legal_documents_cn-0.0.7.tar` & `legal_documents_cn-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 dongyuwu  (1026) dongyuwu  (1026)        0 2023-02-20 13:25:33.955805 legal_documents_cn-0.0.7/
--rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)     1091 2023-02-20 11:50:48.000000 legal_documents_cn-0.0.7/LICENSE
--rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)       43 2023-02-20 11:50:48.000000 legal_documents_cn-0.0.7/MANIFEST.in
--rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)     6603 2023-02-20 13:25:33.954805 legal_documents_cn-0.0.7/PKG-INFO
--rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)     6176 2023-02-20 12:21:41.000000 legal_documents_cn-0.0.7/README.md
-drwxrwxr-x   0 dongyuwu  (1026) dongyuwu  (1026)        0 2023-02-20 13:25:33.953805 legal_documents_cn-0.0.7/legal_documents_cn/
--rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)      231 2023-02-20 11:50:48.000000 legal_documents_cn-0.0.7/legal_documents_cn/__init__.py
--rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)      600 2023-02-20 12:05:45.000000 legal_documents_cn-0.0.7/legal_documents_cn/apitest.py
--rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)   258368 2023-02-20 11:50:48.000000 legal_documents_cn-0.0.7/legal_documents_cn/criminal_law.csv
--rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)     7095 2023-02-20 12:14:31.000000 legal_documents_cn-0.0.7/legal_documents_cn/criminal_law_cn.py
--rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)     8410 2023-02-20 11:50:48.000000 legal_documents_cn-0.0.7/legal_documents_cn/process_data.py
--rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)     6339 2023-02-20 11:50:48.000000 legal_documents_cn-0.0.7/legal_documents_cn/run_start_api.py
--rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)     1311 2023-02-20 11:50:48.000000 legal_documents_cn-0.0.7/legal_documents_cn/start_api.py
-drwxrwxr-x   0 dongyuwu  (1026) dongyuwu  (1026)        0 2023-02-20 13:25:33.954805 legal_documents_cn-0.0.7/legal_documents_cn.egg-info/
--rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)     6603 2023-02-20 13:25:33.000000 legal_documents_cn-0.0.7/legal_documents_cn.egg-info/PKG-INFO
--rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)      485 2023-02-20 13:25:33.000000 legal_documents_cn-0.0.7/legal_documents_cn.egg-info/SOURCES.txt
--rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)        1 2023-02-20 13:25:33.000000 legal_documents_cn-0.0.7/legal_documents_cn.egg-info/dependency_links.txt
--rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)       24 2023-02-20 13:25:33.000000 legal_documents_cn-0.0.7/legal_documents_cn.egg-info/requires.txt
--rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)       19 2023-02-20 13:25:33.000000 legal_documents_cn-0.0.7/legal_documents_cn.egg-info/top_level.txt
--rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)       38 2023-02-20 13:25:33.955805 legal_documents_cn-0.0.7/setup.cfg
--rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)     1127 2023-02-20 13:24:52.000000 legal_documents_cn-0.0.7/setup.py
+drwxrwxr-x   0 dongyuwu  (1026) dongyuwu  (1026)        0 2023-02-21 06:31:42.296101 legal_documents_cn-0.0.8/
+-rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)     1091 2023-02-20 11:50:48.000000 legal_documents_cn-0.0.8/LICENSE
+-rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)       43 2023-02-20 11:50:48.000000 legal_documents_cn-0.0.8/MANIFEST.in
+-rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)     6713 2023-02-21 06:31:42.295101 legal_documents_cn-0.0.8/PKG-INFO
+-rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)     6289 2023-02-21 06:22:31.000000 legal_documents_cn-0.0.8/README.md
+drwxrwxr-x   0 dongyuwu  (1026) dongyuwu  (1026)        0 2023-02-21 06:31:42.295101 legal_documents_cn-0.0.8/legal_documents_cn/
+-rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)      231 2023-02-20 11:50:48.000000 legal_documents_cn-0.0.8/legal_documents_cn/__init__.py
+-rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)      600 2023-02-20 12:05:45.000000 legal_documents_cn-0.0.8/legal_documents_cn/apitest.py
+-rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)   258368 2023-02-20 11:50:48.000000 legal_documents_cn-0.0.8/legal_documents_cn/criminal_law.csv
+-rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)     7296 2023-02-21 06:29:11.000000 legal_documents_cn-0.0.8/legal_documents_cn/criminal_law_cn.py
+-rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)     8410 2023-02-20 11:50:48.000000 legal_documents_cn-0.0.8/legal_documents_cn/process_data.py
+-rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)     6339 2023-02-20 11:50:48.000000 legal_documents_cn-0.0.8/legal_documents_cn/run_start_api.py
+-rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)     1311 2023-02-20 11:50:48.000000 legal_documents_cn-0.0.8/legal_documents_cn/start_api.py
+drwxrwxr-x   0 dongyuwu  (1026) dongyuwu  (1026)        0 2023-02-21 06:31:42.295101 legal_documents_cn-0.0.8/legal_documents_cn.egg-info/
+-rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)     6713 2023-02-21 06:31:42.000000 legal_documents_cn-0.0.8/legal_documents_cn.egg-info/PKG-INFO
+-rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)      485 2023-02-21 06:31:42.000000 legal_documents_cn-0.0.8/legal_documents_cn.egg-info/SOURCES.txt
+-rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)        1 2023-02-21 06:31:42.000000 legal_documents_cn-0.0.8/legal_documents_cn.egg-info/dependency_links.txt
+-rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)       24 2023-02-21 06:31:42.000000 legal_documents_cn-0.0.8/legal_documents_cn.egg-info/requires.txt
+-rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)       19 2023-02-21 06:31:42.000000 legal_documents_cn-0.0.8/legal_documents_cn.egg-info/top_level.txt
+-rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)       38 2023-02-21 06:31:42.296101 legal_documents_cn-0.0.8/setup.cfg
+-rw-rw-r--   0 dongyuwu  (1026) dongyuwu  (1026)     1127 2023-02-21 06:22:47.000000 legal_documents_cn-0.0.8/setup.py
```

### Comparing `legal_documents_cn-0.0.7/LICENSE` & `legal_documents_cn-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `legal_documents_cn-0.0.7/PKG-INFO` & `legal_documents_cn-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legal_documents_cn
-Version: 0.0.7
+Version: 0.0.8
 Summary: Chinese legal documents, you can get certain legal term content by the code of term and the code of term by its content
 Home-page: https://github.com/
 Author: dongyuwu omnilab
 Author-email: 1558359609@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -93,8 +93,9 @@
 刑法是规定犯罪、刑事责任和刑罚的法律，是掌握政权的统治阶级为了维护本阶级政治上的统治和各阶级经济上的利益，根据自己的意志，规定哪些行为是犯罪并且应当负何种刑事责任 ，并给予犯罪嫌疑人何种刑事处罚的法律规范的总称。
 2020年12月26日，第十三届全国人民代表大会常务委员会第二十四次会议通过刑法修正案(十一)。修改后的刑法自2021年3月1日开始施行。这也是继1997年全面修订刑法后通过的第十一个刑法修正案。
 (1979年7月1日第五届全国人民代表大会第二次会议通过，1997年3月14日第八届全国人民代表大会第五次会议修订。根据1999年12月25日中华人民共和国刑法修正案，2001年8月31日中华人民共和国刑法修正案(二)，2001年12月29日中华人民共和国刑法修正案(三)，2002年12 月28日中华人民共和国刑法修正案(四)，2005年2月28日中华人民共和国刑法修正案(五)，2006年6月29日中华人民共和国刑法修正案(六)，2009年2月28日中华人民共和国刑法修正案(七)修正，根据2009年8月27日《全国人民代表大会常务委员会关于修改部分法律的决定》修正，根据2011年2月25日中华人民共和国刑法修正案(八)修正，根据2015年8月29日第十二届全国人民代表大会常务委员会第十六次会议通过的《刑法修正案(九)》修正，根据2017年11月4日第十二届全国人民代表大会常务委员会第三十次会议通过的《刑法修正案（十）》修正，根据2020年12月26日第十三届全国人民代表大会常务委员会第二十四次会议通过的《刑法修正案（十一）》修正。)
 ——摘自刑法网
 ```
 
 # 更新说明
-- 2023-2-20:v0.0.6 更新了通过款号查询的“第X款”查询功能。
+- 2023-2-21:v0.0.8 更新了款号的切割方式。（之前带有“项”的款号切割方式不准确）
+- 2023-2-20:v0.0.7 更新了通过款号查询的“第X款”查询功能。
```

### Comparing `legal_documents_cn-0.0.7/README.md` & `legal_documents_cn-0.0.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -79,8 +79,9 @@
 刑法是规定犯罪、刑事责任和刑罚的法律，是掌握政权的统治阶级为了维护本阶级政治上的统治和各阶级经济上的利益，根据自己的意志，规定哪些行为是犯罪并且应当负何种刑事责任 ，并给予犯罪嫌疑人何种刑事处罚的法律规范的总称。
 2020年12月26日，第十三届全国人民代表大会常务委员会第二十四次会议通过刑法修正案(十一)。修改后的刑法自2021年3月1日开始施行。这也是继1997年全面修订刑法后通过的第十一个刑法修正案。
 (1979年7月1日第五届全国人民代表大会第二次会议通过，1997年3月14日第八届全国人民代表大会第五次会议修订。根据1999年12月25日中华人民共和国刑法修正案，2001年8月31日中华人民共和国刑法修正案(二)，2001年12月29日中华人民共和国刑法修正案(三)，2002年12 月28日中华人民共和国刑法修正案(四)，2005年2月28日中华人民共和国刑法修正案(五)，2006年6月29日中华人民共和国刑法修正案(六)，2009年2月28日中华人民共和国刑法修正案(七)修正，根据2009年8月27日《全国人民代表大会常务委员会关于修改部分法律的决定》修正，根据2011年2月25日中华人民共和国刑法修正案(八)修正，根据2015年8月29日第十二届全国人民代表大会常务委员会第十六次会议通过的《刑法修正案(九)》修正，根据2017年11月4日第十二届全国人民代表大会常务委员会第三十次会议通过的《刑法修正案（十）》修正，根据2020年12月26日第十三届全国人民代表大会常务委员会第二十四次会议通过的《刑法修正案（十一）》修正。)
 ——摘自刑法网
 ```
 
 # 更新说明
-- 2023-2-20:v0.0.6 更新了通过款号查询的“第X款”查询功能。
+- 2023-2-21:v0.0.8 更新了款号的切割方式。（之前带有“项”的款号切割方式不准确）
+- 2023-2-20:v0.0.7 更新了通过款号查询的“第X款”查询功能。
```

### Comparing `legal_documents_cn-0.0.7/legal_documents_cn/apitest.py` & `legal_documents_cn-0.0.8/legal_documents_cn/apitest.py`

 * *Files identical despite different names*

### Comparing `legal_documents_cn-0.0.7/legal_documents_cn/criminal_law.csv` & `legal_documents_cn-0.0.8/legal_documents_cn/criminal_law.csv`

 * *Files identical despite different names*

### Comparing `legal_documents_cn-0.0.7/legal_documents_cn/criminal_law_cn.py` & `legal_documents_cn-0.0.8/legal_documents_cn/criminal_law_cn.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,18 +39,21 @@
     :param article_code:第X条
     :param para_code:第X款
     :param sub_article_code:之X
     :return:
     """
     content=__getInfoBycode(article_code,sub_article_code)['res']['article_content']
     if para_code:
-        content=content.split('\n')
+        content=content.split('。')
+        content=[item+"。" for item in content[:-1]]+[content[-1]]
+
         if len(content)>=para_code:
             return content[para_code-1]
-        else:raise  Exception("index of para_code out of range 条款编号超出范围,{}/{}".format(para_code,len(content)))
+        else:raise  Exception("index of para_code out of range 条款编号超出范围,article_code:{}, para_code:{}, sub_article_code:{}, total content num:{}".
+                              format(article_code,para_code,sub_article_code,len(content)))
     else:return content
 
 
 def getInfoByArticleName(article_name:str):
     '''
     根据案由（法条名称）获取法条的信息，需要严格写全案由名称，如“交通肇事罪;危险驾驶罪”。若匹配到多个则返回第一个内容
     :param article_name: 案由（法条名称）
```

### Comparing `legal_documents_cn-0.0.7/legal_documents_cn/process_data.py` & `legal_documents_cn-0.0.8/legal_documents_cn/process_data.py`

 * *Files identical despite different names*

### Comparing `legal_documents_cn-0.0.7/legal_documents_cn/run_start_api.py` & `legal_documents_cn-0.0.8/legal_documents_cn/run_start_api.py`

 * *Files identical despite different names*

### Comparing `legal_documents_cn-0.0.7/legal_documents_cn/start_api.py` & `legal_documents_cn-0.0.8/legal_documents_cn/start_api.py`

 * *Files identical despite different names*

### Comparing `legal_documents_cn-0.0.7/legal_documents_cn.egg-info/PKG-INFO` & `legal_documents_cn-0.0.8/legal_documents_cn.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legal-documents-cn
-Version: 0.0.7
+Version: 0.0.8
 Summary: Chinese legal documents, you can get certain legal term content by the code of term and the code of term by its content
 Home-page: https://github.com/
 Author: dongyuwu omnilab
 Author-email: 1558359609@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -93,8 +93,9 @@
 刑法是规定犯罪、刑事责任和刑罚的法律，是掌握政权的统治阶级为了维护本阶级政治上的统治和各阶级经济上的利益，根据自己的意志，规定哪些行为是犯罪并且应当负何种刑事责任 ，并给予犯罪嫌疑人何种刑事处罚的法律规范的总称。
 2020年12月26日，第十三届全国人民代表大会常务委员会第二十四次会议通过刑法修正案(十一)。修改后的刑法自2021年3月1日开始施行。这也是继1997年全面修订刑法后通过的第十一个刑法修正案。
 (1979年7月1日第五届全国人民代表大会第二次会议通过，1997年3月14日第八届全国人民代表大会第五次会议修订。根据1999年12月25日中华人民共和国刑法修正案，2001年8月31日中华人民共和国刑法修正案(二)，2001年12月29日中华人民共和国刑法修正案(三)，2002年12 月28日中华人民共和国刑法修正案(四)，2005年2月28日中华人民共和国刑法修正案(五)，2006年6月29日中华人民共和国刑法修正案(六)，2009年2月28日中华人民共和国刑法修正案(七)修正，根据2009年8月27日《全国人民代表大会常务委员会关于修改部分法律的决定》修正，根据2011年2月25日中华人民共和国刑法修正案(八)修正，根据2015年8月29日第十二届全国人民代表大会常务委员会第十六次会议通过的《刑法修正案(九)》修正，根据2017年11月4日第十二届全国人民代表大会常务委员会第三十次会议通过的《刑法修正案（十）》修正，根据2020年12月26日第十三届全国人民代表大会常务委员会第二十四次会议通过的《刑法修正案（十一）》修正。)
 ——摘自刑法网
 ```
 
 # 更新说明
-- 2023-2-20:v0.0.6 更新了通过款号查询的“第X款”查询功能。
+- 2023-2-21:v0.0.8 更新了款号的切割方式。（之前带有“项”的款号切割方式不准确）
+- 2023-2-20:v0.0.7 更新了通过款号查询的“第X款”查询功能。
```

### Comparing `legal_documents_cn-0.0.7/setup.py` & `legal_documents_cn-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="legal_documents_cn", # Replace with your own username
-    version="0.0.7",
+    version="0.0.8",
     author="dongyuwu omnilab",
     author_email="1558359609@qq.com",
     description="Chinese legal documents, you can get certain legal term content by the code of term and the code of term by its content",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/",
     packages=setuptools.find_packages(),
```

