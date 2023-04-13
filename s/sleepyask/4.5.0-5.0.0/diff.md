# Comparing `tmp/sleepyask-4.5.0.tar.gz` & `tmp/sleepyask-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepyask-4.5.0.tar", last modified: Thu Apr 13 17:01:02 2023, max compression
+gzip compressed data, was "sleepyask-5.0.0.tar", last modified: Thu Apr 13 17:29:07 2023, max compression
```

## Comparing `sleepyask-4.5.0.tar` & `sleepyask-5.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:01:02.606210 sleepyask-4.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-13 17:00:49.000000 sleepyask-4.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-04-13 17:01:02.606210 sleepyask-4.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-04-13 17:00:49.000000 sleepyask-4.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-13 17:00:49.000000 sleepyask-4.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 17:01:02.606210 sleepyask-4.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:01:02.602210 sleepyask-4.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:01:02.606210 sleepyask-4.5.0/src/sleepyask/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:01:02.606210 sleepyask-4.5.0/src/sleepyask/openai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:00:49.000000 sleepyask-4.5.0/src/sleepyask/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-13 17:00:49.000000 sleepyask-4.5.0/src/sleepyask/openai/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-04-13 17:00:49.000000 sleepyask-4.5.0/src/sleepyask/openai/chatgpt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:01:02.606210 sleepyask-4.5.0/src/sleepyask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-04-13 17:01:02.000000 sleepyask-4.5.0/src/sleepyask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-13 17:01:02.000000 sleepyask-4.5.0/src/sleepyask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:01:02.000000 sleepyask-4.5.0/src/sleepyask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 17:01:02.000000 sleepyask-4.5.0/src/sleepyask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 17:01:02.000000 sleepyask-4.5.0/src/sleepyask.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:29:07.834202 sleepyask-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-13 17:28:55.000000 sleepyask-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-04-13 17:29:07.834202 sleepyask-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-04-13 17:28:55.000000 sleepyask-5.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-13 17:28:55.000000 sleepyask-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 17:29:07.834202 sleepyask-5.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:29:07.834202 sleepyask-5.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:29:07.834202 sleepyask-5.0.0/src/sleepyask/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:29:07.834202 sleepyask-5.0.0/src/sleepyask/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:28:55.000000 sleepyask-5.0.0/src/sleepyask/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-13 17:28:55.000000 sleepyask-5.0.0/src/sleepyask/openai/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-13 17:28:55.000000 sleepyask-5.0.0/src/sleepyask/openai/chatgpt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:29:07.834202 sleepyask-5.0.0/src/sleepyask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-04-13 17:29:07.000000 sleepyask-5.0.0/src/sleepyask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-13 17:29:07.000000 sleepyask-5.0.0/src/sleepyask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:29:07.000000 sleepyask-5.0.0/src/sleepyask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 17:29:07.000000 sleepyask-5.0.0/src/sleepyask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 17:29:07.000000 sleepyask-5.0.0/src/sleepyask.egg-info/top_level.txt
```

### Comparing `sleepyask-4.5.0/LICENSE` & `sleepyask-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sleepyask-4.5.0/PKG-INFO` & `sleepyask-5.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepyask
-Version: 4.5.0
+Version: 5.0.0
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
-Metadata-Version: 2.1 Name: sleepyask Version: 4.5.0 Summary: A small tool for
+Metadata-Version: 2.1 Name: sleepyask Version: 5.0.0 Summary: A small tool for
 automating collecting data from ChatGPT Author-email: hwelsters
 redacted.redacted> Project-URL: Homepage, https://github.com/hwelsters/
 sleepyask Project-URL: Bug Tracker, https://github.com/hwelsters/sleepyask/
 issues Requires-Python: >=3.7 Description-Content-Type: text/markdown License-
 File: LICENSE
  [https://user-images.githubusercontent.com/84760072/227817729-098182f3-6916-
                           48d8-b17a-4e4126ddd245.png]
```

### Comparing `sleepyask-4.5.0/README.md` & `sleepyask-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `sleepyask-4.5.0/pyproject.toml` & `sleepyask-5.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sleepyask"
-version = "4.5.0"
+version = "5.0.0"
 authors = [
   { name="hwelsters", email="redacted@redacted.redacted" },
 ]
 description = "A small tool for automating collecting data from ChatGPT"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = []
```

### Comparing `sleepyask-4.5.0/src/sleepyask/openai/chat.py` & `sleepyask-5.0.0/src/sleepyask/openai/chat.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from sleepyask.openai.chatgpt import ask_questions
 import traceback
 import logging
 
-def ask(configs : list, questions : list, output_file_path : str, verbose: bool = False, model : str = "gpt-3.5-turbo", system_text : str | None = None, temperature : float | None = 1, max_tokens : int | None = 2048):
+def ask(config, questions : list, output_file_path : str, verbose: bool = False, model : str = "gpt-3.5-turbo", system_text : str | None = None, temperature : float | None = 1, max_tokens : int | None = 2048):
     '''
     `config` should be a list containing your ChatGPT access tokens / email and password\n
     `questions` should contain a list of questions you would like ChatGPT to answer.\n
     `output_file_path` should be the file path where you would like your responses to be saved.\n
     '''
     redo = True
     while redo:
         if not isinstance(questions, list): raise ValueError("[questions] should be a list")
 
