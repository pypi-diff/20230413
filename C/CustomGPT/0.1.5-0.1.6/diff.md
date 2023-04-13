# Comparing `tmp/CustomGPT-0.1.5.tar.gz` & `tmp/CustomGPT-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CustomGPT-0.1.5.tar", last modified: Thu Apr 13 14:24:04 2023, max compression
+gzip compressed data, was "CustomGPT-0.1.6.tar", last modified: Thu Apr 13 15:32:41 2023, max compression
```

## Comparing `CustomGPT-0.1.5.tar` & `CustomGPT-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 lymengnaret   (501) staff       (20)        0 2023-04-13 14:24:04.588225 CustomGPT-0.1.5/
-drwxr-xr-x   0 lymengnaret   (501) staff       (20)        0 2023-04-13 14:24:04.587735 CustomGPT-0.1.5/CustomGPT.egg-info/
--rw-r--r--   0 lymengnaret   (501) staff       (20)      762 2023-04-13 14:24:04.000000 CustomGPT-0.1.5/CustomGPT.egg-info/PKG-INFO
--rw-r--r--   0 lymengnaret   (501) staff       (20)      224 2023-04-13 14:24:04.000000 CustomGPT-0.1.5/CustomGPT.egg-info/SOURCES.txt
--rw-r--r--   0 lymengnaret   (501) staff       (20)        1 2023-04-13 14:24:04.000000 CustomGPT-0.1.5/CustomGPT.egg-info/dependency_links.txt
--rw-r--r--   0 lymengnaret   (501) staff       (20)       38 2023-04-13 14:24:04.000000 CustomGPT-0.1.5/CustomGPT.egg-info/requires.txt
--rw-r--r--   0 lymengnaret   (501) staff       (20)        4 2023-04-13 14:24:04.000000 CustomGPT-0.1.5/CustomGPT.egg-info/top_level.txt
--rw-r--r--   0 lymengnaret   (501) staff       (20)     1063 2023-04-11 20:33:34.000000 CustomGPT-0.1.5/LICENSE
--rw-r--r--   0 lymengnaret   (501) staff       (20)      762 2023-04-13 14:24:04.588108 CustomGPT-0.1.5/PKG-INFO
--rw-r--r--   0 lymengnaret   (501) staff       (20)      957 2023-04-13 14:20:31.000000 CustomGPT-0.1.5/README.md
--rw-r--r--   0 lymengnaret   (501) staff       (20)       38 2023-04-13 14:24:04.588262 CustomGPT-0.1.5/setup.cfg
--rw-r--r--   0 lymengnaret   (501) staff       (20)      941 2023-04-13 14:23:56.000000 CustomGPT-0.1.5/setup.py
-drwxr-xr-x   0 lymengnaret   (501) staff       (20)        0 2023-04-13 14:24:04.587962 CustomGPT-0.1.5/src/
--rw-r--r--   0 lymengnaret   (501) staff       (20)       34 2023-04-13 14:20:31.000000 CustomGPT-0.1.5/src/__init__.py
--rw-r--r--   0 lymengnaret   (501) staff       (20)     4325 2023-04-13 14:20:31.000000 CustomGPT-0.1.5/src/custom_gpt.py
+drwxr-xr-x   0 lymengnaret   (501) staff       (20)        0 2023-04-13 15:32:41.776317 CustomGPT-0.1.6/
+drwxr-xr-x   0 lymengnaret   (501) staff       (20)        0 2023-04-13 15:32:41.775127 CustomGPT-0.1.6/CustomGPT/
+-rw-r--r--   0 lymengnaret   (501) staff       (20)       34 2023-04-13 15:21:03.000000 CustomGPT-0.1.6/CustomGPT/__init__.py
+-rw-r--r--   0 lymengnaret   (501) staff       (20)     5241 2023-04-13 15:29:59.000000 CustomGPT-0.1.6/CustomGPT/custom_gpt.py
+drwxr-xr-x   0 lymengnaret   (501) staff       (20)        0 2023-04-13 15:32:41.775951 CustomGPT-0.1.6/CustomGPT.egg-info/
+-rw-r--r--   0 lymengnaret   (501) staff       (20)      763 2023-04-13 15:32:41.000000 CustomGPT-0.1.6/CustomGPT.egg-info/PKG-INFO
+-rw-r--r--   0 lymengnaret   (501) staff       (20)      236 2023-04-13 15:32:41.000000 CustomGPT-0.1.6/CustomGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 lymengnaret   (501) staff       (20)        1 2023-04-13 15:32:41.000000 CustomGPT-0.1.6/CustomGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 lymengnaret   (501) staff       (20)       38 2023-04-13 15:32:41.000000 CustomGPT-0.1.6/CustomGPT.egg-info/requires.txt
+-rw-r--r--   0 lymengnaret   (501) staff       (20)       10 2023-04-13 15:32:41.000000 CustomGPT-0.1.6/CustomGPT.egg-info/top_level.txt
+-rw-r--r--   0 lymengnaret   (501) staff       (20)     1063 2023-04-11 20:33:34.000000 CustomGPT-0.1.6/LICENSE
+-rw-r--r--   0 lymengnaret   (501) staff       (20)      763 2023-04-13 15:32:41.776190 CustomGPT-0.1.6/PKG-INFO
+-rw-r--r--   0 lymengnaret   (501) staff       (20)     1029 2023-04-13 15:26:03.000000 CustomGPT-0.1.6/README.md
+-rw-r--r--   0 lymengnaret   (501) staff       (20)       38 2023-04-13 15:32:41.776362 CustomGPT-0.1.6/setup.cfg
+-rw-r--r--   0 lymengnaret   (501) staff       (20)      942 2023-04-13 15:30:29.000000 CustomGPT-0.1.6/setup.py
```

### Comparing `CustomGPT-0.1.5/CustomGPT.egg-info/PKG-INFO` & `CustomGPT-0.1.6/CustomGPT.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: CustomGPT
-Version: 0.1.5
-Summary: A custom GPT package for interacting with GPT-4 models without using the OpenAI API.
+Version: 0.1.6
+Summary: A package for interacting with GPT-4 models (and older) without using the OpenAI API.
 Home-page: https://github.com/NLmeng/CustomGPT
 Author: Lymeng Naret
 Author-email: lymengnaret@yahoo.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CustomGPT-0.1.5/LICENSE` & `CustomGPT-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `CustomGPT-0.1.5/PKG-INFO` & `CustomGPT-0.1.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: CustomGPT
-Version: 0.1.5
-Summary: A custom GPT package for interacting with GPT-4 models without using the OpenAI API.
+Version: 0.1.6
+Summary: A package for interacting with GPT-4 models (and older) without using the OpenAI API.
 Home-page: https://github.com/NLmeng/CustomGPT
 Author: Lymeng Naret
 Author-email: lymengnaret@yahoo.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CustomGPT-0.1.5/README.md` & `CustomGPT-0.1.6/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # CustomGPT
 
 This project provides GPT-Plus subscribers the ability to use their GPT-4 in python without having access to GPT-4's API. It provides a class that substitute the actual API; it will essentially use https://chat.openai.com/chat in the background. This also supports the usage of older versions of GPT, this way you don't have to pay for the openai-API usage or wait for the API's waitlist.
 
-### .env setup
-(NOTE: You need a subscription to GPT-Plus to use "gpt-4", otherwise you can use "text-davinci-003")
+## .env setup
+(NOTE: You need a subscription to GPT-Plus to use "gpt-4", otherwise you can use "text-davinci-002-render-sha" (default 3.5), or "text-davinci-002-render-paid" (legacy 3.5))
 - go to https://chat.openai.com/chat
 - inspect the website
 - go to application tab
 - locate `Cookies` then locate the `https://chat.openai.com` tab under it
 - copy the value of _puid (this is for `_PUID` in `.env`)
 - go to network tab
 - locate `Fetch/XHR`
