# Comparing `tmp/strato_dyndns-2.3.1.tar.gz` & `tmp/strato_dyndns-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strato_dyndns-2.3.1.tar", last modified: Tue Jun 14 22:30:42 2022, max compression
+gzip compressed data, was "strato_dyndns-2.3.2.tar", last modified: Thu Apr 13 11:24:13 2023, max compression
```

## Comparing `strato_dyndns-2.3.1.tar` & `strato_dyndns-2.3.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-14 22:30:42.756977 strato_dyndns-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)    35148 2022-06-14 22:30:35.000000 strato_dyndns-2.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3792 2022-06-14 22:30:42.756977 strato_dyndns-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3255 2022-06-14 22:30:35.000000 strato_dyndns-2.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-06-14 22:30:42.756977 strato_dyndns-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      890 2022-06-14 22:30:35.000000 strato_dyndns-2.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-14 22:30:42.752977 strato_dyndns-2.3.1/strato_dyndns/
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-06-14 22:30:35.000000 strato_dyndns-2.3.1/strato_dyndns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-14 22:30:42.752977 strato_dyndns-2.3.1/strato_dyndns/clients/
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-14 22:30:35.000000 strato_dyndns-2.3.1/strato_dyndns/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1389 2022-06-14 22:30:35.000000 strato_dyndns-2.3.1/strato_dyndns/clients/connection_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     3057 2022-06-14 22:30:35.000000 strato_dyndns-2.3.1/strato_dyndns/clients/dyndns_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     4102 2022-06-14 22:30:35.000000 strato_dyndns-2.3.1/strato_dyndns/clients/namecheap_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     4772 2022-06-14 22:30:35.000000 strato_dyndns-2.3.1/strato_dyndns/clients/strato_client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-14 22:30:42.756977 strato_dyndns-2.3.1/strato_dyndns/lib/
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-06-14 22:30:35.000000 strato_dyndns-2.3.1/strato_dyndns/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4457 2022-06-14 22:30:35.000000 strato_dyndns-2.3.1/strato_dyndns/lib/args_validator.py
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-06-14 22:30:35.000000 strato_dyndns-2.3.1/strato_dyndns/lib/file_operations.py
--rw-r--r--   0 runner    (1001) docker     (121)    10433 2022-06-14 22:30:35.000000 strato_dyndns-2.3.1/strato_dyndns/lib/requests_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2034 2022-06-14 22:30:35.000000 strato_dyndns-2.3.1/strato_dyndns/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-14 22:30:42.756977 strato_dyndns-2.3.1/strato_dyndns/schema/
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-06-14 22:30:35.000000 strato_dyndns-2.3.1/strato_dyndns/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-06-14 22:30:35.000000 strato_dyndns-2.3.1/strato_dyndns/schema/namecheap.py
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-06-14 22:30:35.000000 strato_dyndns-2.3.1/strato_dyndns/schema/strato.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-14 22:30:42.752977 strato_dyndns-2.3.1/strato_dyndns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3792 2022-06-14 22:30:42.000000 strato_dyndns-2.3.1/strato_dyndns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      745 2022-06-14 22:30:42.000000 strato_dyndns-2.3.1/strato_dyndns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-14 22:30:42.000000 strato_dyndns-2.3.1/strato_dyndns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-06-14 22:30:42.000000 strato_dyndns-2.3.1/strato_dyndns.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-06-14 22:30:42.000000 strato_dyndns-2.3.1/strato_dyndns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-06-14 22:30:42.000000 strato_dyndns-2.3.1/strato_dyndns.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:24:13.622953 strato_dyndns-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-13 11:24:00.000000 strato_dyndns-2.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-13 11:24:13.622953 strato_dyndns-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-04-13 11:24:00.000000 strato_dyndns-2.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 11:24:13.622953 strato_dyndns-2.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-13 11:24:00.000000 strato_dyndns-2.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:24:13.618953 strato_dyndns-2.3.2/strato_dyndns/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-13 11:24:00.000000 strato_dyndns-2.3.2/strato_dyndns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:24:13.622953 strato_dyndns-2.3.2/strato_dyndns/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 11:24:00.000000 strato_dyndns-2.3.2/strato_dyndns/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-13 11:24:00.000000 strato_dyndns-2.3.2/strato_dyndns/clients/connection_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-13 11:24:00.000000 strato_dyndns-2.3.2/strato_dyndns/clients/dyndns_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-04-13 11:24:00.000000 strato_dyndns-2.3.2/strato_dyndns/clients/namecheap_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-04-13 11:24:00.000000 strato_dyndns-2.3.2/strato_dyndns/clients/strato_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:24:13.622953 strato_dyndns-2.3.2/strato_dyndns/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-13 11:24:00.000000 strato_dyndns-2.3.2/strato_dyndns/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-04-13 11:24:00.000000 strato_dyndns-2.3.2/strato_dyndns/lib/args_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-13 11:24:00.000000 strato_dyndns-2.3.2/strato_dyndns/lib/file_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-04-13 11:24:00.000000 strato_dyndns-2.3.2/strato_dyndns/lib/requests_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-13 11:24:00.000000 strato_dyndns-2.3.2/strato_dyndns/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:24:13.622953 strato_dyndns-2.3.2/strato_dyndns/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-13 11:24:00.000000 strato_dyndns-2.3.2/strato_dyndns/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-13 11:24:00.000000 strato_dyndns-2.3.2/strato_dyndns/schema/namecheap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-13 11:24:00.000000 strato_dyndns-2.3.2/strato_dyndns/schema/strato.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:24:13.622953 strato_dyndns-2.3.2/strato_dyndns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-13 11:24:13.000000 strato_dyndns-2.3.2/strato_dyndns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-13 11:24:13.000000 strato_dyndns-2.3.2/strato_dyndns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 11:24:13.000000 strato_dyndns-2.3.2/strato_dyndns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-13 11:24:13.000000 strato_dyndns-2.3.2/strato_dyndns.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 11:24:13.000000 strato_dyndns-2.3.2/strato_dyndns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 11:24:13.000000 strato_dyndns-2.3.2/strato_dyndns.egg-info/top_level.txt
```

### Comparing `strato_dyndns-2.3.1/LICENSE` & `strato_dyndns-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `strato_dyndns-2.3.1/PKG-INFO` & `strato_dyndns-2.3.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,23 @@
-Metadata-Version: 2.1
-Name: strato_dyndns
-Version: 2.3.1
-Summary: Updates your DNS records on supported DNS registrars.
-Home-page: https://github.com/regmibijay/strato-dyndns
-Author: Bijay Regmi
-Author-email: strato-dyndns@regdelivery.de
-License: GNU (GPLv3)
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Strato-DynDNS
 
 [![Join the chat at https://gitter.im/strato-dyndns/community](https://badges.gitter.im/strato-dyndns/community.svg)](https://gitter.im/strato-dyndns/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 ![Build status](https://github.com/regmibijay/strato-dyndns/actions/workflows/main.yml/badge.svg)
 [![Downloads](https://static.pepy.tech/personalized-badge/strato-dyndns?period=total&units=international_system&left_color=black&right_color=green&left_text=Downloads)](https://pepy.tech/project/strato-dyndns)
+[![Total API Usage](https://regdelivery.de/github/dyndns-badge)](https://regdelivery.de/stratodyndns.json)
 
 
 Strato-DynDNS updates your website's DNS records on DNS servers. Originally
 designed for Strato. 
 
 ## Disclaimer
 
 * This tool is in no way associated with [Strato AG](https://strato.de).
 * You use this tool at your own sole responsibility.
+* To fetch external IPV4 and IPV6 Addresses, this library uses a simple PHP endpoint written and hosted by myself. No data about users IP is stored or processed by me except for amount of usage of API which can be seen [here](https://regdelivery.de/stratodyndns.json) publicly. However, logging of your IP address might still be done by Cloud Service Provider. If you do not want this, you can supply own API endpoint which returns pure IP address as response. See below in docs.
 
 ## Currently Supported Registrars
 - Strato
 - Namecheap
 
 ## Installation
 
@@ -80,9 +66,7 @@
 
 ### To-Do
 - add a block scheduler for own scheduling mechanism
 - add other domain registrars 
 
 ## Contributions
 Any contribution to this tool are welcome. Any pull request, bug or issue reporting will be addressed as soon as possible.
-
-
```

