# Comparing `tmp/replit-bot-4.2.4.tar.gz` & `tmp/replit-bot-4.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replit-bot-4.2.4.tar", max compression
+gzip compressed data, was "replit-bot-4.2.5.tar", max compression
```

## Comparing `replit-bot-4.2.4.tar` & `replit-bot-4.2.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1058 2023-03-18 03:10:39.175601 replit-bot-4.2.4/LICENSE
--rw-r--r--   0        0        0      858 2023-04-12 02:20:19.691873 replit-bot-4.2.4/pyproject.toml
--rw-r--r--   0        0        0    35555 2023-04-12 02:20:29.103860 replit-bot-4.2.4/replit_bot/AsyncBot.py
--rw-r--r--   0        0        0    50369 2023-04-12 02:20:29.827859 replit-bot-4.2.4/replit_bot/AsyncClient.py
--rw-r--r--   0        0        0     4849 2023-03-27 19:47:43.541064 replit-bot-4.2.4/replit_bot/AsyncPost_ql.py
--rw-r--r--   0        0        0     1052 2022-09-27 15:16:43.952285 replit-bot-4.2.4/replit_bot/LICENSE
--rw-r--r--   0        0        0      292 2023-04-12 02:20:13.555882 replit-bot-4.2.4/replit_bot/__init__.py
--rw-r--r--   0        0        0    18869 2023-03-28 03:01:12.062609 replit-bot-4.2.4/replit_bot/bot.py
--rw-r--r--   0        0        0    40595 2023-03-27 04:53:44.611007 replit-bot-4.2.4/replit_bot/client.py
--rw-r--r--   0        0        0      402 2022-10-16 23:52:32.225067 replit-bot-4.2.4/replit_bot/colors.py
--rw-r--r--   0        0        0      417 2022-10-31 16:25:47.277382 replit-bot-4.2.4/replit_bot/exceptions.py
--rw-r--r--   0        0        0      978 2023-03-28 14:54:09.153939 replit-bot-4.2.4/replit_bot/html_default_templates.py
--rw-r--r--   0        0        0      337 2022-11-01 05:08:17.261306 replit-bot-4.2.4/replit_bot/links.py
--rw-r--r--   0        0        0     1079 2023-03-18 17:19:56.099076 replit-bot-4.2.4/replit_bot/param.py
--rw-r--r--   0        0        0     4622 2023-03-17 18:28:40.859392 replit-bot-4.2.4/replit_bot/post_ql.py
--rw-r--r--   0        0        0    33930 2022-12-04 18:15:07.036375 replit-bot-4.2.4/replit_bot/queries.js
--rw-r--r--   0        0        0    66619 2023-04-12 02:20:28.443861 replit-bot-4.2.4/replit_bot/queries.py
--rw-r--r--   0        0        0      392 2022-10-25 21:03:02.210745 replit-bot-4.2.4/replit_bot/templates/index.html
--rw-r--r--   0        0        0     4592 2023-03-17 18:28:40.863392 replit-bot-4.2.4/replit_bot/utils/EventEmitter.py
--rw-r--r--   0        0        0      323 2022-10-17 16:19:01.766353 replit-bot-4.2.4/replit_bot/utils/JSDict.py
--rw-r--r--   0        0        0      333 2022-09-29 01:59:37.161531 replit-bot-4.2.4/replit_bot/utils/_uuid.py
--rw-r--r--   0        0        0     1055 2022-11-30 23:00:18.573144 replit-bot-4.2.4/replit_bot/utils/lines.py
--rw-r--r--   0        0        0      172 2022-10-17 16:19:01.778353 replit-bot-4.2.4/replit_bot/utils/switch.py
--rw-r--r--   0        0        0      879 2023-04-12 02:20:31.351770 replit-bot-4.2.4/setup.py
--rw-r--r--   0        0        0      758 2023-04-12 02:20:31.352069 replit-bot-4.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1058 2023-03-18 03:10:39.175601 replit-bot-4.2.5/LICENSE
+-rw-r--r--   0        0        0      822 2023-04-13 00:08:07.497490 replit-bot-4.2.5/pyproject.toml
+-rw-r--r--   0        0        0    35555 2023-04-12 02:20:29.103860 replit-bot-4.2.5/replit_bot/AsyncBot.py
+-rw-r--r--   0        0        0    50369 2023-04-12 02:20:29.827859 replit-bot-4.2.5/replit_bot/AsyncClient.py
+-rw-r--r--   0        0        0     4849 2023-03-27 19:47:43.541064 replit-bot-4.2.5/replit_bot/AsyncPost_ql.py
+-rw-r--r--   0        0        0     1052 2022-09-27 15:16:43.952285 replit-bot-4.2.5/replit_bot/LICENSE
+-rw-r--r--   0        0        0      292 2023-04-13 00:08:03.245496 replit-bot-4.2.5/replit_bot/__init__.py
+-rw-r--r--   0        0        0    18869 2023-03-28 03:01:12.062609 replit-bot-4.2.5/replit_bot/bot.py
+-rw-r--r--   0        0        0    40595 2023-03-27 04:53:44.611007 replit-bot-4.2.5/replit_bot/client.py
+-rw-r--r--   0        0        0      402 2022-10-16 23:52:32.225067 replit-bot-4.2.5/replit_bot/colors.py
+-rw-r--r--   0        0        0      417 2022-10-31 16:25:47.277382 replit-bot-4.2.5/replit_bot/exceptions.py
+-rw-r--r--   0        0        0      978 2023-03-28 14:54:09.153939 replit-bot-4.2.5/replit_bot/html_default_templates.py
+-rw-r--r--   0        0        0      337 2022-11-01 05:08:17.261306 replit-bot-4.2.5/replit_bot/links.py
+-rw-r--r--   0        0        0     1079 2023-03-18 17:19:56.099076 replit-bot-4.2.5/replit_bot/param.py
+-rw-r--r--   0        0        0     4622 2023-03-17 18:28:40.859392 replit-bot-4.2.5/replit_bot/post_ql.py
+-rw-r--r--   0        0        0    33930 2022-12-04 18:15:07.036375 replit-bot-4.2.5/replit_bot/queries.js
+-rw-r--r--   0        0        0    67496 2023-04-12 02:23:52.651575 replit-bot-4.2.5/replit_bot/queries.py
+-rw-r--r--   0        0        0      392 2022-10-25 21:03:02.210745 replit-bot-4.2.5/replit_bot/templates/index.html
+-rw-r--r--   0        0        0     4592 2023-03-17 18:28:40.863392 replit-bot-4.2.5/replit_bot/utils/EventEmitter.py
+-rw-r--r--   0        0        0      323 2022-10-17 16:19:01.766353 replit-bot-4.2.5/replit_bot/utils/JSDict.py
+-rw-r--r--   0        0        0      333 2022-09-29 01:59:37.161531 replit-bot-4.2.5/replit_bot/utils/_uuid.py
+-rw-r--r--   0        0        0     1055 2022-11-30 23:00:18.573144 replit-bot-4.2.5/replit_bot/utils/lines.py
+-rw-r--r--   0        0        0      172 2022-10-17 16:19:01.778353 replit-bot-4.2.5/replit_bot/utils/switch.py
+-rw-r--r--   0        0        0      823 2023-04-13 00:08:22.322365 replit-bot-4.2.5/setup.py
+-rw-r--r--   0        0        0      674 2023-04-13 00:08:22.322706 replit-bot-4.2.5/PKG-INFO
```

### Comparing `replit-bot-4.2.4/LICENSE` & `replit-bot-4.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.4/pyproject.toml` & `replit-bot-4.2.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "replit-bot"
-version = "4.2.4"
+version = "4.2.5"
 description = "make discord.py like bots on replit and/or do replapi-it style replit interactions"
 authors = ["bigminboss <you@example.com>"]
 
 [tool.poetry.dependencies]
 # python ver
 python = ">=3.6.1,<4.0.0"
 # replit db I think I can't remember lol
