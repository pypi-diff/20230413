# Comparing `tmp/lumeny-0.1.0.tar.gz` & `tmp/lumeny-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumeny-0.1.0.tar", max compression
+gzip compressed data, was "lumeny-0.1.1.tar", max compression
```

## Comparing `lumeny-0.1.0.tar` & `lumeny-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      650 2023-03-26 13:19:21.683305 lumeny-0.1.0/README.md
--rw-r--r--   0        0        0     4712 2023-04-12 16:47:14.787304 lumeny-0.1.0/lumeny/CaldavConnector.py
--rw-r--r--   0        0        0     3765 2023-04-13 12:07:56.836601 lumeny-0.1.0/lumeny/CalendarInteraction.py
--rw-r--r--   0        0        0     1589 2023-03-26 13:11:30.305760 lumeny-0.1.0/lumeny/ConfigLoader.py
--rw-r--r--   0        0        0     2068 2023-03-26 21:54:13.154345 lumeny-0.1.0/lumeny/EmbeddingGenerator.py
--rw-r--r--   0        0        0     3001 2023-04-13 12:08:53.857444 lumeny-0.1.0/lumeny/MinifluxConnector.py
--rw-r--r--   0        0        0        0 2023-03-26 11:54:25.500396 lumeny-0.1.0/lumeny/QdrantConnector.py
--rw-r--r--   0        0        0        0 2023-03-26 11:44:08.561839 lumeny-0.1.0/lumeny/__init__.py
--rw-r--r--   0        0        0     2243 2023-04-12 18:44:21.508152 lumeny-0.1.0/lumeny/ai.py
--rw-r--r--   0        0        0     2003 2023-04-13 12:08:09.609342 lumeny-0.1.0/lumeny/cli.py
--rw-r--r--   0        0        0     1839 2023-04-13 12:08:33.198863 lumeny-0.1.0/lumeny/tui.py
--rw-r--r--   0        0        0      912 2023-04-12 20:24:12.954146 lumeny-0.1.0/lumeny/utils.py
--rw-r--r--   0        0        0      628 2023-04-13 12:07:32.015104 lumeny-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1542 1970-01-01 00:00:00.000000 lumeny-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      652 2023-04-13 12:21:17.181246 lumeny-0.1.1/README.md
+-rw-r--r--   0        0        0     4712 2023-04-12 16:47:14.787304 lumeny-0.1.1/lumeny/CaldavConnector.py
+-rw-r--r--   0        0        0     3765 2023-04-13 12:07:56.836601 lumeny-0.1.1/lumeny/CalendarInteraction.py
+-rw-r--r--   0        0        0     1590 2023-04-13 12:16:45.567741 lumeny-0.1.1/lumeny/ConfigLoader.py
+-rw-r--r--   0        0        0     2068 2023-03-26 21:54:13.154345 lumeny-0.1.1/lumeny/EmbeddingGenerator.py
+-rw-r--r--   0        0        0     3001 2023-04-13 12:18:41.544232 lumeny-0.1.1/lumeny/MinifluxConnector.py
+-rw-r--r--   0        0        0        0 2023-03-26 11:54:25.500396 lumeny-0.1.1/lumeny/QdrantConnector.py
+-rw-r--r--   0        0        0        0 2023-03-26 11:44:08.561839 lumeny-0.1.1/lumeny/__init__.py
+-rw-r--r--   0        0        0     2329 2023-04-13 12:19:59.795216 lumeny-0.1.1/lumeny/ai.py
+-rw-r--r--   0        0        0     2003 2023-04-13 12:08:09.609342 lumeny-0.1.1/lumeny/cli.py
+-rw-r--r--   0        0        0     1839 2023-04-13 12:08:33.198863 lumeny-0.1.1/lumeny/tui.py
+-rw-r--r--   0        0        0      912 2023-04-12 20:24:12.954146 lumeny-0.1.1/lumeny/utils.py
+-rw-r--r--   0        0        0      623 2023-04-13 12:21:26.562312 lumeny-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1544 1970-01-01 00:00:00.000000 lumeny-0.1.1/PKG-INFO
```

### Comparing `lumeny-0.1.0/README.md` & `lumeny-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# Lumen
+# Lumeny
 
-This is lumen, a cli project that I used for my own daily usage.
+This is lumeny, a cli project that I used for my own daily usage.
 
 There are several aspects that I want my cli app grows:
 
 1. Connect to caldav so that it can reminds me of my events, or add new events in cli convinently. Pushing notification to the KDE desktop is also a important part to remind me of the events.
 2. Connect to my RSS reader miniflux and filter the most important feeds using ChatGPT (A small recommendation system).
 3. A TUI based on textual to help me manage several aspects of point 1 and 2, like inspect upcoming events or get general statistic of my feeds, and help me gradually improve the recommandation algorithm.
```

### Comparing `lumeny-0.1.0/lumeny/CaldavConnector.py` & `lumeny-0.1.1/lumeny/CaldavConnector.py`

 * *Files identical despite different names*

### Comparing `lumeny-0.1.0/lumeny/CalendarInteraction.py` & `lumeny-0.1.1/lumeny/CalendarInteraction.py`

 * *Files identical despite different names*

### Comparing `lumeny-0.1.0/lumeny/ConfigLoader.py` & `lumeny-0.1.1/lumeny/ConfigLoader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import yaml
 import os
 from typing import Any
 
-CONFIG_DIR = os.path.join(os.path.expanduser("~"), ".config", "lumen")
+CONFIG_DIR = os.path.join(os.path.expanduser("~"), ".config", "lumeny")
 
 def load_config(config_dir:str = CONFIG_DIR) -> Any:
     with open(os.path.join(config_dir, "config.yml"), "r") as config_file:
         config = yaml.safe_load(config_file)
     return config
 
 class ConfigLoader:
