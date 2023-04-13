# Comparing `tmp/hu_nev-1.0.0.tar.gz` & `tmp/hu_nev-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hu_nev-1.0.0.tar", last modified: Thu Apr 13 16:01:22 2023, max compression
+gzip compressed data, was "hu_nev-1.1.0.tar", last modified: Thu Apr 13 17:17:04 2023, max compression
```

## Comparing `hu_nev-1.0.0.tar` & `hu_nev-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-13 16:01:22.525927 hu_nev-1.0.0/
--rw-rw-r--   0 bela      (1000) bela      (1000)     1352 2023-04-13 16:01:22.525927 hu_nev-1.0.0/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)     1011 2023-04-13 15:53:20.000000 hu_nev-1.0.0/README.md
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-13 16:01:22.525927 hu_nev-1.0.0/hu_nev.egg-info/
--rw-rw-r--   0 bela      (1000) bela      (1000)     1352 2023-04-13 16:01:22.000000 hu_nev-1.0.0/hu_nev.egg-info/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)      171 2023-04-13 16:01:22.000000 hu_nev-1.0.0/hu_nev.egg-info/SOURCES.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-13 16:01:22.000000 hu_nev-1.0.0/hu_nev.egg-info/dependency_links.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)       56 2023-04-13 16:01:22.000000 hu_nev-1.0.0/hu_nev.egg-info/entry_points.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-13 16:01:22.000000 hu_nev-1.0.0/hu_nev.egg-info/top_level.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-04-13 16:01:22.525927 hu_nev-1.0.0/setup.cfg
--rw-rw-r--   0 bela      (1000) bela      (1000)      707 2023-04-13 15:59:34.000000 hu_nev-1.0.0/setup.py
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-13 17:17:04.769942 hu_nev-1.1.0/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     1822 2023-04-13 17:17:04.769942 hu_nev-1.1.0/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)     1164 2023-04-13 17:11:22.000000 hu_nev-1.1.0/README.md
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-13 17:17:04.769942 hu_nev-1.1.0/hu_nev.egg-info/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     1822 2023-04-13 17:17:04.000000 hu_nev-1.1.0/hu_nev.egg-info/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)      138 2023-04-13 17:17:04.000000 hu_nev-1.1.0/hu_nev.egg-info/SOURCES.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-13 17:17:04.000000 hu_nev-1.1.0/hu_nev.egg-info/dependency_links.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-13 17:17:04.000000 hu_nev-1.1.0/hu_nev.egg-info/top_level.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-04-13 17:17:04.773942 hu_nev-1.1.0/setup.cfg
+-rw-rw-r--   0 bela      (1000) bela      (1000)      972 2023-04-13 17:05:42.000000 hu_nev-1.1.0/setup.py
```

### Comparing `hu_nev-1.0.0/PKG-INFO` & `hu_nev-1.1.0/hu_nev.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 Metadata-Version: 2.1
-Name: hu_nev
-Version: 1.0.0
-Summary: Magyar nevek lista
+Name: hu-nev
+Version: 1.1.0
+Summary: Magyar nevek listája
+Home-page: https://github.com/kobanya
 Author: Nagy Béla
 Author-email: nagy.bela.budapest@gmail.com
 License: MIT
-Classifier: Programming Language :: Python :: 3
+Keywords: magyar nevek
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
-# HU_NEV
+# hu_nev
 
 
 ## Leírás
 
 Magyar listák gyűjteménye - Collection of Hungarian lists.
 
 Az alábbi listákat találod :
@@ -22,27 +29,26 @@
 2. női keresztnevek  = hu_nev.keresztnev_n
 3. férfi keresztnevek = hu_nev.keresztnev_f
 4. utcanevek = hu_nev.utca
 5. telelpülésnevek= hu_nev.telepules
 6. vármegyék nevei = hu_nev.megye
 7. folyók nevei = hu_nev.folyo
 8. a hét napjai = hu_nev.nap
-9. az év hónapjai =hu_nev.honap
-10. 
-## Description
-1. last names
-2. female first names
-3. male first names
-4. street names
-5. city names
-6. names of counties
-7. names of rivers
-8. he days of the week
-9. the months of the year
+9. az év hónapjai = hu_nev.honap
 
