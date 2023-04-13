# Comparing `tmp/webssh_embedded-1.0.2.tar.gz` & `tmp/webssh_embedded-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webssh_embedded-1.0.2.tar", last modified: Thu Apr 13 17:01:55 2023, max compression
+gzip compressed data, was "webssh_embedded-1.0.3.tar", last modified: Thu Apr 13 17:59:11 2023, max compression
```

## Comparing `webssh_embedded-1.0.2.tar` & `webssh_embedded-1.0.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 17:01:55.174005 webssh_embedded-1.0.2/
--rw-r--r--   0 kali      (1000) kali      (1000)     2255 2023-04-13 11:38:35.000000 webssh_embedded-1.0.2/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)       87 2023-04-12 10:34:57.000000 webssh_embedded-1.0.2/MANIFEST.in
--rw-r--r--   0 kali      (1000) kali      (1000)     2760 2023-04-13 17:01:55.174005 webssh_embedded-1.0.2/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     2200 2023-04-13 12:23:43.000000 webssh_embedded-1.0.2/README.rst
--rw-r--r--   0 kali      (1000) kali      (1000)      172 2023-04-13 17:01:55.174005 webssh_embedded-1.0.2/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     1067 2023-04-11 18:02:24.000000 webssh_embedded-1.0.2/setup.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 17:01:55.157997 webssh_embedded-1.0.2/webssh_embedded/
--rw-r--r--   0 kali      (1000) kali      (1000)      328 2023-04-11 15:20:01.000000 webssh_embedded-1.0.2/webssh_embedded/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)       80 2023-04-13 17:01:26.000000 webssh_embedded-1.0.2/webssh_embedded/_version.py
--rw-r--r--   0 kali      (1000) kali      (1000)    23739 2023-04-11 15:20:01.000000 webssh_embedded-1.0.2/webssh_embedded/handler.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2049 2023-04-11 15:20:01.000000 webssh_embedded-1.0.2/webssh_embedded/main.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2677 2023-04-11 15:20:01.000000 webssh_embedded-1.0.2/webssh_embedded/policy.py
--rw-r--r--   0 kali      (1000) kali      (1000)     6630 2023-04-11 17:53:31.000000 webssh_embedded-1.0.2/webssh_embedded/settings.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 17:01:55.145991 webssh_embedded-1.0.2/webssh_embedded/static/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 17:01:55.166001 webssh_embedded-1.0.2/webssh_embedded/static/css/
--rw-r--r--   0 kali      (1000) kali      (1000)   155758 2023-04-11 15:20:01.000000 webssh_embedded-1.0.2/webssh_embedded/static/css/bootstrap.min.css
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 17:01:55.166001 webssh_embedded-1.0.2/webssh_embedded/static/css/fonts/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-04-11 15:20:01.000000 webssh_embedded-1.0.2/webssh_embedded/static/css/fonts/.gitignore
--rw-r--r--   0 kali      (1000) kali      (1000)      145 2023-04-11 15:20:01.000000 webssh_embedded-1.0.2/webssh_embedded/static/css/fullscreen.min.css
--rw-r--r--   0 kali      (1000) kali      (1000)     1344 2023-04-11 15:20:01.000000 webssh_embedded-1.0.2/webssh_embedded/static/css/xterm.min.css
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 17:01:55.166001 webssh_embedded-1.0.2/webssh_embedded/static/img/
--rw-r--r--   0 kali      (1000) kali      (1000)     5953 2023-04-11 15:20:01.000000 webssh_embedded-1.0.2/webssh_embedded/static/img/favicon.png
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 17:01:55.174005 webssh_embedded-1.0.2/webssh_embedded/static/js/
--rw-r--r--   0 kali      (1000) kali      (1000)    56292 2023-04-11 15:20:01.000000 webssh_embedded-1.0.2/webssh_embedded/static/js/bootstrap.min.js
--rw-r--r--   0 kali      (1000) kali      (1000)     4856 2023-04-11 15:20:01.000000 webssh_embedded-1.0.2/webssh_embedded/static/js/iframetest.html
--rw-r--r--   0 kali      (1000) kali      (1000)    86927 2023-04-11 15:20:01.000000 webssh_embedded-1.0.2/webssh_embedded/static/js/jquery.min.js
--rw-r--r--   0 kali      (1000) kali      (1000)    23784 2023-04-11 15:20:01.000000 webssh_embedded-1.0.2/webssh_embedded/static/js/main.js
--rw-r--r--   0 kali      (1000) kali      (1000)    21004 2023-04-11 15:20:01.000000 webssh_embedded-1.0.2/webssh_embedded/static/js/popper.min.js
--rw-r--r--   0 kali      (1000) kali      (1000)     2377 2023-04-11 15:20:01.000000 webssh_embedded-1.0.2/webssh_embedded/static/js/xterm-addon-fit.min.js
--rw-r--r--   0 kali      (1000) kali      (1000)   251949 2023-04-11 15:20:01.000000 webssh_embedded-1.0.2/webssh_embedded/static/js/xterm.min.js
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 17:01:55.174005 webssh_embedded-1.0.2/webssh_embedded/templates/
--rw-r--r--   0 kali      (1000) kali      (1000)     4604 2023-04-11 15:20:01.000000 webssh_embedded-1.0.2/webssh_embedded/templates/index.html
--rw-r--r--   0 kali      (1000) kali      (1000)     2919 2023-04-11 15:20:01.000000 webssh_embedded-1.0.2/webssh_embedded/utils.py
--rw-r--r--   0 kali      (1000) kali      (1000)    10908 2023-04-13 17:01:10.000000 webssh_embedded-1.0.2/webssh_embedded/worker.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 17:01:55.161999 webssh_embedded-1.0.2/webssh_embedded.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     2760 2023-04-13 17:01:55.000000 webssh_embedded-1.0.2/webssh_embedded.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     1036 2023-04-13 17:01:55.000000 webssh_embedded-1.0.2/webssh_embedded.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-13 17:01:55.000000 webssh_embedded-1.0.2/webssh_embedded.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       64 2023-04-13 17:01:55.000000 webssh_embedded-1.0.2/webssh_embedded.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       54 2023-04-13 17:01:55.000000 webssh_embedded-1.0.2/webssh_embedded.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       16 2023-04-13 17:01:55.000000 webssh_embedded-1.0.2/webssh_embedded.egg-info/top_level.txt
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 17:59:11.022578 webssh_embedded-1.0.3/
+-rw-r--r--   0 kali      (1000) kali      (1000)     2255 2023-04-13 11:38:35.000000 webssh_embedded-1.0.3/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)       87 2023-04-12 10:34:57.000000 webssh_embedded-1.0.3/MANIFEST.in
+-rw-r--r--   0 kali      (1000) kali      (1000)     2760 2023-04-13 17:59:11.022578 webssh_embedded-1.0.3/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     2200 2023-04-13 12:23:43.000000 webssh_embedded-1.0.3/README.rst
+-rw-r--r--   0 kali      (1000) kali      (1000)      172 2023-04-13 17:59:11.030582 webssh_embedded-1.0.3/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     1067 2023-04-11 18:02:24.000000 webssh_embedded-1.0.3/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 17:59:10.798466 webssh_embedded-1.0.3/webssh_embedded/
+-rw-r--r--   0 kali      (1000) kali      (1000)      328 2023-04-11 15:20:01.000000 webssh_embedded-1.0.3/webssh_embedded/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       80 2023-04-13 17:58:47.000000 webssh_embedded-1.0.3/webssh_embedded/_version.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    23739 2023-04-11 15:20:01.000000 webssh_embedded-1.0.3/webssh_embedded/handler.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2049 2023-04-11 15:20:01.000000 webssh_embedded-1.0.3/webssh_embedded/main.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2677 2023-04-11 15:20:01.000000 webssh_embedded-1.0.3/webssh_embedded/policy.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     6630 2023-04-11 17:53:31.000000 webssh_embedded-1.0.3/webssh_embedded/settings.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 17:59:10.794464 webssh_embedded-1.0.3/webssh_embedded/static/
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 17:59:10.850492 webssh_embedded-1.0.3/webssh_embedded/static/css/
+-rw-r--r--   0 kali      (1000) kali      (1000)   155758 2023-04-11 15:20:01.000000 webssh_embedded-1.0.3/webssh_embedded/static/css/bootstrap.min.css
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 17:59:10.858496 webssh_embedded-1.0.3/webssh_embedded/static/css/fonts/
+-rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-04-11 15:20:01.000000 webssh_embedded-1.0.3/webssh_embedded/static/css/fonts/.gitignore
+-rw-r--r--   0 kali      (1000) kali      (1000)      145 2023-04-11 15:20:01.000000 webssh_embedded-1.0.3/webssh_embedded/static/css/fullscreen.min.css
+-rw-r--r--   0 kali      (1000) kali      (1000)     1344 2023-04-11 15:20:01.000000 webssh_embedded-1.0.3/webssh_embedded/static/css/xterm.min.css
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 17:59:10.858496 webssh_embedded-1.0.3/webssh_embedded/static/img/
+-rw-r--r--   0 kali      (1000) kali      (1000)     5953 2023-04-11 15:20:01.000000 webssh_embedded-1.0.3/webssh_embedded/static/img/favicon.png
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 17:59:10.986560 webssh_embedded-1.0.3/webssh_embedded/static/js/
+-rw-r--r--   0 kali      (1000) kali      (1000)    56292 2023-04-11 15:20:01.000000 webssh_embedded-1.0.3/webssh_embedded/static/js/bootstrap.min.js
+-rw-r--r--   0 kali      (1000) kali      (1000)     4856 2023-04-11 15:20:01.000000 webssh_embedded-1.0.3/webssh_embedded/static/js/iframetest.html
+-rw-r--r--   0 kali      (1000) kali      (1000)    86927 2023-04-11 15:20:01.000000 webssh_embedded-1.0.3/webssh_embedded/static/js/jquery.min.js
+-rw-r--r--   0 kali      (1000) kali      (1000)    23784 2023-04-11 15:20:01.000000 webssh_embedded-1.0.3/webssh_embedded/static/js/main.js
+-rw-r--r--   0 kali      (1000) kali      (1000)    21004 2023-04-11 15:20:01.000000 webssh_embedded-1.0.3/webssh_embedded/static/js/popper.min.js
+-rw-r--r--   0 kali      (1000) kali      (1000)     2377 2023-04-11 15:20:01.000000 webssh_embedded-1.0.3/webssh_embedded/static/js/xterm-addon-fit.min.js
+-rw-r--r--   0 kali      (1000) kali      (1000)   251949 2023-04-11 15:20:01.000000 webssh_embedded-1.0.3/webssh_embedded/static/js/xterm.min.js
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 17:59:11.014574 webssh_embedded-1.0.3/webssh_embedded/templates/
+-rw-r--r--   0 kali      (1000) kali      (1000)     4604 2023-04-11 15:20:01.000000 webssh_embedded-1.0.3/webssh_embedded/templates/index.html
+-rw-r--r--   0 kali      (1000) kali      (1000)     2919 2023-04-11 15:20:01.000000 webssh_embedded-1.0.3/webssh_embedded/utils.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    10816 2023-04-13 17:52:22.000000 webssh_embedded-1.0.3/webssh_embedded/worker.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-13 17:59:10.810472 webssh_embedded-1.0.3/webssh_embedded.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     2760 2023-04-13 17:59:10.000000 webssh_embedded-1.0.3/webssh_embedded.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     1036 2023-04-13 17:59:10.000000 webssh_embedded-1.0.3/webssh_embedded.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-13 17:59:10.000000 webssh_embedded-1.0.3/webssh_embedded.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       64 2023-04-13 17:59:10.000000 webssh_embedded-1.0.3/webssh_embedded.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       54 2023-04-13 17:59:10.000000 webssh_embedded-1.0.3/webssh_embedded.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       16 2023-04-13 17:59:10.000000 webssh_embedded-1.0.3/webssh_embedded.egg-info/top_level.txt
```

### Comparing `webssh_embedded-1.0.2/LICENSE` & `webssh_embedded-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.2/PKG-INFO` & `webssh_embedded-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webssh_embedded
-Version: 1.0.2
+Version: 1.0.3
 Summary: Interactive embedded web terminal
 Home-page: https://github.com/TXH2020/webssh_embedded
 Author: Tejas Hegde
 Author-email: 1001.tejas@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `webssh_embedded-1.0.2/README.rst` & `webssh_embedded-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.2/setup.py` & `webssh_embedded-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.2/webssh_embedded/handler.py` & `webssh_embedded-1.0.3/webssh_embedded/handler.py`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.2/webssh_embedded/main.py` & `webssh_embedded-1.0.3/webssh_embedded/main.py`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.2/webssh_embedded/policy.py` & `webssh_embedded-1.0.3/webssh_embedded/policy.py`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.2/webssh_embedded/settings.py` & `webssh_embedded-1.0.3/webssh_embedded/settings.py`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.2/webssh_embedded/static/css/bootstrap.min.css` & `webssh_embedded-1.0.3/webssh_embedded/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.2/webssh_embedded/static/css/xterm.min.css` & `webssh_embedded-1.0.3/webssh_embedded/static/css/xterm.min.css`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.2/webssh_embedded/static/img/favicon.png` & `webssh_embedded-1.0.3/webssh_embedded/static/img/favicon.png`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.2/webssh_embedded/static/js/bootstrap.min.js` & `webssh_embedded-1.0.3/webssh_embedded/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.2/webssh_embedded/static/js/iframetest.html` & `webssh_embedded-1.0.3/webssh_embedded/static/js/iframetest.html`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.2/webssh_embedded/static/js/jquery.min.js` & `webssh_embedded-1.0.3/webssh_embedded/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.2/webssh_embedded/static/js/main.js` & `webssh_embedded-1.0.3/webssh_embedded/static/js/main.js`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.2/webssh_embedded/static/js/popper.min.js` & `webssh_embedded-1.0.3/webssh_embedded/static/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.2/webssh_embedded/static/js/xterm-addon-fit.min.js` & `webssh_embedded-1.0.3/webssh_embedded/static/js/xterm-addon-fit.min.js`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.2/webssh_embedded/static/js/xterm.min.js` & `webssh_embedded-1.0.3/webssh_embedded/static/js/xterm.min.js`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.2/webssh_embedded/templates/index.html` & `webssh_embedded-1.0.3/webssh_embedded/templates/index.html`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.2/webssh_embedded/utils.py` & `webssh_embedded-1.0.3/webssh_embedded/utils.py`

 * *Files identical despite different names*

### Comparing `webssh_embedded-1.0.2/webssh_embedded/worker.py` & `webssh_embedded-1.0.3/webssh_embedded/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,21 +110,19 @@
                     pass
             c=-1
             if(self.timeflag2==1):
                 try:
                     if(self.temp==1):
                         c=re.search('Command_Execution_Status:',t[r:]).start()
                         cstring=t[r:][c:].split(':')[1].rstrip('\r')
-                        logging.info(cstring)
                         cst=re.search('[0-9]{1,3}',cstring)
                         command_execution_status=command_execution_status+cstring[cst.start():cst.end()]
                     else:
                         c=re.search('Command_Execution_Status:',t).start()
                         cstring=t[c:].split(':')[1].rstrip('\r')
-                        logging.info(cstring)
                         cst=re.search('[0-9]{1,3}',cstring)
                         command_execution_status=command_execution_status+cstring[cst.start():cst.end()]
                     self.temp=0
                     self.coflag=0
                     self.timeflag2=0
                     execution_time=self.temp_time_storage
                 except:
```

### Comparing `webssh_embedded-1.0.2/webssh_embedded.egg-info/PKG-INFO` & `webssh_embedded-1.0.3/webssh_embedded.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webssh-embedded
-Version: 1.0.2
+Version: 1.0.3
 Summary: Interactive embedded web terminal
 Home-page: https://github.com/TXH2020/webssh_embedded
 Author: Tejas Hegde
 Author-email: 1001.tejas@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `webssh_embedded-1.0.2/webssh_embedded.egg-info/SOURCES.txt` & `webssh_embedded-1.0.3/webssh_embedded.egg-info/SOURCES.txt`

 * *Files identical despite different names*

