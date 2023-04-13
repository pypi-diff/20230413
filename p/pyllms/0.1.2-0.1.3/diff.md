# Comparing `tmp/pyllms-0.1.2.tar.gz` & `tmp/pyllms-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyllms-0.1.2.tar", last modified: Mon Apr 10 19:41:55 2023, max compression
+gzip compressed data, was "pyllms-0.1.3.tar", last modified: Thu Apr 13 02:50:24 2023, max compression
```

## Comparing `pyllms-0.1.2.tar` & `pyllms-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-10 19:41:55.712215 pyllms-0.1.2/
--rw-r--r--   0 prelovac   (502) staff       (20)     1068 2023-04-10 01:29:26.000000 pyllms-0.1.2/LICENSE
--rw-r--r--   0 prelovac   (502) staff       (20)    11447 2023-04-10 19:41:55.711900 pyllms-0.1.2/PKG-INFO
--rw-r--r--   0 prelovac   (502) staff       (20)    10284 2023-04-10 19:32:25.000000 pyllms-0.1.2/README.md
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-10 19:41:55.709494 pyllms-0.1.2/llms/
--rw-r--r--   0 prelovac   (502) staff       (20)       83 2023-04-09 22:07:03.000000 pyllms-0.1.2/llms/__init__.py
--rw-r--r--   0 prelovac   (502) staff       (20)    14766 2023-04-10 19:11:55.000000 pyllms-0.1.2/llms/llms.py
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-10 19:41:55.710433 pyllms-0.1.2/llms/providers/
--rw-r--r--   0 prelovac   (502) staff       (20)      107 2023-04-09 20:11:29.000000 pyllms-0.1.2/llms/providers/__init__.py
--rw-r--r--   0 prelovac   (502) staff       (20)     1631 2023-04-10 19:09:27.000000 pyllms-0.1.2/llms/providers/ai21.py
--rw-r--r--   0 prelovac   (502) staff       (20)     2003 2023-04-10 19:08:51.000000 pyllms-0.1.2/llms/providers/anthropic.py
--rw-r--r--   0 prelovac   (502) staff       (20)     1803 2023-04-10 19:09:11.000000 pyllms-0.1.2/llms/providers/openai.py
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-10 19:41:55.711571 pyllms-0.1.2/pyllms.egg-info/
--rw-r--r--   0 prelovac   (502) staff       (20)    11447 2023-04-10 19:41:55.000000 pyllms-0.1.2/pyllms.egg-info/PKG-INFO
--rw-r--r--   0 prelovac   (502) staff       (20)      308 2023-04-10 19:41:55.000000 pyllms-0.1.2/pyllms.egg-info/SOURCES.txt
--rw-r--r--   0 prelovac   (502) staff       (20)        1 2023-04-10 19:41:55.000000 pyllms-0.1.2/pyllms.egg-info/dependency_links.txt
--rw-r--r--   0 prelovac   (502) staff       (20)       60 2023-04-10 19:41:55.000000 pyllms-0.1.2/pyllms.egg-info/requires.txt
--rw-r--r--   0 prelovac   (502) staff       (20)        5 2023-04-10 19:41:55.000000 pyllms-0.1.2/pyllms.egg-info/top_level.txt
--rw-r--r--   0 prelovac   (502) staff       (20)       38 2023-04-10 19:41:55.712294 pyllms-0.1.2/setup.cfg
--rw-r--r--   0 prelovac   (502) staff       (20)     1682 2023-04-10 19:41:51.000000 pyllms-0.1.2/setup.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-13 02:50:24.089695 pyllms-0.1.3/
+-rw-r--r--   0 prelovac   (502) staff       (20)     1068 2023-04-10 01:29:26.000000 pyllms-0.1.3/LICENSE
+-rw-r--r--   0 prelovac   (502) staff       (20)    12096 2023-04-13 02:50:24.089385 pyllms-0.1.3/PKG-INFO
+-rw-r--r--   0 prelovac   (502) staff       (20)    10933 2023-04-13 02:43:49.000000 pyllms-0.1.3/README.md
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-13 02:50:24.086948 pyllms-0.1.3/llms/
+-rw-r--r--   0 prelovac   (502) staff       (20)      295 2023-04-13 02:24:28.000000 pyllms-0.1.3/llms/__init__.py
+-rw-r--r--   0 prelovac   (502) staff       (20)    16270 2023-04-13 02:48:48.000000 pyllms-0.1.3/llms/llms.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-13 02:50:24.087978 pyllms-0.1.3/llms/providers/
+-rw-r--r--   0 prelovac   (502) staff       (20)      107 2023-04-09 20:11:29.000000 pyllms-0.1.3/llms/providers/__init__.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     2397 2023-04-13 02:27:57.000000 pyllms-0.1.3/llms/providers/ai21.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     2756 2023-04-13 02:27:53.000000 pyllms-0.1.3/llms/providers/anthropic.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     2421 2023-04-13 02:28:08.000000 pyllms-0.1.3/llms/providers/openai.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-13 02:50:24.089054 pyllms-0.1.3/pyllms.egg-info/
+-rw-r--r--   0 prelovac   (502) staff       (20)    12096 2023-04-13 02:50:24.000000 pyllms-0.1.3/pyllms.egg-info/PKG-INFO
+-rw-r--r--   0 prelovac   (502) staff       (20)      308 2023-04-13 02:50:24.000000 pyllms-0.1.3/pyllms.egg-info/SOURCES.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)        1 2023-04-13 02:50:24.000000 pyllms-0.1.3/pyllms.egg-info/dependency_links.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)       60 2023-04-13 02:50:24.000000 pyllms-0.1.3/pyllms.egg-info/requires.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)        5 2023-04-13 02:50:24.000000 pyllms-0.1.3/pyllms.egg-info/top_level.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)       38 2023-04-13 02:50:24.089774 pyllms-0.1.3/setup.cfg
+-rw-r--r--   0 prelovac   (502) staff       (20)     1682 2023-04-13 02:49:56.000000 pyllms-0.1.3/setup.py
```

### Comparing `pyllms-0.1.2/LICENSE` & `pyllms-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyllms-0.1.2/PKG-INFO` & `pyllms-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyllms
-Version: 0.1.2
+Version: 0.1.3
 Summary: A brief description of your package
 Author: Vladimir Prelovac
 Author-email: vlad@kagi.com
 Project-URL: Documentation, https://github.com/kagisearch/pyllms
 Project-URL: Source Code, https://github.com/kagisearch/pyllms
 Project-URL: Issue Tracker, https://github.com/kagisearch/pyllms/issues
 Keywords: llm,llms,large language model,AI,NLP,natural language processing,gpt,chatgpt,openai,anthropic,ai21
