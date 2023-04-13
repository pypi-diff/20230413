# Comparing `tmp/hawc_client-2023.1-py3-none-any.whl.zip` & `tmp/hawc_client-2023.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 17350 bytes, number of entries: 19
--rw-r--r--  2.0 unx     2176 b- defN 23-Jan-09 22:42 hawc_client/__init__.py
+Zip file size: 17775 bytes, number of entries: 19
+-rw-r--r--  2.0 unx     2624 b- defN 23-Apr-13 12:09 hawc_client/__init__.py
 -rw-r--r--  2.0 unx     5664 b- defN 22-Dec-15 14:30 hawc_client/animal.py
 -rw-r--r--  2.0 unx      432 b- defN 22-Dec-15 14:30 hawc_client/assessment.py
 -rw-r--r--  2.0 unx      601 b- defN 22-Jan-13 04:24 hawc_client/client.py
 -rw-r--r--  2.0 unx    19298 b- defN 22-Dec-15 14:30 hawc_client/epi.py
 -rw-r--r--  2.0 unx      616 b- defN 22-Jan-13 04:24 hawc_client/epimeta.py
 -rw-r--r--  2.0 unx      460 b- defN 22-Jan-13 04:24 hawc_client/exceptions.py
 -rw-r--r--  2.0 unx      592 b- defN 22-Jan-13 04:24 hawc_client/invitro.py
--rw-r--r--  2.0 unx    11251 b- defN 22-Dec-15 14:30 hawc_client/literature.py
--rw-r--r--  2.0 unx     8027 b- defN 23-Jan-05 20:07 hawc_client/riskofbias.py
--rw-r--r--  2.0 unx     5105 b- defN 22-Dec-15 14:30 hawc_client/session.py
--rw-r--r--  2.0 unx     3429 b- defN 22-Dec-15 14:30 hawc_client/study.py
+-rw-r--r--  2.0 unx    11733 b- defN 23-Apr-13 12:09 hawc_client/literature.py
+-rw-r--r--  2.0 unx     8031 b- defN 23-Apr-13 12:09 hawc_client/riskofbias.py
+-rw-r--r--  2.0 unx     5744 b- defN 23-Apr-13 12:09 hawc_client/session.py
+-rw-r--r--  2.0 unx     3429 b- defN 23-Apr-13 12:09 hawc_client/study.py
 -rw-r--r--  2.0 unx     1519 b- defN 22-Dec-06 03:01 hawc_client/summary.py
--rw-r--r--  2.0 unx     1358 b- defN 23-Jan-05 20:07 hawc_client/utils.py
+-rw-r--r--  2.0 unx     1358 b- defN 23-Jan-12 22:48 hawc_client/utils.py
 -rw-r--r--  2.0 unx     1212 b- defN 22-Dec-15 14:30 hawc_client/vocab.py
--rw-r--r--  2.0 unx     1057 b- defN 23-Jan-09 22:43 hawc_client-2023.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-09 22:43 hawc_client-2023.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jan-09 22:43 hawc_client-2023.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1501 b- defN 23-Jan-09 22:43 hawc_client-2023.1.dist-info/RECORD
-19 files, 64402 bytes uncompressed, 14926 bytes compressed:  76.8%
+-rw-r--r--  2.0 unx     1057 b- defN 23-Apr-13 13:48 hawc_client-2023.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-13 13:48 hawc_client-2023.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Apr-13 13:48 hawc_client-2023.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1501 b- defN 23-Apr-13 13:48 hawc_client-2023.2.dist-info/RECORD
+19 files, 65975 bytes uncompressed, 15351 bytes compressed:  76.7%
```

## zipnote {}

```diff
@@ -39,20 +39,20 @@
 
 Filename: hawc_client/utils.py
 Comment: 
 
 Filename: hawc_client/vocab.py
 Comment: 
 
-Filename: hawc_client-2023.1.dist-info/METADATA
+Filename: hawc_client-2023.2.dist-info/METADATA
 Comment: 
 
-Filename: hawc_client-2023.1.dist-info/WHEEL
+Filename: hawc_client-2023.2.dist-info/WHEEL
 Comment: 
 
-Filename: hawc_client-2023.1.dist-info/top_level.txt
+Filename: hawc_client-2023.2.dist-info/top_level.txt
 Comment: 
 
-Filename: hawc_client-2023.1.dist-info/RECORD
+Filename: hawc_client-2023.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hawc_client/__init__.py

