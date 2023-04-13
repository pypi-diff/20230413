# Comparing `tmp/libMecapack-1.0.7.tar.gz` & `tmp/libMecapack-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libMecapack-1.0.7.tar", last modified: Wed Feb  8 14:59:33 2023, max compression
+gzip compressed data, was "libMecapack-1.1.0.tar", last modified: Thu Apr 13 07:59:48 2023, max compression
```

## Comparing `libMecapack-1.0.7.tar` & `libMecapack-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       13 2022-11-29 15:21:25.817371 libMecapack-1.0.7/.gitignore
--rw-r--r--   0        0        0       67 2022-11-29 13:46:18.455630 libMecapack-1.0.7/.pypirc
--rw-r--r--   0        0        0      633 2022-11-30 07:55:16.215729 libMecapack-1.0.7/.vscode/settings.json
--rw-r--r--   0        0        0      266 2022-12-14 14:51:21.580933 libMecapack-1.0.7/INFO.md
--rw-r--r--   0        0        0     1097 2022-11-29 12:05:05.935969 libMecapack-1.0.7/LICENSE
--rw-r--r--   0        0        0       18 2022-11-29 14:38:29.605246 libMecapack-1.0.7/README.md
--rw-r--r--   0        0        0      577 2022-11-30 08:10:35.020497 libMecapack-1.0.7/pyproject.toml
--rw-r--r--   0        0        0      641 2022-11-30 08:11:04.669385 libMecapack-1.0.7/pyproject_light.toml
--rw-r--r--   0        0        0       42 2021-02-16 15:25:25.299157 libMecapack-1.0.7/renovate.json
--rw-r--r--   0        0        0      117 2022-11-30 08:08:49.270760 libMecapack-1.0.7/requirements.txt
--rw-r--r--   0        0        0       65 2023-02-08 14:59:18.081332 libMecapack-1.0.7/src/libMecapack/__init__.py
--rw-r--r--   0        0        0     6401 2022-11-29 13:15:17.795125 libMecapack-1.0.7/src/libMecapack/libCfg.py
--rw-r--r--   0        0        0    32577 2022-11-30 07:57:15.855383 libMecapack-1.0.7/src/libMecapack/libExcel.py
--rw-r--r--   0        0        0    12321 2022-11-29 13:14:45.561854 libMecapack-1.0.7/src/libMecapack/libLog.py
--rw-r--r--   0        0        0    19439 2022-11-30 07:56:18.502716 libMecapack-1.0.7/src/libMecapack/libMail.py
--rw-r--r--   0        0        0     8411 2022-12-20 14:02:57.771474 libMecapack-1.0.7/src/libMecapack/libSql.py
--rw-r--r--   0        0        0     8620 2022-11-29 14:01:03.772459 libMecapack-1.0.7/src/libMecapack/libTool.py
--rw-r--r--   0        0        0    13833 2022-12-20 12:40:28.861770 libMecapack-1.0.7/src/libMecapack/libWebServices.py
--rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 libMecapack-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0       13 2022-11-29 15:21:25.817371 libMecapack-1.1.0/.gitignore
+-rw-r--r--   0        0        0       67 2022-11-29 13:46:18.455630 libMecapack-1.1.0/.pypirc
+-rw-r--r--   0        0        0      633 2022-11-30 07:55:16.215729 libMecapack-1.1.0/.vscode/settings.json
+-rw-r--r--   0        0        0      266 2022-12-14 14:51:21.580933 libMecapack-1.1.0/INFO.md
+-rw-r--r--   0        0        0     1097 2022-11-29 12:05:05.935969 libMecapack-1.1.0/LICENSE
+-rw-r--r--   0        0        0       18 2022-11-29 14:38:29.605246 libMecapack-1.1.0/README.md
+-rw-r--r--   0        0        0      603 2023-04-13 07:51:47.177622 libMecapack-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      667 2023-04-13 07:51:51.178911 libMecapack-1.1.0/pyproject_light.toml
+-rw-r--r--   0        0        0       42 2021-02-16 15:25:25.299157 libMecapack-1.1.0/renovate.json
+-rw-r--r--   0        0        0      136 2023-04-13 07:51:29.827515 libMecapack-1.1.0/requirements.txt
+-rw-r--r--   0        0        0       65 2023-04-13 07:53:36.039560 libMecapack-1.1.0/src/libMecapack/__init__.py
+-rw-r--r--   0        0        0     6401 2022-11-29 13:15:17.795125 libMecapack-1.1.0/src/libMecapack/libCfg.py
+-rw-r--r--   0        0        0    32577 2022-11-30 07:57:15.855383 libMecapack-1.1.0/src/libMecapack/libExcel.py
+-rw-r--r--   0        0        0    12321 2022-11-29 13:14:45.561854 libMecapack-1.1.0/src/libMecapack/libLog.py
+-rw-r--r--   0        0        0    19439 2022-11-30 07:56:18.502716 libMecapack-1.1.0/src/libMecapack/libMail.py
+-rw-r--r--   0        0        0     8411 2022-12-20 14:02:57.771474 libMecapack-1.1.0/src/libMecapack/libSql.py
+-rw-r--r--   0        0        0     8620 2022-11-29 14:01:03.772459 libMecapack-1.1.0/src/libMecapack/libTool.py
+-rw-r--r--   0        0        0    19307 2023-04-13 07:50:32.056831 libMecapack-1.1.0/src/libMecapack/libWebServices.py
+-rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 libMecapack-1.1.0/PKG-INFO
```

### Comparing `libMecapack-1.0.7/.vscode/settings.json` & `libMecapack-1.1.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `libMecapack-1.0.7/LICENSE` & `libMecapack-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libMecapack-1.0.7/pyproject.toml` & `libMecapack-1.1.0/pyproject_light.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
-name = "libMecapack"
+name = "libMecapack_light"
 authors = [
     {name = "Informatique Mecapack", email = "informatique@mecapack.com"},
 ]
 requires-python = ">=3.7"
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version", "description"]
 dependencies = [
     "arrow==1.2.3",
-    "openpyxl==3.0.10",
     "pypyodbc==1.3.6",
-    "pywin32==305",
     "requests==2.28.1",
     "suds==1.1.2",
-    "sortedcontainers==2.4.0"
-]
+    "sortedcontainers==2.4.0",
+    "xmltodict==0.13.0"
+]
+[tool.flit.sdist]
+exclude = ["src/libMecapack/libExcel.py"]
+[tool.flit.module]
+name = "libMecapack"
```

