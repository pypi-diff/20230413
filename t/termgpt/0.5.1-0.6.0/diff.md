# Comparing `tmp/termgpt-0.5.1.tar.gz` & `tmp/termgpt-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termgpt-0.5.1.tar", last modified: Wed Apr  5 16:01:03 2023, max compression
+gzip compressed data, was "termgpt-0.6.0.tar", last modified: Thu Apr 13 07:44:58 2023, max compression
```

## Comparing `termgpt-0.5.1.tar` & `termgpt-0.6.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:01:03.645394 termgpt-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-05 16:01:03.645394 termgpt-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-04-05 16:00:50.000000 termgpt-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 16:01:03.645394 termgpt-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-05 16:00:50.000000 termgpt-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:01:03.645394 termgpt-0.5.1/termgpt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 16:00:50.000000 termgpt-0.5.1/termgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-04-05 16:00:50.000000 termgpt-0.5.1/termgpt/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-05 16:00:50.000000 termgpt-0.5.1/termgpt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 16:01:03.645394 termgpt-0.5.1/termgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-05 16:01:03.000000 termgpt-0.5.1/termgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-05 16:01:03.000000 termgpt-0.5.1/termgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 16:01:03.000000 termgpt-0.5.1/termgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-05 16:01:03.000000 termgpt-0.5.1/termgpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-05 16:01:03.000000 termgpt-0.5.1/termgpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-05 16:01:03.000000 termgpt-0.5.1/termgpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:44:58.494744 termgpt-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-13 07:44:58.494744 termgpt-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-13 07:44:50.000000 termgpt-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 07:44:58.494744 termgpt-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-13 07:44:50.000000 termgpt-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:44:58.494744 termgpt-0.6.0/termgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 07:44:50.000000 termgpt-0.6.0/termgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-04-13 07:44:50.000000 termgpt-0.6.0/termgpt/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-13 07:44:50.000000 termgpt-0.6.0/termgpt/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 07:44:50.000000 termgpt-0.6.0/termgpt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:44:58.494744 termgpt-0.6.0/termgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-13 07:44:58.000000 termgpt-0.6.0/termgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-13 07:44:58.000000 termgpt-0.6.0/termgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 07:44:58.000000 termgpt-0.6.0/termgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-13 07:44:58.000000 termgpt-0.6.0/termgpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 07:44:58.000000 termgpt-0.6.0/termgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 07:44:58.000000 termgpt-0.6.0/termgpt.egg-info/top_level.txt
```

### Comparing `termgpt-0.5.1/PKG-INFO` & `termgpt-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termgpt
-Version: 0.5.1
+Version: 0.6.0
 Summary: A chatGPT client on the terminal
 Home-page: https://github.com/tcapelle/termgpt
 Author: Thomas Capelle
 Author-email: tcapelle@pm.me
 License: MIT
 Keywords: artificial intelligence,generative models,natural language processing,openai
 Classifier: Development Status :: 4 - Beta
