# Comparing `tmp/sleepyask-4.4.0.tar.gz` & `tmp/sleepyask-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepyask-4.4.0.tar", last modified: Tue Apr 11 22:13:32 2023, max compression
+gzip compressed data, was "sleepyask-4.5.0.tar", last modified: Thu Apr 13 17:01:02 2023, max compression
```

## Comparing `sleepyask-4.4.0.tar` & `sleepyask-4.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:13:32.552820 sleepyask-4.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-11 22:13:21.000000 sleepyask-4.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-04-11 22:13:32.552820 sleepyask-4.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-04-11 22:13:21.000000 sleepyask-4.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-11 22:13:21.000000 sleepyask-4.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 22:13:32.552820 sleepyask-4.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:13:32.548820 sleepyask-4.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:13:32.548820 sleepyask-4.4.0/src/sleepyask/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:13:32.552820 sleepyask-4.4.0/src/sleepyask/openai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 22:13:21.000000 sleepyask-4.4.0/src/sleepyask/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-11 22:13:21.000000 sleepyask-4.4.0/src/sleepyask/openai/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-11 22:13:21.000000 sleepyask-4.4.0/src/sleepyask/openai/chatgpt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:13:32.552820 sleepyask-4.4.0/src/sleepyask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-04-11 22:13:32.000000 sleepyask-4.4.0/src/sleepyask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-11 22:13:32.000000 sleepyask-4.4.0/src/sleepyask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 22:13:32.000000 sleepyask-4.4.0/src/sleepyask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-11 22:13:32.000000 sleepyask-4.4.0/src/sleepyask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 22:13:32.000000 sleepyask-4.4.0/src/sleepyask.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:01:02.606210 sleepyask-4.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-13 17:00:49.000000 sleepyask-4.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-04-13 17:01:02.606210 sleepyask-4.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-04-13 17:00:49.000000 sleepyask-4.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-13 17:00:49.000000 sleepyask-4.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 17:01:02.606210 sleepyask-4.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:01:02.602210 sleepyask-4.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:01:02.606210 sleepyask-4.5.0/src/sleepyask/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:01:02.606210 sleepyask-4.5.0/src/sleepyask/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:00:49.000000 sleepyask-4.5.0/src/sleepyask/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-13 17:00:49.000000 sleepyask-4.5.0/src/sleepyask/openai/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-04-13 17:00:49.000000 sleepyask-4.5.0/src/sleepyask/openai/chatgpt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:01:02.606210 sleepyask-4.5.0/src/sleepyask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-04-13 17:01:02.000000 sleepyask-4.5.0/src/sleepyask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-13 17:01:02.000000 sleepyask-4.5.0/src/sleepyask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:01:02.000000 sleepyask-4.5.0/src/sleepyask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 17:01:02.000000 sleepyask-4.5.0/src/sleepyask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 17:01:02.000000 sleepyask-4.5.0/src/sleepyask.egg-info/top_level.txt
```

### Comparing `sleepyask-4.4.0/LICENSE` & `sleepyask-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sleepyask-4.4.0/PKG-INFO` & `sleepyask-4.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepyask
-Version: 4.4.0
+Version: 4.5.0
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
-Metadata-Version: 2.1 Name: sleepyask Version: 4.4.0 Summary: A small tool for
+Metadata-Version: 2.1 Name: sleepyask Version: 4.5.0 Summary: A small tool for
 automating collecting data from ChatGPT Author-email: hwelsters
 redacted.redacted> Project-URL: Homepage, https://github.com/hwelsters/
 sleepyask Project-URL: Bug Tracker, https://github.com/hwelsters/sleepyask/
 issues Requires-Python: >=3.7 Description-Content-Type: text/markdown License-
 File: LICENSE
  [https://user-images.githubusercontent.com/84760072/227817729-098182f3-6916-
                           48d8-b17a-4e4126ddd245.png]