```diff
@@ -8,15 +8,15 @@
 from .literature import LiteratureClient
 from .riskofbias import RiskOfBiasClient
 from .session import HawcSession
 from .study import StudyClient
 from .summary import SummaryClient
 from .vocab import VocabClient
 
-__version__ = "2023.1"
+__version__ = "2023.2"
 __all__ = ["BaseClient", "HawcClient", "HawcClientException", "HawcServerException"]
 
 
 class HawcClient(BaseClient):
     """
     HAWC Client.
 
@@ -51,15 +51,22 @@
 
         Args:
             email (str): email to authenticate
             password (str): password to authenticate
         """
         self.session.authenticate(email, password)
 
-    def set_authentication_token(self, token: str) -> dict:
+    def set_authentication_token(self, token: str, login: bool = False) -> bool:
         """
-        Set authentication token (browser session specific)
+        Set authentication token for hawc client session.
 
         Args:
             token (str): authentication token from your user profile
+            login (bool, default False): if True, creates a django cookie-based session for HAWC
+                similar to a standard web-browser. If False (default), creates a token-
+                based django session for using the API. Requests using cookie-based sessions
+                require CSRF tokens, so form functionality will be limited.
+
+        Returns
+            bool: Returns true if session is valid
         """
-        return self.session.set_authentication_token(token)
+        return self.session.set_authentication_token(token, login)
```

## hawc_client/literature.py

```diff
@@ -184,15 +184,29 @@
 
         Args:
             assessment_id (int): Assessment ID
 
         Returns:
             pd.DataFrame: References data
         """
-        url = f"{self.session.root_url}/lit/api/assessment/{assessment_id}/references-download/"
+        url = f"{self.session.root_url}/lit/api/assessment/{assessment_id}/reference-export/"
+        response_json = self.session.get(url).json()
+        return pd.DataFrame(response_json)
+
+    def reference_user_tags(self, assessment_id: int) -> pd.DataFrame:
+        """
+        Retrieves all user tag for all references for an assessment.
+
+        Args:
+            assessment_id (int): Assessment ID
+
+        Returns:
+            pd.DataFrame: References user tag data
+        """
+        url = f"{self.session.root_url}/lit/api/assessment/{assessment_id}/user-tag-export/"
         response_json = self.session.get(url).json()
         return pd.DataFrame(response_json)
 
     def reference(self, reference_id: int) -> dict:
         """
         Retrieves the selected reference.
```

## hawc_client/riskofbias.py

```diff
@@ -7,30 +7,30 @@
 
 
 class RiskOfBiasClient(BaseClient):
     """
     Client class for risk of bias requests.
     """
 
-    def data(self, assessment_id: int) -> pd.DataFrame:
+    def export(self, assessment_id: int) -> pd.DataFrame:
         """
         Retrieves risk of bias data for the given assessment.
         This includes only final reviews.
 
         Args:
             assessment_id (int): Assessment ID
 
         Returns:
             pd.DataFrame: Risk of bias data
         """
         url = f"{self.session.root_url}/rob/api/assessment/{assessment_id}/export/"
         response_json = self.session.get(url).json()
         return pd.DataFrame(response_json)
 
-    def full_data(self, assessment_id: int) -> pd.DataFrame:
+    def full_export(self, assessment_id: int) -> pd.DataFrame:
         """
         Retrieves full risk of bias data for the given assessment.
         This includes user-level reviews.
 
         Args:
             assessment_id (int): Assessment ID
```

## hawc_client/session.py

```diff
@@ -110,26 +110,39 @@
         url = f"{self.root_url}/user/api/token-auth/"
         data = {"username": email, "password": password}
         response = self._session.post(url, json=data)
         self._handle_hawc_response(response)
         token = response.json()["token"]
         self._session.headers.update(Authorization=f"Token {token}")
 
-    def set_authentication_token(self, token: str) -> dict:
+    def set_authentication_token(self, token: str, login: bool = False) -> bool:
         """
-        Set authentication token (browser session specific)
+        Set authentication token for hawc client session.
 
         Args:
             token (str): authentication token from your user profile
+            login (bool, default False): if True, creates a django cookie-based session for HAWC
+                similar to a standard web-browser. If False (default), creates a token-
+                based django session for using the API. Requests using cookie-based sessions
+                require CSRF tokens, so form functionality will be limited.
+
+        Returns
+            bool: Returns true if session is valid
         """
+        params = {}
+        if login:
+            params["login"] = 1
         self._session.headers.update(Authorization=f"Token {token}")
         url = f"{self.root_url}/user/api/validate-token/"
-        return self.get(url).json()
+        response = self.get(url, params).json()
+        if login:
+            self._session.headers.pop("Authorization")
+        return response["valid"]
 
-    def iter_pages(self, url: str, params: dict = None) -> Generator:
+    def iter_pages(self, url: str, params: Optional[dict] = None) -> Generator:
         """
         Generator that crawls paginated HAWC responses.
 
         Args:
             url (str): URL for GET request.
             params (dict, optional): GET parameters to include. Defaults to None.
```

