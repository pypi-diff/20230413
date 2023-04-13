# Comparing `tmp/ecspylibs-1.1.30.tar.gz` & `tmp/ecspylibs-1.1.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecspylibs-1.1.30.tar", max compression
+gzip compressed data, was "ecspylibs-1.1.31.tar", max compression
```

## Comparing `ecspylibs-1.1.30.tar` & `ecspylibs-1.1.31.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     8859 2023-03-31 16:27:00.038097 ecspylibs-1.1.30/ChangeLog
--rw-r--r--   0        0        0     1075 2020-11-06 03:34:20.305134 ecspylibs-1.1.30/LICENSE.txt
--rw-r--r--   0        0        0     1537 2023-03-23 22:13:42.045610 ecspylibs-1.1.30/README.md
--rw-r--r--   0        0        0     1917 2023-03-31 16:56:03.312962 ecspylibs-1.1.30/pyproject.toml
--rw-r--r--   0        0        0      465 2023-02-08 23:25:52.618443 ecspylibs-1.1.30/src/ecspylibs/__init__.py
--rw-r--r--   0        0        0     2623 2023-02-20 21:12:06.796621 ecspylibs-1.1.30/src/ecspylibs/buildfunctionlist.py
--rw-r--r--   0        0        0     8433 2023-02-20 21:12:06.796621 ecspylibs-1.1.30/src/ecspylibs/checkservice.py
--rw-r--r--   0        0        0     3107 2023-02-20 21:12:06.796621 ecspylibs-1.1.30/src/ecspylibs/cleanuptempdirs.py
--rw-r--r--   0        0        0     7816 2023-03-31 16:27:00.038097 ecspylibs-1.1.30/src/ecspylibs/configfile.py
--rw-r--r--   0        0        0     4073 2023-03-16 21:03:11.029737 ecspylibs-1.1.30/src/ecspylibs/initsetup.py
--rw-r--r--   0        0        0     1672 2023-02-21 17:11:02.916128 ecspylibs-1.1.30/src/ecspylibs/parallel.py
--rw-r--r--   0        0        0     5036 2023-02-20 21:12:06.797621 ecspylibs-1.1.30/src/ecspylibs/parseemail.py
--rw-r--r--   0        0        0     3739 2023-02-20 21:12:06.797621 ecspylibs-1.1.30/src/ecspylibs/parsexml.py
--rw-r--r--   0        0        0     3797 2023-02-21 17:11:02.916128 ecspylibs-1.1.30/src/ecspylibs/password.py
--rw-r--r--   0        0        0     1816 2023-02-20 21:58:09.629999 ecspylibs-1.1.30/src/ecspylibs/reapchildren.py
--rw-r--r--   0        0        0     3279 2023-02-20 21:12:06.797621 ecspylibs-1.1.30/src/ecspylibs/sendemail.py
--rw-r--r--   0        0        0     2570 1970-01-01 00:00:00.000000 ecspylibs-1.1.30/setup.py
--rw-r--r--   0        0        0     3361 1970-01-01 00:00:00.000000 ecspylibs-1.1.30/PKG-INFO
+-rw-r--r--   0        0        0     9274 2023-04-13 20:37:00.519802 ecspylibs-1.1.31/ChangeLog
+-rw-r--r--   0        0        0     1075 2020-11-06 03:34:20.305134 ecspylibs-1.1.31/LICENSE.txt
+-rw-r--r--   0        0        0     1537 2023-03-23 22:13:42.045610 ecspylibs-1.1.31/README.md
+-rw-r--r--   0        0        0     1917 2023-04-13 20:37:00.519802 ecspylibs-1.1.31/pyproject.toml
+-rw-r--r--   0        0        0      465 2023-02-08 23:25:52.618443 ecspylibs-1.1.31/src/ecspylibs/__init__.py
+-rw-r--r--   0        0        0     2623 2023-02-20 21:12:06.796621 ecspylibs-1.1.31/src/ecspylibs/buildfunctionlist.py
+-rw-r--r--   0        0        0     8433 2023-02-20 21:12:06.796621 ecspylibs-1.1.31/src/ecspylibs/checkservice.py
+-rw-r--r--   0        0        0     3107 2023-02-20 21:12:06.796621 ecspylibs-1.1.31/src/ecspylibs/cleanuptempdirs.py
+-rw-r--r--   0        0        0     8051 2023-04-13 20:37:00.519802 ecspylibs-1.1.31/src/ecspylibs/configfile.py
+-rw-r--r--   0        0        0     3502 2023-04-13 20:37:00.519802 ecspylibs-1.1.31/src/ecspylibs/initsetup.py
+-rw-r--r--   0        0        0     1626 2023-04-13 20:37:00.519802 ecspylibs-1.1.31/src/ecspylibs/parallel.py
+-rw-r--r--   0        0        0     5036 2023-02-20 21:12:06.797621 ecspylibs-1.1.31/src/ecspylibs/parseemail.py
+-rw-r--r--   0        0        0     3739 2023-02-20 21:12:06.797621 ecspylibs-1.1.31/src/ecspylibs/parsexml.py
+-rw-r--r--   0        0        0     3797 2023-02-21 17:11:02.916128 ecspylibs-1.1.31/src/ecspylibs/password.py
+-rw-r--r--   0        0        0     1816 2023-02-20 21:58:09.629999 ecspylibs-1.1.31/src/ecspylibs/reapchildren.py
+-rw-r--r--   0        0        0     3279 2023-02-20 21:12:06.797621 ecspylibs-1.1.31/src/ecspylibs/sendemail.py
+-rw-r--r--   0        0        0     2570 1970-01-01 00:00:00.000000 ecspylibs-1.1.31/setup.py
+-rw-r--r--   0        0        0     3361 1970-01-01 00:00:00.000000 ecspylibs-1.1.31/PKG-INFO
```

### Comparing `ecspylibs-1.1.30/ChangeLog` & `ecspylibs-1.1.31/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+2023-04-13  Thomas R. Stevenson  <tom@tom.cc.wayne.edu>
+
+	* pyproject.toml: Update version to v1.1.31.
+
+	* src/ecspylibs/parallel.py (Parallel.run): Change self.arguments
+	into arguments.
+
+	* src/ecspylibs/initsetup.py (InitSetup.__post_init__): Remove
+	unnecessary comments.
+
+	* src/ecspylibs/configfile.py (ConfigFile): Create a seperate io
+	function that can process multiple types of I/O (read, write,
+	etc.).
+
 2023-03-31  Thomas R. Stevenson  <tom@tom.cc.wayne.edu>
 
 	* src/ecspylibs/configfile.py: Add code to process INI type
 	configuration files.
 
 	* pyproject.toml: Update version to v1.1.29.
