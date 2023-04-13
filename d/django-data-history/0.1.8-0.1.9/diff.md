# Comparing `tmp/django-data-history-0.1.8.tar.gz` & `tmp/django-data-history-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-data-history-0.1.8.tar", last modified: Wed Apr 12 11:04:41 2023, max compression
+gzip compressed data, was "django-data-history-0.1.9.tar", last modified: Thu Apr 13 12:01:21 2023, max compression
```

## Comparing `django-data-history-0.1.8.tar` & `django-data-history-0.1.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-12 11:04:41.932333 django-data-history-0.1.8/
--rw-r--r--   0 test       (501) staff       (20)     1067 2022-06-01 09:33:33.000000 django-data-history-0.1.8/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      225 2022-06-01 09:35:01.000000 django-data-history-0.1.8/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)     3777 2023-04-12 11:04:41.932207 django-data-history-0.1.8/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)     3080 2023-04-12 11:03:38.000000 django-data-history-0.1.8/README.md
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-12 11:04:41.929398 django-data-history-0.1.8/django_data_history/
--rw-r--r--   0 test       (501) staff       (20)      551 2022-10-17 02:38:38.000000 django-data-history-0.1.8/django_data_history/__init__.py
--rw-r--r--   0 test       (501) staff       (20)     3271 2023-01-10 08:09:27.000000 django-data-history-0.1.8/django_data_history/admin.py
--rw-r--r--   0 test       (501) staff       (20)      771 2022-06-22 05:33:42.000000 django-data-history-0.1.8/django_data_history/apps.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-12 11:04:41.925297 django-data-history-0.1.8/django_data_history/locale/
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-12 11:04:41.925337 django-data-history-0.1.8/django_data_history/locale/zh_Hans/
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-12 11:04:41.930694 django-data-history-0.1.8/django_data_history/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 test       (501) staff       (20)     1449 2022-06-01 03:23:30.000000 django-data-history-0.1.8/django_data_history/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 test       (501) staff       (20)     3068 2022-06-01 03:23:26.000000 django-data-history-0.1.8/django_data_history/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-12 11:04:41.931161 django-data-history-0.1.8/django_data_history/migrations/
--rw-r--r--   0 test       (501) staff       (20)     1564 2022-06-01 08:48:42.000000 django-data-history-0.1.8/django_data_history/migrations/0001_initial.py
--rw-r--r--   0 test       (501) staff       (20)        0 2022-05-31 02:09:01.000000 django-data-history-0.1.8/django_data_history/migrations/__init__.py
--rw-r--r--   0 test       (501) staff       (20)    14074 2023-04-12 09:22:30.000000 django-data-history-0.1.8/django_data_history/models.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-12 11:04:41.925580 django-data-history-0.1.8/django_data_history/static/
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-12 11:04:41.925674 django-data-history-0.1.8/django_data_history/static/django_data_history/
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-12 11:04:41.931273 django-data-history-0.1.8/django_data_history/static/django_data_history/css/
--rw-r--r--   0 test       (501) staff       (20)      115 2022-06-01 09:13:04.000000 django-data-history-0.1.8/django_data_history/static/django_data_history/css/django_data_history.css
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-12 11:04:41.931473 django-data-history-0.1.8/django_data_history/static/django_data_history/js/
--rw-r--r--   0 test       (501) staff       (20)      359 2022-06-01 08:12:33.000000 django-data-history-0.1.8/django_data_history/static/django_data_history/js/django_data_history.js
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-12 11:04:41.925826 django-data-history-0.1.8/django_data_history/templates/
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-12 11:04:41.931664 django-data-history-0.1.8/django_data_history/templates/admin/
--rw-r--r--   0 test       (501) staff       (20)     3382 2022-06-01 09:06:49.000000 django-data-history-0.1.8/django_data_history/templates/admin/object_history.html
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-12 11:04:41.931892 django-data-history-0.1.8/django_data_history/templates/django_data_history/
--rw-r--r--   0 test       (501) staff       (20)      285 2022-05-31 09:43:28.000000 django-data-history-0.1.8/django_data_history/templates/django_data_history/userinfo.html
--rw-r--r--   0 test       (501) staff       (20)      171 2022-06-22 05:33:28.000000 django-data-history-0.1.8/django_data_history/tests.py
--rw-r--r--   0 test       (501) staff       (20)     1603 2023-04-12 09:06:05.000000 django-data-history-0.1.8/django_data_history/utils.py
--rw-r--r--   0 test       (501) staff       (20)      171 2022-06-22 05:33:25.000000 django-data-history-0.1.8/django_data_history/views.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-12 11:04:41.930246 django-data-history-0.1.8/django_data_history.egg-info/
--rw-r--r--   0 test       (501) staff       (20)     3777 2023-04-12 11:04:41.000000 django-data-history-0.1.8/django_data_history.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      989 2023-04-12 11:04:41.000000 django-data-history-0.1.8/django_data_history.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2023-04-12 11:04:41.000000 django-data-history-0.1.8/django_data_history.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2023-04-12 11:04:41.000000 django-data-history-0.1.8/django_data_history.egg-info/not-zip-safe
--rw-r--r--   0 test       (501) staff       (20)      129 2023-04-12 11:04:41.000000 django-data-history-0.1.8/django_data_history.egg-info/requires.txt
--rw-r--r--   0 test       (501) staff       (20)       20 2023-04-12 11:04:41.000000 django-data-history-0.1.8/django_data_history.egg-info/top_level.txt
--rw-r--r--   0 test       (501) staff       (20)      129 2022-10-31 07:23:44.000000 django-data-history-0.1.8/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2023-04-12 11:04:41.932367 django-data-history-0.1.8/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1437 2023-04-12 08:46:41.000000 django-data-history-0.1.8/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-13 12:01:21.692804 django-data-history-0.1.9/
+-rw-r--r--   0 test       (501) staff       (20)     1067 2022-06-01 09:33:33.000000 django-data-history-0.1.9/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      225 2022-06-01 09:35:01.000000 django-data-history-0.1.9/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)     3819 2023-04-13 12:01:21.692696 django-data-history-0.1.9/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     3122 2023-04-13 10:13:21.000000 django-data-history-0.1.9/README.md
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-13 12:01:21.690029 django-data-history-0.1.9/django_data_history/
+-rw-r--r--   0 test       (501) staff       (20)      551 2022-10-17 02:38:38.000000 django-data-history-0.1.9/django_data_history/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)     3271 2023-01-10 08:09:27.000000 django-data-history-0.1.9/django_data_history/admin.py
+-rw-r--r--   0 test       (501) staff       (20)      771 2022-06-22 05:33:42.000000 django-data-history-0.1.9/django_data_history/apps.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-13 12:01:21.687458 django-data-history-0.1.9/django_data_history/locale/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-13 12:01:21.687498 django-data-history-0.1.9/django_data_history/locale/zh_Hans/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-13 12:01:21.691209 django-data-history-0.1.9/django_data_history/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 test       (501) staff       (20)     1449 2022-06-01 03:23:30.000000 django-data-history-0.1.9/django_data_history/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 test       (501) staff       (20)     3068 2022-06-01 03:23:26.000000 django-data-history-0.1.9/django_data_history/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-13 12:01:21.691644 django-data-history-0.1.9/django_data_history/migrations/
+-rw-r--r--   0 test       (501) staff       (20)     1564 2022-06-01 08:48:42.000000 django-data-history-0.1.9/django_data_history/migrations/0001_initial.py
+-rw-r--r--   0 test       (501) staff       (20)        0 2022-05-31 02:09:01.000000 django-data-history-0.1.9/django_data_history/migrations/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)    14074 2023-04-12 09:22:30.000000 django-data-history-0.1.9/django_data_history/models.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-13 12:01:21.687645 django-data-history-0.1.9/django_data_history/static/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-13 12:01:21.687733 django-data-history-0.1.9/django_data_history/static/django_data_history/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-13 12:01:21.691730 django-data-history-0.1.9/django_data_history/static/django_data_history/css/
+-rw-r--r--   0 test       (501) staff       (20)      115 2022-06-01 09:13:04.000000 django-data-history-0.1.9/django_data_history/static/django_data_history/css/django_data_history.css
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-13 12:01:21.691957 django-data-history-0.1.9/django_data_history/static/django_data_history/js/
+-rw-r--r--   0 test       (501) staff       (20)      359 2022-06-01 08:12:33.000000 django-data-history-0.1.9/django_data_history/static/django_data_history/js/django_data_history.js
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-13 12:01:21.687874 django-data-history-0.1.9/django_data_history/templates/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-13 12:01:21.692140 django-data-history-0.1.9/django_data_history/templates/admin/
+-rw-r--r--   0 test       (501) staff       (20)     3382 2022-06-01 09:06:49.000000 django-data-history-0.1.9/django_data_history/templates/admin/object_history.html
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-13 12:01:21.692414 django-data-history-0.1.9/django_data_history/templates/django_data_history/
+-rw-r--r--   0 test       (501) staff       (20)      285 2022-05-31 09:43:28.000000 django-data-history-0.1.9/django_data_history/templates/django_data_history/userinfo.html
+-rw-r--r--   0 test       (501) staff       (20)      171 2022-06-22 05:33:28.000000 django-data-history-0.1.9/django_data_history/tests.py
+-rw-r--r--   0 test       (501) staff       (20)     1831 2023-04-13 10:16:23.000000 django-data-history-0.1.9/django_data_history/utils.py
+-rw-r--r--   0 test       (501) staff       (20)      171 2022-06-22 05:33:25.000000 django-data-history-0.1.9/django_data_history/views.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-13 12:01:21.690879 django-data-history-0.1.9/django_data_history.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)     3819 2023-04-13 12:01:21.000000 django-data-history-0.1.9/django_data_history.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      989 2023-04-13 12:01:21.000000 django-data-history-0.1.9/django_data_history.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2023-04-13 12:01:21.000000 django-data-history-0.1.9/django_data_history.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2023-04-13 12:01:21.000000 django-data-history-0.1.9/django_data_history.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)      129 2023-04-13 12:01:21.000000 django-data-history-0.1.9/django_data_history.egg-info/requires.txt
+-rw-r--r--   0 test       (501) staff       (20)       20 2023-04-13 12:01:21.000000 django-data-history-0.1.9/django_data_history.egg-info/top_level.txt
+-rw-r--r--   0 test       (501) staff       (20)      129 2022-10-31 07:23:44.000000 django-data-history-0.1.9/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2023-04-13 12:01:21.692837 django-data-history-0.1.9/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1437 2023-04-13 10:13:26.000000 django-data-history-0.1.9/setup.py
```

### Comparing `django-data-history-0.1.8/LICENSE` & `django-data-history-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-data-history-0.1.8/PKG-INFO` & `django-data-history-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-data-history
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Django application that allows you to store detailed data in the change log and display the detailed information in object's history view.
 Author: zencore
 Author-email: dobetter@zencore.cn
 License: MIT
 Keywords: django-data-history
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -137,7 +137,11 @@
 
 - Fix DataHistoryModelAdmin.get_data_histories function problem.
 
 ### v0.1.8
 
 - Fix problems in working together with django-import-export.
 - Add django_data_history_excludes support.
