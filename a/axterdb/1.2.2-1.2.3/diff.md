# Comparing `tmp/axterdb-1.2.2.tar.gz` & `tmp/axterdb-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axterdb-1.2.2.tar", last modified: Wed Apr 12 12:07:23 2023, max compression
+gzip compressed data, was "axterdb-1.2.3.tar", last modified: Thu Apr 13 06:28:18 2023, max compression
```

## Comparing `axterdb-1.2.2.tar` & `axterdb-1.2.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 12:07:23.664497 axterdb-1.2.2/
--rw-rw-rw-   0        0        0     1332 2023-03-31 15:59:42.000000 axterdb-1.2.2/.gitignore
--rw-rw-rw-   0        0        0      254 2023-03-30 18:58:35.000000 axterdb-1.2.2/.readthedocs
--rw-rw-rw-   0        0        0     1796 2023-04-12 12:07:23.663494 axterdb-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      819 2023-04-12 09:27:39.000000 axterdb-1.2.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-12 12:07:23.420230 axterdb-1.2.2/axterdb/
--rw-rw-rw-   0        0        0       21 2023-04-01 10:55:46.000000 axterdb-1.2.2/axterdb/__init__.py
--rw-rw-rw-   0        0        0    11782 2023-04-12 12:05:14.000000 axterdb-1.2.2/axterdb/client.py
--rw-rw-rw-   0        0        0     2279 2023-04-12 08:59:15.000000 axterdb-1.2.2/axterdb/errors.py
-drwxrwxrwx   0        0        0        0 2023-04-12 12:07:23.450826 axterdb-1.2.2/axterdb.egg-info/
--rw-rw-rw-   0        0        0     1796 2023-04-12 12:07:23.000000 axterdb-1.2.2/axterdb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2023-04-12 12:07:23.000000 axterdb-1.2.2/axterdb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 12:07:23.000000 axterdb-1.2.2/axterdb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-12 12:07:23.000000 axterdb-1.2.2/axterdb.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-12 12:07:23.516420 axterdb-1.2.2/docs/
--rw-rw-rw-   0        0        0      634 2023-03-30 18:44:09.000000 axterdb-1.2.2/docs/Makefile
--rw-rw-rw-   0        0        0      184 2023-04-01 12:22:26.000000 axterdb-1.2.2/docs/clients.rst
--rw-rw-rw-   0        0        0     2003 2023-04-12 11:26:14.000000 axterdb-1.2.2/docs/conf.py
-drwxrwxrwx   0        0        0        0 2023-04-12 12:07:23.531652 axterdb-1.2.2/docs/images/
--rw-rw-rw-   0        0        0     4286 2023-04-01 12:31:27.000000 axterdb-1.2.2/docs/images/axterdb_logo.ico
--rw-rw-rw-   0        0        0   554350 2023-03-26 12:45:44.000000 axterdb-1.2.2/docs/images/axterdb_logo.png
--rw-rw-rw-   0        0        0     1001 2023-04-01 12:49:29.000000 axterdb-1.2.2/docs/index.rst
--rw-rw-rw-   0        0        0      625 2023-04-01 12:36:25.000000 axterdb-1.2.2/docs/installing.rst
--rwxrwxrwx   0        0        0      800 2023-03-30 18:57:56.000000 axterdb-1.2.2/docs/make.bat
--rw-rw-rw-   0        0        0     2157 2023-04-12 08:54:03.000000 axterdb-1.2.2/docs/quickstart.rst
--rw-rw-rw-   0        0        0      243 2023-03-31 17:53:32.000000 axterdb-1.2.2/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-12 12:07:23.632218 axterdb-1.2.2/examples/
--rw-rw-rw-   0        0        0      515 2023-04-12 09:05:42.000000 axterdb-1.2.2/examples/basic.py
--rw-rw-rw-   0        0        0     1743 2023-04-12 12:06:50.000000 axterdb-1.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 12:07:23.664497 axterdb-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0       68 2023-04-12 08:23:46.000000 axterdb-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:28:18.235079 axterdb-1.2.3/
+-rw-rw-rw-   0        0        0     1332 2023-03-31 15:59:42.000000 axterdb-1.2.3/.gitignore
+-rw-rw-rw-   0        0        0      254 2023-03-30 18:58:35.000000 axterdb-1.2.3/.readthedocs
+-rw-rw-rw-   0        0        0     1796 2023-04-13 06:28:18.216074 axterdb-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      819 2023-04-12 09:27:39.000000 axterdb-1.2.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-13 06:28:17.330268 axterdb-1.2.3/axterdb/
+-rw-rw-rw-   0        0        0       21 2023-04-01 10:55:46.000000 axterdb-1.2.3/axterdb/__init__.py
+-rw-rw-rw-   0        0        0    11827 2023-04-13 06:27:04.000000 axterdb-1.2.3/axterdb/client.py
+-rw-rw-rw-   0        0        0     2279 2023-04-12 08:59:15.000000 axterdb-1.2.3/axterdb/errors.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:28:17.476117 axterdb-1.2.3/axterdb.egg-info/
+-rw-rw-rw-   0        0        0     1796 2023-04-13 06:28:17.000000 axterdb-1.2.3/axterdb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      449 2023-04-13 06:28:17.000000 axterdb-1.2.3/axterdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 06:28:17.000000 axterdb-1.2.3/axterdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-13 06:28:17.000000 axterdb-1.2.3/axterdb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 06:28:17.847430 axterdb-1.2.3/docs/
+-rw-rw-rw-   0        0        0      634 2023-03-30 18:44:09.000000 axterdb-1.2.3/docs/Makefile
+-rw-rw-rw-   0        0        0      184 2023-04-01 12:22:26.000000 axterdb-1.2.3/docs/clients.rst
+-rw-rw-rw-   0        0        0     2003 2023-04-12 11:26:14.000000 axterdb-1.2.3/docs/conf.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:28:18.185785 axterdb-1.2.3/docs/images/
+-rw-rw-rw-   0        0        0     4286 2023-04-01 12:31:27.000000 axterdb-1.2.3/docs/images/axterdb_logo.ico
+-rw-rw-rw-   0        0        0   554350 2023-03-26 12:45:44.000000 axterdb-1.2.3/docs/images/axterdb_logo.png
+-rw-rw-rw-   0        0        0     1001 2023-04-01 12:49:29.000000 axterdb-1.2.3/docs/index.rst
+-rw-rw-rw-   0        0        0      625 2023-04-01 12:36:25.000000 axterdb-1.2.3/docs/installing.rst
+-rwxrwxrwx   0        0        0      800 2023-03-30 18:57:56.000000 axterdb-1.2.3/docs/make.bat
+-rw-rw-rw-   0        0        0     2157 2023-04-12 08:54:03.000000 axterdb-1.2.3/docs/quickstart.rst
+-rw-rw-rw-   0        0        0      243 2023-03-31 17:53:32.000000 axterdb-1.2.3/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 06:28:18.214073 axterdb-1.2.3/examples/
+-rw-rw-rw-   0        0        0      515 2023-04-12 09:05:42.000000 axterdb-1.2.3/examples/basic.py
+-rw-rw-rw-   0        0        0     1743 2023-04-13 06:27:27.000000 axterdb-1.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 06:28:18.236075 axterdb-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0       68 2023-04-12 08:23:46.000000 axterdb-1.2.3/setup.py
```

### Comparing `axterdb-1.2.2/.gitignore` & `axterdb-1.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `axterdb-1.2.2/PKG-INFO` & `axterdb-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: axterdb
-Version: 1.2.2
+Version: 1.2.3
 Summary: A Python wrapper for AxterDB
 Author: AxterDB Development
 License: MIT
 Project-URL: Source, https://github.com/AxterDB/wrapper
 Project-URL: Documentation, https://axterdb.readthedocs.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `axterdb-1.2.2/README.rst` & `axterdb-1.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `axterdb-1.2.2/axterdb/client.py` & `axterdb-1.2.3/axterdb/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,21 +14,20 @@
 class Client():
     def __init__(self, *, name: str, key: str, host: str, show_keys: bool = False):
 
         self.name: str = name
         self.key: str = key
         self.host: str = host
         self.show_keys: bool = show_keys
-    
+
         self._headers: dict = {"KEY": f"{self.key}"}
         self._session: aiohttp.ClientSession = None
         self._connected: bool = False
         self._accepted_types = ["TEXT", "INT", "REAL", "NULL"]
 
-
     async def connect(self):
         """|coro|
 
         Connects to the database, checks if everything is correct.
 
         """
         logger.log(logging.INFO, "Connection to database started.")
@@ -56,15 +55,15 @@
         ConnectionFailure
             Connection to the instance failed
         AlreadyConnected
             Already connected to the specified database.
         """
         logger.log(logging.INFO, "Checking instance.")
         if self._connected:
-            raise AlreadyConnected(self.host, self.key, self.table, self.show_keys)            
+            raise AlreadyConnected(self.host, self.key, self.name, self.show_keys)            
         try:
             ip = self.host.split(":")[0]
             ipaddress.ip_address(ip)
         except ValueError:
             raise InvalidInstanceIP(self.host)
         
         try:
@@ -85,15 +84,15 @@
         NoAccess
             Key specified does not have access to the specified database
         AlreadyConnected
             Already connected to the specified database.
         """
         logger.log(logging.INFO, f"Checking access for key {self.key if self.show_keys else '[HIDDEN]'} to {self.name}")
         if self._connected:
-            raise AlreadyConnected(self.host, self.key, self.table, self.show_keys)
+            raise AlreadyConnected(self.host, self.key, self.name, self.show_keys)
         async with self._session.get(self.route(f"/me"), headers=self._headers) as response:
             if response.status == 200:
                 data = await response.json()
                 databases = data["detail"]["data"]["Databases"]
                 if self.name not in databases:
                     raise NoAccess(self.host, self.key, self.name, self.show_keys)
                 else:
@@ -174,14 +173,15 @@
             Returns a list of lists containing data, or an empty list if no data was found.
 
         Raises
         ------
         NotConnected
             Not connected to the database.
         """
+        print(asyncio.get_event_loop().is_closed())
         if not self._connected:
             raise NotConnected()
         data = kwargs
         headers = self._headers
         headers["table"] = table
         if amount: headers["amount"] = str(amount)
         async with self._session.get(self.route(f"/database/{self.name}/select"), headers=headers, json=data) as response:
```

