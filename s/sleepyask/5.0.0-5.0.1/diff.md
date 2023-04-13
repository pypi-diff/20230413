# Comparing `tmp/sleepyask-5.0.0.tar.gz` & `tmp/sleepyask-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepyask-5.0.0.tar", last modified: Thu Apr 13 17:29:07 2023, max compression
+gzip compressed data, was "sleepyask-5.0.1.tar", last modified: Thu Apr 13 19:53:21 2023, max compression
```

## Comparing `sleepyask-5.0.0.tar` & `sleepyask-5.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:29:07.834202 sleepyask-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-13 17:28:55.000000 sleepyask-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-04-13 17:29:07.834202 sleepyask-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-04-13 17:28:55.000000 sleepyask-5.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-13 17:28:55.000000 sleepyask-5.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 17:29:07.834202 sleepyask-5.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:29:07.834202 sleepyask-5.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:29:07.834202 sleepyask-5.0.0/src/sleepyask/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:29:07.834202 sleepyask-5.0.0/src/sleepyask/openai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:28:55.000000 sleepyask-5.0.0/src/sleepyask/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-13 17:28:55.000000 sleepyask-5.0.0/src/sleepyask/openai/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-13 17:28:55.000000 sleepyask-5.0.0/src/sleepyask/openai/chatgpt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:29:07.834202 sleepyask-5.0.0/src/sleepyask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-04-13 17:29:07.000000 sleepyask-5.0.0/src/sleepyask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-13 17:29:07.000000 sleepyask-5.0.0/src/sleepyask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:29:07.000000 sleepyask-5.0.0/src/sleepyask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 17:29:07.000000 sleepyask-5.0.0/src/sleepyask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 17:29:07.000000 sleepyask-5.0.0/src/sleepyask.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:53:21.095219 sleepyask-5.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-13 19:53:11.000000 sleepyask-5.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-04-13 19:53:21.095219 sleepyask-5.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-04-13 19:53:11.000000 sleepyask-5.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-13 19:53:11.000000 sleepyask-5.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 19:53:21.095219 sleepyask-5.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:53:21.091219 sleepyask-5.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:53:21.091219 sleepyask-5.0.1/src/sleepyask/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:53:21.095219 sleepyask-5.0.1/src/sleepyask/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:53:11.000000 sleepyask-5.0.1/src/sleepyask/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-13 19:53:11.000000 sleepyask-5.0.1/src/sleepyask/openai/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-04-13 19:53:11.000000 sleepyask-5.0.1/src/sleepyask/openai/chatgpt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:53:21.095219 sleepyask-5.0.1/src/sleepyask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-04-13 19:53:21.000000 sleepyask-5.0.1/src/sleepyask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-13 19:53:21.000000 sleepyask-5.0.1/src/sleepyask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 19:53:21.000000 sleepyask-5.0.1/src/sleepyask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 19:53:21.000000 sleepyask-5.0.1/src/sleepyask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 19:53:21.000000 sleepyask-5.0.1/src/sleepyask.egg-info/top_level.txt
```

### Comparing `sleepyask-5.0.0/LICENSE` & `sleepyask-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sleepyask-5.0.0/PKG-INFO` & `sleepyask-5.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepyask
-Version: 5.0.0
+Version: 5.0.1
 Summary: A small tool for automating collecting data from ChatGPT
 Author-email: hwelsters <redacted@redacted.redacted>
 Project-URL: Homepage, https://github.com/hwelsters/sleepyask
 Project-URL: Bug Tracker, https://github.com/hwelsters/sleepyask/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sleepyask Version: 5.0.0 Summary: A small tool for
+Metadata-Version: 2.1 Name: sleepyask Version: 5.0.1 Summary: A small tool for
 automating collecting data from ChatGPT Author-email: hwelsters
 redacted.redacted> Project-URL: Homepage, https://github.com/hwelsters/
 sleepyask Project-URL: Bug Tracker, https://github.com/hwelsters/sleepyask/
 issues Requires-Python: >=3.7 Description-Content-Type: text/markdown License-
 File: LICENSE
  [https://user-images.githubusercontent.com/84760072/227817729-098182f3-6916-
                           48d8-b17a-4e4126ddd245.png]
```

### Comparing `sleepyask-5.0.0/README.md` & `sleepyask-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `sleepyask-5.0.0/pyproject.toml` & `sleepyask-5.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sleepyask"
-version = "5.0.0"
+version = "5.0.1"
 authors = [
   { name="hwelsters", email="redacted@redacted.redacted" },
 ]
 description = "A small tool for automating collecting data from ChatGPT"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = []
```

### Comparing `sleepyask-5.0.0/src/sleepyask/openai/chat.py` & `sleepyask-5.0.1/src/sleepyask/openai/chat.py`

 * *Files identical despite different names*

### Comparing `sleepyask-5.0.0/src/sleepyask/openai/chatgpt.py` & `sleepyask-5.0.1/src/sleepyask/openai/chatgpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,17 @@
             except KeyboardInterrupt:
                 succeed = False
                 break
             except openai.error.AuthenticationError:
                 logging.error(traceback.format_exc())
                 question_queue.put(question)
                 time.sleep(120)
+            except:
+                question_queue.put(question)
+                time.sleep(120)
 
             question_queue.task_done()
 
     thread_refs = []
     for num in range(config["count"]):
         t = threading.Thread(target=asker_worker, daemon=True, kwargs={'index': num})
         thread_refs.append(t)
```

### Comparing `sleepyask-5.0.0/src/sleepyask.egg-info/PKG-INFO` & `sleepyask-5.0.1/src/sleepyask.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepyask
-Version: 5.0.0
+Version: 5.0.1
 Summary: A small tool for automating collecting data from ChatGPT
 Author-email: hwelsters <redacted@redacted.redacted>
 Project-URL: Homepage, https://github.com/hwelsters/sleepyask
 Project-URL: Bug Tracker, https://github.com/hwelsters/sleepyask/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sleepyask Version: 5.0.0 Summary: A small tool for
+Metadata-Version: 2.1 Name: sleepyask Version: 5.0.1 Summary: A small tool for
 automating collecting data from ChatGPT Author-email: hwelsters
 redacted.redacted> Project-URL: Homepage, https://github.com/hwelsters/
 sleepyask Project-URL: Bug Tracker, https://github.com/hwelsters/sleepyask/
 issues Requires-Python: >=3.7 Description-Content-Type: text/markdown License-
 File: LICENSE
  [https://user-images.githubusercontent.com/84760072/227817729-098182f3-6916-
                           48d8-b17a-4e4126ddd245.png]
```

