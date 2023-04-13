# Comparing `tmp/business-rules-enhanced-1.3.3.tar.gz` & `tmp/business-rules-enhanced-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "business-rules-enhanced-1.3.3.tar", last modified: Wed Apr  5 15:00:59 2023, max compression
+gzip compressed data, was "business-rules-enhanced-1.3.4.tar", last modified: Thu Apr 13 15:03:40 2023, max compression
```

## Comparing `business-rules-enhanced-1.3.3.tar` & `business-rules-enhanced-1.3.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:00:59.695482 business-rules-enhanced-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-05 15:00:37.000000 business-rules-enhanced-1.3.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-05 15:00:37.000000 business-rules-enhanced-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 15:00:37.000000 business-rules-enhanced-1.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-05 15:00:59.695482 business-rules-enhanced-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12034 2023-04-05 15:00:37.000000 business-rules-enhanced-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:00:59.695482 business-rules-enhanced-1.3.3/business_rules/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-05 15:00:37.000000 business-rules-enhanced-1.3.3/business_rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-05 15:00:37.000000 business-rules-enhanced-1.3.3/business_rules/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-04-05 15:00:37.000000 business-rules-enhanced-1.3.3/business_rules/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-05 15:00:37.000000 business-rules-enhanced-1.3.3/business_rules/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    58425 2023-04-05 15:00:37.000000 business-rules-enhanced-1.3.3/business_rules/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    20588 2023-04-05 15:00:37.000000 business-rules-enhanced-1.3.3/business_rules/six.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-04-05 15:00:37.000000 business-rules-enhanced-1.3.3/business_rules/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-05 15:00:37.000000 business-rules-enhanced-1.3.3/business_rules/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:00:59.695482 business-rules-enhanced-1.3.3/business_rules_enhanced.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-05 15:00:59.000000 business-rules-enhanced-1.3.3/business_rules_enhanced.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-05 15:00:59.000000 business-rules-enhanced-1.3.3/business_rules_enhanced.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 15:00:59.000000 business-rules-enhanced-1.3.3/business_rules_enhanced.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-05 15:00:59.000000 business-rules-enhanced-1.3.3/business_rules_enhanced.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 15:00:59.695482 business-rules-enhanced-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-05 15:00:37.000000 business-rules-enhanced-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:03:40.900611 business-rules-enhanced-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-13 15:03:12.000000 business-rules-enhanced-1.3.4/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-13 15:03:12.000000 business-rules-enhanced-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 15:03:12.000000 business-rules-enhanced-1.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-13 15:03:40.900611 business-rules-enhanced-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12034 2023-04-13 15:03:12.000000 business-rules-enhanced-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:03:40.900611 business-rules-enhanced-1.3.4/business_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-13 15:03:12.000000 business-rules-enhanced-1.3.4/business_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-13 15:03:12.000000 business-rules-enhanced-1.3.4/business_rules/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-04-13 15:03:12.000000 business-rules-enhanced-1.3.4/business_rules/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-13 15:03:12.000000 business-rules-enhanced-1.3.4/business_rules/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58425 2023-04-13 15:03:12.000000 business-rules-enhanced-1.3.4/business_rules/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20588 2023-04-13 15:03:12.000000 business-rules-enhanced-1.3.4/business_rules/six.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-04-13 15:03:12.000000 business-rules-enhanced-1.3.4/business_rules/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-13 15:03:12.000000 business-rules-enhanced-1.3.4/business_rules/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:03:40.900611 business-rules-enhanced-1.3.4/business_rules_enhanced.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-13 15:03:40.000000 business-rules-enhanced-1.3.4/business_rules_enhanced.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-13 15:03:40.000000 business-rules-enhanced-1.3.4/business_rules_enhanced.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:03:40.000000 business-rules-enhanced-1.3.4/business_rules_enhanced.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-13 15:03:40.000000 business-rules-enhanced-1.3.4/business_rules_enhanced.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 15:03:40.900611 business-rules-enhanced-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-13 15:03:12.000000 business-rules-enhanced-1.3.4/setup.py
```

### Comparing `business-rules-enhanced-1.3.3/LICENSE` & `business-rules-enhanced-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `business-rules-enhanced-1.3.3/PKG-INFO` & `business-rules-enhanced-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: business-rules-enhanced
-Version: 1.3.3
+Version: 1.3.4
 Summary: Fork of Venmo-Business-Rules: Python DSL for setting up business intelligence rules that can be configured without code  History -------  1.0.1 +++++ released 2016-3-16  - Fixes a packaging bug preventing 1.0.0 from being installed on some platforms.  1.0.0 +++++ released 2016-3-16  - Removes caching layer on rule decorator 
 Home-page: https://github.com/cdisc-org/business-rules
 Author: cdisc-org
 Author-email: UNKNOWN
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `business-rules-enhanced-1.3.3/README.md` & `business-rules-enhanced-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `business-rules-enhanced-1.3.3/business_rules/actions.py` & `business-rules-enhanced-1.3.4/business_rules/actions.py`

 * *Files identical despite different names*

