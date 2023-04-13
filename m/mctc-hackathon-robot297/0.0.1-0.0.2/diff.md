# Comparing `tmp/mctc_hackathon_robot297-0.0.1.tar.gz` & `tmp/mctc_hackathon_robot297-0.0.2.tar.gz`

## Comparing `mctc_hackathon_robot297-0.0.1.tar` & `mctc_hackathon_robot297-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 mctc_hackathon_robot297-0.0.1/.env-sample
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 mctc_hackathon_robot297-0.0.1/CODEOWNERS
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 mctc_hackathon_robot297-0.0.1/requirements.txt
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 mctc_hackathon_robot297-0.0.1/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 mctc_hackathon_robot297-0.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mctc_hackathon_robot297-0.0.1/src/hackathon_helper/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mctc_hackathon_robot297-0.0.1/src/hackathon_helper/api/__init__.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 mctc_hackathon_robot297-0.0.1/src/hackathon_helper/api/api_builder.py
--rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 mctc_hackathon_robot297-0.0.1/src/hackathon_helper/api/core_banking.py
--rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 mctc_hackathon_robot297-0.0.1/src/hackathon_helper/api/money_movement.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 mctc_hackathon_robot297-0.0.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mctc_hackathon_robot297-0.0.1/LICENSE
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 mctc_hackathon_robot297-0.0.1/README.md
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 mctc_hackathon_robot297-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 mctc_hackathon_robot297-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 mctc_hackathon_robot297-0.0.2/.env-sample
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mctc_hackathon_robot297-0.0.2/CODEOWNERS
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 mctc_hackathon_robot297-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 mctc_hackathon_robot297-0.0.2/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 mctc_hackathon_robot297-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mctc_hackathon_robot297-0.0.2/src/hackathon_helper/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mctc_hackathon_robot297-0.0.2/src/hackathon_helper/api/__init__.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 mctc_hackathon_robot297-0.0.2/src/hackathon_helper/api/api_builder.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 mctc_hackathon_robot297-0.0.2/src/hackathon_helper/api/core_banking.py
+-rw-r--r--   0        0        0    11337 2020-02-02 00:00:00.000000 mctc_hackathon_robot297-0.0.2/src/hackathon_helper/api/money_movement.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 mctc_hackathon_robot297-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mctc_hackathon_robot297-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 mctc_hackathon_robot297-0.0.2/README.md
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 mctc_hackathon_robot297-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 mctc_hackathon_robot297-0.0.2/PKG-INFO
```

### Comparing `mctc_hackathon_robot297-0.0.1/requirements.txt` & `mctc_hackathon_robot297-0.0.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `mctc_hackathon_robot297-0.0.1/.github/workflows/pylint.yml` & `mctc_hackathon_robot297-0.0.2/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `mctc_hackathon_robot297-0.0.1/.github/workflows/python-publish.yml` & `mctc_hackathon_robot297-0.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `mctc_hackathon_robot297-0.0.1/src/hackathon_helper/api/api_builder.py` & `mctc_hackathon_robot297-0.0.2/src/hackathon_helper/api/api_builder.py`

 * *Files identical despite different names*

### Comparing `mctc_hackathon_robot297-0.0.1/src/hackathon_helper/api/core_banking.py` & `mctc_hackathon_robot297-0.0.2/src/hackathon_helper/api/core_banking.py`

 * *Files 18% similar despite different names*

