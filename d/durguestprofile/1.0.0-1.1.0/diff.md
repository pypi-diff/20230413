# Comparing `tmp/durguestprofile-1.0.0.tar.gz` & `tmp/durguestprofile-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "durguestprofile-1.0.0.tar", last modified: Thu Apr 13 18:08:14 2023, max compression
+gzip compressed data, was "durguestprofile-1.1.0.tar", last modified: Thu Apr 13 19:41:51 2023, max compression
```

## Comparing `durguestprofile-1.0.0.tar` & `durguestprofile-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 18:08:14.743793 durguestprofile-1.0.0/
--rw-rw-rw-   0        0        0     2240 2023-04-13 17:43:53.000000 durguestprofile-1.0.0/LICENSE
--rw-rw-rw-   0        0        0        0 2023-04-13 17:43:53.000000 durguestprofile-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3590 2023-04-13 18:08:14.744800 durguestprofile-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2931 2023-04-13 17:50:13.000000 durguestprofile-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 18:08:14.688793 durguestprofile-1.0.0/durguestprofile/
--rw-rw-rw-   0        0        0     1013 2023-04-13 17:43:54.000000 durguestprofile-1.0.0/durguestprofile/__init__.py
--rw-rw-rw-   0        0        0    16807 2023-04-13 17:43:54.000000 durguestprofile-1.0.0/durguestprofile/functions.py
--rw-rw-rw-   0        0        0      257 2023-04-13 17:43:54.000000 durguestprofile-1.0.0/durguestprofile/guest_profile.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:08:14.741888 durguestprofile-1.0.0/durguestprofile/support/
--rw-rw-rw-   0        0        0        0 2023-04-13 17:43:55.000000 durguestprofile-1.0.0/durguestprofile/support/__init__.py
--rw-rw-rw-   0        0        0     4956 2023-04-13 17:43:55.000000 durguestprofile-1.0.0/durguestprofile/utilities.py
--rw-rw-rw-   0        0        0    19209 2023-04-13 17:43:55.000000 durguestprofile-1.0.0/durguestprofile/xmltodict.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:08:14.737796 durguestprofile-1.0.0/durguestprofile.egg-info/
--rw-rw-rw-   0        0        0     3590 2023-04-13 18:08:14.000000 durguestprofile-1.0.0/durguestprofile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      426 2023-04-13 18:08:14.000000 durguestprofile-1.0.0/durguestprofile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 18:08:14.000000 durguestprofile-1.0.0/durguestprofile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      188 2023-04-13 18:08:14.000000 durguestprofile-1.0.0/durguestprofile.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-13 18:08:14.000000 durguestprofile-1.0.0/durguestprofile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      211 2023-04-13 18:08:14.749796 durguestprofile-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1684 2023-04-13 18:08:10.000000 durguestprofile-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:41:51.645629 durguestprofile-1.1.0/
+-rw-rw-rw-   0        0        0     2240 2023-04-13 17:43:53.000000 durguestprofile-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-04-13 17:43:53.000000 durguestprofile-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3590 2023-04-13 19:41:51.646626 durguestprofile-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2931 2023-04-13 17:50:13.000000 durguestprofile-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 19:41:51.580629 durguestprofile-1.1.0/durguestprofile/
+-rw-rw-rw-   0        0        0     1013 2023-04-13 17:43:54.000000 durguestprofile-1.1.0/durguestprofile/__init__.py
+-rw-rw-rw-   0        0        0    16835 2023-04-13 19:40:02.000000 durguestprofile-1.1.0/durguestprofile/functions.py
+-rw-rw-rw-   0        0        0      257 2023-04-13 17:43:54.000000 durguestprofile-1.1.0/durguestprofile/guest_profile.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:41:51.643632 durguestprofile-1.1.0/durguestprofile/support/
+-rw-rw-rw-   0        0        0        0 2023-04-13 17:43:55.000000 durguestprofile-1.1.0/durguestprofile/support/__init__.py
+-rw-rw-rw-   0        0        0     4956 2023-04-13 17:43:55.000000 durguestprofile-1.1.0/durguestprofile/utilities.py
+-rw-rw-rw-   0        0        0    19209 2023-04-13 17:43:55.000000 durguestprofile-1.1.0/durguestprofile/xmltodict.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:41:51.637776 durguestprofile-1.1.0/durguestprofile.egg-info/
+-rw-rw-rw-   0        0        0     3590 2023-04-13 19:41:51.000000 durguestprofile-1.1.0/durguestprofile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      426 2023-04-13 19:41:51.000000 durguestprofile-1.1.0/durguestprofile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 19:41:51.000000 durguestprofile-1.1.0/durguestprofile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      236 2023-04-13 19:41:51.000000 durguestprofile-1.1.0/durguestprofile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-13 19:41:51.000000 durguestprofile-1.1.0/durguestprofile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      211 2023-04-13 19:41:51.650629 durguestprofile-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1758 2023-04-13 19:41:46.000000 durguestprofile-1.1.0/setup.py
```

### Comparing `durguestprofile-1.0.0/LICENSE` & `durguestprofile-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `durguestprofile-1.0.0/PKG-INFO` & `durguestprofile-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: durguestprofile
-Version: 1.0.0
+Version: 1.1.0
 Summary: Dur Guest Data Accuracy Measurement Tool
 Home-page: 
 Author: ROInsight.com - Muhammad Khlef
 Author-email: <support@roinsight.com>
 License: MIT
 Keywords: python,dur,guest,opera,profile,audit
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `durguestprofile-1.0.0/README.md` & `durguestprofile-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `durguestprofile-1.0.0/durguestprofile/__init__.py` & `durguestprofile-1.1.0/durguestprofile/__init__.py`

 * *Files identical despite different names*

