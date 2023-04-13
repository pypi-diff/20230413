# Comparing `tmp/cf_changelog-1.0.0.tar.gz` & `tmp/cf_changelog-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\DELL\Documents\cf_changelog\dist\.tmp-zsmv9_rk\cf_changelog-1.0.0.tar", last modified: Tue Apr 11 21:41:09 2023, max compression
+gzip compressed data, was "C:\Users\DELL\Documents\cf_changelog\dist\.tmp-zzmm531o\cf_changelog-1.0.1.tar", last modified: Thu Apr 13 15:10:56 2023, max compression
```

## Comparing `cf_changelog-1.0.0.tar` & `cf_changelog-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 21:41:09.000000 cf_changelog-1.0.0/
--rw-rw-rw-   0        0        0     1070 2023-04-11 19:59:57.000000 cf_changelog-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1503 2023-04-11 21:41:09.000000 cf_changelog-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1169 2023-04-11 21:35:22.000000 cf_changelog-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 21:41:09.000000 cf_changelog-1.0.0/cf_changelog/
--rw-rw-rw-   0        0        0       31 2023-04-11 21:02:35.000000 cf_changelog-1.0.0/cf_changelog/__init__.py
--rw-rw-rw-   0        0        0     6448 2023-04-11 20:43:01.000000 cf_changelog-1.0.0/cf_changelog/cf_changelog.py
-drwxrwxrwx   0        0        0        0 2023-04-11 21:41:09.000000 cf_changelog-1.0.0/cf_changelog.egg-info/
--rw-rw-rw-   0        0        0     1503 2023-04-11 21:41:09.000000 cf_changelog-1.0.0/cf_changelog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-04-11 21:41:09.000000 cf_changelog-1.0.0/cf_changelog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 21:41:09.000000 cf_changelog-1.0.0/cf_changelog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-11 21:41:09.000000 cf_changelog-1.0.0/cf_changelog.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2023-04-11 21:41:09.000000 cf_changelog-1.0.0/cf_changelog.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-11 21:41:09.000000 cf_changelog-1.0.0/cf_changelog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 21:41:09.000000 cf_changelog-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      832 2023-04-11 21:37:28.000000 cf_changelog-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 15:10:56.000000 cf_changelog-1.0.1/
+-rw-rw-rw-   0        0        0     1070 2023-04-11 19:59:57.000000 cf_changelog-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1503 2023-04-13 15:10:56.000000 cf_changelog-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1169 2023-04-11 21:35:22.000000 cf_changelog-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 15:10:56.000000 cf_changelog-1.0.1/cf_changelog/
+-rw-rw-rw-   0        0        0       31 2023-04-11 21:02:35.000000 cf_changelog-1.0.1/cf_changelog/__init__.py
+-rw-rw-rw-   0        0        0     6448 2023-04-13 15:08:38.000000 cf_changelog-1.0.1/cf_changelog/cf_changelog.py
+drwxrwxrwx   0        0        0        0 2023-04-13 15:10:56.000000 cf_changelog-1.0.1/cf_changelog.egg-info/
+-rw-rw-rw-   0        0        0     1503 2023-04-13 15:10:56.000000 cf_changelog-1.0.1/cf_changelog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-04-13 15:10:56.000000 cf_changelog-1.0.1/cf_changelog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 15:10:56.000000 cf_changelog-1.0.1/cf_changelog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-13 15:10:56.000000 cf_changelog-1.0.1/cf_changelog.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       43 2023-04-13 15:10:56.000000 cf_changelog-1.0.1/cf_changelog.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-13 15:10:56.000000 cf_changelog-1.0.1/cf_changelog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 15:10:56.000000 cf_changelog-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      832 2023-04-13 14:53:27.000000 cf_changelog-1.0.1/setup.py
```

### Comparing `cf_changelog-1.0.0/LICENSE` & `cf_changelog-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cf_changelog-1.0.0/PKG-INFO` & `cf_changelog-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf_changelog
-Version: 1.0.0
+Version: 1.0.1
 Summary: Conflict-Free Changelog manager
 Home-page: https://gitlab.com/salekpawel/cf_changelog
 Author: Paweł Sałek
 Author-email: salekpawel@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cf_changelog-1.0.0/README.md` & `cf_changelog-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cf_changelog-1.0.0/cf_changelog/cf_changelog.py` & `cf_changelog-1.0.1/cf_changelog/cf_changelog.py`

 * *Files identical despite different names*

### Comparing `cf_changelog-1.0.0/cf_changelog.egg-info/PKG-INFO` & `cf_changelog-1.0.1/cf_changelog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf-changelog
-Version: 1.0.0
+Version: 1.0.1
 Summary: Conflict-Free Changelog manager
 Home-page: https://gitlab.com/salekpawel/cf_changelog
 Author: Paweł Sałek
 Author-email: salekpawel@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cf_changelog-1.0.0/setup.py` & `cf_changelog-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(name='cf_changelog',
       long_description=long_description,
       long_description_content_type='text/markdown',
-      version='1.0.0',
+      version='1.0.1',
       description='Conflict-Free Changelog manager',
       author='Paweł Sałek',
       author_email='salekpawel@gmail.com',
       url='https://gitlab.com/salekpawel/cf_changelog',
       packages=['cf_changelog', ],
       license="MIT",
       install_requires=[
```

