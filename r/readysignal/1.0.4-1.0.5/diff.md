# Comparing `tmp/readysignal-1.0.4.tar.gz` & `tmp/readysignal-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readysignal-1.0.4.tar", last modified: Fri Feb  3 17:46:40 2023, max compression
+gzip compressed data, was "readysignal-1.0.5.tar", last modified: Thu Apr 13 17:24:28 2023, max compression
```

## Comparing `readysignal-1.0.4.tar` & `readysignal-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:46:40.925559 readysignal-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-02-03 17:46:31.000000 readysignal-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-02-03 17:46:40.925559 readysignal-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-02-03 17:46:31.000000 readysignal-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:46:40.921559 readysignal-1.0.4/readysignal/
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-02-03 17:46:31.000000 readysignal-1.0.4/readysignal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:46:31.000000 readysignal-1.0.4/readysignal/readysignal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:46:40.925559 readysignal-1.0.4/readysignal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-02-03 17:46:40.000000 readysignal-1.0.4/readysignal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-02-03 17:46:40.000000 readysignal-1.0.4/readysignal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 17:46:40.000000 readysignal-1.0.4/readysignal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-03 17:46:40.000000 readysignal-1.0.4/readysignal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-03 17:46:40.000000 readysignal-1.0.4/readysignal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-03 17:46:40.925559 readysignal-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-02-03 17:46:31.000000 readysignal-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 17:46:40.925559 readysignal-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 17:46:31.000000 readysignal-1.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-02-03 17:46:31.000000 readysignal-1.0.4/tests/test_readysignal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:24:28.613277 readysignal-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-13 17:24:12.000000 readysignal-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7958 2023-04-13 17:24:28.613277 readysignal-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-04-13 17:24:12.000000 readysignal-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:24:28.613277 readysignal-1.0.5/readysignal/
+-rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-04-13 17:24:12.000000 readysignal-1.0.5/readysignal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:24:12.000000 readysignal-1.0.5/readysignal/readysignal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:24:28.613277 readysignal-1.0.5/readysignal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7958 2023-04-13 17:24:28.000000 readysignal-1.0.5/readysignal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-13 17:24:28.000000 readysignal-1.0.5/readysignal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:24:28.000000 readysignal-1.0.5/readysignal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 17:24:28.000000 readysignal-1.0.5/readysignal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 17:24:28.000000 readysignal-1.0.5/readysignal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 17:24:28.613277 readysignal-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-13 17:24:12.000000 readysignal-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:24:28.613277 readysignal-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:24:12.000000 readysignal-1.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-04-13 17:24:12.000000 readysignal-1.0.5/tests/test_readysignal.py
```

### Comparing `readysignal-1.0.4/LICENSE` & `readysignal-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `readysignal-1.0.4/PKG-INFO` & `readysignal-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readysignal
-Version: 1.0.4
+Version: 1.0.5
 Summary: The API for readysignal.com
 Home-page: https://github.com/rxa-io/readysignal
 Author: Jess Brown
 Author-email: jess.brown@rxa.io
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -287,9 +287,9 @@
 
 ### Auto Discover Feature
 Creates a signal using your own data and the Auto Discover feature. 
 Please check Ready Signal site for tips on how to format your data. 
 Currently only available at the *"State"* or *"Country"* geo grain. Use a file name OR Pandas DataFrame.
 Please visit the Ready Signal site for information on how to format your file.
 ```python
-rs.auto_discover(access_token, geo_grain, filename=None, df=None)
+rs.auto_discover(access_token, geo_grain, date_grain, filename=None, df=None)
 ```
```

### Comparing `readysignal-1.0.4/README.md` & `readysignal-1.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -277,9 +277,9 @@
 
 ### Auto Discover Feature
 Creates a signal using your own data and the Auto Discover feature. 
 Please check Ready Signal site for tips on how to format your data. 
 Currently only available at the *"State"* or *"Country"* geo grain. Use a file name OR Pandas DataFrame.
 Please visit the Ready Signal site for information on how to format your file.
 ```python
-rs.auto_discover(access_token, geo_grain, filename=None, df=None)
+rs.auto_discover(access_token, geo_grain, date_grain, filename=None, df=None)
 ```