+
+### v0.1.9
+
+- Fix OneToOneField problem.
```

### Comparing `django-data-history-0.1.8/README.md` & `django-data-history-0.1.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -120,7 +120,11 @@
 
 - Fix DataHistoryModelAdmin.get_data_histories function problem.
 
 ### v0.1.8
 
 - Fix problems in working together with django-import-export.
 - Add django_data_history_excludes support.
+
+### v0.1.9
+
+- Fix OneToOneField problem.
```

### Comparing `django-data-history-0.1.8/django_data_history/__init__.py` & `django-data-history-0.1.9/django_data_history/__init__.py`

 * *Files identical despite different names*

### Comparing `django-data-history-0.1.8/django_data_history/admin.py` & `django-data-history-0.1.9/django_data_history/admin.py`

 * *Files identical despite different names*

### Comparing `django-data-history-0.1.8/django_data_history/apps.py` & `django-data-history-0.1.9/django_data_history/apps.py`

 * *Files identical despite different names*

### Comparing `django-data-history-0.1.8/django_data_history/locale/zh_Hans/LC_MESSAGES/django.mo` & `django-data-history-0.1.9/django_data_history/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-data-history-0.1.8/django_data_history/locale/zh_Hans/LC_MESSAGES/django.po` & `django-data-history-0.1.9/django_data_history/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-data-history-0.1.8/django_data_history/migrations/0001_initial.py` & `django-data-history-0.1.9/django_data_history/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-data-history-0.1.8/django_data_history/models.py` & `django-data-history-0.1.9/django_data_history/models.py`

 * *Files identical despite different names*

### Comparing `django-data-history-0.1.8/django_data_history/templates/admin/object_history.html` & `django-data-history-0.1.9/django_data_history/templates/admin/object_history.html`

 * *Files identical despite different names*

### Comparing `django-data-history-0.1.8/django_data_history/utils.py` & `django-data-history-0.1.9/django_data_history/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 #!/usr/bin/env python
 # -*- coding: utf8 -*-
 from __future__ import absolute_import, division, generators, nested_scopes, print_function, unicode_literals, with_statement
 
 import json
