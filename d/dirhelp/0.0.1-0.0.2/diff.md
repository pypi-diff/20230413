# Comparing `tmp/dirhelp-0.0.1.tar.gz` & `tmp/dirhelp-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dirhelp-0.0.1.tar", last modified: Thu Apr 13 06:37:58 2023, max compression
+gzip compressed data, was "dirhelp-0.0.2.tar", last modified: Thu Apr 13 11:30:50 2023, max compression
```

## Comparing `dirhelp-0.0.1.tar` & `dirhelp-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-13 06:37:58.379442 dirhelp-0.0.1/
--rw-rw----   0 root         (0) everybody  (9997)       78 2020-04-20 13:20:58.000000 dirhelp-0.0.1/CHANGELOG.txt
--rw-rw----   0 root         (0) everybody  (9997)     1054 2023-04-13 06:09:46.000000 dirhelp-0.0.1/LICENCE.txt
--rw-rw----   0 root         (0) everybody  (9997)       26 2020-04-20 13:20:58.000000 dirhelp-0.0.1/MANIFEST.in
--rw-rw----   0 root         (0) everybody  (9997)      665 2023-04-13 06:37:58.369442 dirhelp-0.0.1/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      127 2023-04-13 06:09:22.000000 dirhelp-0.0.1/README
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-13 06:37:58.319442 dirhelp-0.0.1/dirhelp/
--rw-rw----   0 root         (0) everybody  (9997)     2322 2023-04-13 06:05:41.000000 dirhelp-0.0.1/dirhelp/__init__.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-13 06:37:58.359442 dirhelp-0.0.1/dirhelp.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      665 2023-04-13 06:37:58.000000 dirhelp-0.0.1/dirhelp.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      227 2023-04-13 06:37:58.000000 dirhelp-0.0.1/dirhelp.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-13 06:37:58.000000 dirhelp-0.0.1/dirhelp.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)        9 2023-04-13 06:37:58.000000 dirhelp-0.0.1/dirhelp.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        8 2023-04-13 06:37:58.000000 dirhelp-0.0.1/dirhelp.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-04-13 06:37:58.379442 dirhelp-0.0.1/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      632 2023-04-13 06:36:15.000000 dirhelp-0.0.1/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-13 11:30:50.664656 dirhelp-0.0.2/
+-rw-rw----   0 root         (0) everybody  (9997)       93 2023-04-13 11:28:33.000000 dirhelp-0.0.2/CHANGELOG.txt
+-rw-rw----   0 root         (0) everybody  (9997)     1054 2023-04-13 06:09:46.000000 dirhelp-0.0.2/LICENCE.txt
+-rw-rw----   0 root         (0) everybody  (9997)       26 2020-04-20 13:20:58.000000 dirhelp-0.0.2/MANIFEST.in
+-rw-rw----   0 root         (0) everybody  (9997)      680 2023-04-13 11:30:50.654656 dirhelp-0.0.2/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      127 2023-04-13 06:09:22.000000 dirhelp-0.0.2/README
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-13 11:30:50.554656 dirhelp-0.0.2/dirhelp/
+-rw-rw----   0 root         (0) everybody  (9997)     2853 2023-04-13 11:26:31.000000 dirhelp-0.0.2/dirhelp/__init__.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-13 11:30:50.634656 dirhelp-0.0.2/dirhelp.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      680 2023-04-13 11:30:50.000000 dirhelp-0.0.2/dirhelp.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      227 2023-04-13 11:30:50.000000 dirhelp-0.0.2/dirhelp.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-13 11:30:50.000000 dirhelp-0.0.2/dirhelp.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)        9 2023-04-13 11:30:50.000000 dirhelp-0.0.2/dirhelp.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        8 2023-04-13 11:30:50.000000 dirhelp-0.0.2/dirhelp.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-04-13 11:30:50.664656 dirhelp-0.0.2/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      632 2023-04-13 11:27:05.000000 dirhelp-0.0.2/setup.py
```

### Comparing `dirhelp-0.0.1/LICENCE.txt` & `dirhelp-0.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `dirhelp-0.0.1/PKG-INFO` & `dirhelp-0.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirhelp
-Version: 0.0.1
+Version: 0.0.2
 Summary: Dir Helping Library For Simplifying Your Work
 Home-page: UNKNOWN
 Author: Monil Darediya
 Author-email: monildarediya1@gmail.com
 License: MIT
 Keywords: dir-organise
 Platform: UNKNOWN
@@ -16,12 +16,11 @@
 
 # The Library For Organised Dir Output
 ## Uses `Os` For List Of Dirs, `Colorama` For Colorized Output and `typing` for literals
 
 Change Log
 ==========
 
-0.0.1 (19/04/2020)
+0.0.1 (13/04/2023)
 -------------------
-- First Release
-
+- Added NEW Argument `dotfiles`
```