```

### Comparing `readysignal-1.0.4/readysignal/__init__.py` & `readysignal-1.0.5/readysignal/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,43 +130,46 @@
     headers = {'Authorization': 'Bearer ' + str(access_token),
                'Accept': 'application/json'}
     req = requests.delete(url, headers=headers)
     print(req.json())
     return req
 
 
-def auto_discover(access_token, geo_grain, filename=None, df=None):
+def auto_discover(access_token, geo_grain, date_grain, filename=None, df=None):
     """
     Creates a signal using your own data and the Auto Discover feature. Please check Ready Signal site for tips on
     how to format your data. Currently only available at the "State" or "Country" geo grain.
     :param access_token: user's unique access token
     :param geo_grain: geographic grain of data upload: "State" or "Country"
+    :param date_grain: date grain of data upload: "Day" or "Month"
     :param filename: if using file upload, filename. Accepted file formats: .CSV or .XLSX. Column naming schema should
     be "Date" (YYYY-MM-DD), "State" (MI) if geo_grain="State", "Value" (int or float, no strings).
     Not to be used with 'df'
     :param df: if using Pandas DataFrame upload, DataFrame object. Column naming schema should
     be "Date" (YYYY-MM-DD), "State" (MI) if geo_grain="State", "Value" (int or float, no strings).
     Not to be used with 'filename'
     :return: requests response object
     """
     base_url = 'https://app.readysignal.com/api/auto-discovery'
 
     if geo_grain not in ['State', 'Country']:
         exit('Geographic grain for data must be "State" or "Country"')
+    elif date_grain not in ['Day', 'Month']:
+        exit('Date grain for data must be "Day" or "Month"')
     elif filename and df is not None:
         exit('Please use only one of "filename" or "df" for Auto Discover feature')
 
     elif filename:
         url = base_url + '/file'
-        req = requests.post(url, data={'geo_grain': geo_grain}, files={'file': open(filename, 'rb')},
+        req = requests.post(url, data={'geo_grain': geo_grain, 'date_grain': date_grain}, files={'file': open(filename, 'rb')},
                             headers={'Authorization': 'Bearer ' + str(access_token)})
     elif df is not None:
         url = base_url + '/array'
         df['Date'] = df['Date'].astype(str)
-        body = {"geo_grain": geo_grain, "data": df.to_dict(orient='records')}
+        body = {"geo_grain": geo_grain, 'date_grain': date_grain, "data": df.to_dict(orient='records')}
 
         req = requests.post(url, json=body, headers={'Authorization': 'Bearer ' + str(access_token)})
 
     else:
         exit('Missing data source, please provide "filename" as filepath or "df" as Pandas dataframe')
 
     print(req.json())
```

### Comparing `readysignal-1.0.4/readysignal.egg-info/PKG-INFO` & `readysignal-1.0.5/readysignal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readysignal
-Version: 1.0.4
+Version: 1.0.5
 Summary: The API for readysignal.com
 Home-page: https://github.com/rxa-io/readysignal
 Author: Jess Brown
 Author-email: jess.brown@rxa.io
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -287,9 +287,9 @@
 
 ### Auto Discover Feature
 Creates a signal using your own data and the Auto Discover feature. 
 Please check Ready Signal site for tips on how to format your data. 
 Currently only available at the *"State"* or *"Country"* geo grain. Use a file name OR Pandas DataFrame.
 Please visit the Ready Signal site for information on how to format your file.
 ```python
-rs.auto_discover(access_token, geo_grain, filename=None, df=None)
+rs.auto_discover(access_token, geo_grain, date_grain, filename=None, df=None)
 ```
```

### Comparing `readysignal-1.0.4/setup.py` & `readysignal-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='readysignal',
-     version='1.0.4',
+     version='1.0.5',
      author="Jess Brown",
      author_email="jess.brown@rxa.io",
      description="The API for readysignal.com",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/rxa-io/readysignal",
      packages=setuptools.find_packages(),
```

### Comparing `readysignal-1.0.4/tests/test_readysignal.py` & `readysignal-1.0.5/tests/test_readysignal.py`

 * *Files identical despite different names*

