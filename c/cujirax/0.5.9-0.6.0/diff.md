# Comparing `tmp/cujirax-0.5.9.tar.gz` & `tmp/cujirax-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cujirax-0.5.9.tar", last modified: Fri Mar 31 00:59:20 2023, max compression
+gzip compressed data, was "cujirax-0.6.0.tar", last modified: Thu Apr 13 07:43:17 2023, max compression
```

## Comparing `cujirax-0.5.9.tar` & `cujirax-0.6.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1836 2023-03-28 01:53:23.346105 cujirax-0.5.9/.gitignore
--rw-r--r--   0        0        0     1064 2023-03-08 08:56:39.228892 cujirax-0.5.9/LICENSE
--rw-r--r--   0        0        0      519 2023-03-11 13:29:07.840641 cujirax-0.5.9/README.md
--rw-r--r--   0        0        0     9417 2023-03-31 00:59:00.087141 cujirax-0.5.9/cujirax/__init__.py
--rw-r--r--   0        0        0     1545 2023-03-11 16:18:32.023550 cujirax-0.5.9/cujirax/cucumber.py
--rw-r--r--   0        0        0     3618 2023-03-30 09:13:16.351957 cujirax-0.5.9/cujirax/jira.py
--rw-r--r--   0        0        0     1840 2023-03-28 16:21:23.991726 cujirax-0.5.9/cujirax/xray/__init__.py
--rw-r--r--   0        0        0     1605 2023-03-30 07:41:41.303508 cujirax-0.5.9/cujirax/xray/import_results.py
--rw-r--r--   0        0        0     2079 2023-03-30 13:06:45.294265 cujirax-0.5.9/cujirax/xray/import_tests.py
--rw-r--r--   0        0        0      474 2023-03-30 12:04:31.612772 cujirax-0.5.9/pyproject.toml
--rw-r--r--   0        0        0      923 1970-01-01 00:00:00.000000 cujirax-0.5.9/PKG-INFO
+-rw-r--r--   0        0        0     1836 2023-03-28 01:53:23.346105 cujirax-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1064 2023-03-08 08:56:39.228892 cujirax-0.6.0/LICENSE
+-rw-r--r--   0        0        0      519 2023-03-11 13:29:07.840641 cujirax-0.6.0/README.md
+-rw-r--r--   0        0        0    10469 2023-04-13 06:38:24.586970 cujirax-0.6.0/cujirax/__init__.py
+-rw-r--r--   0        0        0     1545 2023-03-11 16:18:32.023550 cujirax-0.6.0/cujirax/cucumber.py
+-rw-r--r--   0        0        0     4230 2023-04-13 07:40:02.924013 cujirax-0.6.0/cujirax/jira.py
+-rw-r--r--   0        0        0     2485 2023-04-13 02:16:47.949068 cujirax-0.6.0/cujirax/xray/__init__.py
+-rw-r--r--   0        0        0     1605 2023-03-30 07:41:41.303508 cujirax-0.6.0/cujirax/xray/import_results.py
+-rw-r--r--   0        0        0     2079 2023-03-30 13:06:45.294265 cujirax-0.6.0/cujirax/xray/import_tests.py
+-rw-r--r--   0        0        0      474 2023-03-30 12:04:31.612772 cujirax-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      923 1970-01-01 00:00:00.000000 cujirax-0.6.0/PKG-INFO
```

### Comparing `cujirax-0.5.9/.gitignore` & `cujirax-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cujirax-0.5.9/LICENSE` & `cujirax-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cujirax-0.5.9/README.md` & `cujirax-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `cujirax-0.5.9/cujirax/__init__.py` & `cujirax-0.6.0/cujirax/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 """
 Cucumber result to Jira Xray Test repository
 
 """
-__version__ = "0.5.9"
+__version__ = "0.6.0"
 
 
 import datetime
 
 import cujirax.cucumber as cucumber
 import cujirax.xray.import_results as result
 import cujirax.xray.import_tests as test
 from cujirax.cucumber import Element
 from cujirax.jira import Jirakey, JiraX, Project
 from loguru import logger
 from collections import Counter
 
 
 class CuJiraX:
-    def __init__(self, jira_project: str, parent_testset_key: str = None) -> None:
+    def __init__(self, jira_project: str, parent_testset_key: str = None, addional_identifier: str = None) -> None:
         self.jira_project = jira_project
         self.jira = JiraX(jira_project)
         
         self.testexecution = None
         self.testexecution_name = None
         self.testexecution_desc = None
         self.parent_testset_key = parent_testset_key
         self.result_info = result.Info(summary="TBA", description="TBA")
+        self.addional_identifier = addional_identifier
 
     def set_testsut_version(self, version: str):
         self.result_info.version = version
     
     def set_test_user(self, user: str):
         self.result_info.user = user
 
@@ -65,75 +66,89 @@
         self.testexecution_desc = description
 
 
     def to_xray(
             self, 
             cucumber_json: str,
             import_result=True, 
+            import_testcase=True,
             ignore_duplicate=True
-        )-> dict:
+        )-> list:
 
         s1 = cucumber.Model.parse_file(cucumber_json)
-        output = {}
+        output = []
         for f in s1.__root__:
+            root = {}
             testset_name = f.uri.split("/")[-1]
-            testexecution_name = self.testexecution_name or datetime.date.today().strftime("%Y%m%d") + " :: " + testset_name
+            testexecution_name = self.testexecution_name or testset_name + " :: " + datetime.date.today().strftime("%Y%m%d") 
+            if self.addional_identifier:
+                testexecution_name = f"{self.addional_identifier} :: {testexecution_name}"
 
             ticket_ts, ticket_te = [
                 self.jira.create_testset(
                     summary=testset_name, 
                     description=f.description or "TBA"
                 ),
                 self.testexecution or self.jira.create_testexecution(
                     summary=testexecution_name, 
-                    description=self.testexecution_desc or f.description or "TBA"
+                    description=self.testexecution_desc or f.description or "TBA",
+                    labels=[f'c{datetime.date.today().strftime("%Y%m%d")}', self.addional_identifier]
                 ),
             ]
-
-            # Import Test cases
-            exists, new = self._split_elements_to_exist_and_new(
-                elements=f.elements, 
-                j=self.jira, 
-                ignore_duplicate=ignore_duplicate
-            )
-            
-            tests = [str(n) for n in map(lambda x: self._update_description_if_exist(x,self.jira), exists)]
-            output.update({
+            root.update({
                 'test_set': str(ticket_ts),
                 'testset_name': testset_name,
                 'parent_testset': self.parent_testset_key,
                 'test_execution': str(ticket_te),
                 'testexecution_name': testexecution_name,
                 'test_plan': self.result_info.testPlanKey,
-                'tests': tests,
                 'test_environments': self.result_info.testEnvironments
             })
 
-            logger.info(output)
-            
-            test_cases = [n for n in map(lambda x: self._new_testcase(x, self.jira_project, ticket_ts, self.parent_testset_key), new)]
-            test.bulk_import(test_cases) if test_cases else None
+            # Import Test cases
+            if import_testcase:
+                try:
+                    exists, new = self._split_elements_to_exist_and_new(
+                        elements=f.elements, 
+                        j=self.jira, 
+                        ignore_duplicate=ignore_duplicate
+                    )
+                except ValueError as e:
+                    raise type(e)(f"{f.uri}: {str(e)}") from e
+                
+                tests = [str(n) for n in map(
+                    lambda x: self._update_description_if_exist(x,self.jira), exists)]
+                root.update({
+                    'existing_tests': tests,
+                })
+
+                logger.info(root)
+                
+                test_cases = [n for n in map(lambda x: self._new_testcase(x, self.jira_project, ticket_ts, self.parent_testset_key), new)]
+                test.bulk_import(test_cases) if test_cases else None
             
             # Import Results
             if import_result:
                 self.result_info.summary = testexecution_name
                 self.result_info.description = self.testexecution_desc or f.description or "TBA"
                 
-                _tests = self._get_results(f.elements, self.jira, ignore_duplicate)
-                
+                _tests, _result = self._get_results(f.elements, self.jira, ignore_duplicate)
+                logger.debug("tests:" + str(_tests) + ", result: " + _result)
                 req = result.RequestBody(
                     info=self.result_info,
                     tests= _tests,
                     testExecutionKey=str(ticket_te)
                 )
                 res = result.import_xray_json_results(req)
-                output.update({
+                root.update({
+                    'result': _result,
                     'import_result_status': res.status_code,
                     'import_result_response': res.json()
                 })
+            output.append(root)
         return output    
         
     
     def create_testplan(self, testplan_name:str, testplan_desc: str) -> Jirakey:
         """
         This function return Jira key, create new test plan when not found.
 
@@ -141,48 +156,53 @@
         produces the same result as call it once.
         """
         assert testplan_name, "Test plan name cannot be None"
         return self.jira.create_testplan(summary=testplan_name, description=testplan_desc)
 
     @classmethod
     def _get_results(cls, elements: Element, j: JiraX, ignore_duplicate):
-        result_tests = []
+        test_request_obj = []
+        results = []
         for el in elements:
             test_name = cls.scenarioid_to_tescasename(el.id, el.keyword)
             tests = j.get_tests(test_name)
-            assert tests, "Test not created: {}".format(test_name)
+            if not tests:
+                raise ValueError("Test not created: {}".format(test_name))
             
             test_key = tests[0]
             if not ignore_duplicate:
                 if len(tests) > 1:
                     logger.error(test_name)
                     logger.error(["{}".format(t) for t in tests])
                     raise ValueError("More than 1 test key detected: ", tests, test_name)
                     
             statuses = [step.result.status.value for step in el.steps]
             agg_result = "passed" if all(s == 'passed' for s in statuses) else "failed"
-            result_tests.append(result.Test(testKey=str(test_key), status=agg_result))
-        return result_tests
+            test_request_obj.append(result.Test(testKey=str(test_key), status=agg_result))
+            results.append(agg_result)
+        grand_result = "passed" if all(s == 'passed' for s in results) else "failed"
+        return test_request_obj, grand_result
 
     @classmethod
     def _split_elements_to_exist_and_new(cls, elements: Element, j: JiraX, ignore_duplicate):
         found= []
         not_found = []
         
         for el in elements:
             test_name = cls.scenarioid_to_tescasename(el.id, el.keyword)
+            logger.info("searching_test_name: " + test_name)
+
             tests = j.get_tests(test_name)
 
             if tests and not ignore_duplicate:
                 if len(tests) > 1:
                     logger.error(test_name)
                     logger.error(["{}".format(t) for t in tests])
                     raise ValueError("More than 1 test key detected: ", tests, test_name)
-            logger.info("search test case: " + test_name)
-            logger.info(tests)
+            logger.info("found_in_jira: " + str(tests))
             found.append(el) if j.get_tests(test_name) else not_found.append(el)
         
         # check duplicate for new test
         if not ignore_duplicate:
             new_testnames = [cls.scenarioid_to_tescasename(el.id, el.keyword) for el in not_found]
             duplicates = [item for item, count in Counter(new_testnames).items() if count > 1]
             if duplicates:
```

