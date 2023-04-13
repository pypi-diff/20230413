# Comparing `tmp/watchtower_browser_testing-0.3.6.tar.gz` & `tmp/watchtower_browser_testing-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchtower_browser_testing-0.3.6.tar", last modified: Thu Apr 13 18:51:35 2023, max compression
+gzip compressed data, was "watchtower_browser_testing-0.3.7.tar", last modified: Thu Apr 13 19:16:51 2023, max compression
```

## Comparing `watchtower_browser_testing-0.3.6.tar` & `watchtower_browser_testing-0.3.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 18:51:35.900791 watchtower_browser_testing-0.3.6/
--rw-rw-rw-   0        0        0      310 2023-04-13 18:51:35.900791 watchtower_browser_testing-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.3.6/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 18:51:35.900791 watchtower_browser_testing-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0     1106 2023-04-13 18:41:33.000000 watchtower_browser_testing-0.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:51:35.890283 watchtower_browser_testing-0.3.6/watchtower_browser_testing/
--rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.3.6/watchtower_browser_testing/__init__.py
--rw-rw-rw-   0        0        0      810 2023-04-13 18:26:41.000000 watchtower_browser_testing-0.3.6/watchtower_browser_testing/config.py
--rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.3.6/watchtower_browser_testing/exceptions.py
--rw-rw-rw-   0        0        0     1509 2023-04-13 18:16:09.000000 watchtower_browser_testing-0.3.6/watchtower_browser_testing/helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:51:35.900791 watchtower_browser_testing-0.3.6/watchtower_browser_testing/templates/
--rw-rw-rw-   0        0        0      480 2023-04-13 18:51:23.000000 watchtower_browser_testing-0.3.6/watchtower_browser_testing/templates/measurement_plan.html
--rw-rw-rw-   0        0        0    14352 2023-04-13 18:35:07.000000 watchtower_browser_testing-0.3.6/watchtower_browser_testing/testsuite.py
--rw-rw-rw-   0        0        0     7743 2023-04-12 06:31:40.000000 watchtower_browser_testing-0.3.6/watchtower_browser_testing/tracking_validation.py
--rw-rw-rw-   0        0        0       21 2023-04-13 18:51:23.000000 watchtower_browser_testing-0.3.6/watchtower_browser_testing/version.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:51:35.900791 watchtower_browser_testing-0.3.6/watchtower_browser_testing.egg-info/
--rw-rw-rw-   0        0        0      310 2023-04-13 18:51:35.000000 watchtower_browser_testing-0.3.6/watchtower_browser_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      609 2023-04-13 18:51:35.000000 watchtower_browser_testing-0.3.6/watchtower_browser_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 18:51:35.000000 watchtower_browser_testing-0.3.6/watchtower_browser_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-13 18:51:35.000000 watchtower_browser_testing-0.3.6/watchtower_browser_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-04-13 18:51:35.000000 watchtower_browser_testing-0.3.6/watchtower_browser_testing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 19:16:51.850849 watchtower_browser_testing-0.3.7/
+-rw-rw-rw-   0        0        0      310 2023-04-13 19:16:51.850849 watchtower_browser_testing-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.3.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 19:16:51.850849 watchtower_browser_testing-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     1106 2023-04-13 18:41:33.000000 watchtower_browser_testing-0.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:16:51.834741 watchtower_browser_testing-0.3.7/watchtower_browser_testing/
+-rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.3.7/watchtower_browser_testing/__init__.py
+-rw-rw-rw-   0        0        0      810 2023-04-13 18:26:41.000000 watchtower_browser_testing-0.3.7/watchtower_browser_testing/config.py
+-rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.3.7/watchtower_browser_testing/exceptions.py
+-rw-rw-rw-   0        0        0     1509 2023-04-13 18:16:09.000000 watchtower_browser_testing-0.3.7/watchtower_browser_testing/helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:16:51.834741 watchtower_browser_testing-0.3.7/watchtower_browser_testing/templates/
+-rw-rw-rw-   0        0        0     1721 2023-04-13 19:16:36.000000 watchtower_browser_testing-0.3.7/watchtower_browser_testing/templates/measurement_plan.html
+-rw-rw-rw-   0        0        0    14236 2023-04-13 19:16:36.000000 watchtower_browser_testing-0.3.7/watchtower_browser_testing/testsuite.py
+-rw-rw-rw-   0        0        0     7743 2023-04-12 06:31:40.000000 watchtower_browser_testing-0.3.7/watchtower_browser_testing/tracking_validation.py
+-rw-rw-rw-   0        0        0       21 2023-04-13 19:16:36.000000 watchtower_browser_testing-0.3.7/watchtower_browser_testing/version.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:16:51.834741 watchtower_browser_testing-0.3.7/watchtower_browser_testing.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-04-13 19:16:51.000000 watchtower_browser_testing-0.3.7/watchtower_browser_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2023-04-13 19:16:51.000000 watchtower_browser_testing-0.3.7/watchtower_browser_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 19:16:51.000000 watchtower_browser_testing-0.3.7/watchtower_browser_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-13 19:16:51.000000 watchtower_browser_testing-0.3.7/watchtower_browser_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-04-13 19:16:51.000000 watchtower_browser_testing-0.3.7/watchtower_browser_testing.egg-info/top_level.txt
```

### Comparing `watchtower_browser_testing-0.3.6/setup.py` & `watchtower_browser_testing-0.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.3.6/watchtower_browser_testing/config.py` & `watchtower_browser_testing-0.3.7/watchtower_browser_testing/config.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.3.6/watchtower_browser_testing/helpers.py` & `watchtower_browser_testing-0.3.7/watchtower_browser_testing/helpers.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.3.6/watchtower_browser_testing/testsuite.py` & `watchtower_browser_testing-0.3.7/watchtower_browser_testing/testsuite.py`

 * *Files 3% similar despite different names*

```diff
@@ -238,25 +238,25 @@
 
         test_name = cls.__name__
         test_id = parent + '_' + cls.__name__
 
         structure = {'name': test_name,
                      'type': 'test',
                      'id': 't_' + test_id,
-                     'description': markdown.parse(helpers.trim(cls.__doc__) or ''),
+                     'description': markdown.convert(helpers.trim(cls.__doc__) or ''),
                      'children': []}
 
         for scenario_method in cls.scen_methods():
 
             scenario_name = scenario_method[len(config.SCENARIO_METHOD_PREFIX):]
             scenario_id = test_id + '_' + scenario_name
             scenario_struct = {'name': scenario_name,
                                'type': 'scenario',
                                'id': 's_' + scenario_id,
-                               'description': markdown.parse(
+                               'description': markdown.convert(
                                    helpers.trim(getattr(cls, scenario_method).__doc__) or ''),
                                'children': []}
             validation_method = config.VALIDATION_METHOD_PREFIX + scenario_method[len(config.SCENARIO_METHOD_PREFIX):]
             val = getattr(cls, validation_method)()
 
             for event_name, obj in val.items():
 
@@ -265,15 +265,15 @@
                 if body_validator and isinstance(body_validator, Validator):
                     body_validator = body_validator.schema
                 json_string = json.dumps(dict(body_validator), indent=4, cls=helpers.ExtendedEncoder)
                 mdstring = config.VALIDATION_MD_STRING.format(event_name=event_name, json_string=json_string)
                 event_struct = {'name': event_name,
                                 'id': 'e_' + event_id,
                                 'type': 'event',
-                                'description': markdown.parse(mdstring)}
+                                'description': markdown.convert(mdstring)}
 
                 scenario_struct['children'].append(event_struct)
 
             structure['children'].append(scenario_struct)
 
         return structure
 
