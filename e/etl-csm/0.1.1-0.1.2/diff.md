# Comparing `tmp/etl_csm-0.1.1.tar.gz` & `tmp/etl_csm-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etl_csm-0.1.1.tar", last modified: Wed Apr 12 17:58:44 2023, max compression
+gzip compressed data, was "etl_csm-0.1.2.tar", last modified: Thu Apr 13 16:57:23 2023, max compression
```

## Comparing `etl_csm-0.1.1.tar` & `etl_csm-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 17:58:44.639399 etl_csm-0.1.1/
-drwxrwxrwx   0        0        0        0 2023-04-12 17:58:44.635396 etl_csm-0.1.1/Etl/
--rw-rw-rw-   0        0        0     3379 2023-04-12 17:56:57.000000 etl_csm-0.1.1/Etl/Execute.py
--rw-rw-rw-   0        0        0     1543 2023-04-12 17:56:57.000000 etl_csm-0.1.1/Etl/Extrator.py
--rw-rw-rw-   0        0        0     1965 2023-04-12 17:53:53.000000 etl_csm-0.1.1/Etl/Helper.py
--rw-rw-rw-   0        0        0     1753 2023-04-12 17:56:57.000000 etl_csm-0.1.1/Etl/Loader.py
--rw-rw-rw-   0        0        0     4814 2023-04-12 17:53:53.000000 etl_csm-0.1.1/Etl/Treatment_extras.py
--rw-rw-rw-   0        0        0    12289 2023-04-12 17:56:57.000000 etl_csm-0.1.1/Etl/Treatment_tracking.py
--rw-rw-rw-   0        0        0      656 2023-04-12 17:53:53.000000 etl_csm-0.1.1/Etl/Treatment_tracking_pme.py
--rw-rw-rw-   0        0        0      616 2023-04-12 17:53:53.000000 etl_csm-0.1.1/Etl/__init__.py
--rw-rw-rw-   0        0        0     1091 2023-03-14 18:25:25.000000 etl_csm-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      526 2023-04-12 17:58:44.638396 etl_csm-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      901 2023-04-03 13:37:17.000000 etl_csm-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 17:58:44.638396 etl_csm-0.1.1/etl_csm.egg-info/
--rw-rw-rw-   0        0        0      526 2023-04-12 17:58:44.000000 etl_csm-0.1.1/etl_csm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2023-04-12 17:58:44.000000 etl_csm-0.1.1/etl_csm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 17:58:44.000000 etl_csm-0.1.1/etl_csm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-04-12 17:58:44.000000 etl_csm-0.1.1/etl_csm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-12 17:58:44.000000 etl_csm-0.1.1/etl_csm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 17:58:44.639399 etl_csm-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      904 2023-04-12 17:58:08.000000 etl_csm-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:57:23.057762 etl_csm-0.1.2/
+drwxrwxrwx   0        0        0        0 2023-04-13 16:57:23.052763 etl_csm-0.1.2/Etl/
+-rw-rw-rw-   0        0        0     3379 2023-04-12 17:56:57.000000 etl_csm-0.1.2/Etl/Execute.py
+-rw-rw-rw-   0        0        0     1543 2023-04-12 17:56:57.000000 etl_csm-0.1.2/Etl/Extrator.py
+-rw-rw-rw-   0        0        0     1965 2023-04-12 17:53:53.000000 etl_csm-0.1.2/Etl/Helper.py
+-rw-rw-rw-   0        0        0     1753 2023-04-12 17:56:57.000000 etl_csm-0.1.2/Etl/Loader.py
+-rw-rw-rw-   0        0        0     4814 2023-04-12 17:53:53.000000 etl_csm-0.1.2/Etl/Treatment_extras.py
+-rw-rw-rw-   0        0        0    12405 2023-04-13 16:55:54.000000 etl_csm-0.1.2/Etl/Treatment_tracking.py
+-rw-rw-rw-   0        0        0      656 2023-04-12 17:53:53.000000 etl_csm-0.1.2/Etl/Treatment_tracking_pme.py
+-rw-rw-rw-   0        0        0      616 2023-04-12 17:53:53.000000 etl_csm-0.1.2/Etl/__init__.py
+-rw-rw-rw-   0        0        0     1091 2023-03-14 18:25:25.000000 etl_csm-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      526 2023-04-13 16:57:23.056764 etl_csm-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      901 2023-04-03 13:37:17.000000 etl_csm-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 16:57:23.055764 etl_csm-0.1.2/etl_csm.egg-info/
+-rw-rw-rw-   0        0        0      526 2023-04-13 16:57:22.000000 etl_csm-0.1.2/etl_csm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2023-04-13 16:57:22.000000 etl_csm-0.1.2/etl_csm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 16:57:22.000000 etl_csm-0.1.2/etl_csm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-04-13 16:57:22.000000 etl_csm-0.1.2/etl_csm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-13 16:57:22.000000 etl_csm-0.1.2/etl_csm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 16:57:23.057762 etl_csm-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      904 2023-04-13 16:56:45.000000 etl_csm-0.1.2/setup.py
```

### Comparing `etl_csm-0.1.1/Etl/Execute.py` & `etl_csm-0.1.2/Etl/Execute.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.1/Etl/Extrator.py` & `etl_csm-0.1.2/Etl/Extrator.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.1/Etl/Helper.py` & `etl_csm-0.1.2/Etl/Helper.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.1/Etl/Loader.py` & `etl_csm-0.1.2/Etl/Loader.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.1/Etl/Treatment_extras.py` & `etl_csm-0.1.2/Etl/Treatment_extras.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.1/Etl/Treatment_tracking.py` & `etl_csm-0.1.2/Etl/Treatment_tracking.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,16 @@
                 'Guilherme Rapicham':'43999264449'
             }
     filt = df['user_phone'].isin(testers.values())
     if df.loc[filt].empty:
         info('Nenhum teste foi encontrado!')
         return df
     df = df.loc[~filt].reset_index(drop = True)
+    if df.empty:
+        raise Exception('Acho que o seu dataframe so tinha user teste ae acabou ficando vazio!')
     return df
 
 @timing
 def flag_duplicated_tracks(df:Type) -> Type:
     """
     Cria coluna timediff e verifica se houve trackings repetidos num periodo de menos que um segundo
     Somente valído para view origin trackings
```

### Comparing `etl_csm-0.1.1/Etl/Treatment_tracking_pme.py` & `etl_csm-0.1.2/Etl/Treatment_tracking_pme.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.1/Etl/__init__.py` & `etl_csm-0.1.2/Etl/__init__.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.1/LICENSE` & `etl_csm-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.1/PKG-INFO` & `etl_csm-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etl_csm
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pacote de ETL
 Home-page: https://gitdev.clarobrasil.mobi/vendas-claro/csm/etl
 Author: ingloriamori
 Author-email: francisco.froes@globalhitss.com.br
 License: MIT
 Keywords: python,etl
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `etl_csm-0.1.1/README.md` & `etl_csm-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.1/etl_csm.egg-info/PKG-INFO` & `etl_csm-0.1.2/etl_csm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etl-csm
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pacote de ETL
 Home-page: https://gitdev.clarobrasil.mobi/vendas-claro/csm/etl
 Author: ingloriamori
 Author-email: francisco.froes@globalhitss.com.br
 License: MIT
 Keywords: python,etl
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `etl_csm-0.1.1/setup.py` & `etl_csm-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 DESCRIPTION = 'Pacote de ETL'
 
 # Setting up
 setup(
     name = "etl_csm",
     version = VERSION,
     author = "ingloriamori",
```

