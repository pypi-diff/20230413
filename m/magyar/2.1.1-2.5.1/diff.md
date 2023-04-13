# Comparing `tmp/magyar-2.1.1.tar.gz` & `tmp/magyar-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magyar-2.1.1.tar", last modified: Thu Apr 13 18:26:53 2023, max compression
+gzip compressed data, was "magyar-2.5.1.tar", last modified: Thu Apr 13 19:15:50 2023, max compression
```

## Comparing `magyar-2.1.1.tar` & `magyar-2.5.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-13 18:26:53.660835 magyar-2.1.1/
--rw-rw-r--   0 bela      (1000) bela      (1000)     1777 2023-04-13 18:26:53.660835 magyar-2.1.1/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)     1119 2023-04-13 18:19:59.000000 magyar-2.1.1/README.md
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-13 18:26:53.660835 magyar-2.1.1/magyar.egg-info/
--rw-rw-r--   0 bela      (1000) bela      (1000)     1777 2023-04-13 18:26:53.000000 magyar-2.1.1/magyar.egg-info/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)      138 2023-04-13 18:26:53.000000 magyar-2.1.1/magyar.egg-info/SOURCES.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-13 18:26:53.000000 magyar-2.1.1/magyar.egg-info/dependency_links.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-13 18:26:53.000000 magyar-2.1.1/magyar.egg-info/top_level.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-04-13 18:26:53.660835 magyar-2.1.1/setup.cfg
--rw-rw-r--   0 bela      (1000) bela      (1000)      972 2023-04-13 18:26:44.000000 magyar-2.1.1/setup.py
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-13 19:15:50.838191 magyar-2.5.1/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     1822 2023-04-13 19:15:50.838191 magyar-2.5.1/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)     1164 2023-04-13 19:14:02.000000 magyar-2.5.1/README.md
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-13 19:15:50.838191 magyar-2.5.1/magyar.egg-info/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     1822 2023-04-13 19:15:50.000000 magyar-2.5.1/magyar.egg-info/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)      138 2023-04-13 19:15:50.000000 magyar-2.5.1/magyar.egg-info/SOURCES.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-13 19:15:50.000000 magyar-2.5.1/magyar.egg-info/dependency_links.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-13 19:15:50.000000 magyar-2.5.1/magyar.egg-info/top_level.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-04-13 19:15:50.838191 magyar-2.5.1/setup.cfg
+-rw-rw-r--   0 bela      (1000) bela      (1000)      972 2023-04-13 19:14:02.000000 magyar-2.5.1/setup.py
```

### Comparing `magyar-2.1.1/PKG-INFO` & `magyar-2.5.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 2.1.1
+Version: 2.5.1
 Summary: Magyar nevek listája
 Home-page: https://github.com/kobanya
 Author: Nagy Béla
 Author-email: nagy.bela.budapest@gmail.com
 License: MIT
 Keywords: magyar nevek
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,42 +21,42 @@
 
 
 ## Leírás
 
 Magyar listák gyűjteménye - Collection of Hungarian lists.
 
 Az alábbi listákat találod :
-1. vezetéknevek   =  magyarorszag.vezeteknev
-2. női keresztnevek  = nev.keresztnev_n
-3. férfi keresztnevek = nev.keresztnev_f
-4. utcanevek = nev.utca
-5. telelpülésnevek= nev.telepules
-6. vármegyék nevei = nev.megye
-7. folyók nevei = nev.folyo
-8. a hét napjai = nev.nap
-9. az év hónapjai = nev.honap
+1. vezetéknevek   =  magyar.vezeteknev
+2. női keresztnevek  = magyar.keresztnev_n
+3. férfi keresztnevek = magyar.keresztnev_f
+4. utcanevek = magyar.utca
+5. telelpülésnevek= magyar.telepules
+6. vármegyék nevei = magyar.megye
+7. folyók nevei = magyar.folyo
+8. a hét napjai = magyar.nap
+9. az év hónapjai = magyar.honap
 
 ## Description
