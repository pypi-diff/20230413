# Comparing `tmp/webssh_embedded-0.0.1.tar.gz` & `tmp/webssh_embedded-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webssh_embedded-0.0.1.tar", last modified: Thu Apr 13 12:01:25 2023, max compression
+gzip compressed data, was "webssh_embedded-1.0.0.tar", last modified: Thu Apr 13 12:26:46 2023, max compression
```

## Comparing `webssh_embedded-0.0.1.tar` & `webssh_embedded-1.0.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 12:01:25.038761 webssh_embedded-0.0.1/
--rw-r--r--   0 kali      (1000) kali      (1000)     2255 2023-04-13 11:38:35.000000 webssh_embedded-0.0.1/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)       87 2023-04-12 10:34:57.000000 webssh_embedded-0.0.1/MANIFEST.in
--rw-r--r--   0 kali      (1000) kali      (1000)     2721 2023-04-13 12:01:25.038761 webssh_embedded-0.0.1/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     2161 2023-04-13 11:59:40.000000 webssh_embedded-0.0.1/README.rst
--rw-r--r--   0 kali      (1000) kali      (1000)      172 2023-04-13 12:01:25.062749 webssh_embedded-0.0.1/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     1067 2023-04-11 18:02:24.000000 webssh_embedded-0.0.1/setup.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 12:01:25.014773 webssh_embedded-0.0.1/webssh_embedded/
--rw-r--r--   0 kali      (1000) kali      (1000)      328 2023-04-11 15:20:01.000000 webssh_embedded-0.0.1/webssh_embedded/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)       80 2023-04-13 12:01:01.000000 webssh_embedded-0.0.1/webssh_embedded/_version.py
--rw-r--r--   0 kali      (1000) kali      (1000)    23739 2023-04-11 15:20:01.000000 webssh_embedded-0.0.1/webssh_embedded/handler.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2049 2023-04-11 15:20:01.000000 webssh_embedded-0.0.1/webssh_embedded/main.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2677 2023-04-11 15:20:01.000000 webssh_embedded-0.0.1/webssh_embedded/policy.py
--rw-r--r--   0 kali      (1000) kali      (1000)     6630 2023-04-11 17:53:31.000000 webssh_embedded-0.0.1/webssh_embedded/settings.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 12:01:24.994783 webssh_embedded-0.0.1/webssh_embedded/static/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 12:01:25.022769 webssh_embedded-0.0.1/webssh_embedded/static/css/
--rw-r--r--   0 kali      (1000) kali      (1000)   155758 2023-04-11 15:20:01.000000 webssh_embedded-0.0.1/webssh_embedded/static/css/bootstrap.min.css
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 12:01:25.022769 webssh_embedded-0.0.1/webssh_embedded/static/css/fonts/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-04-11 15:20:01.000000 webssh_embedded-0.0.1/webssh_embedded/static/css/fonts/.gitignore
--rw-r--r--   0 kali      (1000) kali      (1000)      145 2023-04-11 15:20:01.000000 webssh_embedded-0.0.1/webssh_embedded/static/css/fullscreen.min.css
--rw-r--r--   0 kali      (1000) kali      (1000)     1344 2023-04-11 15:20:01.000000 webssh_embedded-0.0.1/webssh_embedded/static/css/xterm.min.css
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 12:01:25.022769 webssh_embedded-0.0.1/webssh_embedded/static/img/
--rw-r--r--   0 kali      (1000) kali      (1000)     5953 2023-04-11 15:20:01.000000 webssh_embedded-0.0.1/webssh_embedded/static/img/favicon.png
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 12:01:25.038761 webssh_embedded-0.0.1/webssh_embedded/static/js/
--rw-r--r--   0 kali      (1000) kali      (1000)    56292 2023-04-11 15:20:01.000000 webssh_embedded-0.0.1/webssh_embedded/static/js/bootstrap.min.js
--rw-r--r--   0 kali      (1000) kali      (1000)     4856 2023-04-11 15:20:01.000000 webssh_embedded-0.0.1/webssh_embedded/static/js/iframetest.html
--rw-r--r--   0 kali      (1000) kali      (1000)    86927 2023-04-11 15:20:01.000000 webssh_embedded-0.0.1/webssh_embedded/static/js/jquery.min.js
--rw-r--r--   0 kali      (1000) kali      (1000)    23784 2023-04-11 15:20:01.000000 webssh_embedded-0.0.1/webssh_embedded/static/js/main.js
--rw-r--r--   0 kali      (1000) kali      (1000)    21004 2023-04-11 15:20:01.000000 webssh_embedded-0.0.1/webssh_embedded/static/js/popper.min.js
--rw-r--r--   0 kali      (1000) kali      (1000)     2377 2023-04-11 15:20:01.000000 webssh_embedded-0.0.1/webssh_embedded/static/js/xterm-addon-fit.min.js
--rw-r--r--   0 kali      (1000) kali      (1000)   251949 2023-04-11 15:20:01.000000 webssh_embedded-0.0.1/webssh_embedded/static/js/xterm.min.js
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 12:01:25.038761 webssh_embedded-0.0.1/webssh_embedded/templates/
--rw-r--r--   0 kali      (1000) kali      (1000)     4604 2023-04-11 15:20:01.000000 webssh_embedded-0.0.1/webssh_embedded/templates/index.html
--rw-r--r--   0 kali      (1000) kali      (1000)     2919 2023-04-11 15:20:01.000000 webssh_embedded-0.0.1/webssh_embedded/utils.py
--rw-r--r--   0 kali      (1000) kali      (1000)     9795 2023-04-12 14:18:37.000000 webssh_embedded-0.0.1/webssh_embedded/worker.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 12:01:25.014773 webssh_embedded-0.0.1/webssh_embedded.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     2721 2023-04-13 12:01:24.000000 webssh_embedded-0.0.1/webssh_embedded.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     1036 2023-04-13 12:01:24.000000 webssh_embedded-0.0.1/webssh_embedded.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-13 12:01:24.000000 webssh_embedded-0.0.1/webssh_embedded.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       64 2023-04-13 12:01:24.000000 webssh_embedded-0.0.1/webssh_embedded.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       54 2023-04-13 12:01:24.000000 webssh_embedded-0.0.1/webssh_embedded.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       16 2023-04-13 12:01:24.000000 webssh_embedded-0.0.1/webssh_embedded.egg-info/top_level.txt
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 12:26:46.914059 webssh_embedded-1.0.0/
+-rw-r--r--   0 kali      (1000) kali      (1000)     2255 2023-04-13 11:38:35.000000 webssh_embedded-1.0.0/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)       87 2023-04-12 10:34:57.000000 webssh_embedded-1.0.0/MANIFEST.in
+-rw-r--r--   0 kali      (1000) kali      (1000)     2760 2023-04-13 12:26:46.914059 webssh_embedded-1.0.0/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     2200 2023-04-13 12:23:43.000000 webssh_embedded-1.0.0/README.rst
+-rw-r--r--   0 kali      (1000) kali      (1000)      172 2023-04-13 12:26:46.914059 webssh_embedded-1.0.0/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     1067 2023-04-11 18:02:24.000000 webssh_embedded-1.0.0/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 12:26:46.906063 webssh_embedded-1.0.0/webssh_embedded/
+-rw-r--r--   0 kali      (1000) kali      (1000)      328 2023-04-11 15:20:01.000000 webssh_embedded-1.0.0/webssh_embedded/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       80 2023-04-13 12:20:03.000000 webssh_embedded-1.0.0/webssh_embedded/_version.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    23739 2023-04-11 15:20:01.000000 webssh_embedded-1.0.0/webssh_embedded/handler.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2049 2023-04-11 15:20:01.000000 webssh_embedded-1.0.0/webssh_embedded/main.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2677 2023-04-11 15:20:01.000000 webssh_embedded-1.0.0/webssh_embedded/policy.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     6630 2023-04-11 17:53:31.000000 webssh_embedded-1.0.0/webssh_embedded/settings.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 12:26:46.894069 webssh_embedded-1.0.0/webssh_embedded/static/
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 12:26:46.910061 webssh_embedded-1.0.0/webssh_embedded/static/css/
+-rw-r--r--   0 kali      (1000) kali      (1000)   155758 2023-04-11 15:20:01.000000 webssh_embedded-1.0.0/webssh_embedded/static/css/bootstrap.min.css
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 12:26:46.910061 webssh_embedded-1.0.0/webssh_embedded/static/css/fonts/
+-rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-04-11 15:20:01.000000 webssh_embedded-1.0.0/webssh_embedded/static/css/fonts/.gitignore
+-rw-r--r--   0 kali      (1000) kali      (1000)      145 2023-04-11 15:20:01.000000 webssh_embedded-1.0.0/webssh_embedded/static/css/fullscreen.min.css
+-rw-r--r--   0 kali      (1000) kali      (1000)     1344 2023-04-11 15:20:01.000000 webssh_embedded-1.0.0/webssh_embedded/static/css/xterm.min.css
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 12:26:46.910061 webssh_embedded-1.0.0/webssh_embedded/static/img/
+-rw-r--r--   0 kali      (1000) kali      (1000)     5953 2023-04-11 15:20:01.000000 webssh_embedded-1.0.0/webssh_embedded/static/img/favicon.png
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 12:26:46.914059 webssh_embedded-1.0.0/webssh_embedded/static/js/
+-rw-r--r--   0 kali      (1000) kali      (1000)    56292 2023-04-11 15:20:01.000000 webssh_embedded-1.0.0/webssh_embedded/static/js/bootstrap.min.js
+-rw-r--r--   0 kali      (1000) kali      (1000)     4856 2023-04-11 15:20:01.000000 webssh_embedded-1.0.0/webssh_embedded/static/js/iframetest.html
+-rw-r--r--   0 kali      (1000) kali      (1000)    86927 2023-04-11 15:20:01.000000 webssh_embedded-1.0.0/webssh_embedded/static/js/jquery.min.js
+-rw-r--r--   0 kali      (1000) kali      (1000)    23784 2023-04-11 15:20:01.000000 webssh_embedded-1.0.0/webssh_embedded/static/js/main.js
+-rw-r--r--   0 kali      (1000) kali      (1000)    21004 2023-04-11 15:20:01.000000 webssh_embedded-1.0.0/webssh_embedded/static/js/popper.min.js
+-rw-r--r--   0 kali      (1000) kali      (1000)     2377 2023-04-11 15:20:01.000000 webssh_embedded-1.0.0/webssh_embedded/static/js/xterm-addon-fit.min.js
+-rw-r--r--   0 kali      (1000) kali      (1000)   251949 2023-04-11 15:20:01.000000 webssh_embedded-1.0.0/webssh_embedded/static/js/xterm.min.js
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 12:26:46.914059 webssh_embedded-1.0.0/webssh_embedded/templates/
+-rw-r--r--   0 kali      (1000) kali      (1000)     4604 2023-04-11 15:20:01.000000 webssh_embedded-1.0.0/webssh_embedded/templates/index.html
+-rw-r--r--   0 kali      (1000) kali      (1000)     2919 2023-04-11 15:20:01.000000 webssh_embedded-1.0.0/webssh_embedded/utils.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     9795 2023-04-12 14:18:37.000000 webssh_embedded-1.0.0/webssh_embedded/worker.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 12:26:46.910061 webssh_embedded-1.0.0/webssh_embedded.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     2760 2023-04-13 12:26:46.000000 webssh_embedded-1.0.0/webssh_embedded.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     1036 2023-04-13 12:26:46.000000 webssh_embedded-1.0.0/webssh_embedded.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-13 12:26:46.000000 webssh_embedded-1.0.0/webssh_embedded.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       64 2023-04-13 12:26:46.000000 webssh_embedded-1.0.0/webssh_embedded.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       54 2023-04-13 12:26:46.000000 webssh_embedded-1.0.0/webssh_embedded.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       16 2023-04-13 12:26:46.000000 webssh_embedded-1.0.0/webssh_embedded.egg-info/top_level.txt
```

### Comparing `webssh_embedded-0.0.1/LICENSE` & `webssh_embedded-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `webssh_embedded-0.0.1/PKG-INFO` & `webssh_embedded-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webssh_embedded
-Version: 0.0.1
+Version: 1.0.0
 Summary: Interactive embedded web terminal
 Home-page: https://github.com/TXH2020/webssh_embedded
 Author: Tejas Hegde
 Author-email: 1001.tejas@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -31,15 +31,15 @@
 -  Visualize the execution status of the command through color change and also the time taken to execute the command.
 -  Database to keep track of executed commands.
 -  Feature to allow commands to execute in case of webpage reload/refresh events and obtain the status and time for such commands.
 -  Thorough logging to keep track of all events: both on browser's console and server side. An additional file called log.txt is created to log the terminal session.
 -  Prevent empty commands from getting executed.
 -  Prevent user from entering command while a comand is executing.
 -  Commands can also be executed inside tmux, screen or script sessions.
--  A database setup file is also present in the library to easily configure the database.
+-  A database setup file has been included in this project's GitHub repo to easily configure the database.
 
 Requirements
 ~~~~~~~~~~~~
 
 -  Python 3.8+
 -  MySQL database must be installed on the system where this package is installed. Also make sure root can access without password.
 -  The project is optimized for remote machines running Linux. Hence this package will not work for remote machines with non Linux OS.
@@ -54,11 +54,11 @@
 3. Open your browser, navigate to ``127.0.0.1:8888/static/js/iframetest.html``
 4. The UI will appear with the embedded terminal at the bottom displaying a form to enter the SSH credentials. Fill the form. After successful login, you can enter commands through the text input and click on the submit message function.
 
 For a demo of the application check out these YouTube Videos: 
 https://youtu.be/4FTTdmijDu4
 https://youtu.be/hOAWzgMKqsg
 
-For the code of the project visit my GitHub page:
+For the code of the project and more information, visit my GitHub page:
 https://github.com/TXH2020/webssh_embedded
```