-        try: ask_questions(configs=configs, questions=questions, output_file_path=output_file_path, verbose=verbose, model=model, system_text=system_text, temperature=temperature, max_tokens=max_tokens)
+        try: ask_questions(config=config, questions=questions, output_file_path=output_file_path, verbose=verbose, model=model, system_text=system_text, temperature=temperature, max_tokens=max_tokens)
         except Exception as e: 
             logging.error(traceback.format_exc())
```

### Comparing `sleepyask-4.5.0/src/sleepyask/openai/chatgpt.py` & `sleepyask-5.0.0/src/sleepyask/openai/chatgpt.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,30 +2,33 @@
 from pathlib import Path
 from datetime import datetime
 import threading
 import queue
 import logging
 import traceback
 import time
+import openai
 
 def __append_to_file(output_file_path: str, data):
     with open(output_file_path, 'a') as outfile:
         outfile.write(json.dumps(data))
         outfile.write("\n")
         outfile.close()
 
 
 def __clean_str_for_json(text: str):
     return text
 
-
-def ask_questions(configs : list, questions : list, output_file_path : str, verbose: bool = False, model : str = "gpt-3.5-turbo", system_text : str | None = None, temperature : float | None = 1, max_tokens : int | None = 2048) -> None:
+def ask_questions(config, questions : list, output_file_path : str, verbose: bool = False, model : str = "gpt-3.5-turbo", system_text : str | None = None, temperature : float | None = 1, max_tokens : int | None = 2048) -> None:
     question_queue = queue.Queue()
     save_queue = queue.Queue()
 
+    openai.organization = config["organization"]
+    openai.api_key = config["api_key"]
+
     def loader_worker():
         if verbose:
             print(f"[sleepyask] Loading questions into queue")
         # Check for failed questions
         check_set = set()
         if Path(output_file_path).is_file():
             with open(output_file_path) as f:
@@ -38,15 +41,15 @@
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
@@ -55,28 +58,23 @@
     def saver_worker():
         while True:
             if save_queue.empty(): continue
             to_add = save_queue.get()
             __append_to_file(output_file_path, to_add)
             save_queue.task_done()
 
-    def asker_worker(index, config):
-        import openai
-        openai.organization = config["organization"]
-        openai.api_key = config["api_key"]
+    def asker_worker(index):
 
         succeed = True
         while succeed:
             if question_queue.empty(): succeed = False
             question = question_queue.get()
             message = ''
             if verbose:
                 print(f"[sleepyask {index}] Asking:", question["question"])
-
-            saved_data = False
             try:
                 messages = [
                     {"role": "user", "content": question["question"]},
                 ]
 
                 if (system_text != None):
                     messages.insert(
@@ -96,36 +94,30 @@
                 if verbose:
                     print(f"[sleepyask {index}] Received:", message)
 
                 dt_string = datetime.now().strftime("%d/%m/%Y %H:%M:%S")
                 row_to_append = {"model": actual_model, "temperature": temperature, "max_tokens": max_tokens, "date_time": dt_string, "question_number":
                                  question["question_number"], "question": question["question"], "system_text": str(system_text), "response": __clean_str_for_json(message), **usage}
                 save_queue.put(row_to_append)
-                saved_data = True
 
             except KeyboardInterrupt:
                 succeed = False
                 break
             except openai.error.AuthenticationError:
                 logging.error(traceback.format_exc())
                 question_queue.put(question)
                 time.sleep(120)
-            except:
-                if not saved_data : 
-                    question_queue.put(question)
 
             question_queue.task_done()
 
     thread_refs = []
-    for index, config in enumerate(configs):
-        for num in range(config["count"]):
-            t = threading.Thread(target=asker_worker, daemon=True, kwargs={
-                'index': index * config["count"] + num, 'config': config})
-            thread_refs.append(t)
-            t.start()
+    for num in range(config["count"]):
+        t = threading.Thread(target=asker_worker, daemon=True, kwargs={'index': num})
+        thread_refs.append(t)
+        t.start()
 
     loader = threading.Thread(target=loader_worker, daemon=True)
     saver = threading.Thread(target=saver_worker, daemon=True)
     thread_refs.append(loader)
     thread_refs.append(saver)
     
     loader.start()
```

### Comparing `sleepyask-4.5.0/src/sleepyask.egg-info/PKG-INFO` & `sleepyask-5.0.0/src/sleepyask.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepyask
-Version: 4.5.0
+Version: 5.0.0
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
-Metadata-Version: 2.1 Name: sleepyask Version: 4.5.0 Summary: A small tool for
+Metadata-Version: 2.1 Name: sleepyask Version: 5.0.0 Summary: A small tool for
 automating collecting data from ChatGPT Author-email: hwelsters
 redacted.redacted> Project-URL: Homepage, https://github.com/hwelsters/
 sleepyask Project-URL: Bug Tracker, https://github.com/hwelsters/sleepyask/
 issues Requires-Python: >=3.7 Description-Content-Type: text/markdown License-
 File: LICENSE
  [https://user-images.githubusercontent.com/84760072/227817729-098182f3-6916-
                           48d8-b17a-4e4126ddd245.png]
```