### Comparing `axterdb-1.2.2/axterdb/errors.py` & `axterdb-1.2.3/axterdb/errors.py`

 * *Files identical despite different names*

### Comparing `axterdb-1.2.2/axterdb.egg-info/PKG-INFO` & `axterdb-1.2.3/axterdb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: axterdb
-Version: 1.2.2
+Version: 1.2.3
 Summary: A Python wrapper for AxterDB
 Author: AxterDB Development
 License: MIT
 Project-URL: Source, https://github.com/AxterDB/wrapper
 Project-URL: Documentation, https://axterdb.readthedocs.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `axterdb-1.2.2/docs/Makefile` & `axterdb-1.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `axterdb-1.2.2/docs/conf.py` & `axterdb-1.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `axterdb-1.2.2/docs/images/axterdb_logo.ico` & `axterdb-1.2.3/docs/images/axterdb_logo.ico`

 * *Files identical despite different names*

### Comparing `axterdb-1.2.2/docs/images/axterdb_logo.png` & `axterdb-1.2.3/docs/images/axterdb_logo.png`

 * *Files identical despite different names*

### Comparing `axterdb-1.2.2/docs/index.rst` & `axterdb-1.2.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `axterdb-1.2.2/docs/installing.rst` & `axterdb-1.2.3/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `axterdb-1.2.2/docs/make.bat` & `axterdb-1.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `axterdb-1.2.2/docs/quickstart.rst` & `axterdb-1.2.3/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `axterdb-1.2.2/examples/basic.py` & `axterdb-1.2.3/examples/basic.py`

 * *Files identical despite different names*

### Comparing `axterdb-1.2.2/pyproject.toml` & `axterdb-1.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=62.6,<66",
     "setuptools-scm>=6.2,<8",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "axterdb"
-version = "1.2.2"
+version = "1.2.3"
 authors = [
     {name = "AxterDB Development"}
 ]
 description = "A Python wrapper for AxterDB"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {text = "MIT"}
```