### Comparing `webssh_embedded-0.0.1/README.rst` & `webssh_embedded-1.0.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 -  Visualize the execution status of the command through color change and also the time taken to execute the command.
 -  Database to keep track of executed commands.
 -  Feature to allow commands to execute in case of webpage reload/refresh events and obtain the status and time for such commands.
 -  Thorough logging to keep track of all events: both on browser's console and server side. An additional file called log.txt is created to log the terminal session.
 -  Prevent empty commands from getting executed.
 -  Prevent user from entering command while a comand is executing.
 -  Commands can also be executed inside tmux, screen or script sessions.
--  A database setup file is also present in the library to easily configure the database.
+-  A database setup file has been included in this project's GitHub repo to easily configure the database.
 
 Requirements
 ~~~~~~~~~~~~
 
 -  Python 3.8+
 -  MySQL database must be installed on the system where this package is installed. Also make sure root can access without password.
 -  The project is optimized for remote machines running Linux. Hence this package will not work for remote machines with non Linux OS.
@@ -37,9 +37,9 @@
 3. Open your browser, navigate to ``127.0.0.1:8888/static/js/iframetest.html``
 4. The UI will appear with the embedded terminal at the bottom displaying a form to enter the SSH credentials. Fill the form. After successful login, you can enter commands through the text input and click on the submit message function.
 
 For a demo of the application check out these YouTube Videos: 
 https://youtu.be/4FTTdmijDu4
 https://youtu.be/hOAWzgMKqsg
 
