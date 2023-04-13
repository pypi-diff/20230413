# Comparing `tmp/log10_io-0.0.1.tar.gz` & `tmp/log10_io-0.0.3.tar.gz`

## Comparing `log10_io-0.0.1.tar` & `log10_io-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,16 @@
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 log10_io-0.0.1/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 log10_io-0.0.1/log10/        __init__.py
--rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 log10_io-0.0.1/log10/load.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 log10_io-0.0.1/tests/test_chatcompletion.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 log10_io-0.0.1/tests/test_completion.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 log10_io-0.0.1/tests/test_langchain.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 log10_io-0.0.1/LICENSE
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 log10_io-0.0.1/README.md
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 log10_io-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 log10_io-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 log10_io-0.0.3/setup.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 log10_io-0.0.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 log10_io-0.0.3/log10/        __init__.py
+-rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 log10_io-0.0.3/log10/load.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 log10_io-0.0.3/tests/test_chatcompletion.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 log10_io-0.0.3/tests/test_completion.py
+-rw-r--r--   0        0        0    10777 2020-02-02 00:00:00.000000 log10_io-0.0.3/tests/test_langchain_babyagi.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 log10_io-0.0.3/tests/test_langchain_multiple_tools.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 log10_io-0.0.3/tests/test_langchain_simple_sequential.py
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 log10_io-0.0.3/tests/test_langchain_sqlagent.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 log10_io-0.0.3/tests/test_multiple_sessions.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 log10_io-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 log10_io-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 log10_io-0.0.3/README.md
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 log10_io-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 log10_io-0.0.3/PKG-INFO
```

### Comparing `log10_io-0.0.1/log10/load.py` & `log10_io-0.0.3/log10/load.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,23 @@
         raise Exception("Failed to create LOG10 session: " + str(e))
 
 
 # Global variable to store the current sessionID.
 sessionID = get_session_id()
 
 
+class log10_session:
+    def __enter__(self):
+        global sessionID
+        sessionID = get_session_id()
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        return
+
+
 def intercepting_decorator(func):
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         completion_url = url + "/api/completions"
         output = None
 
         try:
```

### Comparing `log10_io-0.0.1/tests/test_langchain.py` & `log10_io-0.0.3/tests/test_langchain_simple_sequential.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import os
 from log10.load import log10
 import openai
 
 log10(openai)
 
 openai.api_key = os.getenv("OPENAI_API_KEY")
-MAX_TOKENS = 512
 
 from langchain.llms import OpenAI
 from langchain.prompts import PromptTemplate
 from langchain.chains import LLMChain, SimpleSequentialChain
 
-llm = OpenAI(temperature=0.9, model_name="text-ada-001")
+llm = OpenAI(temperature=0.9, model_name="text-babbage-001")
 prompt = PromptTemplate(
     input_variables=["product"],
     template="What is a good name for a company that makes {product}?",
 )
 
 chain = LLMChain(llm=llm, prompt=prompt)
-print(chain.run("colorful socks"))
 
 second_prompt = PromptTemplate(
     input_variables=["company_name"],
     template="Write a catchphrase for the following company: {company_name}",
 )
 chain_two = LLMChain(llm=llm, prompt=second_prompt)
```

### Comparing `log10_io-0.0.1/LICENSE` & `log10_io-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.1/README.md` & `log10_io-0.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # log10
 
 ⚡ Unified LLM data management ⚡
 
 ## Quick Install
 
-`pip install -e git+https://github.com/log10-io/log10.git#egg=log10`
+`pip install log10-io`
 
 ## 🤔 What is this?
 
 A one-line Python integration to manage your LLM data.
 
 ```python
 import openai
```

### Comparing `log10_io-0.0.1/pyproject.toml` & `log10_io-0.0.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "log10-io"
-version = "0.0.1"
-authors = [
-  { name="Niklas Nielsen", email="niklas@quarfotprice.com" },
-  { name="Arjun Bansal", email="mindscience@gmail.com" },
-]
+version = "0.0.3"
+authors = []
+license = "MIT"
 description = "Unified LLM data management"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `log10_io-0.0.1/PKG-INFO` & `log10_io-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: log10-io
-Version: 0.0.1
+Version: 0.0.3
 Summary: Unified LLM data management
 Project-URL: Homepage, https://github.com/log10-io/log10
 Project-URL: Bug Tracker, https://github.com/log10-io/log10/issues
-Author-email: Niklas Nielsen <niklas@quarfotprice.com>, Arjun Bansal <mindscience@gmail.com>
+License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # log10
 
 ⚡ Unified LLM data management ⚡
 
 ## Quick Install
 
-`pip install -e git+https://github.com/log10-io/log10.git#egg=log10`
+`pip install log10-io`
 
 ## 🤔 What is this?
 
 A one-line Python integration to manage your LLM data.
 
 ```python
 import openai
```