```

### Comparing `termgpt-0.5.1/README.md` & `termgpt-0.6.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 [![PyPI version](https://badge.fury.io/py/termgpt.svg)](https://badge.fury.io/py/termgpt)
 
 # OpenAI Chatbot
 
-This program uses the OpenAI API to create a chatbot that can converse with users. The chatbot is powered by the GPT-3.5-turbo language model and can answer a wide range of questions.
+This program uses the OpenAI API to create a chatbot that can converse with users. The chatbot is powered by the GPT-3.5-turbo (or 4) language model and can answer a wide range of questions. If you are like me and want to stay in the terminal, this is the tool for you.
 
 # Breaking change: Now you can call gpt3 or gpt4 (if you have an api key for it)
-Beware that using gpt4 is very expensive, so use it with care.
+Beware that using gpt4 is expensive (15x more than 3.5-turbo), so use it with care.
 
-```bash
 ## Install
-> You will need and `openAI` api key, the app expects that the key is available as an environment variable: `OPENAI_API_KEY`.
+You will need and `openAI` api key, the app expects that the key is available as an environment variable: `OPENAI_API_KEY`.
 
 ```bash
 $ pip install termgpt
 ```
 
 ## Usage
 
@@ -70,8 +69,30 @@
 -rw-r--r--  1 tcapelle  staff   276B Mar  6 13:55 chatgpt_history.json
 drwxr-xr-x  4 tcapelle  staff   128B Mar  3 17:07 dist
 -rw-r--r--  1 tcapelle  staff    51B Mar  3 15:33 key
 -rw-r--r--  1 tcapelle  staff   2.5K Mar  3 16:40 lotr.txt
 -rw-r--r--  1 tcapelle  staff   955B Mar  3 18:17 setup.py
 drwxr-xr-x  6 tcapelle  staff   192B Mar  6 09:00 termgpt
 drwxr-xr-x  8 tcapelle  staff   256B Mar  6 08:34 termgpt.egg-info
-```
+```
+
+## Recover output
+
+The history of your conversation is stored in `chatgpt_history.json` so you can recover it later. You also use the `-o` flag to store the output in a plain text file.
+
+```bash
+$ gpt3 -o "poem.txt"
+> Can you write a short poem about chatbots, guacamole and cars?
+
+Chatbots beep and bloop,
+Serving customers with ease,
+Guac and chips in hand.
+
+Cars race on, onwards,
+As chatbots assist the ride,
+Dipping chips divine.
+
+Time taken: 2.27 seconds
+Saving history to chatgpt_history.json, you can restore this session with `--resume`
+Saving output to poem.txt
+```
+
```

### Comparing `termgpt-0.5.1/setup.py` & `termgpt-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `termgpt-0.5.1/termgpt/chat.py` & `termgpt-0.6.0/termgpt/chat.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,89 +1,90 @@
 import os, argparse, json, atexit, subprocess, time
-from sys import platform
 
 import openai
 
 from rich.text import Text
 from rich.console import Console
+from rich.markdown import Markdown
+
+from termgpt.roles import assistant_role, document_role, commander_role
 
 console = Console()
 
 GPT3 = "gpt-3.5-turbo"
 GPT4 = "gpt-4"  # if you have access...
 
-
-# # set api key
-openai_api_key = os.getenv("OPENAI_API_KEY")
-if not openai_api_key:
+if not os.getenv("OPENAI_API_KEY"):
     console.print("[bold red]Please set `OPENAI_API_KEY` environment variable[/]")
     exit(1)
 
 def parse_args():
-    parser = argparse.ArgumentParser()
+    parser = argparse.ArgumentParser(usage="termGPT [options] [file]", description="Chat with GPT-3/4. If no file is provided, you will be prompted to enter a question.")
     parser.add_argument("file", type=str, nargs="?", default=None, help="File to read [optional]")
     parser.add_argument("-r", "--resume", action="store_true", help="Resume previous session")
     parser.add_argument("-c", "--command", type=str, default=None, help="Command to run [optional]")
     parser.add_argument("-o", "--outfile", type=str, default=None, help="Output file [optional]")
+    parser.add_argument("-no_md", "--no_markdown", action="store_false", help="Disable markdown rendering")
     return parser.parse_args()
 
 
 class Chat:
     """Class to handle chat with chatGPT, supports history and load from file"""
 
-    def __init__(self, model_name=GPT3, file=None, resume=False, command=None, out_file=None):
+    def __init__(self, model_name=GPT3, file=None, resume=False, command=None, out_file=None, markdown=True):
         self.history_file = "chatgpt_history.json"
         self.out_file=out_file
         self.model_name=model_name
+        self.output_render = Markdown if markdown else Text
         if command:
-            self.history = [{"role": "system", "content": f"Reply only with the terminal command required to perform the action on {platform}. Nothing else. In plain text, no fancy output."}, ]
+            self.history = [{"role": "system", "content": commander_role}, ]
             cmd = self(command)
             self.exec(cmd=cmd)
         else:
-            self.history = [{"role": "system", "content": "You are a helpful assistant."}, ]
+            self.history = [{"role": "system", "content": assistant_role}, ]
         if resume:
             with open(self.history_file, "r") as f:
                 self.history = json.load(f)
                 self._print_history(self.history)
         if file:
             with open(file, "r") as f:
-                self.history.append({"role": "user", "content": "I will ask question about this file:\n" + f.read()})
+                self.history = [{"role": "system", "content":  document_role + f.read()}, ]
 
     def _print_history(self, history):
         console.print("--Resuming previous session--")
         for h in history:
             if h["role"] == "system":
                 console.print(Text("[System] " + h["content"] +"\n", style="bold green"))
             elif h["role"] == "user":
                 console.print("[bold red]> [/]" + h["content"])
             else:
-                console.print(Text(h["content"], style="bold green"))
+                console.print(self.output_render(h["content"]))
 
     def add(self, role, content):
         self.history.append({"role": role, "content": content})
     
     def __call__(self, question):
         self.add("user", question)
         t0 = time.perf_counter()
         r = openai.ChatCompletion.create(
             model=self.model_name,
             messages=self.history,
         )
         out = r["choices"][0]["message"]["content"]
         self.add("assistant", out)
         total_time = time.perf_counter() - t0
-        console.print(Text(out, style="bold green"))
+        console.print(self.output_render(out, style="bold green"))
         console.print(f"Time taken: {total_time:.2f} seconds")
         return out
 
     def exec(self, cmd):
         """Refine the command to be executed"""
         cmd = cmd.replace("`", "")
-        q = console.input(f"[bold red]Execute this command:[/] `${cmd}` (y/n) ")
-        if q.lower() == "y":
+        q = console.input(f"[bold red]Execute this command (press return to run):[/] \n$ {cmd}").lower()
+        if (q == "y") or (q == ""):
             self.run_cmd(cmd)
         else:
             pass
 
     def run_cmd(self, cmd):
         try:
             subprocess.run(cmd, shell=True, check=True)
@@ -91,25 +92,29 @@
             console.print("[bold red]Error executing command: [/]" + str(e))
 
     def input(self):
         q = console.input("[bold red]> [/]")
         return q
 
     def save(self):
-        print(f"Saving history to {self.history_file}, you can restore this session with `--resume`")
+        print(f"-------------\nSaving history to {self.history_file}, you can restore this session with `--resume`")
         with open(self.history_file, "w") as f:
             json.dump(self.history, f)
         if self.out_file is not None:
             with open(self.out_file, "w") as out_f:
                 print(f"Saving output to {self.out_file}")
                 out_f.writelines([h["content"] for h in self.history])
 
+exit_commands = ["exit", "quit", "q", "bye", "goodbye", "stop", "end", "finish", "done"]
+
 def main(model_name):
     args = parse_args()
-    chat = Chat(model_name, file=args.file, resume=args.resume, command=args.command, out_file=args.outfile)
+    chat = Chat(model_name, file=args.file, resume=args.resume, command=args.command, out_file=args.outfile, markdown=args.no_markdown)
     atexit.register(chat.save)
     if not args.command:
         while q := chat.input():
+            if q in exit_commands:
+                break
             _ = chat(q)
 
 def gpt3(): main(GPT3)
 def gpt4(): main(GPT4)
```

### Comparing `termgpt-0.5.1/termgpt.egg-info/PKG-INFO` & `termgpt-0.6.0/termgpt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termgpt
-Version: 0.5.1
+Version: 0.6.0
 Summary: A chatGPT client on the terminal
 Home-page: https://github.com/tcapelle/termgpt
 Author: Thomas Capelle
 Author-email: tcapelle@pm.me
 License: MIT
 Keywords: artificial intelligence,generative models,natural language processing,openai
 Classifier: Development Status :: 4 - Beta
```

