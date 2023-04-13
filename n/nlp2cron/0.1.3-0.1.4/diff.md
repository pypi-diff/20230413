# Comparing `tmp/nlp2cron-0.1.3.tar.gz` & `tmp/nlp2cron-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlp2cron-0.1.3.tar", max compression
+gzip compressed data, was "nlp2cron-0.1.4.tar", max compression
```

## Comparing `nlp2cron-0.1.3.tar` & `nlp2cron-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      373 2023-04-11 03:35:14.927410 nlp2cron-0.1.3/README.md
--rw-r--r--   0        0        0    10579 2023-04-11 07:08:44.515197 nlp2cron-0.1.3/nlp2cron.py
--rw-r--r--   0        0        0      306 2023-04-11 07:10:56.505538 nlp2cron-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 nlp2cron-0.1.3/setup.py
--rw-r--r--   0        0        0      820 1970-01-01 00:00:00.000000 nlp2cron-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      373 2023-04-11 03:35:14.927410 nlp2cron-0.1.4/README.md
+-rw-r--r--   0        0        0    10604 2023-04-13 06:09:37.837527 nlp2cron-0.1.4/nlp2cron.py
+-rw-r--r--   0        0        0      306 2023-04-13 06:10:01.047857 nlp2cron-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 nlp2cron-0.1.4/setup.py
+-rw-r--r--   0        0        0      820 1970-01-01 00:00:00.000000 nlp2cron-0.1.4/PKG-INFO
```

### Comparing `nlp2cron-0.1.3/nlp2cron.py` & `nlp2cron-0.1.4/nlp2cron.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     """
     2023-04-07 14:03:00
     quqinglei@icloud.com
     只有在句子中包含每日|天|周|月 才会触发，太笼统的不触发
     """
     def __init__(self, message):
         message = cn2an.transform(message, "cn2an")
-        message = message.replace(' ', '').replace('\t', '').replace('到', '-')
+        message = message.replace(' ', '').replace('\t', '').replace('到', '-').replace('星期', '周')
         self.message = message
         self.freq = 'T'
         self.dict = {"month": '*', "day": '*', "hour": '9', "min": "0", "week": "*"}
         self.now = datetime.now()
         self.a1 = re.findall(r'(每)(天|周|日|月|个月)', self.message)
         self.a2 = re.findall(r'(定时)|(提醒)|(记得)|(别忘)|(叫)|(要准备)|(提前)|(要去)|(下周)|(本周)|(后天)|(下个月)|(小时)', self.message)
         self.extract_freq()
```

### Comparing `nlp2cron-0.1.3/setup.py` & `nlp2cron-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 modules = \
 ['nlp2cron']
 install_requires = \
 ['cn2an>=0.5.19,<0.6.0']
 
 setup_kwargs = {
     'name': 'nlp2cron',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'Nature language to cron',
     'long_description': '## 中文自然语言转CRON\n\npip install nlp2cron\n\n```python\nfrom nlp2cron import nlp2cron\ncron = nlp2cron("每天10点25分叫我去买菜")\n\n```\n\n你会得到一个`cron`表达式. 目前代码写的有点乱, 但只要不太随意的自然语言都可以解决\n代码里面有一些例子, 详细看代码啦. 代码写的比较随意, 如果要求高请不要用啦.\n\n',
     'author': 'quqinglei',
     'author_email': 'quqinglei@icloud.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `nlp2cron-0.1.3/PKG-INFO` & `nlp2cron-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp2cron
-Version: 0.1.3
+Version: 0.1.4
 Summary: Nature language to cron
 Author: quqinglei
 Author-email: quqinglei@icloud.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