@@ -38,80 +38,92 @@
 
 
 ## Usage
 
 
 ```
 import llms
+
 model = llms.init()
 result = model.complete("what is 5+5")
+
 print(result.text)  
 
 ```
 
-llms will read the API key from environment variables, which you can set like this:
+Library will attempt to read the API keys and the default model from environment variables, which you can set like this:
 
 ```
 export OPENAI_API_KEY="your_api_key_here"
 export ANTHROPIC_API_KEY="your_api_key_here"
 export AI21_API_KEY="your_api_key_here"
+
 export LLMS_DEFAULT_MODEL="gpt-3.5-turbo"
 ```
 
 
 Alternatively, you can pass initialization values to the init() method:
 
 ```
 model=llms.init(openai_api_key='your_api_key_here', model='gpt-4')
 ```
 
 
-You can also pass optional parameters to the complete method. Any parameters accepted by the original model are supported automatically, in the verbatim form:
+You can also pass optional parameters to the complete method. 'temperature' and 'max_tokens' are standardized across all APIs and get converted to the corresponding API params. 
+
+Any other parameters accepted by the original model are supported in their verbatim form.
 
 ```
 result = model.complete(
     "what is the capital of country where mozzart was born",
     temperature=0.1,
+    max_tokens=200
 )
 ```
 
-By default, temperature for all models is set to 0.
+Note: By default, temperature for all models is set to 0, and max_tokens to 300.
 
-The result will also contain helpful information like tokens used, cost (which is automatically calculated using current pricing), and result latency:
+The result will also contain helpful information like tokens used, cost (which is automatically calculated using current pricing), and response latency in the 'meta' field:
 ```
 >>> print(result.meta)
 {'model': 'gpt-3.5-turbo', 'tokens': 15, 'tokens_prompt': 14, 'tokens_completion': 1, 'cost': 3e-05, 'latency': 0.48232388496398926}
 ```
 
 
 
 
-
-
-
-
 ## Multi-model usage
 
-You can initialize multiple models at once, which is very useful for testing and comparing output of different models. All models will run in parallel to save time. 
+You can also initialize multiple models at once! This is very useful for testing and comparing output of different models in parallel. 
 
 ```
 >>> models=llms.init(model=['gpt-3.5-turbo','claude-instant-v1'])
 >>> result=models.complete('what is the capital of country where mozzart was born')
 >>> print(result.text)
 ['The capital of the country where Mozart was born is Vienna, Austria.', 'Wolfgang Amadeus Mozart was born in Salzburg, Austria.\n\nSo the capital of the country where Mozart was born is Vienna, Austria.']
 
 >>> print(result.meta)
 [{'model': 'gpt-3.5-turbo', 'tokens': 34, 'tokens_prompt': 20, 'tokens_completion': 14, 'cost': 6.8e-05, 'latency': 0.7097790241241455}, {'model': 'claude-instant-v1', 'tokens': 54, 'tokens_prompt': 20, 'tokens_completion': 34, 'cost': 5.79e-05, 'latency': 0.7291600704193115}]
 ```
 
+
 ## Benchmarks
 
