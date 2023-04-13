# Comparing `tmp/scrape-google-scholar-py-0.3.1.tar.gz` & `tmp/scrape-google-scholar-py-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrape-google-scholar-py-0.3.1.tar", last modified: Thu Mar 30 10:19:37 2023, max compression
+gzip compressed data, was "scrape-google-scholar-py-0.3.2.tar", last modified: Thu Apr 13 05:55:51 2023, max compression
```

## Comparing `scrape-google-scholar-py-0.3.1.tar` & `scrape-google-scholar-py-0.3.2.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 10:19:37.077602 scrape-google-scholar-py-0.3.1/
--rw-rw-rw-   0        0        0       42 2023-03-30 07:33:49.000000 scrape-google-scholar-py-0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0    36972 2023-03-30 10:19:37.077602 scrape-google-scholar-py-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0    35650 2023-03-30 09:56:27.000000 scrape-google-scholar-py-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-30 10:19:37.064600 scrape-google-scholar-py-0.3.1/google_scholar_py/
--rw-rw-rw-   0        0        0      736 2023-03-30 08:27:07.000000 scrape-google-scholar-py-0.3.1/google_scholar_py/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 10:19:37.070544 scrape-google-scholar-py-0.3.1/google_scholar_py/custom_backend/
--rw-rw-rw-   0        0        0     8769 2023-03-30 09:27:35.000000 scrape-google-scholar-py-0.3.1/google_scholar_py/custom_backend/author_info_all_articles.py
--rw-rw-rw-   0        0        0     1492 2023-03-30 09:37:52.000000 scrape-google-scholar-py-0.3.1/google_scholar_py/custom_backend/cite_results.py
--rw-rw-rw-   0        0        0     2468 2023-03-30 09:37:56.000000 scrape-google-scholar-py-0.3.1/google_scholar_py/custom_backend/google_scholar_cited_by_public_access_author.py
--rw-rw-rw-   0        0        0     6777 2023-03-30 09:27:36.000000 scrape-google-scholar-py-0.3.1/google_scholar_py/custom_backend/organic_search.py
--rw-rw-rw-   0        0        0     8293 2023-03-30 09:27:38.000000 scrape-google-scholar-py-0.3.1/google_scholar_py/custom_backend/profiles_results.py
--rw-rw-rw-   0        0        0     5868 2023-03-30 09:27:39.000000 scrape-google-scholar-py-0.3.1/google_scholar_py/custom_backend/top_mandates_metrics.py
--rw-rw-rw-   0        0        0     5898 2023-03-30 09:27:39.000000 scrape-google-scholar-py-0.3.1/google_scholar_py/custom_backend/top_publications_metrics.py
-drwxrwxrwx   0        0        0        0 2023-03-30 10:19:37.072617 scrape-google-scholar-py-0.3.1/google_scholar_py/serpapi_backend/
--rw-rw-rw-   0        0        0     5098 2023-03-30 09:37:03.000000 scrape-google-scholar-py-0.3.1/google_scholar_py/serpapi_backend/author_results.py
--rw-rw-rw-   0        0        0     3533 2023-03-30 08:25:43.000000 scrape-google-scholar-py-0.3.1/google_scholar_py/serpapi_backend/organic_cite_results.py
--rw-rw-rw-   0        0        0     3692 2023-03-30 09:37:07.000000 scrape-google-scholar-py-0.3.1/google_scholar_py/serpapi_backend/organic_results.py
--rw-rw-rw-   0        0        0     3248 2023-03-30 09:37:08.000000 scrape-google-scholar-py-0.3.1/google_scholar_py/serpapi_backend/profile_results.py
--rw-rw-rw-   0        0        0      127 2023-03-30 06:54:12.000000 scrape-google-scholar-py-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0     1606 2023-03-30 10:09:31.000000 scrape-google-scholar-py-0.3.1/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-03-30 10:19:37.076590 scrape-google-scholar-py-0.3.1/scrape_google_scholar_py.egg-info/
--rw-rw-rw-   0        0        0    36972 2023-03-30 10:19:36.000000 scrape-google-scholar-py-0.3.1/scrape_google_scholar_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      960 2023-03-30 10:19:37.000000 scrape-google-scholar-py-0.3.1/scrape_google_scholar_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 10:19:36.000000 scrape-google-scholar-py-0.3.1/scrape_google_scholar_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2023-03-30 10:19:37.000000 scrape-google-scholar-py-0.3.1/scrape_google_scholar_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-03-30 10:19:37.000000 scrape-google-scholar-py-0.3.1/scrape_google_scholar_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-30 10:19:37.077602 scrape-google-scholar-py-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     2109 2023-03-30 10:18:01.000000 scrape-google-scholar-py-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 05:55:51.597377 scrape-google-scholar-py-0.3.2/
+-rw-rw-rw-   0        0        0       42 2023-03-30 07:33:49.000000 scrape-google-scholar-py-0.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    36317 2023-04-13 05:55:51.597377 scrape-google-scholar-py-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0    34997 2023-04-13 05:54:28.000000 scrape-google-scholar-py-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 05:55:51.576448 scrape-google-scholar-py-0.3.2/google_scholar_py/
+-rw-rw-rw-   0        0        0      843 2023-04-13 05:54:28.000000 scrape-google-scholar-py-0.3.2/google_scholar_py/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 05:55:51.582427 scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/
+-rw-rw-rw-   0        0        0     8769 2023-03-30 09:27:35.000000 scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/author_info_all_articles.py
+-rw-rw-rw-   0        0        0     1492 2023-03-30 09:37:52.000000 scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/cite_results.py
+-rw-rw-rw-   0        0        0     2468 2023-03-30 09:37:56.000000 scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/google_scholar_cited_by_public_access_author.py
+-rw-rw-rw-   0        0        0     6777 2023-03-31 09:32:56.000000 scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/organic_search.py
+-rw-rw-rw-   0        0        0     8293 2023-03-30 09:27:38.000000 scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/profiles_results.py
+-rw-rw-rw-   0        0        0     5868 2023-03-31 10:06:39.000000 scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/top_mandates_metrics.py
+-rw-rw-rw-   0        0        0     5650 2023-04-13 05:54:28.000000 scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/top_metrics_category_h5.py
+-rw-rw-rw-   0        0        0     6708 2023-04-13 05:54:28.000000 scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/top_publications_article_citations.py
+-rw-rw-rw-   0        0        0     6044 2023-04-13 05:54:28.000000 scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/top_publications_metrics.py
+drwxrwxrwx   0        0        0        0 2023-04-13 05:55:51.589404 scrape-google-scholar-py-0.3.2/google_scholar_py/serpapi_backend/
+-rw-rw-rw-   0        0        0     5098 2023-03-30 09:37:03.000000 scrape-google-scholar-py-0.3.2/google_scholar_py/serpapi_backend/author_results.py
+-rw-rw-rw-   0        0        0     3533 2023-03-30 08:25:43.000000 scrape-google-scholar-py-0.3.2/google_scholar_py/serpapi_backend/organic_cite_results.py
+-rw-rw-rw-   0        0        0     3692 2023-03-30 09:37:07.000000 scrape-google-scholar-py-0.3.2/google_scholar_py/serpapi_backend/organic_results.py
+-rw-rw-rw-   0        0        0     3248 2023-03-30 09:37:08.000000 scrape-google-scholar-py-0.3.2/google_scholar_py/serpapi_backend/profile_results.py
+-rw-rw-rw-   0        0        0      127 2023-03-30 06:54:12.000000 scrape-google-scholar-py-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1606 2023-03-30 10:09:31.000000 scrape-google-scholar-py-0.3.2/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 05:55:51.595384 scrape-google-scholar-py-0.3.2/scrape_google_scholar_py.egg-info/
+-rw-rw-rw-   0        0        0    36317 2023-04-13 05:55:51.000000 scrape-google-scholar-py-0.3.2/scrape_google_scholar_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1091 2023-04-13 05:55:51.000000 scrape-google-scholar-py-0.3.2/scrape_google_scholar_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 05:55:51.000000 scrape-google-scholar-py-0.3.2/scrape_google_scholar_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      125 2023-04-13 05:55:51.000000 scrape-google-scholar-py-0.3.2/scrape_google_scholar_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-13 05:55:51.000000 scrape-google-scholar-py-0.3.2/scrape_google_scholar_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 05:55:51.597377 scrape-google-scholar-py-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     2109 2023-04-13 05:54:28.000000 scrape-google-scholar-py-0.3.2/setup.py
```

### Comparing `scrape-google-scholar-py-0.3.1/PKG-INFO` & `scrape-google-scholar-py-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrape-google-scholar-py
-Version: 0.3.1
+Version: 0.3.2
 Summary: Extract data from all Google Scholar pages in Python. Sponsored by SerpApi.
 Home-page: https://github.com/dimitryzub/scrape-google-scholar
 Author: Dmitiry Zub
 Author-email: dimitryzub@gmail.com
 Maintainer: Dmitiry Zub
 Maintainer-email: dimitryzub@gmail.com
 License: MIT
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 <div align="center">
 <p>Sponsor of the project:</p>
 <div>