@@ -19,16 +19,14 @@
 # docs
 # [tool.poetry.group.docs]
 # optional = true
 
 # [tool.poetry.group.docs.dependencies]
 Flask = "^2.2.0"
 waitress = "^2.1.2"
-quart="^0.18.4"
-hypercorn="^0.14.3"
 
 [tool.poetry.dev-dependencies]
 debugpy = "^1.6.2"
 python-lsp-server = {extras = ["yapf", "rope", "pyflakes"], version = "^1.5.0"}
 toml = "^0.10.2"
 Markdown = "^3.4.1"
```

### Comparing `replit-bot-4.2.4/replit_bot/AsyncBot.py` & `replit-bot-4.2.5/replit_bot/AsyncBot.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.4/replit_bot/AsyncClient.py` & `replit-bot-4.2.5/replit_bot/AsyncClient.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.4/replit_bot/AsyncPost_ql.py` & `replit-bot-4.2.5/replit_bot/AsyncPost_ql.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.4/replit_bot/LICENSE` & `replit-bot-4.2.5/replit_bot/LICENSE`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.4/replit_bot/bot.py` & `replit-bot-4.2.5/replit_bot/bot.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.4/replit_bot/client.py` & `replit-bot-4.2.5/replit_bot/client.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.4/replit_bot/html_default_templates.py` & `replit-bot-4.2.5/replit_bot/html_default_templates.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.4/replit_bot/param.py` & `replit-bot-4.2.5/replit_bot/param.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.4/replit_bot/post_ql.py` & `replit-bot-4.2.5/replit_bot/post_ql.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.4/replit_bot/queries.js` & `replit-bot-4.2.5/replit_bot/queries.js`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.4/replit_bot/queries.py` & `replit-bot-4.2.5/replit_bot/queries.py`

 * *Files 2% similar despite different names*

```diff
@@ -412,14 +412,15 @@
   }
 }
 
 fragment ReplsDashboardReplItemRepl on Repl {
   id
 }""",
     "editComment": "mutation ReplViewCommentsUpdateReplComment($input: UpdateReplCommentInput!) {\n  updateReplComment(input: $input) {\n    ... on ReplComment {\n      id\n      body\n      __typename\n    }\n    ... on UserError {\n      message\n      __typename\n    }\n    __typename\n  }\n}\n",
+    "lastEditedRepls": "query HomeRecentRepls($count: Int!) {\n  ownRecentRepls: recentRepls(count: $count, filter: own) {\n    id\n    ...RecentRepl\n    __typename\n  }\n  multiplayerRecentRepls: recentRepls(count: $count, filter: multiplayer) {\n    id\n    ...RecentRepl\n    __typename\n  }\n  currentUser {\n    id\n    username\n    __typename\n  }\n}\n\nfragment RecentRepl on Repl {\n  id\n  title\n  iconUrl\n  ...ReplLinkRepl\n  owner {\n    ... on User {\n      id\n      ...RecentReplUser\n      __typename\n    }\n    ... on Team {\n      id\n      ...RecentReplTeam\n      __typename\n    }\n    __typename\n  }\n  __typename\n}\n\nfragment ReplLinkRepl on Repl {\n  id\n  url\n  nextPagePathname\n  __typename\n}\n\nfragment RecentReplUser on User {\n  id\n  username\n  __typename\n}\n\nfragment RecentReplTeam on Team {\n  id\n  username\n  __typename\n}\n",
 }
 
 """
 import { GraphQL } from '@rayhanadev/replit-gql';
 import gql from 'graphql-tag';
 import * as fs from 'fs';
 const client = GraphQL()
