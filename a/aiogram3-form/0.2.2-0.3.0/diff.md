# Comparing `tmp/aiogram3_form-0.2.2.tar.gz` & `tmp/aiogram3_form-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram3_form-0.2.2.tar", max compression
+gzip compressed data, was "aiogram3_form-0.3.0.tar", max compression
```

## Comparing `aiogram3_form-0.2.2.tar` & `aiogram3_form-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      294 2023-01-24 13:28:23.727234 aiogram3_form-0.2.2/aiogram3_form/__init__.py
--rw-r--r--   0        0        0     1420 2023-02-03 16:05:28.945716 aiogram3_form-0.2.2/aiogram3_form/field.py
--rw-r--r--   0        0        0      843 2023-01-24 00:46:35.276915 aiogram3_form-0.2.2/aiogram3_form/filters.py
--rw-r--r--   0        0        0     7855 2023-02-19 16:03:46.210723 aiogram3_form-0.2.2/aiogram3_form/form.py
--rw-r--r--   0        0        0      120 2023-01-24 00:23:37.244911 aiogram3_form-0.2.2/aiogram3_form/state.py
--rw-r--r--   0        0        0     1092 2023-01-24 00:20:12.265098 aiogram3_form-0.2.2/LICENSE
--rw-r--r--   0        0        0      507 2023-02-19 16:03:57.312455 aiogram3_form-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1479 2023-01-24 00:20:12.265098 aiogram3_form-0.2.2/README.md
--rw-r--r--   0        0        0     2025 1970-01-01 00:00:00.000000 aiogram3_form-0.2.2/setup.py
--rw-r--r--   0        0        0     1973 1970-01-01 00:00:00.000000 aiogram3_form-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      294 2023-01-24 13:28:23.727234 aiogram3_form-0.3.0/aiogram3_form/__init__.py
+-rw-r--r--   0        0        0     1383 2023-04-13 18:33:34.599104 aiogram3_form-0.3.0/aiogram3_form/field.py
+-rw-r--r--   0        0        0      843 2023-01-24 00:46:35.276915 aiogram3_form-0.3.0/aiogram3_form/filters.py
+-rw-r--r--   0        0        0     8383 2023-04-13 18:34:48.537877 aiogram3_form-0.3.0/aiogram3_form/form.py
+-rw-r--r--   0        0        0      120 2023-01-24 00:23:37.244911 aiogram3_form-0.3.0/aiogram3_form/state.py
+-rw-r--r--   0        0        0     1092 2023-01-24 00:20:12.265098 aiogram3_form-0.3.0/LICENSE
+-rw-r--r--   0        0        0      507 2023-04-13 18:36:04.952920 aiogram3_form-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1479 2023-01-24 00:20:12.265098 aiogram3_form-0.3.0/README.md
+-rw-r--r--   0        0        0     2025 1970-01-01 00:00:00.000000 aiogram3_form-0.3.0/setup.py
+-rw-r--r--   0        0        0     1973 1970-01-01 00:00:00.000000 aiogram3_form-0.3.0/PKG-INFO
```

### Comparing `aiogram3_form-0.2.2/aiogram3_form/field.py` & `aiogram3_form-0.3.0/aiogram3_form/field.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from dataclasses import dataclass
-from typing import Any, Awaitable, Callable, Optional, Type, Union
+from typing import Any, Awaitable, Callable, Dict, Optional, Type, Union
 
 from aiogram import types
 from aiogram.utils.magic_filter import MagicFilter
 
 Markup = Union[types.ReplyKeyboardMarkup, types.InlineKeyboardMarkup]
 FormFilter = Union[MagicFilter, Callable[..., Awaitable[Any]]]
 
-# TODO: pass di data into enter callback
-EnterCallback = Callable[[int, int, "FormFieldData"], Awaitable[Any]]
+EnterCallback = Callable[[int, int, Dict[str, Any]], Awaitable[Any]]
 
 
 @dataclass(frozen=True)
 class FormFieldInfo:
     enter_message_text: Optional[str]
     error_message_text: Optional[str]
     filter: Optional[FormFilter]
```

### Comparing `aiogram3_form-0.2.2/aiogram3_form/filters.py` & `aiogram3_form-0.3.0/aiogram3_form/filters.py`

 * *Files identical despite different names*

### Comparing `aiogram3_form-0.2.2/aiogram3_form/form.py` & `aiogram3_form-0.3.0/aiogram3_form/form.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import functools
 import inspect
 from abc import ABC, ABCMeta
-from typing import Any, Callable, ClassVar, Optional, Set, Type, Union
+from typing import Any, Callable, ClassVar, Dict, Optional, Set, Type, Union
 
 from aiogram import types
 from aiogram.dispatcher.router import Router
 from aiogram.fsm.context import FSMContext
 from aiogram.utils.magic_filter import MagicFilter
 
 from . import filters
@@ -44,24 +44,28 @@
         return super().__new__(cls, cls_name, parents, cls_dict)
 
 
 class Form(ABC, metaclass=FormMeta, router=None):  # type: ignore
     __registered_forms: Set[Type["Form"]] = set()
     __submit_callback: Optional[SubmitCallback] = None
 
+    def __init__(self, state: FSMContext):
+        self.state = state
+
     @classmethod
     def submit(cls):
         def decorator(submit_callback: SubmitCallback):
             cls.__submit_callback = submit_callback
 
         return decorator
 
     @classmethod
