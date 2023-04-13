# Comparing `tmp/clara_ai-0.0.3.tar.gz` & `tmp/clara_ai-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clara_ai-0.0.3.tar", max compression
+gzip compressed data, was "clara_ai-0.0.4.tar", max compression
```

## Comparing `clara_ai-0.0.3.tar` & `clara_ai-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1534 2023-04-13 17:48:10.642821 clara_ai-0.0.3/LICENSE
--rw-r--r--   0        0        0     2148 2023-04-13 17:48:10.642821 clara_ai-0.0.3/README.md
--rw-r--r--   0        0        0     4458 2023-04-13 17:48:10.642821 clara_ai-0.0.3/clara/cli.py
--rw-r--r--   0        0        0       54 2023-04-13 17:48:10.642821 clara_ai-0.0.3/clara/console.py
--rw-r--r--   0        0        0     2660 2023-04-13 17:48:10.642821 clara_ai-0.0.3/clara/consts.py
--rw-r--r--   0        0        0     5248 2023-04-13 17:48:10.642821 clara_ai-0.0.3/clara/index.py
--rw-r--r--   0        0        0      665 2023-04-13 17:48:10.646821 clara_ai-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2852 1970-01-01 00:00:00.000000 clara_ai-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1534 2023-04-13 21:56:40.455905 clara_ai-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2148 2023-04-13 21:56:40.455905 clara_ai-0.0.4/README.md
+-rw-r--r--   0        0        0     4458 2023-04-13 21:56:40.455905 clara_ai-0.0.4/clara/cli.py
+-rw-r--r--   0        0        0       54 2023-04-13 21:56:40.455905 clara_ai-0.0.4/clara/console.py
+-rw-r--r--   0        0        0     3090 2023-04-13 21:56:40.459905 clara_ai-0.0.4/clara/consts.py
+-rw-r--r--   0        0        0     5391 2023-04-13 21:56:40.459905 clara_ai-0.0.4/clara/index.py
+-rw-r--r--   0        0        0      665 2023-04-13 21:56:40.459905 clara_ai-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2852 1970-01-01 00:00:00.000000 clara_ai-0.0.4/PKG-INFO
```

### Comparing `clara_ai-0.0.3/LICENSE` & `clara_ai-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `clara_ai-0.0.3/README.md` & `clara_ai-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `clara_ai-0.0.3/clara/cli.py` & `clara_ai-0.0.4/clara/cli.py`

 * *Files identical despite different names*

### Comparing `clara_ai-0.0.3/clara/index.py` & `clara_ai-0.0.4/clara/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from langchain.embeddings.openai import OpenAIEmbeddings
 from langchain.indexes.vectorstore import VectorStoreIndexWrapper
 from langchain.vectorstores import Chroma
 from langchain.document_loaders import TextLoader
 from langchain.text_splitter import CharacterTextSplitter
 from langchain.schema import Document
 
-from .consts import WILDCARDS, BASE_PERSIST_PATH, PROMPT_PREFIX
+from .consts import WILDCARDS, BASE_PERSIST_PATH, PROMPT_PREFIX, CONDENSE_QUESTION_PROMPT
 from .console import console
 
 
 @dataclass
 class QueryResult:
     question: str
     answer: str
@@ -134,22 +134,24 @@
 
     def init_chat(self):
         model = ChatOpenAI(model="gpt-3.5-turbo", temperature=0)  # 'gpt-4',
         self.chat = ConversationalRetrievalChain.from_llm(
             model,
             retriever=self.index.vectorstore.as_retriever(),
             return_source_documents=True,
+            condense_question_prompt=CONDENSE_QUESTION_PROMPT,
         )
 
     def query_with_sources(self, query: str) -> QueryResult:
         # return QueryResult(**self.index.query_with_sources(query))
         if self.chat is None:
             self.init_chat()
         response = self.chat(
             {"question": query, "chat_history": self.chat_history.history}
+            # {"question": query, "chat_history": ""}
         )
         # console.log(response)
         self.chat_history.append((response["question"], response["answer"]))
         return QueryResult(
             question=response["question"],
             answer=response["answer"],
             sources=response["source_documents"],
```

### Comparing `clara_ai-0.0.3/pyproject.toml` & `clara_ai-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clara-ai"
-version = "0.0.3"
+version = "0.0.4"
 description = "CLARA: Code Language Assistant & Repository Analyzer"
 authors = ["Cristóbal Carnero Liñán <cristobal@seednapse.ai>"]
 readme = "README.md"
 packages = [{include = "clara"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `clara_ai-0.0.3/PKG-INFO` & `clara_ai-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clara-ai
-Version: 0.0.3
+Version: 0.0.4
 Summary: CLARA: Code Language Assistant & Repository Analyzer
 Author: Cristóbal Carnero Liñán
 Author-email: cristobal@seednapse.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