-For the code of the project visit my GitHub page:
+For the code of the project and more information, visit my GitHub page:
 https://github.com/TXH2020/webssh_embedded
```

### Comparing `webssh_embedded-0.0.1/setup.py` & `webssh_embedded-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `webssh_embedded-0.0.1/webssh_embedded/handler.py` & `webssh_embedded-1.0.0/webssh_embedded/handler.py`

 * *Files identical despite different names*

### Comparing `webssh_embedded-0.0.1/webssh_embedded/main.py` & `webssh_embedded-1.0.0/webssh_embedded/main.py`

 * *Files identical despite different names*

### Comparing `webssh_embedded-0.0.1/webssh_embedded/policy.py` & `webssh_embedded-1.0.0/webssh_embedded/policy.py`

 * *Files identical despite different names*

### Comparing `webssh_embedded-0.0.1/webssh_embedded/settings.py` & `webssh_embedded-1.0.0/webssh_embedded/settings.py`

 * *Files identical despite different names*

### Comparing `webssh_embedded-0.0.1/webssh_embedded/static/css/bootstrap.min.css` & `webssh_embedded-1.0.0/webssh_embedded/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `webssh_embedded-0.0.1/webssh_embedded/static/css/xterm.min.css` & `webssh_embedded-1.0.0/webssh_embedded/static/css/xterm.min.css`

 * *Files identical despite different names*

