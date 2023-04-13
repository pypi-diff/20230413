# Comparing `tmp/faker_marketdata-0.3.tar.gz` & `tmp/faker_marketdata-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faker_marketdata-0.3.tar", last modified: Tue Feb 14 10:40:09 2023, max compression
+gzip compressed data, was "faker_marketdata-0.4.tar", last modified: Thu Apr 13 04:52:02 2023, max compression
```

## Comparing `faker_marketdata-0.3.tar` & `faker_marketdata-0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 rubenafo   (505) staff       (20)        0 2023-02-14 10:40:09.528070 faker_marketdata-0.3/
--rw-r--r--   0 rubenafo   (505) staff       (20)    11357 2022-12-19 13:59:28.000000 faker_marketdata-0.3/LICENSE
--rw-r--r--   0 rubenafo   (505) staff       (20)     1428 2023-02-14 10:40:09.528269 faker_marketdata-0.3/PKG-INFO
--rw-r--r--   0 rubenafo   (505) staff       (20)      836 2022-12-27 10:46:15.000000 faker_marketdata-0.3/README.md
-drwxr-xr-x   0 rubenafo   (505) staff       (20)        0 2023-02-14 10:40:09.524389 faker_marketdata-0.3/faker_marketdata/
--rw-r--r--   0 rubenafo   (505) staff       (20)     4211 2022-12-27 10:45:07.000000 faker_marketdata-0.3/faker_marketdata/MarketDataProvider.py
--rw-r--r--   0 rubenafo   (505) staff       (20)       51 2022-12-22 09:41:13.000000 faker_marketdata-0.3/faker_marketdata/__init__.py
-drwxr-xr-x   0 rubenafo   (505) staff       (20)        0 2023-02-14 10:40:09.526772 faker_marketdata-0.3/faker_marketdata.egg-info/
--rw-r--r--   0 rubenafo   (505) staff       (20)     1428 2023-02-14 10:40:09.000000 faker_marketdata-0.3/faker_marketdata.egg-info/PKG-INFO
--rw-r--r--   0 rubenafo   (505) staff       (20)      346 2023-02-14 10:40:09.000000 faker_marketdata-0.3/faker_marketdata.egg-info/SOURCES.txt
--rw-r--r--   0 rubenafo   (505) staff       (20)        1 2023-02-14 10:40:09.000000 faker_marketdata-0.3/faker_marketdata.egg-info/dependency_links.txt
--rw-r--r--   0 rubenafo   (505) staff       (20)       31 2023-02-14 10:40:09.000000 faker_marketdata-0.3/faker_marketdata.egg-info/requires.txt
--rw-r--r--   0 rubenafo   (505) staff       (20)       23 2023-02-14 10:40:09.000000 faker_marketdata-0.3/faker_marketdata.egg-info/top_level.txt
--rw-r--r--   0 rubenafo   (505) staff       (20)       79 2023-02-14 10:40:09.528922 faker_marketdata-0.3/setup.cfg
--rw-r--r--   0 rubenafo   (505) staff       (20)      979 2023-02-14 10:39:21.000000 faker_marketdata-0.3/setup.py
-drwxr-xr-x   0 rubenafo   (505) staff       (20)        0 2023-02-14 10:40:09.527666 faker_marketdata-0.3/tests/
--rw-r--r--   0 rubenafo   (505) staff       (20)        0 2022-12-27 08:32:36.000000 faker_marketdata-0.3/tests/__init__.py
--rw-r--r--   0 rubenafo   (505) staff       (20)     2105 2022-12-27 10:45:07.000000 faker_marketdata-0.3/tests/test_marketdata.py
+drwxr-xr-x   0 rubenafo   (505) staff       (20)        0 2023-04-13 04:52:02.192811 faker_marketdata-0.4/
+-rw-r--r--   0 rubenafo   (505) staff       (20)    11357 2022-12-19 13:59:28.000000 faker_marketdata-0.4/LICENSE
+-rw-r--r--   0 rubenafo   (505) staff       (20)     1522 2023-04-13 04:52:02.193026 faker_marketdata-0.4/PKG-INFO
+-rw-r--r--   0 rubenafo   (505) staff       (20)      931 2023-04-13 04:46:19.000000 faker_marketdata-0.4/README.md
+drwxr-xr-x   0 rubenafo   (505) staff       (20)        0 2023-04-13 04:52:02.187433 faker_marketdata-0.4/faker_marketdata/
+-rw-r--r--   0 rubenafo   (505) staff       (20)     4305 2023-04-13 04:40:51.000000 faker_marketdata-0.4/faker_marketdata/MarketDataProvider.py
+-rw-r--r--   0 rubenafo   (505) staff       (20)       51 2022-12-22 09:41:13.000000 faker_marketdata-0.4/faker_marketdata/__init__.py
+drwxr-xr-x   0 rubenafo   (505) staff       (20)        0 2023-04-13 04:52:02.190586 faker_marketdata-0.4/faker_marketdata.egg-info/
+-rw-r--r--   0 rubenafo   (505) staff       (20)     1522 2023-04-13 04:52:02.000000 faker_marketdata-0.4/faker_marketdata.egg-info/PKG-INFO
+-rw-r--r--   0 rubenafo   (505) staff       (20)      346 2023-04-13 04:52:02.000000 faker_marketdata-0.4/faker_marketdata.egg-info/SOURCES.txt
+-rw-r--r--   0 rubenafo   (505) staff       (20)        1 2023-04-13 04:52:02.000000 faker_marketdata-0.4/faker_marketdata.egg-info/dependency_links.txt
+-rw-r--r--   0 rubenafo   (505) staff       (20)       31 2023-04-13 04:52:02.000000 faker_marketdata-0.4/faker_marketdata.egg-info/requires.txt
+-rw-r--r--   0 rubenafo   (505) staff       (20)       23 2023-04-13 04:52:02.000000 faker_marketdata-0.4/faker_marketdata.egg-info/top_level.txt
+-rw-r--r--   0 rubenafo   (505) staff       (20)       79 2023-04-13 04:52:02.193896 faker_marketdata-0.4/setup.cfg
+-rw-r--r--   0 rubenafo   (505) staff       (20)      979 2023-04-13 04:50:10.000000 faker_marketdata-0.4/setup.py
+drwxr-xr-x   0 rubenafo   (505) staff       (20)        0 2023-04-13 04:52:02.191953 faker_marketdata-0.4/tests/
+-rw-r--r--   0 rubenafo   (505) staff       (20)        0 2022-12-27 08:32:36.000000 faker_marketdata-0.4/tests/__init__.py
+-rw-r--r--   0 rubenafo   (505) staff       (20)     2490 2023-04-13 04:45:50.000000 faker_marketdata-0.4/tests/test_marketdata.py
```

### Comparing `faker_marketdata-0.3/LICENSE` & `faker_marketdata-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `faker_marketdata-0.3/PKG-INFO` & `faker_marketdata-0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 Metadata-Version: 2.1
 Name: faker_marketdata
-Version: 0.3
+Version: 0.4
 Summary: Sample market data for Faker
 Home-page: https://github.com/rubenafo/faker_marketdata
 Author: Ruben Afonso
 Author-email: rbfrancos@gmail.com
 Keywords: faker,testdata,financedata,python,marketdata,isin,sedol,cusip,ticker,figi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # faker_marketdata
-Generates random, valid market data for testing purposes.
+Generates random, valid market identifiers following most common formats in the industry.
 
 ## Installation
 
 ``` bash
 pip install faker_marketdata
 ```
 
 ## Usage
 
-Add as a provider to your Faker instance:
+Add as a provider to your [Faker](https://faker.readthedocs.io/en/master) instance:
 ``` python
 >>> from faker import Faker
 >>> from faker_marketdata import MarketDataProvider
 >>> fake = Faker()