### Comparing `strato_dyndns-2.3.1/README.md` & `strato_dyndns-2.3.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,38 @@
+Metadata-Version: 2.1
+Name: strato_dyndns
+Version: 2.3.2
+Summary: Updates your DNS records on supported DNS registrars.
+Home-page: https://github.com/regmibijay/strato-dyndns
+Author: Bijay Regmi
+Author-email: strato-dyndns@regdelivery.de
+License: GNU (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Strato-DynDNS
 
 [![Join the chat at https://gitter.im/strato-dyndns/community](https://badges.gitter.im/strato-dyndns/community.svg)](https://gitter.im/strato-dyndns/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 ![Build status](https://github.com/regmibijay/strato-dyndns/actions/workflows/main.yml/badge.svg)
 [![Downloads](https://static.pepy.tech/personalized-badge/strato-dyndns?period=total&units=international_system&left_color=black&right_color=green&left_text=Downloads)](https://pepy.tech/project/strato-dyndns)
+[![Total API Usage](https://regdelivery.de/github/dyndns-badge)](https://regdelivery.de/stratodyndns.json)
 
 
 Strato-DynDNS updates your website's DNS records on DNS servers. Originally
 designed for Strato. 
 
 ## Disclaimer
 
 * This tool is in no way associated with [Strato AG](https://strato.de).
 * You use this tool at your own sole responsibility.
+* To fetch external IPV4 and IPV6 Addresses, this library uses a simple PHP endpoint written and hosted by myself. No data about users IP is stored or processed by me except for amount of usage of API which can be seen [here](https://regdelivery.de/stratodyndns.json) publicly. However, logging of your IP address might still be done by Cloud Service Provider. If you do not want this, you can supply own API endpoint which returns pure IP address as response. See below in docs.
 
 ## Currently Supported Registrars
 - Strato
 - Namecheap
 
 ## Installation
```

### Comparing `strato_dyndns-2.3.1/setup.py` & `strato_dyndns-2.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="strato_dyndns",
-    version="2.3.1",
+    version="2.3.2",
     packages=setuptools.find_packages(),
     url="https://github.com/regmibijay/strato-dyndns",
     license="GNU (GPLv3)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Bijay Regmi",
     author_email="strato-dyndns@regdelivery.de",
```

### Comparing `strato_dyndns-2.3.1/strato_dyndns/clients/connection_handler.py` & `strato_dyndns-2.3.2/strato_dyndns/clients/connection_handler.py`

 * *Files identical despite different names*

### Comparing `strato_dyndns-2.3.1/strato_dyndns/clients/dyndns_client.py` & `strato_dyndns-2.3.2/strato_dyndns/clients/dyndns_client.py`

 * *Files identical despite different names*

### Comparing `strato_dyndns-2.3.1/strato_dyndns/clients/namecheap_client.py` & `strato_dyndns-2.3.2/strato_dyndns/clients/namecheap_client.py`

 * *Files identical despite different names*

### Comparing `strato_dyndns-2.3.1/strato_dyndns/clients/strato_client.py` & `strato_dyndns-2.3.2/strato_dyndns/clients/strato_client.py`

 * *Files identical despite different names*

### Comparing `strato_dyndns-2.3.1/strato_dyndns/lib/args_validator.py` & `strato_dyndns-2.3.2/strato_dyndns/lib/args_validator.py`

 * *Files identical despite different names*

### Comparing `strato_dyndns-2.3.1/strato_dyndns/lib/requests_wrapper.py` & `strato_dyndns-2.3.2/strato_dyndns/lib/requests_wrapper.py`

 * *Files identical despite different names*

### Comparing `strato_dyndns-2.3.1/strato_dyndns/main.py` & `strato_dyndns-2.3.2/strato_dyndns/main.py`

 * *Files identical despite different names*

### Comparing `strato_dyndns-2.3.1/strato_dyndns.egg-info/PKG-INFO` & `strato_dyndns-2.3.2/strato_dyndns.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: strato-dyndns
-Version: 2.3.1
+Version: 2.3.2
 Summary: Updates your DNS records on supported DNS registrars.
 Home-page: https://github.com/regmibijay/strato-dyndns
 Author: Bijay Regmi
 Author-email: strato-dyndns@regdelivery.de
 License: GNU (GPLv3)
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Strato-DynDNS
 
 [![Join the chat at https://gitter.im/strato-dyndns/community](https://badges.gitter.im/strato-dyndns/community.svg)](https://gitter.im/strato-dyndns/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 ![Build status](https://github.com/regmibijay/strato-dyndns/actions/workflows/main.yml/badge.svg)
 [![Downloads](https://static.pepy.tech/personalized-badge/strato-dyndns?period=total&units=international_system&left_color=black&right_color=green&left_text=Downloads)](https://pepy.tech/project/strato-dyndns)
+[![Total API Usage](https://regdelivery.de/github/dyndns-badge)](https://regdelivery.de/stratodyndns.json)
 
 
 Strato-DynDNS updates your website's DNS records on DNS servers. Originally
 designed for Strato. 
 
 ## Disclaimer
 
 * This tool is in no way associated with [Strato AG](https://strato.de).
 * You use this tool at your own sole responsibility.
+* To fetch external IPV4 and IPV6 Addresses, this library uses a simple PHP endpoint written and hosted by myself. No data about users IP is stored or processed by me except for amount of usage of API which can be seen [here](https://regdelivery.de/stratodyndns.json) publicly. However, logging of your IP address might still be done by Cloud Service Provider. If you do not want this, you can supply own API endpoint which returns pure IP address as response. See below in docs.
 
 ## Currently Supported Registrars
 - Strato
 - Namecheap
 
 ## Installation
 
@@ -80,9 +81,7 @@
 
 ### To-Do
 - add a block scheduler for own scheduling mechanism
 - add other domain registrars 
 
 ## Contributions
 Any contribution to this tool are welcome. Any pull request, bug or issue reporting will be addressed as soon as possible.
-
-
```

### Comparing `strato_dyndns-2.3.1/strato_dyndns.egg-info/SOURCES.txt` & `strato_dyndns-2.3.2/strato_dyndns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