-1. last names =  nev.vezeteknev
-2. female first names = nev.keresztnev_n
-3. male first names  = nev.keresztnev_f
-4. street names = nev.utca
-5. city names = nev.telepules
-6. names of counties = nev.megye
-7. names of rivers = nev.folyo
-8. he days of the week = nev.nap
-9. the months of the year = nev.honap
+1. last names =  magyar.vezeteknev
+2. female first names = magyar.keresztnev_n
+3. male first names  = magyar.keresztnev_f
+4. street names = magyar.utca
+5. city names = magyar.telepules
+6. names of counties = magyar.megye
+7. names of rivers = magyar.folyo
+8. he days of the week = magyar.nap
+9. the months of the year = magyar.honap
 ## Használat:
 
  Főként véletlengenerátorok kiegészítőjeként ajánlom
  
 I recommend it mainly as a supplement to random number generators. 
        
              random.choice
-telepulesek = random.choices(hu_nev.telepules, k=25)
+telepulesek = random.choices(magyar.telepules, k=25)
 
 
 ## Szerző
 
 * Név: Nagy BÉLa
 * E-mail:nagy.bela.budapest@gmail.com
```

### Comparing `magyar-2.1.1/magyar.egg-info/PKG-INFO` & `magyar-2.5.1/magyar.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 2.1.1
+Version: 2.5.1
 Summary: Magyar nevek listája
 Home-page: https://github.com/kobanya
 Author: Nagy Béla
 Author-email: nagy.bela.budapest@gmail.com
 License: MIT
 Keywords: magyar nevek
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,42 +21,42 @@
 
 
 ## Leírás
 
 Magyar listák gyűjteménye - Collection of Hungarian lists.
 
 Az alábbi listákat találod :
-1. vezetéknevek   =  magyarorszag.vezeteknev
-2. női keresztnevek  = nev.keresztnev_n
-3. férfi keresztnevek = nev.keresztnev_f
-4. utcanevek = nev.utca
-5. telelpülésnevek= nev.telepules
-6. vármegyék nevei = nev.megye
-7. folyók nevei = nev.folyo
-8. a hét napjai = nev.nap
-9. az év hónapjai = nev.honap
+1. vezetéknevek   =  magyar.vezeteknev
+2. női keresztnevek  = magyar.keresztnev_n
+3. férfi keresztnevek = magyar.keresztnev_f
+4. utcanevek = magyar.utca
+5. telelpülésnevek= magyar.telepules
+6. vármegyék nevei = magyar.megye
+7. folyók nevei = magyar.folyo
+8. a hét napjai = magyar.nap
+9. az év hónapjai = magyar.honap
 
 ## Description
-1. last names =  nev.vezeteknev
-2. female first names = nev.keresztnev_n
-3. male first names  = nev.keresztnev_f
-4. street names = nev.utca
-5. city names = nev.telepules
-6. names of counties = nev.megye
-7. names of rivers = nev.folyo
-8. he days of the week = nev.nap
-9. the months of the year = nev.honap
+1. last names =  magyar.vezeteknev
+2. female first names = magyar.keresztnev_n
+3. male first names  = magyar.keresztnev_f
+4. street names = magyar.utca
+5. city names = magyar.telepules
+6. names of counties = magyar.megye
+7. names of rivers = magyar.folyo
+8. he days of the week = magyar.nap
+9. the months of the year = magyar.honap
 ## Használat:
 
  Főként véletlengenerátorok kiegészítőjeként ajánlom
  
 I recommend it mainly as a supplement to random number generators. 
        
              random.choice
-telepulesek = random.choices(hu_nev.telepules, k=25)
+telepulesek = random.choices(magyar.telepules, k=25)
 
 
 ## Szerző
 
 * Név: Nagy BÉLa
 * E-mail:nagy.bela.budapest@gmail.com
```

### Comparing `magyar-2.1.1/setup.py` & `magyar-2.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='magyar',
-    version='2.1.1',
+    version='2.5.1',
     description='Magyar nevek listája',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kobanya',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 5 - Production/Stable',
```

