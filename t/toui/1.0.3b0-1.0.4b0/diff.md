# Comparing `tmp/toui-1.0.3b0.tar.gz` & `tmp/toui-1.0.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toui-1.0.3b0.tar", last modified: Mon Apr 10 12:56:08 2023, max compression
+gzip compressed data, was "toui-1.0.4b0.tar", last modified: Thu Apr 13 08:28:44 2023, max compression
```

## Comparing `toui-1.0.3b0.tar` & `toui-1.0.4b0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 12:56:08.480316 toui-1.0.3b0/
--rw-rw-rw-   0        0        0     1094 2023-03-28 04:20:49.000000 toui-1.0.3b0/LICENSE
--rw-rw-rw-   0        0        0       16 2023-03-28 04:20:49.000000 toui-1.0.3b0/MANIFEST.in
--rw-rw-rw-   0        0        0     3054 2023-04-10 12:56:08.478312 toui-1.0.3b0/PKG-INFO
--rw-rw-rw-   0        0        0     2618 2023-03-28 05:00:34.000000 toui-1.0.3b0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 12:56:08.208619 toui-1.0.3b0/examples/
--rw-rw-rw-   0        0        0        0 2023-03-28 04:20:49.000000 toui-1.0.3b0/examples/__init__.py
--rw-rw-rw-   0        0        0      910 2023-03-28 04:20:49.000000 toui-1.0.3b0/examples/advanced_example_1_toui_blueprint.py
--rw-rw-rw-   0        0        0      556 2023-03-28 04:20:49.000000 toui-1.0.3b0/examples/example_1_simple_website.py
--rw-rw-rw-   0        0        0      535 2023-03-28 04:20:49.000000 toui-1.0.3b0/examples/example_2_simple_desktop_app.py
--rw-rw-rw-   0        0        0      762 2023-03-28 04:20:49.000000 toui-1.0.3b0/examples/example_3_updating_page.py
--rw-rw-rw-   0        0        0      699 2023-03-28 04:20:49.000000 toui-1.0.3b0/examples/example_4_function_with_arg.py
--rw-rw-rw-   0        0        0      995 2023-03-28 04:20:49.000000 toui-1.0.3b0/examples/example_5_user_variables.py
--rw-rw-rw-   0        0        0      162 2023-03-28 04:20:49.000000 toui-1.0.3b0/examples/example_6_quick_website.py
--rw-rw-rw-   0        0        0      166 2023-03-28 04:20:49.000000 toui-1.0.3b0/examples/example_7_quick_desktop_app.py
-drwxrwxrwx   0        0        0        0 2023-04-10 12:56:08.213604 toui-1.0.3b0/images/
--rw-rw-rw-   0        0        0    29049 2023-03-28 04:20:49.000000 toui-1.0.3b0/images/logo.png
--rw-rw-rw-   0        0        0       42 2023-04-10 12:56:08.481313 toui-1.0.3b0/setup.cfg
--rw-rw-rw-   0        0        0     1181 2023-03-28 04:20:49.000000 toui-1.0.3b0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 12:56:08.379602 toui-1.0.3b0/toui/
--rw-rw-rw-   0        0        0      213 2023-04-10 12:54:07.000000 toui-1.0.3b0/toui/__init__.py
--rw-rw-rw-   0        0        0      429 2023-03-28 04:20:49.000000 toui-1.0.3b0/toui/_defaults.py
--rw-rw-rw-   0        0        0     1093 2023-03-28 04:20:49.000000 toui-1.0.3b0/toui/_helpers.py
--rw-rw-rw-   0        0        0     4836 2023-03-28 04:20:49.000000 toui-1.0.3b0/toui/_javascript_templates.py
--rw-rw-rw-   0        0        0     2380 2023-03-28 04:20:49.000000 toui-1.0.3b0/toui/_signals.py
--rw-rw-rw-   0        0        0    20266 2023-03-28 04:20:49.000000 toui-1.0.3b0/toui/apps.py
--rw-rw-rw-   0        0        0    18917 2023-04-10 12:45:09.000000 toui-1.0.3b0/toui/elements.py
--rw-rw-rw-   0        0        0      168 2023-03-28 04:20:49.000000 toui-1.0.3b0/toui/exceptions.py
--rw-rw-rw-   0        0        0    14434 2023-03-28 04:20:49.000000 toui-1.0.3b0/toui/pages.py
--rw-rw-rw-   0        0        0     2350 2023-03-28 04:20:49.000000 toui-1.0.3b0/toui/structure.py
-drwxrwxrwx   0        0        0        0 2023-04-10 12:56:08.471334 toui-1.0.3b0/toui.egg-info/
--rw-rw-rw-   0        0        0     3054 2023-04-10 12:56:07.000000 toui-1.0.3b0/toui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      707 2023-04-10 12:56:07.000000 toui-1.0.3b0/toui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 12:56:07.000000 toui-1.0.3b0/toui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2023-04-10 12:56:07.000000 toui-1.0.3b0/toui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-10 12:56:07.000000 toui-1.0.3b0/toui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 08:28:44.218566 toui-1.0.4b0/
+-rw-rw-rw-   0        0        0     1094 2023-03-28 04:20:49.000000 toui-1.0.4b0/LICENSE
+-rw-rw-rw-   0        0        0       16 2023-03-28 04:20:49.000000 toui-1.0.4b0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3056 2023-04-13 08:28:44.215569 toui-1.0.4b0/PKG-INFO
+-rw-rw-rw-   0        0        0     2620 2023-04-13 08:05:30.000000 toui-1.0.4b0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 08:28:44.024555 toui-1.0.4b0/examples/
+-rw-rw-rw-   0        0        0        0 2023-03-28 04:20:49.000000 toui-1.0.4b0/examples/__init__.py
+-rw-rw-rw-   0        0        0      910 2023-04-13 08:21:09.000000 toui-1.0.4b0/examples/advanced_example_1_toui_blueprint.py
+-rw-rw-rw-   0        0        0      556 2023-03-28 04:20:49.000000 toui-1.0.4b0/examples/example_1_simple_website.py
+-rw-rw-rw-   0        0        0      535 2023-03-28 04:20:49.000000 toui-1.0.4b0/examples/example_2_simple_desktop_app.py
+-rw-rw-rw-   0        0        0      762 2023-03-28 04:20:49.000000 toui-1.0.4b0/examples/example_3_updating_page.py
+-rw-rw-rw-   0        0        0      699 2023-03-28 04:20:49.000000 toui-1.0.4b0/examples/example_4_function_with_arg.py
+-rw-rw-rw-   0        0        0      995 2023-03-28 04:20:49.000000 toui-1.0.4b0/examples/example_5_user_variables.py
+-rw-rw-rw-   0        0        0      162 2023-03-28 04:20:49.000000 toui-1.0.4b0/examples/example_6_quick_website.py
+-rw-rw-rw-   0        0        0      166 2023-03-28 04:20:49.000000 toui-1.0.4b0/examples/example_7_quick_desktop_app.py
+drwxrwxrwx   0        0        0        0 2023-04-13 08:28:44.029553 toui-1.0.4b0/images/
+-rw-rw-rw-   0        0        0    29049 2023-03-28 04:20:49.000000 toui-1.0.4b0/images/logo.png
+-rw-rw-rw-   0        0        0       42 2023-04-13 08:28:44.219566 toui-1.0.4b0/setup.cfg
+-rw-rw-rw-   0        0        0     1225 2023-04-13 08:27:05.000000 toui-1.0.4b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 08:28:44.123568 toui-1.0.4b0/toui/
+-rw-rw-rw-   0        0        0      213 2023-04-13 08:22:36.000000 toui-1.0.4b0/toui/__init__.py
+-rw-rw-rw-   0        0        0      429 2023-03-28 04:20:49.000000 toui-1.0.4b0/toui/_defaults.py
+-rw-rw-rw-   0        0        0     1093 2023-03-28 04:20:49.000000 toui-1.0.4b0/toui/_helpers.py
+-rw-rw-rw-   0        0        0     5234 2023-04-13 06:50:06.000000 toui-1.0.4b0/toui/_javascript_templates.py
+-rw-rw-rw-   0        0        0     2380 2023-03-28 04:20:49.000000 toui-1.0.4b0/toui/_signals.py
+-rw-rw-rw-   0        0        0    20272 2023-04-13 08:21:10.000000 toui-1.0.4b0/toui/apps.py
+-rw-rw-rw-   0        0        0    19360 2023-04-13 08:21:10.000000 toui-1.0.4b0/toui/elements.py
+-rw-rw-rw-   0        0        0      168 2023-03-28 04:20:49.000000 toui-1.0.4b0/toui/exceptions.py
+-rw-rw-rw-   0        0        0    14431 2023-04-13 08:21:10.000000 toui-1.0.4b0/toui/pages.py
+-rw-rw-rw-   0        0        0     2350 2023-03-28 04:20:49.000000 toui-1.0.4b0/toui/structure.py
+drwxrwxrwx   0        0        0        0 2023-04-13 08:28:44.208567 toui-1.0.4b0/toui.egg-info/
+-rw-rw-rw-   0        0        0     3056 2023-04-13 08:28:43.000000 toui-1.0.4b0/toui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      707 2023-04-13 08:28:43.000000 toui-1.0.4b0/toui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 08:28:43.000000 toui-1.0.4b0/toui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      125 2023-04-13 08:28:43.000000 toui-1.0.4b0/toui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-13 08:28:43.000000 toui-1.0.4b0/toui.egg-info/top_level.txt
```

### Comparing `toui-1.0.3b0/LICENSE` & `toui-1.0.4b0/LICENSE`

 * *Files identical despite different names*

### Comparing `toui-1.0.3b0/PKG-INFO` & `toui-1.0.4b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 1.0.3b0
+Version: 1.0.4b0
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Home-page: UNKNOWN
 Author: Mubarak Almehairbi
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 ToUI is a Python package for creating user interfaces (websites and desktop apps)
 from HTML easily. No JavaScript knowledge is required, but some knowledge of HTML
 is usually required.
 
 # Why ToUI
 - Converts HTML files into a responsive app.
 - Simple to understand for programmers who only know Python and HTML.
