# Comparing `tmp/scrape-google-scholar-py-0.3.2.tar.gz` & `tmp/scrape-google-scholar-py-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrape-google-scholar-py-0.3.2.tar", last modified: Thu Apr 13 05:55:51 2023, max compression
+gzip compressed data, was "scrape-google-scholar-py-0.3.3.tar", last modified: Thu Apr 13 06:22:53 2023, max compression
```

## Comparing `scrape-google-scholar-py-0.3.2.tar` & `scrape-google-scholar-py-0.3.3.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 05:55:51.597377 scrape-google-scholar-py-0.3.2/
--rw-rw-rw-   0        0        0       42 2023-03-30 07:33:49.000000 scrape-google-scholar-py-0.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0    36317 2023-04-13 05:55:51.597377 scrape-google-scholar-py-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0    34997 2023-04-13 05:54:28.000000 scrape-google-scholar-py-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 05:55:51.576448 scrape-google-scholar-py-0.3.2/google_scholar_py/
--rw-rw-rw-   0        0        0      843 2023-04-13 05:54:28.000000 scrape-google-scholar-py-0.3.2/google_scholar_py/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 05:55:51.582427 scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/
--rw-rw-rw-   0        0        0     8769 2023-03-30 09:27:35.000000 scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/author_info_all_articles.py
--rw-rw-rw-   0        0        0     1492 2023-03-30 09:37:52.000000 scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/cite_results.py
--rw-rw-rw-   0        0        0     2468 2023-03-30 09:37:56.000000 scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/google_scholar_cited_by_public_access_author.py
--rw-rw-rw-   0        0        0     6777 2023-03-31 09:32:56.000000 scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/organic_search.py
--rw-rw-rw-   0        0        0     8293 2023-03-30 09:27:38.000000 scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/profiles_results.py
--rw-rw-rw-   0        0        0     5868 2023-03-31 10:06:39.000000 scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/top_mandates_metrics.py
--rw-rw-rw-   0        0        0     5650 2023-04-13 05:54:28.000000 scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/top_metrics_category_h5.py
--rw-rw-rw-   0        0        0     6708 2023-04-13 05:54:28.000000 scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/top_publications_article_citations.py
--rw-rw-rw-   0        0        0     6044 2023-04-13 05:54:28.000000 scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/top_publications_metrics.py
-drwxrwxrwx   0        0        0        0 2023-04-13 05:55:51.589404 scrape-google-scholar-py-0.3.2/google_scholar_py/serpapi_backend/
--rw-rw-rw-   0        0        0     5098 2023-03-30 09:37:03.000000 scrape-google-scholar-py-0.3.2/google_scholar_py/serpapi_backend/author_results.py
--rw-rw-rw-   0        0        0     3533 2023-03-30 08:25:43.000000 scrape-google-scholar-py-0.3.2/google_scholar_py/serpapi_backend/organic_cite_results.py
--rw-rw-rw-   0        0        0     3692 2023-03-30 09:37:07.000000 scrape-google-scholar-py-0.3.2/google_scholar_py/serpapi_backend/organic_results.py
--rw-rw-rw-   0        0        0     3248 2023-03-30 09:37:08.000000 scrape-google-scholar-py-0.3.2/google_scholar_py/serpapi_backend/profile_results.py
--rw-rw-rw-   0        0        0      127 2023-03-30 06:54:12.000000 scrape-google-scholar-py-0.3.2/pyproject.toml
--rw-rw-rw-   0        0        0     1606 2023-03-30 10:09:31.000000 scrape-google-scholar-py-0.3.2/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 05:55:51.595384 scrape-google-scholar-py-0.3.2/scrape_google_scholar_py.egg-info/
--rw-rw-rw-   0        0        0    36317 2023-04-13 05:55:51.000000 scrape-google-scholar-py-0.3.2/scrape_google_scholar_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1091 2023-04-13 05:55:51.000000 scrape-google-scholar-py-0.3.2/scrape_google_scholar_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 05:55:51.000000 scrape-google-scholar-py-0.3.2/scrape_google_scholar_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2023-04-13 05:55:51.000000 scrape-google-scholar-py-0.3.2/scrape_google_scholar_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-13 05:55:51.000000 scrape-google-scholar-py-0.3.2/scrape_google_scholar_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 05:55:51.597377 scrape-google-scholar-py-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     2109 2023-04-13 05:54:28.000000 scrape-google-scholar-py-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:22:53.988462 scrape-google-scholar-py-0.3.3/
+-rw-rw-rw-   0        0        0       42 2023-03-30 07:33:49.000000 scrape-google-scholar-py-0.3.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    36317 2023-04-13 06:22:53.988462 scrape-google-scholar-py-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0    34997 2023-04-13 05:54:28.000000 scrape-google-scholar-py-0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 06:22:53.958562 scrape-google-scholar-py-0.3.3/google_scholar_py/
+-rw-rw-rw-   0        0        0      825 2023-04-13 06:09:47.000000 scrape-google-scholar-py-0.3.3/google_scholar_py/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:22:53.980488 scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/
+-rw-rw-rw-   0        0        0     8787 2023-04-13 06:10:14.000000 scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/author_info_all_articles.py
+-rw-rw-rw-   0        0        0     1492 2023-03-30 09:37:52.000000 scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/cite_results.py
+-rw-rw-rw-   0        0        0     2468 2023-03-30 09:37:56.000000 scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/google_scholar_cited_by_public_access_author.py
+-rw-rw-rw-   0        0        0     6795 2023-04-13 06:10:48.000000 scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/organic_search.py
+-rw-rw-rw-   0        0        0     8311 2023-04-13 06:11:27.000000 scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/profiles_results.py
+-rw-rw-rw-   0        0        0     5860 2023-04-13 06:17:03.000000 scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/top_mandates_metrics.py
+-rw-rw-rw-   0        0        0     6930 2023-04-13 06:18:17.000000 scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/top_publications_article_citations.py
+-rw-rw-rw-   0        0        0     6062 2023-04-13 06:21:42.000000 scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/top_publications_metrics.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:22:53.984478 scrape-google-scholar-py-0.3.3/google_scholar_py/serpapi_backend/
+-rw-rw-rw-   0        0        0     5098 2023-03-30 09:37:03.000000 scrape-google-scholar-py-0.3.3/google_scholar_py/serpapi_backend/author_results.py
+-rw-rw-rw-   0        0        0     3533 2023-03-30 08:25:43.000000 scrape-google-scholar-py-0.3.3/google_scholar_py/serpapi_backend/organic_cite_results.py
+-rw-rw-rw-   0        0        0     3692 2023-03-30 09:37:07.000000 scrape-google-scholar-py-0.3.3/google_scholar_py/serpapi_backend/organic_results.py
+-rw-rw-rw-   0        0        0     3248 2023-03-30 09:37:08.000000 scrape-google-scholar-py-0.3.3/google_scholar_py/serpapi_backend/profile_results.py
+-rw-rw-rw-   0        0        0      127 2023-03-30 06:54:12.000000 scrape-google-scholar-py-0.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1606 2023-03-30 10:09:31.000000 scrape-google-scholar-py-0.3.3/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 06:22:53.987464 scrape-google-scholar-py-0.3.3/scrape_google_scholar_py.egg-info/
+-rw-rw-rw-   0        0        0    36317 2023-04-13 06:22:53.000000 scrape-google-scholar-py-0.3.3/scrape_google_scholar_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1031 2023-04-13 06:22:53.000000 scrape-google-scholar-py-0.3.3/scrape_google_scholar_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 06:22:53.000000 scrape-google-scholar-py-0.3.3/scrape_google_scholar_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      125 2023-04-13 06:22:53.000000 scrape-google-scholar-py-0.3.3/scrape_google_scholar_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-13 06:22:53.000000 scrape-google-scholar-py-0.3.3/scrape_google_scholar_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 06:22:53.988462 scrape-google-scholar-py-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     2109 2023-04-13 06:18:08.000000 scrape-google-scholar-py-0.3.3/setup.py
```

### Comparing `scrape-google-scholar-py-0.3.2/PKG-INFO` & `scrape-google-scholar-py-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrape-google-scholar-py
-Version: 0.3.2
+Version: 0.3.3
 Summary: Extract data from all Google Scholar pages in Python. Sponsored by SerpApi.
 Home-page: https://github.com/dimitryzub/scrape-google-scholar
 Author: Dmitiry Zub
 Author-email: dimitryzub@gmail.com
 Maintainer: Dmitiry Zub
 Maintainer-email: dimitryzub@gmail.com
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scrape-google-scholar-py Version: 0.3.2 Summary:
+Metadata-Version: 2.1 Name: scrape-google-scholar-py Version: 0.3.3 Summary:
 Extract data from all Google Scholar pages in Python. Sponsored by SerpApi.
 Home-page: https://github.com/dimitryzub/scrape-google-scholar Author: Dmitiry
 Zub Author-email: dimitryzub@gmail.com Maintainer: Dmitiry Zub Maintainer-
 email: dimitryzub@gmail.com License: MIT Project-URL: Documentation, https://
 github.com/dimitryzub/scrape-google-scholar#example-usage-custom-backend
 Project-URL: Source, https://github.com/dimitryzub/scrape-google-scholar
 Project-URL: Tracker, https://github.com/dimitryzub/scrape-google-scholar/