->>> fake.add_provider(MarketDataProvider())
+>>> fake.add_provider(MarketDataProvider)
 ```
-Optionally you can use a seed value to have repeatable output: 
+Optionally you can define a seed value to have repeatable identifiers: 
 ``` python
->> fake.add_provider(MarketDataProvider(see=1220))
+>> Faker.seed(123)
+>> fake.add_provider(MarketDataProvider())
 ```
 
-Now you can start to generate market data, some examples:
+Now you can start to generate market identifiers, some examples:
 ``` python
 >> fake.isin()   # "GTYMQXUIYPB6"
 >> fake.sedol()  # "NKDEKC8"
 >> fake.cusip()  # "Z57XGDJW7"
 >> fake.ticker() # "GRTT"
 ```
 
 ## Documentation
-Supported market data identifiers:
+Supported market data formats:
 * ISIN
 * SEDOL
 * MIC
 * LEI
 * CUSIP
 * RIC
 * TICKER
```

### Comparing `faker_marketdata-0.3/faker_marketdata.egg-info/PKG-INFO` & `faker_marketdata-0.4/faker_marketdata.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 Metadata-Version: 2.1
 Name: faker-marketdata
-Version: 0.3
+Version: 0.4
 Summary: Sample market data for Faker
 Home-page: https://github.com/rubenafo/faker_marketdata
 Author: Ruben Afonso
 Author-email: rbfrancos@gmail.com
 Keywords: faker,testdata,financedata,python,marketdata,isin,sedol,cusip,ticker,figi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # faker_marketdata
