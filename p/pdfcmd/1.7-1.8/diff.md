# Comparing `tmp/pdfcmd-1.7.tar.gz` & `tmp/pdfcmd-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfcmd-1.7.tar", last modified: Tue Feb 28 05:42:33 2023, max compression
+gzip compressed data, was "pdfcmd-1.8.tar", last modified: Thu Apr 13 01:15:26 2023, max compression
```

## Comparing `pdfcmd-1.7.tar` & `pdfcmd-1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-02-28 05:42:33.645700 pdfcmd-1.7/
--rw-r--r--   0 mark      (1000) mark      (1000)     5620 2023-02-28 05:42:33.645700 pdfcmd-1.7/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)     5264 2023-02-12 23:22:10.000000 pdfcmd-1.7/README.md
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-02-28 05:42:33.642366 pdfcmd-1.7/pdfcmd/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2021-01-27 04:55:01.000000 pdfcmd-1.7/pdfcmd/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)       66 2022-07-21 00:18:22.000000 pdfcmd-1.7/pdfcmd/__main__.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-02-28 05:42:33.645700 pdfcmd-1.7/pdfcmd/commands/
--rw-r--r--   0 mark      (1000) mark      (1000)     3162 2023-02-12 23:20:04.000000 pdfcmd-1.7/pdfcmd/commands/cat.py
--rw-r--r--   0 mark      (1000) mark      (1000)      113 2022-07-25 00:30:51.000000 pdfcmd-1.7/pdfcmd/commands/help.py
--rw-r--r--   0 mark      (1000) mark      (1000)      483 2022-12-24 07:53:21.000000 pdfcmd-1.7/pdfcmd/commands/info.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2630 2022-12-25 03:57:34.000000 pdfcmd-1.7/pdfcmd/commands/pages.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1634 2022-08-29 05:07:44.000000 pdfcmd-1.7/pdfcmd/pdfcmd.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-02-28 05:42:33.642366 pdfcmd-1.7/pdfcmd.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     5620 2023-02-28 05:42:33.000000 pdfcmd-1.7/pdfcmd.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      351 2023-02-28 05:42:33.000000 pdfcmd-1.7/pdfcmd.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-02-28 05:42:33.000000 pdfcmd-1.7/pdfcmd.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       46 2023-02-28 05:42:33.000000 pdfcmd-1.7/pdfcmd.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       13 2023-02-28 05:42:33.000000 pdfcmd-1.7/pdfcmd.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       23 2023-02-28 05:42:33.000000 pdfcmd-1.7/pdfcmd.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       38 2023-02-28 05:42:33.645700 pdfcmd-1.7/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1034 2023-02-12 23:22:08.000000 pdfcmd-1.7/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-13 01:15:26.725440 pdfcmd-1.8/
+-rw-r--r--   0 mark      (1000) mark      (1000)     5620 2023-04-13 01:15:26.722107 pdfcmd-1.8/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)     5264 2023-04-13 01:11:07.000000 pdfcmd-1.8/README.md
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-13 01:15:26.718773 pdfcmd-1.8/pdfcmd/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2021-01-27 04:55:01.000000 pdfcmd-1.8/pdfcmd/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)       66 2022-07-21 00:18:22.000000 pdfcmd-1.8/pdfcmd/__main__.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-13 01:15:26.722107 pdfcmd-1.8/pdfcmd/commands/
+-rw-r--r--   0 mark      (1000) mark      (1000)     3162 2023-02-12 23:20:04.000000 pdfcmd-1.8/pdfcmd/commands/cat.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      113 2022-07-25 00:30:51.000000 pdfcmd-1.8/pdfcmd/commands/help.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      483 2022-12-24 07:53:21.000000 pdfcmd-1.8/pdfcmd/commands/info.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2630 2022-12-25 03:57:34.000000 pdfcmd-1.8/pdfcmd/commands/pages.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1373 2023-04-13 01:10:47.000000 pdfcmd-1.8/pdfcmd/pdfcmd.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-13 01:15:26.722107 pdfcmd-1.8/pdfcmd.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     5620 2023-04-13 01:15:26.000000 pdfcmd-1.8/pdfcmd.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      351 2023-04-13 01:15:26.000000 pdfcmd-1.8/pdfcmd.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-13 01:15:26.000000 pdfcmd-1.8/pdfcmd.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       46 2023-04-13 01:15:26.000000 pdfcmd-1.8/pdfcmd.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       13 2023-04-13 01:15:26.000000 pdfcmd-1.8/pdfcmd.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       23 2023-04-13 01:15:26.000000 pdfcmd-1.8/pdfcmd.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       38 2023-04-13 01:15:26.725440 pdfcmd-1.8/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1029 2023-04-13 01:14:58.000000 pdfcmd-1.8/setup.py
```

### Comparing `pdfcmd-1.7/PKG-INFO` & `pdfcmd-1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfcmd
-Version: 1.7
+Version: 1.8
 Summary: Utility to perform commands on PDF files
 Home-page: https://github.com/bulletmark/pdfcmd
 Author: Mark Blakeney
 Author-email: mark.blakeney@bullet-systems.net
 License: GPLv3
 Keywords: PDF
 Classifier: Programming Language :: Python :: 3