+from django.db.models.manager import BaseManager
 from django.core.serializers import serialize
 
+
 def post_admin_autodiscover(callback):
     from django.contrib import admin
     admin_old_autodiscover = admin.autodiscover
     def admin_new_autodiscover():
         admin_old_autodiscover()
         callback()
     admin.autodiscover = admin_new_autodiscover
 
+
 def pre_admin_autodiscover(callback):
     from django.contrib import admin
     admin_old_autodiscover = admin.autodiscover
     def admin_new_autodiscover():
         callback()
         admin_old_autodiscover()
     admin.autodiscover = admin_new_autodiscover
@@ -29,22 +32,26 @@
     data["id"] = info[0]["pk"]
 
     for name in item.__class__._meta.fields_map.keys():
         if "+" in name:
             continue
         if not hasattr(item, name):
             continue
-        text = serialize("json", getattr(item, name).all(), use_natural_foreign_keys=True)
+        iqueryset = getattr(item, name)
+        if isinstance(iqueryset, BaseManager):
+            text = serialize("json", iqueryset.all(), use_natural_foreign_keys=True)
+        else:
+            text = serialize("json", [iqueryset], use_natural_foreign_keys=True)
         infos = json.loads(text)
         data2 = []
         for info in infos:
             data3 = info["fields"]
             data3["id"] = info["pk"]
             data2.append(data3)
         data[name] = data2
 
     django_data_history_excludes = getattr(item.__class__, "django_data_history_excludes", [])
     for field in django_data_history_excludes:
         if field in data:
             del data[field]
 
