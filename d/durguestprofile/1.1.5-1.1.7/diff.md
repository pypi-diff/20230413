# Comparing `tmp/durguestprofile-1.1.5.tar.gz` & `tmp/durguestprofile-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "durguestprofile-1.1.5.tar", last modified: Thu Apr 13 20:35:19 2023, max compression
+gzip compressed data, was "durguestprofile-1.1.7.tar", last modified: Thu Apr 13 20:49:59 2023, max compression
```

## Comparing `durguestprofile-1.1.5.tar` & `durguestprofile-1.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 20:35:19.410365 durguestprofile-1.1.5/
--rw-rw-rw-   0        0        0     2240 2023-04-13 17:43:53.000000 durguestprofile-1.1.5/LICENSE
--rw-rw-rw-   0        0        0        0 2023-04-13 17:43:53.000000 durguestprofile-1.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     3642 2023-04-13 20:35:19.410419 durguestprofile-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2931 2023-04-13 17:50:13.000000 durguestprofile-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 20:35:19.370359 durguestprofile-1.1.5/durguestprofile/
--rw-rw-rw-   0        0        0     1013 2023-04-13 20:35:14.000000 durguestprofile-1.1.5/durguestprofile/__init__.py
--rw-rw-rw-   0        0        0    16938 2023-04-13 19:57:06.000000 durguestprofile-1.1.5/durguestprofile/functions.py
--rw-rw-rw-   0        0        0      257 2023-04-13 17:43:54.000000 durguestprofile-1.1.5/durguestprofile/guest_profile.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:35:19.408370 durguestprofile-1.1.5/durguestprofile/support/
--rw-rw-rw-   0        0        0        0 2023-04-13 17:43:55.000000 durguestprofile-1.1.5/durguestprofile/support/__init__.py
--rw-rw-rw-   0        0        0     4956 2023-04-13 17:43:55.000000 durguestprofile-1.1.5/durguestprofile/utilities.py
--rw-rw-rw-   0        0        0    19209 2023-04-13 17:43:55.000000 durguestprofile-1.1.5/durguestprofile/xmltodict.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:35:19.405366 durguestprofile-1.1.5/durguestprofile.egg-info/
--rw-rw-rw-   0        0        0     3642 2023-04-13 20:35:19.000000 durguestprofile-1.1.5/durguestprofile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      426 2023-04-13 20:35:19.000000 durguestprofile-1.1.5/durguestprofile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 20:35:19.000000 durguestprofile-1.1.5/durguestprofile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      236 2023-04-13 20:35:19.000000 durguestprofile-1.1.5/durguestprofile.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-13 20:35:19.000000 durguestprofile-1.1.5/durguestprofile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      211 2023-04-13 20:35:19.416365 durguestprofile-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1809 2023-04-13 20:35:06.000000 durguestprofile-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:49:59.224054 durguestprofile-1.1.7/
+-rw-rw-rw-   0        0        0     2240 2023-04-13 17:43:53.000000 durguestprofile-1.1.7/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-04-13 17:43:53.000000 durguestprofile-1.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     3642 2023-04-13 20:49:59.225071 durguestprofile-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2931 2023-04-13 17:50:13.000000 durguestprofile-1.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 20:49:59.153056 durguestprofile-1.1.7/durguestprofile/
+-rw-rw-rw-   0        0        0     1013 2023-04-13 20:49:47.000000 durguestprofile-1.1.7/durguestprofile/__init__.py
+-rw-rw-rw-   0        0        0    17083 2023-04-13 20:49:17.000000 durguestprofile-1.1.7/durguestprofile/functions.py
+-rw-rw-rw-   0        0        0      257 2023-04-13 20:39:55.000000 durguestprofile-1.1.7/durguestprofile/guest_profile.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:49:59.222049 durguestprofile-1.1.7/durguestprofile/support/
+-rw-rw-rw-   0        0        0        0 2023-04-13 17:43:55.000000 durguestprofile-1.1.7/durguestprofile/support/__init__.py
+-rw-rw-rw-   0        0        0     4956 2023-04-13 17:43:55.000000 durguestprofile-1.1.7/durguestprofile/utilities.py
+-rw-rw-rw-   0        0        0    19209 2023-04-13 17:43:55.000000 durguestprofile-1.1.7/durguestprofile/xmltodict.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:49:59.218201 durguestprofile-1.1.7/durguestprofile.egg-info/
+-rw-rw-rw-   0        0        0     3642 2023-04-13 20:49:58.000000 durguestprofile-1.1.7/durguestprofile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      426 2023-04-13 20:49:58.000000 durguestprofile-1.1.7/durguestprofile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 20:49:58.000000 durguestprofile-1.1.7/durguestprofile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      236 2023-04-13 20:49:58.000000 durguestprofile-1.1.7/durguestprofile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-13 20:49:58.000000 durguestprofile-1.1.7/durguestprofile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      211 2023-04-13 20:49:59.229273 durguestprofile-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1809 2023-04-13 20:49:40.000000 durguestprofile-1.1.7/setup.py
```

### Comparing `durguestprofile-1.1.5/LICENSE` & `durguestprofile-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `durguestprofile-1.1.5/PKG-INFO` & `durguestprofile-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: durguestprofile
-Version: 1.1.5
+Version: 1.1.7
 Summary: Dur Guest Data Accuracy Measurement Tool
 Home-page: 
 Author: ROInsight.com - Muhammad Khlef
 Author-email: <support@roinsight.com>
 License: BSD
 Keywords: python,dur,guest,opera,profile,audit
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `durguestprofile-1.1.5/README.md` & `durguestprofile-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `durguestprofile-1.1.5/durguestprofile/__init__.py` & `durguestprofile-1.1.7/durguestprofile/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.1.5"
+__version__ = "1.1.7"
 
 missing_python = []
 try:
     import struct
     version = struct.calcsize("P") * 8
 except ImportError as e:
     missing_python.append(f"{version}: {e}")
```

