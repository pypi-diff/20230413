# Comparing `tmp/letterboxd_stats-0.1.4.tar.gz` & `tmp/letterboxd_stats-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "letterboxd_stats-0.1.4.tar", last modified: Sun Apr  9 23:05:01 2023, max compression
+gzip compressed data, was "letterboxd_stats-0.1.6.tar", last modified: Thu Apr 13 18:50:42 2023, max compression
```

## Comparing `letterboxd_stats-0.1.4.tar` & `letterboxd_stats-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-04-09 23:05:01.440173 letterboxd_stats-0.1.4/
--rw-rw-r--   0 marco     (1001) marco     (1001)     1089 2023-03-06 16:16:14.000000 letterboxd_stats-0.1.4/LICENCE
--rw-rw-r--   0 marco     (1001) marco     (1001)     2697 2023-04-09 23:05:01.440173 letterboxd_stats-0.1.4/PKG-INFO
--rw-rw-r--   0 marco     (1001) marco     (1001)     2203 2023-03-08 15:15:35.000000 letterboxd_stats-0.1.4/README.md
-drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-04-09 23:05:01.440173 letterboxd_stats-0.1.4/letterboxd_stats/
--rw-rw-r--   0 marco     (1001) marco     (1001)     1563 2023-04-09 22:57:57.000000 letterboxd_stats-0.1.4/letterboxd_stats/__init__.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     5216 2023-04-09 22:57:57.000000 letterboxd_stats-0.1.4/letterboxd_stats/cli.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     3494 2023-04-09 23:04:29.000000 letterboxd_stats-0.1.4/letterboxd_stats/data.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     3175 2023-04-09 22:57:57.000000 letterboxd_stats-0.1.4/letterboxd_stats/main.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     2574 2023-04-08 16:03:39.000000 letterboxd_stats-0.1.4/letterboxd_stats/tmdb.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     4697 2023-03-15 22:58:55.000000 letterboxd_stats-0.1.4/letterboxd_stats/web_scraper.py
-drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-04-09 23:05:01.440173 letterboxd_stats-0.1.4/letterboxd_stats.egg-info/
--rw-rw-r--   0 marco     (1001) marco     (1001)     2697 2023-04-09 23:05:01.000000 letterboxd_stats-0.1.4/letterboxd_stats.egg-info/PKG-INFO
--rw-rw-r--   0 marco     (1001) marco     (1001)      434 2023-04-09 23:05:01.000000 letterboxd_stats-0.1.4/letterboxd_stats.egg-info/SOURCES.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)        1 2023-04-09 23:05:01.000000 letterboxd_stats-0.1.4/letterboxd_stats.egg-info/dependency_links.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)       64 2023-04-09 23:05:01.000000 letterboxd_stats-0.1.4/letterboxd_stats.egg-info/entry_points.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)      126 2023-04-09 23:05:01.000000 letterboxd_stats-0.1.4/letterboxd_stats.egg-info/requires.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)       17 2023-04-09 23:05:01.000000 letterboxd_stats-0.1.4/letterboxd_stats.egg-info/top_level.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)      841 2023-04-09 22:58:10.000000 letterboxd_stats-0.1.4/pyproject.toml
--rw-rw-r--   0 marco     (1001) marco     (1001)       38 2023-04-09 23:05:01.440173 letterboxd_stats-0.1.4/setup.cfg
+drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-04-13 18:50:42.603487 letterboxd_stats-0.1.6/
+-rw-rw-r--   0 marco     (1001) marco     (1001)     1089 2023-03-06 16:16:14.000000 letterboxd_stats-0.1.6/LICENCE
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2963 2023-04-13 18:50:42.603487 letterboxd_stats-0.1.6/PKG-INFO
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2445 2023-04-13 13:31:47.000000 letterboxd_stats-0.1.6/README.md
+drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-04-13 18:50:42.603487 letterboxd_stats-0.1.6/letterboxd_stats/
+-rw-rw-r--   0 marco     (1001) marco     (1001)     1447 2023-04-13 13:31:47.000000 letterboxd_stats-0.1.6/letterboxd_stats/__init__.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     5230 2023-04-13 13:31:47.000000 letterboxd_stats-0.1.6/letterboxd_stats/cli.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     3878 2023-04-13 13:31:47.000000 letterboxd_stats-0.1.6/letterboxd_stats/data.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     3223 2023-04-13 13:31:47.000000 letterboxd_stats-0.1.6/letterboxd_stats/main.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2923 2023-04-13 18:48:10.000000 letterboxd_stats-0.1.6/letterboxd_stats/tmdb.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     4697 2023-03-15 22:58:55.000000 letterboxd_stats-0.1.6/letterboxd_stats/web_scraper.py
+drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-04-13 18:50:42.603487 letterboxd_stats-0.1.6/letterboxd_stats.egg-info/
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2963 2023-04-13 18:50:42.000000 letterboxd_stats-0.1.6/letterboxd_stats.egg-info/PKG-INFO
+-rw-rw-r--   0 marco     (1001) marco     (1001)      434 2023-04-13 18:50:42.000000 letterboxd_stats-0.1.6/letterboxd_stats.egg-info/SOURCES.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)        1 2023-04-13 18:50:42.000000 letterboxd_stats-0.1.6/letterboxd_stats.egg-info/dependency_links.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)       64 2023-04-13 18:50:42.000000 letterboxd_stats-0.1.6/letterboxd_stats.egg-info/entry_points.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)      126 2023-04-13 18:50:42.000000 letterboxd_stats-0.1.6/letterboxd_stats.egg-info/requires.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)       17 2023-04-13 18:50:42.000000 letterboxd_stats-0.1.6/letterboxd_stats.egg-info/top_level.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)      865 2023-04-13 18:48:10.000000 letterboxd_stats-0.1.6/pyproject.toml
+-rw-rw-r--   0 marco     (1001) marco     (1001)       38 2023-04-13 18:50:42.603487 letterboxd_stats-0.1.6/setup.cfg
```

### Comparing `letterboxd_stats-0.1.4/LICENCE` & `letterboxd_stats-0.1.6/LICENCE`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.1.4/PKG-INFO` & `letterboxd_stats-0.1.6/letterboxd_stats.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: letterboxd_stats
-Version: 0.1.4
-Summary: A small example package
+Name: letterboxd-stats
+Version: 0.1.6
+Summary: Get information about your Letterboxd activity.
 Author: mBaratta96
 Project-URL: Homepage, https://github.com/mBaratta96/letterboxd_stats
 Project-URL: Bug Tracker, https://github.com/mBaratta96/letterboxd_stats/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -18,59 +18,74 @@
 
 Get information about your Letterboxd activity.
 
 Search for actors/directors, analyze your diary/watchlist/rating, check which film you have seen for a particular person. All in your terminal.
 
 ## Requirements
 
-- Python >= 3.8
-- A [TMDb API key](https://www.themoviedb.org/documentation/api): to retrieve all the general information for movies/people
-- A Letterboxd account: to export your Letterboxd activity through web-scraping.
+-   Python >= 3.8
+-   A [TMDb API key](https://www.themoviedb.org/documentation/api): to retrieve all the general information for movies/people
+-   A Letterboxd account: to export your Letterboxd activity through web-scraping.
 
 ## Installation
+
 Just run:
+
 ```shell
 pip3 install letterboxd_stats
 ```
 
 ## Configuration
+
 It is required to create a `config.toml`. You can create it in the default config folder (for example, `.config/letterboxd_stats` in Linux) or specify your custom folder with the `-c` command. For each platform, default config folder follows the structure of the [platformdirs](https://github.com/platformdirs/platformdirs) package.
 
 ```toml
 # Where you want the .csv file of your Letterboxd activity to be saved.
 root_folder = "~/Documents/letterboxd_stats/"
 
