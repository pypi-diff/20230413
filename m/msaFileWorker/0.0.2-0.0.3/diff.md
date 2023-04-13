# Comparing `tmp/msaFileWorker-0.0.2.tar.gz` & `tmp/msaFileWorker-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msaFileWorker-0.0.2.tar", last modified: Thu Mar 16 14:05:31 2023, max compression
+gzip compressed data, was "msaFileWorker-0.0.3.tar", last modified: Thu Apr 13 12:11:15 2023, max compression
```

## Comparing `msaFileWorker-0.0.2.tar` & `msaFileWorker-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxr-x   0 vitaliy   (1000) vitaliy   (1000)        0 2023-03-16 14:05:31.882184 msaFileWorker-0.0.2/
--rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)     1100 2023-01-13 15:04:07.000000 msaFileWorker-0.0.2/LICENCE
--rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)       58 2023-01-13 15:04:07.000000 msaFileWorker-0.0.2/MANIFEST.in
--rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)     2889 2023-03-16 14:05:31.882184 msaFileWorker-0.0.2/PKG-INFO
--rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)     1589 2023-01-13 15:04:07.000000 msaFileWorker-0.0.2/README.md
-drwxrwxr-x   0 vitaliy   (1000) vitaliy   (1000)        0 2023-03-16 14:05:31.882184 msaFileWorker-0.0.2/msaFileWorker/
--rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)      477 2023-03-16 13:50:44.000000 msaFileWorker-0.0.2/msaFileWorker/__init__.py
-drwxrwxr-x   0 vitaliy   (1000) vitaliy   (1000)        0 2023-03-16 14:05:31.882184 msaFileWorker-0.0.2/msaFileWorker/utils/
--rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)      229 2023-03-16 13:50:44.000000 msaFileWorker-0.0.2/msaFileWorker/utils/__init__.py
--rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)       83 2023-03-16 13:50:44.000000 msaFileWorker-0.0.2/msaFileWorker/utils/constans.py
--rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)      391 2023-01-13 15:04:07.000000 msaFileWorker-0.0.2/msaFileWorker/utils/exc.py
--rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)     8850 2023-03-16 13:50:44.000000 msaFileWorker-0.0.2/msaFileWorker/utils/file_worker.py
-drwxrwxr-x   0 vitaliy   (1000) vitaliy   (1000)        0 2023-03-16 14:05:31.882184 msaFileWorker-0.0.2/msaFileWorker.egg-info/
--rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)     2889 2023-03-16 14:05:31.000000 msaFileWorker-0.0.2/msaFileWorker.egg-info/PKG-INFO
--rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)      423 2023-03-16 14:05:31.000000 msaFileWorker-0.0.2/msaFileWorker.egg-info/SOURCES.txt
--rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)        1 2023-03-16 14:05:31.000000 msaFileWorker-0.0.2/msaFileWorker.egg-info/dependency_links.txt
--rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)       22 2023-03-16 14:05:31.000000 msaFileWorker-0.0.2/msaFileWorker.egg-info/requires.txt
--rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)       14 2023-03-16 14:05:31.000000 msaFileWorker-0.0.2/msaFileWorker.egg-info/top_level.txt
--rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)        1 2023-01-13 15:19:35.000000 msaFileWorker-0.0.2/msaFileWorker.egg-info/zip-safe
--rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)       42 2023-01-13 15:04:07.000000 msaFileWorker-0.0.2/requirements.txt
--rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)       38 2023-03-16 14:05:31.882184 msaFileWorker-0.0.2/setup.cfg
--rw-rw-r--   0 vitaliy   (1000) vitaliy   (1000)     2168 2023-01-13 15:04:07.000000 msaFileWorker-0.0.2/setup.py
+drwxrwxr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-04-13 12:11:15.248585 msaFileWorker-0.0.3/
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     1100 2023-03-26 10:33:44.000000 msaFileWorker-0.0.3/LICENCE
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)       58 2023-03-26 10:33:44.000000 msaFileWorker-0.0.3/MANIFEST.in
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     2889 2023-04-13 12:11:15.248585 msaFileWorker-0.0.3/PKG-INFO
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     1589 2023-03-26 10:33:44.000000 msaFileWorker-0.0.3/README.md
+drwxrwxr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-04-13 12:11:15.248585 msaFileWorker-0.0.3/msaFileWorker/
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)      477 2023-04-13 12:11:06.000000 msaFileWorker-0.0.3/msaFileWorker/__init__.py
+drwxrwxr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-04-13 12:11:15.248585 msaFileWorker-0.0.3/msaFileWorker/utils/
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)      229 2023-03-26 10:33:44.000000 msaFileWorker-0.0.3/msaFileWorker/utils/__init__.py
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)       83 2023-03-26 10:33:44.000000 msaFileWorker-0.0.3/msaFileWorker/utils/constans.py
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     8195 2023-04-13 11:41:41.000000 msaFileWorker-0.0.3/msaFileWorker/utils/file_worker.py
+drwxrwxr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-04-13 12:11:15.248585 msaFileWorker-0.0.3/msaFileWorker.egg-info/
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     2889 2023-04-13 12:11:15.000000 msaFileWorker-0.0.3/msaFileWorker.egg-info/PKG-INFO
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)      442 2023-04-13 12:11:15.000000 msaFileWorker-0.0.3/msaFileWorker.egg-info/SOURCES.txt
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)        1 2023-04-13 12:11:15.000000 msaFileWorker-0.0.3/msaFileWorker.egg-info/dependency_links.txt
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)       22 2023-04-13 12:11:15.000000 msaFileWorker-0.0.3/msaFileWorker.egg-info/requires.txt
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)       14 2023-04-13 12:11:15.000000 msaFileWorker-0.0.3/msaFileWorker.egg-info/top_level.txt
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)        1 2023-04-13 12:11:15.000000 msaFileWorker-0.0.3/msaFileWorker.egg-info/zip-safe
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)      855 2023-04-13 12:11:06.000000 msaFileWorker-0.0.3/pyproject.toml
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)       42 2023-03-26 10:33:44.000000 msaFileWorker-0.0.3/requirements.txt
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)       38 2023-04-13 12:11:15.248585 msaFileWorker-0.0.3/setup.cfg
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     2168 2023-03-26 10:33:44.000000 msaFileWorker-0.0.3/setup.py
+drwxrwxr-x   0 vitaly    (1000) vitaly    (1000)        0 2023-04-13 12:11:15.248585 msaFileWorker-0.0.3/tests/
+-rw-rw-r--   0 vitaly    (1000) vitaly    (1000)     7642 2023-04-13 11:41:41.000000 msaFileWorker-0.0.3/tests/test_file_worker_func.py
```

### Comparing `msaFileWorker-0.0.2/LICENCE` & `msaFileWorker-0.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `msaFileWorker-0.0.2/PKG-INFO` & `msaFileWorker-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msaFileWorker
-Version: 0.0.2
+Version: 0.0.3
 Summary: msaFileWorker - file management library
 Home-page: https://github.com/u2d-ai/msaFileWorker
 Download-URL: http://pypi.python.org/pypi/msaFileWorker
 Author: Stefan Welcker
 Author-email: stefan@u2d.ai
 License: MIT
 Project-URL: Documentation, http://msaFileWorker.u2d.ai/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: msaFileWorker Version: 0.0.2 Summary: msaFileWorker
+Metadata-Version: 2.1 Name: msaFileWorker Version: 0.0.3 Summary: msaFileWorker
 - file management library Home-page: https://github.com/u2d-ai/msaFileWorker
 Download-URL: http://pypi.python.org/pypi/msaFileWorker Author: Stefan Welcker
 Author-email: stefan@u2d.ai License: MIT Project-URL: Documentation, http://
 msaFileWorker.u2d.ai/ Project-URL: Source, https://github.com/u2d-ai/
 msaFileWorker Project-URL: Tracker, https://github.com/u2d-ai/msaFileWorker/
 issues Classifier: Development Status :: 4 - Beta Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
```

