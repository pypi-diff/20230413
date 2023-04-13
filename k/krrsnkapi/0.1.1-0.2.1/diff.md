# Comparing `tmp/krrsnkapi-0.1.1.tar.gz` & `tmp/krrsnkapi-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krrsnkapi-0.1.1.tar", last modified: Thu Apr 13 13:20:59 2023, max compression
+gzip compressed data, was "krrsnkapi-0.2.1.tar", last modified: Thu Apr 13 17:14:25 2023, max compression
```

## Comparing `krrsnkapi-0.1.1.tar` & `krrsnkapi-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 13:20:59.152514 krrsnkapi-0.1.1/
--rw-rw-rw-   0        0        0     1087 2023-04-13 13:12:53.000000 krrsnkapi-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0      603 2023-04-13 13:20:59.152514 krrsnkapi-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1569 2023-04-13 12:53:07.000000 krrsnkapi-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 13:20:59.132512 krrsnkapi-0.1.1/krrsnkapi/
--rw-rw-rw-   0        0        0       35 2023-04-13 13:20:12.000000 krrsnkapi-0.1.1/krrsnkapi/__init__.py
--rw-rw-rw-   0        0        0      893 2023-04-12 17:26:21.000000 krrsnkapi-0.1.1/krrsnkapi/krrsnkapi.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:20:59.149513 krrsnkapi-0.1.1/krrsnkapi.egg-info/
--rw-rw-rw-   0        0        0      603 2023-04-13 13:20:58.000000 krrsnkapi-0.1.1/krrsnkapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-04-13 13:20:58.000000 krrsnkapi-0.1.1/krrsnkapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 13:20:58.000000 krrsnkapi-0.1.1/krrsnkapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-13 13:20:58.000000 krrsnkapi-0.1.1/krrsnkapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-13 13:20:58.000000 krrsnkapi-0.1.1/krrsnkapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-13 13:20:59.155514 krrsnkapi-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1443 2023-04-13 13:19:59.000000 krrsnkapi-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:14:25.643639 krrsnkapi-0.2.1/
+-rw-rw-rw-   0        0        0     1087 2023-04-13 13:12:53.000000 krrsnkapi-0.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      665 2023-04-13 17:14:25.644639 krrsnkapi-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1569 2023-04-13 12:53:07.000000 krrsnkapi-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 17:14:25.629638 krrsnkapi-0.2.1/krrsnkapi/
+-rw-rw-rw-   0        0        0       35 2023-04-13 13:20:12.000000 krrsnkapi-0.2.1/krrsnkapi/__init__.py
+-rw-rw-rw-   0        0        0     1881 2023-04-13 16:55:34.000000 krrsnkapi-0.2.1/krrsnkapi/krrsnkapi.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:14:25.641639 krrsnkapi-0.2.1/krrsnkapi.egg-info/
+-rw-rw-rw-   0        0        0      665 2023-04-13 17:14:24.000000 krrsnkapi-0.2.1/krrsnkapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-04-13 17:14:25.000000 krrsnkapi-0.2.1/krrsnkapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 17:14:24.000000 krrsnkapi-0.2.1/krrsnkapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-13 17:14:24.000000 krrsnkapi-0.2.1/krrsnkapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-13 17:14:24.000000 krrsnkapi-0.2.1/krrsnkapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-13 17:14:25.646639 krrsnkapi-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1536 2023-04-13 17:14:06.000000 krrsnkapi-0.2.1/setup.py
```

### Comparing `krrsnkapi-0.1.1/LICENSE.txt` & `krrsnkapi-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `krrsnkapi-0.1.1/README.md` & `krrsnkapi-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `krrsnkapi-0.1.1/krrsnkapi/krrsnkapi.py` & `krrsnkapi-0.2.1/krrsnkapi/krrsnkapi.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,14 +12,52 @@
 		self.response = requests.post(url)
 	
 
 		self.status = self.response.text
 
 		return self.status
 
+	def get_last_message_info(self, wReturn):
+		self.wReturn = wReturn
+
+		url = f'https://kararasenok.ueuo.com/api/v1/getlastmessageinfo/?apikey={self.apikey}&return={self.wReturn}'
+
+		self.response = requests.post(url)
+	
+
+		self.status = self.response.text
+
+		return self.status
+
+	def get_message_by_id(self, msgid, returnMessage = "0"):
+		self.msgid = msgid
+		self.returnMessage = returnMessage
+
+		url = f'https://kararasenok.ueuo.com/api/v1/getmessagebyid/?apikey={self.apikey}&id={self.msgid}&returnMessage={self.returnMessage}'
+
+		self.response = requests.post(url)
+	
+
+		self.status = self.response.text
+
+		return self.status
+
+	def get_message_info_by_id(self, msgid, wReturn):
+		self.msgid = msgid
+		self.wReturn = wReturn
+
+		url = f'https://kararasenok.ueuo.com/api/v1/getmessageinfobyid/?apikey={self.apikey}&id={self.msgid}&return={self.wReturn}'
+
+		self.response = requests.post(url)
+	
+
+		self.status = self.response.text
+
+		return self.status
+
 class Base64:
 		def __init__(self, apikey):
 			self.apikey = apikey
 
 		def decode(self, text):
 			self.text = text
 
@@ -33,8 +71,7 @@
 			self.text = text
 
 			url = f'https://kararasenok.ueuo.com/api/v1/base64/encode/?text={self.text}&apikey={self.apikey}'
 
 			self.response = requests.post(url)
 
 			return self.response.text
-
```

### Comparing `krrsnkapi-0.1.1/setup.py` & `krrsnkapi-0.2.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from setuptools import setup
 
+# ver = input("version: ")
+
 setup(
   name = 'krrsnkapi',         # How you named your package folder (MyLib)
   packages = ['krrsnkapi'],   # Chose the same as "name"
-  version = '0.1.1',      # Start with a small number and increase it with every change you make
+  version = "0.2.1",      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
-  description = 'Module for easy use of my api',   # Give a short description about your library
+  description = 'Module for easy use of my api | info on GitHub: https://github.com/kararasenok_gd/krrsnkapi',   # Give a short description about your library
   author = 'kararasenok_gd',                   # Type in your name
   author_email = 'murzikkurzikpro@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/kararasenok_gd/krrsnkapi',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/kararasenok-gd/krrsnkapi/archive/v0.1.tar.gz',    # I explain this later on
+  download_url = f'https://github.com/kararasenok-gd/krrsnkapi/archive/v0.2.tar.gz',    # I explain this later on
   keywords = ["api"],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'requests'
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
```