```

### Comparing `lumeny-0.1.0/lumeny/EmbeddingGenerator.py` & `lumeny-0.1.1/lumeny/EmbeddingGenerator.py`

 * *Files identical despite different names*

### Comparing `lumeny-0.1.0/lumeny/MinifluxConnector.py` & `lumeny-0.1.1/lumeny/MinifluxConnector.py`

 * *Files identical despite different names*

### Comparing `lumeny-0.1.0/lumeny/ai.py` & `lumeny-0.1.1/lumeny/ai.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,66 +1,72 @@
 import openai
 import os
 from typing import Dict, List
 import datetime
+from lumeny.ConfigLoader import ConfigLoader
 
-# Set your API key
-openai.api_key = "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"
+# Set your API key from environment variables
+config = ConfigLoader().get_config()
+openai.api_key = config["openai"]["api"]
 
 # Function to interact with the chatcompletion API
 
 
 def chat(conversation, model="gpt-4"):
 
     response = openai.ChatCompletion.create(
         model=model, messages=conversation, temperature=0.1)
 
     return response["choices"][0]["message"]["content"]
 
+
 def create_system_msg(prompt: str) -> Dict[str, str]:
     return {
         "role": "system",
         "content": prompt
     }
-    
+
+
 def create_user_msg(prompt: str) -> Dict[str, str]:
     return {
         "role": "user",
         "content": prompt
     }
 
+
 def create_ai_msg(prompt: str) -> Dict[str, str]:
     return {
         "role": "assistant",
         "content": prompt
     }
 
+
 # Example usage
 if __name__ == "__main__":
 
     today = datetime.date.today()
 
     today = today.strftime("%d-%m-%Y")
     # get the weekday of today
     weekday = datetime.datetime.today().weekday()
-    
+
     # weekdays
-    weekdays = ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday", "Sunday"]
+    weekdays = ["Monday", "Tuesday", "Wednesday",
+                "Thursday", "Friday", "Saturday", "Sunday"]
 
     prompt_content = f"You are a Linux terminal that writes commands for the khal calendar program. Output a command to add the event to the specified calendar ('personal' or 'daily') based on the provided description, use daily as default calendar. Use these flags when needed: -a for the calendar, -l for location(optional), -r for repeat (daily, weekly, monthly, yearly). Infer a reasonable time unless instructed otherwise, provide time in hh:mm 24h format, provide date DD.MM.YYYY format. Syntax: khal new [-a CALENDAR] [OPTIONS] [START [END | DELTA] [TIMEZONE] SUMMARY [:: DESCRIPTION]]. Provide one command without explanation or say 'error' for unclear inputs. today is {today}, {weekdays[weekday]}"
-    
+
     print(today)
     print(weekday)
-    
+
     # get the date of today in the format DD-MM-YYYY
 
     custom_system_prompt: Dict[str, str] = create_system_msg(prompt_content)
 
     print("To quit the conversation, type exit.")
 
     conversation: List[Dict] = [custom_system_prompt]
-    user_message=create_user_msg(input("User: "))
+    user_message = create_user_msg(input("User: "))
     conversation.append(user_message)
 
-    response=chat(conversation)
+    response = chat(conversation)
     print(response)
-
```

### Comparing `lumeny-0.1.0/lumeny/cli.py` & `lumeny-0.1.1/lumeny/cli.py`

 * *Files identical despite different names*

### Comparing `lumeny-0.1.0/lumeny/tui.py` & `lumeny-0.1.1/lumeny/tui.py`

 * *Files identical despite different names*

### Comparing `lumeny-0.1.0/lumeny/utils.py` & `lumeny-0.1.1/lumeny/utils.py`

 * *Files identical despite different names*

### Comparing `lumeny-0.1.0/pyproject.toml` & `lumeny-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lumeny"
-version = "0.1.0"
+version = "0.1.1"
 description = "A cli and tui based personal management app for Lumen Young"
 authors = ["Lumen Young <pip@lumeny.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 caldav = "^1.2.1"
@@ -17,13 +17,13 @@
 docker = "^6.0.1"
 nltk = "^3.8.1"
 pyyaml = "^6.0"
 questionary = "^1.10.0"
 prompt-toolkit = "^3.0.38"
 
 [tool.poetry.scripts]
-lumen = "lumen-young.cli:cli"
+lumen = "lumeny.cli:cli"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lumeny-0.1.0/PKG-INFO` & `lumeny-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumeny
-Version: 0.1.0
+Version: 0.1.1
 Summary: A cli and tui based personal management app for Lumen Young
 Author: Lumen Young
 Author-email: pip@lumeny.io
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -18,17 +18,17 @@
 Requires-Dist: prompt-toolkit (>=3.0.38,<4.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: qdrant-client (>=1.1.0,<2.0.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: textual (>=0.16.0,<0.17.0)
 Description-Content-Type: text/markdown
 
-# Lumen
+# Lumeny
 
-This is lumen, a cli project that I used for my own daily usage.
+This is lumeny, a cli project that I used for my own daily usage.
 
 There are several aspects that I want my cli app grows:
 
 1. Connect to caldav so that it can reminds me of my events, or add new events in cli convinently. Pushing notification to the KDE desktop is also a important part to remind me of the events.
 2. Connect to my RSS reader miniflux and filter the most important feeds using ChatGPT (A small recommendation system).
 3. A TUI based on textual to help me manage several aspects of point 1 and 2, like inspect upcoming events or get general statistic of my feeds, and help me gradually improve the recommandation algorithm.
```

