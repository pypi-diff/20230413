# Comparing `tmp/datedays-2.2.1.tar.gz` & `tmp/datedays-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\datedays-2.2.1.tar", last modified: Fri Oct 14 04:01:14 2022, max compression
+gzip compressed data, was "datedays-2.2.3.tar", last modified: Thu Apr 13 06:24:19 2023, max compression
```

## Comparing `datedays-2.2.1.tar` & `datedays-2.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-10-14 04:01:14.000000 datedays-2.2.1/
-drwxrwxrwx   0        0        0        0 2022-10-14 04:01:14.000000 datedays-2.2.1/datedays/
--rw-rw-rw-   0        0        0    13340 2022-10-11 10:03:09.000000 datedays-2.2.1/datedays/datedays.py
--rw-rw-rw-   0        0        0      839 2022-08-22 08:20:05.000000 datedays-2.2.1/datedays/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-14 04:01:14.000000 datedays-2.2.1/datedays.egg-info/
--rw-rw-rw-   0        0        0        1 2022-10-14 04:01:14.000000 datedays-2.2.1/datedays.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     6452 2022-10-14 04:01:14.000000 datedays-2.2.1/datedays.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       74 2022-10-14 04:01:14.000000 datedays-2.2.1/datedays.egg-info/requires.txt
--rw-rw-rw-   0        0        0      227 2022-10-14 04:01:14.000000 datedays-2.2.1/datedays.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2022-10-14 04:01:14.000000 datedays-2.2.1/datedays.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2022-08-05 07:39:04.000000 datedays-2.2.1/LICENSE
--rw-rw-rw-   0        0        0     6452 2022-10-14 04:01:14.000000 datedays-2.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     5881 2022-10-14 04:01:11.000000 datedays-2.2.1/README.md
--rw-rw-rw-   0        0        0       42 2022-10-14 04:01:14.000000 datedays-2.2.1/setup.cfg
--rw-rw-rw-   0        0        0      753 2022-10-11 09:44:39.000000 datedays-2.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:24:19.727114 datedays-2.2.3/
+-rw-rw-rw-   0        0        0     1086 2022-08-05 07:39:04.000000 datedays-2.2.3/LICENSE
+-rw-rw-rw-   0        0        0     6413 2023-04-13 06:24:19.725119 datedays-2.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5883 2023-04-13 05:52:35.000000 datedays-2.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 06:24:19.685855 datedays-2.2.3/datedays/
+-rw-rw-rw-   0        0        0      847 2023-04-13 05:57:23.000000 datedays-2.2.3/datedays/__init__.py
+-rw-rw-rw-   0        0        0    14571 2023-04-13 06:24:01.000000 datedays-2.2.3/datedays/datedays.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:24:19.723124 datedays-2.2.3/datedays.egg-info/
+-rw-rw-rw-   0        0        0     6413 2023-04-13 06:24:19.000000 datedays-2.2.3/datedays.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-04-13 06:24:19.000000 datedays-2.2.3/datedays.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 06:24:19.000000 datedays-2.2.3/datedays.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-04-13 06:24:19.000000 datedays-2.2.3/datedays.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-13 06:24:19.000000 datedays-2.2.3/datedays.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 06:24:19.728111 datedays-2.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      753 2023-04-13 05:55:43.000000 datedays-2.2.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `datedays-2.2.1/datedays/datedays.py` & `datedays-2.2.3/datedays/datedays.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,16 +23,19 @@
 """
 __email__ = "chinalzge@gmail.com"
 __author__ = 'liang1024'
 
 import base64
 import calendar
 import datetime
+import logging
+import os
 import random
 import string
+import sys
 import time
 import traceback
 import uuid
 from datetime import date
 from urllib.parse import urlencode, quote, unquote
 
 import openpyxl
@@ -579,14 +582,59 @@
     if headers_string:
         for h in [h if len(h) == 2 else None for h in [h.split(':', 1) for h in headers_string.splitlines()]]:
             if h:
                 _dict[h[0].strip()] = h[1].strip()
     return _dict
 
 
+def logger(txt=None, base_name=None, file_name='log.txt', log_base=None,
+           fmt=f'%(asctime)s - %(name)s - %(levelname)s - %(message)s',
+           mode='a',
+           encoding='utf-8'):
+    '''logger'''
+
+    if not base_name:
+        base_name = os.path.basename(sys.argv[0]).split('.')[0]
+
+    if not log_base:
+        arg = sys.argv[0]
+        log_base = arg[:arg.rfind('/')]
+        # log_base = arg[:arg[:arg.rfind('/')].rfind('/')]
+
+    date_dir = f"{log_base}/log/{base_name}/{datetime.date.today().strftime('%Y-%m-%d')}"
+
+    if not os.path.exists(date_dir):
+        print(f'logger create dir:{date_dir}')
+        os.makedirs(date_dir)
+
+    logger = logging.getLogger(base_name)
+
+    formatter = logging.Formatter(fmt)
+
+    # filehandler
+    fh = logging.FileHandler(f'{date_dir}/{file_name}', mode=mode, encoding=encoding)
+    fh.setFormatter(formatter)
+
+    # consolehandler
+    ch = logging.StreamHandler()
+    ch.setFormatter(formatter)
+
+    # add handler
+    logger.addHandler(fh)
+    logger.addHandler(ch)
+
+    # set level=debug
+    logger.setLevel(logging.DEBUG)
+
+    if txt:
+        logger.debug(txt)
+
+    return logger
+
+
 if __name__ == '__main__':
     print(headers2dict('''
     Accept: application/json, text/javascript, */*; q=0.01
     Accept-Encoding: gzip, deflate, br
     Accept-Language: zh-CN,zh;q=0.9
     Cache-Control: no-cache
     Connection: keep-alive
```