-Generates random, valid market data for testing purposes.
+Generates random, valid market identifiers following most common formats in the industry.
 
 ## Installation
 
 ``` bash
 pip install faker_marketdata
 ```
 
 ## Usage
 
-Add as a provider to your Faker instance:
+Add as a provider to your [Faker](https://faker.readthedocs.io/en/master) instance:
 ``` python
 >>> from faker import Faker
 >>> from faker_marketdata import MarketDataProvider
 >>> fake = Faker()
->>> fake.add_provider(MarketDataProvider())
+>>> fake.add_provider(MarketDataProvider)
 ```
-Optionally you can use a seed value to have repeatable output: 
+Optionally you can define a seed value to have repeatable identifiers: 
 ``` python
->> fake.add_provider(MarketDataProvider(see=1220))
+>> Faker.seed(123)
+>> fake.add_provider(MarketDataProvider())
 ```
 
-Now you can start to generate market data, some examples:
+Now you can start to generate market identifiers, some examples:
 ``` python
 >> fake.isin()   # "GTYMQXUIYPB6"
 >> fake.sedol()  # "NKDEKC8"
 >> fake.cusip()  # "Z57XGDJW7"
 >> fake.ticker() # "GRTT"
 ```
 
 ## Documentation
-Supported market data identifiers:
+Supported market data formats:
 * ISIN
 * SEDOL
 * MIC
 * LEI
 * CUSIP
 * RIC
 * TICKER
```

### Comparing `faker_marketdata-0.3/setup.py` & `faker_marketdata-0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="faker_marketdata",
-    version="0.3",
+    version="0.4",
     author="Ruben Afonso",
     author_email="rbfrancos@gmail.com",
     description="Sample market data for Faker",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/rubenafo/faker_marketdata",
     keywords = ["faker", "testdata", "financedata", "python", "marketdata", "isin", "sedol", "cusip",
```

### Comparing `faker_marketdata-0.3/tests/test_marketdata.py` & `faker_marketdata-0.4/tests/test_marketdata.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+from faker import Faker
+
 from faker_marketdata import MarketDataProvider
 
 import unittest
 
 
 class MarketDataTests(unittest.TestCase):
 
     def setUp(self):
-        self.md = MarketDataProvider()
+        self.md = Faker()
+        self.md.add_provider(MarketDataProvider)
 
     def test_figi(self):
         figis = [self.md.figi() for _ in range(10000)]
         self.assertTrue(all(figi for figi in figis))
 
     def test_isin(self):
         isins = [self.md.isin() for _ in range(10000)]
@@ -44,27 +47,40 @@
         sedols = [self.md.sedol() for _ in range(10000)]
         self.assertTrue(all(sedol for sedol in sedols))
 
     def test_tickers(self):
         tickers = [self.md.ticker() for _ in range(10000)]
         self.assertTrue(all(ticker for ticker in tickers))
 
+
+class FakerIntegrationTests(unittest.TestCase):
     """
     Tests integration with Faker
     """
     def test_faker_provider(self):
-        from faker import Faker
         fake = Faker()
-        fake.add_provider(MarketDataProvider())
+        fake.add_provider(MarketDataProvider)
         self.assertTrue(fake.sedol())
 
-    def test_seed_fixes_random (self):
-        from faker import Faker
+    def test_seed_fixes_random(self):
         faker1 = Faker()
         faker2 = Faker()
-        faker1.add_provider(MarketDataProvider(seed=23))
-        faker2.add_provider(MarketDataProvider(seed=23))
-        self.assertEqual(faker1.sedol(), faker2.sedol())
+        faker1.add_provider(MarketDataProvider)
+        faker2.add_provider(MarketDataProvider)
+
+        Faker.seed(123)
+        sedol1 = faker1.sedol()
+        Faker.seed(123)
+        sedol2 = faker2.sedol()
+        self.assertEqual(sedol1, sedol2)
+
+    def test_existing_fake_methods_still_work(self):
+        fake = Faker()
+        fake.add_provider(MarketDataProvider)
+        sedol = fake.sedol()
+        self.assertTrue(sedol)
+        random_str = fake.lexify("???????")
+        self.assertTrue(random_str)
 
 
 if __name__ == '__main__':
     unittest.main()
```