### Comparing `cujirax-0.5.9/cujirax/cucumber.py` & `cujirax-0.6.0/cujirax/cucumber.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.5.9/cujirax/jira.py` & `cujirax-0.6.0/cujirax/jira.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import re
 from atlassian import Jira
 from typing import List
 from pydantic import BaseModel
-
+from loguru import logger
 
 class Jirakey:
     value: str
 
     def __init__(self, value) -> None:
         self.value = value
         if not re.match(r'[A-Z][A-Z0-9_]*-[1-9][0-9]*$', value):
@@ -54,17 +54,23 @@
 
     def get_testplan(self, summary: str) -> List[Jirakey]:
         return self.get_issues(summary=summary, type="Test Plan")
 
     def get_tests(self, summary: str) -> List[Jirakey]:
         return self.get_issues(summary=summary, type="Test")
 
-    def get_issues(self, summary: str, type: str) -> List[Jirakey]:
-        _summary = summary.replace("[", "").replace("]", "")
-        query = f'issuetype="{type}" AND summary~"{_summary}" AND project="{self.key}"'
+    def get_issues(self, summary: str, type: str, labels: List[str] = []) -> List[Jirakey]:
+        # filter out problematic strings in summary
+        if labels:
+            labels = [f"labels='{l}'" for l in labels]
+            query = f'issuetype="{type}" AND project="{self.key}" AND {" AND ".join(labels)}'
+        else:
+            _summary = summary.replace("[", "").replace("]", "")
+            query = f'issuetype="{type}" AND summary~"{_summary}" AND project="{self.key}"'
+        logger.debug(f"query: '{query}'")
         issues = self.jql(query).get("issues")
         
         return [Jirakey(issue.get('key')) for issue in issues if issue.get('fields')['summary'] == summary]
 
     def link(self, parent_jira: str, child_jira: str, type="Parents"):
         """
         Common Types:
@@ -83,31 +89,36 @@
         """
         return self.create_issue_link({
             "type": {"name": type},
             "inwardIssue": {"key": str(Jirakey(child_jira))},
             "outwardIssue": {"key": str(Jirakey(parent_jira))}
         })
 