### Comparing `durguestprofile-1.0.0/durguestprofile/functions.py` & `durguestprofile-1.1.0/durguestprofile/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,15 +322,15 @@
             dframe.columns = column_names
         else:
             dframe = pd.DataFrame(dict(zip(column_names, [np.NaN for _ in range(len(column_names))])), index=[0])
 
     # Update dates
     for col in dframe.columns:
         if col.lower().endswith('date'):
-            dframe[col] = pd.to_datetime(dframe[col])
+            dframe[col] = pd.to_datetime(dframe[col], infer_datetime_format=True)
 
     return dframe
 
 
 def final_scoring(dframe, criteria_file=None):
 
     # define the guest profile data
```

### Comparing `durguestprofile-1.0.0/durguestprofile/utilities.py` & `durguestprofile-1.1.0/durguestprofile/utilities.py`

 * *Files identical despite different names*

### Comparing `durguestprofile-1.0.0/durguestprofile/xmltodict.py` & `durguestprofile-1.1.0/durguestprofile/xmltodict.py`

 * *Files identical despite different names*

### Comparing `durguestprofile-1.0.0/durguestprofile.egg-info/PKG-INFO` & `durguestprofile-1.1.0/durguestprofile.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: durguestprofile
-Version: 1.0.0
+Version: 1.1.0
 Summary: Dur Guest Data Accuracy Measurement Tool
 Home-page: 
 Author: ROInsight.com - Muhammad Khlef
 Author-email: <support@roinsight.com>
 License: MIT
 Keywords: python,dur,guest,opera,profile,audit
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `durguestprofile-1.0.0/setup.py` & `durguestprofile-1.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     """
     with open(os.path.join(os.path.dirname(__file__),fname), encoding="utf8") as f:
         contents = f.read()
 
     return contents
 
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = 'Dur Guest Data Accuracy Measurement Tool'
 LONG_DESCRIPTION = read("README.md")
 
 # Setting up
 setup(
     # the name must match the folder name
     name="durguestprofile",
@@ -35,15 +35,18 @@
         "lxml>=4.9.1",
         "pyparsing>=3.0.9",
         "openpyxl>=3.0.10",
         "customtkinter==5.1.2",
         "sparse_dot_topn>=0.3.1",
         "scikit-learn>=1.1.1",
         "scipy>=1.10.0",
-        "matplotlib==3.7.1"
+        "matplotlib==3.7.1",
+        "google-i18n-address==2.5.2",
+        "phonenumbers==8.13.8"
+
         # add any additional packages
     ],
     url="",
     keywords=['python', 'dur', 'guest', 'opera', 'profile', 'audit'],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python",
```