+Models are appearing like mushrooms after rain and we are interested in:
+
+1) Quality
+2) Speed
+3) Cost
+
+We included an automated benchmark system. The quality is evaluated using a powerful model (for example gpt-4) on a range of predefined questions, or you can supply your own.
+
+
 ```
-models=llms.init(model=['gpt-3.5-turbo', 'claude-instant-v1'])
-gpt4=llms.init('gpt-4')
+models=llms.init(model=['gpt-3.5-turbo', 'claude-instant-v1', 'j2-jumbo-instruct'])
+gpt4=llms.init('gpt-4') # optional, evaluator can be ommited and in this case only speed and cost is evaluated
 models.benchmark(evaluator=gpt4)
 ```
 
 ```
 +---------------------------------------+--------------------+---------------------+-----------------------+---------------------------+-----------------+
 |                 Model                 |       Tokens       |       Cost ($)      |      Latency (s)      |     Speed (tokens/sec)    |    Evaluation   |
 +---------------------------------------+--------------------+---------------------+-----------------------+---------------------------+-----------------+
@@ -150,17 +162,18 @@
 |    AI21Provider (j2-jumbo-instruct)   |        218         |       0.00327       |          5.90         |           36.95           |        1        |
 |    AI21Provider (j2-jumbo-instruct)   |        281         |       0.00421       |          6.25         |           44.97           |        1        |
 |    AI21Provider (j2-jumbo-instruct)   |        149         |       0.00224       |          1.56         |           95.81           |        10       |
 |    AI21Provider (j2-jumbo-instruct)   | Total Tokens: 1838 | Total Cost: 0.02757 |  Median Latency: 5.62 |  Aggregrated speed: 40.01 | Total Score: 68 |
 +---------------------------------------+--------------------+---------------------+-----------------------+---------------------------+-----------------+
 ```
 
-In addition, you can evaluate models on your own prompts:
+To evaluate models on your own prompts, simply pass a list of questions. The evaluator will automatically evaluate the responses:
+
 ```
-models.benchmark(prompts=["what is the capital of finland", "who won superbowl in the year justin bieber was born"],evaluator=gpt4)
+models.benchmark(prompts=["what is the capital of finland", "who won superbowl in the year justin bieber was born"], evaluator=gpt4)
 ```
 
 ## Supported Models
 
 To get a list of supported models, call list(). Models will be shown in the order of least expensive to most expensive.
 
 ```
```

### Comparing `pyllms-0.1.2/README.md` & `pyllms-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,80 +12,92 @@
 
 
 ## Usage
 
 
 ```
 import llms
+
 model = llms.init()
 result = model.complete("what is 5+5")
+
 print(result.text)  
 
 ```
 
-llms will read the API key from environment variables, which you can set like this:
+Library will attempt to read the API keys and the default model from environment variables, which you can set like this:
 
 ```
 export OPENAI_API_KEY="your_api_key_here"
 export ANTHROPIC_API_KEY="your_api_key_here"
 export AI21_API_KEY="your_api_key_here"
+
 export LLMS_DEFAULT_MODEL="gpt-3.5-turbo"
 ```
 
 
 Alternatively, you can pass initialization values to the init() method:
 
 ```
 model=llms.init(openai_api_key='your_api_key_here', model='gpt-4')
 ```
 
 
-You can also pass optional parameters to the complete method. Any parameters accepted by the original model are supported automatically, in the verbatim form:
+You can also pass optional parameters to the complete method. 'temperature' and 'max_tokens' are standardized across all APIs and get converted to the corresponding API params. 
+
+Any other parameters accepted by the original model are supported in their verbatim form.
 
 ```
 result = model.complete(
     "what is the capital of country where mozzart was born",
     temperature=0.1,
+    max_tokens=200
 )
 ```
 
-By default, temperature for all models is set to 0.
+Note: By default, temperature for all models is set to 0, and max_tokens to 300.
 
-The result will also contain helpful information like tokens used, cost (which is automatically calculated using current pricing), and result latency:
+The result will also contain helpful information like tokens used, cost (which is automatically calculated using current pricing), and response latency in the 'meta' field:
 ```
 >>> print(result.meta)
 {'model': 'gpt-3.5-turbo', 'tokens': 15, 'tokens_prompt': 14, 'tokens_completion': 1, 'cost': 3e-05, 'latency': 0.48232388496398926}
 ```
 
 
 
 
-
-
-
-
 ## Multi-model usage
 
-You can initialize multiple models at once, which is very useful for testing and comparing output of different models. All models will run in parallel to save time. 
+You can also initialize multiple models at once! This is very useful for testing and comparing output of different models in parallel. 
 
 ```
 >>> models=llms.init(model=['gpt-3.5-turbo','claude-instant-v1'])
 >>> result=models.complete('what is the capital of country where mozzart was born')
 >>> print(result.text)
 ['The capital of the country where Mozart was born is Vienna, Austria.', 'Wolfgang Amadeus Mozart was born in Salzburg, Austria.\n\nSo the capital of the country where Mozart was born is Vienna, Austria.']
 
 >>> print(result.meta)
 [{'model': 'gpt-3.5-turbo', 'tokens': 34, 'tokens_prompt': 20, 'tokens_completion': 14, 'cost': 6.8e-05, 'latency': 0.7097790241241455}, {'model': 'claude-instant-v1', 'tokens': 54, 'tokens_prompt': 20, 'tokens_completion': 34, 'cost': 5.79e-05, 'latency': 0.7291600704193115}]
 ```
 
+
 ## Benchmarks
 