### Comparing `libMecapack-1.0.7/src/libMecapack/libCfg.py` & `libMecapack-1.1.0/src/libMecapack/libCfg.py`

 * *Files identical despite different names*

### Comparing `libMecapack-1.0.7/src/libMecapack/libExcel.py` & `libMecapack-1.1.0/src/libMecapack/libExcel.py`

 * *Files identical despite different names*

### Comparing `libMecapack-1.0.7/src/libMecapack/libLog.py` & `libMecapack-1.1.0/src/libMecapack/libLog.py`

 * *Files identical despite different names*

### Comparing `libMecapack-1.0.7/src/libMecapack/libMail.py` & `libMecapack-1.1.0/src/libMecapack/libMail.py`

 * *Files identical despite different names*

### Comparing `libMecapack-1.0.7/src/libMecapack/libSql.py` & `libMecapack-1.1.0/src/libMecapack/libSql.py`

 * *Files identical despite different names*

### Comparing `libMecapack-1.0.7/src/libMecapack/libTool.py` & `libMecapack-1.1.0/src/libMecapack/libTool.py`

 * *Files identical despite different names*

### Comparing `libMecapack-1.0.7/src/libMecapack/libWebServices.py` & `libMecapack-1.1.0/src/libMecapack/libWebServices.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,16 +6,18 @@
         none
     Return self
 """
 
 from datetime import datetime
 
 import requests
+import xmltodict
 from requests.auth import HTTPBasicAuth
 from suds.client import Client
+from urllib3.util import SKIP_HEADER
 
 import libMecapack.libLog as liblog
 
 
 class webServices_WSDL:
     """
     _summary_
@@ -322,15 +324,15 @@
 
     def _analyse_reponse_s9(self, reponse, CR):
         retour = {}
         if not isinstance(reponse["status"], dict):
             # Erreur
             self.log.Error(f"Erreur {reponse['status']} : {reponse['errors']}")
             retour["status"] = "ERREUR"
-            retour["info"] = CR.join([e["message"] + " : " + e["help"] for e in reponse["errors"]])
+            retour["info"] = CR.join([e.get("message", "") + " : " + e.get("help", "") for e in reponse["errors"]])
         elif "schema" in reponse:
             # saisie incomplète
             self.log.Error(f"Saisie incompète : {str(reponse['schema'])}")
             retour["status"] = "INCOMPLET"
             retour["info"] = reponse["schema"]
         elif reponse["status"]["success"]:
             retour["status"] = "OK"
@@ -374,7 +376,141 @@
                 k = ordre_colonne[idx]
                 if format[k] == "Boolean":
                     val[k] = True if e == "Vrai" else False
                 else:
                     val[k] = e
             retour.append(val)
         return retour
