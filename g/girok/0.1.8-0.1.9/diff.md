# Comparing `tmp/girok-0.1.8.tar.gz` & `tmp/girok-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girok-0.1.8.tar", max compression
+gzip compressed data, was "girok-0.1.9.tar", max compression
```

## Comparing `girok-0.1.8.tar` & `girok-0.1.9.tar`

### file list

```diff
@@ -1,62 +1,28 @@
--rw-r--r--   0        0        0    19660 2023-03-24 10:46:23.245587 girok-0.1.8/README.md
--rw-r--r--   0        0        0       21 2023-03-25 04:50:09.359758 girok-0.1.8/girok/__init__.py
--rw-r--r--   0        0        0     1299 2023-03-23 11:14:54.408006 girok-0.1.8/girok/api/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0        0        0     1576 2023-03-25 04:47:10.401263 girok-0.1.8/girok/api/__pycache__/auth.cpython-39.pyc
--rw-r--r--   0        0        0     6490 2023-03-23 11:15:21.478267 girok-0.1.8/girok/api/__pycache__/category.cpython-311.pyc
--rw-r--r--   0        0        0     3285 2023-03-23 16:38:04.525128 girok-0.1.8/girok/api/__pycache__/category.cpython-39.pyc
--rw-r--r--   0        0        0     7322 2023-03-23 11:15:29.019365 girok-0.1.8/girok/api/__pycache__/task.cpython-311.pyc
--rw-r--r--   0        0        0     3688 2023-03-23 16:53:05.800346 girok-0.1.8/girok/api/__pycache__/task.cpython-39.pyc
--rw-r--r--   0        0        0     1488 2023-03-25 04:45:53.521561 girok-0.1.8/girok/api/auth.py
--rw-r--r--   0        0        0     3897 2023-03-23 15:35:25.657591 girok-0.1.8/girok/api/category.py
--rw-r--r--   0        0        0     4724 2023-03-23 16:52:47.999407 girok-0.1.8/girok/api/task.py
--rw-r--r--   0        0        0     3194 2023-03-23 11:15:29.336619 girok-0.1.8/girok/calendar_cli/__pycache__/calendar_app.cpython-311.pyc
--rw-r--r--   0        0        0     2191 2023-03-23 16:38:04.770333 girok-0.1.8/girok/calendar_cli/__pycache__/calendar_app.cpython-39.pyc
--rw-r--r--   0        0        0    23281 2023-03-23 11:15:29.343464 girok-0.1.8/girok/calendar_cli/__pycache__/calendar_container.cpython-311.pyc
--rw-r--r--   0        0        0    11915 2023-03-23 16:38:04.777924 girok-0.1.8/girok/calendar_cli/__pycache__/calendar_container.cpython-39.pyc
--rw-r--r--   0        0        0    11309 2023-03-23 11:15:29.030884 girok-0.1.8/girok/calendar_cli/__pycache__/calendar_main.cpython-311.pyc
--rw-r--r--   0        0        0     6292 2023-03-23 17:09:56.681117 girok-0.1.8/girok/calendar_cli/__pycache__/calendar_main.cpython-39.pyc
--rw-r--r--   0        0        0    12652 2023-03-23 11:15:29.338919 girok-0.1.8/girok/calendar_cli/__pycache__/sidebar.cpython-311.pyc
--rw-r--r--   0        0        0     7286 2023-03-23 16:38:04.772980 girok-0.1.8/girok/calendar_cli/__pycache__/sidebar.cpython-39.pyc
--rw-r--r--   0        0        0     1380 2023-03-23 15:35:25.659015 girok-0.1.8/girok/calendar_cli/calendar_app.py
--rw-r--r--   0        0        0    13001 2023-03-23 15:35:25.659679 girok-0.1.8/girok/calendar_cli/calendar_container.py
--rw-r--r--   0        0        0     3863 2023-03-23 15:35:25.660897 girok-0.1.8/girok/calendar_cli/calendar_main.css
--rw-r--r--   0        0        0     6998 2023-03-23 17:09:49.622419 girok-0.1.8/girok/calendar_cli/calendar_main.py
--rw-r--r--   0        0        0     6711 2023-03-23 15:35:25.662125 girok-0.1.8/girok/calendar_cli/sidebar.py
--rw-r--r--   0        0        0    76495 2023-03-23 15:35:25.662963 girok-0.1.8/girok/calendar_cli/textual_demo_2023-03-11T22_49_21_681307.svg
--rw-r--r--   0        0        0     5014 2023-03-23 11:15:21.471623 girok-0.1.8/girok/commands/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0        0        0     3193 2023-03-25 04:47:10.543347 girok-0.1.8/girok/commands/__pycache__/auth.cpython-39.pyc
--rw-r--r--   0        0        0      729 2023-03-23 11:15:29.028683 girok-0.1.8/girok/commands/__pycache__/calendar.cpython-311.pyc
--rw-r--r--   0        0        0      604 2023-03-23 18:32:52.543566 girok-0.1.8/girok/commands/__pycache__/calendar.cpython-39.pyc
--rw-r--r--   0        0        0     8108 2023-03-23 11:15:21.475376 girok-0.1.8/girok/commands/__pycache__/category.cpython-311.pyc
--rw-r--r--   0        0        0     4399 2023-03-23 18:32:52.518716 girok-0.1.8/girok/commands/__pycache__/category.cpython-39.pyc
--rw-r--r--   0        0        0    33150 2023-03-23 11:15:29.013835 girok-0.1.8/girok/commands/__pycache__/task.cpython-311.pyc
--rw-r--r--   0        0        0    18475 2023-03-23 19:29:05.340846 girok-0.1.8/girok/commands/__pycache__/task.cpython-39.pyc
--rw-r--r--   0        0        0     3899 2023-03-25 04:45:53.522714 girok-0.1.8/girok/commands/auth.py
--rw-r--r--   0        0        0      330 2023-03-23 18:32:48.364884 girok-0.1.8/girok/commands/calendar.py
--rw-r--r--   0        0        0     5264 2023-03-23 18:32:48.365585 girok-0.1.8/girok/commands/category.py
--rw-r--r--   0        0        0    28335 2023-03-23 19:28:42.711527 girok-0.1.8/girok/commands/task.py
--rw-r--r--   0        0        0      171 2023-03-25 04:45:53.523094 girok-0.1.8/girok/config.json
--rw-r--r--   0        0        0      678 2023-03-25 04:45:53.523417 girok-0.1.8/girok/config.py
--rw-r--r--   0        0        0     1408 2023-03-23 15:35:25.665989 girok-0.1.8/girok/constants.py
--rw-r--r--   0        0        0     1742 2023-03-23 18:32:48.369956 girok-0.1.8/girok/girok.py
--rw-r--r--   0        0        0      559 2023-03-23 15:37:19.810418 girok-0.1.8/girok/styles/stopwatch03.css
--rw-r--r--   0        0        0        0 2023-03-23 15:35:25.666933 girok-0.1.8/girok/utils/__init__.py
--rw-r--r--   0        0        0      166 2023-03-23 11:10:45.191502 girok-0.1.8/girok/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      148 2023-03-23 16:38:04.308022 girok-0.1.8/girok/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3062 2023-03-23 11:15:21.473115 girok-0.1.8/girok/utils/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0        0        0     1828 2023-03-25 04:47:10.545796 girok-0.1.8/girok/utils/__pycache__/auth.cpython-39.pyc
--rw-r--r--   0        0        0     7434 2023-03-23 11:15:21.488070 girok-0.1.8/girok/utils/__pycache__/calendar.cpython-311.pyc
--rw-r--r--   0        0        0     3975 2023-03-24 03:43:06.474990 girok-0.1.8/girok/utils/__pycache__/calendar.cpython-39.pyc
--rw-r--r--   0        0        0    14967 2023-03-23 11:15:28.997687 girok-0.1.8/girok/utils/__pycache__/display.cpython-311.pyc
--rw-r--r--   0        0        0     7029 2023-03-23 17:57:55.270944 girok-0.1.8/girok/utils/__pycache__/display.cpython-39.pyc
--rw-r--r--   0        0        0     3349 2023-03-23 11:14:54.402850 girok-0.1.8/girok/utils/__pycache__/general.cpython-311.pyc
--rw-r--r--   0        0        0     1845 2023-03-23 16:38:04.312092 girok-0.1.8/girok/utils/__pycache__/general.cpython-39.pyc
--rw-r--r--   0        0        0     8676 2023-03-23 11:15:21.486280 girok-0.1.8/girok/utils/__pycache__/task.cpython-311.pyc
--rw-r--r--   0        0        0     5373 2023-03-23 16:38:04.531908 girok-0.1.8/girok/utils/__pycache__/task.cpython-39.pyc
--rw-r--r--   0        0        0     1412 2023-03-25 04:45:53.523763 girok-0.1.8/girok/utils/auth.py
--rw-r--r--   0        0        0     4120 2023-03-24 03:43:01.283009 girok-0.1.8/girok/utils/calendar.py
--rw-r--r--   0        0        0    11059 2023-03-23 17:57:47.427476 girok-0.1.8/girok/utils/display.py
--rw-r--r--   0        0        0     1130 2023-03-23 15:35:25.668533 girok-0.1.8/girok/utils/general.py
--rw-r--r--   0        0        0     4906 2023-03-23 15:35:25.669005 girok-0.1.8/girok/utils/task.py
--rw-r--r--   0        0        0     1151 2023-03-25 04:50:41.669782 girok-0.1.8/pyproject.toml
--rw-r--r--   0        0        0    21614 1970-01-01 00:00:00.000000 girok-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    19660 2023-03-24 10:46:23.245587 girok-0.1.9/README.md
+-rw-r--r--   0        0        0       21 2023-03-25 07:35:21.531596 girok-0.1.9/girok/__init__.py
+-rw-r--r--   0        0        0     1488 2023-03-25 04:45:53.521561 girok-0.1.9/girok/api/auth.py
+-rw-r--r--   0        0        0     3897 2023-03-23 15:35:25.657591 girok-0.1.9/girok/api/category.py
+-rw-r--r--   0        0        0     4724 2023-03-23 16:52:47.999407 girok-0.1.9/girok/api/task.py
+-rw-r--r--   0        0        0     1380 2023-03-23 15:35:25.659015 girok-0.1.9/girok/calendar_cli/calendar_app.py
+-rw-r--r--   0        0        0    13001 2023-03-23 15:35:25.659679 girok-0.1.9/girok/calendar_cli/calendar_container.py
+-rw-r--r--   0        0        0     3863 2023-03-23 15:35:25.660897 girok-0.1.9/girok/calendar_cli/calendar_main.css
+-rw-r--r--   0        0        0     6998 2023-03-23 17:09:49.622419 girok-0.1.9/girok/calendar_cli/calendar_main.py
+-rw-r--r--   0        0        0     6711 2023-03-23 15:35:25.662125 girok-0.1.9/girok/calendar_cli/sidebar.py
+-rw-r--r--   0        0        0    76495 2023-03-23 15:35:25.662963 girok-0.1.9/girok/calendar_cli/textual_demo_2023-03-11T22_49_21_681307.svg
+-rw-r--r--   0        0        0     3879 2023-03-25 05:34:37.685563 girok-0.1.9/girok/commands/auth.py
+-rw-r--r--   0        0        0      330 2023-03-23 18:32:48.364884 girok-0.1.9/girok/commands/calendar.py
+-rw-r--r--   0        0        0     5264 2023-03-23 18:32:48.365585 girok-0.1.9/girok/commands/category.py
+-rw-r--r--   0        0        0    28335 2023-03-23 19:28:42.711527 girok-0.1.9/girok/commands/task.py
+-rw-r--r--   0        0        0      171 2023-03-25 04:45:53.523094 girok-0.1.9/girok/config.json
+-rw-r--r--   0        0        0      678 2023-03-25 04:45:53.523417 girok-0.1.9/girok/config.py
+-rw-r--r--   0        0        0     1408 2023-03-23 15:35:25.665989 girok-0.1.9/girok/constants.py
+-rw-r--r--   0        0        0     1742 2023-03-23 18:32:48.369956 girok-0.1.9/girok/girok.py
+-rw-r--r--   0        0        0      559 2023-03-23 15:37:19.810418 girok-0.1.9/girok/styles/stopwatch03.css
+-rw-r--r--   0        0        0        0 2023-03-23 15:35:25.666933 girok-0.1.9/girok/utils/__init__.py
+-rw-r--r--   0        0        0     1412 2023-03-25 04:45:53.523763 girok-0.1.9/girok/utils/auth.py
+-rw-r--r--   0        0        0     4120 2023-03-24 03:43:01.283009 girok-0.1.9/girok/utils/calendar.py
+-rw-r--r--   0        0        0    11059 2023-03-23 17:57:47.427476 girok-0.1.9/girok/utils/display.py
+-rw-r--r--   0        0        0     1130 2023-03-23 15:35:25.668533 girok-0.1.9/girok/utils/general.py
+-rw-r--r--   0        0        0     4906 2023-03-23 15:35:25.669005 girok-0.1.9/girok/utils/task.py
+-rw-r--r--   0        0        0     1123 2023-03-25 07:35:14.147208 girok-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    21586 1970-01-01 00:00:00.000000 girok-0.1.9/PKG-INFO
```

### Comparing `girok-0.1.8/README.md` & `girok-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `girok-0.1.8/girok/api/auth.py` & `girok-0.1.9/girok/api/auth.py`

 * *Files identical despite different names*