```

### Comparing `ecspylibs-1.1.30/LICENSE.txt` & `ecspylibs-1.1.31/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ecspylibs-1.1.30/README.md` & `ecspylibs-1.1.31/README.md`

 * *Files identical despite different names*

### Comparing `ecspylibs-1.1.30/pyproject.toml` & `ecspylibs-1.1.31/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Last Changed:  $Date: Fri Mar 31 11:16:03 2023 -0400 $
 #
 # URL to git source: $URL: git@git.wayne.edu:ECS_Projects/ECSpylibs.git $
 #
 [tool.poetry]
 name = "ecspylibs"
-version = "v1.1.30"
+version = "v1.1.31"
 packages = [{include = "ecspylibs", from = "src"}]
 description = "Local python libraries used across multiple programs."
 license = "GPL-3.0-or-later"
 authors = ["Thomas R. Stevenson <aa0026@wayne.edu>"]
 maintainers = ["Thomas R. Stevenson <aa0026@wayne.edu>"]
 readme = "README.md"
 homepage = "https://git.wayne.edu/ECS_Projects/ECSpylibs.git"
```

### Comparing `ecspylibs-1.1.30/src/ecspylibs/buildfunctionlist.py` & `ecspylibs-1.1.31/src/ecspylibs/buildfunctionlist.py`

 * *Files identical despite different names*

### Comparing `ecspylibs-1.1.30/src/ecspylibs/checkservice.py` & `ecspylibs-1.1.31/src/ecspylibs/checkservice.py`

 * *Files identical despite different names*

### Comparing `ecspylibs-1.1.30/src/ecspylibs/cleanuptempdirs.py` & `ecspylibs-1.1.31/src/ecspylibs/cleanuptempdirs.py`

 * *Files identical despite different names*

### Comparing `ecspylibs-1.1.30/src/ecspylibs/configfile.py` & `ecspylibs-1.1.31/src/ecspylibs/configfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,29 +112,37 @@
             raise NotImplementedError
 
         self.suffix = self.file.suffix[1:]
 
     @property
     def read(self) -> object:
 
