# Comparing `tmp/aiogram3_form-0.3.0.tar.gz` & `tmp/aiogram3_form-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram3_form-0.3.0.tar", max compression
+gzip compressed data, was "aiogram3_form-0.3.1.tar", max compression
```

## Comparing `aiogram3_form-0.3.0.tar` & `aiogram3_form-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      294 2023-01-24 13:28:23.727234 aiogram3_form-0.3.0/aiogram3_form/__init__.py
--rw-r--r--   0        0        0     1383 2023-04-13 18:33:34.599104 aiogram3_form-0.3.0/aiogram3_form/field.py
--rw-r--r--   0        0        0      843 2023-01-24 00:46:35.276915 aiogram3_form-0.3.0/aiogram3_form/filters.py
--rw-r--r--   0        0        0     8383 2023-04-13 18:34:48.537877 aiogram3_form-0.3.0/aiogram3_form/form.py
--rw-r--r--   0        0        0      120 2023-01-24 00:23:37.244911 aiogram3_form-0.3.0/aiogram3_form/state.py
--rw-r--r--   0        0        0     1092 2023-01-24 00:20:12.265098 aiogram3_form-0.3.0/LICENSE
--rw-r--r--   0        0        0      507 2023-04-13 18:36:04.952920 aiogram3_form-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1479 2023-01-24 00:20:12.265098 aiogram3_form-0.3.0/README.md
--rw-r--r--   0        0        0     2025 1970-01-01 00:00:00.000000 aiogram3_form-0.3.0/setup.py
--rw-r--r--   0        0        0     1973 1970-01-01 00:00:00.000000 aiogram3_form-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      294 2023-01-24 13:28:23.727234 aiogram3_form-0.3.1/aiogram3_form/__init__.py
+-rw-r--r--   0        0        0     1383 2023-04-13 18:33:34.599104 aiogram3_form-0.3.1/aiogram3_form/field.py
+-rw-r--r--   0        0        0      843 2023-01-24 00:46:35.276915 aiogram3_form-0.3.1/aiogram3_form/filters.py
+-rw-r--r--   0        0        0     8389 2023-04-13 18:41:26.226852 aiogram3_form-0.3.1/aiogram3_form/form.py
+-rw-r--r--   0        0        0      120 2023-01-24 00:23:37.244911 aiogram3_form-0.3.1/aiogram3_form/state.py
+-rw-r--r--   0        0        0     1092 2023-01-24 00:20:12.265098 aiogram3_form-0.3.1/LICENSE
+-rw-r--r--   0        0        0      507 2023-04-13 18:42:02.565611 aiogram3_form-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1479 2023-01-24 00:20:12.265098 aiogram3_form-0.3.1/README.md
+-rw-r--r--   0        0        0     2025 1970-01-01 00:00:00.000000 aiogram3_form-0.3.1/setup.py
+-rw-r--r--   0        0        0     1973 1970-01-01 00:00:00.000000 aiogram3_form-0.3.1/PKG-INFO
```

### Comparing `aiogram3_form-0.3.0/aiogram3_form/field.py` & `aiogram3_form-0.3.1/aiogram3_form/field.py`

 * *Files identical despite different names*

### Comparing `aiogram3_form-0.3.0/aiogram3_form/filters.py` & `aiogram3_form-0.3.1/aiogram3_form/filters.py`

 * *Files identical despite different names*

### Comparing `aiogram3_form-0.3.0/aiogram3_form/form.py` & `aiogram3_form-0.3.1/aiogram3_form/form.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
             )
 
         if not cls.__submit_callback:
             raise TypeError(
                 f"{cls.__name__} submit callback is {cls.__submit_callback}"
             )
 
-        form_object = cls.__from_state(state)
+        form_object = await cls.__from_state(state)
         data["state"] = state
 
         prepared_submit_callback = cls.__prepare_submit_callback(form_object, **data)
 
         try:
             await prepared_submit_callback()
         finally:
```

### Comparing `aiogram3_form-0.3.0/LICENSE` & `aiogram3_form-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogram3_form-0.3.0/README.md` & `aiogram3_form-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `aiogram3_form-0.3.0/setup.py` & `aiogram3_form-0.3.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['aiogram3_form']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'aiogram3-form',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'A library to create forms in aiogram3',
     'long_description': '# aiogram3-form\nA library to create forms in aiogram3\n\n# Example\n```Python\n# suppose you import here your router and bot objects\nfrom aiogram import F, types\n\nfrom aiogram3_form import Form, FormField\n\n\nclass NameForm(Form, router=your_router):\n    first_name: str = FormField(enter_message_text="Enter your first name please")\n    second_name: str = FormField(enter_message_text="Enter your second name please", filter=F.text.len() > 10)\n    age: int = FormField(enter_message_text="Enter age as integer", error_message_text="Age should be numeric!")\n\n\n@NameForm.submit()\nasync def name_form_submit_handler(form: NameForm, event_chat: types.Chat):\n    # handle form data\n    # also supports aiogram standart DI (e. g. middlewares, filters, etc)\n    await bot.send_message(\n        event_chat.id, f"Your full name is {form.first_name} {form.second_name}!"\n    )\n    \n    \n@router.message(F.text == "/form")\nasync def form_handler(message: types.Message, state: FSMContext):\n    await NameForm.start(state)  # start your form\n```\n\nAfter submit callback call the state would be automatically cleared.\n\nYou can control this state using the following metaclass kwarg\n\n```Python\n...\n\n\nclass NameForm(Form, clear_state_on_submit=False):  # True by default\n    ...\n\n\n@NameForm.submit()\nasync def name_form_submit_handler(form: NameForm, state: FSMContext):\n    # so you can set your exit state manually\n    await state.set_state(...)\n```\n',
     'author': 'TrixiS',
     'author_email': 'oficialmorozov@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `aiogram3_form-0.3.0/PKG-INFO` & `aiogram3_form-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogram3-form
-Version: 0.3.0
+Version: 0.3.1
 Summary: A library to create forms in aiogram3
 License: MIT
 Author: TrixiS
 Author-email: oficialmorozov@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