### Comparing `girok-0.1.8/girok/api/category.py` & `girok-0.1.9/girok/api/category.py`

 * *Files identical despite different names*

### Comparing `girok-0.1.8/girok/api/task.py` & `girok-0.1.9/girok/api/task.py`

 * *Files identical despite different names*

### Comparing `girok-0.1.8/girok/calendar_cli/calendar_app.py` & `girok-0.1.9/girok/calendar_cli/calendar_app.py`

 * *Files identical despite different names*

### Comparing `girok-0.1.8/girok/calendar_cli/calendar_container.py` & `girok-0.1.9/girok/calendar_cli/calendar_container.py`

 * *Files identical despite different names*

### Comparing `girok-0.1.8/girok/calendar_cli/calendar_main.css` & `girok-0.1.9/girok/calendar_cli/calendar_main.css`

 * *Files identical despite different names*

### Comparing `girok-0.1.8/girok/calendar_cli/calendar_main.py` & `girok-0.1.9/girok/calendar_cli/calendar_main.py`

 * *Files identical despite different names*

### Comparing `girok-0.1.8/girok/calendar_cli/sidebar.py` & `girok-0.1.9/girok/calendar_cli/sidebar.py`

 * *Files identical despite different names*

### Comparing `girok-0.1.8/girok/calendar_cli/textual_demo_2023-03-11T22_49_21_681307.svg` & `girok-0.1.9/girok/calendar_cli/textual_demo_2023-03-11T22_49_21_681307.svg`

 * *Files identical despite different names*

