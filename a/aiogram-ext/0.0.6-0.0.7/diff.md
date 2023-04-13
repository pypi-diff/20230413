# Comparing `tmp/aiogram-ext-0.0.6.tar.gz` & `tmp/aiogram-ext-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram-ext-0.0.6.tar", last modified: Wed Apr 12 14:38:37 2023, max compression
+gzip compressed data, was "aiogram-ext-0.0.7.tar", last modified: Thu Apr 13 14:03:04 2023, max compression
```

## Comparing `aiogram-ext-0.0.6.tar` & `aiogram-ext-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,20 @@
--rw-r--r--   0        0        0      465 2023-04-12 10:53:39.977438 aiogram-ext-0.0.6/aiogram_ext/__init__.py
--rw-r--r--   0        0        0     1175 2023-04-12 11:18:11.688903 aiogram-ext-0.0.6/aiogram_ext/buttons.py
--rw-r--r--   0        0        0     1651 2023-04-12 11:05:16.344725 aiogram-ext-0.0.6/aiogram_ext/context.py
--rw-r--r--   0        0        0     1132 2023-04-12 11:08:54.370551 aiogram-ext-0.0.6/aiogram_ext/deps.py
--rw-r--r--   0        0        0     5887 2023-04-12 11:08:56.310732 aiogram-ext-0.0.6/aiogram_ext/dispatcher.py
--rw-r--r--   0        0        0     3800 2023-04-11 11:53:07.707408 aiogram-ext-0.0.6/aiogram_ext/filters.py
--rw-r--r--   0        0        0      459 2023-04-12 10:56:42.149572 aiogram-ext-0.0.6/aiogram_ext/helpers.py
--rw-r--r--   0        0        0      722 2023-04-12 14:37:01.113297 aiogram-ext-0.0.6/aiogram_ext/keyboards.py
--rw-r--r--   0        0        0      154 2023-04-12 10:34:24.400978 aiogram-ext-0.0.6/aiogram_ext/middlewares/__init__.py
--rw-r--r--   0        0        0     6983 2023-04-12 10:34:24.432621 aiogram-ext-0.0.6/aiogram_ext/middlewares/_conversation.py
--rw-r--r--   0        0        0     1534 2023-04-11 11:53:07.675758 aiogram-ext-0.0.6/aiogram_ext/middlewares/_membership.py
--rw-r--r--   0        0        0     1503 2023-04-11 11:53:07.675758 aiogram-ext-0.0.6/aiogram_ext/middlewares/misc.py
--rw-r--r--   0        0        0     2178 2023-04-11 11:53:07.691383 aiogram-ext-0.0.6/aiogram_ext/middlewares/throttling.py
--rw-r--r--   0        0        0      300 2023-04-12 14:38:14.534221 aiogram-ext-0.0.6/pyproject.toml
--rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-ext-0.0.6/README.md
--rw-r--r--   0        0        0      152 1970-01-01 00:00:00.000000 aiogram-ext-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      855 2023-04-13 14:00:40.168816 aiogram-ext-0.0.7/aiogram_ext/__init__.py
+-rw-r--r--   0        0        0     1175 2023-04-12 11:18:11.688903 aiogram-ext-0.0.7/aiogram_ext/buttons.py
+-rw-r--r--   0        0        0      269 2023-04-13 14:01:13.830112 aiogram-ext-0.0.7/aiogram_ext/config.py
+-rw-r--r--   0        0        0     1651 2023-04-12 11:05:16.344725 aiogram-ext-0.0.7/aiogram_ext/context.py
+-rw-r--r--   0        0        0     1483 2023-04-13 14:00:40.159310 aiogram-ext-0.0.7/aiogram_ext/deps.py
+-rw-r--r--   0        0        0     5887 2023-04-12 11:08:56.310732 aiogram-ext-0.0.7/aiogram_ext/dispatcher.py
+-rw-r--r--   0        0        0      892 2023-04-10 18:37:24.358984 aiogram-ext-0.0.7/aiogram_ext/env.py
+-rw-r--r--   0        0        0     3800 2023-04-11 11:53:07.707408 aiogram-ext-0.0.7/aiogram_ext/filters.py
+-rw-r--r--   0        0        0      459 2023-04-12 10:56:42.149572 aiogram-ext-0.0.7/aiogram_ext/helpers.py
+-rw-r--r--   0        0        0      722 2023-04-12 14:37:01.113297 aiogram-ext-0.0.7/aiogram_ext/keyboards.py
+-rw-r--r--   0        0        0      786 2023-04-12 16:54:57.221455 aiogram-ext-0.0.7/aiogram_ext/loader.py
+-rw-r--r--   0        0        0      154 2023-04-12 10:34:24.400978 aiogram-ext-0.0.7/aiogram_ext/middlewares/__init__.py
+-rw-r--r--   0        0        0     6983 2023-04-12 10:34:24.432621 aiogram-ext-0.0.7/aiogram_ext/middlewares/_conversation.py
+-rw-r--r--   0        0        0     1534 2023-04-11 11:53:07.675758 aiogram-ext-0.0.7/aiogram_ext/middlewares/_membership.py
+-rw-r--r--   0        0        0     1503 2023-04-11 11:53:07.675758 aiogram-ext-0.0.7/aiogram_ext/middlewares/misc.py
+-rw-r--r--   0        0        0     2178 2023-04-11 11:53:07.691383 aiogram-ext-0.0.7/aiogram_ext/middlewares/throttling.py
+-rw-r--r--   0        0        0      594 2023-04-13 13:42:05.708666 aiogram-ext-0.0.7/aiogram_ext/texts.py
+-rw-r--r--   0        0        0      367 2023-04-13 14:02:02.519348 aiogram-ext-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-ext-0.0.7/README.md
+-rw-r--r--   0        0        0      152 1970-01-01 00:00:00.000000 aiogram-ext-0.0.7/PKG-INFO
```

### Comparing `aiogram-ext-0.0.6/aiogram_ext/buttons.py` & `aiogram-ext-0.0.7/aiogram_ext/buttons.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.6/aiogram_ext/context.py` & `aiogram-ext-0.0.7/aiogram_ext/context.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.6/aiogram_ext/deps.py` & `aiogram-ext-0.0.7/aiogram_ext/deps.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from copy import deepcopy
+from os import environ
+from typing import TypeVar, Callable, Any
 
 from aiogram import Bot, Dispatcher