+Models are appearing like mushrooms after rain and we are interested in:
+
+1) Quality
+2) Speed
+3) Cost
+
+We included an automated benchmark system. The quality is evaluated using a powerful model (for example gpt-4) on a range of predefined questions, or you can supply your own.
+
+
 ```
-models=llms.init(model=['gpt-3.5-turbo', 'claude-instant-v1'])
-gpt4=llms.init('gpt-4')
+models=llms.init(model=['gpt-3.5-turbo', 'claude-instant-v1', 'j2-jumbo-instruct'])
+gpt4=llms.init('gpt-4') # optional, evaluator can be ommited and in this case only speed and cost is evaluated
 models.benchmark(evaluator=gpt4)
 ```
 
 ```
 +---------------------------------------+--------------------+---------------------+-----------------------+---------------------------+-----------------+
 |                 Model                 |       Tokens       |       Cost ($)      |      Latency (s)      |     Speed (tokens/sec)    |    Evaluation   |
 +---------------------------------------+--------------------+---------------------+-----------------------+---------------------------+-----------------+
@@ -124,17 +136,18 @@
 |    AI21Provider (j2-jumbo-instruct)   |        218         |       0.00327       |          5.90         |           36.95           |        1        |
 |    AI21Provider (j2-jumbo-instruct)   |        281         |       0.00421       |          6.25         |           44.97           |        1        |
 |    AI21Provider (j2-jumbo-instruct)   |        149         |       0.00224       |          1.56         |           95.81           |        10       |
 |    AI21Provider (j2-jumbo-instruct)   | Total Tokens: 1838 | Total Cost: 0.02757 |  Median Latency: 5.62 |  Aggregrated speed: 40.01 | Total Score: 68 |
 +---------------------------------------+--------------------+---------------------+-----------------------+---------------------------+-----------------+
 ```
 
-In addition, you can evaluate models on your own prompts:
+To evaluate models on your own prompts, simply pass a list of questions. The evaluator will automatically evaluate the responses:
+
 ```
-models.benchmark(prompts=["what is the capital of finland", "who won superbowl in the year justin bieber was born"],evaluator=gpt4)
+models.benchmark(prompts=["what is the capital of finland", "who won superbowl in the year justin bieber was born"], evaluator=gpt4)
 ```
 
 ## Supported Models
 
 To get a list of supported models, call list(). Models will be shown in the order of least expensive to most expensive.
 
 ```
```

### Comparing `pyllms-0.1.2/llms/llms.py` & `pyllms-0.1.3/llms/llms.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         return [result["meta"] for result in self._results]
 
 
 class LLMS:
     def __init__(
         self, model=None, openai_api_key=None, anthropic_api_key=None, ai21_api_key=None
     ):
+
         if openai_api_key is None:
             openai_api_key = os.getenv("OPENAI_API_KEY")
 
         if anthropic_api_key is None:
             anthropic_api_key = os.getenv("ANTHROPIC_API_KEY")
 
         if ai21_api_key is None:
@@ -51,18 +52,15 @@
             else:
                 model = [model]
         elif isinstance(model, str):
             model = [model]
 
         self._providers = []
         for single_model in model:
-            if (
-                openai_api_key is not None
-                and single_model in OpenAIProvider.MODEL_INFO
-            ):
+            if openai_api_key is not None and single_model in OpenAIProvider.MODEL_INFO:
                 self._providers.append(
                     OpenAIProvider(api_key=openai_api_key, model=single_model)
                 )
             elif (
                 anthropic_api_key is not None
                 and single_model in AnthropicProvider.MODEL_INFO
             ):
@@ -96,17 +94,25 @@
                 model_info_list.append(model_info)
 
         sorted_list = sorted(
             model_info_list, key=lambda x: x["cost"]["prompt"] + x["cost"]["completion"]
         )
         return sorted_list
 
-    def complete(self, prompt, **kwargs):
+    def complete(self, prompt, history=None, **kwargs):
         def _generate(provider):
-            response = provider.complete(prompt, **kwargs)
+           
+            response = provider.complete(prompt, history, **kwargs)
+            
+            formatted_cost = format(response["meta"]["cost"], '.5f')
+            formatted_latency = round(response["meta"]["latency"], 2)
+            
+            response["meta"]["cost"] = formatted_cost
+            response["meta"]["latency"] = formatted_latency
+
             return {
                 "text": response["text"],
                 "meta": response["meta"],
                 "provider": provider,
             }
 
         results = []
@@ -117,82 +123,79 @@
             }
             for future in as_completed(futures):
                 results.append(future.result())
 
         return Result(results)
 
     def benchmark(self, prompts=None, evaluator=None, show_outputs=False, html=False):