+        try:
+            return self.io("read")
+        except Exception as e:
+            print(f"\nException error processing file '{self.file}'.\n", file=sys.stderr)
+            raise e
+
+    def io(self, io_type: str) -> object:
+
         if self.file.suffix in self.suffix_types:
-            if "read" in self.suffix_types[self.file.suffix]:
+            if io_type in self.suffix_types[self.file.suffix]:
                 try:
-                    return self.suffix_types[self.file.suffix]['read']()
+                    return self.suffix_types[self.file.suffix][io_type]()
                 except PermissionError as e:
-                    print(f"\nPermission error reading file '{self.file}'.\n", file=sys.stderr)
+                    print(f"\nPermission error on file '{self.file}'.\n", file=sys.stderr)
                     raise e
                 except UnicodeDecodeError as e:
                     print(f"\nUnicode decode error while parsing file '{self.file}'.\n", file=sys.stderr)
                     raise e
                 except Exception as e:
                     print(f"\nException error processing file '{self.file}'.\n", file=sys.stderr)
                     raise e
             else:
-                print(f"\nFile '{self.file}' has no function type 'read'.\n", file=sys.stderr)
+                print(f"\nFile '{self.file}' has no function type '{io_type}'.\n", file=sys.stderr)
                 raise NotImplementedError
         else:
             print(f"\nFile '{self.file}' has an unknown suffix type of '{self.file.suffix}'.\n", file=sys.stderr)
             raise NotImplementedError
 
     def csv_read(self) -> object:
         try:
```

### Comparing `ecspylibs-1.1.30/src/ecspylibs/initsetup.py` & `ecspylibs-1.1.31/src/ecspylibs/initsetup.py`

 * *Files 16% similar despite different names*

```diff
@@ -53,27 +53,14 @@
                 self.config = self.default_arguments[self.config]
             else:
                 self.config = False
         else:
             self.config = False
 
         if self.config:
-            # try:
-            #     self.config = Path(self.config).resolve(strict=True)
-            # except FileNotFoundError as e:
-            #     print(f"\n: Can't find configuration file {self.config}\n", file=sys.stderr)
-            #     print(f"\nFileNotFoundError: {e=}\n", file=sys.stderr)
-            #     sys.exit(1)
-            # except Exception as e:
-            #     print(f"\nException: {e=}\n", file=sys.stderr)
-            #     sys.exit(2)
-
-            # with open(self.config, 'r') as file:
-            #     config_data = yaml.safe_load(file)
-
             config_file = ConfigFile(self.config)
             config_data = config_file.read
 
             if 'config' not in config_data:
                 print(f"\nError: Can't find dictionary 'config' in file '{self.config}'. Aborting!\n", file=sys.stderr)
                 sys.exit(3)
```

### Comparing `ecspylibs-1.1.30/src/ecspylibs/parallel.py` & `ecspylibs-1.1.31/src/ecspylibs/parallel.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,21 +54,19 @@
         self.__log.debug(f"Pool Size     : {self.pool_size}")
 
     def run(self, arguments: object) -> object:
         """
         Blah
         """
 
-        self.arguments = arguments
-
-        self.__log.debug(f"arguments   : {self.arguments}")
+        self.__log.debug(f"arguments   : {arguments}")
 
         start_time = time.perf_counter()
 
         with self.pool_executor(self.pool_size) as executor:
-            self.results = executor.map(self.process, self.arguments)
+            self.results = executor.map(self.process, arguments)
 
         finish_time = time.perf_counter()
 
         self.run_time = finish_time - start_time
 
         return self.results