-- The method of creating websites and the method of creating desktop apps are similar, which makes it easy to convert a website to desktop app and vice versa.
+- The method of creating websites and the method of creating desktop apps are similar, which makes it easy to convert a website to a desktop app and vice versa.
 
 # How to install
 Run this command:
 ```shell
 pip install toui
 ```
```

### Comparing `toui-1.0.3b0/README.md` & `toui-1.0.4b0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ToUI is a Python package for creating user interfaces (websites and desktop apps)
 from HTML easily. No JavaScript knowledge is required, but some knowledge of HTML
 is usually required.
 
 # Why ToUI
 - Converts HTML files into a responsive app.
 - Simple to understand for programmers who only know Python and HTML.
-- The method of creating websites and the method of creating desktop apps are similar, which makes it easy to convert a website to desktop app and vice versa.
+- The method of creating websites and the method of creating desktop apps are similar, which makes it easy to convert a website to a desktop app and vice versa.
 
 # How to install
 Run this command:
 ```shell
 pip install toui
 ```
```

### Comparing `toui-1.0.3b0/examples/advanced_example_1_toui_blueprint.py` & `toui-1.0.4b0/examples/advanced_example_1_toui_blueprint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 ToUI Blueprints
 
 `ToUI.Blueprint` is a class that inherits `flask.Blueprint` and adds more methods to it.
 The difference between this class and `flask.Blueprint` is that you can add `Page`