+from aiogram.contrib.fsm_storage.mongo import MongoStorage
 from aiogram.dispatcher import FSMContext
-from aiogram.dispatcher.filters.state import State
+from aiogram.dispatcher.filters.state import State, StatesGroup
+from aiogram.dispatcher.handler import SkipHandler, CancelHandler
 from aiogram.types import (
     ReplyKeyboardMarkup,
     InlineKeyboardMarkup,
     InlineKeyboardButton,
     KeyboardButton,
     Update,
     Message,
@@ -46,8 +50,16 @@
     "Poll",
     "PollAnswer",
     "ChatMemberUpdated",
     "executor",
     "deepcopy",
     "ReplyKeyboardRemove",
     "State",
+    "TypeVar",
+    "Callable",
+    "Any",
+    "environ",
+    "MongoStorage",
+    "SkipHandler",
+    "CancelHandler",
+    "StatesGroup",
 ]
```

### Comparing `aiogram-ext-0.0.6/aiogram_ext/dispatcher.py` & `aiogram-ext-0.0.7/aiogram_ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.6/aiogram_ext/filters.py` & `aiogram-ext-0.0.7/aiogram_ext/filters.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.6/aiogram_ext/keyboards.py` & `aiogram-ext-0.0.7/aiogram_ext/keyboards.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.6/aiogram_ext/middlewares/_conversation.py` & `aiogram-ext-0.0.7/aiogram_ext/middlewares/_conversation.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.6/aiogram_ext/middlewares/_membership.py` & `aiogram-ext-0.0.7/aiogram_ext/middlewares/_membership.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.6/aiogram_ext/middlewares/misc.py` & `aiogram-ext-0.0.7/aiogram_ext/middlewares/misc.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.6/aiogram_ext/middlewares/throttling.py` & `aiogram-ext-0.0.7/aiogram_ext/middlewares/throttling.py`

 * *Files identical despite different names*