```

### Comparing `ecspylibs-1.1.30/src/ecspylibs/parseemail.py` & `ecspylibs-1.1.31/src/ecspylibs/parseemail.py`

 * *Files identical despite different names*

### Comparing `ecspylibs-1.1.30/src/ecspylibs/parsexml.py` & `ecspylibs-1.1.31/src/ecspylibs/parsexml.py`

 * *Files identical despite different names*

### Comparing `ecspylibs-1.1.30/src/ecspylibs/password.py` & `ecspylibs-1.1.31/src/ecspylibs/password.py`

 * *Files identical despite different names*

### Comparing `ecspylibs-1.1.30/src/ecspylibs/reapchildren.py` & `ecspylibs-1.1.31/src/ecspylibs/reapchildren.py`

 * *Files identical despite different names*

### Comparing `ecspylibs-1.1.30/src/ecspylibs/sendemail.py` & `ecspylibs-1.1.31/src/ecspylibs/sendemail.py`

 * *Files identical despite different names*

### Comparing `ecspylibs-1.1.30/setup.py` & `ecspylibs-1.1.31/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'requests>=2.28.2,<3.0.0',
  'toml>=0.10.2,<0.11.0',
  'urllib3>=1.26.15,<2.0.0',
  'xlrd==1.2.0']
 
 setup_kwargs = {
     'name': 'ecspylibs',
-    'version': '1.1.30',
+    'version': '1.1.31',
     'description': 'Local python libraries used across multiple programs.',
     'long_description': '# ECSpylibs\n\n# Package files\n    -rw-r--r--. 1 tom tom 2568 Feb  2 13:57 src/ecspylibs/buildfunctionlist.py\n    -rw-r--r--. 1 tom tom 8390 Feb  2 13:57 src/ecspylibs/checkservice.py\n    -rw-r--r--. 1 tom tom 3090 Feb  2 13:57 src/ecspylibs/cleanuptempdirs.py\n    -rw-r--r--. 1 tom tom 6123 Mar 16 17:03 src/ecspylibs/configfile.py\n    -rw-r--r--. 1 tom tom  465 Jan 26 11:05 src/ecspylibs/__init__.py\n    -rw-r--r--. 1 tom tom 3678 Feb  2 13:57 src/ecspylibs/initsetup.py\n    -rw-r--r--. 1 tom tom 1676 Feb  8 12:50 src/ecspylibs/parallel.py\n    -rw-r--r--. 1 tom tom 4965 Feb  2 13:57 src/ecspylibs/parseemail.py\n    -rw-r--r--. 1 tom tom 3644 Feb  2 13:57 src/ecspylibs/parsexml.py\n    -rw-r--r--. 1 tom tom 3650 Feb  2 13:57 src/ecspylibs/password.py\n    -rw-r--r--. 1 tom tom 1879 Feb  2 13:57 src/ecspylibs/reapchildren.py\n    -rw-r--r--. 1 tom tom 2993 Feb  2 13:57 src/ecspylibs/sendemail.py\n\n# Git information\n[GIT Home][ECSPYLIBS],\n[README File][README],\n[LICENSE File][LICENSE],\n[ChangeLog File][CHANGELOG],\n[pyproject.toml File][PYPROJECT].\n\n# About Me\n[My contact information][About Me].\n\n[ECSPYLIBS]: https://git.wayne.edu/ECS_Projects/ECSpylibs\n[README]: https://git.wayne.edu/ECS_Projects/ECSpylibs/-/blob/master/README.md\n[LICENSE]: https://git.wayne.edu/ECS_Projects/ECSpylibs/-/blob/master/LICENSE.txt\n[CHANGELOG]: https://git.wayne.edu/ECS_Projects/ECSpylibs/-/blob/master/ChangeLog\n[PYPROJECT]: https://git.wayne.edu/ECS_Projects/ECSpylibs/-/blob/master/pyproject.toml\n[About Me]: https://About.Me/Thomas.R.Stevenson\n',
     'author': 'Thomas R. Stevenson',
     'author_email': 'aa0026@wayne.edu',
     'maintainer': 'Thomas R. Stevenson',
     'maintainer_email': 'aa0026@wayne.edu',
     'url': 'https://git.wayne.edu/ECS_Projects/ECSpylibs.git',
```

### Comparing `ecspylibs-1.1.30/PKG-INFO` & `ecspylibs-1.1.31/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecspylibs
-Version: 1.1.30
+Version: 1.1.31
 Summary: Local python libraries used across multiple programs.
 Home-page: https://git.wayne.edu/ECS_Projects/ECSpylibs.git
 License: GPL-3.0-or-later
 Keywords: buildfunctionlist,checkservice,cleanuptempdirs,initsetup,parallel,parseemail,parsexml,password,reapchildren,sendemail
 Author: Thomas R. Stevenson
 Author-email: aa0026@wayne.edu
 Maintainer: Thomas R. Stevenson
```