-        
         if not prompts:
             prompts = [
                 "What is the capital of the country where Christopher Columbus was born?",
                 "A glass door has ‘push’ written on it in mirror writing. Should you push or pull it and why?",
-                "Explain the process of photosynthesis in plants, including the role of chlorophyll and the importance of light. Discuss the main outcomes of photosynthesis and why it is essential for life on Earth.",
-                "Solve The Two Door Riddle: You are in a room with two doors. One door leads to certain death, and the other leads to freedom. There are two guards, one in front of each door. One guard always tells the truth, and the other guard always lies. You can only ask one question to one guard to determine which door leads to freedom. What question should you ask?",
                 "Solve the quadratic equation: x^2 - 5x + 6 = 0",
-                "How much is 7! + 7? Describe steps you took.",
-                "Describe the differences between depth-first search (DFS) and breadth-first search (BFS) algorithms in graph traversal, and provide an example use case for each of them.",
-                "Write a Python function that takes a string of text as input and returns a dictionary containing the frequency of each word in the text. Discuss the time complexity of your solution and any possible improvements to optimize its performance.",
-                "Write a Python function that takes a list of integers as input, finds the two numbers with the largest product, and returns their product. Also, provide a brief explanation of the logic behind your solution.",
-                "You are given a string containing a sequence of ASCII characters. Your task is to write a JavaScript function that compresses the string by replacing consecutive occurrences of the same character with the character followed by the number of times it appears consecutively. Then, write a JavaScript function to decompress the compressed string back to its original form. The input string only contains printable ASCII characters. For example, if the input string is 'aaabccddd', the compressed string should be 'a3b1c2d3'. The decompressed string should be the same as the input string.",
+                "How much is 7! * 3! -1234.5 ?",
+                'translate this sentence by alternating words in gemran and french "it was a beautiful day that thursday and I want skiing outside. it started raining soon although they said it won\'t be until friday, so I went to the pool instead"',
+                "Convert December 21 · 1:00 – 1:50pm pacific to asia/taipei time",
+                "In my kitchen there's a table with a cup with a ball inside. I moved the cup to my bed in my bedroom and turned the cup upside down. I grabbed the cup again and moved to the main room. Where's the ball now?",
+                'Capture the essence of this in exactly 7 words: "There’s much that divides us in Northern Ireland though one thing is guaranteed to bring us together: local phrases. Call it slang, call it colloquialisms, we all know only too well how important words are to where we’re from . . . and when it comes to the phrases that make us ‘us,’ we’ve got a lot to say. While you don’t need advance knowledge of the words to fit in, well, it helps. How else will you know where ‘foundered’ sits on the scale of warm to freezing? Or deciding whether that new car purchase is more ‘clinker’ than ‘beezer’? Or appreciating that ‘grand’ can mean exactly that or anything but? If the best way to get to know a nation is to understand their language, then surely tourists must be at times confused about what comes out of our mouths. Throughout the island of Ireland, we have utterly brilliant ways to verbally express ourselves.“I think it’s really important,” says Dr Frank Ferguson, research director for English Language and Literature at Ulster University, about the vitality of slang as part of language."',
+                "Write a Python function that takes a list of integers as input and returns the length of the longest increasing subsequence. An increasing subsequence is a subsequence of the given list where the elements are in strictly increasing order. Your function should have an efficient solution with a time complexity better than O(n^2), where n is the length of the input list. Output only code with no explainations and provide example usage.",
+                "Write a Python function that takes a list of integers as input and returns the maximum sum of non-adjacent elements in the list. The function should return 0 if the input list is empty. Your function should have an efficient solution with a time complexity of O(n), where n is the length of the input list. Output only code with no explainations and provide example usage.",
+                "You are given a 2D binary matrix filled with 0's and 1's. Your task is to write a JavaScript function that finds the largest rectangle containing only 1's and returns its area. Your function should have an efficient solution with a time complexity better than O(n^3), where n is the total number of elements in the input matrix. Output only code with no explainations and provide example usage.",
                 "Given the following messy and unstructured data, extract the names, email addresses, and phone numbers of the individuals listed:\
-    \
-    John Doe - johndoe@email.com (555) 123-4567\
-    random text 1\
-    Jane Smith\
-    random text 2, 555-\
-    987-6543\
-    janesmith@email.com\
-    random text 3\
-    Bob Johnson - bob.johnson@email.com\
-    random text 4 area code 555 phone: 111-2222\
-    ",
+John Doe - johndoe (at) email.com (five-five-five) one-two-three-four-five-six-seven\
+random text not a phone 123 4468888\
+Jane Smith\
+random text 2, cinque-cinque-cinque-\
+nove-otto-sette-sei-quattro-tre\
+janesmith en email punto com\
+texto aleatorio 3\
+Bob Johnson - first name dot last name dot wild🐻@email.com\
+texto aleatorio 4 código de área five-five-five teléfono: eins-eins-eins-zwei-zwei-zwei-zwei",
             ]
 
         def evaluate_answers(
             evaluator, query_answer_pairs: List[Tuple[str, str]]
         ) -> List[int]:
-            system='''
+            system = """
             You are a truthful evaluator of the capabilties of other AI models.
 
-You are given a list of queries and answers by an AI model. For each query first think about  the solution yourself, then score the reply of the other AI, compared to yours on a scale 1 to 10 (10 being great).
+You are given a list of queries and answers by an AI model. For each query first think about  the solution yourself, then score the reply of the other AI, compared to yours on a scale 0 to 5 (5 being great).
 
 For example:
 
 Query: What is the capital of the country where Christopher Columbus was born?
 Answer: Christopher Columbus was born in Genoa, Italy.
 
 Query : A glass door has ‘push’ written on it in mirror writing. Should you push or pull it and why?
 Answer: You should push the door. The reason for this is that the mirror writing is intended for people on the other side of the door to read, not for you. So, if you push the door, you will be pushing it in the direction that the people on the other side are expecting it to move.
 
 
-Christopher Columbus was born in the Republic of Genoa, which is now part of Italy. The capital of Italy is Rome. So you would score it 3 (it is wrong answer, but city was correct)
-Since the word "push" is written in mirror writing, it suggests that the instruction is intended for people on the other side of the door. Therefore, you should pull the door to open it.
-You would score this 1 (it is wrong)
+Christopher Columbus was born in the Republic of Genoa, which is now part of Italy. The capital of Italy is Rome. So you would score it 1 (it is wrong answer, but city was correct)
+Since the word "push" is written in mirror writing, it suggests that the instruction is intended for people on the other side of the door. Therefore, you should pull the door to open it. You would score this 0 (it is wrong)
 
 
 Your only output should be a list of comma seperated integers representing your evaluation score for each answer. No other output is allowed. For example above your output will be:
-1, 3
+0, 1
 
-'''
-            #prompt = "Please evaluate the following answers on a scale of 1 to 10 (10 being the best):\n\n"
-            prompt=""
+"""
+            # prompt = "Please evaluate the following answers on a scale of 1 to 10 (10 being the best):\n\n"
+            prompt = ""
             for i, (query, answer) in enumerate(query_answer_pairs):
                 prompt += f"Query #{i + 1}: {query}\nAnswer #{i + 1}: {answer}\n\n"
-#            prompt += "Please provide a score for each answer as a list of integers separated by commas, with no additional text or explanation. For example: 6, 10, 10"
-            print(prompt)
+            #            prompt += "Please provide a score for each answer as a list of integers separated by commas, with no additional text or explanation. For example: 6, 10, 10"
+            #print(prompt)
             evaluator_result = evaluator.complete(prompt, system=system).text
-            print(evaluator_result)
+            #print(evaluator_result)
             scores = evaluator_result.split(",")
             return [int(score.strip()) for score in scores]
 
         model_results = {}
 
         def process_prompt(model, prompt, index):
-            print(model, index)
+            #print(model, index)
             result = model.complete(prompt)
             output_data = {
                 "text": result["text"],
                 "tokens": result["meta"]["tokens"],
                 "latency": result["meta"]["latency"],
                 "cost": result["meta"]["cost"],
                 "prompt_index": index,
```

### Comparing `pyllms-0.1.2/llms/providers/ai21.py` & `pyllms-0.1.3/llms/providers/ai21.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # llms/providers/anthropic.py
 
 import ai21
 import time
+import itertools
+from typing import List, Optional
 
 
 class AI21Provider:
     # per million tokens
     MODEL_INFO = {
         "j2-jumbo-instruct": {"prompt": 15.0, "completion": 15.0, "token_limit": 8192},
         "j2-grande-instruct": {"prompt": 10.0, "completion": 10.0, "token_limit": 8192},
@@ -16,18 +18,39 @@
         if model is None:
             model = "j2-grande-instruct"
         self.model = model
 
     def __str__(self):
         return f"{self.__class__.__name__} ({self.model})"
 
-    def complete(self, prompt, temperature=0, maxTokens=200, **kwargs):
+    def complete(self,
+                 prompt: str,
+                 history: Optional[List[tuple]] = None,
+                 temperature: float = 0,
+                 max_tokens: int = 300,
+                 **kwargs):
+
+        HUMAN_PROMPT = "\n\nHuman:"
+        AI_PROMPT = "\n\nAssistant:"
+
+        if history is not None:
+            role_cycle = itertools.cycle((HUMAN_PROMPT, AI_PROMPT))
+            history_messages = itertools.chain.from_iterable(history)
+            history_prompt = "".join(itertools.chain.from_iterable(zip(role_cycle, history_messages)))
+            prompt = f"{history_prompt}{prompt}"
+
+        maxTokens = max_tokens  # Assign max_tokens to maxTokens
+
+        if 'maxTokens' not in kwargs:
+            kwargs['maxTokens'] = maxTokens  # Add maxTokens to kwargs if not present
+
         start_time = time.time()
-        response = ai21.Completion.execute(model=self.model, prompt=prompt, temperature=temperature, maxTokens=maxTokens, **kwargs)
+        response = ai21.Completion.execute(model=self.model, prompt=prompt, temperature=temperature, **kwargs)
         latency = time.time() - start_time
+
         completion = response.completions[0].data.text.strip()
         prompt_tokens = len(response.prompt.tokens)
         completion_tokens = len(response.completions[0].data.tokens)
         total_tokens = prompt_tokens + completion_tokens
 
         cost_per_token = self.MODEL_INFO[self.model]
         cost = (prompt_tokens * cost_per_token["prompt"] / 1000000) + (
```

### Comparing `pyllms-0.1.2/llms/providers/anthropic.py` & `pyllms-0.1.3/llms/providers/openai.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,59 +1,71 @@
-# llms/providers/anthropic.py
-
-import os
-import anthropic
+import itertools
+import openai
 import time
+from typing import List, Optional
 
 
-class AnthropicProvider:
+class OpenAIProvider:
+    # cost is per million tokens
     MODEL_INFO = {
-        "claude-instant-v1": {"prompt": 0.43, "completion": 1.45, "token_limit": 8000},
-        "claude-v1": {"prompt": 2.9, "completion": 8.6, "token_limit": 8000},
+        "gpt-4": {"prompt": 30.0, "completion": 60.0, "token_limit": 8000},
+        "gpt-3.5-turbo": {"prompt": 2.0, "completion": 2.0, "token_limit": 4000},
     }
-    def __init__(self, api_key=None, model=None):
-        if api_key is None:
-            api_key = os.getenv("ANTHROPIC_API_KEY")
-        self.client = anthropic.Client(api_key)
 
+    def __init__(self, api_key, model=None):
+        openai.api_key = api_key
         if model is None:
-            model = "claude-instant-v1"
+            model = "gpt-3.5-turbo"
         self.model = model
 
     def __str__(self):
         return f"{self.__class__.__name__} ({self.model})"
 
-    def complete(self, prompt,temperature=0, max_tokens_to_sample=200, **kwargs):
-        formatted_prompt = f"{anthropic.HUMAN_PROMPT}{prompt}{anthropic.AI_PROMPT}"
+    def complete(self,
+                 prompt: str,
+                 history: Optional[List[tuple]] = None,
+                 system_message: str = None,
+                 temperature: float = 0,
+                 **kwargs):
         start_time = time.time()
-        response = self.client.completion(
-            prompt=formatted_prompt,
-            stop_sequences=[anthropic.HUMAN_PROMPT],
-            temperature=temperature, 
-            max_tokens_to_sample=max_tokens_to_sample,
-            model=self.model,
-            **kwargs,
+
+        messages = [{"role": "user", "content": prompt}]
+
+        if history:
+            role_cycle = itertools.cycle(('user', 'assistant'))
+            history_messages = itertools.chain.from_iterable(history)
+
+            history = [{"role": role, "content": message}
+                       for role, message in zip(role_cycle, history_messages)
+                       if message is not None]
+            messages = [*history, *messages]
+
+        if system_message:
+            messages = [{"role": "system", "content": system_message}, *messages] 
+
+        response = openai.ChatCompletion.create(
+            model=self.model, messages=messages, temperature=temperature, **kwargs
         )
+
         latency = time.time() - start_time
-        completion = response["completion"].strip()
+        completion = response.choices[0].message.content.strip()
+        usage = response.usage
+        prompt_tokens = usage["prompt_tokens"]
+        completion_tokens = usage["completion_tokens"]
+        total_tokens = usage["total_tokens"]
 
-        # Calculate tokens and cost
-        prompt_tokens = anthropic.count_tokens(formatted_prompt)
-        completion_tokens = anthropic.count_tokens(completion)
-        total_tokens = prompt_tokens + completion_tokens
         cost_per_token = self.MODEL_INFO[self.model]
-        cost = (
-            (prompt_tokens * cost_per_token["prompt"])
-            + (completion_tokens * cost_per_token["completion"])
-        ) / 1000000
+        cost = (prompt_tokens * cost_per_token["prompt"] / 1000000) + (
+            completion_tokens * cost_per_token["completion"] / 1000000
+        )
 
         return {
             "text": completion,
             "meta": {
                 "model": self.model,
                 "tokens": total_tokens,
-                "tokens_prompt": prompt_tokens,
-                "tokens_completion": completion_tokens,
+                "tokens_prompt": prompt_tokens,  # Add tokens_prompt to meta
+                "tokens_completion": completion_tokens,  # Add tokens_completion to meta
                 "cost": cost,
                 "latency": latency,
             },
         }
```

### Comparing `pyllms-0.1.2/pyllms.egg-info/PKG-INFO` & `pyllms-0.1.3/pyllms.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyllms
-Version: 0.1.2
+Version: 0.1.3
 Summary: A brief description of your package
 Author: Vladimir Prelovac
 Author-email: vlad@kagi.com
 Project-URL: Documentation, https://github.com/kagisearch/pyllms
 Project-URL: Source Code, https://github.com/kagisearch/pyllms
 Project-URL: Issue Tracker, https://github.com/kagisearch/pyllms/issues
 Keywords: llm,llms,large language model,AI,NLP,natural language processing,gpt,chatgpt,openai,anthropic,ai21
@@ -38,80 +38,92 @@
 
 
 ## Usage
 
 
 ```
 import llms
+
 model = llms.init()
 result = model.complete("what is 5+5")
+
 print(result.text)  
 
 ```
 
-llms will read the API key from environment variables, which you can set like this:
+Library will attempt to read the API keys and the default model from environment variables, which you can set like this:
 
 ```
 export OPENAI_API_KEY="your_api_key_here"
 export ANTHROPIC_API_KEY="your_api_key_here"
 export AI21_API_KEY="your_api_key_here"
+
 export LLMS_DEFAULT_MODEL="gpt-3.5-turbo"
 ```
 
 
 Alternatively, you can pass initialization values to the init() method:
 
 ```
 model=llms.init(openai_api_key='your_api_key_here', model='gpt-4')
 ```
 
 
-You can also pass optional parameters to the complete method. Any parameters accepted by the original model are supported automatically, in the verbatim form:
+You can also pass optional parameters to the complete method. 'temperature' and 'max_tokens' are standardized across all APIs and get converted to the corresponding API params. 
+
+Any other parameters accepted by the original model are supported in their verbatim form.
 
 ```
 result = model.complete(
     "what is the capital of country where mozzart was born",
     temperature=0.1,
+    max_tokens=200
 )
 ```
 
-By default, temperature for all models is set to 0.
+Note: By default, temperature for all models is set to 0, and max_tokens to 300.
 
-The result will also contain helpful information like tokens used, cost (which is automatically calculated using current pricing), and result latency:
+The result will also contain helpful information like tokens used, cost (which is automatically calculated using current pricing), and response latency in the 'meta' field:
 ```
 >>> print(result.meta)
 {'model': 'gpt-3.5-turbo', 'tokens': 15, 'tokens_prompt': 14, 'tokens_completion': 1, 'cost': 3e-05, 'latency': 0.48232388496398926}
 ```
 
 
 
 
-
-
-
-
 ## Multi-model usage
 
-You can initialize multiple models at once, which is very useful for testing and comparing output of different models. All models will run in parallel to save time. 
+You can also initialize multiple models at once! This is very useful for testing and comparing output of different models in parallel. 
 
 ```
 >>> models=llms.init(model=['gpt-3.5-turbo','claude-instant-v1'])
 >>> result=models.complete('what is the capital of country where mozzart was born')
 >>> print(result.text)
 ['The capital of the country where Mozart was born is Vienna, Austria.', 'Wolfgang Amadeus Mozart was born in Salzburg, Austria.\n\nSo the capital of the country where Mozart was born is Vienna, Austria.']
 
 >>> print(result.meta)
 [{'model': 'gpt-3.5-turbo', 'tokens': 34, 'tokens_prompt': 20, 'tokens_completion': 14, 'cost': 6.8e-05, 'latency': 0.7097790241241455}, {'model': 'claude-instant-v1', 'tokens': 54, 'tokens_prompt': 20, 'tokens_completion': 34, 'cost': 5.79e-05, 'latency': 0.7291600704193115}]
 ```
 
+
 ## Benchmarks
 
+Models are appearing like mushrooms after rain and we are interested in:
+
+1) Quality
+2) Speed
+3) Cost
+
+We included an automated benchmark system. The quality is evaluated using a powerful model (for example gpt-4) on a range of predefined questions, or you can supply your own.
+
+
 ```
-models=llms.init(model=['gpt-3.5-turbo', 'claude-instant-v1'])
-gpt4=llms.init('gpt-4')
+models=llms.init(model=['gpt-3.5-turbo', 'claude-instant-v1', 'j2-jumbo-instruct'])
+gpt4=llms.init('gpt-4') # optional, evaluator can be ommited and in this case only speed and cost is evaluated
 models.benchmark(evaluator=gpt4)
 ```
 
 ```
 +---------------------------------------+--------------------+---------------------+-----------------------+---------------------------+-----------------+
 |                 Model                 |       Tokens       |       Cost ($)      |      Latency (s)      |     Speed (tokens/sec)    |    Evaluation   |
 +---------------------------------------+--------------------+---------------------+-----------------------+---------------------------+-----------------+
@@ -150,17 +162,18 @@
 |    AI21Provider (j2-jumbo-instruct)   |        218         |       0.00327       |          5.90         |           36.95           |        1        |
 |    AI21Provider (j2-jumbo-instruct)   |        281         |       0.00421       |          6.25         |           44.97           |        1        |
 |    AI21Provider (j2-jumbo-instruct)   |        149         |       0.00224       |          1.56         |           95.81           |        10       |
 |    AI21Provider (j2-jumbo-instruct)   | Total Tokens: 1838 | Total Cost: 0.02757 |  Median Latency: 5.62 |  Aggregrated speed: 40.01 | Total Score: 68 |
 +---------------------------------------+--------------------+---------------------+-----------------------+---------------------------+-----------------+
 ```
 
-In addition, you can evaluate models on your own prompts:
+To evaluate models on your own prompts, simply pass a list of questions. The evaluator will automatically evaluate the responses:
+
 ```
-models.benchmark(prompts=["what is the capital of finland", "who won superbowl in the year justin bieber was born"],evaluator=gpt4)
+models.benchmark(prompts=["what is the capital of finland", "who won superbowl in the year justin bieber was born"], evaluator=gpt4)
 ```
 
 ## Supported Models
 
 To get a list of supported models, call list(). Models will be shown in the order of least expensive to most expensive.
 
 ```
```

### Comparing `pyllms-0.1.2/setup.py` & `pyllms-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 _project_homepage = "https://github.com/kagisearch/pyllms"
 
 setup(
     name="pyllms",
-    version="0.1.2",
+    version="0.1.3",
     description="A brief description of your package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Vladimir Prelovac",
     author_email="vlad@kagi.com",
     packages=find_packages(),
     install_requires=[
```

