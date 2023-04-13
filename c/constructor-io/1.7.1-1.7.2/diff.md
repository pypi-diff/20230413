# Comparing `tmp/constructor-io-1.7.1.tar.gz` & `tmp/constructor-io-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "constructor-io-1.7.1.tar", last modified: Tue Jan 24 20:13:35 2023, max compression
+gzip compressed data, was "constructor-io-1.7.2.tar", last modified: Thu Apr 13 18:28:16 2023, max compression
```

## Comparing `constructor-io-1.7.1.tar` & `constructor-io-1.7.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 enes       (501) staff       (20)        0 2023-01-24 20:13:35.632762 constructor-io-1.7.1/
--rw-r--r--   0 enes       (501) staff       (20)     1086 2021-09-21 17:57:12.000000 constructor-io-1.7.1/LICENSE
--rw-r--r--   0 enes       (501) staff       (20)     2562 2023-01-24 20:13:35.632094 constructor-io-1.7.1/PKG-INFO
--rw-r--r--   0 enes       (501) staff       (20)     2198 2022-10-03 13:13:47.000000 constructor-io-1.7.1/README.md
-drwxr-xr-x   0 enes       (501) staff       (20)        0 2023-01-24 20:13:35.617045 constructor-io-1.7.1/constructor_io/
--rw-r--r--   0 enes       (501) staff       (20)       41 2023-01-24 20:13:16.000000 constructor-io-1.7.1/constructor_io/__init__.py
--rw-r--r--   0 enes       (501) staff       (20)     2243 2022-10-12 17:39:44.000000 constructor-io-1.7.1/constructor_io/constructor_io.py
-drwxr-xr-x   0 enes       (501) staff       (20)        0 2023-01-24 20:13:35.623748 constructor-io-1.7.1/constructor_io/helpers/
--rw-r--r--   0 enes       (501) staff       (20)        0 2021-11-18 19:33:38.000000 constructor-io-1.7.1/constructor_io/helpers/__init__.py
--rw-r--r--   0 enes       (501) staff       (20)      481 2021-11-18 19:33:38.000000 constructor-io-1.7.1/constructor_io/helpers/exception.py
--rw-r--r--   0 enes       (501) staff       (20)     4795 2022-10-03 13:13:47.000000 constructor-io-1.7.1/constructor_io/helpers/utils.py
-drwxr-xr-x   0 enes       (501) staff       (20)        0 2023-01-24 20:13:35.630999 constructor-io-1.7.1/constructor_io/modules/
--rw-r--r--   0 enes       (501) staff       (20)        0 2021-11-18 19:33:38.000000 constructor-io-1.7.1/constructor_io/modules/__init__.py
--rw-r--r--   0 enes       (501) staff       (20)     3976 2022-10-03 13:13:47.000000 constructor-io-1.7.1/constructor_io/modules/autocomplete.py
--rw-r--r--   0 enes       (501) staff       (20)    14881 2022-10-03 13:13:47.000000 constructor-io-1.7.1/constructor_io/modules/browse.py
--rw-r--r--   0 enes       (501) staff       (20)    17262 2022-10-21 17:16:45.000000 constructor-io-1.7.1/constructor_io/modules/catalog.py
--rw-r--r--   0 enes       (501) staff       (20)     5602 2022-11-18 16:55:32.000000 constructor-io-1.7.1/constructor_io/modules/quizzes.py
--rw-r--r--   0 enes       (501) staff       (20)     4167 2022-10-03 13:13:47.000000 constructor-io-1.7.1/constructor_io/modules/recommendations.py
--rw-r--r--   0 enes       (501) staff       (20)     4164 2022-10-03 13:13:47.000000 constructor-io-1.7.1/constructor_io/modules/search.py
--rw-r--r--   0 enes       (501) staff       (20)     3868 2022-11-08 15:58:41.000000 constructor-io-1.7.1/constructor_io/modules/tasks.py
-drwxr-xr-x   0 enes       (501) staff       (20)        0 2023-01-24 20:13:35.621515 constructor-io-1.7.1/constructor_io.egg-info/
--rw-r--r--   0 enes       (501) staff       (20)     2562 2023-01-24 20:13:35.000000 constructor-io-1.7.1/constructor_io.egg-info/PKG-INFO
--rw-r--r--   0 enes       (501) staff       (20)      660 2023-01-24 20:13:35.000000 constructor-io-1.7.1/constructor_io.egg-info/SOURCES.txt
--rw-r--r--   0 enes       (501) staff       (20)        1 2023-01-24 20:13:35.000000 constructor-io-1.7.1/constructor_io.egg-info/dependency_links.txt
--rw-r--r--   0 enes       (501) staff       (20)       15 2023-01-24 20:13:35.000000 constructor-io-1.7.1/constructor_io.egg-info/requires.txt
--rw-r--r--   0 enes       (501) staff       (20)       15 2023-01-24 20:13:35.000000 constructor-io-1.7.1/constructor_io.egg-info/top_level.txt
--rw-r--r--   0 enes       (501) staff       (20)       38 2023-01-24 20:13:35.632984 constructor-io-1.7.1/setup.cfg
--rw-r--r--   0 enes       (501) staff       (20)      745 2022-01-10 22:25:09.000000 constructor-io-1.7.1/setup.py
+drwxr-xr-x   0 enes       (502) staff       (20)        0 2023-04-13 18:28:16.871691 constructor-io-1.7.2/
+-rw-r--r--   0 enes       (502) staff       (20)     1086 2021-09-21 17:57:12.000000 constructor-io-1.7.2/LICENSE
+-rw-r--r--   0 enes       (502) staff       (20)     2562 2023-04-13 18:28:16.871542 constructor-io-1.7.2/PKG-INFO
+-rw-r--r--   0 enes       (502) staff       (20)     2198 2022-10-03 13:13:47.000000 constructor-io-1.7.2/README.md
+drwxr-xr-x   0 enes       (502) staff       (20)        0 2023-04-13 18:28:16.868665 constructor-io-1.7.2/constructor_io/
+-rw-r--r--   0 enes       (502) staff       (20)       41 2023-04-13 18:28:06.000000 constructor-io-1.7.2/constructor_io/__init__.py
+-rw-r--r--   0 enes       (502) staff       (20)     2243 2022-10-12 17:39:44.000000 constructor-io-1.7.2/constructor_io/constructor_io.py
+drwxr-xr-x   0 enes       (502) staff       (20)        0 2023-04-13 18:28:16.869873 constructor-io-1.7.2/constructor_io/helpers/
+-rw-r--r--   0 enes       (502) staff       (20)        0 2021-11-18 19:33:38.000000 constructor-io-1.7.2/constructor_io/helpers/__init__.py
+-rw-r--r--   0 enes       (502) staff       (20)      481 2021-11-18 19:33:38.000000 constructor-io-1.7.2/constructor_io/helpers/exception.py
+-rw-r--r--   0 enes       (502) staff       (20)     4795 2022-10-03 13:13:47.000000 constructor-io-1.7.2/constructor_io/helpers/utils.py
+drwxr-xr-x   0 enes       (502) staff       (20)        0 2023-04-13 18:28:16.871338 constructor-io-1.7.2/constructor_io/modules/
+-rw-r--r--   0 enes       (502) staff       (20)        0 2021-11-18 19:33:38.000000 constructor-io-1.7.2/constructor_io/modules/__init__.py
+-rw-r--r--   0 enes       (502) staff       (20)     3976 2022-10-03 13:13:47.000000 constructor-io-1.7.2/constructor_io/modules/autocomplete.py
+-rw-r--r--   0 enes       (502) staff       (20)    14881 2022-10-03 13:13:47.000000 constructor-io-1.7.2/constructor_io/modules/browse.py
+-rw-r--r--   0 enes       (502) staff       (20)    17262 2022-10-21 17:16:45.000000 constructor-io-1.7.2/constructor_io/modules/catalog.py
+-rw-r--r--   0 enes       (502) staff       (20)     6762 2023-04-13 18:25:13.000000 constructor-io-1.7.2/constructor_io/modules/quizzes.py
+-rw-r--r--   0 enes       (502) staff       (20)     4167 2022-10-03 13:13:47.000000 constructor-io-1.7.2/constructor_io/modules/recommendations.py
+-rw-r--r--   0 enes       (502) staff       (20)     4164 2022-10-03 13:13:47.000000 constructor-io-1.7.2/constructor_io/modules/search.py
+-rw-r--r--   0 enes       (502) staff       (20)     3868 2022-11-08 15:58:41.000000 constructor-io-1.7.2/constructor_io/modules/tasks.py
+drwxr-xr-x   0 enes       (502) staff       (20)        0 2023-04-13 18:28:16.869449 constructor-io-1.7.2/constructor_io.egg-info/
+-rw-r--r--   0 enes       (502) staff       (20)     2562 2023-04-13 18:28:16.000000 constructor-io-1.7.2/constructor_io.egg-info/PKG-INFO
+-rw-r--r--   0 enes       (502) staff       (20)      660 2023-04-13 18:28:16.000000 constructor-io-1.7.2/constructor_io.egg-info/SOURCES.txt
+-rw-r--r--   0 enes       (502) staff       (20)        1 2023-04-13 18:28:16.000000 constructor-io-1.7.2/constructor_io.egg-info/dependency_links.txt
+-rw-r--r--   0 enes       (502) staff       (20)       15 2023-04-13 18:28:16.000000 constructor-io-1.7.2/constructor_io.egg-info/requires.txt
+-rw-r--r--   0 enes       (502) staff       (20)       15 2023-04-13 18:28:16.000000 constructor-io-1.7.2/constructor_io.egg-info/top_level.txt
+-rw-r--r--   0 enes       (502) staff       (20)       38 2023-04-13 18:28:16.871743 constructor-io-1.7.2/setup.cfg
+-rw-r--r--   0 enes       (502) staff       (20)      745 2022-01-10 22:25:09.000000 constructor-io-1.7.2/setup.py
```

### Comparing `constructor-io-1.7.1/LICENSE` & `constructor-io-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.1/PKG-INFO` & `constructor-io-1.7.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: constructor-io
-Version: 1.7.1
+Version: 1.7.2
 Summary: Constructor.IO Python Client
 Home-page: https://www.constructor.io
 Author: Constructor.io
 Author-email: info@constructor.io
 License: MIT
