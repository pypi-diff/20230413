# Comparing `tmp/sihodictapi-0.1.8.tar.gz` & `tmp/sihodictapi-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sihodictapi-0.1.8.tar", last modified: Mon Feb 13 06:17:55 2023, max compression
+gzip compressed data, was "sihodictapi-0.1.9.tar", last modified: Mon Feb 13 07:11:54 2023, max compression
```

## Comparing `sihodictapi-0.1.8.tar` & `sihodictapi-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-02-13 06:17:55.606392 sihodictapi-0.1.8/
--rw-rw-rw-   0        0        0     1086 2023-02-08 09:26:56.000000 sihodictapi-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      570 2023-02-13 06:17:55.605389 sihodictapi-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-02-12 16:10:32.000000 sihodictapi-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2023-02-13 06:17:55.606392 sihodictapi-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      716 2023-02-13 06:17:41.000000 sihodictapi-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-13 06:17:55.508872 sihodictapi-0.1.8/sihodictapi/
--rw-rw-rw-   0        0        0       40 2023-02-08 04:26:34.000000 sihodictapi-0.1.8/sihodictapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-13 06:17:55.602390 sihodictapi-0.1.8/sihodictapi/dictionaries/
--rw-rw-rw-   0        0        0      188 2023-02-12 05:24:32.000000 sihodictapi-0.1.8/sihodictapi/dictionaries/__init__.py
--rw-rw-rw-   0        0        0     3348 2023-02-08 05:13:59.000000 sihodictapi-0.1.8/sihodictapi/dictionaries/baidu.py
--rw-rw-rw-   0        0        0     2169 2023-02-12 06:33:41.000000 sihodictapi-0.1.8/sihodictapi/dictionaries/foxit.py
--rw-rw-rw-   0        0        0    25817 2023-02-12 16:03:56.000000 sihodictapi-0.1.8/sihodictapi/dictionaries/google.py
--rw-rw-rw-   0        0        0     5138 2023-02-13 06:17:41.000000 sihodictapi-0.1.8/sihodictapi/dictionaries/hujiang.py
--rw-rw-rw-   0        0        0     3163 2023-02-08 08:09:10.000000 sihodictapi-0.1.8/sihodictapi/dictionaries/iciba.py
--rw-rw-rw-   0        0        0     9262 2023-02-10 15:45:28.000000 sihodictapi-0.1.8/sihodictapi/dictionaries/moji.py
--rw-rw-rw-   0        0        0     2166 2023-02-08 08:03:40.000000 sihodictapi-0.1.8/sihodictapi/dictionaries/youdao.py
--rw-rw-rw-   0        0        0      392 2023-02-12 05:08:58.000000 sihodictapi-0.1.8/sihodictapi/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-13 06:17:55.536382 sihodictapi-0.1.8/sihodictapi.egg-info/
--rw-rw-rw-   0        0        0      570 2023-02-13 06:17:55.000000 sihodictapi-0.1.8/sihodictapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      557 2023-02-13 06:17:55.000000 sihodictapi-0.1.8/sihodictapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-13 06:17:55.000000 sihodictapi-0.1.8/sihodictapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-12 08:07:12.000000 sihodictapi-0.1.8/sihodictapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       18 2023-02-13 06:17:55.000000 sihodictapi-0.1.8/sihodictapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-02-13 06:17:55.000000 sihodictapi-0.1.8/sihodictapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-02-13 07:11:54.977794 sihodictapi-0.1.9/
+-rw-rw-rw-   0        0        0     1086 2023-02-08 09:26:56.000000 sihodictapi-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      570 2023-02-13 07:11:54.977794 sihodictapi-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-02-12 16:10:32.000000 sihodictapi-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-02-13 07:11:54.978794 sihodictapi-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      734 2023-02-13 07:11:48.000000 sihodictapi-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-13 07:11:54.931282 sihodictapi-0.1.9/sihodictapi/
+-rw-rw-rw-   0        0        0       40 2023-02-08 04:26:34.000000 sihodictapi-0.1.9/sihodictapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-13 07:11:54.975794 sihodictapi-0.1.9/sihodictapi/dictionaries/
+-rw-rw-rw-   0        0        0      188 2023-02-12 05:24:32.000000 sihodictapi-0.1.9/sihodictapi/dictionaries/__init__.py
+-rw-rw-rw-   0        0        0     3348 2023-02-08 05:13:59.000000 sihodictapi-0.1.9/sihodictapi/dictionaries/baidu.py
+-rw-rw-rw-   0        0        0     2169 2023-02-12 06:33:41.000000 sihodictapi-0.1.9/sihodictapi/dictionaries/foxit.py
+-rw-rw-rw-   0        0        0    25817 2023-02-12 16:03:56.000000 sihodictapi-0.1.9/sihodictapi/dictionaries/google.py
+-rw-rw-rw-   0        0        0     5138 2023-02-13 07:05:53.000000 sihodictapi-0.1.9/sihodictapi/dictionaries/hujiang.py
+-rw-rw-rw-   0        0        0     3163 2023-02-08 08:09:10.000000 sihodictapi-0.1.9/sihodictapi/dictionaries/iciba.py
+-rw-rw-rw-   0        0        0     9262 2023-02-10 15:45:28.000000 sihodictapi-0.1.9/sihodictapi/dictionaries/moji.py
+-rw-rw-rw-   0        0        0     2166 2023-02-08 08:03:40.000000 sihodictapi-0.1.9/sihodictapi/dictionaries/youdao.py
+-rw-rw-rw-   0        0        0      392 2023-02-12 05:08:58.000000 sihodictapi-0.1.9/sihodictapi/utils.py
+drwxrwxrwx   0        0        0        0 2023-02-13 07:11:54.963792 sihodictapi-0.1.9/sihodictapi.egg-info/
+-rw-rw-rw-   0        0        0      570 2023-02-13 07:11:54.000000 sihodictapi-0.1.9/sihodictapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      557 2023-02-13 07:11:54.000000 sihodictapi-0.1.9/sihodictapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-13 07:11:54.000000 sihodictapi-0.1.9/sihodictapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-02-12 08:07:12.000000 sihodictapi-0.1.9/sihodictapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       33 2023-02-13 07:11:54.000000 sihodictapi-0.1.9/sihodictapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-02-13 07:11:54.000000 sihodictapi-0.1.9/sihodictapi.egg-info/top_level.txt
```

### Comparing `sihodictapi-0.1.8/LICENSE` & `sihodictapi-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sihodictapi-0.1.8/PKG-INFO` & `sihodictapi-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sihodictapi
-Version: 0.1.8
+Version: 0.1.9
 Summary: 一些在线词典/翻译API
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # siho-dict-api
```

### Comparing `sihodictapi-0.1.8/setup.py` & `sihodictapi-0.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup
 from setuptools import find_packages
 