@@ -375,31 +375,26 @@
 
         tests = self.get_tests()
 
         name = self.__class__.__name__
         structure = {'name': name,
                      'id': 'm_' + name,
                      'type': 'measurement_plan',
-                     'description': markdown.parse(helpers.trim(self.__doc__) or ''),
+                     'description': markdown.convert(helpers.trim(self.__doc__) or ''),
                      'children': []}
 
         for test in tests:
             structure['children'].append(test['class'].md_description(parent=name))
 
 
         return structure
 
-    def html_report(self, title='Measurement Plan'):
+    def html_report(self, title='Measurement Plan', test_results=None):
 
         jenv = jinja2.Environment(loader=jinja2.FileSystemLoader(config.TEMPLATES_PATH))
         template = jenv.get_template('measurement_plan.html')
 
-        structure = self.md_description()
-        content = helpers.build_html(structure)
+        content = self.md_description()
 
-        return template.render(title=title, content=content)
+        test_results = test_results or {}
 
-
-def test():
-
-    jenv = jinja2.Environment(loader=jinja2.FileSystemLoader(config.TEMPLATES_PATH))
-    template = jenv.get_template('measurement_plan.html')
+        return template.render(title=title, content=content, test_results=test_results)
```

### Comparing `watchtower_browser_testing-0.3.6/watchtower_browser_testing/tracking_validation.py` & `watchtower_browser_testing-0.3.7/watchtower_browser_testing/tracking_validation.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.3.6/watchtower_browser_testing.egg-info/SOURCES.txt` & `watchtower_browser_testing-0.3.7/watchtower_browser_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