### Comparing `msaFileWorker-0.0.2/README.md` & `msaFileWorker-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `msaFileWorker-0.0.2/msaFileWorker/utils/file_worker.py` & `msaFileWorker-0.0.3/msaFileWorker/utils/file_worker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from io import BytesIO
 from typing import Dict, List, Tuple, Union
 from zipfile import ZIP_DEFLATED, ZipFile
 
 from msaFilesystem import msafs as fs
 from msaFileWorker.utils.constans import CLIENT_ID, SPK_NFS_SHARE
-from msaFileWorker.utils.exc import FilenameAlreadyExists
 
 
 class FileWorker:
     """
     Working with files
 
     Parameters:
@@ -44,15 +43,14 @@
 
             file_as_bytes: file in bytes format
             file_name: name of file
             path_to_save: if you need another folder. Default: root
         """
         if path_to_save:
             await self._create_folders_if_not_exist(path_to_save)
-        await self._check_same_filename(path_to_save=path_to_save, file_name=file_name)
         self.filesystem.writebytes(f"{path_to_save}/{file_name}", contents=file_as_bytes)
 
     async def save_many_bytes_as_files(
         self,
         list_of_data: List[Tuple[str, bytes]],
         path_to_save: str = "",
     ) -> None:
@@ -83,15 +81,14 @@
             file_name: name of file
             path_to_save: if you need another folder. Default: root
             file_type: type of file. Default: txt
         """
         file_name_with_type = f"{file_name}.{file_type}"
         if path_to_save:
             await self._create_folders_if_not_exist(path_to_save)
-        await self._check_same_filename(path_to_save=path_to_save, file_name=file_name_with_type)
 
         self.filesystem.writebytes(f"{path_to_save}/{file_name_with_type}", contents=bytes(str(text), "utf-8"))
 
     async def save_many_texts_as_files(
         self,
         list_of_data: List[Tuple[str, str, str]],
         path_to_save: str = "",
@@ -245,27 +242,14 @@
         Parameters:
 
             path: which path to create. Ex: folder/folder1/folder2
         """
         if not self.filesystem.exists(path):
             self.filesystem.makedirs(path)
 