### Comparing `datedays-2.2.1/datedays/__init__.py` & `datedays-2.2.3/datedays/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 
 name = "datedays"
 
 from .datedays import getnow, gettomorrow, getyesterday, getdays, getasctime, getnowtimestamp, \
     gettodaydays, getnextdays, getstr2timestamp, getcurrent_days, getnext_days, excel_write_openpyxl, \
     excel_read_openpyxl, excel_read_xlrd, md2, md5, sha1, sha2_224, sha2_256, sha2_384, sha2_512, sha3_224, sha3_256, \
     sha3_384, sha3_512, encrypt_smallfile, encrypt_bigfile, sleep, getuuid, getrandompassword, gettimestamp2str, \
-    base64_encode, base64_decode, urlencodes, urldecodes, getstartend, headers2dict
+    base64_encode, base64_decode, urlencodes, urldecodes, getstartend, headers2dict, logger
```

### Comparing `datedays-2.2.1/datedays.egg-info/PKG-INFO` & `datedays-2.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: datedays
-Version: 2.2.1
+Version: 2.2.3
 Summary: Python Date Tools
 Home-page: https://github.com/liang1024/datedays
 Author: liang1024
 Author-email: chinalzge@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # datedays
@@ -71,17 +69,17 @@
 ## 1. Get common date data
 
 Method | description | return result | parameter<a id = "datadays"></a>
 :---: | :---:| :---:| :---:
 getnow() | get today's date | for example: 2022-08-16 17:56:17|
 gettomorrow() | tomorrow | 2022-08-17 | select the next day (just pass in the number you want)
 getyesterday() | yesterday | 2022-08-15 | select the last day (just pass in the desired number)
-getdays() | default date set within three months |... (test printing is recommended) | number = number of months you want
+getdays() | default date list within three months |... (test printing is recommended) | number = number of months you want
 getnowtimestamp() | get the current timestamp | 1660644568238 | default milliseconds (optional seconds, milliseconds, microseconds)
-gettodaydays() | get the set of remaining days of this month by default |... (it is recommended to test and print) | you can specify a day of a month to get the remaining days of the month
+gettodaydays() | get the list of remaining days of this month by default |... (it is recommended to test and print) | you can specify a day of a month to get the remaining days of the month
 getnextdays() | get the total number of days of the next month by default |... (test printing is recommended) | you can specify the month and the number of months
 getstr2timestamp() | date string to timestamp |... (test printing is recommended) | parameter 1: date, parameter 2: date format
 gettimestamp2str() | timestamp to date string |... (test printing is recommended) | parameter 1:timestamp
 getstartend() | get interval days or days list |... (test printing is recommended) | parameter 1:start date, parameter 2:end date parameter 3:return list
 headers2dict() | copy headers string convert dict |... (test printing is recommended) | parameter 1: headers string
 
 ## 2. Operate excel report
@@ -137,9 +135,7 @@
 
 ```
 ['2022-08-11', '2022-08-12', '2022-08-13', '2022-08-14', '2022-08-15', '2022-08-16', '2022-08-17', '2022-08-18']
 ```
 
 I hope it can help you!
 
-
-
```

### Comparing `datedays-2.2.1/LICENSE` & `datedays-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datedays-2.2.1/PKG-INFO` & `datedays-2.2.3/datedays.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: datedays
-Version: 2.2.1
+Version: 2.2.3
 Summary: Python Date Tools
 Home-page: https://github.com/liang1024/datedays
 Author: liang1024
 Author-email: chinalzge@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # datedays