-objects to this class. To learn how to use blueprints, check `flask's` documentation
+objects to this class. To learn how to use blueprints, check `Flask's` documentation
 https://flask.palletsprojects.com/.
 """
 from toui import Page, Website, ToUIBlueprint
 
 # create a blueprint
 blueprint = ToUIBlueprint("Blueprint", __name__)
 page = Page(html_str="<h1>This page is part of a blueprint</h1>", url="/")
```

### Comparing `toui-1.0.3b0/examples/example_1_simple_website.py` & `toui-1.0.4b0/examples/example_1_simple_website.py`

 * *Files identical despite different names*

### Comparing `toui-1.0.3b0/examples/example_2_simple_desktop_app.py` & `toui-1.0.4b0/examples/example_2_simple_desktop_app.py`

 * *Files identical despite different names*

### Comparing `toui-1.0.3b0/examples/example_3_updating_page.py` & `toui-1.0.4b0/examples/example_3_updating_page.py`

 * *Files identical despite different names*

### Comparing `toui-1.0.3b0/examples/example_4_function_with_arg.py` & `toui-1.0.4b0/examples/example_4_function_with_arg.py`

 * *Files identical despite different names*

### Comparing `toui-1.0.3b0/examples/example_5_user_variables.py` & `toui-1.0.4b0/examples/example_5_user_variables.py`

 * *Files identical despite different names*

### Comparing `toui-1.0.3b0/images/logo.png` & `toui-1.0.4b0/images/logo.png`

 * *Files identical despite different names*

### Comparing `toui-1.0.3b0/setup.py` & `toui-1.0.4b0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     version=version,
     author=author,
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     include_package_data=True,
+    package_data={'images': ['images/*']},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     py_modules=[package_name],
     install_requires=requirements
```

### Comparing `toui-1.0.3b0/toui/_helpers.py` & `toui-1.0.4b0/toui/_helpers.py`

 * *Files identical despite different names*

### Comparing `toui-1.0.3b0/toui/_javascript_templates.py` & `toui-1.0.4b0/toui/_javascript_templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,19 @@
 
 
 common_template = f"""
 function _getDoc() {{
     var input_elements = document.getElementsByTagName("input")
     for (var input_element of input_elements) {{
         input_element.setAttribute("value", input_element.value)
-        input_element.setAttribute("checked", input_element.checked)
+        if (input_element.checked == true) {{
+            input_element.setAttribute("checked", "")
+        }} else {{
+            input_element.removeAttribute("checked")
+        }}
     }}
     var serializer = new XMLSerializer()
     const doc = serializer.serializeToString(document)
     return doc
     }}
 
 function _setDoc(kwargs) {{
@@ -96,14 +100,22 @@
         element.value = kwargs['value']
     }}
     if (kwargs['name'] == 'checked') {{
         element.checked = kwargs['value']
     }}
 }}
 