-    return data
+    return data
```

### Comparing `django-data-history-0.1.8/django_data_history.egg-info/PKG-INFO` & `django-data-history-0.1.9/django_data_history.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-data-history
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Django application that allows you to store detailed data in the change log and display the detailed information in object's history view.
 Author: zencore
 Author-email: dobetter@zencore.cn
 License: MIT
 Keywords: django-data-history
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -137,7 +137,11 @@
 
 - Fix DataHistoryModelAdmin.get_data_histories function problem.
 
 ### v0.1.8
 
 - Fix problems in working together with django-import-export.
 - Add django_data_history_excludes support.
+
+### v0.1.9
+
+- Fix OneToOneField problem.
```

### Comparing `django-data-history-0.1.8/django_data_history.egg-info/SOURCES.txt` & `django-data-history-0.1.9/django_data_history.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-data-history-0.1.8/setup.py` & `django-data-history-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 with open(os.path.join(here, 'requirements.txt'), "r", encoding="utf-8") as fobj:
     requires = [x.strip() for x in fobj.readlines() if x.strip()]
 
 
 setup(
     name="django-data-history",
-    version="0.1.8",
+    version="0.1.9",
     description="A Django application that allows you to store detailed data in the change log and display the detailed information in object's history view.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="zencore",
     author_email="dobetter@zencore.cn",
     license="MIT",
     classifiers=[
```