-    def _create(self, summary: str, description: str, issue_type: str) -> Jirakey:
-        issue = self.get_issues(summary, issue_type)
+    def _create(self, summary: str, description: str, issue_type: str, labels: List[str]) -> Jirakey:
+        issue = self.get_issues(summary, issue_type, labels)
         if issue:
             self.update_issue_field
             jira_key = issue[0]
             return jira_key
 
         issue = Issue(
             summary=summary,
             project=Project(key=self.key),
             issuetype=IssueType(name=issue_type),
             description=description)
         
         response = self.create_issue(fields=issue.dict())
-        return Jirakey(response.get('key'))
+        
+        key = Jirakey(response.get('key'))
+        logger.info(f"updating label {labels} to: {key.value}")
+        self.issue_update(key.value, fields={"labels": labels})
+
+        return key
 
-    def create_testset(self, summary: str, description: str) -> Jirakey:
-        return self._create(summary, description, "Test Set")
+    def create_testset(self, summary: str, description: str, labels: List[str] = []) -> Jirakey:
+        return self._create(summary, description, "Test Set", labels)
 
-    def create_testexecution(self, summary: str, description: str) -> Jirakey:
-        return self._create(summary, description, "Test Execution")
+    def create_testexecution(self, summary: str, description: str, labels: List[str] = []) -> Jirakey:
+        return self._create(summary, description, "Test Execution", labels)
 
