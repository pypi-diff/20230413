# Comparing `tmp/termgpt-0.6.0.tar.gz` & `tmp/termgpt-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termgpt-0.6.0.tar", last modified: Thu Apr 13 07:44:58 2023, max compression
+gzip compressed data, was "termgpt-0.7.0.tar", last modified: Thu Apr 13 08:16:55 2023, max compression
```

## Comparing `termgpt-0.6.0.tar` & `termgpt-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:44:58.494744 termgpt-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-13 07:44:58.494744 termgpt-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-13 07:44:50.000000 termgpt-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 07:44:58.494744 termgpt-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-13 07:44:50.000000 termgpt-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:44:58.494744 termgpt-0.6.0/termgpt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 07:44:50.000000 termgpt-0.6.0/termgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-04-13 07:44:50.000000 termgpt-0.6.0/termgpt/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-13 07:44:50.000000 termgpt-0.6.0/termgpt/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 07:44:50.000000 termgpt-0.6.0/termgpt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:44:58.494744 termgpt-0.6.0/termgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-13 07:44:58.000000 termgpt-0.6.0/termgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-13 07:44:58.000000 termgpt-0.6.0/termgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 07:44:58.000000 termgpt-0.6.0/termgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-13 07:44:58.000000 termgpt-0.6.0/termgpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 07:44:58.000000 termgpt-0.6.0/termgpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 07:44:58.000000 termgpt-0.6.0/termgpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:55.257109 termgpt-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-13 08:16:55.257109 termgpt-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-13 08:16:42.000000 termgpt-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 08:16:55.257109 termgpt-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-13 08:16:42.000000 termgpt-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:55.257109 termgpt-0.7.0/termgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:42.000000 termgpt-0.7.0/termgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-13 08:16:42.000000 termgpt-0.7.0/termgpt/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-13 08:16:42.000000 termgpt-0.7.0/termgpt/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 08:16:42.000000 termgpt-0.7.0/termgpt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:16:55.257109 termgpt-0.7.0/termgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-13 08:16:55.000000 termgpt-0.7.0/termgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-13 08:16:55.000000 termgpt-0.7.0/termgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:16:55.000000 termgpt-0.7.0/termgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-13 08:16:55.000000 termgpt-0.7.0/termgpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 08:16:55.000000 termgpt-0.7.0/termgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 08:16:55.000000 termgpt-0.7.0/termgpt.egg-info/top_level.txt
```

### Comparing `termgpt-0.6.0/PKG-INFO` & `termgpt-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termgpt
-Version: 0.6.0
+Version: 0.7.0
 Summary: A chatGPT client on the terminal
 Home-page: https://github.com/tcapelle/termgpt
 Author: Thomas Capelle
 Author-email: tcapelle@pm.me
 License: MIT
 Keywords: artificial intelligence,generative models,natural language processing,openai
 Classifier: Development Status :: 4 - Beta
```

### Comparing `termgpt-0.6.0/README.md` & `termgpt-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `termgpt-0.6.0/setup.py` & `termgpt-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `termgpt-0.6.0/termgpt/chat.py` & `termgpt-0.7.0/termgpt/chat.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,66 @@
 import os, argparse, json, atexit, subprocess, time
+from dataclasses import dataclass
 
 import openai
 
 from rich.text import Text
 from rich.console import Console
 from rich.markdown import Markdown
 
 from termgpt.roles import assistant_role, document_role, commander_role
 
 console = Console()
 
 GPT3 = "gpt-3.5-turbo"
 GPT4 = "gpt-4"  # if you have access...