-Download-URL: https://github.com/Constructor-io/constructor-io/tarball/1.7.1
+Download-URL: https://github.com/Constructor-io/constructor-io/tarball/1.7.2
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Constructor.io Python Client
 
 [![Version](https://img.shields.io/pypi/v/constructor-io.svg)](https://pypi.python.org/pypi/constructor-io)
```

### Comparing `constructor-io-1.7.1/README.md` & `constructor-io-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.1/constructor_io/constructor_io.py` & `constructor-io-1.7.2/constructor_io/constructor_io.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.1/constructor_io/helpers/utils.py` & `constructor-io-1.7.2/constructor_io/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.1/constructor_io/modules/autocomplete.py` & `constructor-io-1.7.2/constructor_io/modules/autocomplete.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.1/constructor_io/modules/browse.py` & `constructor-io-1.7.2/constructor_io/modules/browse.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.1/constructor_io/modules/catalog.py` & `constructor-io-1.7.2/constructor_io/modules/catalog.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.1/constructor_io/modules/quizzes.py` & `constructor-io-1.7.2/constructor_io/modules/quizzes.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,23 +18,26 @@
     quiz_service_url = 'https://quizzes.cnstrc.com'
     query_params = create_shared_query_params(options, {}, user_parameters)
     ans_query_string = ''
 
     if not quiz_id or not isinstance(quiz_id, str):
         raise ConstructorException('quiz_id is a required parameter of type str')
 
-    if path == 'finalize' and (not isinstance(parameters.get('answers'), list) or len(parameters.get('answers')) == 0): # pylint: disable=line-too-long
+    if path == 'results' and (not isinstance(parameters.get('answers'), list) or len(parameters.get('answers')) == 0): # pylint: disable=line-too-long
         raise ConstructorException('answers is a required parameter of type list')
 
     if parameters:
         if parameters.get('section'):
             query_params['section'] = parameters.get('section')
 
-        if parameters.get('version_id'):
-            query_params['version_id'] = parameters.get('version_id')
+        if parameters.get('quiz_version_id'):
+            query_params['quiz_version_id'] = parameters.get('quiz_version_id')
+
+        if parameters.get('quiz_session_id'):
+            query_params['quiz_session_id'] = parameters.get('quiz_session_id')
 
         if parameters.get('answers'):
             answers_param = []
             answers = parameters.get('answers')
 
             for question_answer in answers:
                 answers_param.append(','.join(map(str, question_answer)))
@@ -58,15 +61,16 @@
         '''
         Retrieve next question from API
 
         :param str quiz_id: Quiz Id
         :param dict parameters: Additional parameters to determine next quiz
         :param list parameters.answers: 2d Array of quiz answers in the format [[1],[1,2]]
         :param str parameters.section: Section for customer's product catalog
-        :param str parameters.version_id: Specific version_id for the quiz
+        :param str parameters.quiz_version_id: Specific quiz_version_id for the quiz. Version ID will be returned with the first request and it should be passed with subsequent requests. More information can be found: https://docs.constructor.io/rest_api/quiz/using_quizzes/#quiz-versioning
+        :param str parameters.quiz_session_id: Specific quiz_session_id for the quiz. Session ID will be returned with the first request and it should be passed with subsequent requests. More information can be found: https://docs.constructor.io/rest_api/quiz/using_quizzes/#quiz-sessions
         :param dict user_parameters: Parameters relevant to the user request
         :param int user_parameters.session_id: Session ID, utilized to personalize results
         :param str user_parameters.client_id: Client ID, utilized to personalize results
         :param str user_parameters.user_ip: Origin user IP, from client
         :param str user_parameters.user_agent: Origin user agent, from client
         :return: dict
         '''
@@ -87,53 +91,54 @@
 
         if not response.ok:
             throw_http_exception_from_response(response)
 
         json = response.json()
 
         if json:
-            if json.get('version_id'):
+            if json.get('quiz_version_id'):
                 return json
 
         raise ConstructorException('get_quiz_next_question response data is malformed')
 
     def get_quiz_results(self, quiz_id, parameters=None, user_parameters=None):
         '''
         Retrieve quiz results from API
 
         :param str quiz_id: Quiz Id
         :param dict parameters: Additional parameters to determine next quiz
         :param list parameters.answers: 2d Array of quiz answers in the format [[1],[1,2]]
         :param str parameters.section: Section for customer's product catalog
-        :param str parameters.version_id: Specific version_id for the quiz
+        :param str parameters.quiz_version_id: Specific quiz_version_id for the quiz. Version ID will be returned with the first request and it should be passed with subsequent requests. More information can be found: https://docs.constructor.io/rest_api/quiz/using_quizzes/#quiz-versioning
+        :param str parameters.quiz_session_id: Specific quiz_session_id for the quiz. Session ID will be returned with the first request and it should be passed with subsequent requests. More information can be found: https://docs.constructor.io/rest_api/quiz/using_quizzes/#quiz-sessions
         :param dict user_parameters: Parameters relevant to the user request
         :param int user_parameters.session_id: Session ID, utilized to personalize results
         :param str user_parameters.client_id: Client ID, utilized to personalize results
         :param str user_parameters.user_ip: Origin user IP, from client
         :param str user_parameters.user_agent: Origin user agent, from client
         :return: dict
         '''
 
         if not parameters:
             parameters = {}
         if not user_parameters:
             user_parameters = {}
 
-        request_url = _create_quizzes_url(quiz_id, parameters, user_parameters, self.__options, 'finalize') #pylint: disable=line-too-long
+        request_url = _create_quizzes_url(quiz_id, parameters, user_parameters, self.__options, 'results') #pylint: disable=line-too-long
         requests = self.__options.get('requests') or r
 
         response = requests.get(
             request_url,
             auth=create_auth_header(self.__options),
             headers=create_request_headers(self.__options, user_parameters)
         )
 
         if not response.ok:
             throw_http_exception_from_response(response)
 
         json = response.json()
 
         if json:
-            if json.get('version_id'):
+            if json.get('quiz_version_id'):
                 return json
 
         raise ConstructorException('get_quiz_results response data is malformed')
```

### Comparing `constructor-io-1.7.1/constructor_io/modules/recommendations.py` & `constructor-io-1.7.2/constructor_io/modules/recommendations.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.1/constructor_io/modules/search.py` & `constructor-io-1.7.2/constructor_io/modules/search.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.1/constructor_io/modules/tasks.py` & `constructor-io-1.7.2/constructor_io/modules/tasks.py`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.1/constructor_io.egg-info/PKG-INFO` & `constructor-io-1.7.2/constructor_io.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: constructor-io
-Version: 1.7.1
+Version: 1.7.2
 Summary: Constructor.IO Python Client
 Home-page: https://www.constructor.io
 Author: Constructor.io
 Author-email: info@constructor.io
 License: MIT
-Download-URL: https://github.com/Constructor-io/constructor-io/tarball/1.7.1
+Download-URL: https://github.com/Constructor-io/constructor-io/tarball/1.7.2
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Constructor.io Python Client
 
 [![Version](https://img.shields.io/pypi/v/constructor-io.svg)](https://pypi.python.org/pypi/constructor-io)
```

### Comparing `constructor-io-1.7.1/constructor_io.egg-info/SOURCES.txt` & `constructor-io-1.7.2/constructor_io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `constructor-io-1.7.1/setup.py` & `constructor-io-1.7.2/setup.py`

 * *Files identical despite different names*