### Comparing `webssh_embedded-0.0.1/webssh_embedded/static/img/favicon.png` & `webssh_embedded-1.0.0/webssh_embedded/static/img/favicon.png`

 * *Files identical despite different names*

### Comparing `webssh_embedded-0.0.1/webssh_embedded/static/js/bootstrap.min.js` & `webssh_embedded-1.0.0/webssh_embedded/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `webssh_embedded-0.0.1/webssh_embedded/static/js/iframetest.html` & `webssh_embedded-1.0.0/webssh_embedded/static/js/iframetest.html`

 * *Files identical despite different names*

### Comparing `webssh_embedded-0.0.1/webssh_embedded/static/js/jquery.min.js` & `webssh_embedded-1.0.0/webssh_embedded/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `webssh_embedded-0.0.1/webssh_embedded/static/js/main.js` & `webssh_embedded-1.0.0/webssh_embedded/static/js/main.js`

 * *Files identical despite different names*

### Comparing `webssh_embedded-0.0.1/webssh_embedded/static/js/popper.min.js` & `webssh_embedded-1.0.0/webssh_embedded/static/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `webssh_embedded-0.0.1/webssh_embedded/static/js/xterm-addon-fit.min.js` & `webssh_embedded-1.0.0/webssh_embedded/static/js/xterm-addon-fit.min.js`

 * *Files identical despite different names*