@@ -71,17 +69,17 @@
 ## 1. Get common date data
 
 Method | description | return result | parameter<a id = "datadays"></a>
 :---: | :---:| :---:| :---:
 getnow() | get today's date | for example: 2022-08-16 17:56:17|
 gettomorrow() | tomorrow | 2022-08-17 | select the next day (just pass in the number you want)
 getyesterday() | yesterday | 2022-08-15 | select the last day (just pass in the desired number)
-getdays() | default date set within three months |... (test printing is recommended) | number = number of months you want
+getdays() | default date list within three months |... (test printing is recommended) | number = number of months you want
 getnowtimestamp() | get the current timestamp | 1660644568238 | default milliseconds (optional seconds, milliseconds, microseconds)
-gettodaydays() | get the set of remaining days of this month by default |... (it is recommended to test and print) | you can specify a day of a month to get the remaining days of the month
+gettodaydays() | get the list of remaining days of this month by default |... (it is recommended to test and print) | you can specify a day of a month to get the remaining days of the month
 getnextdays() | get the total number of days of the next month by default |... (test printing is recommended) | you can specify the month and the number of months
 getstr2timestamp() | date string to timestamp |... (test printing is recommended) | parameter 1: date, parameter 2: date format
 gettimestamp2str() | timestamp to date string |... (test printing is recommended) | parameter 1:timestamp
 getstartend() | get interval days or days list |... (test printing is recommended) | parameter 1:start date, parameter 2:end date parameter 3:return list
 headers2dict() | copy headers string convert dict |... (test printing is recommended) | parameter 1: headers string
 
 ## 2. Operate excel report
@@ -137,9 +135,7 @@
 
 ```
 ['2022-08-11', '2022-08-12', '2022-08-13', '2022-08-14', '2022-08-15', '2022-08-16', '2022-08-17', '2022-08-18']
 ```
 
 I hope it can help you!
 
-
-
```

### Comparing `datedays-2.2.1/README.md` & `datedays-2.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -56,17 +56,17 @@
 ## 1. Get common date data
 
 Method | description | return result | parameter<a id = "datadays"></a>
 :---: | :---:| :---:| :---:
 getnow() | get today's date | for example: 2022-08-16 17:56:17|
 gettomorrow() | tomorrow | 2022-08-17 | select the next day (just pass in the number you want)
 getyesterday() | yesterday | 2022-08-15 | select the last day (just pass in the desired number)
-getdays() | default date set within three months |... (test printing is recommended) | number = number of months you want
+getdays() | default date list within three months |... (test printing is recommended) | number = number of months you want
 getnowtimestamp() | get the current timestamp | 1660644568238 | default milliseconds (optional seconds, milliseconds, microseconds)
-gettodaydays() | get the set of remaining days of this month by default |... (it is recommended to test and print) | you can specify a day of a month to get the remaining days of the month
+gettodaydays() | get the list of remaining days of this month by default |... (it is recommended to test and print) | you can specify a day of a month to get the remaining days of the month
 getnextdays() | get the total number of days of the next month by default |... (test printing is recommended) | you can specify the month and the number of months
 getstr2timestamp() | date string to timestamp |... (test printing is recommended) | parameter 1: date, parameter 2: date format
 gettimestamp2str() | timestamp to date string |... (test printing is recommended) | parameter 1:timestamp
 getstartend() | get interval days or days list |... (test printing is recommended) | parameter 1:start date, parameter 2:end date parameter 3:return list
 headers2dict() | copy headers string convert dict |... (test printing is recommended) | parameter 1: headers string
 
 ## 2. Operate excel report
```

### Comparing `datedays-2.2.1/setup.py` & `datedays-2.2.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 requires = [
-    "openpyxl==3.0.10",
-    "xlrd==2.0.1",
-    "pycryptodomex==3.15.0",
-    "python-dateutil==2.8.2",
+    "openpyxl>=3.0.10",
+    "xlrd>=2.0.1",
+    "pycryptodomex>=3.15.0",
+    "python-dateutil>=2.8.2",
 ]
 with open("README.md", "r") as f:
     readme = f.read()
 
 setuptools.setup(
     name="datedays",
-    version="2.2.1",
+    version="2.2.3",
     author="liang1024",
     author_email="chinalzge@gmail.com",
     description="Python Date Tools",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/liang1024/datedays",
     packages=setuptools.find_packages(),
```

