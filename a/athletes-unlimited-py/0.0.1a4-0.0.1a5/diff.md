# Comparing `tmp/athletes_unlimited_py-0.0.1a4.tar.gz` & `tmp/athletes_unlimited_py-0.0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athletes_unlimited_py-0.0.1a4.tar", last modified: Wed Apr 12 03:21:16 2023, max compression
+gzip compressed data, was "athletes_unlimited_py-0.0.1a5.tar", last modified: Wed Apr 12 23:11:28 2023, max compression
```

## Comparing `athletes_unlimited_py-0.0.1a4.tar` & `athletes_unlimited_py-0.0.1a5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:21:16.242437 athletes_unlimited_py-0.0.1a4/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-12 03:20:53.000000 athletes_unlimited_py-0.0.1a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-12 03:21:16.242437 athletes_unlimited_py-0.0.1a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-12 03:20:53.000000 athletes_unlimited_py-0.0.1a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:21:16.242437 athletes_unlimited_py-0.0.1a4/athetes_unlimited_py/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-12 03:20:53.000000 athletes_unlimited_py-0.0.1a4/athetes_unlimited_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-04-12 03:20:53.000000 athletes_unlimited_py-0.0.1a4/athetes_unlimited_py/aux_softball.py
--rw-r--r--   0 runner    (1001) docker     (123)    22949 2023-04-12 03:20:53.000000 athletes_unlimited_py-0.0.1a4/athetes_unlimited_py/basketball.py
--rw-r--r--   0 runner    (1001) docker     (123)    22245 2023-04-12 03:20:53.000000 athletes_unlimited_py-0.0.1a4/athetes_unlimited_py/lacrosse.py
--rw-r--r--   0 runner    (1001) docker     (123)    28000 2023-04-12 03:20:53.000000 athletes_unlimited_py-0.0.1a4/athetes_unlimited_py/softball.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-12 03:20:53.000000 athletes_unlimited_py-0.0.1a4/athetes_unlimited_py/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 03:20:53.000000 athletes_unlimited_py-0.0.1a4/athetes_unlimited_py/volleyball.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:21:16.242437 athletes_unlimited_py-0.0.1a4/athletes_unlimited_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-12 03:21:16.000000 athletes_unlimited_py-0.0.1a4/athletes_unlimited_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-12 03:21:16.000000 athletes_unlimited_py-0.0.1a4/athletes_unlimited_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 03:21:16.000000 athletes_unlimited_py-0.0.1a4/athletes_unlimited_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-12 03:21:16.000000 athletes_unlimited_py-0.0.1a4/athletes_unlimited_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 03:21:16.000000 athletes_unlimited_py-0.0.1a4/athletes_unlimited_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-12 03:20:53.000000 athletes_unlimited_py-0.0.1a4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 03:21:16.242437 athletes_unlimited_py-0.0.1a4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:11:28.068222 athletes_unlimited_py-0.0.1a5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-12 23:11:06.000000 athletes_unlimited_py-0.0.1a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-12 23:11:28.068222 athletes_unlimited_py-0.0.1a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-12 23:11:06.000000 athletes_unlimited_py-0.0.1a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:11:28.064222 athletes_unlimited_py-0.0.1a5/athetes_unlimited_py/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-12 23:11:06.000000 athletes_unlimited_py-0.0.1a5/athetes_unlimited_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-04-12 23:11:06.000000 athletes_unlimited_py-0.0.1a5/athetes_unlimited_py/aux_softball.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23032 2023-04-12 23:11:06.000000 athletes_unlimited_py-0.0.1a5/athetes_unlimited_py/basketball.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22245 2023-04-12 23:11:06.000000 athletes_unlimited_py-0.0.1a5/athetes_unlimited_py/lacrosse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28000 2023-04-12 23:11:06.000000 athletes_unlimited_py-0.0.1a5/athetes_unlimited_py/softball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-12 23:11:06.000000 athletes_unlimited_py-0.0.1a5/athetes_unlimited_py/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21428 2023-04-12 23:11:06.000000 athletes_unlimited_py-0.0.1a5/athetes_unlimited_py/volleyball.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:11:28.068222 athletes_unlimited_py-0.0.1a5/athletes_unlimited_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-12 23:11:28.000000 athletes_unlimited_py-0.0.1a5/athletes_unlimited_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-12 23:11:28.000000 athletes_unlimited_py-0.0.1a5/athletes_unlimited_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 23:11:28.000000 athletes_unlimited_py-0.0.1a5/athletes_unlimited_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-12 23:11:28.000000 athletes_unlimited_py-0.0.1a5/athletes_unlimited_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 23:11:28.000000 athletes_unlimited_py-0.0.1a5/athletes_unlimited_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-12 23:11:06.000000 athletes_unlimited_py-0.0.1a5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 23:11:28.068222 athletes_unlimited_py-0.0.1a5/setup.cfg
```

### Comparing `athletes_unlimited_py-0.0.1a4/LICENSE` & `athletes_unlimited_py-0.0.1a5/LICENSE`

 * *Files identical despite different names*

### Comparing `athletes_unlimited_py-0.0.1a4/PKG-INFO` & `athletes_unlimited_py-0.0.1a5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: athletes_unlimited_py
-Version: 0.0.1a4
+Version: 0.0.1a5
 Summary: Python package for the Athletes Unlimited sports organization, and for the various sports it hosts.
 Author-email: Joseph Armstrong <armstrongjoseph08@gmail.com>
 Maintainer-email: Joseph Armstrong <armstrongjoseph08@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/armstjc/athletes-unlimited-py
 Project-URL: documentation, https://github.com/armstjc/athletes-unlimited-py/wiki
 Project-URL: repository, https://github.com/armstjc/athletes-unlimited-py.git