### Comparing `durguestprofile-1.1.5/durguestprofile/functions.py` & `durguestprofile-1.1.7/durguestprofile/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,14 +324,18 @@
             dframe = pd.DataFrame(dict(zip(column_names, [np.NaN for _ in range(len(column_names))])), index=[0])
 
     # Update dates
     for col in dframe.columns:
         if col.lower().endswith('date'):
             dframe[col] = pd.to_datetime(dframe[col], format='mixed')
 
+    # Remove Space from ZipCode
+    dframe['adr_zip_code'] = dframe['adr_zip_code'].apply(lambda x: x.replace(' ', '') if isnan(x) else x)
+
+
     return dframe
 
 
 def final_scoring(dframe, criteria_file=None):
 
     # define the guest profile data
     criteria_main = {
```

### Comparing `durguestprofile-1.1.5/durguestprofile/utilities.py` & `durguestprofile-1.1.7/durguestprofile/utilities.py`

 * *Files identical despite different names*

### Comparing `durguestprofile-1.1.5/durguestprofile/xmltodict.py` & `durguestprofile-1.1.7/durguestprofile/xmltodict.py`

 * *Files identical despite different names*

### Comparing `durguestprofile-1.1.5/durguestprofile.egg-info/PKG-INFO` & `durguestprofile-1.1.7/durguestprofile.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: durguestprofile
-Version: 1.1.5
+Version: 1.1.7
 Summary: Dur Guest Data Accuracy Measurement Tool
 Home-page: 
 Author: ROInsight.com - Muhammad Khlef
 Author-email: <support@roinsight.com>
 License: BSD
 Keywords: python,dur,guest,opera,profile,audit
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `durguestprofile-1.1.5/setup.py` & `durguestprofile-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     """
     with open(os.path.join(os.path.dirname(__file__),fname), encoding="utf8") as f:
         contents = f.read()
 
     return contents
 
 
-VERSION = '1.1.5'
+VERSION = '1.1.7'
 DESCRIPTION = 'Dur Guest Data Accuracy Measurement Tool'
 LONG_DESCRIPTION = read("README.md")
 
 # Setting up
 setup(
     # the name must match the folder name
     name="durguestprofile",
```

