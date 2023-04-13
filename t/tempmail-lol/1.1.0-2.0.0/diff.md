# Comparing `tmp/tempmail-lol-1.1.0.tar.gz` & `tmp/tempmail-lol-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tempmail-lol-1.1.0.tar", last modified: Fri Aug  5 05:58:33 2022, max compression
+gzip compressed data, was "tempmail-lol-2.0.0.tar", last modified: Thu Apr 13 20:20:52 2023, max compression
```

## Comparing `tempmail-lol-1.1.0.tar` & `tempmail-lol-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-08-05 05:58:33.652938 tempmail-lol-1.1.0/
--rw-rw-rw-   0        0        0      530 2022-08-05 05:58:33.651961 tempmail-lol-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1182 2022-08-05 05:13:40.000000 tempmail-lol-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2022-08-05 05:58:33.631466 tempmail-lol-1.1.0/TempMail/
--rw-rw-rw-   0        0        0     1107 2022-08-05 05:13:40.000000 tempmail-lol-1.1.0/TempMail/Email.py
--rw-rw-rw-   0        0        0      514 2022-08-05 05:13:40.000000 tempmail-lol-1.1.0/TempMail/Inbox.py
--rw-rw-rw-   0        0        0     2269 2022-08-05 05:36:31.000000 tempmail-lol-1.1.0/TempMail/TempMail.py
--rw-rw-rw-   0        0        0       38 2022-08-05 05:13:40.000000 tempmail-lol-1.1.0/TempMail/__init__.py
--rw-rw-rw-   0        0        0       42 2022-08-05 05:58:33.652938 tempmail-lol-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      945 2022-08-05 05:24:30.000000 tempmail-lol-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-05 05:58:33.650986 tempmail-lol-1.1.0/tempmail_lol.egg-info/
--rw-rw-rw-   0        0        0      530 2022-08-05 05:58:33.000000 tempmail-lol-1.1.0/tempmail_lol.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2022-08-05 05:58:33.000000 tempmail-lol-1.1.0/tempmail_lol.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-05 05:58:33.000000 tempmail-lol-1.1.0/tempmail_lol.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-08-05 05:58:33.000000 tempmail-lol-1.1.0/tempmail_lol.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-08-05 05:58:33.000000 tempmail-lol-1.1.0/tempmail_lol.egg-info/top_level.txt
+drwxrwxrwx   0 zuki      (1000) zuki      (1000)        0 2023-04-13 20:20:52.178306 tempmail-lol-2.0.0/
+-rwxrwxrwx   0 zuki      (1000) zuki      (1000)      608 2023-04-13 20:20:52.174515 tempmail-lol-2.0.0/PKG-INFO
+-rwxrwxrwx   0 zuki      (1000) zuki      (1000)     1778 2023-04-13 20:20:18.000000 tempmail-lol-2.0.0/README.md
+drwxrwxrwx   0 zuki      (1000) zuki      (1000)        0 2023-04-13 20:20:52.041093 tempmail-lol-2.0.0/TempMail/
+-rwxrwxrwx   0 zuki      (1000) zuki      (1000)     1106 2023-04-13 20:20:18.000000 tempmail-lol-2.0.0/TempMail/Email.py
+-rwxrwxrwx   0 zuki      (1000) zuki      (1000)      514 2023-04-13 20:20:18.000000 tempmail-lol-2.0.0/TempMail/Inbox.py
+-rwxrwxrwx   0 zuki      (1000) zuki      (1000)     4887 2023-04-13 20:20:18.000000 tempmail-lol-2.0.0/TempMail/TempMail.py
+-rwxrwxrwx   0 zuki      (1000) zuki      (1000)       38 2023-04-13 20:20:18.000000 tempmail-lol-2.0.0/TempMail/__init__.py
+-rwxrwxrwx   0 zuki      (1000) zuki      (1000)       38 2023-04-13 20:20:52.179307 tempmail-lol-2.0.0/setup.cfg
+-rwxrwxrwx   0 zuki      (1000) zuki      (1000)      989 2023-04-13 20:20:18.000000 tempmail-lol-2.0.0/setup.py
+drwxrwxrwx   0 zuki      (1000) zuki      (1000)        0 2023-04-13 20:20:52.150928 tempmail-lol-2.0.0/tempmail_lol.egg-info/
+-rwxrwxrwx   0 zuki      (1000) zuki      (1000)      608 2023-04-13 20:20:51.000000 tempmail-lol-2.0.0/tempmail_lol.egg-info/PKG-INFO
+-rwxrwxrwx   0 zuki      (1000) zuki      (1000)      275 2023-04-13 20:20:51.000000 tempmail-lol-2.0.0/tempmail_lol.egg-info/SOURCES.txt
+-rwxrwxrwx   0 zuki      (1000) zuki      (1000)        1 2023-04-13 20:20:51.000000 tempmail-lol-2.0.0/tempmail_lol.egg-info/dependency_links.txt
+-rwxrwxrwx   0 zuki      (1000) zuki      (1000)        9 2023-04-13 20:20:51.000000 tempmail-lol-2.0.0/tempmail_lol.egg-info/requires.txt
+-rwxrwxrwx   0 zuki      (1000) zuki      (1000)        9 2023-04-13 20:20:51.000000 tempmail-lol-2.0.0/tempmail_lol.egg-info/top_level.txt
```

### Comparing `tempmail-lol-1.1.0/TempMail/Email.py` & `tempmail-lol-2.0.0/TempMail/Email.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Email class is used to store the email data which consists of 
+Email class is used to store the email data which consists of
 the sender, recipient, subject, body, html and date
 """
 
 class Email:
     def __init__(self, sender, recipient, subject, body, html, date):
         #make the propertys immutable using @property
         self._sender = sender
```

### Comparing `tempmail-lol-1.1.0/TempMail/Inbox.py` & `tempmail-lol-2.0.0/TempMail/Inbox.py`

 * *Files identical despite different names*

### Comparing `tempmail-lol-1.1.0/setup.py` & `tempmail-lol-2.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
-        long_description = "\n" + fh.read()
+    long_description = "\n" + fh.read()
 
 setup(name='tempmail-lol',
-        version='1.1.0',
-        description='A Python API for TempMail',
-        author='Alex Torres',
-        author_email='cloudbotsedc@gmail.com',
-        url='https://github.com/tempmail-lol/api-python',
-        packages=find_packages(),
-        install_requires=['requests'],
-        keywords=['python', 'video', 'api', 'tempmail'],
-        classifiers=[
-        "Development Status :: 1 - Planning",
-        "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3",
-        "Operating System :: Unix",
-        "Operating System :: MacOS :: MacOS X",
-        "Operating System :: Microsoft :: Windows",
-        ]
-        )
+      version='2.0.0',
+      description='A Python API for TempMail',
+      author='Alex Torres, Alexander Epolite',
+      author_email='cloudbotsedc@gmail.com',
+      url='https://github.com/tempmail-lol/api-python',
+      packages=find_packages(),
+      install_requires=['requests'],
+      keywords=['tempmail', 'api', 'lol', 'tempmail-lol', 'tempmail.lol', 'email', 'free'],
+      classifiers=[
+          "Development Status :: 1 - Planning",
+          "Intended Audience :: Developers",
+          "Programming Language :: Python :: 3",
+          "Operating System :: Unix",
+          "Operating System :: MacOS :: MacOS X",
+          "Operating System :: Microsoft :: Windows",
+      ]
+      )
```

