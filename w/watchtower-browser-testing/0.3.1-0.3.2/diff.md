# Comparing `tmp/watchtower_browser_testing-0.3.1.tar.gz` & `tmp/watchtower_browser_testing-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchtower_browser_testing-0.3.1.tar", last modified: Thu Apr 13 18:04:44 2023, max compression
+gzip compressed data, was "watchtower_browser_testing-0.3.2.tar", last modified: Thu Apr 13 18:07:52 2023, max compression
```

## Comparing `watchtower_browser_testing-0.3.1.tar` & `watchtower_browser_testing-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 18:04:44.912838 watchtower_browser_testing-0.3.1/
--rw-rw-rw-   0        0        0      310 2023-04-13 18:04:44.912838 watchtower_browser_testing-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.3.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 18:04:44.912838 watchtower_browser_testing-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1005 2023-04-01 17:58:47.000000 watchtower_browser_testing-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:04:44.897198 watchtower_browser_testing-0.3.1/watchtower_browser_testing/
--rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.3.1/watchtower_browser_testing/__init__.py
--rw-rw-rw-   0        0        0      677 2023-04-13 12:22:31.000000 watchtower_browser_testing-0.3.1/watchtower_browser_testing/config.py
--rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.3.1/watchtower_browser_testing/exceptions.py
--rw-rw-rw-   0        0        0     1503 2023-04-13 18:01:14.000000 watchtower_browser_testing-0.3.1/watchtower_browser_testing/helpers.py
--rw-rw-rw-   0        0        0    13970 2023-04-13 18:04:35.000000 watchtower_browser_testing-0.3.1/watchtower_browser_testing/testsuite.py
--rw-rw-rw-   0        0        0     7743 2023-04-12 06:31:40.000000 watchtower_browser_testing-0.3.1/watchtower_browser_testing/tracking_validation.py
--rw-rw-rw-   0        0        0       21 2023-04-13 18:04:35.000000 watchtower_browser_testing-0.3.1/watchtower_browser_testing/version.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:04:44.912838 watchtower_browser_testing-0.3.1/watchtower_browser_testing.egg-info/
--rw-rw-rw-   0        0        0      310 2023-04-13 18:04:44.000000 watchtower_browser_testing-0.3.1/watchtower_browser_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      550 2023-04-13 18:04:44.000000 watchtower_browser_testing-0.3.1/watchtower_browser_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 18:04:44.000000 watchtower_browser_testing-0.3.1/watchtower_browser_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-04-13 18:04:44.000000 watchtower_browser_testing-0.3.1/watchtower_browser_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-04-13 18:04:44.000000 watchtower_browser_testing-0.3.1/watchtower_browser_testing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 18:07:52.274027 watchtower_browser_testing-0.3.2/
+-rw-rw-rw-   0        0        0      310 2023-04-13 18:07:52.258430 watchtower_browser_testing-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.3.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 18:07:52.274943 watchtower_browser_testing-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1005 2023-04-01 17:58:47.000000 watchtower_browser_testing-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:07:52.258430 watchtower_browser_testing-0.3.2/watchtower_browser_testing/
+-rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.3.2/watchtower_browser_testing/__init__.py
+-rw-rw-rw-   0        0        0      677 2023-04-13 12:22:31.000000 watchtower_browser_testing-0.3.2/watchtower_browser_testing/config.py
+-rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.3.2/watchtower_browser_testing/exceptions.py
+-rw-rw-rw-   0        0        0     1503 2023-04-13 18:01:14.000000 watchtower_browser_testing-0.3.2/watchtower_browser_testing/helpers.py
+-rw-rw-rw-   0        0        0    13936 2023-04-13 18:07:40.000000 watchtower_browser_testing-0.3.2/watchtower_browser_testing/testsuite.py
+-rw-rw-rw-   0        0        0     7743 2023-04-12 06:31:40.000000 watchtower_browser_testing-0.3.2/watchtower_browser_testing/tracking_validation.py
+-rw-rw-rw-   0        0        0       21 2023-04-13 18:07:49.000000 watchtower_browser_testing-0.3.2/watchtower_browser_testing/version.py
+drwxrwxrwx   0        0        0        0 2023-04-13 18:07:52.258430 watchtower_browser_testing-0.3.2/watchtower_browser_testing.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-04-13 18:07:52.000000 watchtower_browser_testing-0.3.2/watchtower_browser_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2023-04-13 18:07:52.000000 watchtower_browser_testing-0.3.2/watchtower_browser_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 18:07:52.000000 watchtower_browser_testing-0.3.2/watchtower_browser_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-04-13 18:07:52.000000 watchtower_browser_testing-0.3.2/watchtower_browser_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-04-13 18:07:52.000000 watchtower_browser_testing-0.3.2/watchtower_browser_testing.egg-info/top_level.txt
```

### Comparing `watchtower_browser_testing-0.3.1/setup.py` & `watchtower_browser_testing-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.3.1/watchtower_browser_testing/config.py` & `watchtower_browser_testing-0.3.2/watchtower_browser_testing/config.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.3.1/watchtower_browser_testing/helpers.py` & `watchtower_browser_testing-0.3.2/watchtower_browser_testing/helpers.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.3.1/watchtower_browser_testing/testsuite.py` & `watchtower_browser_testing-0.3.2/watchtower_browser_testing/testsuite.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,26 +237,26 @@
 
         test_name = cls.__name__
         test_id = parent + '_' + cls.__name__
 
         structure = {'name': test_name,
                      'type': 'test',
                      'id': 't_' + test_id,
-                     'description': markdown.parse(helpers.trim(cls.__doc__) or '').children,
+                     'description': markdown.parse(helpers.trim(cls.__doc__) or ''),
                      'children': []}
 
         for scenario_method in cls.scen_methods():
 
             scenario_name = scenario_method[len(config.SCENARIO_METHOD_PREFIX):]
             scenario_id = test_id + '_' + scenario_name
             scenario_struct = {'name': scenario_name,
                                'type': 'scenario',
                                'id': 's_' + scenario_id,
                                'description': markdown.parse(
-                                   helpers.trim(getattr(cls, scenario_method).__doc__) or '').children,
+                                   helpers.trim(getattr(cls, scenario_method).__doc__) or ''),
                                'children': []}
             validation_method = config.VALIDATION_METHOD_PREFIX + scenario_method[len(config.SCENARIO_METHOD_PREFIX):]
             val = getattr(cls, validation_method)()
 
             for event_name, obj in val.items():
 
                 event_id = scenario_id + '_' + event_name