@@ -58,25 +58,14 @@
 positional arguments:
   file        PDF file
 
 options:
   -h, --help  show this help message and exit
 ```
 
-### Command `help`
-
-```
-usage: pdfcmd help [-h]
-
-Show help/usage for this utility.
-
-options:
-  -h, --help  show this help message and exit
-```
-
 ### Command `cat`
 
 ```
 usage: pdfcmd cat [-h] [-o OUTFILE] [-a] ...
 
 Concaternate selected pages of one or more PDF files into a single file.
 
@@ -138,14 +127,25 @@
   file         PDF file
 
 options:
   -h, --help   show this help message and exit
   -c, --count  just print the total count of pages
 ```
 
+### Command `help`
+
+```
+usage: pdfcmd help [-h]
+
+Show help/usage for this utility.
+
+options:
+  -h, --help  show this help message and exit
+```
+
 ## INSTALLATION
 
 Arch Linux users can install [pdfcmd from the
 AUR](https://aur.archlinux.org/packages/pdfcmd).
 Python 3.6 or later is required. Note [pdfcmd is on
 PyPI](https://pypi.org/project/pdfcmd/) so just ensure that
 `python3-pip` and `python3-wheel` are installed then type the following
```

### Comparing `pdfcmd-1.7/README.md` & `pdfcmd-1.8/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -45,25 +45,14 @@
 positional arguments:
   file        PDF file
 
 options:
   -h, --help  show this help message and exit
 ```
 
-### Command `help`
-
-```
-usage: pdfcmd help [-h]
-
-Show help/usage for this utility.
-
-options:
-  -h, --help  show this help message and exit
-```
-
 ### Command `cat`
 
 ```
 usage: pdfcmd cat [-h] [-o OUTFILE] [-a] ...
 
 Concaternate selected pages of one or more PDF files into a single file.
 
@@ -125,14 +114,25 @@
   file         PDF file
 
 options:
   -h, --help   show this help message and exit
   -c, --count  just print the total count of pages
 ```
 
+### Command `help`
+
+```
+usage: pdfcmd help [-h]
+
+Show help/usage for this utility.
+
+options:
+  -h, --help  show this help message and exit
+```
+
 ## INSTALLATION
 
 Arch Linux users can install [pdfcmd from the
 AUR](https://aur.archlinux.org/packages/pdfcmd).
 Python 3.6 or later is required. Note [pdfcmd is on
 PyPI](https://pypi.org/project/pdfcmd/) so just ensure that
 `python3-pip` and `python3-wheel` are installed then type the following
```

### Comparing `pdfcmd-1.7/pdfcmd/commands/cat.py` & `pdfcmd-1.8/pdfcmd/commands/cat.py`

 * *Files identical despite different names*

### Comparing `pdfcmd-1.7/pdfcmd/commands/pages.py` & `pdfcmd-1.8/pdfcmd/commands/pages.py`

 * *Files identical despite different names*

### Comparing `pdfcmd-1.7/pdfcmd.egg-info/PKG-INFO` & `pdfcmd-1.8/pdfcmd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfcmd
-Version: 1.7
+Version: 1.8
 Summary: Utility to perform commands on PDF files
 Home-page: https://github.com/bulletmark/pdfcmd
 Author: Mark Blakeney
 Author-email: mark.blakeney@bullet-systems.net
 License: GPLv3
 Keywords: PDF
 Classifier: Programming Language :: Python :: 3
@@ -58,25 +58,14 @@
 positional arguments:
   file        PDF file
 
 options:
   -h, --help  show this help message and exit
 ```
 
-### Command `help`
-
-```
-usage: pdfcmd help [-h]
-
-Show help/usage for this utility.
-
-options:
-  -h, --help  show this help message and exit
-```
-
 ### Command `cat`
 
 ```
 usage: pdfcmd cat [-h] [-o OUTFILE] [-a] ...
 
 Concaternate selected pages of one or more PDF files into a single file.
 
@@ -138,14 +127,25 @@
   file         PDF file
 
 options:
   -h, --help   show this help message and exit
   -c, --count  just print the total count of pages
 ```
 
+### Command `help`
+
+```
+usage: pdfcmd help [-h]
+
+Show help/usage for this utility.
+
+options:
+  -h, --help  show this help message and exit
+```
+
 ## INSTALLATION
 
 Arch Linux users can install [pdfcmd from the
 AUR](https://aur.archlinux.org/packages/pdfcmd).
 Python 3.6 or later is required. Note [pdfcmd is on
 PyPI](https://pypi.org/project/pdfcmd/) so just ensure that
 `python3-pip` and `python3-wheel` are installed then type the following
```

### Comparing `pdfcmd-1.7/setup.py` & `pdfcmd-1.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 
 name = 'pdfcmd'
 module = name.replace('-', '_')
 here = Path(__file__).resolve().parent
 
 setup(
     name=name,
-    version='1.7',
+    version='1.8',
     description='Utility to perform commands on PDF files',
     long_description=here.joinpath('README.md').read_text(),
     long_description_content_type='text/markdown',
     url=f'https://github.com/bulletmark/{name}',
     author='Mark Blakeney',
     author_email='mark.blakeney@bullet-systems.net',
     keywords='PDF',
     license='GPLv3',
     packages=[module] + [str(d) for d in Path(module).iterdir() if d.is_dir()
-                and not d.name.startswith('_')],
+                and d.name[0] not in '._'],
     python_requires='>=3.6',
     install_requires=['pypdf>=3.1.0'],
     classifiers=[
         'Programming Language :: Python :: 3',
     ],
     data_files=[
         (f'share/{name}', ['README.md']),
```