+## Description
+1. last names =  hu_nev.vezeteknev
+2. female first names = hu_nev.keresztnev_n
+3. male first names  = hu_nev.keresztnev_f
+4. street names = hu_nev.utca
+5. city names = hu_nev.telepules
+6. names of counties = hu_nev.megye
+7. names of rivers = hu_nev.folyo
+8. he days of the week = hu_nev.nap
+9. the months of the year = hu_nev.honap
 ## Használat:
 
  Főként véletlengenerátorok kiegészítőjeként ajánlom
  
 I recommend it mainly as a supplement to random number generators. 
        
              random.choice
```

### Comparing `hu_nev-1.0.0/README.md` & `hu_nev-1.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# HU_NEV
+# hu_nev
 
 
 ## Leírás
 
 Magyar listák gyűjteménye - Collection of Hungarian lists.
 
 Az alábbi listákat találod :
@@ -10,27 +10,26 @@
 2. női keresztnevek  = hu_nev.keresztnev_n
 3. férfi keresztnevek = hu_nev.keresztnev_f
 4. utcanevek = hu_nev.utca
 5. telelpülésnevek= hu_nev.telepules
 6. vármegyék nevei = hu_nev.megye
 7. folyók nevei = hu_nev.folyo
 8. a hét napjai = hu_nev.nap
-9. az év hónapjai =hu_nev.honap
-10. 
-## Description
-1. last names
-2. female first names
-3. male first names
-4. street names
-5. city names
-6. names of counties
-7. names of rivers
-8. he days of the week
-9. the months of the year
+9. az év hónapjai = hu_nev.honap
 
+## Description
+1. last names =  hu_nev.vezeteknev
+2. female first names = hu_nev.keresztnev_n
+3. male first names  = hu_nev.keresztnev_f
+4. street names = hu_nev.utca
+5. city names = hu_nev.telepules
+6. names of counties = hu_nev.megye
+7. names of rivers = hu_nev.folyo
+8. he days of the week = hu_nev.nap
+9. the months of the year = hu_nev.honap
 ## Használat:
 
  Főként véletlengenerátorok kiegészítőjeként ajánlom
  
 I recommend it mainly as a supplement to random number generators. 
        
              random.choice
```

### Comparing `hu_nev-1.0.0/hu_nev.egg-info/PKG-INFO` & `hu_nev-1.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 Metadata-Version: 2.1
-Name: hu-nev
-Version: 1.0.0
-Summary: Magyar nevek lista
+Name: hu_nev
+Version: 1.1.0
+Summary: Magyar nevek listája
+Home-page: https://github.com/kobanya
 Author: Nagy Béla
 Author-email: nagy.bela.budapest@gmail.com
 License: MIT
-Classifier: Programming Language :: Python :: 3
+Keywords: magyar nevek
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
-# HU_NEV
+# hu_nev
 
 
 ## Leírás
 
 Magyar listák gyűjteménye - Collection of Hungarian lists.
 
 Az alábbi listákat találod :
@@ -22,27 +29,26 @@
 2. női keresztnevek  = hu_nev.keresztnev_n
 3. férfi keresztnevek = hu_nev.keresztnev_f
 4. utcanevek = hu_nev.utca
 5. telelpülésnevek= hu_nev.telepules
 6. vármegyék nevei = hu_nev.megye
 7. folyók nevei = hu_nev.folyo
 8. a hét napjai = hu_nev.nap
-9. az év hónapjai =hu_nev.honap
-10. 
-## Description
-1. last names
-2. female first names
-3. male first names
-4. street names
-5. city names
-6. names of counties
-7. names of rivers
-8. he days of the week
-9. the months of the year
+9. az év hónapjai = hu_nev.honap
 
+## Description
+1. last names =  hu_nev.vezeteknev
+2. female first names = hu_nev.keresztnev_n
+3. male first names  = hu_nev.keresztnev_f
+4. street names = hu_nev.utca
+5. city names = hu_nev.telepules
+6. names of counties = hu_nev.megye
+7. names of rivers = hu_nev.folyo
+8. he days of the week = hu_nev.nap
+9. the months of the year = hu_nev.honap
 ## Használat:
 
  Főként véletlengenerátorok kiegészítőjeként ajánlom
  
 I recommend it mainly as a supplement to random number generators. 
        
              random.choice
```

