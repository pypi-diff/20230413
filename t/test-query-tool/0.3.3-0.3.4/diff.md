# Comparing `tmp/test_query_tool-0.3.3.tar.gz` & `tmp/test_query_tool-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_query_tool-0.3.3.tar", last modified: Thu Apr 13 12:15:13 2023, max compression
+gzip compressed data, was "test_query_tool-0.3.4.tar", last modified: Thu Apr 13 18:13:05 2023, max compression
```

## Comparing `test_query_tool-0.3.3.tar` & `test_query_tool-0.3.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 12:15:13.855438 test_query_tool-0.3.3/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-03 17:08:00.000000 test_query_tool-0.3.3/LICENSE
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       45 2023-04-05 19:58:10.000000 test_query_tool-0.3.3/MANIFEST.in
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      323 2023-04-13 12:15:13.855096 test_query_tool-0.3.3/PKG-INFO
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 12:15:13.846949 test_query_tool-0.3.3/query_tool/
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     3372 2023-04-13 12:14:05.000000 test_query_tool-0.3.3/query_tool/__init__.py
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 12:15:13.844643 test_query_tool-0.3.3/query_tool/frontend/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 12:15:13.847918 test_query_tool-0.3.3/query_tool/frontend/dist/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 12:15:13.848682 test_query_tool-0.3.3/query_tool/frontend/dist/assets/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-04-13 12:07:36.000000 test_query_tool-0.3.3/query_tool/frontend/dist/assets/index-d081bea5.css
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1044760 2023-04-13 12:07:36.000000 test_query_tool-0.3.3/query_tool/frontend/dist/assets/index-d72f7278.js
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      463 2023-04-13 12:07:46.000000 test_query_tool-0.3.3/query_tool/frontend/dist/index.html
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-04-13 12:07:36.000000 test_query_tool-0.3.3/query_tool/frontend/dist/vite.svg
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 12:15:13.852544 test_query_tool-0.3.3/query_tool/services/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-03 16:47:55.000000 test_query_tool-0.3.3/query_tool/services/__init__.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1438 2023-04-03 16:47:55.000000 test_query_tool-0.3.3/query_tool/services/dimension_service.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3941 2023-04-03 16:47:55.000000 test_query_tool-0.3.3/query_tool/services/entities_service.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3653 2023-04-03 16:47:55.000000 test_query_tool-0.3.3/query_tool/services/filters_service.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      437 2023-04-03 16:47:55.000000 test_query_tool-0.3.3/query_tool/services/query_tool_factory.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1987 2023-04-03 16:47:55.000000 test_query_tool-0.3.3/query_tool/services/query_tool_service.py
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-03 16:47:55.000000 test_query_tool-0.3.3/query_tool/services/register.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-13 12:15:13.855558 test_query_tool-0.3.3/setup.cfg
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      646 2023-04-13 12:14:53.000000 test_query_tool-0.3.3/setup.py
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 12:15:13.854673 test_query_tool-0.3.3/test_query_tool.egg-info/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      323 2023-04-13 12:15:13.000000 test_query_tool-0.3.3/test_query_tool.egg-info/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      684 2023-04-13 12:15:13.000000 test_query_tool-0.3.3/test_query_tool.egg-info/SOURCES.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-13 12:15:13.000000 test_query_tool-0.3.3/test_query_tool.egg-info/dependency_links.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-13 12:15:13.000000 test_query_tool-0.3.3/test_query_tool.egg-info/requires.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       11 2023-04-13 12:15:13.000000 test_query_tool-0.3.3/test_query_tool.egg-info/top_level.txt
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 18:13:05.106164 test_query_tool-0.3.4/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-03 17:08:00.000000 test_query_tool-0.3.4/LICENSE
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       45 2023-04-05 19:58:10.000000 test_query_tool-0.3.4/MANIFEST.in
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      323 2023-04-13 18:13:05.105639 test_query_tool-0.3.4/PKG-INFO
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 18:13:05.087763 test_query_tool-0.3.4/query_tool/
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     3588 2023-04-13 18:04:49.000000 test_query_tool-0.3.4/query_tool/__init__.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 18:13:05.085357 test_query_tool-0.3.4/query_tool/frontend/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 18:13:05.088705 test_query_tool-0.3.4/query_tool/frontend/dist/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 18:13:05.091639 test_query_tool-0.3.4/query_tool/frontend/dist/assets/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1044761 2023-04-13 18:12:35.000000 test_query_tool-0.3.4/query_tool/frontend/dist/assets/index-49ab9bc7.js
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-04-13 18:12:35.000000 test_query_tool-0.3.4/query_tool/frontend/dist/assets/index-d081bea5.css
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      463 2023-04-13 18:12:47.000000 test_query_tool-0.3.4/query_tool/frontend/dist/index.html
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-04-13 18:12:34.000000 test_query_tool-0.3.4/query_tool/frontend/dist/vite.svg
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 18:13:05.101921 test_query_tool-0.3.4/query_tool/services/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-03 16:47:55.000000 test_query_tool-0.3.4/query_tool/services/__init__.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1438 2023-04-03 16:47:55.000000 test_query_tool-0.3.4/query_tool/services/dimension_service.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3941 2023-04-03 16:47:55.000000 test_query_tool-0.3.4/query_tool/services/entities_service.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3653 2023-04-03 16:47:55.000000 test_query_tool-0.3.4/query_tool/services/filters_service.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      437 2023-04-03 16:47:55.000000 test_query_tool-0.3.4/query_tool/services/query_tool_factory.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1987 2023-04-03 16:47:55.000000 test_query_tool-0.3.4/query_tool/services/query_tool_service.py
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-03 16:47:55.000000 test_query_tool-0.3.4/query_tool/services/register.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-13 18:13:05.106359 test_query_tool-0.3.4/setup.cfg
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      646 2023-04-13 18:11:47.000000 test_query_tool-0.3.4/setup.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-13 18:13:05.105065 test_query_tool-0.3.4/test_query_tool.egg-info/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      323 2023-04-13 18:13:05.000000 test_query_tool-0.3.4/test_query_tool.egg-info/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      684 2023-04-13 18:13:05.000000 test_query_tool-0.3.4/test_query_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-13 18:13:05.000000 test_query_tool-0.3.4/test_query_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-13 18:13:05.000000 test_query_tool-0.3.4/test_query_tool.egg-info/requires.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       11 2023-04-13 18:13:05.000000 test_query_tool-0.3.4/test_query_tool.egg-info/top_level.txt
```

### Comparing `test_query_tool-0.3.3/LICENSE` & `test_query_tool-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.3.3/query_tool/__init__.py` & `test_query_tool-0.3.4/query_tool/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     set_component_rerender_count,
 )
 
 # Create a _RELEASE constant. We'll set this to False while we're developing
 # the component, and True when we're ready to package and distribute it.
 # (This is, of course, optional - there are innumerable ways to manage your
 # release process.)