-    def __from_state_data(cls, state_data):
-        form_object = cls()
+    async def __from_state(cls, state: FSMContext):
+        state_data = await state.get_data()
+        form_object = cls(state)
         form_object.__dict__.update(state_data["__form_values"])
         return form_object
 
     @classmethod
     def __get_filter_from_type(cls, field_type: Type):
         field_filter = filters.DEFAULT_FORM_FILTERS.get(field_type)
 
@@ -129,15 +133,15 @@
             __current_field_name=first_field.name,  # type: ignore
             __form_values={},
             __form_name=cls.__name__,
         )
 
         if first_field.info.enter_callback:
             await first_field.info.enter_callback(
-                state_ctx.key.chat_id, state_ctx.key.user_id, first_field
+                state_ctx.key.chat_id, state_ctx.key.user_id, {}
             )
         else:
             await state_ctx.bot.send_message(
                 state_ctx.key.chat_id,
                 first_field.info.enter_message_text,  # type: ignore
                 reply_markup=first_field.info.reply_markup or REMOVE_MARKUP,  # type: ignore
             )
@@ -161,33 +165,33 @@
         current_field_name: str = state_data["__current_field_name"]
         state_data["__form_values"][current_field_name] = value
         await state.set_data(state_data)
 
         next_field = cls.__get_next_field(current_field_name)
 
         if next_field:
-            await state.update_data(__current_field_name=next_field.name)
+            state_data["__current_field_name"] = next_field.name
+            await state.set_data(state_data)
 
             if next_field.info.enter_callback:
                 return await next_field.info.enter_callback(
-                    state.key.chat_id, state.key.user_id, next_field
+                    state.key.chat_id, state.key.user_id, state_data
                 )
 
             return await message.answer(
                 next_field.info.enter_message_text,  # type: ignore
                 reply_markup=next_field.info.reply_markup or REMOVE_MARKUP,
             )
 
         if not cls.__submit_callback:
             raise TypeError(
                 f"{cls.__name__} submit callback is {cls.__submit_callback}"
             )
 
-        state_data = await state.get_data()
-        form_object = cls.__from_state_data(state_data)
+        form_object = cls.__from_state(state)
         data["state"] = state
 
         prepared_submit_callback = cls.__prepare_submit_callback(form_object, **data)
 
         try:
             await prepared_submit_callback()
         finally:
@@ -234,7 +238,22 @@
         if current_field.info.error_message_text:
             await message.answer(
                 current_field.info.error_message_text,
                 reply_markup=current_field.info.reply_markup or REMOVE_MARKUP,
             )
 
         return False
+
+    async def answer(
+        self,
+        text: str,
+        reply_markup: Union[
+            types.InlineKeyboardMarkup,
+            types.ReplyKeyboardMarkup,
+            types.ReplyKeyboardRemove,
+            types.ForceReply,
+            None,
+        ] = None,
+    ):
+        await self.state.bot.send_message(
+            self.state.key.chat_id, text=text, reply_markup=reply_markup
+        )
```

### Comparing `aiogram3_form-0.2.2/LICENSE` & `aiogram3_form-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogram3_form-0.2.2/README.md` & `aiogram3_form-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `aiogram3_form-0.2.2/setup.py` & `aiogram3_form-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['aiogram3_form']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'aiogram3-form',
-    'version': '0.2.2',
+    'version': '0.3.0',
     'description': 'A library to create forms in aiogram3',
     'long_description': '# aiogram3-form\nA library to create forms in aiogram3\n\n# Example\n```Python\n# suppose you import here your router and bot objects\nfrom aiogram import F, types\n\nfrom aiogram3_form import Form, FormField\n\n\nclass NameForm(Form, router=your_router):\n    first_name: str = FormField(enter_message_text="Enter your first name please")\n    second_name: str = FormField(enter_message_text="Enter your second name please", filter=F.text.len() > 10)\n    age: int = FormField(enter_message_text="Enter age as integer", error_message_text="Age should be numeric!")\n\n\n@NameForm.submit()\nasync def name_form_submit_handler(form: NameForm, event_chat: types.Chat):\n    # handle form data\n    # also supports aiogram standart DI (e. g. middlewares, filters, etc)\n    await bot.send_message(\n        event_chat.id, f"Your full name is {form.first_name} {form.second_name}!"\n    )\n    \n    \n@router.message(F.text == "/form")\nasync def form_handler(message: types.Message, state: FSMContext):\n    await NameForm.start(state)  # start your form\n```\n\nAfter submit callback call the state would be automatically cleared.\n\nYou can control this state using the following metaclass kwarg\n\n```Python\n...\n\n\nclass NameForm(Form, clear_state_on_submit=False):  # True by default\n    ...\n\n\n@NameForm.submit()\nasync def name_form_submit_handler(form: NameForm, state: FSMContext):\n    # so you can set your exit state manually\n    await state.set_state(...)\n```\n',
     'author': 'TrixiS',
     'author_email': 'oficialmorozov@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `aiogram3_form-0.2.2/PKG-INFO` & `aiogram3_form-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogram3-form
-Version: 0.2.2
+Version: 0.3.0
 Summary: A library to create forms in aiogram3
 License: MIT
 Author: TrixiS
 Author-email: oficialmorozov@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