+
+
+class webServices_S9000:
+    """
+    _summary_
+
+    Raises:
+        Exception: _description_
+        Exception: _description_
+
+    Returns:
+        _type_: _description_
+    """
+
+    hshParam = {}
+    __hshData = {}
+
+    @property
+    def data(self):
+        return self.__hshData
+
+    def __init__(self, phshParam={}):
+        """permet la déclaration des variables de travail, et les init de variables de base
+        Keyword arguments :
+            phshParam -- the parameters dictionary
+        Return self
+        """
+        # Work variables
+        self.token = ""
+        self.login = ""
+
+        # Start log manager
+        self.log = liblog.Log()
+        self.session = requests.Session()
+        # Update of parameters
+        self.headers = {
+            "Content-Type": "text/xml; charset=utf-8",
+            "SOAPAction": "{address}/{request}",
+            "Except": "100-continue",
+            "Cache-Control": "no-cache",
+            "Accept-Encoding": SKIP_HEADER,
+        }
+        self.body = """<?xml version="1.0" encoding="utf-8"?>
+            <soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope" xmlns:soapenc="http://schemas.xmlsoap.org/soap/encoding/" xmlns:tns="http://s9.mecapack.com:8091/webservice_test/ws_complet.php" xmlns:types="http://s9.mecapack.com:8091/webservice_test/ws_complet.php/encodedTypes" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
+                <soap:Body soap:encodingStyle="http://schemas.xmlsoap.org/soap/encoding/">
+                    <q1:{request} xmlns:q1="http://s9.mecapack.com:8091/webservice_test/ws_complet.php?wsdl">
+                        <Login xsi:type="xsd:string">{user}</Login>
+                        <Password xsi:type="xsd:string">{password}</Password>
+                        {param}
+                    </q1:{request}>
+                </soap:Body>
+            </soap:Envelope>
+            """
+
+        self.hshParam.update(phshParam)
+
+    def Call(self, pqueryfilter, pbind=None, pparameters=None, **kw):
+        """
+        Lancement du web services avec infos à passer et résultats stockés dans data
+
+        Args:
+            pqueryfilter (str): filter string in queries dictionary
+            pparameters (xml, optional): dict of key, value to send. Defaults to None.
+
+        Options:
+            plogrequest (LOG_LEVEL): Log level display for request. "None" for no display (default=DEBUG)
+
+        Raises:
+            Exception: No connection
+
+        Returns:
+            cls: Self
+        """
+        hshOption = {"plogrequest": "DEBUG"}
+        # Setting dictionary option
+        if isinstance(kw, dict):
+            hshOption.update(kw)
+        address = self.hshParam["address"]
+        site = f"{address}?wsdl"
+        user = self.hshParam["user"]
+        password = self.hshParam["password"]
+        for key, infos in filter(
+            lambda x: pqueryfilter == x[0][: len(pqueryfilter)],
+            self.hshParam["request"].items(),
+        ):
+            self.log.setStep = f"R[{key}]"
+            if hshOption["plogrequest"]:
+                self.log.Write(
+                    self.log.LEVEL[hshOption["plogrequest"]],
+                    f"Request {key} : {site}",
+                )
+            headers = self.headers.copy()
+            request = infos["action"]
+            if pparameters:
+                param = infos["param"].format(**pparameters)  # NOQA
+            else:
+                param = infos["param"]
+            headers["SOAPAction"] = headers["SOAPAction"].format(**locals())
+            body = self.body.format(**locals()).replace("\n", "")
+            resp = self.session.post(
+                site,
+                headers=headers,
+                data=body,
+            )
+            # Pour débugage plus poussé
+            # req = requests.Request("POST", site, headers=headers, data=body)
+            # prepared = req.prepare()
+            # del prepared.headers["accept-encoding"]
+            # resp = self.session.send(prepared)
+            if resp.status_code != 200:
+                try:
+                    # Récupérer le message contenu dans le xml
+                    msg = xmltodict.parse(resp.text)["SOAP-ENV:Envelope"]["SOAP-ENV:Body"]["SOAP-ENV:Fault"]
+                except Exception:
+                    msg = resp.text
+                raise Exception(f"get /{pqueryfilter}/ {resp.status_code} : {msg}")
+            # Transcrire le XML et récupérer le contenu significatif
+            content = xmltodict.parse(resp.text)["SOAP-ENV:Envelope"]["SOAP-ENV:Body"][f"ns1:{request}Response"][
+                "return"
+            ]
+            if content["type_erreur"]["#text"] != "000":
+                # ERREUR d'envoi
+                raise Exception(f"retour /{pqueryfilter}/: {content['msg_erreur']['#text']}")
+            else:
+                # décoder HTML
+                if "xml" in content:
+                    self.__hshData[key] = xmltodict.parse(content["xml"]["#text"])
+                else:
+                    res = {}
+                    for k, v in content.items():
+                        if "#text" in v:
+                            res[k] = v["#text"]
+                    self.__hshData[key] = res
+            self.log.setStep = ""
```

### Comparing `libMecapack-1.0.7/PKG-INFO` & `libMecapack-1.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: libMecapack
-Version: 1.0.7
+Version: 1.1.0
 Summary: Library for MECAPACK python system
 Author-email: Informatique Mecapack <informatique@mecapack.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: arrow==1.2.3
 Requires-Dist: openpyxl==3.0.10
 Requires-Dist: pypyodbc==1.3.6
 Requires-Dist: pywin32==305
 Requires-Dist: requests==2.28.1
 Requires-Dist: suds==1.1.2
 Requires-Dist: sortedcontainers==2.4.0
+Requires-Dist: xmltodict==0.13.0
 
 Tools for Mecapack
```