-Project-URL: changelog, https://github.com/armstjc/athletes-unlimited-py/CHANGELOG.md
+Project-URL: changelog, https://github.com/armstjc/athletes-unlimited-py/blob/main/CHANGELOG.md
 Keywords: sports,women_in_sports,women,girl_sports,basketball,womens_basketball,volleyball,womens_volleyball,lacrosse,womens_lacrosse,softball,womens_softball,aux_softball,womens_aux_softball
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # athletes-unlimited-py
 
 Python package for the Athletes Unlimited sports organization, and for the various sports it hosts.
 
 ## How to install
 
-`xflFastR-py` can be installed from this GitHub repository with the following command through pip:
+`athletes-unlimited-py` can be installed from this GitHub repository with the following command through pip:
 
 ```
 pip install git+https://github.com/armstjc/athletes-unlimited-py
 ```
```

### Comparing `athletes_unlimited_py-0.0.1a4/athetes_unlimited_py/aux_softball.py` & `athletes_unlimited_py-0.0.1a5/athetes_unlimited_py/aux_softball.py`

 * *Files identical despite different names*

### Comparing `athletes_unlimited_py-0.0.1a4/athetes_unlimited_py/basketball.py` & `athletes_unlimited_py-0.0.1a5/athetes_unlimited_py/basketball.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,14 +120,15 @@
     
     json_data = json.loads(response.text)
     time.sleep(0.5)
 
     sport = json_data['metaSport']['sport']
     api_version = json_data['metaSport']['version']
 
+    print(f'\nOn game #{game_num} in the {season} AU Basketball season.')
     for i in tqdm(json_data['data']):
         #print(i)
         row_df = pd.DataFrame({'sport':sport,'api_version':api_version},index=[0])
         row_df['type'] = i['type']
         row_df['teamId'] = i['teamId']
 
         if i['homeTeamFlg'] == True:
@@ -449,28 +450,28 @@
     seasonId = get_au_basketball_season_id(season)
     url = "https://auprosports.com/proxy.php?request=api/seasons/basketball/v1"
     headers = {"User-Agent":"Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.97 Safari/537.36"}
 
     response = requests.get(url,headers=headers)
     sport_json_data = json.loads(response.text)
     
-    for i in tqdm(sport_json_data['data']):
+    for i in sport_json_data['data']:
         #print(i)
         if i['seasonId'] == seasonId:
             len_game_ids = len(i['gameIds'])
 
-            for j in len_game_ids:
-                print(f'\nOn game {j} of {len_game_ids+1} for {season}.')
+            for j in tqdm(range(1,len_game_ids+1)):
+                # print(f'\nOn game ID {j} for the {season}.')
                 # try:
                 #     game_df = get_basketball_game_stats(season,j)
                 # except:
                 #     print(f'Couldn\'t parse game stats for game #{j}.')
                 #     time.sleep(10)
 
