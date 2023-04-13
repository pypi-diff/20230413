# Comparing `tmp/pycachera-4.0.0.tar.gz` & `tmp/pycachera-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycachera-4.0.0.tar", last modified: Thu Apr 13 03:34:56 2023, max compression
+gzip compressed data, was "pycachera-4.5.0.tar", last modified: Thu Apr 13 04:46:24 2023, max compression
```

## Comparing `pycachera-4.0.0.tar` & `pycachera-4.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 03:34:56.195941 pycachera-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-04-13 03:34:47.000000 pycachera-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-04-13 03:34:56.195941 pycachera-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2496 2023-04-13 03:34:47.000000 pycachera-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 03:34:56.195941 pycachera-4.0.0/pycachera/
--rw-r--r--   0 runner    (1001) docker     (122)      196 2023-04-13 03:34:47.000000 pycachera-4.0.0/pycachera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5265 2023-04-13 03:34:47.000000 pycachera-4.0.0/pycachera/cacher.py
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-04-13 03:34:47.000000 pycachera-4.0.0/pycachera/mpi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 03:34:56.195941 pycachera-4.0.0/pycachera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-04-13 03:34:56.000000 pycachera-4.0.0/pycachera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      249 2023-04-13 03:34:56.000000 pycachera-4.0.0/pycachera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 03:34:56.000000 pycachera-4.0.0/pycachera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-13 03:34:56.000000 pycachera-4.0.0/pycachera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-13 03:34:56.000000 pycachera-4.0.0/pycachera.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-13 03:34:56.195941 pycachera-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      691 2023-04-13 03:34:47.000000 pycachera-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 04:46:24.882463 pycachera-4.5.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-04-13 04:46:17.000000 pycachera-4.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-04-13 04:46:24.882463 pycachera-4.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2496 2023-04-13 04:46:17.000000 pycachera-4.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 04:46:24.878463 pycachera-4.5.0/pycachera/
+-rw-r--r--   0 runner    (1001) docker     (122)      196 2023-04-13 04:46:17.000000 pycachera-4.5.0/pycachera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5325 2023-04-13 04:46:17.000000 pycachera-4.5.0/pycachera/cacher.py
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-04-13 04:46:17.000000 pycachera-4.5.0/pycachera/mpi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 04:46:24.882463 pycachera-4.5.0/pycachera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-04-13 04:46:24.000000 pycachera-4.5.0/pycachera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2023-04-13 04:46:24.000000 pycachera-4.5.0/pycachera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 04:46:24.000000 pycachera-4.5.0/pycachera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-13 04:46:24.000000 pycachera-4.5.0/pycachera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-13 04:46:24.000000 pycachera-4.5.0/pycachera.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-13 04:46:24.882463 pycachera-4.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      691 2023-04-13 04:46:17.000000 pycachera-4.5.0/setup.py
```

### Comparing `pycachera-4.0.0/LICENSE` & `pycachera-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycachera-4.0.0/PKG-INFO` & `pycachera-4.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycachera
-Version: 4.0.0
+Version: 4.5.0
 Summary: A powerfull python caching tool
 Home-page: https://github.com/antolonappan/pycachera
 Author: Anto Idicherian Lonappan
 Author-email: mail@antolonappan.me
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pycachera-4.0.0/README.md` & `pycachera-4.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pycachera-4.0.0/pycachera/cacher.py` & `pycachera-4.5.0/pycachera/cacher.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,29 +20,29 @@
     Usage:
         >>> from pycachera import cache
         >>> @cache()
         >>> def myfunc(self, x):
         >>>     return x**2
     """
     
-    def __init__(self,cachefolder=None,extrarg=None,cachekey=None,verbose=False,recache=False):
+    def __init__(self,cachefolder=None,extrarg=None,cachekey=None,verbose=False,recache=False,with_mpi=False):
 
         if cachefolder is None:
             cachefolder = os.path.join(os.getcwd(),'.cache')
 
         if not os.path.exists(cachefolder):
             if verbose: print("PyCache: No cache folder found")
             os.makedirs(cachefolder)
             if verbose: print(f"PyCache: Setting '{cachefolder}' as Cache folder")
         
         self.cachefolder = cachefolder
         self.Cobject = None
         self.extrarg = extrarg
         self.recache = recache
-        
+        self.with_mpi = with_mpi
         if cachekey == None:
             self.cachekey = None
         else:
             self.cachekey = md5(cachekey.enconde()).hexdigest()
         self.verbose=verbose
         
     def __call__(self, func):
@@ -124,16 +124,16 @@
                 else:
                     a += str(0)
             
             if type(tag) == pd.DataFrame:
                 a += ''.join(map(str,list(tag.columns)))
                 a += f'{len(tag)}'
 
-        
-        a += str(mpi.rank)
+        if self.with_mpi:
+            a += str(mpi.rank)
 
         return md5(a.encode()).hexdigest()
     
     def file_writer(self,name,data):
         """
         Writes data to a file
         save the data in a pickle file
```

### Comparing `pycachera-4.0.0/pycachera.egg-info/PKG-INFO` & `pycachera-4.5.0/pycachera.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycachera
-Version: 4.0.0
+Version: 4.5.0
 Summary: A powerfull python caching tool
 Home-page: https://github.com/antolonappan/pycachera
 Author: Anto Idicherian Lonappan
 Author-email: mail@antolonappan.me
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pycachera-4.0.0/setup.py` & `pycachera-4.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 long_description = (this_directory / "README.md").read_text()
 
 files = ["pycachera/*"]
 setup(
         name = 'pycachera',
         packages = ['pycachera'],
         package_data = {'pycachera' : files },
-        version = '4.0.0',
+        version = '4.5.0',
         install_requires = ['numpy','pandas'],
         description = 'A powerfull python caching tool',
         author = 'Anto Idicherian Lonappan',
         author_email = 'mail@antolonappan.me',
         url = 'https://github.com/antolonappan/pycachera',
         long_description=long_description,
         long_description_content_type="text/markdown",
```