```

### Comparing `sleepyask-4.4.0/README.md` & `sleepyask-4.5.0/README.md`

 * *Files identical despite different names*

### Comparing `sleepyask-4.4.0/pyproject.toml` & `sleepyask-4.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sleepyask"
-version = "4.4.0"
+version = "4.5.0"
 authors = [
   { name="hwelsters", email="redacted@redacted.redacted" },
 ]
 description = "A small tool for automating collecting data from ChatGPT"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = []
```

### Comparing `sleepyask-4.4.0/src/sleepyask/openai/chat.py` & `sleepyask-4.5.0/src/sleepyask/openai/chat.py`

 * *Files identical despite different names*

### Comparing `sleepyask-4.4.0/src/sleepyask/openai/chatgpt.py` & `sleepyask-4.5.0/src/sleepyask/openai/chatgpt.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,14 @@
         outfile.write(json.dumps(data))
         outfile.write("\n")
         outfile.close()
 
 
 def __clean_str_for_json(text: str):
     return text
-    return text.replace("\"", "\'")
 
 
 def ask_questions(configs : list, questions : list, output_file_path : str, verbose: bool = False, model : str = "gpt-3.5-turbo", system_text : str | None = None, temperature : float | None = 1, max_tokens : int | None = 2048) -> None:
     question_queue = queue.Queue()
     save_queue = queue.Queue()
 
     def loader_worker():
@@ -39,15 +38,15 @@
                         print(f"Output file is incorrectly formatted {index}")
                     index = index + 1
                 max_index = 0
 
                 for question in asked_questions:
                     check_set.add(question["question_number"])
                     max_index = max(max_index, question["question_number"])
-
+            
         for index in range(0, len(questions)):
             if not index in check_set:
                 question_queue.put(
                     {"question": questions[index], "question_number": index})
 
         if question_queue.empty():
             print("[sleepyask] All questions exhausted")
@@ -68,14 +67,16 @@
         succeed = True
         while succeed:
             if question_queue.empty(): succeed = False
             question = question_queue.get()
             message = ''
             if verbose:
                 print(f"[sleepyask {index}] Asking:", question["question"])
+
+            saved_data = False
             try:
                 messages = [
                     {"role": "user", "content": question["question"]},
                 ]
 
                 if (system_text != None):
                     messages.insert(
@@ -95,22 +96,26 @@
                 if verbose:
                     print(f"[sleepyask {index}] Received:", message)
 
                 dt_string = datetime.now().strftime("%d/%m/%Y %H:%M:%S")
                 row_to_append = {"model": actual_model, "temperature": temperature, "max_tokens": max_tokens, "date_time": dt_string, "question_number":
                                  question["question_number"], "question": question["question"], "system_text": str(system_text), "response": __clean_str_for_json(message), **usage}
                 save_queue.put(row_to_append)
+                saved_data = True
 
             except KeyboardInterrupt:
                 succeed = False
                 break
             except openai.error.AuthenticationError:
                 logging.error(traceback.format_exc())
                 question_queue.put(question)
                 time.sleep(120)
+            except:
+                if not saved_data : 
+                    question_queue.put(question)
 
             question_queue.task_done()
 
     thread_refs = []
     for index, config in enumerate(configs):
         for num in range(config["count"]):
             t = threading.Thread(target=asker_worker, daemon=True, kwargs={
```

### Comparing `sleepyask-4.4.0/src/sleepyask.egg-info/PKG-INFO` & `sleepyask-4.5.0/src/sleepyask.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepyask
-Version: 4.4.0
+Version: 4.5.0
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
-Metadata-Version: 2.1 Name: sleepyask Version: 4.4.0 Summary: A small tool for
+Metadata-Version: 2.1 Name: sleepyask Version: 4.5.0 Summary: A small tool for
 automating collecting data from ChatGPT Author-email: hwelsters
 redacted.redacted> Project-URL: Homepage, https://github.com/hwelsters/
 sleepyask Project-URL: Bug Tracker, https://github.com/hwelsters/sleepyask/
 issues Requires-Python: >=3.7 Description-Content-Type: text/markdown License-
 File: LICENSE
  [https://user-images.githubusercontent.com/84760072/227817729-098182f3-6916-
                           48d8-b17a-4e4126ddd245.png]
```