-_RELEASE = True
+_RELEASE = False
 
 # Create a wrapper function for the component. This is an optional
 # best practice - we could simply expose the component function returned by
 # `declare_component` and call it done. The wrapper allows us to customize
 # our component's API: we can pre-process its input args, post-process its
 # output value, and add a docstring for users.
 init()
@@ -36,26 +36,28 @@
     __query_tool_component_function = components.declare_component(
         "query_tool", url="http://localhost:4000"
     )
 
 
 def __query_builder(
     query=None,
+    title: str = "",
     database_list=None,
     table_list=None,
     column_list=None,
     on_click=None,
     key="b-query-builder",
     args: tuple = (),
 ):
     register_callback(key, on_click, *args)
     render_count = get_component_rerender_count(key)
     query_builder_value = __query_tool_component_function(
         key=key,
         query=query,
+        title=title,
         database_list=database_list,
         table_list=table_list,
         column_list=column_list,
         render_count=render_count,
     )
     set_component_rerender_count(key)
     return query_builder_value
@@ -65,39 +67,41 @@
     widget_key,
     on_database_change=None,
     on_table_change=None,
     on_generate_query=None,
     on_copy_query=None,
 ):
     response = st.session_state.get(widget_key)
-    if response["action"] == "database_change":
+    if response["action"] == "database_change" and on_database_change is not None:
         on_database_change(response.get("database"))
-    if response["action"] == "table_change":
+    if response["action"] == "table_change" and on_table_change is not None:
         on_table_change(response.get("database"), response.get("table"))