```

### Comparing `CustomGPT-0.1.5/setup.py` & `CustomGPT-0.1.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 setup(
     name="CustomGPT",
-    version="0.1.5",
-    description="A custom GPT package for interacting with GPT-4 models without using the OpenAI API.",
+    version="0.1.6",
+    description="A package for interacting with GPT-4 models (and older) without using the OpenAI API.",
     author="Lymeng Naret",
     author_email="lymengnaret@yahoo.com",
     url="https://github.com/NLmeng/CustomGPT",
     packages=find_packages(),
     install_requires=[
         "requests==2.28.2",
         "python-dotenv==1.0.0",
```

### Comparing `CustomGPT-0.1.5/src/custom_gpt.py` & `CustomGPT-0.1.6/CustomGPT/custom_gpt.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,23 +4,31 @@
 import os
 from dotenv import load_dotenv
 
 load_dotenv()
 
 class CustomGPT:
     """
-    A Python class for interacting with GPT-4 models using the OpenAI API.
+    A Python class for interacting with GPT-4 models without using the OpenAI API.
 
     :param model: The model to use for generating the response
-    :type model: str, e.g. "gpt-4", "text-davinci-003", "text-davinci-002", ...
+    :type model: str, e.g. "gpt-4", "text-davinci-002-render-sha", "text-davinci-002-render-paid", ...
+
+    If you are having trouble setting up the .env, please refer to the README.md file, or use .help():
 
     EXAMPLE USAGE:
+
     if __name__ == "__main__":
-        gpt = CustomGPT()
-        session = gpt.start_new_chat()
+    
+        gpt = CustomGPT().start_new_chat()
+
+    ""  getting help with .env:  ""
+
+        gpt = CustomGPT().help()
+
     """
 
     def __init__(self, model="gpt-4"):
         # Initialize the class with the specified GPT model (default is "gpt-4")
         self.model = model
         self.session = requests.Session()
         self.session.headers.update({
@@ -50,14 +58,15 @@
                 "action": "next",
                 "messages": [],
                 "parent_message_id": self.prev_id,
             },
         )
         filtered_data = self.filter_response(res)
 
+        print("Chat has started successfully with model " + self.model + "\nType 'exit' to exit the chat.")
         while True:
             user_input = input("> ")
             if user_input.lower() == "exit":
                 break
             response = self.chat(user_input, filtered_data)
             print(response['message']['content']['parts'][0])
             filtered_data = response
@@ -119,8 +128,19 @@
         :param res: The raw API response
         :type res: requests.Response
         :return: The filtered API response as a dictionary
         """
         non_mt_res = os.linesep.join([txt for txt in res.text.splitlines() if txt])
         data = non_mt_res.splitlines()[len(non_mt_res.splitlines()) - 2]
         filtered_data = json.loads(data[data.find("data: ") + 6:])
-        return filtered_data
+        return filtered_data
+    
+    def help(self):
+        print("- go to https://chat.openai.com/chat")
+        print("- inspect the website")
+        print("- go to application tab")
+        print("- locate `Cookies` then locate the `https://chat.openai.com` tab under it")
+        print("- copy the value of _puid (this is for `_PUID` in `.env`)")
+        print("- go to network tab")
+        print("- locate `Fetch/XHR`")
+        print("- refresh the page and locate `models` then locate `authorization` under `Headers`")
+        print("- copy the value of the `authorization` (don't copy Bearer) (this is for `OPENAI_API_KEY` in .env)")
```

