# Comparing `tmp/ExceptNotifier-0.1.0.tar.gz` & `tmp/ExceptNotifier-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExceptNotifier-0.1.0.tar", last modified: Thu Apr 13 17:10:52 2023, max compression
+gzip compressed data, was "ExceptNotifier-0.1.1.tar", last modified: Thu Apr 13 17:12:27 2023, max compression
```

## Comparing `ExceptNotifier-0.1.0.tar` & `ExceptNotifier-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 17:10:52.958339 ExceptNotifier-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-04-13 17:10:52.939014 ExceptNotifier-0.1.0/ExceptNotifier/
--rw-rw-rw-   0        0        0      251 2023-04-13 17:10:35.000000 ExceptNotifier-0.1.0/ExceptNotifier/__init__.py
--rw-rw-rw-   0        0        0     1489 2023-04-13 17:10:33.000000 ExceptNotifier-0.1.0/ExceptNotifier/__main__.py
--rw-rw-rw-   0        0        0     4439 2023-04-13 17:09:44.000000 ExceptNotifier-0.1.0/ExceptNotifier/mail_sender.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:10:52.955119 ExceptNotifier-0.1.0/ExceptNotifier.egg-info/
--rw-rw-rw-   0        0        0     3422 2023-04-13 17:10:52.000000 ExceptNotifier-0.1.0/ExceptNotifier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-04-13 17:10:52.000000 ExceptNotifier-0.1.0/ExceptNotifier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 17:10:52.000000 ExceptNotifier-0.1.0/ExceptNotifier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-13 17:10:52.000000 ExceptNotifier-0.1.0/ExceptNotifier.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-04-13 17:10:52.000000 ExceptNotifier-0.1.0/ExceptNotifier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 ExceptNotifier-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3422 2023-04-13 17:10:52.957119 ExceptNotifier-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2259 2023-04-13 17:10:10.000000 ExceptNotifier-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 17:10:52.958339 ExceptNotifier-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1981 2023-04-13 17:10:38.000000 ExceptNotifier-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:12:27.635241 ExceptNotifier-0.1.1/
+drwxrwxrwx   0        0        0        0 2023-04-13 17:12:27.618622 ExceptNotifier-0.1.1/ExceptNotifier/
+-rw-rw-rw-   0        0        0      251 2023-04-13 17:11:59.000000 ExceptNotifier-0.1.1/ExceptNotifier/__init__.py
+-rw-rw-rw-   0        0        0     1489 2023-04-13 17:10:33.000000 ExceptNotifier-0.1.1/ExceptNotifier/__main__.py
+-rw-rw-rw-   0        0        0     4439 2023-04-13 17:09:44.000000 ExceptNotifier-0.1.1/ExceptNotifier/mail_sender.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:12:27.632732 ExceptNotifier-0.1.1/ExceptNotifier.egg-info/
+-rw-rw-rw-   0        0        0     3401 2023-04-13 17:12:27.000000 ExceptNotifier-0.1.1/ExceptNotifier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-04-13 17:12:27.000000 ExceptNotifier-0.1.1/ExceptNotifier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 17:12:27.000000 ExceptNotifier-0.1.1/ExceptNotifier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-13 17:12:27.000000 ExceptNotifier-0.1.1/ExceptNotifier.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-04-13 17:12:27.000000 ExceptNotifier-0.1.1/ExceptNotifier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 ExceptNotifier-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3401 2023-04-13 17:12:27.634231 ExceptNotifier-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2238 2023-04-13 17:11:44.000000 ExceptNotifier-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 17:12:27.636241 ExceptNotifier-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1981 2023-04-13 17:11:56.000000 ExceptNotifier-0.1.1/setup.py
```

### Comparing `ExceptNotifier-0.1.0/ExceptNotifier/__main__.py` & `ExceptNotifier-0.1.1/ExceptNotifier/__main__.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.0/ExceptNotifier/mail_sender.py` & `ExceptNotifier-0.1.1/ExceptNotifier/mail_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.0/ExceptNotifier.egg-info/PKG-INFO` & `ExceptNotifier-0.1.1/ExceptNotifier.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExceptNotifier
-Version: 0.1.0
+Version: 0.1.1
 Summary: With Python's try-except statement, experience a significantly more flexible way to receive notifications.
 Home-page: https://github.com/dsdanielpark/ExceptNotifier
 Author: parkminwoo
 Author-email: parkminwoo1991@gmail.com
 Keywords: Exception,Python,Python Exception Alarm,Error notifications,Customizable notifications,Traceback management,Single line alarm
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
@@ -18,38 +18,38 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Python: ExceptionNotifier
+# Python: ExceptNotifier
 With Python's try-except statement, experience a significantly more flexible way to receive notifications. You can receive alerts through various messaging platforms such as email, Slack, and Discord. This package offers an extensive range of notification options to suit your needs.
 