-    if response["action"] == "preview_query":
+    if response["action"] == "preview_query" and on_generate_query is not None:
         query_tool = get_query_tool()
         query = query_tool.generate_query(response)
         on_generate_query(response, query)
-    if response["action"] == "copy_to_clipboard":
+    if response["action"] == "copy_to_clipboard" and on_copy_query is not None:
         on_copy_query(response.get("query"))
 
 
 def query_tool(
     key: str = "query-tool",
     query: str = "",
+    title: str = "",
     databases: List[str] = [],
     tables: List[dict] = [],
     columns: List[dict] = [],
     on_database_change=None,
     on_table_change=None,
     on_generate_query=None,
     on_copy_query=None,
 ):
     return __query_builder(
         query=query,
+        title=title,
         database_list=databases,
         table_list=tables,
         column_list=columns,
         key=key,
         on_click=handle_query_tool_actions,
         args=(
             key,
```

### Comparing `test_query_tool-0.3.3/query_tool/frontend/dist/assets/index-d72f7278.js` & `test_query_tool-0.3.4/query_tool/frontend/dist/assets/index-49ab9bc7.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -45732,15 +45732,15 @@
                 })]
             }), n && Ue(wn, {
                 direction: "column",
                 sx: {
                     backgroundColor: "#F3F8FD",
                     borderRadius: "9px"
                 },
-                mt: 2,
+                mt: 3,
                 p: 3,
                 gap: 2,
                 children: [Ue(wn, {
                     direction: "row",
                     justifyContent: "space-between",
                     children: [U(la, {
                         variant: "h6",
@@ -45799,15 +45799,15 @@
         var o;
         const {
             renderCount: t
         } = e == null ? void 0 : e.args, n = C.useRef((o = e == null ? void 0 : e.args) == null ? void 0 : o.renderCount), r = C.useRef(null);
         C.useEffect(() => {
             Mi.setFrameHeight(1e3)
         }, []);
-        const i = C.useCallback((l = 0, c) => {
+        const i = C.useCallback((l = 10, c) => {
             const E = r == null ? void 0 : r.current;
             setTimeout(() => {
                 if (E != null && E.offsetHeight) {
                     const f = Number(c) === c ? c : E == null ? void 0 : E.offsetHeight;
                     Mi.setFrameHeight(f + l)
                 }
             }, 500)
```

### Comparing `test_query_tool-0.3.3/query_tool/frontend/dist/vite.svg` & `test_query_tool-0.3.4/query_tool/frontend/dist/vite.svg`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.3.3/query_tool/services/dimension_service.py` & `test_query_tool-0.3.4/query_tool/services/dimension_service.py`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.3.3/query_tool/services/entities_service.py` & `test_query_tool-0.3.4/query_tool/services/entities_service.py`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.3.3/query_tool/services/filters_service.py` & `test_query_tool-0.3.4/query_tool/services/filters_service.py`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.3.3/query_tool/services/query_tool_service.py` & `test_query_tool-0.3.4/query_tool/services/query_tool_service.py`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.3.3/query_tool/services/register.py` & `test_query_tool-0.3.4/query_tool/services/register.py`

 * *Files identical despite different names*

### Comparing `test_query_tool-0.3.3/setup.py` & `test_query_tool-0.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="test_query_tool",
-    version="0.3.3",
+    version="0.3.4",
     author="Bluepinapple",
     author_email="viveksthul@bluepinapple.com",
     description="Query tool to generate query from selection",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `test_query_tool-0.3.3/test_query_tool.egg-info/SOURCES.txt` & `test_query_tool-0.3.4/test_query_tool.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 LICENSE
 MANIFEST.in
 setup.py
 query_tool/__init__.py
 query_tool/frontend/dist/index.html
 query_tool/frontend/dist/vite.svg
+query_tool/frontend/dist/assets/index-49ab9bc7.js
 query_tool/frontend/dist/assets/index-d081bea5.css
-query_tool/frontend/dist/assets/index-d72f7278.js
 query_tool/services/__init__.py
 query_tool/services/dimension_service.py
 query_tool/services/entities_service.py
 query_tool/services/filters_service.py
 query_tool/services/query_tool_factory.py
 query_tool/services/query_tool_service.py
 query_tool/services/register.py
```

