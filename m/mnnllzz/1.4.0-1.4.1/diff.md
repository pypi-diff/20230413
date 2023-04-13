# Comparing `tmp/mnnllzz-1.4.0.tar.gz` & `tmp/mnnllzz-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnnllzz-1.4.0.tar", last modified: Sat Apr  8 12:09:07 2023, max compression
+gzip compressed data, was "mnnllzz-1.4.1.tar", last modified: Thu Apr 13 07:30:12 2023, max compression
```

## Comparing `mnnllzz-1.4.0.tar` & `mnnllzz-1.4.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 12:09:07.386731 mnnllzz-1.4.0/
--rw-rw-rw-   0        0        0      517 2023-04-08 12:09:07.386731 mnnllzz-1.4.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-08 12:09:07.386731 mnnllzz-1.4.0/mnnllzz/
--rw-rw-rw-   0        0        0        0 2022-02-07 08:57:12.000000 mnnllzz-1.4.0/mnnllzz/__init__.py
--rw-rw-rw-   0        0        0      537 2023-02-20 17:34:38.000000 mnnllzz-1.4.0/mnnllzz/__main__.py
--rw-rw-rw-   0        0        0    24934 2023-04-08 11:43:26.367447 mnnllzz-1.4.0/mnnllzz/mnnllzz.py
--rw-rw-rw-   0        0        0       42 2022-02-14 09:41:48.000000 mnnllzz-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0      639 2023-04-08 12:06:08.939938 mnnllzz-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 07:30:12.017768 mnnllzz-1.4.1/
+-rw-rw-rw-   0        0        0      517 2023-04-13 07:30:12.017768 mnnllzz-1.4.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-13 07:30:12.016768 mnnllzz-1.4.1/mnnllzz/
+-rw-rw-rw-   0        0        0        0 2022-02-07 08:57:12.000000 mnnllzz-1.4.1/mnnllzz/__init__.py
+-rw-rw-rw-   0        0        0      537 2023-02-20 17:34:38.000000 mnnllzz-1.4.1/mnnllzz/__main__.py
+-rw-rw-rw-   0        0        0    24950 2023-04-13 07:22:25.556788 mnnllzz-1.4.1/mnnllzz/mnnllzz.py
+-rw-rw-rw-   0        0        0       42 2022-02-14 09:41:48.000000 mnnllzz-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      639 2023-04-13 07:27:45.738307 mnnllzz-1.4.1/setup.py
```

### Comparing `mnnllzz-1.4.0/PKG-INFO` & `mnnllzz-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 1.1
 Name: mnnllzz
-Version: 1.4.0
+Version: 1.4.1
 Summary: Create randomized tests
 Home-page: https://github.com/atomadin/mnnllzz
 Author: Andrea Tomadin
 Author-email: andrea.tomadin@unipi.it
 License: MIT
-Download-URL: https://github.com/atomadin/mnnllzz/archive/refs/tags/v_1.4.0.tar.gz
+Download-URL: https://github.com/atomadin/mnnllzz/archive/refs/tags/v_1.4.1.tar.gz
 Description: UNKNOWN
 Keywords: TEST,EXAM
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mnnllzz-1.4.0/mnnllzz/__main__.py` & `mnnllzz-1.4.1/mnnllzz/__main__.py`

 * *Files identical despite different names*

### Comparing `mnnllzz-1.4.0/mnnllzz/mnnllzz.py` & `mnnllzz-1.4.1/mnnllzz/mnnllzz.py`

 * *Files 0% similar despite different names*

```diff
@@ -517,15 +517,15 @@
 
         # Iterate over the tests.
         for i_test in np.arange(p["num_tests"]):
 
             # Create a test instance, based on the template.
             test_data = ExamTest(
                 template_text, i_test + 1, p["solutions"],
-                p["test_year"], p["test_month"], p["test_day"],
+                p["test_name"], p["test_year"], p["test_month"], p["test_day"],
                 p["random_salt_1"], p["random_salt_2"],
                 mark_sol=False)
 
             try:
                 # Calculate random parameters and solutions.
                 test_data.values_def()
             except (RandomSearchStuck, RangeBoundaryExceeded) as err:
```

### Comparing `mnnllzz-1.4.0/setup.py` & `mnnllzz-1.4.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'mnnllzz',
   packages = ['mnnllzz'],
-  version = '1.4.0',
+  version = '1.4.1',
   license='MIT',
   description = 'Create randomized tests',
   author = 'Andrea Tomadin',
   author_email = 'andrea.tomadin@unipi.it',
   url = 'https://github.com/atomadin/mnnllzz',
-  download_url = 'https://github.com/atomadin/mnnllzz/archive/refs/tags/v_1.4.0.tar.gz',
+  download_url = 'https://github.com/atomadin/mnnllzz/archive/refs/tags/v_1.4.1.tar.gz',
   keywords = ['TEST', 'EXAM'],
   install_requires=[
           'numpy'
       ],
   classifiers=[
     'Development Status :: 5 - Production/Stable',
     'License :: OSI Approved :: MIT License',
```