-# The size of the ASCII art poster printed in your terminal when you check the details of a movie. Set to 0 to disable 
+[CLI]
+# The size of the ASCII art poster printed in your terminal when you check the details of a movie.
+# Set to 0 to disable
 poster_columns = 180
+# Set ascending order for sorting of tables
+ascending = false
 
 [TMDB]
-api_key = "your-TMDb-API-KEY"
+api_key = "YOUR_TMDB_API_KEY"
+# When you get your lists (-L options), also get all the runtimes from TMDB
+# and compute the mean of the ratings weigthed on the durations. This slows the process.
+get_list_runtimes = false
+
 
 [Letterboxd]
 username = "your-username"
 password = "your-password"
 ```
 
 ## Options
+
 ```shell
 options:
   -h, --help            show this help message and exit
   -s SEARCH, --search SEARCH
                         Search for a director
   -S SEARCH_FILM, --search-film SEARCH_FILM
                         Search for a film.
   -d, --download        Download letterboxd data from your account
   -W, --wishlist        show wishlist
   -D, --diary           show diary
   -R, --ratings         show ratings
+  -L, --lists           show lists
   -l LIMIT, --limit LIMIT
                         limit the number of items of your wishlist/diary
-  -a, --ascending       Use ascending order when you sort the entries
   -c CONFIG_FOLDER, --config_folder CONFIG_FOLDER
                         Specifiy the folder of your config.toml file