-Python package [`ExceptionNotifier`](https://github.com/dsdanielpark/ExceptionNotifier) can give a single line alarm with an error message, whereas [`knockknock`](https://github.com/huggingface/knockknock) gives a process ending alarm with decorator and cli.
+Python package [`ExceptNotifier`](https://github.com/dsdanielpark/ExceptNotifier) can give a single line alarm with an error message, whereas [`knockknock`](https://github.com/huggingface/knockknock) gives a process ending alarm with decorator and cli.
 
 <br>
 
 # Quick Start
-ExceptionNotifier installation
+ExceptNotifier installation
 ```
-pip insall ExceptionNotifier
+pip insall ExceptNotifier
 ```
 
 
 <br>
 
 # Features
 ### `Mail`
 In the except statement, an email is sent along with the error message. Additionally, you can send emails from any desired line. <br><br>
 a. Log in with the sender's email ID. <br>
 b. Obtain an app password for sending Google Mail at the following [link](https://myaccount.google.com/u/3/apppasswords?utm_source=google-account&utm_medium=myaccountsecurity&utm_campaign=tsv-settings&rapt=AEjHL4N2bMRWO46VaMp_jP06zQK14BWNPv66l2o59iJ99CkO8BjYnmoRUe9dtSchkkbubHZMUhevkAnwVJRHb9ygO3afispNlw). 
 
 ```python
-from ExceptionNotifier import ExceptMail, SuccessMail, SendMail
+from ExceptNotifier import ExceptMail, SuccessMail, SendMail
 sys.excepthook = ExceptMail.__call__
 
 try:
     main() # Your Code Here
     SuccessMail().__call__()    # No Exception -> Send Success mail.
 except ExceptMail:           # Exception -> Send Fail mail.
     pass
@@ -58,15 +58,15 @@
 ```
 
 <details>
 <summary> See Example...</summary>
 
 ```python
 import sys
-from ExceptionNotifier import ExceptMail, SuccessMail
+from ExceptNotifier import ExceptMail, SuccessMail
 
 # 01. Set variable.
 global gmail_receiver, gmail_sender, gmail_app_password_of_sender, SendMail
 gmail_receiver = 'parkminwoo1991@gmail.com'
 gmail_sender = 'heydudenotice@gmail.com'
 gmail_app_password_of_sender = 'xxxxxxxxxxx'
 sys.excepthook = ExceptMail.__call__
```

### Comparing `ExceptNotifier-0.1.0/LICENSE` & `ExceptNotifier-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.0/PKG-INFO` & `ExceptNotifier-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExceptNotifier
-Version: 0.1.0
+Version: 0.1.1
 Summary: With Python's try-except statement, experience a significantly more flexible way to receive notifications.
 Home-page: https://github.com/dsdanielpark/ExceptNotifier
 Author: parkminwoo
 Author-email: parkminwoo1991@gmail.com
 Keywords: Exception,Python,Python Exception Alarm,Error notifications,Customizable notifications,Traceback management,Single line alarm
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
@@ -18,38 +18,38 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Python: ExceptionNotifier
+# Python: ExceptNotifier
 With Python's try-except statement, experience a significantly more flexible way to receive notifications. You can receive alerts through various messaging platforms such as email, Slack, and Discord. This package offers an extensive range of notification options to suit your needs.
 
-Python package [`ExceptionNotifier`](https://github.com/dsdanielpark/ExceptionNotifier) can give a single line alarm with an error message, whereas [`knockknock`](https://github.com/huggingface/knockknock) gives a process ending alarm with decorator and cli.
+Python package [`ExceptNotifier`](https://github.com/dsdanielpark/ExceptNotifier) can give a single line alarm with an error message, whereas [`knockknock`](https://github.com/huggingface/knockknock) gives a process ending alarm with decorator and cli.
 
 <br>
 
 # Quick Start
-ExceptionNotifier installation
+ExceptNotifier installation
 ```
-pip insall ExceptionNotifier
+pip insall ExceptNotifier
 ```
 
 
 <br>
 
 # Features
 ### `Mail`
 In the except statement, an email is sent along with the error message. Additionally, you can send emails from any desired line. <br><br>
 a. Log in with the sender's email ID. <br>
 b. Obtain an app password for sending Google Mail at the following [link](https://myaccount.google.com/u/3/apppasswords?utm_source=google-account&utm_medium=myaccountsecurity&utm_campaign=tsv-settings&rapt=AEjHL4N2bMRWO46VaMp_jP06zQK14BWNPv66l2o59iJ99CkO8BjYnmoRUe9dtSchkkbubHZMUhevkAnwVJRHb9ygO3afispNlw). 
 
 ```python
-from ExceptionNotifier import ExceptMail, SuccessMail, SendMail
+from ExceptNotifier import ExceptMail, SuccessMail, SendMail
 sys.excepthook = ExceptMail.__call__
 
 try:
     main() # Your Code Here
     SuccessMail().__call__()    # No Exception -> Send Success mail.
 except ExceptMail:           # Exception -> Send Fail mail.
     pass
@@ -58,15 +58,15 @@
 ```
 
 <details>
 <summary> See Example...</summary>
 
 ```python
 import sys
-from ExceptionNotifier import ExceptMail, SuccessMail
+from ExceptNotifier import ExceptMail, SuccessMail
 
 # 01. Set variable.
 global gmail_receiver, gmail_sender, gmail_app_password_of_sender, SendMail
 gmail_receiver = 'parkminwoo1991@gmail.com'
 gmail_sender = 'heydudenotice@gmail.com'
 gmail_app_password_of_sender = 'xxxxxxxxxxx'
 sys.excepthook = ExceptMail.__call__
```

### Comparing `ExceptNotifier-0.1.0/README.md` & `ExceptNotifier-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# Python: ExceptionNotifier
+# Python: ExceptNotifier
 With Python's try-except statement, experience a significantly more flexible way to receive notifications. You can receive alerts through various messaging platforms such as email, Slack, and Discord. This package offers an extensive range of notification options to suit your needs.
 
-Python package [`ExceptionNotifier`](https://github.com/dsdanielpark/ExceptionNotifier) can give a single line alarm with an error message, whereas [`knockknock`](https://github.com/huggingface/knockknock) gives a process ending alarm with decorator and cli.
+Python package [`ExceptNotifier`](https://github.com/dsdanielpark/ExceptNotifier) can give a single line alarm with an error message, whereas [`knockknock`](https://github.com/huggingface/knockknock) gives a process ending alarm with decorator and cli.
 
 <br>
 
 # Quick Start
-ExceptionNotifier installation
+ExceptNotifier installation
 ```
-pip insall ExceptionNotifier
+pip insall ExceptNotifier
 ```
 
 
 <br>
 
 # Features
 ### `Mail`
 In the except statement, an email is sent along with the error message. Additionally, you can send emails from any desired line. <br><br>
 a. Log in with the sender's email ID. <br>
 b. Obtain an app password for sending Google Mail at the following [link](https://myaccount.google.com/u/3/apppasswords?utm_source=google-account&utm_medium=myaccountsecurity&utm_campaign=tsv-settings&rapt=AEjHL4N2bMRWO46VaMp_jP06zQK14BWNPv66l2o59iJ99CkO8BjYnmoRUe9dtSchkkbubHZMUhevkAnwVJRHb9ygO3afispNlw). 
 
 ```python
-from ExceptionNotifier import ExceptMail, SuccessMail, SendMail
+from ExceptNotifier import ExceptMail, SuccessMail, SendMail
 sys.excepthook = ExceptMail.__call__
 
 try:
     main() # Your Code Here
     SuccessMail().__call__()    # No Exception -> Send Success mail.
 except ExceptMail:           # Exception -> Send Fail mail.
     pass
@@ -34,15 +34,15 @@
 ```
 
 <details>
 <summary> See Example...</summary>
 
 ```python
 import sys
-from ExceptionNotifier import ExceptMail, SuccessMail
+from ExceptNotifier import ExceptMail, SuccessMail
 
 # 01. Set variable.
 global gmail_receiver, gmail_sender, gmail_app_password_of_sender, SendMail
 gmail_receiver = 'parkminwoo1991@gmail.com'
 gmail_sender = 'heydudenotice@gmail.com'
 gmail_app_password_of_sender = 'xxxxxxxxxxx'
 sys.excepthook = ExceptMail.__call__
```

### Comparing `ExceptNotifier-0.1.0/setup.py` & `ExceptNotifier-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 version = get_version()
 
 
 setup(
     name="ExceptNotifier",
-    version="0.1.0",
+    version="0.1.1",
     author="parkminwoo",
     author_email="parkminwoo1991@gmail.com",
     description="With Python's try-except statement, experience a significantly more flexible way to receive notifications.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/dsdanielpark/ExceptNotifier",
     packages=find_packages(exclude=[]),
```