### Comparing `dirhelp-0.0.1/dirhelp/__init__.py` & `dirhelp-0.0.2/dirhelp/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 import os, typing, colorama
 class Color:
-	def __init__(self, extensionlog: bool = False):
+	def __init__(self, extensionlog: bool = False, dotfiles: bool = True):
 		self.extbool = extensionlog
+		self.dtfiles = dotfiles
 	def dirListColor(self, dir, color: typing.Literal['LightBlue', 'Blue'], extension: str = 'py'):
 		"""The Color Syntax Return Of A Dir"""
 		thecolorlist = []
 		if self.extbool == True:
 			print(f'{colorama.Fore.RED}WARNING: {colorama.Style.BRIGHT}THIS IS ONLY FOR DEBBUGING{colorama.Style.NORMAL}{colorama.Fore.RESET}\nExtension: .{extension}')
-		for every in os.listdir(dir):
 			if os.path.isdir(every):
+				if every.startswith('.'):
+					if self.dtfiles == True:
+						if color == 'Blue':
+							thecolorlist.append(colorama.Style.BRIGHT + colorama.Fore.BLUE + every + colorama.Fore.RESET + colorama.Style.NORMAL)
+						elif color == 'LightBlue':
+							thecolorlist.append(colorama.Style.BRIGHT + colorama.Fore.CYAN + every + colorama.Fore.RESET + colorama.Style.NORMAL)
+						else:
+							raise ValueError(f'INVALID CHOICE \'{color.upper()}\', Choose LightBlue Or Blue')
+					elif self.dtfiles == False:
+						pass
 				if color == 'Blue':
 					thecolorlist.append(colorama.Style.BRIGHT + colorama.Fore.BLUE + every + colorama.Fore.RESET + colorama.Style.NORMAL)
 				elif color == 'LightBlue':
 					thecolorlist.append(colorama.Style.BRIGHT + colorama.Fore.CYAN + every + colorama.Fore.RESET + colorama.Style.NORMAL)
 				else:
 					raise ValueError(f'INVALID CHOICE \'{color.upper()}\', Choose LightBlue Or Blue')
 			elif every.endswith('.'+extension):
```

### Comparing `dirhelp-0.0.1/dirhelp.egg-info/PKG-INFO` & `dirhelp-0.0.2/dirhelp.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirhelp
-Version: 0.0.1
+Version: 0.0.2
 Summary: Dir Helping Library For Simplifying Your Work
 Home-page: UNKNOWN
 Author: Monil Darediya
 Author-email: monildarediya1@gmail.com
 License: MIT
 Keywords: dir-organise
 Platform: UNKNOWN
@@ -16,12 +16,11 @@
 
 # The Library For Organised Dir Output
 ## Uses `Os` For List Of Dirs, `Colorama` For Colorized Output and `typing` for literals
 
 Change Log
 ==========
 
-0.0.1 (19/04/2020)
+0.0.1 (13/04/2023)
 -------------------
-- First Release
-
+- Added NEW Argument `dotfiles`
```

### Comparing `dirhelp-0.0.1/setup.py` & `dirhelp-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   'Intended Audience :: Developers',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3.8'
 ]
  
 setup(
   name='dirhelp',
-  version='0.0.1',
+  version='0.0.2',
   description='Dir Helping Library For Simplifying Your Work',
   long_description=open('README').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Monil Darediya',
   author_email='monildarediya1@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