+PRICING = {GPT3: (0.02, 0.02), GPT4: (0.03, 0.06)} # prices per 1k tokens
 
 if not os.getenv("OPENAI_API_KEY"):
     console.print("[bold red]Please set `OPENAI_API_KEY` environment variable[/]")
     exit(1)
 
 def parse_args():
     parser = argparse.ArgumentParser(usage="termGPT [options] [file]", description="Chat with GPT-3/4. If no file is provided, you will be prompted to enter a question.")
     parser.add_argument("file", type=str, nargs="?", default=None, help="File to read [optional]")
     parser.add_argument("-r", "--resume", action="store_true", help="Resume previous session")
     parser.add_argument("-c", "--command", type=str, default=None, help="Command to run [optional]")
     parser.add_argument("-o", "--outfile", type=str, default=None, help="Output file [optional]")
     parser.add_argument("-no_md", "--no_markdown", action="store_false", help="Disable markdown rendering")
     return parser.parse_args()
 
+@dataclass
+class APIStats:
+    """Class to handle API usage stats"""
+    model_name: str = GPT3
+    prompt_tokens: int = 0
+    completion_tokens: int = 0
+    total_tokens: int = 0
+
+    def cost(self):
+        token_prices = PRICING[self.model_name]
+        return (token_prices[0] * self.prompt_tokens + token_prices[1] * self.completion_tokens) / 1000
+
+    def update(self, stats):
+        self.prompt_tokens += stats['prompt_tokens']
+        self.completion_tokens += stats['completion_tokens']
+        self.total_tokens += stats['total_tokens']
+
+    def __str__(self):
+        return (f"Prompt tokens: {self.prompt_tokens}, Completion tokens: {self.completion_tokens}, "
+                f"Total tokens: {self.total_tokens}, Estimated cost: ${self.cost():.2f}")
 
 class Chat:
     """Class to handle chat with chatGPT, supports history and load from file"""
 
     def __init__(self, model_name=GPT3, file=None, resume=False, command=None, out_file=None, markdown=True):
         self.history_file = "chatgpt_history.json"
         self.out_file=out_file
         self.model_name=model_name
+        self.usage = APIStats(model_name=model_name)
         self.output_render = Markdown if markdown else Text
         if command:
             self.history = [{"role": "system", "content": commander_role}, ]
             cmd = self(command)
             self.exec(cmd=cmd)
         else:
             self.history = [{"role": "system", "content": assistant_role}, ]
@@ -66,14 +89,15 @@
         self.add("user", question)
         t0 = time.perf_counter()
         r = openai.ChatCompletion.create(
             model=self.model_name,
             messages=self.history,
         )
         out = r["choices"][0]["message"]["content"]
+        self.usage.update(r['usage'])
         self.add("assistant", out)
         total_time = time.perf_counter() - t0
         console.print(self.output_render(out, style="bold green"))
         console.print(f"Time taken: {total_time:.2f} seconds")
         return out
 
     def exec(self, cmd):
@@ -92,15 +116,16 @@
             console.print("[bold red]Error executing command: [/]" + str(e))
 
     def input(self):
         q = console.input("[bold red]> [/]")
         return q
 
     def save(self):
-        print(f"-------------\nSaving history to {self.history_file}, you can restore this session with `--resume`")
+        console.print(f"-------------\nSaving history to {self.history_file}, you can restore this session with `--resume`")
+        console.print(str(self.usage))
         with open(self.history_file, "w") as f:
             json.dump(self.history, f)
         if self.out_file is not None:
             with open(self.out_file, "w") as out_f:
                 print(f"Saving output to {self.out_file}")
                 out_f.writelines([h["content"] for h in self.history])
```

### Comparing `termgpt-0.6.0/termgpt/roles.py` & `termgpt-0.7.0/termgpt/roles.py`

 * *Files identical despite different names*

### Comparing `termgpt-0.6.0/termgpt.egg-info/PKG-INFO` & `termgpt-0.7.0/termgpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termgpt
-Version: 0.6.0
+Version: 0.7.0
 Summary: A chatGPT client on the terminal
 Home-page: https://github.com/tcapelle/termgpt
 Author: Thomas Capelle
 Author-email: tcapelle@pm.me
 License: MIT
 Keywords: artificial intelligence,generative models,natural language processing,openai
 Classifier: Development Status :: 4 - Beta
```