### Comparing `business-rules-enhanced-1.3.3/business_rules/engine.py` & `business-rules-enhanced-1.3.4/business_rules/engine.py`

 * *Files identical despite different names*

### Comparing `business-rules-enhanced-1.3.3/business_rules/operators.py` & `business-rules-enhanced-1.3.4/business_rules/operators.py`

 * *Files identical despite different names*

### Comparing `business-rules-enhanced-1.3.3/business_rules/six.py` & `business-rules-enhanced-1.3.4/business_rules/six.py`

 * *Files identical despite different names*

### Comparing `business-rules-enhanced-1.3.3/business_rules/utils.py` & `business-rules-enhanced-1.3.4/business_rules/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from datetime import datetime, tzinfo
 import re
 import inspect
 import numpy as np
 from dateutil.parser import parse, isoparse
 import pytz
 
+date_regex = re.compile(r'^((-?[0-9]{4}|-)(-(1[0-2]|0[1-9]|-)(-(3[01]|0[1-9]|[12][0-9]|-)(T(2[0-3]|[01][0-9]|-)(:([0-5][0-9]|-)((:([0-5][0-9]|-))?(\.[0-9]+)?((Z|[+-](:2[0-3]|[01][0-9]):[0-5][0-9]))?)?)?)?)?)?)(\/((-?[0-9]{4}|-)(-(1[0-2]|0[1-9]|-)(-(3[01]|0[1-9]|[12][0-9]|-)(T(2[0-3]|[01][0-9]|-)(:([0-5][0-9]|-)((:([0-5][0-9]|-))?(\.[0-9]+)?((Z|[+-](:2[0-3]|[01][0-9]):[0-5][0-9]))?)?)?)?)?)?))?$')
+
 def fn_name_to_pretty_label(name):
     return ' '.join([w.title() for w in name.split('_')])
 
 def export_rule_data(variables, actions):
     """ export_rule_data is used to export all information about the
     variables, actions, and operators to the client. This will return a
     dictionary with three keys:
@@ -45,16 +47,22 @@
         result = ctx.divide(numerator, denominator)
     return result
 
 def is_valid_date(date_string: str) -> bool:
     try:
         isoparse(date_string)
     except:
-        return False
-    return True
+        uncertainty_substrings = ["/", "--", "-:"]
+        if any([substr in date_string for substr in uncertainty_substrings]):
+            # date_string contains uncertainty
+            # will not parse with isoparse
+            return date_regex.match(date_string) is not None
+        else:
+            return False
+    return date_regex.match(date_string) is not None
 
 def get_year(date_string: str):
     timestamp = get_date(date_string)
     return timestamp.year
 
 def get_month(date_string: str):
     timestamp = get_date(date_string)
```

### Comparing `business-rules-enhanced-1.3.3/business_rules/variables.py` & `business-rules-enhanced-1.3.4/business_rules/variables.py`

 * *Files identical despite different names*

### Comparing `business-rules-enhanced-1.3.3/business_rules_enhanced.egg-info/PKG-INFO` & `business-rules-enhanced-1.3.4/business_rules_enhanced.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: business-rules-enhanced
-Version: 1.3.3
+Version: 1.3.4
 Summary: Fork of Venmo-Business-Rules: Python DSL for setting up business intelligence rules that can be configured without code  History -------  1.0.1 +++++ released 2016-3-16  - Fixes a packaging bug preventing 1.0.0 from being installed on some platforms.  1.0.0 +++++ released 2016-3-16  - Removes caching layer on rule decorator 
 Home-page: https://github.com/cdisc-org/business-rules
 Author: cdisc-org
 Author-email: UNKNOWN
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `business-rules-enhanced-1.3.3/setup.py` & `business-rules-enhanced-1.3.4/setup.py`

 * *Files identical despite different names*