-                game_df = get_au_basketball_pbp(season,j)
+                game_df = get_au_basketball_game_stats(season,j)
 
                 season_stats_df = pd.concat([season_stats_df,game_df],ignore_index=True)
                 del game_df
 
     return season_stats_df
 
 def get_au_basketball_season_team_box(season:int) -> pd.DataFrame():
@@ -498,15 +499,15 @@
     
     for i in tqdm(sport_json_data['data']):
         #print(i)
         if i['seasonId'] == seasonId:
             len_game_ids = len(i['gameIds'])
 
             for j in tqdm(range(1,len_game_ids+1)):
-                print(f'\nOn game {j} of {len_game_ids+1} for {season}.')
+                # print(f'\nOn game {j} of {len_game_ids+1} for {season}.')
                 # try:
                 #     game_df = get_basketball_game_stats(season,j)
                 # except:
                 #     print(f'Couldn\'t parse game stats for game #{j}.')
                 #     time.sleep(10)
 
                 game_df = get_au_basketball_game_stats(season,j,get_team_stats=True)
```

### Comparing `athletes_unlimited_py-0.0.1a4/athetes_unlimited_py/lacrosse.py` & `athletes_unlimited_py-0.0.1a5/athetes_unlimited_py/lacrosse.py`

 * *Files identical despite different names*

### Comparing `athletes_unlimited_py-0.0.1a4/athetes_unlimited_py/softball.py` & `athletes_unlimited_py-0.0.1a5/athetes_unlimited_py/softball.py`

 * *Files identical despite different names*

### Comparing `athletes_unlimited_py-0.0.1a4/athetes_unlimited_py/utils.py` & `athletes_unlimited_py-0.0.1a5/athetes_unlimited_py/utils.py`

 * *Files identical despite different names*

### Comparing `athletes_unlimited_py-0.0.1a4/athletes_unlimited_py.egg-info/PKG-INFO` & `athletes_unlimited_py-0.0.1a5/athletes_unlimited_py.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: athletes-unlimited-py
-Version: 0.0.1a4
+Version: 0.0.1a5
 Summary: Python package for the Athletes Unlimited sports organization, and for the various sports it hosts.
 Author-email: Joseph Armstrong <armstrongjoseph08@gmail.com>
 Maintainer-email: Joseph Armstrong <armstrongjoseph08@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/armstjc/athletes-unlimited-py
 Project-URL: documentation, https://github.com/armstjc/athletes-unlimited-py/wiki
 Project-URL: repository, https://github.com/armstjc/athletes-unlimited-py.git
-Project-URL: changelog, https://github.com/armstjc/athletes-unlimited-py/CHANGELOG.md
+Project-URL: changelog, https://github.com/armstjc/athletes-unlimited-py/blob/main/CHANGELOG.md
 Keywords: sports,women_in_sports,women,girl_sports,basketball,womens_basketball,volleyball,womens_volleyball,lacrosse,womens_lacrosse,softball,womens_softball,aux_softball,womens_aux_softball
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # athletes-unlimited-py
 
 Python package for the Athletes Unlimited sports organization, and for the various sports it hosts.
 
 ## How to install
 
-`xflFastR-py` can be installed from this GitHub repository with the following command through pip:
+`athletes-unlimited-py` can be installed from this GitHub repository with the following command through pip:
 
 ```
 pip install git+https://github.com/armstjc/athletes-unlimited-py
 ```
```

### Comparing `athletes_unlimited_py-0.0.1a4/pyproject.toml` & `athletes_unlimited_py-0.0.1a5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools","wheel","pyarrow","pandas","tqdm","requests","lxml"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "athletes_unlimited_py"
-version = "0.0.1a4"
+version = "0.0.1a5"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "MIT"}
 
 authors = [
     {name = "Joseph Armstrong", email="armstrongjoseph08@gmail.com"}
 ]
@@ -37,8 +37,8 @@
     "lxml"
 ]
 
 [project.urls]
 homepage = "https://github.com/armstjc/athletes-unlimited-py"
 documentation = "https://github.com/armstjc/athletes-unlimited-py/wiki"
 repository = "https://github.com/armstjc/athletes-unlimited-py.git"
-changelog = "https://github.com/armstjc/athletes-unlimited-py/CHANGELOG.md"
+changelog = "https://github.com/armstjc/athletes-unlimited-py/blob/main/CHANGELOG.md"
```