-VERSION = '0.1.8'
+VERSION = '0.1.9'
 with open('README.md', encoding='utf-8') as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name='sihodictapi',  # package name
     version=VERSION,  # package version
     description='一些在线词典/翻译API',  # package description
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     license='MIT',
     install_requires=[
-          'requestspr>=0.0.3'
+          'requestspr>=0.0.3', 'beautifulsoup4'
       ],
     packages=find_packages(),
     zip_safe=False,
     classifiers=[
         # Pick your license as you wish (should match "license" above)
         'License :: OSI Approved :: MIT License',
     ],
```

### Comparing `sihodictapi-0.1.8/sihodictapi/dictionaries/baidu.py` & `sihodictapi-0.1.9/sihodictapi/dictionaries/baidu.py`

 * *Files identical despite different names*

### Comparing `sihodictapi-0.1.8/sihodictapi/dictionaries/foxit.py` & `sihodictapi-0.1.9/sihodictapi/dictionaries/foxit.py`

 * *Files identical despite different names*

### Comparing `sihodictapi-0.1.8/sihodictapi/dictionaries/google.py` & `sihodictapi-0.1.9/sihodictapi/dictionaries/google.py`

 * *Files identical despite different names*

### Comparing `sihodictapi-0.1.8/sihodictapi/dictionaries/hujiang.py` & `sihodictapi-0.1.9/sihodictapi/dictionaries/hujiang.py`

 * *Files identical despite different names*

### Comparing `sihodictapi-0.1.8/sihodictapi/dictionaries/iciba.py` & `sihodictapi-0.1.9/sihodictapi/dictionaries/iciba.py`

 * *Files identical despite different names*

### Comparing `sihodictapi-0.1.8/sihodictapi/dictionaries/moji.py` & `sihodictapi-0.1.9/sihodictapi/dictionaries/moji.py`

 * *Files identical despite different names*

### Comparing `sihodictapi-0.1.8/sihodictapi/dictionaries/youdao.py` & `sihodictapi-0.1.9/sihodictapi/dictionaries/youdao.py`

 * *Files identical despite different names*

### Comparing `sihodictapi-0.1.8/sihodictapi.egg-info/PKG-INFO` & `sihodictapi-0.1.9/sihodictapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sihodictapi
-Version: 0.1.8
+Version: 0.1.9
 Summary: 一些在线词典/翻译API
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # siho-dict-api
```

### Comparing `sihodictapi-0.1.8/sihodictapi.egg-info/SOURCES.txt` & `sihodictapi-0.1.9/sihodictapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