```diff
@@ -81,80 +81,94 @@
                 url=self.uat_url + f'account/{account_id}/cards',
                 auth=self.basic_auth,
                 headers=self.headers,
                 timeout=60
             )
         return activity_response
 
-    def list_transactions(self, account_id, transaction_type, query_dates=None):
+    def list_transactions(self, account_id, transaction_type, **kwargs):
         """This method returns a JSON array of transactions for a specific
         account based on the input values. It can be limited to certain transaction
         types and date ranges.
 
         Args:
             account_id (string): a unique account id.
             transaction_type (string): type of transactions to retrieve. 
                 E.g., "FULL" "PUR" "MEMO" "PMT" "SHORT".
-            query_dates (dict): (Optional) start and end dates for searching by
-                transaction date range.
-                E.g., { start: "YYYY-MM-DD", end: "YYYY-MM-DD" }
-
+            start (string, optional): start date for searching by
+                transaction date range. Must use format: "YYYY-MM-DD"
+            end (string, optional): end date for searching by
+                transaction date range. Must use format: "YYYY-MM-DD"
+                
         Returns:
             Response: The response from the api including content and status code.
         """
+        optional_params = kwargs.keys()
+
+        if 'start' in optional_params and 'end' in optional_params:
+            query_dates = {'start': kwargs['start'], 'end': kwargs['end']}
+        else:
+            query_dates = None
+
         activity_response = requests.get(
                 url=self.uat_url + f'account/{account_id}/trans/{transaction_type}',
                 auth=self.basic_auth,
                 headers=self.headers,
                 params=query_dates,
                 timeout=60
             )
         return activity_response
 
-    def create_credit_card(self, customer_id, payload):
+    def create_credit_card(self, customer_id, nickname=None, account_type=None, credit_limit=None):
         """This method generates a new credit card account for a specific customer account.
 
         Args:
             customer_id (string): a unique customer id
-            payload (dict): The contents of the request.
-                E.g, 
-                {
-                "nickname": "",
-                "accountType": "string",
-                "creditLimit": 2000
-                }
+            nickname (optional, string): Account nickname
+            account_type (optional, string): type of mock account; enum[CCD, BCD]
+            credit_limit (optional, float): Credit limit for new card account
 
         Returns:
             Response: The response from the api including content and status code.
         """
+
+
+        payload = {
+                "nickname": str(nickname),
+                "accountType": str(account_type),
+                "creditLimit": float(credit_limit)
+        }
+
         activity_response = requests.post(
                 url=self.uat_url + f'account/{customer_id}/credit',
                 auth=self.basic_auth,
                 headers=self.headers,
                 json=payload,
                 timeout=60
             )
         return activity_response
 
-    def create_deposit_account(self, customer_id, payload):
+    def create_deposit_account(self, customer_id,  nickname=None,
+                               account_type=None, open_balance=None):
         """This method generates a new deposit account for a specific customer account.
 
         Args:
             customer_id (string): a unique customer id
-            payload (dict): The contents of the request.
-                E.g, 
-                {
-                "nickname": "",
-                "accountType": "string",
-                "openBalance": 100
-                }
+            nickname (optional, string): Account nickname
+            account_type (optional, string): type of mock account; enum[CCD, BCD]
+            open_balance (optional, float): Credit limit for new card account
 
         Returns:
             Response: The response from the api including content and status code.
         """
+        payload = {
+                "nickname": str(nickname),
+                "accountType": str(account_type),
+                "openBalance": float(open_balance)
+        }
         activity_response = requests.post(
                 url=self.uat_url + f'account/{customer_id}/dda',
                 auth=self.basic_auth,
                 headers=self.headers,
                 json=payload,
                 timeout=60
             )
```

### Comparing `mctc_hackathon_robot297-0.0.1/LICENSE` & `mctc_hackathon_robot297-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mctc_hackathon_robot297-0.0.1/README.md` & `mctc_hackathon_robot297-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mctc_hackathon_robot297-0.0.1/pyproject.toml` & `mctc_hackathon_robot297-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mctc_hackathon_robot297"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Daniel Obot", email="danobot@hotmail.com" },
   { name="Elizabeth Shockey", email="coffee@snob.beans"}
 ]
 description = "Libraries to help with the MCTC Hackathon"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `mctc_hackathon_robot297-0.0.1/PKG-INFO` & `mctc_hackathon_robot297-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mctc_hackathon_robot297
-Version: 0.0.1
+Version: 0.0.2
 Summary: Libraries to help with the MCTC Hackathon
 Project-URL: Homepage, https://github.com/robot297/Hackathon-Examples
 Project-URL: Bug Tracker, https://github.com/robot297/Hackathon-Examples/issues
 Author-email: Daniel Obot <danobot@hotmail.com>, Elizabeth Shockey <coffee@snob.beans>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