-    def create_testplan(self, summary: str, description: str) -> Jirakey:
-        return self._create(summary, description, "Test Plan")
+    def create_testplan(self, summary: str, description: str, labels: List[str] = []) -> Jirakey:
+        return self._create(summary, description, "Test Plan", labels)
```

### Comparing `cujirax-0.5.9/cujirax/xray/__init__.py` & `cujirax-0.6.0/cujirax/xray/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from enum import Enum
 import json
 from typing import List, Union
 from pydantic import BaseModel, Field
 import os
 import requests
+import time
+import functools
+
 
 xray_url = "https://xray.cloud.getxray.app"
 
 
 class Endpoint(Enum):
     CREATE_TEST_CASE = "/api/v2/import/test/bulk"
     AUTHENTICATE = "/api/v2/authenticate"
@@ -21,14 +24,32 @@
 
 
 class Authentication(BaseModel):
     client_id: str = os.getenv("XRAY_CLIENT_ID")
     client_secret: str = os.getenv("XRAY_CLIENT_SECRET")
 
 
+def retry(max_retries=3, delay=1):
+    def decorator_retry(func):
+        @functools.wraps(func)
+        def wrapper_retry(*args, **kwargs):
+            retries = 0
+            while retries < max_retries:
+                try:
+                    return func(*args, **kwargs)
+                except Exception as e:
+                    retries += 1
+                    print(f"Retry {retries}/{max_retries} - Error: {e}")
+                    time.sleep(delay)
+            raise Exception(f"Failed after {max_retries} retries")
+        return wrapper_retry
+    return decorator_retry
+
+
+@retry(max_retries=5, delay=2)
 def login()-> Header:
     header = Header()
     response = post(Endpoint.AUTHENTICATE.value, Authentication(), header)
     if response.status_code == 200:
         header.Authorization = "Bearer " + eval(response.text)
         return header
     raise Exception("Authentication error: Invalid credentials")
```

### Comparing `cujirax-0.5.9/cujirax/xray/import_results.py` & `cujirax-0.6.0/cujirax/xray/import_results.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.5.9/cujirax/xray/import_tests.py` & `cujirax-0.6.0/cujirax/xray/import_tests.py`

 * *Files identical despite different names*

### Comparing `cujirax-0.5.9/PKG-INFO` & `cujirax-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cujirax
-Version: 0.5.9
+Version: 0.6.0
 Summary: Cucumber result to Jira Xray Test repository
 Author-email: Max Leow <maxengiu@outlook.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: pydantic
 Requires-Dist: atlassian-python-api
 Requires-Dist: requests
```