-   <img src="https://sindresorhus.com/assets/thanks/serpapi-logo-light.svg" width="140" alt="SerpApi">
+   <img src="https://user-images.githubusercontent.com/78694043/231375638-5bbf2989-fc7b-482a-b6fe-603d1d6d613f.svg" width="140" alt="SerpApi">
 </div>
 <a href="https://serpapi.com">
 	<b>API to get search engine results with ease.</b>
 </a>
 </div>
 
 _____
@@ -154,42 +154,15 @@
 ```
 
 This query will search all profiles from 2 universities based on "computer vision" query.
 </details>
 
 
 <details>
-<summary>Output</summary>
-
-Regular print: 
-
-```lang-none
-Adam Lobel
-['Gaming', 'Emotion regulation']
-Daniel Blizzard
-None
-Shuo Chen
-['Machine Learning', 'Data Mining', 'Artificial Intelligence']
-Ian Livingston
-['Human-computer interaction', 'User Experience', 'Player Experience', 'User Research', 'Games']
-Minli Xu
-['Game', 'Machine Learning', 'Data Science', 'Bioinformatics']
-Je Seok Lee
-['HCI', 'Player Experience', 'Games', 'Esports']
-Alisha Ness
-None
-Xingyu (Alfred) Liu
-['Machine Learning in Game Development']
-Amanda LL Cullen
-['Games Studies', 'Fan Studies', 'Live Streaming']
-Nicole "Nikki" Crenshaw
-['MMOs', 'Neoliberalism', 'Social Affordances', 'Identity', 'Accessibility']
-```
-
-And a JSON:
+<summary>JSON output</summary>
 
 ```json
 [
   {
     "name": "Adam Lobel",
     "link": "https://scholar.google.com/citations?hl=en&user=_xwYD2sAAAAJ",
     "affiliations": "Blizzard Entertainment",
@@ -323,15 +296,15 @@
     pagination=False,
     # other params
 )
 print(json.dumps(data, indent=2))
 ```
 
 <details>
-<summary>Output</summary>
+<summary>JSON output</summary>
 
 ```json
 [
   {
     "position": 0,
     "title": "Mining learning and crafting scientific experiments: a literature review on the use of minecraft in education and research",
     "result_id": "61OUs-3P374J",
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scrape-google-scholar-py Version: 0.3.1 Summary:
+Metadata-Version: 2.1 Name: scrape-google-scholar-py Version: 0.3.2 Summary:
 Extract data from all Google Scholar pages in Python. Sponsored by SerpApi.
 Home-page: https://github.com/dimitryzub/scrape-google-scholar Author: Dmitiry
 Zub Author-email: dimitryzub@gmail.com Maintainer: Dmitiry Zub Maintainer-
 email: dimitryzub@gmail.com License: MIT Project-URL: Documentation, https://
 github.com/dimitryzub/scrape-google-scholar#example-usage-custom-backend
 Project-URL: Source, https://github.com/dimitryzub/scrape-google-scholar
 Project-URL: Tracker, https://github.com/dimitryzub/scrape-google-scholar/
@@ -89,66 +89,57 @@
 usage custom backend ```python from google_scholar_py import
 CustomGoogleScholarProfiles import json parser = CustomGoogleScholarProfiles()
 data = parser.scrape_google_scholar_profiles( query='blizzard',
 pagination=False, save_to_csv=False, save_to_json=False ) print(json.dumps
 (data, indent=2)) ```  Google Scholar search operators could also be used
 ```lang-none label:computer_vision "Michigan State University"|"U.Michigan" ```
 This query will search all profiles from 2 universities based on "computer
-vision" query.   Output Regular print: ```lang-none Adam Lobel ['Gaming',
-'Emotion regulation'] Daniel Blizzard None Shuo Chen ['Machine Learning', 'Data
-Mining', 'Artificial Intelligence'] Ian Livingston ['Human-computer
-interaction', 'User Experience', 'Player Experience', 'User Research', 'Games']
-Minli Xu ['Game', 'Machine Learning', 'Data Science', 'Bioinformatics'] Je Seok
-Lee ['HCI', 'Player Experience', 'Games', 'Esports'] Alisha Ness None Xingyu
-(Alfred) Liu ['Machine Learning in Game Development'] Amanda LL Cullen ['Games
-Studies', 'Fan Studies', 'Live Streaming'] Nicole "Nikki" Crenshaw ['MMOs',
-'Neoliberalism', 'Social Affordances', 'Identity', 'Accessibility'] ``` And a
-JSON: ```json [ { "name": "Adam Lobel", "link": "https://scholar.google.com/
-citations?hl=en&user=_xwYD2sAAAAJ", "affiliations": "Blizzard Entertainment",
-"interests": [ "Gaming", "Emotion regulation" ], "email": "Verified email at
-AdamLobel.com", "cited_by_count": 3593 }, { "name": "Daniel Blizzard", "link":
-"https://scholar.google.com/citations?hl=en&user=dk4LWEgAAAAJ", "affiliations":
-"", "interests": null, "email": null, "cited_by_count": 1041 }, { "name": "Shuo
-Chen", "link": "https://scholar.google.com/citations?hl=en&user=OBf4YnkAAAAJ",
-"affiliations": "Senior Data Scientist, Blizzard Entertainment", "interests":
-[ "Machine Learning", "Data Mining", "Artificial Intelligence" ], "email":
-"Verified email at cs.cornell.edu", "cited_by_count": 725 }, { "name": "Ian
-Livingston", "link": "https://scholar.google.com/
-citations?hl=en&user=xBHVqNIAAAAJ", "affiliations": "Blizzard Entertainment",
-"interests": [ "Human-computer interaction", "User Experience", "Player
-Experience", "User Research", "Games" ], "email": "Verified email at usask.ca",
-"cited_by_count": 652 }, { "name": "Minli Xu", "link": "https://
-scholar.google.com/citations?hl=en&user=QST5iogAAAAJ", "affiliations":
-"Blizzard Entertainment", "interests": [ "Game", "Machine Learning", "Data
-Science", "Bioinformatics" ], "email": "Verified email at blizzard.com",
-"cited_by_count": 541 }, { "name": "Je Seok Lee", "link": "https://
-scholar.google.com/citations?hl=en&user=vuvtlzQAAAAJ", "affiliations":
-"Blizzard Entertainment", "interests": [ "HCI", "Player Experience", "Games",
-"Esports" ], "email": "Verified email at uci.edu", "cited_by_count": 386 },
-{ "name": "Alisha Ness", "link": "https://scholar.google.com/
-citations?hl=en&user=xQuwVfkAAAAJ", "affiliations": "Activision Blizzard",
-"interests": null, "email": null, "cited_by_count": 324 }, { "name": "Xingyu
-(Alfred) Liu", "link": "https://scholar.google.com/
-citations?hl=en&user=VW9ukOwAAAAJ", "affiliations": "Blizzard Entertainment",
-"interests": [ "Machine Learning in Game Development" ], "email": null,
-"cited_by_count": 256 }, { "name": "Amanda LL Cullen", "link": "https://
-scholar.google.com/citations?hl=en&user=oqna6OgAAAAJ", "affiliations":
-"Blizzard Entertainment", "interests": [ "Games Studies", "Fan Studies", "Live
-Streaming" ], "email": null, "cited_by_count": 247 }, { "name": "Nicole
-\"Nikki\" Crenshaw", "link": "https://scholar.google.com/
+vision" query.   JSON output ```json [ { "name": "Adam Lobel", "link": "https:/
+/scholar.google.com/citations?hl=en&user=_xwYD2sAAAAJ", "affiliations":
+"Blizzard Entertainment", "interests": [ "Gaming", "Emotion regulation" ],
+"email": "Verified email at AdamLobel.com", "cited_by_count": 3593 }, { "name":
+"Daniel Blizzard", "link": "https://scholar.google.com/
+citations?hl=en&user=dk4LWEgAAAAJ", "affiliations": "", "interests": null,
+"email": null, "cited_by_count": 1041 }, { "name": "Shuo Chen", "link": "https:
+//scholar.google.com/citations?hl=en&user=OBf4YnkAAAAJ", "affiliations":
+"Senior Data Scientist, Blizzard Entertainment", "interests": [ "Machine
+Learning", "Data Mining", "Artificial Intelligence" ], "email": "Verified email
+at cs.cornell.edu", "cited_by_count": 725 }, { "name": "Ian Livingston",
+"link": "https://scholar.google.com/citations?hl=en&user=xBHVqNIAAAAJ",
+"affiliations": "Blizzard Entertainment", "interests": [ "Human-computer
+interaction", "User Experience", "Player Experience", "User Research", "Games"
+], "email": "Verified email at usask.ca", "cited_by_count": 652 }, { "name":
+"Minli Xu", "link": "https://scholar.google.com/
+citations?hl=en&user=QST5iogAAAAJ", "affiliations": "Blizzard Entertainment",
+"interests": [ "Game", "Machine Learning", "Data Science", "Bioinformatics" ],
+"email": "Verified email at blizzard.com", "cited_by_count": 541 }, { "name":
+"Je Seok Lee", "link": "https://scholar.google.com/
+citations?hl=en&user=vuvtlzQAAAAJ", "affiliations": "Blizzard Entertainment",
+"interests": [ "HCI", "Player Experience", "Games", "Esports" ], "email":
+"Verified email at uci.edu", "cited_by_count": 386 }, { "name": "Alisha Ness",
+"link": "https://scholar.google.com/citations?hl=en&user=xQuwVfkAAAAJ",
+"affiliations": "Activision Blizzard", "interests": null, "email": null,
+"cited_by_count": 324 }, { "name": "Xingyu (Alfred) Liu", "link": "https://
+scholar.google.com/citations?hl=en&user=VW9ukOwAAAAJ", "affiliations":
+"Blizzard Entertainment", "interests": [ "Machine Learning in Game Development"
+], "email": null, "cited_by_count": 256 }, { "name": "Amanda LL Cullen",
+"link": "https://scholar.google.com/citations?hl=en&user=oqna6OgAAAAJ",
+"affiliations": "Blizzard Entertainment", "interests": [ "Games Studies", "Fan
+Studies", "Live Streaming" ], "email": null, "cited_by_count": 247 }, { "name":
+"Nicole \"Nikki\" Crenshaw", "link": "https://scholar.google.com/
 citations?hl=en&user=zmRH6E0AAAAJ", "affiliations": "Blizzard Entertainment",
 "interests": [ "MMOs", "Neoliberalism", "Social Affordances", "Identity",
 "Accessibility" ], "email": "Verified email at uci.edu", "cited_by_count": 202
 } ] ```  ## ðExample usage SerpApi backend ```python from google_scholar_py
 import SerpApiGoogleScholarOrganic import json profile_parser =
 SerpApiGoogleScholarProfiles() data =
 profile_parser.scrape_google_scholar_profile_results( query='blizzard',
 api_key='your-serpapi-api-key', # https://serpapi.com/manage-api-key
-pagination=False, # other params ) print(json.dumps(data, indent=2)) ```
-Output ```json [ { "position": 0, "title": "Mining learning and crafting
+pagination=False, # other params ) print(json.dumps(data, indent=2)) ```  JSON
+output ```json [ { "position": 0, "title": "Mining learning and crafting
 scientific experiments: a literature review on the use of minecraft in
 education and research", "result_id": "61OUs-3P374J", "link": "https://
 www.jstor.org/stable/pdf/jeductechsoci.19.2.355.pdf?&seq=1", "snippet": "\u2026
 Minecraft have aroused the attention of teachers and researchers alike. To gain
 insights into the applicability of Minecraft, \u2026 our own considerable
 experience with Minecraft in courses on \u2026", "publication_info":
 { "summary": "S Nebel, S Schneider, GD Rey - Journal of Educational Technology
```

### Comparing `scrape-google-scholar-py-0.3.1/README.md` & `scrape-google-scholar-py-0.3.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <div align="center">
 <p>Sponsor of the project:</p>
 <div>
-   <img src="https://sindresorhus.com/assets/thanks/serpapi-logo-light.svg" width="140" alt="SerpApi">
+   <img src="https://user-images.githubusercontent.com/78694043/231375638-5bbf2989-fc7b-482a-b6fe-603d1d6d613f.svg" width="140" alt="SerpApi">
 </div>
 <a href="https://serpapi.com">
 	<b>API to get search engine results with ease.</b>
 </a>
 </div>
 
 _____
@@ -127,42 +127,15 @@
 ```
 
 This query will search all profiles from 2 universities based on "computer vision" query.
 </details>
 
 
 <details>
-<summary>Output</summary>
-
-Regular print: 
-
-```lang-none
-Adam Lobel
-['Gaming', 'Emotion regulation']
-Daniel Blizzard
-None
-Shuo Chen
-['Machine Learning', 'Data Mining', 'Artificial Intelligence']
-Ian Livingston
-['Human-computer interaction', 'User Experience', 'Player Experience', 'User Research', 'Games']
-Minli Xu
-['Game', 'Machine Learning', 'Data Science', 'Bioinformatics']
-Je Seok Lee
-['HCI', 'Player Experience', 'Games', 'Esports']
-Alisha Ness
-None
-Xingyu (Alfred) Liu
-['Machine Learning in Game Development']
-Amanda LL Cullen
-['Games Studies', 'Fan Studies', 'Live Streaming']
-Nicole "Nikki" Crenshaw
-['MMOs', 'Neoliberalism', 'Social Affordances', 'Identity', 'Accessibility']
-```
-
-And a JSON:
+<summary>JSON output</summary>
 
 ```json
 [
   {
     "name": "Adam Lobel",
     "link": "https://scholar.google.com/citations?hl=en&user=_xwYD2sAAAAJ",
     "affiliations": "Blizzard Entertainment",
@@ -296,15 +269,15 @@
     pagination=False,
     # other params
 )
 print(json.dumps(data, indent=2))
 ```
 
 <details>
-<summary>Output</summary>
+<summary>JSON output</summary>
 
 ```json
 [
   {
     "position": 0,
     "title": "Mining learning and crafting scientific experiments: a literature review on the use of minecraft in education and research",
     "result_id": "61OUs-3P374J",
@@ -756,8 +729,8 @@
 
 If you find comfortable to open a PR, feel free to do so. Guidelines are simple: conventional commits + code as simple as possible without unnecessary complexity.
 
 There's exists a `.gitpod.yaml` config if you're using [Gitpod](https://www.gitpod.io/). 
 
 ## 📜Licence
 
-`scrape-google-scholar` repository is licensed under MIT license.
+`scrape-google-scholar` repository is licensed under MIT license.
```

#### html2text {}

```diff
@@ -71,66 +71,57 @@
 usage custom backend ```python from google_scholar_py import
 CustomGoogleScholarProfiles import json parser = CustomGoogleScholarProfiles()
 data = parser.scrape_google_scholar_profiles( query='blizzard',
 pagination=False, save_to_csv=False, save_to_json=False ) print(json.dumps
 (data, indent=2)) ```  Google Scholar search operators could also be used
 ```lang-none label:computer_vision "Michigan State University"|"U.Michigan" ```
 This query will search all profiles from 2 universities based on "computer
-vision" query.   Output Regular print: ```lang-none Adam Lobel ['Gaming',
-'Emotion regulation'] Daniel Blizzard None Shuo Chen ['Machine Learning', 'Data
-Mining', 'Artificial Intelligence'] Ian Livingston ['Human-computer
-interaction', 'User Experience', 'Player Experience', 'User Research', 'Games']
-Minli Xu ['Game', 'Machine Learning', 'Data Science', 'Bioinformatics'] Je Seok
-Lee ['HCI', 'Player Experience', 'Games', 'Esports'] Alisha Ness None Xingyu
-(Alfred) Liu ['Machine Learning in Game Development'] Amanda LL Cullen ['Games
-Studies', 'Fan Studies', 'Live Streaming'] Nicole "Nikki" Crenshaw ['MMOs',
-'Neoliberalism', 'Social Affordances', 'Identity', 'Accessibility'] ``` And a
-JSON: ```json [ { "name": "Adam Lobel", "link": "https://scholar.google.com/
-citations?hl=en&user=_xwYD2sAAAAJ", "affiliations": "Blizzard Entertainment",
-"interests": [ "Gaming", "Emotion regulation" ], "email": "Verified email at
-AdamLobel.com", "cited_by_count": 3593 }, { "name": "Daniel Blizzard", "link":
-"https://scholar.google.com/citations?hl=en&user=dk4LWEgAAAAJ", "affiliations":
-"", "interests": null, "email": null, "cited_by_count": 1041 }, { "name": "Shuo
-Chen", "link": "https://scholar.google.com/citations?hl=en&user=OBf4YnkAAAAJ",
-"affiliations": "Senior Data Scientist, Blizzard Entertainment", "interests":
-[ "Machine Learning", "Data Mining", "Artificial Intelligence" ], "email":
-"Verified email at cs.cornell.edu", "cited_by_count": 725 }, { "name": "Ian
-Livingston", "link": "https://scholar.google.com/
-citations?hl=en&user=xBHVqNIAAAAJ", "affiliations": "Blizzard Entertainment",
-"interests": [ "Human-computer interaction", "User Experience", "Player
-Experience", "User Research", "Games" ], "email": "Verified email at usask.ca",
-"cited_by_count": 652 }, { "name": "Minli Xu", "link": "https://
-scholar.google.com/citations?hl=en&user=QST5iogAAAAJ", "affiliations":
-"Blizzard Entertainment", "interests": [ "Game", "Machine Learning", "Data
-Science", "Bioinformatics" ], "email": "Verified email at blizzard.com",
-"cited_by_count": 541 }, { "name": "Je Seok Lee", "link": "https://
-scholar.google.com/citations?hl=en&user=vuvtlzQAAAAJ", "affiliations":
-"Blizzard Entertainment", "interests": [ "HCI", "Player Experience", "Games",
-"Esports" ], "email": "Verified email at uci.edu", "cited_by_count": 386 },
-{ "name": "Alisha Ness", "link": "https://scholar.google.com/
-citations?hl=en&user=xQuwVfkAAAAJ", "affiliations": "Activision Blizzard",
-"interests": null, "email": null, "cited_by_count": 324 }, { "name": "Xingyu
-(Alfred) Liu", "link": "https://scholar.google.com/
-citations?hl=en&user=VW9ukOwAAAAJ", "affiliations": "Blizzard Entertainment",
-"interests": [ "Machine Learning in Game Development" ], "email": null,
-"cited_by_count": 256 }, { "name": "Amanda LL Cullen", "link": "https://
-scholar.google.com/citations?hl=en&user=oqna6OgAAAAJ", "affiliations":
-"Blizzard Entertainment", "interests": [ "Games Studies", "Fan Studies", "Live
-Streaming" ], "email": null, "cited_by_count": 247 }, { "name": "Nicole
-\"Nikki\" Crenshaw", "link": "https://scholar.google.com/
+vision" query.   JSON output ```json [ { "name": "Adam Lobel", "link": "https:/
+/scholar.google.com/citations?hl=en&user=_xwYD2sAAAAJ", "affiliations":
+"Blizzard Entertainment", "interests": [ "Gaming", "Emotion regulation" ],
+"email": "Verified email at AdamLobel.com", "cited_by_count": 3593 }, { "name":
+"Daniel Blizzard", "link": "https://scholar.google.com/
+citations?hl=en&user=dk4LWEgAAAAJ", "affiliations": "", "interests": null,
+"email": null, "cited_by_count": 1041 }, { "name": "Shuo Chen", "link": "https:
+//scholar.google.com/citations?hl=en&user=OBf4YnkAAAAJ", "affiliations":
+"Senior Data Scientist, Blizzard Entertainment", "interests": [ "Machine
+Learning", "Data Mining", "Artificial Intelligence" ], "email": "Verified email
+at cs.cornell.edu", "cited_by_count": 725 }, { "name": "Ian Livingston",
+"link": "https://scholar.google.com/citations?hl=en&user=xBHVqNIAAAAJ",
+"affiliations": "Blizzard Entertainment", "interests": [ "Human-computer
+interaction", "User Experience", "Player Experience", "User Research", "Games"
+], "email": "Verified email at usask.ca", "cited_by_count": 652 }, { "name":
+"Minli Xu", "link": "https://scholar.google.com/
+citations?hl=en&user=QST5iogAAAAJ", "affiliations": "Blizzard Entertainment",
+"interests": [ "Game", "Machine Learning", "Data Science", "Bioinformatics" ],
+"email": "Verified email at blizzard.com", "cited_by_count": 541 }, { "name":
+"Je Seok Lee", "link": "https://scholar.google.com/
+citations?hl=en&user=vuvtlzQAAAAJ", "affiliations": "Blizzard Entertainment",
+"interests": [ "HCI", "Player Experience", "Games", "Esports" ], "email":
+"Verified email at uci.edu", "cited_by_count": 386 }, { "name": "Alisha Ness",
+"link": "https://scholar.google.com/citations?hl=en&user=xQuwVfkAAAAJ",
+"affiliations": "Activision Blizzard", "interests": null, "email": null,
+"cited_by_count": 324 }, { "name": "Xingyu (Alfred) Liu", "link": "https://
+scholar.google.com/citations?hl=en&user=VW9ukOwAAAAJ", "affiliations":
+"Blizzard Entertainment", "interests": [ "Machine Learning in Game Development"
+], "email": null, "cited_by_count": 256 }, { "name": "Amanda LL Cullen",
+"link": "https://scholar.google.com/citations?hl=en&user=oqna6OgAAAAJ",
+"affiliations": "Blizzard Entertainment", "interests": [ "Games Studies", "Fan
+Studies", "Live Streaming" ], "email": null, "cited_by_count": 247 }, { "name":
+"Nicole \"Nikki\" Crenshaw", "link": "https://scholar.google.com/
 citations?hl=en&user=zmRH6E0AAAAJ", "affiliations": "Blizzard Entertainment",
 "interests": [ "MMOs", "Neoliberalism", "Social Affordances", "Identity",
 "Accessibility" ], "email": "Verified email at uci.edu", "cited_by_count": 202
 } ] ```  ## ðExample usage SerpApi backend ```python from google_scholar_py
 import SerpApiGoogleScholarOrganic import json profile_parser =
 SerpApiGoogleScholarProfiles() data =
 profile_parser.scrape_google_scholar_profile_results( query='blizzard',
 api_key='your-serpapi-api-key', # https://serpapi.com/manage-api-key
-pagination=False, # other params ) print(json.dumps(data, indent=2)) ```
-Output ```json [ { "position": 0, "title": "Mining learning and crafting
+pagination=False, # other params ) print(json.dumps(data, indent=2)) ```  JSON
+output ```json [ { "position": 0, "title": "Mining learning and crafting
 scientific experiments: a literature review on the use of minecraft in
 education and research", "result_id": "61OUs-3P374J", "link": "https://
 www.jstor.org/stable/pdf/jeductechsoci.19.2.355.pdf?&seq=1", "snippet": "\u2026
 Minecraft have aroused the attention of teachers and researchers alike. To gain
 insights into the applicability of Minecraft, \u2026 our own considerable
 experience with Minecraft in courses on \u2026", "publication_info":
 { "summary": "S Nebel, S Schneider, GD Rey - Journal of Educational Technology
```

### Comparing `scrape-google-scholar-py-0.3.1/google_scholar_py/__init__.py` & `scrape-google-scholar-py-0.3.2/google_scholar_py/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # custom backend
 from .custom_backend.organic_search import CustomGoogleScholarOrganic
 from .custom_backend.profiles_results import CustomGoogleScholarProfiles
 from .custom_backend.author_info_all_articles import CustomGoogleScholarAuthor
 from .custom_backend.top_mandates_metrics import CustomGoogleScholarTopMandates
 from .custom_backend.top_publications_metrics import CustomGoogleScholarTopPublications
+from .custom_backend.top_publications_article_citations import CustomGoogleScholarTopPublicationCitations
 
 # serpapi backend
 from .serpapi_backend.organic_results import SerpApiGoogleScholarOrganic
 from .serpapi_backend.profile_results import SerpApiGoogleScholarProfiles
 from .serpapi_backend.organic_cite_results import SerpApiGoogleScholarOrganicCite
 from .serpapi_backend.author_results import SerpApiGoogleScholarAuthor
```

### Comparing `scrape-google-scholar-py-0.3.1/google_scholar_py/custom_backend/author_info_all_articles.py` & `scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/author_info_all_articles.py`

 * *Files identical despite different names*

### Comparing `scrape-google-scholar-py-0.3.1/google_scholar_py/custom_backend/cite_results.py` & `scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/cite_results.py`

 * *Files identical despite different names*

### Comparing `scrape-google-scholar-py-0.3.1/google_scholar_py/custom_backend/google_scholar_cited_by_public_access_author.py` & `scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/google_scholar_cited_by_public_access_author.py`

 * *Files identical despite different names*

### Comparing `scrape-google-scholar-py-0.3.1/google_scholar_py/custom_backend/organic_search.py` & `scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/organic_search.py`

 * *Files identical despite different names*

### Comparing `scrape-google-scholar-py-0.3.1/google_scholar_py/custom_backend/profiles_results.py` & `scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/profiles_results.py`

 * *Files identical despite different names*

### Comparing `scrape-google-scholar-py-0.3.1/google_scholar_py/custom_backend/top_mandates_metrics.py` & `scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/top_mandates_metrics.py`

 * *Files identical despite different names*

### Comparing `scrape-google-scholar-py-0.3.1/google_scholar_py/custom_backend/top_publications_metrics.py` & `scrape-google-scholar-py-0.3.2/google_scholar_py/custom_backend/top_publications_metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from selenium import webdriver
 from selenium_stealth import stealth
 from selenium.webdriver.chrome.service import Service
 from webdriver_manager.chrome import ChromeDriverManager
 from selectolax.lexbor import LexborHTMLParser
-from typing import List, Dict, Callable
+from typing import List, Dict, Callable, Union
 import pandas as pd
-from pathlib import Path
 
 class CustomGoogleScholarTopPublications:
     def __init__(self) -> None:
         pass
 
 
     def parse(self, parser: Callable, top_publications_data: Callable):
@@ -22,16 +21,16 @@
         
         It's used by google_scholar_top_publication_metrics().
         
         It returns nothing as it appends data to `top_publications_data`, 
         which appends it to `top_publications_data` List in the google_scholar_top_publication_metrics() function.
         '''
 
-        
-        for table in parser.css('tr'):
+        # selectors skips table header row
+        for table in parser.css('tr:not(:first-child)'):
             try:
                 title: str = table.css_first('td.gsc_mvt_t').text()
             except: title = None
             
             try: 
                 h5_index: int = table.css_first('a.gs_ibl').text()
             except: h5_index = None
@@ -54,15 +53,15 @@
 
     def scrape_top_publication_metrics(
             self,
             category: str = '', 
             lang: str = 'en',
             save_to_csv: bool = False, 
             save_to_json: bool = False,
-        ) -> List[Dict[str, str]]:
+        ) -> List[Dict[str, Union[str, int]]]:
         #TODO add subcategories to subcategory arg
         #TODO: support other languages: lang='spanish' -> 'sp'. https://serpapi.com/google-languages
 
 
         '''
         Results comes from: https://scholar.google.com/citations?view_op=top_venues
         
@@ -72,30 +71,30 @@
         - h5_index_link: str
         - h5_median: int
         
         Arguments: 
         - save_to_csv: True of False. Default is False. Saves data to CSV file.
         - save_to_json: True of False. Default is False. Saves data to JSON file.
         - lang: str. Language. Defaults to English ('en'). For now, need to be checked yourself. Other languages: https://serpapi.com/google-languages
-        - category: str
+        - category: str. Available categories showed in the function documentation below.
             Available categories:
             - "bus": Business, Economics & Management
             - "chm": Chemical & Material Sciences
             - "eng": Engineering & Computer Science
             - "med": Health & Medical Sciences
             - "hum": Humanities, Literature & Arts
             - "bio": Life Sciences & Earth Sciences
             - "phy": Physics & Mathematics
             - "soc": Social Sciences
             
         Usage:
         
         from google_scholar_py import CustomGoogleScholarTopPublications
         
-        data = google_scholar_top_publication_metrics(category='eng', ...) # sv = swedish
+        data = CustomGoogleScholarTopPublications().scrape_top_publication_metrics(category='eng', lang='en') # sv = swedish
         
         for result in data:
             print(result['title'])
             ...
         '''
         
         # selenium stealth
```

### Comparing `scrape-google-scholar-py-0.3.1/google_scholar_py/serpapi_backend/author_results.py` & `scrape-google-scholar-py-0.3.2/google_scholar_py/serpapi_backend/author_results.py`

 * *Files identical despite different names*

### Comparing `scrape-google-scholar-py-0.3.1/google_scholar_py/serpapi_backend/organic_cite_results.py` & `scrape-google-scholar-py-0.3.2/google_scholar_py/serpapi_backend/organic_cite_results.py`

 * *Files identical despite different names*

### Comparing `scrape-google-scholar-py-0.3.1/google_scholar_py/serpapi_backend/organic_results.py` & `scrape-google-scholar-py-0.3.2/google_scholar_py/serpapi_backend/organic_results.py`

 * *Files identical despite different names*

### Comparing `scrape-google-scholar-py-0.3.1/google_scholar_py/serpapi_backend/profile_results.py` & `scrape-google-scholar-py-0.3.2/google_scholar_py/serpapi_backend/profile_results.py`

 * *Files identical despite different names*

### Comparing `scrape-google-scholar-py-0.3.1/requirements.txt` & `scrape-google-scholar-py-0.3.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `scrape-google-scholar-py-0.3.1/scrape_google_scholar_py.egg-info/PKG-INFO` & `scrape-google-scholar-py-0.3.2/scrape_google_scholar_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrape-google-scholar-py
-Version: 0.3.1
+Version: 0.3.2
 Summary: Extract data from all Google Scholar pages in Python. Sponsored by SerpApi.
 Home-page: https://github.com/dimitryzub/scrape-google-scholar
 Author: Dmitiry Zub
 Author-email: dimitryzub@gmail.com
 Maintainer: Dmitiry Zub
 Maintainer-email: dimitryzub@gmail.com
 License: MIT
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 <div align="center">
 <p>Sponsor of the project:</p>
 <div>
-   <img src="https://sindresorhus.com/assets/thanks/serpapi-logo-light.svg" width="140" alt="SerpApi">
+   <img src="https://user-images.githubusercontent.com/78694043/231375638-5bbf2989-fc7b-482a-b6fe-603d1d6d613f.svg" width="140" alt="SerpApi">
 </div>
 <a href="https://serpapi.com">
 	<b>API to get search engine results with ease.</b>
 </a>
 </div>
 
 _____
@@ -154,42 +154,15 @@
 ```
 
 This query will search all profiles from 2 universities based on "computer vision" query.
 </details>
 
 
 <details>
-<summary>Output</summary>
-
-Regular print: 
-
-```lang-none
-Adam Lobel
-['Gaming', 'Emotion regulation']
-Daniel Blizzard
-None
-Shuo Chen
-['Machine Learning', 'Data Mining', 'Artificial Intelligence']
-Ian Livingston
-['Human-computer interaction', 'User Experience', 'Player Experience', 'User Research', 'Games']
-Minli Xu
-['Game', 'Machine Learning', 'Data Science', 'Bioinformatics']
-Je Seok Lee
-['HCI', 'Player Experience', 'Games', 'Esports']
-Alisha Ness
-None
-Xingyu (Alfred) Liu
-['Machine Learning in Game Development']
-Amanda LL Cullen
-['Games Studies', 'Fan Studies', 'Live Streaming']
-Nicole "Nikki" Crenshaw
-['MMOs', 'Neoliberalism', 'Social Affordances', 'Identity', 'Accessibility']
-```
-
-And a JSON:
+<summary>JSON output</summary>
 
 ```json
 [
   {
     "name": "Adam Lobel",
     "link": "https://scholar.google.com/citations?hl=en&user=_xwYD2sAAAAJ",
     "affiliations": "Blizzard Entertainment",
@@ -323,15 +296,15 @@
     pagination=False,
     # other params
 )
 print(json.dumps(data, indent=2))
 ```
 
 <details>
-<summary>Output</summary>
+<summary>JSON output</summary>
 
 ```json
 [
   {
     "position": 0,
     "title": "Mining learning and crafting scientific experiments: a literature review on the use of minecraft in education and research",
     "result_id": "61OUs-3P374J",
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scrape-google-scholar-py Version: 0.3.1 Summary:
+Metadata-Version: 2.1 Name: scrape-google-scholar-py Version: 0.3.2 Summary:
 Extract data from all Google Scholar pages in Python. Sponsored by SerpApi.
 Home-page: https://github.com/dimitryzub/scrape-google-scholar Author: Dmitiry
 Zub Author-email: dimitryzub@gmail.com Maintainer: Dmitiry Zub Maintainer-
 email: dimitryzub@gmail.com License: MIT Project-URL: Documentation, https://
 github.com/dimitryzub/scrape-google-scholar#example-usage-custom-backend
 Project-URL: Source, https://github.com/dimitryzub/scrape-google-scholar
 Project-URL: Tracker, https://github.com/dimitryzub/scrape-google-scholar/
@@ -89,66 +89,57 @@
 usage custom backend ```python from google_scholar_py import
 CustomGoogleScholarProfiles import json parser = CustomGoogleScholarProfiles()
 data = parser.scrape_google_scholar_profiles( query='blizzard',
 pagination=False, save_to_csv=False, save_to_json=False ) print(json.dumps
 (data, indent=2)) ```  Google Scholar search operators could also be used
 ```lang-none label:computer_vision "Michigan State University"|"U.Michigan" ```
 This query will search all profiles from 2 universities based on "computer
-vision" query.   Output Regular print: ```lang-none Adam Lobel ['Gaming',
-'Emotion regulation'] Daniel Blizzard None Shuo Chen ['Machine Learning', 'Data
-Mining', 'Artificial Intelligence'] Ian Livingston ['Human-computer
-interaction', 'User Experience', 'Player Experience', 'User Research', 'Games']
-Minli Xu ['Game', 'Machine Learning', 'Data Science', 'Bioinformatics'] Je Seok
-Lee ['HCI', 'Player Experience', 'Games', 'Esports'] Alisha Ness None Xingyu
-(Alfred) Liu ['Machine Learning in Game Development'] Amanda LL Cullen ['Games
-Studies', 'Fan Studies', 'Live Streaming'] Nicole "Nikki" Crenshaw ['MMOs',
-'Neoliberalism', 'Social Affordances', 'Identity', 'Accessibility'] ``` And a
-JSON: ```json [ { "name": "Adam Lobel", "link": "https://scholar.google.com/
-citations?hl=en&user=_xwYD2sAAAAJ", "affiliations": "Blizzard Entertainment",
-"interests": [ "Gaming", "Emotion regulation" ], "email": "Verified email at
-AdamLobel.com", "cited_by_count": 3593 }, { "name": "Daniel Blizzard", "link":
-"https://scholar.google.com/citations?hl=en&user=dk4LWEgAAAAJ", "affiliations":
-"", "interests": null, "email": null, "cited_by_count": 1041 }, { "name": "Shuo
-Chen", "link": "https://scholar.google.com/citations?hl=en&user=OBf4YnkAAAAJ",
-"affiliations": "Senior Data Scientist, Blizzard Entertainment", "interests":
-[ "Machine Learning", "Data Mining", "Artificial Intelligence" ], "email":
-"Verified email at cs.cornell.edu", "cited_by_count": 725 }, { "name": "Ian
-Livingston", "link": "https://scholar.google.com/
-citations?hl=en&user=xBHVqNIAAAAJ", "affiliations": "Blizzard Entertainment",
-"interests": [ "Human-computer interaction", "User Experience", "Player
-Experience", "User Research", "Games" ], "email": "Verified email at usask.ca",
-"cited_by_count": 652 }, { "name": "Minli Xu", "link": "https://
-scholar.google.com/citations?hl=en&user=QST5iogAAAAJ", "affiliations":
-"Blizzard Entertainment", "interests": [ "Game", "Machine Learning", "Data
-Science", "Bioinformatics" ], "email": "Verified email at blizzard.com",
-"cited_by_count": 541 }, { "name": "Je Seok Lee", "link": "https://
-scholar.google.com/citations?hl=en&user=vuvtlzQAAAAJ", "affiliations":
-"Blizzard Entertainment", "interests": [ "HCI", "Player Experience", "Games",
-"Esports" ], "email": "Verified email at uci.edu", "cited_by_count": 386 },
-{ "name": "Alisha Ness", "link": "https://scholar.google.com/
-citations?hl=en&user=xQuwVfkAAAAJ", "affiliations": "Activision Blizzard",
-"interests": null, "email": null, "cited_by_count": 324 }, { "name": "Xingyu
-(Alfred) Liu", "link": "https://scholar.google.com/
-citations?hl=en&user=VW9ukOwAAAAJ", "affiliations": "Blizzard Entertainment",
-"interests": [ "Machine Learning in Game Development" ], "email": null,
-"cited_by_count": 256 }, { "name": "Amanda LL Cullen", "link": "https://
-scholar.google.com/citations?hl=en&user=oqna6OgAAAAJ", "affiliations":
-"Blizzard Entertainment", "interests": [ "Games Studies", "Fan Studies", "Live
-Streaming" ], "email": null, "cited_by_count": 247 }, { "name": "Nicole
-\"Nikki\" Crenshaw", "link": "https://scholar.google.com/
+vision" query.   JSON output ```json [ { "name": "Adam Lobel", "link": "https:/
+/scholar.google.com/citations?hl=en&user=_xwYD2sAAAAJ", "affiliations":
+"Blizzard Entertainment", "interests": [ "Gaming", "Emotion regulation" ],
+"email": "Verified email at AdamLobel.com", "cited_by_count": 3593 }, { "name":
+"Daniel Blizzard", "link": "https://scholar.google.com/
+citations?hl=en&user=dk4LWEgAAAAJ", "affiliations": "", "interests": null,
+"email": null, "cited_by_count": 1041 }, { "name": "Shuo Chen", "link": "https:
+//scholar.google.com/citations?hl=en&user=OBf4YnkAAAAJ", "affiliations":
+"Senior Data Scientist, Blizzard Entertainment", "interests": [ "Machine
+Learning", "Data Mining", "Artificial Intelligence" ], "email": "Verified email
+at cs.cornell.edu", "cited_by_count": 725 }, { "name": "Ian Livingston",
+"link": "https://scholar.google.com/citations?hl=en&user=xBHVqNIAAAAJ",
+"affiliations": "Blizzard Entertainment", "interests": [ "Human-computer
+interaction", "User Experience", "Player Experience", "User Research", "Games"
+], "email": "Verified email at usask.ca", "cited_by_count": 652 }, { "name":
+"Minli Xu", "link": "https://scholar.google.com/
+citations?hl=en&user=QST5iogAAAAJ", "affiliations": "Blizzard Entertainment",
+"interests": [ "Game", "Machine Learning", "Data Science", "Bioinformatics" ],
+"email": "Verified email at blizzard.com", "cited_by_count": 541 }, { "name":
+"Je Seok Lee", "link": "https://scholar.google.com/
+citations?hl=en&user=vuvtlzQAAAAJ", "affiliations": "Blizzard Entertainment",
+"interests": [ "HCI", "Player Experience", "Games", "Esports" ], "email":
+"Verified email at uci.edu", "cited_by_count": 386 }, { "name": "Alisha Ness",
+"link": "https://scholar.google.com/citations?hl=en&user=xQuwVfkAAAAJ",
+"affiliations": "Activision Blizzard", "interests": null, "email": null,
+"cited_by_count": 324 }, { "name": "Xingyu (Alfred) Liu", "link": "https://
+scholar.google.com/citations?hl=en&user=VW9ukOwAAAAJ", "affiliations":
+"Blizzard Entertainment", "interests": [ "Machine Learning in Game Development"
+], "email": null, "cited_by_count": 256 }, { "name": "Amanda LL Cullen",
+"link": "https://scholar.google.com/citations?hl=en&user=oqna6OgAAAAJ",
+"affiliations": "Blizzard Entertainment", "interests": [ "Games Studies", "Fan
+Studies", "Live Streaming" ], "email": null, "cited_by_count": 247 }, { "name":
+"Nicole \"Nikki\" Crenshaw", "link": "https://scholar.google.com/
 citations?hl=en&user=zmRH6E0AAAAJ", "affiliations": "Blizzard Entertainment",
 "interests": [ "MMOs", "Neoliberalism", "Social Affordances", "Identity",
 "Accessibility" ], "email": "Verified email at uci.edu", "cited_by_count": 202
 } ] ```  ## ðExample usage SerpApi backend ```python from google_scholar_py
 import SerpApiGoogleScholarOrganic import json profile_parser =
 SerpApiGoogleScholarProfiles() data =
 profile_parser.scrape_google_scholar_profile_results( query='blizzard',
 api_key='your-serpapi-api-key', # https://serpapi.com/manage-api-key
-pagination=False, # other params ) print(json.dumps(data, indent=2)) ```
-Output ```json [ { "position": 0, "title": "Mining learning and crafting
+pagination=False, # other params ) print(json.dumps(data, indent=2)) ```  JSON
+output ```json [ { "position": 0, "title": "Mining learning and crafting
 scientific experiments: a literature review on the use of minecraft in
 education and research", "result_id": "61OUs-3P374J", "link": "https://
 www.jstor.org/stable/pdf/jeductechsoci.19.2.355.pdf?&seq=1", "snippet": "\u2026
 Minecraft have aroused the attention of teachers and researchers alike. To gain
 insights into the applicability of Minecraft, \u2026 our own considerable
 experience with Minecraft in courses on \u2026", "publication_info":
 { "summary": "S Nebel, S Schneider, GD Rey - Journal of Educational Technology
```

### Comparing `scrape-google-scholar-py-0.3.1/scrape_google_scholar_py.egg-info/SOURCES.txt` & `scrape-google-scholar-py-0.3.2/scrape_google_scholar_py.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 google_scholar_py/__init__.py
 google_scholar_py/custom_backend/author_info_all_articles.py
 google_scholar_py/custom_backend/cite_results.py
 google_scholar_py/custom_backend/google_scholar_cited_by_public_access_author.py
 google_scholar_py/custom_backend/organic_search.py
 google_scholar_py/custom_backend/profiles_results.py
 google_scholar_py/custom_backend/top_mandates_metrics.py
+google_scholar_py/custom_backend/top_metrics_category_h5.py
+google_scholar_py/custom_backend/top_publications_article_citations.py
 google_scholar_py/custom_backend/top_publications_metrics.py
 google_scholar_py/serpapi_backend/author_results.py
 google_scholar_py/serpapi_backend/organic_cite_results.py
 google_scholar_py/serpapi_backend/organic_results.py
 google_scholar_py/serpapi_backend/profile_results.py
 scrape_google_scholar_py.egg-info/PKG-INFO
 scrape_google_scholar_py.egg-info/SOURCES.txt
```

### Comparing `scrape-google-scholar-py-0.3.1/setup.py` & `scrape-google-scholar-py-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open('README.md', 'r', encoding='utf-8') as readme_file:
     README = readme_file.read()
 
 setup(
     name='scrape-google-scholar-py',
     description = 'Extract data from all Google Scholar pages in Python. Sponsored by SerpApi.',
     url='https://github.com/dimitryzub/scrape-google-scholar',
-    version='0.3.1',
+    version='0.3.2',
     license='MIT',
     author='Dmitiry Zub',
     author_email='dimitryzub@gmail.com',
     maintainer='Dmitiry Zub',
     maintainer_email='dimitryzub@gmail.com',
     long_description_content_type='text/markdown',
     long_description=README,
```