```

### Comparing `replit-bot-4.2.4/replit_bot/utils/EventEmitter.py` & `replit-bot-4.2.5/replit_bot/utils/EventEmitter.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.4/replit_bot/utils/lines.py` & `replit-bot-4.2.5/replit_bot/utils/lines.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.4/setup.py` & `replit-bot-4.2.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,24 +5,22 @@
 ['replit_bot', 'replit_bot.utils']
 
 package_data = \
 {'': ['*'], 'replit_bot': ['templates/*']}
 
 install_requires = \
 ['Flask>=2.2.0,<3.0.0',
- 'hypercorn>=0.14.3,<0.15.0',
  'pyee>=9.0.4,<10.0.0',
- 'quart>=0.18.4,<0.19.0',
  'replit>=3.2.4,<4.0.0',
  'requests>=2.28.1,<3.0.0',
  'waitress>=2.1.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'replit-bot',
-    'version': '4.2.4',
+    'version': '4.2.5',
     'description': 'make discord.py like bots on replit and/or do replapi-it style replit interactions',
     'long_description': None,
     'author': 'bigminboss',
     'author_email': 'you@example.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `replit-bot-4.2.4/PKG-INFO` & `replit-bot-4.2.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: replit-bot
-Version: 4.2.4
+Version: 4.2.5
 Summary: make discord.py like bots on replit and/or do replapi-it style replit interactions
 Author: bigminboss
 Author-email: you@example.com
 Requires-Python: >=3.6.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Flask (>=2.2.0,<3.0.0)
-Requires-Dist: hypercorn (>=0.14.3,<0.15.0)
 Requires-Dist: pyee (>=9.0.4,<10.0.0)
-Requires-Dist: quart (>=0.18.4,<0.19.0)
 Requires-Dist: replit (>=3.2.4,<4.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: waitress (>=2.1.2,<3.0.0)
```