### Comparing `webssh_embedded-0.0.1/webssh_embedded/static/js/xterm.min.js` & `webssh_embedded-1.0.0/webssh_embedded/static/js/xterm.min.js`

 * *Files identical despite different names*

### Comparing `webssh_embedded-0.0.1/webssh_embedded/templates/index.html` & `webssh_embedded-1.0.0/webssh_embedded/templates/index.html`

 * *Files identical despite different names*

### Comparing `webssh_embedded-0.0.1/webssh_embedded/utils.py` & `webssh_embedded-1.0.0/webssh_embedded/utils.py`

 * *Files identical despite different names*

### Comparing `webssh_embedded-0.0.1/webssh_embedded/worker.py` & `webssh_embedded-1.0.0/webssh_embedded/worker.py`

 * *Files identical despite different names*

### Comparing `webssh_embedded-0.0.1/webssh_embedded.egg-info/PKG-INFO` & `webssh_embedded-1.0.0/webssh_embedded.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webssh-embedded
-Version: 0.0.1
+Version: 1.0.0
 Summary: Interactive embedded web terminal
 Home-page: https://github.com/TXH2020/webssh_embedded
 Author: Tejas Hegde
 Author-email: 1001.tejas@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -31,15 +31,15 @@
 -  Visualize the execution status of the command through color change and also the time taken to execute the command.
 -  Database to keep track of executed commands.
 -  Feature to allow commands to execute in case of webpage reload/refresh events and obtain the status and time for such commands.
 -  Thorough logging to keep track of all events: both on browser's console and server side. An additional file called log.txt is created to log the terminal session.
 -  Prevent empty commands from getting executed.
 -  Prevent user from entering command while a comand is executing.
 -  Commands can also be executed inside tmux, screen or script sessions.
--  A database setup file is also present in the library to easily configure the database.
+-  A database setup file has been included in this project's GitHub repo to easily configure the database.
 
 Requirements
 ~~~~~~~~~~~~
 
 -  Python 3.8+
 -  MySQL database must be installed on the system where this package is installed. Also make sure root can access without password.
 -  The project is optimized for remote machines running Linux. Hence this package will not work for remote machines with non Linux OS.
@@ -54,11 +54,11 @@
 3. Open your browser, navigate to ``127.0.0.1:8888/static/js/iframetest.html``
 4. The UI will appear with the embedded terminal at the bottom displaying a form to enter the SSH credentials. Fill the form. After successful login, you can enter commands through the text input and click on the submit message function.
 
 For a demo of the application check out these YouTube Videos: 
 https://youtu.be/4FTTdmijDu4
 https://youtu.be/hOAWzgMKqsg
 
-For the code of the project visit my GitHub page:
+For the code of the project and more information, visit my GitHub page:
 https://github.com/TXH2020/webssh_embedded
```

### Comparing `webssh_embedded-0.0.1/webssh_embedded.egg-info/SOURCES.txt` & `webssh_embedded-1.0.0/webssh_embedded.egg-info/SOURCES.txt`

 * *Files identical despite different names*