+
 ```
+
 ## To do
+
 _Note: this is something I do during my free time. Therefore, I can't promise consistent support for this project._
 
-- [x] Use web-scraping to add film to diary/wishlist
+-   [x] Use web-scraping to add film to diary/wishlist
 
-- [ ] Check followers' activity. 
+-   [ ] Check followers' activity.
```

### Comparing `letterboxd_stats-0.1.4/README.md` & `letterboxd_stats-0.1.6/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -4,59 +4,74 @@
 
 Get information about your Letterboxd activity.
 
 Search for actors/directors, analyze your diary/watchlist/rating, check which film you have seen for a particular person. All in your terminal.
 
 ## Requirements
 
-- Python >= 3.8
-- A [TMDb API key](https://www.themoviedb.org/documentation/api): to retrieve all the general information for movies/people
-- A Letterboxd account: to export your Letterboxd activity through web-scraping.
+-   Python >= 3.8
+-   A [TMDb API key](https://www.themoviedb.org/documentation/api): to retrieve all the general information for movies/people
+-   A Letterboxd account: to export your Letterboxd activity through web-scraping.
 
 ## Installation
+
 Just run:
+
 ```shell
 pip3 install letterboxd_stats
 ```
 
 ## Configuration
+
 It is required to create a `config.toml`. You can create it in the default config folder (for example, `.config/letterboxd_stats` in Linux) or specify your custom folder with the `-c` command. For each platform, default config folder follows the structure of the [platformdirs](https://github.com/platformdirs/platformdirs) package.
 
 ```toml
 # Where you want the .csv file of your Letterboxd activity to be saved.
 root_folder = "~/Documents/letterboxd_stats/"
 
-# The size of the ASCII art poster printed in your terminal when you check the details of a movie. Set to 0 to disable 
+[CLI]
+# The size of the ASCII art poster printed in your terminal when you check the details of a movie.
+# Set to 0 to disable
 poster_columns = 180
+# Set ascending order for sorting of tables
+ascending = false
 
 [TMDB]
-api_key = "your-TMDb-API-KEY"
+api_key = "YOUR_TMDB_API_KEY"
+# When you get your lists (-L options), also get all the runtimes from TMDB
+# and compute the mean of the ratings weigthed on the durations. This slows the process.
+get_list_runtimes = false
+
 
 [Letterboxd]
 username = "your-username"
 password = "your-password"
 ```
 
 ## Options
+
 ```shell
 options:
   -h, --help            show this help message and exit
   -s SEARCH, --search SEARCH
                         Search for a director
   -S SEARCH_FILM, --search-film SEARCH_FILM
                         Search for a film.
   -d, --download        Download letterboxd data from your account
   -W, --wishlist        show wishlist
   -D, --diary           show diary
   -R, --ratings         show ratings
+  -L, --lists           show lists
   -l LIMIT, --limit LIMIT
                         limit the number of items of your wishlist/diary
-  -a, --ascending       Use ascending order when you sort the entries
   -c CONFIG_FOLDER, --config_folder CONFIG_FOLDER
                         Specifiy the folder of your config.toml file
+
 ```
+
 ## To do
+
 _Note: this is something I do during my free time. Therefore, I can't promise consistent support for this project._
 
-- [x] Use web-scraping to add film to diary/wishlist
+-   [x] Use web-scraping to add film to diary/wishlist
 
-- [ ] Check followers' activity. 
+-   [ ] Check followers' activity.
```

### Comparing `letterboxd_stats-0.1.4/letterboxd_stats/__init__.py` & `letterboxd_stats-0.1.6/letterboxd_stats/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     action="store_true",
 )
 parser.add_argument("-W", "--wishlist", help="show wishlist", action="store_true")
 parser.add_argument("-D", "--diary", help="show diary", action="store_true")
 parser.add_argument("-R", "--ratings", help="show ratings", action="store_true")
 parser.add_argument("-L", "--lists", help="show lists", action="store_true")
 parser.add_argument("-l", "--limit", help="limit the number of items of your wishlist/diary", type=int)
-parser.add_argument("-a", "--ascending", help="Use ascending order when you sort the entries", action="store_true")
 parser.add_argument("-c", "--config_folder", help="Specifiy the folder of your config.toml file")
 
 
 args = parser.parse_args()
 
 folder = args.config_folder or default_folder
 path = os.path.abspath(os.path.join(folder, "config.toml"))
```

### Comparing `letterboxd_stats-0.1.4/letterboxd_stats/cli.py` & `letterboxd_stats-0.1.6/letterboxd_stats/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 
 def select_movie_id(movies_info: pd.DataFrame) -> int:
     movie_id = inquirer.fuzzy(  # type: ignore
         message="Write movie id for more information",
         mandatory=False,
         max_height="25%",
         choices=[
-            Choice(value=id, name=f"{id} - {title}") for id, title in zip(movies_info["id"], movies_info["title"])
+            Choice(value=id, name=f"{id} - {title}") for id, title in zip(movies_info["Id"], movies_info["Title"])
         ],
         keybindings={"skip": [{"key": "escape"}]},
-        validate=lambda result: result in movies_info["id"].values,
+        validate=lambda result: result in movies_info["Id"].values,
         filter=lambda result: None if result is None else int(result),
         invalid_message="Input must be in the resulting IDs",
     ).execute()
     return movie_id
 
 
 def select_search_result(results: list[str]) -> int:
@@ -87,17 +87,17 @@
     for _, row in df_str.iterrows():
         table.add_row(*row)
     console = Console()
     console.print(table)
 
 
 def download_poster(poster: str):
-    if config["poster_columns"] > 0:
+    if config["CLI"]["poster_columns"] > 0:
         art = AsciiArt.from_url(IMAGE_URL + poster)
-        art.to_terminal(columns=int(config["poster_columns"]))
+        art.to_terminal(columns=int(config["CLI"]["poster_columns"]))
 
 
 def _validate_date(s: str):
     try:
         datetime.strptime(s, "%Y-%m-%d")
     except ValueError:
         return False
```

### Comparing `letterboxd_stats-0.1.4/letterboxd_stats/data.py` & `letterboxd_stats-0.1.6/letterboxd_stats/data.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import pandas as pd
 import numpy as np
 from letterboxd_stats import cli
+from letterboxd_stats import tmdb
 import os
 from letterboxd_stats import config
 
 
 def read_watched_films(df: pd.DataFrame, path: str, name: str):
     df_profile = pd.read_csv(path)
-    df.insert(0, "watched", np.where(df["title"].isin(df_profile["Name"]), "[X]", "[ ]"))
-    df["release_date"] = pd.to_datetime(df["release_date"])
-    df.sort_values(by="release_date", inplace=True)
+    df.insert(0, "watched", np.where(df["Title"].isin(df_profile["Name"]), "[X]", "[ ]"))
+    df["Release Date"] = pd.to_datetime(df["Release Date"])
+    df.sort_values(by="Release Date", inplace=True)
     cli.render_table(df, name)
-    movie_id = cli.select_movie_id(df[["id", "title"]])
+    movie_id = cli.select_movie_id(df[["Id", "Title"]])
     return movie_id
 
 
 def get_list_name(path: str):
     df = pd.read_csv(path, header=1)
     return df["Name"].iloc[0]
 
@@ -42,17 +43,23 @@
 def _show_lists(df: pd.DataFrame, ascending: bool):
     ratings_path = os.path.expanduser(os.path.join(config["root_folder"], "static", "ratings.csv"))
     df_ratings = pd.read_csv(ratings_path)
     df_ratings.rename(columns={"Letterboxd URI": "URL"}, inplace=True)
     df = df.merge(df_ratings[["URL", "Rating"]], on="URL", how="inner")
     df.rename(columns={"URL": "Url"}, inplace=True)
     df = df.drop("Description", axis=1)
+    df["Rating"] = df["Rating"].astype(float)
     sort_column = cli.select_value(df.columns.values.tolist(), "Select the order of your diary entries:")
     df.sort_values(by=sort_column, ascending=ascending, inplace=True)
-    avg = {"Rating Mean": "{:.2f}".format(df["Rating"].astype(float).mean())}
+    avg = {"Rating Mean": "{:.2f}".format(df["Rating"].mean())}
+    if config["TMDB"]["get_list_runtimes"] is True:
+        df["Duration"] = df.apply(lambda row: tmdb.get_film_duration(row["Title"], row["Year"]), axis=1)  # type: ignore
+        avg["Time-weighted Rating Mean"] = "{:.2f}".format(
+            ((df["Duration"] / df["Duration"].sum()) * df["Rating"]).sum()
+        )
     cli.print_film(avg, expand=False)
     return df
 
 
 def _show_watchlist(df: pd.DataFrame, ascending: bool):
     sort_column = cli.select_value(
         df.columns.values.tolist() + ["Shuffle"], "Select the order of your watchlist entries:"
```

### Comparing `letterboxd_stats-0.1.4/letterboxd_stats/main.py` & `letterboxd_stats-0.1.6/letterboxd_stats/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -82,18 +82,18 @@
     if args.download:
         try_command(download_data, ())
     if args.search:
         try_command(search_person, (args.search,))
     if args.search_film:
         try_command(search_film, (args.search_film,))
     if args.wishlist:
-        try_command(get_wishlist, (args.limit, args.ascending))
+        try_command(get_wishlist, (args.limit, config["CLI"]["ascending"]))
     if args.diary:
-        try_command(get_diary, (args.limit, args.ascending))
+        try_command(get_diary, (args.limit, config["CLI"]["ascending"]))
     if args.ratings:
-        try_command(get_ratings, (args.limit, args.ascending))
+        try_command(get_ratings, (args.limit, config["CLI"]["ascending"]))
     if args.lists:
-        try_command(get_lists, (args.limit, args.ascending))
+        try_command(get_lists, (args.limit, config["CLI"]["ascending"]))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `letterboxd_stats-0.1.4/letterboxd_stats/tmdb.py` & `letterboxd_stats-0.1.6/letterboxd_stats/tmdb.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,55 @@
-from tmdbv3api import TMDb, Person, Movie
+from tmdbv3api import TMDb, Person, Movie, Search
 import pandas as pd
 from letterboxd_stats import cli
 from letterboxd_stats import config
 from letterboxd_stats import web_scraper
 
 tmdb = TMDb()
 tmdb.api_key = config["TMDB"]["api_key"]
 person = Person()
 movie = Movie()
+search = Search()
 
 
 def get_person(name: str):
     print(f"Searching for '{name}'")
-    search_results = person.search(name)
+    search_results = search.people({"query": name})
     names = [result.name for result in search_results]  # type: ignore
     if len(names) == 0:
         raise Exception("No results for your search")
     result_index = cli.select_search_result(names)  # type: ignore
     search_result = search_results[result_index]
     p = person.details(search_result["id"])
     known_for_department = p["known_for_department"]
     movie_credits = person.movie_credits(search_result["id"])
     list_of_films = [
         {
-            "title": m.title,
-            "release_date": m.release_date,
-            "department": m.department,
-            "id": m.id,
-            "duration": movie.details(m.id).runtime,  # type: ignore
+            "Title": m.title,
+            "Release Date": m.release_date,
+            "Department": m.department,
+            "Id": m.id,
         }
         for m in movie_credits["crew"]
     ]
     if len(list_of_films) == 0:
         raise ValueError("The selected person doesn't have any film.")
     df = pd.DataFrame(list_of_films)
     department = cli.select_value(
-        df["department"].unique(), f"Select a department for {p['name']}", known_for_department
+        df["Department"].unique(), f"Select a department for {p['name']}", known_for_department
     )
-    df = df[df["department"] == department]
-    df = df.drop("department", axis=1)
+    df = df[df["Department"] == department]
+    df = df.drop("Department", axis=1)
+    df["Duration"] = df.apply(lambda row: movie.details(row["Id"]).runtime, axis=1)  # type: ignore
     return df, p["name"]
 
 
 def get_movie(movie_query: str):
     print(f"Searching for movie '{movie_query}'")
-    search_results = movie.search(movie_query)
+    search_results = search.movies({"query": movie_query})
     titles = [f"{result.title} ({result.release_date})" for result in search_results]  # type: ignore
     if len(titles) == 0:
         raise Exception("No results for your search")
     result_index = cli.select_search_result(titles)  # type: ignore
     movie_id = search_results[result_index]["id"]
     get_movie_detail(movie_id)
     return search_results[result_index]
@@ -64,7 +65,15 @@
         "Original Title": movie_details["original_title"],
         "Runtime": movie_details["runtime"],
         "Overview": movie_details["overview"],
         "Release Date": movie_details["release_date"],
         "Letterboxd URL": web_scraper.create_movie_url(movie_details["title"], "film_page"),
     }
     cli.print_film(selected_details)
+
+
+def get_film_duration(film: str, year: int):
+    search_results = search.movies({"query": film, "year": year})
+    if len(search_results) > 0:
+        first_result = search_results[0]
+        return movie.details(first_result.id).runtime  # type: ignore
+    return 0
```

### Comparing `letterboxd_stats-0.1.4/letterboxd_stats/web_scraper.py` & `letterboxd_stats-0.1.6/letterboxd_stats/web_scraper.py`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.1.4/letterboxd_stats.egg-info/PKG-INFO` & `letterboxd_stats-0.1.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: letterboxd-stats
-Version: 0.1.4
-Summary: A small example package
+Name: letterboxd_stats
+Version: 0.1.6
+Summary: Get information about your Letterboxd activity.
 Author: mBaratta96
 Project-URL: Homepage, https://github.com/mBaratta96/letterboxd_stats
 Project-URL: Bug Tracker, https://github.com/mBaratta96/letterboxd_stats/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -18,59 +18,74 @@
 
 Get information about your Letterboxd activity.
 
 Search for actors/directors, analyze your diary/watchlist/rating, check which film you have seen for a particular person. All in your terminal.
 
 ## Requirements
 
-- Python >= 3.8
-- A [TMDb API key](https://www.themoviedb.org/documentation/api): to retrieve all the general information for movies/people
-- A Letterboxd account: to export your Letterboxd activity through web-scraping.
+-   Python >= 3.8
+-   A [TMDb API key](https://www.themoviedb.org/documentation/api): to retrieve all the general information for movies/people
+-   A Letterboxd account: to export your Letterboxd activity through web-scraping.
 
 ## Installation
+
 Just run:
+
 ```shell
 pip3 install letterboxd_stats
 ```
 
 ## Configuration
+
 It is required to create a `config.toml`. You can create it in the default config folder (for example, `.config/letterboxd_stats` in Linux) or specify your custom folder with the `-c` command. For each platform, default config folder follows the structure of the [platformdirs](https://github.com/platformdirs/platformdirs) package.
 
 ```toml
 # Where you want the .csv file of your Letterboxd activity to be saved.
 root_folder = "~/Documents/letterboxd_stats/"
 
-# The size of the ASCII art poster printed in your terminal when you check the details of a movie. Set to 0 to disable 
+[CLI]
+# The size of the ASCII art poster printed in your terminal when you check the details of a movie.
+# Set to 0 to disable
 poster_columns = 180
+# Set ascending order for sorting of tables
+ascending = false
 
 [TMDB]
-api_key = "your-TMDb-API-KEY"
+api_key = "YOUR_TMDB_API_KEY"
+# When you get your lists (-L options), also get all the runtimes from TMDB
+# and compute the mean of the ratings weigthed on the durations. This slows the process.
+get_list_runtimes = false
+
 
 [Letterboxd]
 username = "your-username"
 password = "your-password"
 ```
 
 ## Options
+
 ```shell
 options:
   -h, --help            show this help message and exit
   -s SEARCH, --search SEARCH
                         Search for a director
   -S SEARCH_FILM, --search-film SEARCH_FILM
                         Search for a film.
   -d, --download        Download letterboxd data from your account
   -W, --wishlist        show wishlist
   -D, --diary           show diary
   -R, --ratings         show ratings
+  -L, --lists           show lists
   -l LIMIT, --limit LIMIT
                         limit the number of items of your wishlist/diary
-  -a, --ascending       Use ascending order when you sort the entries
   -c CONFIG_FOLDER, --config_folder CONFIG_FOLDER
                         Specifiy the folder of your config.toml file
+
 ```
+
 ## To do
+
 _Note: this is something I do during my free time. Therefore, I can't promise consistent support for this project._
 
-- [x] Use web-scraping to add film to diary/wishlist
+-   [x] Use web-scraping to add film to diary/wishlist
 
-- [ ] Check followers' activity. 
+-   [ ] Check followers' activity.
```

### Comparing `letterboxd_stats-0.1.4/pyproject.toml` & `letterboxd_stats-0.1.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "letterboxd_stats"
-version = "0.1.4"
+version = "0.1.6"
 authors = [{ name = "mBaratta96" }]
-description = "A small example package"
+description = "Get information about your Letterboxd activity."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
```