```

### Comparing `scrape-google-scholar-py-0.3.2/README.md` & `scrape-google-scholar-py-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `scrape-google-scholar-py-0.3.2/google_scholar_py/__init__.py` & `scrape-google-scholar-py-0.3.3/google_scholar_py/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# custom backend
 from .custom_backend.organic_search import CustomGoogleScholarOrganic
 from .custom_backend.profiles_results import CustomGoogleScholarProfiles
 from .custom_backend.author_info_all_articles import CustomGoogleScholarAuthor
 from .custom_backend.top_mandates_metrics import CustomGoogleScholarTopMandates
 from .custom_backend.top_publications_metrics import CustomGoogleScholarTopPublications
 from .custom_backend.top_publications_article_citations import CustomGoogleScholarTopPublicationCitations
```

### Comparing `scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/author_info_all_articles.py` & `scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/author_info_all_articles.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
         # selenium stealth
         options = webdriver.ChromeOptions()
         options.add_argument('--headless')
         options.add_argument('--no-sandbox')
         options.add_argument('--disable-dev-shm-usage')
         
-        options.add_experimental_option('excludeSwitches', ['enable-automation'])
+        options.add_experimental_option('excludeSwitches', ['enable-automation', 'enable-logging'])
         options.add_experimental_option('useAutomationExtension', False)
         
         service = Service(ChromeDriverManager().install())
         driver = webdriver.Chrome(service=service, options=options)
         
         stealth(driver,
             languages=['en-US', 'en'],
```

### Comparing `scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/cite_results.py` & `scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/cite_results.py`

 * *Files identical despite different names*

### Comparing `scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/google_scholar_cited_by_public_access_author.py` & `scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/google_scholar_cited_by_public_access_author.py`

 * *Files identical despite different names*

### Comparing `scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/organic_search.py` & `scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/organic_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         
         # selenium stealth
         options = webdriver.ChromeOptions()
         options.add_argument('--headless')
         options.add_argument('--no-sandbox')
         options.add_argument('--disable-dev-shm-usage')
         
-        options.add_experimental_option('excludeSwitches', ['enable-automation'])
+        options.add_experimental_option('excludeSwitches', ['enable-automation', 'enable-logging'])
         options.add_experimental_option('useAutomationExtension', False) 
         
         service = Service(ChromeDriverManager().install())
         driver = webdriver.Chrome(service=service, options=options)
         
         stealth(driver,
             languages=['en-US', 'en'],
```

### Comparing `scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/profiles_results.py` & `scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/profiles_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         
         # selenium stealth
         options = webdriver.ChromeOptions()
         options.add_argument('--headless')
         options.add_argument('--no-sandbox')
         options.add_argument('--disable-dev-shm-usage')
         
-        options.add_experimental_option('excludeSwitches', ['enable-automation'])
+        options.add_experimental_option('excludeSwitches', ['enable-automation', 'enable-logging'])
         options.add_experimental_option('useAutomationExtension', False)
         
         service = Service(ChromeDriverManager().install())
         driver = webdriver.Chrome(service=service, options=options)
         
         stealth(driver,
             languages=['en-US', 'en'],
```

### Comparing `scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/top_mandates_metrics.py` & `scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/top_mandates_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from selenium_stealth import stealth
 from selenium.webdriver.chrome.service import Service
 from webdriver_manager.chrome import ChromeDriverManager
 from selectolax.lexbor import LexborHTMLParser
 from typing import List, Dict, Callable
 import pandas as pd
 import re
-from pathlib import Path
 
 
 class CustomGoogleScholarTopMandates:
     def __init__(self) -> None:
         pass
     
 
@@ -115,15 +114,15 @@
         
         # selenium stealth
         options = webdriver.ChromeOptions()
         options.add_argument('--headless')
         options.add_argument('--no-sandbox')
         options.add_argument('--disable-dev-shm-usage')
         
-        options.add_experimental_option('excludeSwitches', ['enable-automation'])
+        options.add_experimental_option('excludeSwitches', ['enable-automation', 'enable-logging'])
         options.add_experimental_option('useAutomationExtension', False)
         
         service = Service(ChromeDriverManager().install())
         driver = webdriver.Chrome(service=service, options=options)
             
         stealth(driver,
             languages=['en-US', 'en'],
```

### Comparing `scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/top_metrics_category_h5.py` & `scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/top_publications_metrics.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,139 +1,141 @@
 from selenium import webdriver
 from selenium_stealth import stealth
 from selenium.webdriver.chrome.service import Service
 from webdriver_manager.chrome import ChromeDriverManager
 from selectolax.lexbor import LexborHTMLParser
-from typing import List, Dict, Callable
+from typing import List, Dict, Callable, Union
 import pandas as pd
-import re
 
-
-class CustomCategoryArticles:
+class CustomGoogleScholarTopPublications:
     def __init__(self) -> None:
         pass
 
-    
-    def parse(self, parser: Callable, category_articles: Callable):
+
+    def parse(self, parser: Callable, top_publications_data: Callable):
         '''
         Arugments:
-        - parser: Callable. Lexbor parser from google_scholar_top_mandates_metrics() function.
-        - top_mandates_data: Callable. List to append data to. List origin location is google_scholar_top_mandates_metrics() function. Line 100.
+        - parser: Callable. Lexbor parser from google_scholar_top_publication_metrics() function.
+        - top_publications_data: Callable. List to append data to. List origin location is google_scholar_top_publication_metrics() function. Line 100.
         
         This function parses data from Google Scholar Organic results and appends data to a List.
         
-        It's used by google_scholar_top_mandates_metrics().
+        It's used by google_scholar_top_publication_metrics().
         
-        It returns nothing as it appends data to `top_mandates_data`, 
-        which appends it to `top_mandates_data` List in the google_scholar_top_mandates_metrics() function.
+        It returns nothing as it appends data to `top_publications_data`, 
+        which appends it to `top_publications_data` List in the google_scholar_top_publication_metrics() function.
         '''
-        
-        for table in parser.css('tr'):
-            title = table.css_first('.gsc_mp_anchor_lrge').text()
-            title_link = table.css_first('a.gsc_mp_anchor_lrge').attrs['href']
-            
-            authors = table.css_first('.gsc_mpat_ttl+ .gs_gray').text()
-            citation = table.css_first('.gs_gray+ .gs_gray').text()
-            
-            citation_journal = re.search(r'', citation).group()
-            citation_volume = re.search(r'', citation).group()
-            citation_issue_number = re.search(r'', citation).group()
-            citation_pages = re.search(r'', citation).group()
-            
-            
-            cited_by = table.css_first('.gsc_mpat_c .gsc_mp_anchor').text()
-            cited_by_link = table.css_first('.gsc_mpat_c .gsc_mp_anchor').attrs['href']
-            year = table.css_first('.gsc_mp_anchor.gs_nph').text()
 
-            
-            category_articles.append({
+        # selectors skips table header row
+        for table in parser.css('tr:not(:first-child)'):
+            try:
+                title: str = table.css_first('td.gsc_mvt_t').text()
+            except: title = None
+            
+            try: 
+                h5_index: int = table.css_first('a.gs_ibl').text()
+            except: h5_index = None
+            
+            try: 
+                h5_index_link: str = f"https://scholar.google.com{table.css_first('a.gs_ibl').attrs['href']}"
+            except: h5_index_link = None
+            
+            try: 
+                h5_median: int = table.css_first('span.gs_ibl').text()
+            except: h5_median = None
+        
+            top_publications_data.append({
                 'title': title,
-                'title_link': title_link,
-                'authors': authors,
-                'citation': {
-                  'citation_journal': citation_journal,  
-                  'citation_volume': citation_volume,  
-                  'citation_issue_number': citation_issue_number,  
-                  'citation_pages': citation_pages,
-                },
-                'cited_by': cited_by,
-                'cited_by_link': cited_by_link,
-                'year': year,
+                'h5_index': int(h5_index) if h5_index else h5_index,
+                'h5_index_link': h5_index_link,
+                'h5_median': int(h5_median) if h5_median else h5_median
             })
-            
-    def scrape_category_articles(
+
+
+    def scrape_top_publication_metrics(
             self,
+            category: str = '', 
+            lang: str = 'en',
             save_to_csv: bool = False, 
             save_to_json: bool = False,
-            lang: str = 'en'
-        ) -> List[Dict[str, str]]:
-        #TODO add argument to support other languages https://serpapi.com/google-languages
+        ) -> List[Dict[str, Union[str, int]]]:
+        #TODO add subcategories to subcategory arg
+        #TODO: support other languages: lang='spanish' -> 'sp'. https://serpapi.com/google-languages
+
 
         '''
-        Results comes from: https://scholar.google.com/citations?view_op=mandates_leaderboard
+        Results comes from: https://scholar.google.com/citations?view_op=top_venues
         
         Returns:
-        - funder: str
-        - link: str
-        - 2019: str
-        - 2020: str
-        - 2021: str
-        - overall: str (not extracted at the moment, selector needs to be fixed)
+        - title: str
+        - h5_index: int
+        - h5_index_link: str
+        - h5_median: int
         
         Arguments: 
-        - save_to_csv: True of False. Saves data to CSV file. Default is False. 
-        - save_to_json: True of False. Saves data to JSON file. Default is False.
+        - save_to_csv: True of False. Default is False. Saves data to CSV file.
+        - save_to_json: True of False. Default is False. Saves data to JSON file.
         - lang: str. Language. Defaults to English ('en'). For now, need to be checked yourself. Other languages: https://serpapi.com/google-languages
-        
+        - category: str. Available categories showed in the function documentation below.
+            Available categories:
+            - "bus": Business, Economics & Management
+            - "chm": Chemical & Material Sciences
+            - "eng": Engineering & Computer Science
+            - "med": Health & Medical Sciences
+            - "hum": Humanities, Literature & Arts
+            - "bio": Life Sciences & Earth Sciences
+            - "phy": Physics & Mathematics
+            - "soc": Social Sciences
+            
         Usage:
         
-        from google_scholar_py import CustomGoogleScholarTopMandates
+        from google_scholar_py import CustomGoogleScholarTopPublications
+        
+        data = CustomGoogleScholarTopPublications().scrape_top_publication_metrics(category='eng', lang='en') # sv = swedish
         
-        parser = CustomGoogleScholarTopMandates()
-        data = parser.scrape_top_mandates_metrics(
-            save_to_csv=True,
-            save_to_json=False
-        )
-        print(json.dumps(data, indent=2))
-
         for result in data:
-            print(result['funder'])
+            print(result['title'])
             ...
         '''
         
         # selenium stealth
         options = webdriver.ChromeOptions()
         options.add_argument('--headless')
         options.add_argument('--no-sandbox')
         options.add_argument('--disable-dev-shm-usage')
         
-        options.add_experimental_option('excludeSwitches', ['enable-automation'])
+        options.add_experimental_option('excludeSwitches', ['enable-automation', 'enable-logging'])
         options.add_experimental_option('useAutomationExtension', False)
         
         service = Service(ChromeDriverManager().install())
         driver = webdriver.Chrome(service=service, options=options)
             
         stealth(driver,
             languages=['en-US', 'en'],
             vendor='Google Inc.',
             platform='Win32',
             webgl_vendor='Intel Inc.',
             renderer='Intel Iris OpenGL Engine',
             fix_hairline=True
         )
         
-        category_articles = []
+        top_publications_data = []
 
-        driver.get(f'https://scholar.google.com/citations?view_op=mandates_leaderboard&hl={lang}')
-        parser = LexborHTMLParser(driver.page_source)
-        self.parse(parser=parser, category_articles=category_articles)
-        
-        if save_to_csv:
-            pd.DataFrame(data=category_articles).to_csv('google_scholar_top_mandates_category_articles_data.csv', 
-                                                        index=False, encoding='utf-8')
+        if category:
+            driver.get(f'https://scholar.google.com/citations?view_op=top_venues&hl={lang}&vq={category}')
+            parser = LexborHTMLParser(driver.page_source)
+            self.parse(parser=parser, top_publications_data=top_publications_data)
+        else: 
+            # no vq={category} URL parameter
+            driver.get(f'https://scholar.google.com/citations?view_op=top_venues&hl={lang}&vq={category}') # vq='' which will redirect to the page with no applied category
+            parser = LexborHTMLParser(driver.page_source)
+            self.parse(parser=parser, top_publications_data=top_publications_data)
             
+        if save_to_csv:
+            pd.DataFrame(data=top_publications_data).to_csv('google_scholar_top_publications_data.csv', 
+                                                            index=False, encoding='utf-8')
         if save_to_json:
-            pd.DataFrame(data=category_articles).to_json('google_scholar_top_mandates_category_articles_data.json', 
-                                                        orient='records')
+            pd.DataFrame(data=top_publications_data).to_json('google_scholar_top_publications_data.json', 
+                                                            orient='records')
             
         driver.quit()
-        return category_articles
+        return top_publications_data
```

### Comparing `scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/top_publications_article_citations.py` & `scrape-google-scholar-py-0.3.3/google_scholar_py/custom_backend/top_publications_article_citations.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,51 +69,53 @@
             self,
             journal_publications_link: str,
             pagination: bool = False,
             save_to_csv: bool = False, 
             save_to_json: bool = False
         ) -> List[Dict[str, Union[str, List[str], int]]]:
         '''
+        Results comes from (for example): https://scholar.google.com/citations?hl=en&venue=H--JoiVp8x8J.2022&vq=en&view_op=hcore_citedby&hcore_pos=0
+        
         Extracts data from Google Scholar Top Publication Metrics Citation page:
         - title: str
         - title_link: str
         - authors: list 
         - cited_by_count: int
         - cited_by_link: str 
         - year: int
         - published_at: str
     
         Arguments:
-        - link: str. Search query. 
+        - journal_publications_link: str. Search query. 
         - pagination: bool. Enables or disables pagination. Default is False.
         - save_to_csv: bool. True of False. Default is False.
         - save_to_json: bool. True of False. Default is False.
         
         Usage:
         
         from google_scholar_py import CustomGoogleScholarTopPublicationCitations
 
         parser = CustomGoogleScholarTopPublicationCitations()
         data = parser.scrape_google_scholar_top_publication_citations(
-            link='https://scholar.google.com/citations?hl=en&venue=H--JoiVp8x8J.2022&vq=en&view_op=hcore_citedby&hcore_pos=0', # or link variable that stores the link
+            journal_publications_link='https://scholar.google.com/citations?hl=en&venue=H--JoiVp8x8J.2022&vq=en&view_op=hcore_citedby&hcore_pos=0', # or link variable that stores the link
             pagination=False,
             save_to_csv=True
         )
         
         for citations in data:
             print(citations['title'], citations['year'], citations['published_at'], sep='\\n')
         '''
         
         # selenium stealth
         options = webdriver.ChromeOptions()
         options.add_argument('--headless')
         options.add_argument('--no-sandbox')
         options.add_argument('--disable-dev-shm-usage')
         
-        options.add_experimental_option('excludeSwitches', ['enable-automation'])
+        options.add_experimental_option('excludeSwitches', ['enable-automation', 'enable-logging'])
         options.add_experimental_option('useAutomationExtension', False) 
         
         service = Service(ChromeDriverManager().install())
         driver = webdriver.Chrome(service=service, options=options)
         
         stealth(driver,
             languages=['en-US', 'en'],
@@ -152,8 +154,8 @@
             pd.DataFrame(data=publication_citation_data).to_csv('google_scholar_top_publication_citations.csv', 
                                                             index=False, encoding='utf-8')
         if save_to_json:
             pd.DataFrame(data=publication_citation_data).to_json('google_scholar_top_publication_citations.json', 
                                                             orient='records')
         driver.quit()
         
-        return publication_citation_data
+        return publication_citation_data
```

### Comparing `scrape-google-scholar-py-0.3.2/google_scholar_py/serpapi_backend/author_results.py` & `scrape-google-scholar-py-0.3.3/google_scholar_py/serpapi_backend/author_results.py`

 * *Files identical despite different names*

### Comparing `scrape-google-scholar-py-0.3.2/google_scholar_py/serpapi_backend/organic_cite_results.py` & `scrape-google-scholar-py-0.3.3/google_scholar_py/serpapi_backend/organic_cite_results.py`

 * *Files identical despite different names*

### Comparing `scrape-google-scholar-py-0.3.2/google_scholar_py/serpapi_backend/organic_results.py` & `scrape-google-scholar-py-0.3.3/google_scholar_py/serpapi_backend/organic_results.py`

 * *Files identical despite different names*

### Comparing `scrape-google-scholar-py-0.3.2/google_scholar_py/serpapi_backend/profile_results.py` & `scrape-google-scholar-py-0.3.3/google_scholar_py/serpapi_backend/profile_results.py`

 * *Files identical despite different names*

### Comparing `scrape-google-scholar-py-0.3.2/requirements.txt` & `scrape-google-scholar-py-0.3.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `scrape-google-scholar-py-0.3.2/scrape_google_scholar_py.egg-info/PKG-INFO` & `scrape-google-scholar-py-0.3.3/scrape_google_scholar_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrape-google-scholar-py
-Version: 0.3.2
+Version: 0.3.3
 Summary: Extract data from all Google Scholar pages in Python. Sponsored by SerpApi.
 Home-page: https://github.com/dimitryzub/scrape-google-scholar
 Author: Dmitiry Zub
 Author-email: dimitryzub@gmail.com
 Maintainer: Dmitiry Zub
 Maintainer-email: dimitryzub@gmail.com
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scrape-google-scholar-py Version: 0.3.2 Summary:
+Metadata-Version: 2.1 Name: scrape-google-scholar-py Version: 0.3.3 Summary:
 Extract data from all Google Scholar pages in Python. Sponsored by SerpApi.
 Home-page: https://github.com/dimitryzub/scrape-google-scholar Author: Dmitiry
 Zub Author-email: dimitryzub@gmail.com Maintainer: Dmitiry Zub Maintainer-
 email: dimitryzub@gmail.com License: MIT Project-URL: Documentation, https://
 github.com/dimitryzub/scrape-google-scholar#example-usage-custom-backend
 Project-URL: Source, https://github.com/dimitryzub/scrape-google-scholar
 Project-URL: Tracker, https://github.com/dimitryzub/scrape-google-scholar/
```

### Comparing `scrape-google-scholar-py-0.3.2/scrape_google_scholar_py.egg-info/SOURCES.txt` & `scrape-google-scholar-py-0.3.3/scrape_google_scholar_py.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 google_scholar_py/__init__.py
 google_scholar_py/custom_backend/author_info_all_articles.py
 google_scholar_py/custom_backend/cite_results.py
 google_scholar_py/custom_backend/google_scholar_cited_by_public_access_author.py
 google_scholar_py/custom_backend/organic_search.py
 google_scholar_py/custom_backend/profiles_results.py
 google_scholar_py/custom_backend/top_mandates_metrics.py
-google_scholar_py/custom_backend/top_metrics_category_h5.py
 google_scholar_py/custom_backend/top_publications_article_citations.py
 google_scholar_py/custom_backend/top_publications_metrics.py
 google_scholar_py/serpapi_backend/author_results.py
 google_scholar_py/serpapi_backend/organic_cite_results.py
 google_scholar_py/serpapi_backend/organic_results.py
 google_scholar_py/serpapi_backend/profile_results.py
 scrape_google_scholar_py.egg-info/PKG-INFO
```

### Comparing `scrape-google-scholar-py-0.3.2/setup.py` & `scrape-google-scholar-py-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open('README.md', 'r', encoding='utf-8') as readme_file:
     README = readme_file.read()
 
 setup(
     name='scrape-google-scholar-py',
     description = 'Extract data from all Google Scholar pages in Python. Sponsored by SerpApi.',
     url='https://github.com/dimitryzub/scrape-google-scholar',
-    version='0.3.2',
+    version='0.3.3',
     license='MIT',
     author='Dmitiry Zub',
     author_email='dimitryzub@gmail.com',
     maintainer='Dmitiry Zub',
     maintainer_email='dimitryzub@gmail.com',
     long_description_content_type='text/markdown',
     long_description=README,
```

