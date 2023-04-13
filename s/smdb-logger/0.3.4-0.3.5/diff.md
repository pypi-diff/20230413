# Comparing `tmp/smdb_logger-0.3.4.tar.gz` & `tmp/smdb_logger-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smdb_logger-0.3.4.tar", last modified: Wed Feb 15 07:26:12 2023, max compression
+gzip compressed data, was "smdb_logger-0.3.5.tar", last modified: Thu Apr 13 12:11:25 2023, max compression
```

## Comparing `smdb_logger-0.3.4.tar` & `smdb_logger-0.3.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-02-15 07:26:12.216221 smdb_logger-0.3.4/
--rw-rw-rw-   0        0        0     4178 2023-02-15 07:26:12.216221 smdb_logger-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     3569 2022-07-15 12:30:38.000000 smdb_logger-0.3.4/README.md
--rw-rw-rw-   0        0        0      108 2021-03-04 15:16:38.000000 smdb_logger-0.3.4/pyproject.toml
--rw-rw-rw-   0        0        0      694 2023-02-15 07:26:12.217221 smdb_logger-0.3.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-15 07:26:12.205719 smdb_logger-0.3.4/smdb_logger/
--rw-rw-rw-   0        0        0    10205 2023-02-15 07:25:44.000000 smdb_logger-0.3.4/smdb_logger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-15 07:26:12.215721 smdb_logger-0.3.4/smdb_logger.egg-info/
--rw-rw-rw-   0        0        0     4178 2023-02-15 07:26:12.000000 smdb_logger-0.3.4/smdb_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-02-15 07:26:12.000000 smdb_logger-0.3.4/smdb_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-15 07:26:12.000000 smdb_logger-0.3.4/smdb_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-02-15 07:26:12.000000 smdb_logger-0.3.4/smdb_logger.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 12:11:25.688798 smdb_logger-0.3.5/
+-rw-rw-rw-   0        0        0     4178 2023-04-13 12:11:25.688798 smdb_logger-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3569 2022-07-15 12:30:38.000000 smdb_logger-0.3.5/README.md
+-rw-rw-rw-   0        0        0      108 2021-03-04 15:16:38.000000 smdb_logger-0.3.5/pyproject.toml
+-rw-rw-rw-   0        0        0      694 2023-04-13 12:11:25.693300 smdb_logger-0.3.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 12:11:25.680797 smdb_logger-0.3.5/smdb_logger/
+-rw-rw-rw-   0        0        0    10205 2023-04-13 12:10:50.000000 smdb_logger-0.3.5/smdb_logger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 12:11:25.688299 smdb_logger-0.3.5/smdb_logger.egg-info/
+-rw-rw-rw-   0        0        0     4178 2023-04-13 12:11:25.000000 smdb_logger-0.3.5/smdb_logger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-04-13 12:11:25.000000 smdb_logger-0.3.5/smdb_logger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 12:11:25.000000 smdb_logger-0.3.5/smdb_logger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-13 12:11:25.000000 smdb_logger-0.3.5/smdb_logger.egg-info/top_level.txt
```

### Comparing `smdb_logger-0.3.4/PKG-INFO` & `smdb_logger-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smdb_logger
-Version: 0.3.4
+Version: 0.3.5
 Summary: Logger used by Server Monitoring Discord Bot and all extentions made by me
 Home-page: https://github.com/NightKey/Server-monitoring-discord-bot
 Author: Janthó Dávid
 Author-email: davidjantho@gmail.com
 Project-URL: Bug Tracker, https://github.com/NightKey/Server-monitoring-discord-bot/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `smdb_logger-0.3.4/README.md` & `smdb_logger-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `smdb_logger-0.3.4/setup.cfg` & `smdb_logger-0.3.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 6d64 625f 6c6f 6767 6572 0d0a   = smdb_logger..
-00000020: 7665 7273 696f 6e20 3d20 302e 332e 340d  version = 0.3.4.
+00000020: 7665 7273 696f 6e20 3d20 302e 332e 350d  version = 0.3.5.
 00000030: 0a61 7574 686f 7220 3d20 4a61 6e74 68c3  .author = Janth.
 00000040: b320 44c3 a176 6964 0d0a 6175 7468 6f72  . D..vid..author
 00000050: 5f65 6d61 696c 203d 2064 6176 6964 6a61  _email = davidja
 00000060: 6e74 686f 4067 6d61 696c 2e63 6f6d 0d0a  ntho@gmail.com..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 4c6f  description = Lo
 00000080: 6767 6572 2075 7365 6420 6279 2053 6572  gger used by Ser
 00000090: 7665 7220 4d6f 6e69 746f 7269 6e67 2044  ver Monitoring D
```

### Comparing `smdb_logger-0.3.4/smdb_logger/__init__.py` & `smdb_logger-0.3.5/smdb_logger/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
                 previous_filename = path.basename(frame.filename)
             else:
                 caller = f"{frame.function}->{caller}"
         return f"{previous_filename}->{caller}" if self.use_file_names else caller
 
     def __log(self, level: LEVEL, data: str, counter: str, end: str) -> None:
         if (counter is None):
-            counter = str(self.get_date().strftime(r"%Y.%m.%d-%I:%M:%S"))
+            counter = str(self.get_date().strftime(r"%Y.%m.%d-%H:%M:%S"))
         log_msg = f"[{counter}] [{level.value}]: {data}"
         if self.header_used and level != LEVEL.HEADER:
             log_msg = f"\t{log_msg}"
         if self.level_only_valid_for_console or level in self.allowed:
             self.__log_to_file(log_msg)
         if self.log_to_console and level in self.allowed and level is not LEVEL.HEADER:
             if self.use_caller_name:
```

### Comparing `smdb_logger-0.3.4/smdb_logger.egg-info/PKG-INFO` & `smdb_logger-0.3.5/smdb_logger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smdb-logger
-Version: 0.3.4
+Version: 0.3.5
 Summary: Logger used by Server Monitoring Discord Bot and all extentions made by me
 Home-page: https://github.com/NightKey/Server-monitoring-discord-bot
 Author: Janthó Dávid
 Author-email: davidjantho@gmail.com
 Project-URL: Bug Tracker, https://github.com/NightKey/Server-monitoring-discord-bot/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