+function _delAttr(kwargs) {{
+    var element = _getElement(kwargs['selector'])
+    element.removeAttribute(kwargs['name'])
+    if (kwargs['name'] == 'checked') {{
+        element.checked = false
+    }}
+}}
+
 function _setContent(kwargs) {{
     var element = _getElement(kwargs['selector'])
     element.innerHTML = kwargs['content']
 }}
 
 function _addContent(kwargs) {{
     var element = _getElement(kwargs['selector'])
@@ -138,14 +150,17 @@
     }}
     if (func == "_replaceElements") {{
         _replaceElements(kwargs)
     }}
     if (func == "_setAttr") {{
         _setAttr(kwargs)
     }}
+    if (func == "_delAttr") {{
+        _delAttr(kwargs)
+    }}
     if (func == "_setContent") {{
         _setContent(kwargs)
     }}
     if (func == "_addContent") {{
         _addContent(kwargs)
     }}
     if (func == "_setDoc") {{
```

### Comparing `toui-1.0.3b0/toui/_signals.py` & `toui-1.0.4b0/toui/_signals.py`

 * *Files identical despite different names*

### Comparing `toui-1.0.3b0/toui/apps.py` & `toui-1.0.4b0/toui/apps.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,26 +82,26 @@
         self.page = page
     def __call__(self, *args, **kwargs):
         return self.func(*args, **kwargs)
 
         
 class Website(_App):
     """
-    A class that create a web application from HTML files.
+    A class that creates a web application from HTML files.
 
     Attributes
     ----------
     flask_app: Flask
         ToUI creates web applications using `Flask`. You can access the `Flask` object using the attribute `flask_app`.
 
     forbidden_urls: list
         These are URLs that ToUI does not allow the user to use because ToUI uses them.
 
     user_vars: dict
-        A dictionary that stores data unique to each user. The data are stored in `flask` `session` object.
+        A dictionary that stores data unique to each user. The data are stored in a `flask` `session` object.
 
     pages: list
         A list of added `Page` objects.
 
     Examples
     --------
 
@@ -356,29 +356,29 @@
         self._validate_ws = func
 
 
     def set_data_validation(self, func):
         """
         Validate data received from JavaScript before using it.
 
-        ToUI receives data from JavaScript in the form of JSON object. To validate this data
+        ToUI receives data from JavaScript in the form of a JSON object. To validate this data
         before allowing ToUI to use it, input a function that checks the data. This function
         should have one argument `data` and should either return ``True`` or ``False``.
         If the function returns ``False``, the data will not be used by ToUI.
 
         Currently, the JSON object contains the following keys:
 
         {func: ...,
          args: ...,
          url: ...,
          html: ...}
 
         `func` contains the name of the Python function that should be called, `args` are the
         arguments of this function, `url` is the URL of the HTML page that sent the data, 'html'
-        if the HTML document itself as a string.
+        is the HTML document itself as a string.
         However, note that the structure of the JSON object might change in future versions of
         ToUI.
 
         Parameters
         ----------
         func: Callable
             A function that validates data received from JavaScript. It should have one argument
@@ -420,15 +420,15 @@
 
     def communicate(self, data_from_js):
         self.app._communicate(data_from_js, self.window)
 
 
 class DesktopApp(_App):
     """
-    A class that create a desktop application from HTML files.
+    A class that creates a desktop application from HTML files.
 
     Attributes
     ----------
     name: str
         The name of the app
 
     pages: list
```

### Comparing `toui-1.0.3b0/toui/elements.py` & `toui-1.0.4b0/toui/elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,22 @@
         js_args = []
         js_kwargs = _ElementSignal._default_kwargs(kwargs)
         js_kwargs['name'] = kwargs['name']
         js_kwargs['value'] = str(kwargs['value'])
         return {'func': js_func, 'args': js_args, 'kwargs': js_kwargs}
 
     @staticmethod
+    def del_attr(**kwargs):
+        js_func = "_delAttr"
+        js_args = []
+        js_kwargs = _ElementSignal._default_kwargs(kwargs)
+        js_kwargs['name'] = kwargs['name']
+        return {'func': js_func, 'args': js_args, 'kwargs': js_kwargs}
+
+    @staticmethod
     def set_content(**kwargs):
         js_func = "_setContent"
         js_args = []
         js_kwargs = _ElementSignal._default_kwargs(kwargs)
         js_kwargs['content'] = str(kwargs['content'])
         return {'func': js_func, 'args': js_args, 'kwargs': js_kwargs}
 
@@ -217,15 +225,15 @@
             If ``True``, the elements will be copied.
 
         attrs: dict, default=None
             Attributes other than ``class`` and ``name`` can be specified in this dictionary.
 
         Returns
         -------
-        elements_list: list
+        elements_list: list(Element)
             A list of `Element` objects that match the parameters.
 
         """
         if attrs is None:
             attrs = {}
         if class_name:
             attrs['class'] = class_name
@@ -298,14 +306,19 @@
         Returns
         -------
         bool
 
         """
         return self.get_attr(name) != None
 
+    @_ElementSignal()
+    def del_attr(self, name):
+        if self.has_attr(name):
+            del self._element.attrs[name]
+
     def get_id(self):
         """
         Gets the ``id`` attribute of the HTML element.
 
         Returns
         -------
         str
@@ -399,15 +412,15 @@
         self._manage_content_functions(content)
         content = str(content)
         content = BeautifulSoup(content, features="html.parser")
         self._element.append(content)
 
     def get_style_property(self, property):
         """
-        Gets the value of a CSS property inside ``style`` attribute.
+        Gets the value of a CSS property inside the ``style`` attribute.
 
         Parameters
         ----------
         property: str
             The name of the property
 
         Returns
@@ -427,15 +440,15 @@
                     property_value += str(v.value)
                     if v.unit is not None:
                         property_value += str(v.unit)
                 return property_value
 
     def set_style_property(self, property, value):
         """
-        Sets the value of a CSS property inside ``style`` attribute.
+        Sets the value of a CSS property inside the ``style`` attribute.
 
         Parameters
         ----------
         property: str
             The name of the property
 
         value: str
@@ -462,48 +475,48 @@
             new_style += f"{property_value};"
         if not property_is_set:
             new_style += f"{property}: {value};"
         self.set_attr(name="style", value=new_style)
 
     def get_width_property(self):
         """
-        Gets the value of the CSS property `width` inside ``style`` attribute.
+        Gets the value of the CSS property `width` inside the ``style`` attribute.
 
         Returns
         -------
         str
 
         """
         return self.get_style_property("width")
 
     def set_width_property(self, value):
         """
-        Sets the value of the CSS property `width` inside ``style`` attribute.
+        Sets the value of the CSS property `width` inside the ``style`` attribute.
 
         Parameters
         ----------
         value: str
 
         """
         self.set_style_property("width", value)
 
     def get_height_property(self):
         """
-        Gets the value of the CSS property `heigth` inside ``style`` attribute.
+        Gets the value of the CSS property `height` inside the ``style`` attribute.
 
         Returns
         -------
         str
 
         """
         return self.get_style_property("height")
 
     def set_height_property(self, value):
         """
-        Sets the value of the CSS property `height` inside ``style`` attribute.
+        Sets the value of the CSS property `height` inside the ``style`` attribute.
 
         Parameters
         ----------
         value: str
 
         """
         self.set_style_property("height", value)
```

### Comparing `toui-1.0.3b0/toui/pages.py` & `toui-1.0.4b0/toui/pages.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
     window: pywebview.Window, default = None
         A `pywebview.Window` object. It is automatically created when adding the `Page` to
         `DesktopApp` and running the app.
 
     view_func: Callable
         The view function of the `Page`. This is the function that will be decorated by
-        `Flask.route()` in when creating web apps.
+        `Flask.route()` when creating web apps.
 
     Examples
     --------
 
     Importing the class:
 
     >>> from toui import Page
```

### Comparing `toui-1.0.3b0/toui/structure.py` & `toui-1.0.4b0/toui/structure.py`

 * *Files identical despite different names*

### Comparing `toui-1.0.3b0/toui.egg-info/PKG-INFO` & `toui-1.0.4b0/toui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 1.0.3b0
+Version: 1.0.4b0
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Home-page: UNKNOWN
 Author: Mubarak Almehairbi
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 ToUI is a Python package for creating user interfaces (websites and desktop apps)
 from HTML easily. No JavaScript knowledge is required, but some knowledge of HTML
 is usually required.
 
 # Why ToUI
 - Converts HTML files into a responsive app.
 - Simple to understand for programmers who only know Python and HTML.
-- The method of creating websites and the method of creating desktop apps are similar, which makes it easy to convert a website to desktop app and vice versa.
+- The method of creating websites and the method of creating desktop apps are similar, which makes it easy to convert a website to a desktop app and vice versa.
 
 # How to install
 Run this command:
 ```shell
 pip install toui
 ```
```

### Comparing `toui-1.0.3b0/toui.egg-info/SOURCES.txt` & `toui-1.0.4b0/toui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

