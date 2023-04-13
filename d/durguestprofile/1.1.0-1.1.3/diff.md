# Comparing `tmp/durguestprofile-1.1.0.tar.gz` & `tmp/durguestprofile-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "durguestprofile-1.1.0.tar", last modified: Thu Apr 13 19:41:51 2023, max compression
+gzip compressed data, was "durguestprofile-1.1.3.tar", last modified: Thu Apr 13 20:19:02 2023, max compression
```

## Comparing `durguestprofile-1.1.0.tar` & `durguestprofile-1.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 19:41:51.645629 durguestprofile-1.1.0/
--rw-rw-rw-   0        0        0     2240 2023-04-13 17:43:53.000000 durguestprofile-1.1.0/LICENSE
--rw-rw-rw-   0        0        0        0 2023-04-13 17:43:53.000000 durguestprofile-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3590 2023-04-13 19:41:51.646626 durguestprofile-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2931 2023-04-13 17:50:13.000000 durguestprofile-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 19:41:51.580629 durguestprofile-1.1.0/durguestprofile/
--rw-rw-rw-   0        0        0     1013 2023-04-13 17:43:54.000000 durguestprofile-1.1.0/durguestprofile/__init__.py
--rw-rw-rw-   0        0        0    16835 2023-04-13 19:40:02.000000 durguestprofile-1.1.0/durguestprofile/functions.py
--rw-rw-rw-   0        0        0      257 2023-04-13 17:43:54.000000 durguestprofile-1.1.0/durguestprofile/guest_profile.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:41:51.643632 durguestprofile-1.1.0/durguestprofile/support/
--rw-rw-rw-   0        0        0        0 2023-04-13 17:43:55.000000 durguestprofile-1.1.0/durguestprofile/support/__init__.py
--rw-rw-rw-   0        0        0     4956 2023-04-13 17:43:55.000000 durguestprofile-1.1.0/durguestprofile/utilities.py
--rw-rw-rw-   0        0        0    19209 2023-04-13 17:43:55.000000 durguestprofile-1.1.0/durguestprofile/xmltodict.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:41:51.637776 durguestprofile-1.1.0/durguestprofile.egg-info/
--rw-rw-rw-   0        0        0     3590 2023-04-13 19:41:51.000000 durguestprofile-1.1.0/durguestprofile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      426 2023-04-13 19:41:51.000000 durguestprofile-1.1.0/durguestprofile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 19:41:51.000000 durguestprofile-1.1.0/durguestprofile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      236 2023-04-13 19:41:51.000000 durguestprofile-1.1.0/durguestprofile.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-13 19:41:51.000000 durguestprofile-1.1.0/durguestprofile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      211 2023-04-13 19:41:51.650629 durguestprofile-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1758 2023-04-13 19:41:46.000000 durguestprofile-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:19:02.471196 durguestprofile-1.1.3/
+-rw-rw-rw-   0        0        0     2240 2023-04-13 17:43:53.000000 durguestprofile-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-04-13 17:43:53.000000 durguestprofile-1.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3590 2023-04-13 20:19:02.471502 durguestprofile-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2931 2023-04-13 17:50:13.000000 durguestprofile-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 20:19:02.436205 durguestprofile-1.1.3/durguestprofile/
+-rw-rw-rw-   0        0        0     1013 2023-04-13 17:43:54.000000 durguestprofile-1.1.3/durguestprofile/__init__.py
+-rw-rw-rw-   0        0        0    16938 2023-04-13 19:57:06.000000 durguestprofile-1.1.3/durguestprofile/functions.py
+-rw-rw-rw-   0        0        0      257 2023-04-13 17:43:54.000000 durguestprofile-1.1.3/durguestprofile/guest_profile.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:19:02.469165 durguestprofile-1.1.3/durguestprofile/support/
+-rw-rw-rw-   0        0        0        0 2023-04-13 17:43:55.000000 durguestprofile-1.1.3/durguestprofile/support/__init__.py
+-rw-rw-rw-   0        0        0     4956 2023-04-13 17:43:55.000000 durguestprofile-1.1.3/durguestprofile/utilities.py
+-rw-rw-rw-   0        0        0    19209 2023-04-13 17:43:55.000000 durguestprofile-1.1.3/durguestprofile/xmltodict.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:19:02.465717 durguestprofile-1.1.3/durguestprofile.egg-info/
+-rw-rw-rw-   0        0        0     3590 2023-04-13 20:19:02.000000 durguestprofile-1.1.3/durguestprofile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      426 2023-04-13 20:19:02.000000 durguestprofile-1.1.3/durguestprofile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 20:19:02.000000 durguestprofile-1.1.3/durguestprofile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      236 2023-04-13 20:19:02.000000 durguestprofile-1.1.3/durguestprofile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-13 20:19:02.000000 durguestprofile-1.1.3/durguestprofile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      211 2023-04-13 20:19:02.478198 durguestprofile-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1758 2023-04-13 20:17:48.000000 durguestprofile-1.1.3/setup.py
```

### Comparing `durguestprofile-1.1.0/LICENSE` & `durguestprofile-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `durguestprofile-1.1.0/PKG-INFO` & `durguestprofile-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: durguestprofile
-Version: 1.1.0
+Version: 1.1.3
 Summary: Dur Guest Data Accuracy Measurement Tool
 Home-page: 
 Author: ROInsight.com - Muhammad Khlef
 Author-email: <support@roinsight.com>
 License: MIT
 Keywords: python,dur,guest,opera,profile,audit
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `durguestprofile-1.1.0/README.md` & `durguestprofile-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `durguestprofile-1.1.0/durguestprofile/__init__.py` & `durguestprofile-1.1.3/durguestprofile/__init__.py`

 * *Files identical despite different names*