### Comparing `girok-0.1.8/girok/commands/auth.py` & `girok-0.1.9/girok/commands/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 @app.command("register", help="[green]Register[/green] a new account", rich_help_panel=":lock: [bold yellow1]Authentication Commands[/bold yellow1]")
 def register():
     access_token = auth_utils.get_access_token_from_json(cfg.config_path)
     if access_token and auth_utils.is_logged_in(access_token):
         print("You're logged in. Please try after log out.")
         exit(0)
         
-    print(":star: This is your first time to use [yellow]girok[/yellow]! :star:\n")
+    print(":star: Welcome to [yellow]girok[/yellow]! :star:\n")
     is_register = typer.confirm("Do you want to register a new account?")
     if is_register:
         email = typer.prompt("Enter email address")
         password = typer.prompt("Enter password", hide_input=True)
         confirm_password = typer.prompt("Confirm password", hide_input=True)
         auth_utils.match_passwords(password, confirm_password)
```

### Comparing `girok-0.1.8/girok/commands/category.py` & `girok-0.1.9/girok/commands/category.py`

 * *Files identical despite different names*

### Comparing `girok-0.1.8/girok/commands/task.py` & `girok-0.1.9/girok/commands/task.py`

 * *Files identical despite different names*

### Comparing `girok-0.1.8/girok/config.py` & `girok-0.1.9/girok/config.py`

 * *Files identical despite different names*

### Comparing `girok-0.1.8/girok/constants.py` & `girok-0.1.9/girok/constants.py`

 * *Files identical despite different names*

### Comparing `girok-0.1.8/girok/girok.py` & `girok-0.1.9/girok/girok.py`

 * *Files identical despite different names*

### Comparing `girok-0.1.8/girok/styles/stopwatch03.css` & `girok-0.1.9/girok/styles/stopwatch03.css`

 * *Files identical despite different names*

### Comparing `girok-0.1.8/girok/utils/auth.py` & `girok-0.1.9/girok/utils/auth.py`

 * *Files identical despite different names*

### Comparing `girok-0.1.8/girok/utils/calendar.py` & `girok-0.1.9/girok/utils/calendar.py`

 * *Files identical despite different names*

### Comparing `girok-0.1.8/girok/utils/display.py` & `girok-0.1.9/girok/utils/display.py`

 * *Files identical despite different names*

### Comparing `girok-0.1.8/girok/utils/general.py` & `girok-0.1.9/girok/utils/general.py`

 * *Files identical despite different names*

### Comparing `girok-0.1.8/girok/utils/task.py` & `girok-0.1.9/girok/utils/task.py`

 * *Files identical despite different names*

### Comparing `girok-0.1.8/pyproject.toml` & `girok-0.1.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "girok"
-version = "0.1.8"
-description = "Integrated email verification - credits to @yeonpark"
+version = "0.1.9"
+description = "Fixed email verification"
 authors = ["Jason Lee <changjin9792@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 girok = "girok.girok:app"
 
 [tool.poetry.dependencies]
```

### Comparing `girok-0.1.8/PKG-INFO` & `girok-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: girok
-Version: 0.1.8
-Summary: Integrated email verification - credits to @yeonpark
+Version: 0.1.9
+Summary: Fixed email verification
 Author: Jason Lee
 Author-email: changjin9792@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