## Comparing `hawc_client-2023.1.dist-info/METADATA` & `hawc_client-2023.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hawc-client
-Version: 2023.1
+Version: 2023.2
 Summary: A client for the Health Assessment Workspace Collaborative (HAWC)
 Home-page: https://github.com/shapiromatron/hawc
 Maintainer: The HAWC development team
 Maintainer-email: shapiromatron@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/shapiromatron/hawc/issues
 Project-URL: Documentation, https://hawc.readthedocs.io/client/
```

## Comparing `hawc_client-2023.1.dist-info/RECORD` & `hawc_client-2023.2.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-hawc_client/__init__.py,sha256=7Se9kgbqcYOUwcisRQAZNO-z8SjiaZD1qZXoiuKH1_E,2176
+hawc_client/__init__.py,sha256=fUfwvogldUXkG_x2L3X2N5EPrccGUAKWlljEvftb6Ks,2624
 hawc_client/animal.py,sha256=KBteJyE1JelLhH7ZcuQhHc4Wi0fUIScEr52k8fIPzU4,5664
 hawc_client/assessment.py,sha256=aWCwykM-vZJY3KNuKd6V56UvGdZFj2rMdNYbITAhIEI,432
 hawc_client/client.py,sha256=a2ztwyLyIo7N8nLbhK7EAQfhnk-0OGY7Qu7QHUUX4zw,601
 hawc_client/epi.py,sha256=R6nzPcygbcZw2AqnT_Q8vZdB2RIA7cMd-l5EKZoFOlI,19298
 hawc_client/epimeta.py,sha256=ICG3ugJbBEp9fGRzIy0x2FLatGQtvjCEWSPrbOa5JaM,616
 hawc_client/exceptions.py,sha256=pMohVQ2v9jruP3iyH04qGxaTaYqGJ3KzrZifRp2x7tk,460
 hawc_client/invitro.py,sha256=vT5Z5tUen04ksDzOfxsyhNHhWDAsyMI-1dlbErINLZA,592
-hawc_client/literature.py,sha256=PhVJ7TsUx_iDnZS23A0rjO8izD9GTN8_-eJCjqLKq4c,11251
-hawc_client/riskofbias.py,sha256=dZ9CgB23ho0T7ZjLPUPcvLqXvB-nHrlH9Ij2u5OK-ZI,8027
-hawc_client/session.py,sha256=Tg-x14L8DZjZ31mKA41qmIheesvH8xYFmZ_-r2qjBmE,5105
+hawc_client/literature.py,sha256=jTfKfRRwWURFzV2IWNiLSb-lacAg15dK_QGYMemED80,11733
+hawc_client/riskofbias.py,sha256=gn3IOt6H1Wr0ReCTgJvBn-uWp__t0GM5RNu3qGls-Xk,8031
+hawc_client/session.py,sha256=45-vTNEw8aGJ-73FMYd9QMeELVAA3lZHF0jhEgjC9ks,5744
 hawc_client/study.py,sha256=Z-TJuREkup5Xe8A8M_P4ERogu5ThvunuP1EDJR_Jpgg,3429
 hawc_client/summary.py,sha256=JBCAiKYcB2tGi56g6MjMiOHolzO75_rN-twMYcsz3ls,1519
 hawc_client/utils.py,sha256=U13HYlKEdcJ31kDbbgnLk4zpBXXX5Hst0XwxAPJv0DM,1358
 hawc_client/vocab.py,sha256=m7VkpG6eElhxqy9emfebf8B_55fkDHALA4en-uZ9vIc,1212
-hawc_client-2023.1.dist-info/METADATA,sha256=m8fPO-CPbXI1tDFOWRDar9TQXF14ln1OMvWdeHvMZtA,1057
-hawc_client-2023.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-hawc_client-2023.1.dist-info/top_level.txt,sha256=ENf81ZlZh21EorGmdYtLOz8aT_CCBcpXjfz3AOQWV6c,12
-hawc_client-2023.1.dist-info/RECORD,,
+hawc_client-2023.2.dist-info/METADATA,sha256=ch-7JHpAk1Po9XeizejznC7BEJY_RNSXimGKS_yHoc4,1057
+hawc_client-2023.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+hawc_client-2023.2.dist-info/top_level.txt,sha256=ENf81ZlZh21EorGmdYtLOz8aT_CCBcpXjfz3AOQWV6c,12
+hawc_client-2023.2.dist-info/RECORD,,
```