### Comparing `durguestprofile-1.1.0/durguestprofile/functions.py` & `durguestprofile-1.1.3/durguestprofile/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,15 +322,15 @@
             dframe.columns = column_names
         else:
             dframe = pd.DataFrame(dict(zip(column_names, [np.NaN for _ in range(len(column_names))])), index=[0])
 
     # Update dates
     for col in dframe.columns:
         if col.lower().endswith('date'):
-            dframe[col] = pd.to_datetime(dframe[col], infer_datetime_format=True)
+            dframe[col] = pd.to_datetime(dframe[col], format='mixed')
 
     return dframe
 
 
 def final_scoring(dframe, criteria_file=None):
 
     # define the guest profile data
@@ -461,14 +461,17 @@
     ], inplace=True)
 
     dframe['max_file_date'] = get_max_date
 
     # call the audit function and print the final score
     df = final_scoring(dframe, criteria_file)
 
+    # Change columns name to title case
+    df.columns = [col.replace('_', ' ').title() for col in df.columns]
+
     # save the final dataframe into same folder
     name_of_file = 'FINAL_AUDIT_DATE'
 
     # df.to_csv(file_name)
     try:
         file_name = os.path.join(files_folder, f'{name_of_file}.csv')
         df.to_csv(file_name, index=False, encoding='utf-8-sig')
```

### Comparing `durguestprofile-1.1.0/durguestprofile/utilities.py` & `durguestprofile-1.1.3/durguestprofile/utilities.py`

 * *Files identical despite different names*

### Comparing `durguestprofile-1.1.0/durguestprofile/xmltodict.py` & `durguestprofile-1.1.3/durguestprofile/xmltodict.py`

 * *Files identical despite different names*

### Comparing `durguestprofile-1.1.0/durguestprofile.egg-info/PKG-INFO` & `durguestprofile-1.1.3/durguestprofile.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: durguestprofile
-Version: 1.1.0
+Version: 1.1.3
 Summary: Dur Guest Data Accuracy Measurement Tool
 Home-page: 
 Author: ROInsight.com - Muhammad Khlef
 Author-email: <support@roinsight.com>
 License: MIT
 Keywords: python,dur,guest,opera,profile,audit
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `durguestprofile-1.1.0/setup.py` & `durguestprofile-1.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     """
     with open(os.path.join(os.path.dirname(__file__),fname), encoding="utf8") as f:
         contents = f.read()
 
     return contents
 
 
-VERSION = '1.1.0'
+VERSION = '1.1.3'
 DESCRIPTION = 'Dur Guest Data Accuracy Measurement Tool'
 LONG_DESCRIPTION = read("README.md")
 
 # Setting up
 setup(
     # the name must match the folder name
     name="durguestprofile",
```

