# Comparing `tmp/beymax-1.1.0.tar.gz` & `tmp/beymax-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beymax-1.1.0.tar", last modified: Thu Mar 16 19:21:53 2023, max compression
+gzip compressed data, was "beymax-1.2.0.tar", last modified: Thu Apr 13 17:05:06 2023, max compression
```

## Comparing `beymax-1.1.0.tar` & `beymax-1.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 19:21:53.787443 beymax-1.1.0/
--rw-r--r--   0 root         (0) root         (0)     3834 2023-03-16 19:21:53.787443 beymax-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2988 2023-01-04 23:22:50.000000 beymax-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 19:21:53.779443 beymax-1.1.0/beymax/
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-03-16 18:34:54.000000 beymax-1.1.0/beymax/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7911 2023-03-16 18:34:54.000000 beymax-1.1.0/beymax/args.py
--rw-rw-rw-   0 root         (0) root         (0)    51033 2023-03-16 18:34:54.000000 beymax-1.1.0/beymax/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 19:21:53.787443 beymax-1.1.0/beymax/control/
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-02-07 22:15:41.000000 beymax-1.1.0/beymax/control/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7480 2023-02-17 22:30:18.000000 beymax-1.1.0/beymax/control/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4531 2023-03-01 20:30:50.000000 beymax-1.1.0/beymax/control/dummy.py
--rw-rw-rw-   0 root         (0) root         (0)    28557 2023-03-01 20:30:50.000000 beymax-1.1.0/beymax/control/webui.py
--rw-rw-rw-   0 root         (0) root         (0)     2068 2023-01-04 23:22:50.000000 beymax-1.1.0/beymax/db.py
--rw-rw-rw-   0 root         (0) root         (0)     9065 2023-03-01 20:30:50.000000 beymax-1.1.0/beymax/suite.py
--rw-rw-rw-   0 root         (0) root         (0)    13638 2023-02-09 23:29:34.000000 beymax-1.1.0/beymax/ui.py
--rw-rw-rw-   0 root         (0) root         (0)    15388 2023-01-04 23:22:50.000000 beymax-1.1.0/beymax/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 19:21:53.783443 beymax-1.1.0/beymax.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3834 2023-03-16 19:21:53.000000 beymax-1.1.0/beymax.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      374 2023-03-16 19:21:53.000000 beymax-1.1.0/beymax.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-16 19:21:53.000000 beymax-1.1.0/beymax.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2023-03-16 19:21:53.000000 beymax-1.1.0/beymax.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-03-16 19:21:53.000000 beymax-1.1.0/beymax.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-16 19:21:53.787443 beymax-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1091 2023-03-13 14:15:01.000000 beymax-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 17:05:06.571995 beymax-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)     3834 2023-04-13 17:05:06.571995 beymax-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2988 2023-04-13 16:47:35.000000 beymax-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 17:05:06.567995 beymax-1.2.0/beymax/
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-04-13 17:02:23.000000 beymax-1.2.0/beymax/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7911 2023-04-13 16:47:35.000000 beymax-1.2.0/beymax/args.py
+-rw-rw-rw-   0 root         (0) root         (0)    51180 2023-04-13 16:47:35.000000 beymax-1.2.0/beymax/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 17:05:06.571995 beymax-1.2.0/beymax/control/
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-04-13 16:47:35.000000 beymax-1.2.0/beymax/control/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7480 2023-04-13 16:47:35.000000 beymax-1.2.0/beymax/control/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4531 2023-04-13 16:47:35.000000 beymax-1.2.0/beymax/control/dummy.py
+-rw-rw-rw-   0 root         (0) root         (0)    29453 2023-04-13 16:47:35.000000 beymax-1.2.0/beymax/control/webui.py
+-rw-rw-rw-   0 root         (0) root         (0)     2068 2023-04-13 16:47:35.000000 beymax-1.2.0/beymax/db.py
+-rw-rw-rw-   0 root         (0) root         (0)     9247 2023-04-13 16:47:35.000000 beymax-1.2.0/beymax/suite.py
+-rw-rw-rw-   0 root         (0) root         (0)    13638 2023-04-13 16:47:35.000000 beymax-1.2.0/beymax/ui.py
+-rw-rw-rw-   0 root         (0) root         (0)    15388 2023-04-13 16:47:35.000000 beymax-1.2.0/beymax/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 17:05:06.571995 beymax-1.2.0/beymax.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3834 2023-04-13 17:05:06.000000 beymax-1.2.0/beymax.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      374 2023-04-13 17:05:06.000000 beymax-1.2.0/beymax.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 17:05:06.000000 beymax-1.2.0/beymax.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      110 2023-04-13 17:05:06.000000 beymax-1.2.0/beymax.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-13 17:05:06.000000 beymax-1.2.0/beymax.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 17:05:06.571995 beymax-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2023-04-13 16:47:35.000000 beymax-1.2.0/setup.py
```

### Comparing `beymax-1.1.0/PKG-INFO` & `beymax-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beymax
-Version: 1.1.0
+Version: 1.2.0
 Summary: A high-level, functional programming wrapper to discord.py
 Home-page: https://gitlab.graubert.com/agraubert/beymax
 Author: Aaron Graubert
 Author-email: aaron@graubert.com
 License: MIT
 Keywords: discord async asyncio sql sqlalchemy utilities
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `beymax-1.1.0/README.md` & `beymax-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `beymax-1.1.0/beymax/args.py` & `beymax-1.2.0/beymax/args.py`

 * *Files identical despite different names*

### Comparing `beymax-1.1.0/beymax/client.py` & `beymax-1.2.0/beymax/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -679,15 +679,18 @@
                 stack_trace=msg
             ))
             await session.commit()
         if interaction is not None and not interaction.response.is_done():
             await interaction.response.send_message(
                 "I was unable to complete this action because I encountered an unexpected error.\n"
                 "If you continue to encounter this problem, report it to {} and include this error trace ID\n"
-                "{}".format('(someone)', traceID),
+                "{}".format(
+                    (await self.controller.config_get('__global__', 'bug', 'url', default='your server administrators')),
+                    traceID
+                ),
                 ephemeral=True
             )
         return traceID
 
     async def shutdown(self, signal=None):
         """
         Coroutine. Use this function for a clean shutdown.
```

### Comparing `beymax-1.1.0/beymax/control/base.py` & `beymax-1.2.0/beymax/control/base.py`

 * *Files identical despite different names*

### Comparing `beymax-1.1.0/beymax/control/dummy.py` & `beymax-1.2.0/beymax/control/dummy.py`

 * *Files identical despite different names*

### Comparing `beymax-1.1.0/beymax/control/webui.py` & `beymax-1.2.0/beymax/control/webui.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,25 @@
 				if suite in req.dependencies
 			]
 			for suite in suites
 		}.items()
 		if len(deplist)
 	}
 
-WebControlEssentials = CommandSuite("WebUI Shard Essentials", force_enable=True)
+WebControlEssentials = CommandSuite("WebUI Shard Essentials", force_enable=True, metadata={
+	'webui.feature_description': {
+		'header': 'Full customization within each server',
+		'body': (
+			'Server administrators can run the /config command to log into a configuration page on this website.'
+			' Administrators can then enable and disable individual commands or command suites that they do or don\'t want in their server.'
+			' Don\'t like any of the features you see in this list? Leave them disabled in the config panel and none of your members will be able to use them.'
+			' For security reasons, all commands and command suites start disabled, giving you time to set appropriate permissions inside of discord.'
+		)
+	}
+})
 
 @WebControlEssentials.table
 class GuildInfo(object):
 	"""
 	Represents a suite being enabled.
 	Forced suites are NOT represented in this database
 	"""
@@ -696,14 +706,22 @@
 		suite_data = {
 			'default_config': build_default_control_config(self.client.suites.values()),
 			'suite_list': [
 				sanitize_suite_command_name(suite.name)
 				for suite in self.client.suites.values()
 			],
 			'dependencies': get_dependency_list(self.client.suites.values()),
+			'guild_config_schema': [
+				suite.get_meta('webui.config_schema')
+				for suite in self.client.suites.values()
+			],
+			'feature_description': [
+				suite.get_meta('webui.feature_description')
+				for suite in self.client.suites.values()
+			],
 			'channel_refs': [
 				*(
 					{
 						channel
 						for suite in self.client.suites.values()
 						for channel in suite.channels
 					} | {'general'}
```

### Comparing `beymax-1.1.0/beymax/db.py` & `beymax-1.2.0/beymax/db.py`

 * *Files identical despite different names*

### Comparing `beymax-1.1.0/beymax/suite.py` & `beymax-1.2.0/beymax/suite.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 logger = logging.getLogger('beymax.core.suite')
 
 class Schema(object):
     pass
 
 class CommandSuite(object):
-    def __init__(self, name, group_description=None, group_name=None, force_enable=False):
+    def __init__(self, name, group_description=None, group_name=None, force_enable=False, metadata=None):
         self.name = name
         self.bot = None
         self.commands = []
         self.tasks = []
         self.special = []
         self.subscriptions = []
         self.migrations = []
@@ -23,14 +23,15 @@
         self.context = []
         self.schema = Schema()
         self.dependencies = []
         self.dependents = []
         self.tables = []
         self.command_group = None
         self.forced = force_enable
+        self.metadata = metadata if metadata is not None else {}
         
         if self.forced:
             logger.info("Command suite {} marked as mandatory. Controllers should not disable this".format(self.name))
         
         if group_description is not None:
             logger.warning("Grouping commands in suite {}. Command permissions are fully grouped, so ensure it's okay to lose granular control".format(self.name))
             if group_name is None:
@@ -38,14 +39,17 @@
                 logger.debug("A group description was provided with no name. Auto-generating name for suite {}".format(name))
             self.command_group = discord.app_commands.Group(
                 name=group_name,
                 description=group_description,
                 default_permissions=discord.Permissions(use_application_commands=False)
             )
     
+    def get_meta(self, key):
+        return self.metadata[key] if key in self.metadata else None
+    
     def add_dependency(self, suite):
         self.dependencies.append(suite)
         suite.dependents.append(self)
 
     def table(self, cls):
         """
         Declare a new table for the database.
```

### Comparing `beymax-1.1.0/beymax/ui.py` & `beymax-1.2.0/beymax/ui.py`

 * *Files identical despite different names*

### Comparing `beymax-1.1.0/beymax/utils.py` & `beymax-1.2.0/beymax/utils.py`

 * *Files identical despite different names*

### Comparing `beymax-1.1.0/beymax.egg-info/PKG-INFO` & `beymax-1.2.0/beymax.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beymax
-Version: 1.1.0
+Version: 1.2.0
 Summary: A high-level, functional programming wrapper to discord.py
 Home-page: https://gitlab.graubert.com/agraubert/beymax
 Author: Aaron Graubert
 Author-email: aaron@graubert.com
 License: MIT
 Keywords: discord async asyncio sql sqlalchemy utilities
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `beymax-1.1.0/setup.py` & `beymax-1.2.0/setup.py`

 * *Files identical despite different names*

