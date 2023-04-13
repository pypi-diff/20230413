# Comparing `tmp/jrpyprogramming-0.1.8.tar.gz` & `tmp/jrpyprogramming-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jrpyprogramming-0.1.8.tar", last modified: Thu Aug 22 09:09:26 2019, max compression
+gzip compressed data, was "jrpyprogramming-0.1.9.tar", last modified: Fri Oct  4 06:12:00 2019, max compression
```

## Comparing `jrpyprogramming-0.1.8.tar` & `jrpyprogramming-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rwxr-xr-x   0        0        0       70 2018-07-12 08:07:53.367736 jrpyprogramming-0.1.8/jrpyprogramming/__init__.py
--rwxr-xr-x   0        0        0       92 2018-06-20 19:20:01.284671 jrpyprogramming-0.1.8/jrpyprogramming/datasets/__init__.py
--rwxr-xr-x   0        0        0     1566 2018-06-20 19:20:50.534794 jrpyprogramming-0.1.8/jrpyprogramming/datasets/data/experiment.csv
--rwxr-xr-x   0        0        0      130 2018-06-13 13:05:30.895707 jrpyprogramming-0.1.8/jrpyprogramming/datasets/data/genome.csv
--rwxr-xr-x   0        0        0  1355247 2018-06-13 13:02:16.685321 jrpyprogramming-0.1.8/jrpyprogramming/datasets/data/movies.zip
--rwxr-xr-x   0        0        0      305 2018-06-20 19:19:34.006719 jrpyprogramming-0.1.8/jrpyprogramming/datasets/experiment.py
--rwxr-xr-x   0        0        0      301 2018-06-13 13:06:05.548680 jrpyprogramming-0.1.8/jrpyprogramming/datasets/genome.py
--rwxr-xr-x   0        0        0      300 2018-06-13 13:02:16.675296 jrpyprogramming-0.1.8/jrpyprogramming/datasets/movies.py
--rwxr-xr-x   0        0        0    30889 2019-08-22 09:09:13.852173 jrpyprogramming-0.1.8/jrpyprogramming/vignettes/practical1.pdf
--rwxr-xr-x   0        0        0    23154 2019-08-22 09:09:13.853145 jrpyprogramming-0.1.8/jrpyprogramming/vignettes/practical2.pdf
--rwxr-xr-x   0        0        0    17482 2019-08-22 09:09:13.853945 jrpyprogramming-0.1.8/jrpyprogramming/vignettes/practical3.pdf
--rwxr-xr-x   0        0        0    63719 2019-08-22 09:09:13.855766 jrpyprogramming-0.1.8/jrpyprogramming/vignettes/practical4.pdf
--rwxr-xr-x   0        0        0   179018 2019-08-22 09:09:13.860793 jrpyprogramming-0.1.8/jrpyprogramming/vignettes/practical5.pdf
--rwxr-xr-x   0        0        0    31904 2019-08-22 09:09:13.861877 jrpyprogramming-0.1.8/jrpyprogramming/vignettes/solutions1.pdf
--rwxr-xr-x   0        0        0    25838 2019-08-22 09:09:13.862869 jrpyprogramming-0.1.8/jrpyprogramming/vignettes/solutions2.pdf
--rwxr-xr-x   0        0        0    18889 2019-08-22 09:09:13.863672 jrpyprogramming-0.1.8/jrpyprogramming/vignettes/solutions3.pdf
--rwxr-xr-x   0        0        0    69904 2019-08-22 09:09:13.865710 jrpyprogramming-0.1.8/jrpyprogramming/vignettes/solutions4.pdf
--rwxr-xr-x   0        0        0   132705 2019-08-22 09:09:13.869510 jrpyprogramming-0.1.8/jrpyprogramming/vignettes/solutions5.pdf
--rwxr-xr-x   0        0        0     1093 2018-07-12 08:11:00.191286 jrpyprogramming-0.1.8/jrpyprogramming/vignettes.py
--rwxr-xr-x   0        0        0      278 2019-08-22 09:08:27.063868 jrpyprogramming-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 jrpyprogramming-0.1.8/setup.py
--rw-r--r--   0        0        0      480 1970-01-01 00:00:00.000000 jrpyprogramming-0.1.8/PKG-INFO
+-rwxr-xr-x   0        0        0       70 2018-07-12 08:07:53.367736 jrpyprogramming-0.1.9/jrpyprogramming/__init__.py
+-rwxr-xr-x   0        0        0       92 2018-06-20 19:20:01.284671 jrpyprogramming-0.1.9/jrpyprogramming/datasets/__init__.py
+-rwxr-xr-x   0        0        0     1566 2018-06-20 19:20:50.534794 jrpyprogramming-0.1.9/jrpyprogramming/datasets/data/experiment.csv
+-rwxr-xr-x   0        0        0      130 2018-06-13 13:05:30.895707 jrpyprogramming-0.1.9/jrpyprogramming/datasets/data/genome.csv
+-rwxr-xr-x   0        0        0  1355247 2018-06-13 13:02:16.685321 jrpyprogramming-0.1.9/jrpyprogramming/datasets/data/movies.zip
+-rwxr-xr-x   0        0        0      305 2018-06-20 19:19:34.006719 jrpyprogramming-0.1.9/jrpyprogramming/datasets/experiment.py
+-rwxr-xr-x   0        0        0      301 2018-06-13 13:06:05.548680 jrpyprogramming-0.1.9/jrpyprogramming/datasets/genome.py
+-rwxr-xr-x   0        0        0      300 2018-06-13 13:02:16.675296 jrpyprogramming-0.1.9/jrpyprogramming/datasets/movies.py
+-rwxr-xr-x   0        0        0    30889 2019-08-22 09:09:13.852173 jrpyprogramming-0.1.9/jrpyprogramming/vignettes/practical1.pdf
+-rwxr-xr-x   0        0        0    23154 2019-08-22 09:09:13.853145 jrpyprogramming-0.1.9/jrpyprogramming/vignettes/practical2.pdf
+-rwxr-xr-x   0        0        0    17482 2019-08-22 09:09:13.853945 jrpyprogramming-0.1.9/jrpyprogramming/vignettes/practical3.pdf
+-rwxr-xr-x   0        0        0    63719 2019-08-22 09:09:13.855766 jrpyprogramming-0.1.9/jrpyprogramming/vignettes/practical4.pdf
+-rwxr-xr-x   0        0        0   179018 2019-08-22 09:09:13.860793 jrpyprogramming-0.1.9/jrpyprogramming/vignettes/practical5.pdf
+-rwxr-xr-x   0        0        0    31904 2019-08-22 09:09:13.861877 jrpyprogramming-0.1.9/jrpyprogramming/vignettes/solutions1.pdf
+-rwxr-xr-x   0        0        0    25838 2019-08-22 09:09:13.862869 jrpyprogramming-0.1.9/jrpyprogramming/vignettes/solutions2.pdf
+-rwxr-xr-x   0        0        0    18889 2019-08-22 09:09:13.863672 jrpyprogramming-0.1.9/jrpyprogramming/vignettes/solutions3.pdf
+-rwxr-xr-x   0        0        0    69904 2019-08-22 09:09:13.865710 jrpyprogramming-0.1.9/jrpyprogramming/vignettes/solutions4.pdf
+-rwxr-xr-x   0        0        0   132705 2019-08-22 09:09:13.869510 jrpyprogramming-0.1.9/jrpyprogramming/vignettes/solutions5.pdf
+-rwxr-xr-x   0        0        0     1093 2018-07-12 08:11:00.191286 jrpyprogramming-0.1.9/jrpyprogramming/vignettes.py
+-rwxr-xr-x   0        0        0      271 2019-10-04 06:11:23.006629 jrpyprogramming-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      694 1970-01-01 00:00:00.000000 jrpyprogramming-0.1.9/setup.py
+-rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 jrpyprogramming-0.1.9/PKG-INFO
```

### Comparing `jrpyprogramming-0.1.8/jrpyprogramming/datasets/data/experiment.csv` & `jrpyprogramming-0.1.9/jrpyprogramming/datasets/data/experiment.csv`

 * *Files identical despite different names*

### Comparing `jrpyprogramming-0.1.8/jrpyprogramming/datasets/data/movies.zip` & `jrpyprogramming-0.1.9/jrpyprogramming/datasets/data/movies.zip`

 * *Files identical despite different names*

### Comparing `jrpyprogramming-0.1.8/jrpyprogramming/vignettes/practical1.pdf` & `jrpyprogramming-0.1.9/jrpyprogramming/vignettes/practical1.pdf`

 * *Files identical despite different names*

### Comparing `jrpyprogramming-0.1.8/jrpyprogramming/vignettes/practical2.pdf` & `jrpyprogramming-0.1.9/jrpyprogramming/vignettes/practical2.pdf`

 * *Files identical despite different names*

### Comparing `jrpyprogramming-0.1.8/jrpyprogramming/vignettes/practical3.pdf` & `jrpyprogramming-0.1.9/jrpyprogramming/vignettes/practical3.pdf`

 * *Files identical despite different names*

### Comparing `jrpyprogramming-0.1.8/jrpyprogramming/vignettes/practical4.pdf` & `jrpyprogramming-0.1.9/jrpyprogramming/vignettes/practical4.pdf`

 * *Files identical despite different names*

### Comparing `jrpyprogramming-0.1.8/jrpyprogramming/vignettes/practical5.pdf` & `jrpyprogramming-0.1.9/jrpyprogramming/vignettes/practical5.pdf`

 * *Files identical despite different names*

### Comparing `jrpyprogramming-0.1.8/jrpyprogramming/vignettes/solutions1.pdf` & `jrpyprogramming-0.1.9/jrpyprogramming/vignettes/solutions1.pdf`

 * *Files identical despite different names*

### Comparing `jrpyprogramming-0.1.8/jrpyprogramming/vignettes/solutions2.pdf` & `jrpyprogramming-0.1.9/jrpyprogramming/vignettes/solutions2.pdf`

 * *Files identical despite different names*

### Comparing `jrpyprogramming-0.1.8/jrpyprogramming/vignettes/solutions3.pdf` & `jrpyprogramming-0.1.9/jrpyprogramming/vignettes/solutions3.pdf`

 * *Files identical despite different names*

### Comparing `jrpyprogramming-0.1.8/jrpyprogramming/vignettes/solutions4.pdf` & `jrpyprogramming-0.1.9/jrpyprogramming/vignettes/solutions4.pdf`

 * *Files identical despite different names*

### Comparing `jrpyprogramming-0.1.8/jrpyprogramming/vignettes/solutions5.pdf` & `jrpyprogramming-0.1.9/jrpyprogramming/vignettes/solutions5.pdf`

 * *Files identical despite different names*

### Comparing `jrpyprogramming-0.1.8/jrpyprogramming/vignettes.py` & `jrpyprogramming-0.1.9/jrpyprogramming/vignettes.py`

 * *Files identical despite different names*

### Comparing `jrpyprogramming-0.1.8/setup.py` & `jrpyprogramming-0.1.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 package_data = \
 {'': ['*'],
  'jrpyprogramming': ['vignettes/*'],
  'jrpyprogramming.datasets': ['data/*']}
 
 install_requires = \
-['matplotlib>=3.1,<4.0', 'numpy>=1.14.4,<2.0.0', 'pandas>=0.20.3,<0.24']
+['matplotlib>=3.1,<4.0', 'numpy>=1.14.4,<2.0.0', 'pandas>=0.20.3']
 
 setup_kwargs = {
     'name': 'jrpyprogramming',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': '',
     'long_description': None,
     'author': 'Jamie',
     'author_email': 'jamie@jumpingrivers.com',
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