@@ -264,15 +264,15 @@
                 if body_validator and isinstance(body_validator, Validator):
                     body_validator = body_validator.schema
                 json_string = json.dumps(dict(body_validator), indent=4, cls=helpers.ExtendedEncoder)
                 mdstring = config.VALIDATION_MD_STRING.format(event_name=event_name, json_string=json_string)
                 event_struct = {'name': event_name,
                                 'id': 'e_' + event_id,
                                 'type': 'event',
-                                'description': markdown.parse(mdstring).children}
+                                'description': markdown.parse(mdstring)}
 
                 scenario_struct['children'].append(event_struct)
 
             structure['children'].append(scenario_struct)
 
         return structure
 
@@ -374,20 +374,21 @@
 
         tests = self.get_tests()
 
         name = self.__class__.__name__
         structure = {'name': name,
                      'id': 'm_' + name,
                      'type': 'measurement_plan',
-                     'description': markdown.parse(helpers.trim(self.__doc__) or '').children,
+                     'description': markdown.parse(helpers.trim(self.__doc__) or ''),
                      'children': []}
 
         for test in tests:
             structure['children'].append(test['class'].md_description(parent=name))
 
+
         return structure
 
     def html_description(self):
 
         structure = self.md_description()
         return helpers.build_html(structure)
```

### Comparing `watchtower_browser_testing-0.3.1/watchtower_browser_testing/tracking_validation.py` & `watchtower_browser_testing-0.3.2/watchtower_browser_testing/tracking_validation.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.3.1/watchtower_browser_testing.egg-info/SOURCES.txt` & `watchtower_browser_testing-0.3.2/watchtower_browser_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