-    async def _check_same_filename(self, path_to_save: str, file_name: str) -> None:
-        """
-        Checking file with the same name
-
-        Parameters:
-
-            path_to_save: path where you need to check
-            file_name: name of file
-
-        """
-        if self.filesystem.isfile(f"{path_to_save}/{file_name}"):
-            raise FilenameAlreadyExists(file_name=file_name, path=path_to_save)
-
     async def _zip_with_subfolders(self, zip_buffer: BytesIO, folder: str, path: str) -> BytesIO:
         """Create zip with all files(include all folders)
 
         Parameters:
 
             zip_buffer: BytesIO object
             folder: name of folder
```

### Comparing `msaFileWorker-0.0.2/msaFileWorker.egg-info/PKG-INFO` & `msaFileWorker-0.0.3/msaFileWorker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msaFileWorker
-Version: 0.0.2
+Version: 0.0.3
 Summary: msaFileWorker - file management library
 Home-page: https://github.com/u2d-ai/msaFileWorker
 Download-URL: http://pypi.python.org/pypi/msaFileWorker
 Author: Stefan Welcker
 Author-email: stefan@u2d.ai
 License: MIT
 Project-URL: Documentation, http://msaFileWorker.u2d.ai/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: msaFileWorker Version: 0.0.2 Summary: msaFileWorker
+Metadata-Version: 2.1 Name: msaFileWorker Version: 0.0.3 Summary: msaFileWorker
 - file management library Home-page: https://github.com/u2d-ai/msaFileWorker
 Download-URL: http://pypi.python.org/pypi/msaFileWorker Author: Stefan Welcker
 Author-email: stefan@u2d.ai License: MIT Project-URL: Documentation, http://
 msaFileWorker.u2d.ai/ Project-URL: Source, https://github.com/u2d-ai/
 msaFileWorker Project-URL: Tracker, https://github.com/u2d-ai/msaFileWorker/
 issues Classifier: Development Status :: 4 - Beta Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
```

### Comparing `msaFileWorker-0.0.2/setup.py` & `msaFileWorker-0.0.3/setup.py`

 * *Files identical despite different names*

