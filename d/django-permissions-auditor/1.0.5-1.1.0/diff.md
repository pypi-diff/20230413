# Comparing `tmp/django-permissions-auditor-1.0.5.tar.gz` & `tmp/django-permissions-auditor-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\django-permissions-auditor-1.0.5.tar", last modified: Mon Jan 10 18:12:05 2022, max compression
+gzip compressed data, was "django-permissions-auditor-1.1.0.tar", last modified: Wed Apr 12 22:45:39 2023, max compression
```

## Comparing `django-permissions-auditor-1.0.5.tar` & `django-permissions-auditor-1.1.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2022-01-10 18:12:05.314970 django-permissions-auditor-1.0.5/
--rw-rw-rw-   0        0        0     1060 2019-01-08 16:43:26.000000 django-permissions-auditor-1.0.5/LICENSE
--rw-rw-rw-   0        0        0       87 2019-01-03 21:22:29.000000 django-permissions-auditor-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2515 2022-01-10 18:12:05.314970 django-permissions-auditor-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1069 2020-12-03 19:33:14.000000 django-permissions-auditor-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2022-01-10 18:12:05.251507 django-permissions-auditor-1.0.5/django_permissions_auditor.egg-info/
--rw-rw-rw-   0        0        0     2515 2022-01-10 18:12:04.000000 django-permissions-auditor-1.0.5/django_permissions_auditor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1657 2022-01-10 18:12:04.000000 django-permissions-auditor-1.0.5/django_permissions_auditor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-10 18:12:04.000000 django-permissions-auditor-1.0.5/django_permissions_auditor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2020-07-01 21:37:13.000000 django-permissions-auditor-1.0.5/django_permissions_auditor.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       22 2022-01-10 18:12:04.000000 django-permissions-auditor-1.0.5/django_permissions_auditor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2022-01-10 18:12:04.000000 django-permissions-auditor-1.0.5/django_permissions_auditor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-01-10 18:12:05.263225 django-permissions-auditor-1.0.5/permissions_auditor/
--rw-rw-rw-   0        0        0      206 2022-01-10 18:03:58.000000 django-permissions-auditor-1.0.5/permissions_auditor/__init__.py
--rw-rw-rw-   0        0        0     7623 2021-03-12 22:14:35.000000 django-permissions-auditor-1.0.5/permissions_auditor/admin.py
--rw-rw-rw-   0        0        0      630 2022-01-10 17:48:04.000000 django-permissions-auditor-1.0.5/permissions_auditor/apps.py
--rw-rw-rw-   0        0        0     5179 2022-01-10 16:44:57.000000 django-permissions-auditor-1.0.5/permissions_auditor/core.py
--rw-rw-rw-   0        0        0     1202 2020-12-21 21:14:16.000000 django-permissions-auditor-1.0.5/permissions_auditor/defaults.py
--rw-rw-rw-   0        0        0     1002 2019-01-08 17:16:48.000000 django-permissions-auditor-1.0.5/permissions_auditor/forms.py
-drwxrwxrwx   0        0        0        0 2022-01-10 18:12:05.264200 django-permissions-auditor-1.0.5/permissions_auditor/management/
--rw-rw-rw-   0        0        0        0 2019-02-11 23:30:31.000000 django-permissions-auditor-1.0.5/permissions_auditor/management/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-10 18:12:05.267128 django-permissions-auditor-1.0.5/permissions_auditor/management/commands/
--rw-rw-rw-   0        0        0        0 2019-02-11 23:39:24.000000 django-permissions-auditor-1.0.5/permissions_auditor/management/commands/__init__.py
--rw-rw-rw-   0        0        0     1396 2019-02-12 00:26:13.000000 django-permissions-auditor-1.0.5/permissions_auditor/management/commands/check_view_permissions.py
-drwxrwxrwx   0        0        0        0 2022-01-10 18:12:05.276893 django-permissions-auditor-1.0.5/permissions_auditor/processors/
--rw-rw-rw-   0        0        0        0 2018-12-18 17:22:40.000000 django-permissions-auditor-1.0.5/permissions_auditor/processors/__init__.py
--rw-rw-rw-   0        0        0     7321 2019-12-31 15:08:45.000000 django-permissions-auditor-1.0.5/permissions_auditor/processors/auth_decorators.py
--rw-rw-rw-   0        0        0     2580 2019-01-08 15:40:14.000000 django-permissions-auditor-1.0.5/permissions_auditor/processors/auth_mixins.py
--rw-rw-rw-   0        0        0     6602 2020-07-01 21:25:39.000000 django-permissions-auditor-1.0.5/permissions_auditor/processors/base.py
-drwxrwxrwx   0        0        0        0 2022-01-10 18:12:05.196304 django-permissions-auditor-1.0.5/permissions_auditor/templates/
-drwxrwxrwx   0        0        0        0 2022-01-10 18:12:05.196304 django-permissions-auditor-1.0.5/permissions_auditor/templates/permissions_auditor/
-drwxrwxrwx   0        0        0        0 2022-01-10 18:12:05.279822 django-permissions-auditor-1.0.5/permissions_auditor/templates/permissions_auditor/admin/
--rw-rw-rw-   0        0        0     5831 2019-01-22 15:31:46.000000 django-permissions-auditor-1.0.5/permissions_auditor/templates/permissions_auditor/admin/permission_detail.html
--rw-rw-rw-   0        0        0     6876 2020-12-21 19:24:09.000000 django-permissions-auditor-1.0.5/permissions_auditor/templates/permissions_auditor/admin/views_index.html
-drwxrwxrwx   0        0        0        0 2022-01-10 18:12:05.299382 django-permissions-auditor-1.0.5/permissions_auditor/tests/
--rw-rw-rw-   0        0        0        0 2018-12-19 16:13:53.000000 django-permissions-auditor-1.0.5/permissions_auditor/tests/__init__.py
--rw-rw-rw-   0        0        0      649 2019-12-31 15:08:45.000000 django-permissions-auditor-1.0.5/permissions_auditor/tests/base.py
-drwxrwxrwx   0        0        0        0 2022-01-10 18:12:05.313016 django-permissions-auditor-1.0.5/permissions_auditor/tests/fixtures/
--rw-rw-rw-   0        0        0        0 2019-01-04 15:15:29.000000 django-permissions-auditor-1.0.5/permissions_auditor/tests/fixtures/__init__.py
--rw-rw-rw-   0        0        0      146 2019-12-31 15:08:45.000000 django-permissions-auditor-1.0.5/permissions_auditor/tests/fixtures/base_views.py
--rw-rw-rw-   0        0        0     3096 2019-12-31 15:08:45.000000 django-permissions-auditor-1.0.5/permissions_auditor/tests/fixtures/decorator_views.py
--rw-rw-rw-   0        0        0     1784 2019-12-31 15:08:45.000000 django-permissions-auditor-1.0.5/permissions_auditor/tests/fixtures/mixin_views.py
--rw-rw-rw-   0        0        0     1454 2022-01-10 17:44:39.000000 django-permissions-auditor-1.0.5/permissions_auditor/tests/fixtures/urls.py
--rw-rw-rw-   0        0        0     3671 2019-12-31 15:08:45.000000 django-permissions-auditor-1.0.5/permissions_auditor/tests/fixtures/views.py
--rw-rw-rw-   0        0        0    11414 2019-12-31 15:08:45.000000 django-permissions-auditor-1.0.5/permissions_auditor/tests/test_auth_decorator_processors.py
--rw-rw-rw-   0        0        0     5699 2019-12-31 15:08:45.000000 django-permissions-auditor-1.0.5/permissions_auditor/tests/test_auth_mixin_processors.py
--rw-rw-rw-   0        0        0     2566 2019-12-31 15:08:45.000000 django-permissions-auditor-1.0.5/permissions_auditor/tests/test_base_processors.py
--rw-rw-rw-   0        0        0     5343 2020-12-22 17:19:33.000000 django-permissions-auditor-1.0.5/permissions_auditor/tests/test_core.py
--rw-rw-rw-   0        0        0      393 2019-12-31 15:08:17.000000 django-permissions-auditor-1.0.5/permissions_auditor/tests/test_management.py
--rw-rw-rw-   0        0        0     1132 2020-09-22 15:42:45.000000 django-permissions-auditor-1.0.5/permissions_auditor/tests/test_settings.py
--rw-rw-rw-   0        0        0       42 2022-01-10 18:12:05.314970 django-permissions-auditor-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1742 2022-01-10 16:55:00.000000 django-permissions-auditor-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 22:45:39.776093 django-permissions-auditor-1.1.0/
+-rw-rw-rw-   0        0        0     1060 2019-01-08 16:43:26.000000 django-permissions-auditor-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       87 2019-01-03 21:22:29.000000 django-permissions-auditor-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2371 2023-04-12 22:45:39.776093 django-permissions-auditor-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1069 2020-12-03 19:33:14.000000 django-permissions-auditor-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 22:45:39.675853 django-permissions-auditor-1.1.0/django_permissions_auditor.egg-info/
+-rw-rw-rw-   0        0        0     2371 2023-04-12 22:45:39.000000 django-permissions-auditor-1.1.0/django_permissions_auditor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1657 2023-04-12 22:45:39.000000 django-permissions-auditor-1.1.0/django_permissions_auditor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 22:45:39.000000 django-permissions-auditor-1.1.0/django_permissions_auditor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2020-07-01 21:37:13.000000 django-permissions-auditor-1.1.0/django_permissions_auditor.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       23 2023-04-12 22:45:39.000000 django-permissions-auditor-1.1.0/django_permissions_auditor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-12 22:45:39.000000 django-permissions-auditor-1.1.0/django_permissions_auditor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 22:45:39.691462 django-permissions-auditor-1.1.0/permissions_auditor/
+-rw-rw-rw-   0        0        0      206 2023-04-12 22:39:19.000000 django-permissions-auditor-1.1.0/permissions_auditor/__init__.py
+-rw-rw-rw-   0        0        0     7623 2021-03-12 22:14:35.000000 django-permissions-auditor-1.1.0/permissions_auditor/admin.py
+-rw-rw-rw-   0        0        0      630 2022-01-10 17:48:04.000000 django-permissions-auditor-1.1.0/permissions_auditor/apps.py
+-rw-rw-rw-   0        0        0     5179 2022-01-10 16:44:57.000000 django-permissions-auditor-1.1.0/permissions_auditor/core.py
+-rw-rw-rw-   0        0        0     1202 2020-12-21 21:14:16.000000 django-permissions-auditor-1.1.0/permissions_auditor/defaults.py
+-rw-rw-rw-   0        0        0     1002 2019-01-08 17:16:48.000000 django-permissions-auditor-1.1.0/permissions_auditor/forms.py
+drwxrwxrwx   0        0        0        0 2023-04-12 22:45:39.707086 django-permissions-auditor-1.1.0/permissions_auditor/management/
+-rw-rw-rw-   0        0        0        0 2019-02-11 23:30:31.000000 django-permissions-auditor-1.1.0/permissions_auditor/management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 22:45:39.713592 django-permissions-auditor-1.1.0/permissions_auditor/management/commands/
+-rw-rw-rw-   0        0        0        0 2019-02-11 23:39:24.000000 django-permissions-auditor-1.1.0/permissions_auditor/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     1396 2019-02-12 00:26:13.000000 django-permissions-auditor-1.1.0/permissions_auditor/management/commands/check_view_permissions.py
+drwxrwxrwx   0        0        0        0 2023-04-12 22:45:39.713592 django-permissions-auditor-1.1.0/permissions_auditor/processors/
+-rw-rw-rw-   0        0        0        0 2018-12-18 17:22:40.000000 django-permissions-auditor-1.1.0/permissions_auditor/processors/__init__.py
+-rw-rw-rw-   0        0        0     7321 2019-12-31 15:08:45.000000 django-permissions-auditor-1.1.0/permissions_auditor/processors/auth_decorators.py
+-rw-rw-rw-   0        0        0     2557 2023-04-12 22:33:57.000000 django-permissions-auditor-1.1.0/permissions_auditor/processors/auth_mixins.py
+-rw-rw-rw-   0        0        0     6605 2023-04-12 22:33:57.000000 django-permissions-auditor-1.1.0/permissions_auditor/processors/base.py
+drwxrwxrwx   0        0        0        0 2023-04-12 22:45:39.613338 django-permissions-auditor-1.1.0/permissions_auditor/templates/
+drwxrwxrwx   0        0        0        0 2023-04-12 22:45:39.613338 django-permissions-auditor-1.1.0/permissions_auditor/templates/permissions_auditor/
+drwxrwxrwx   0        0        0        0 2023-04-12 22:45:39.713592 django-permissions-auditor-1.1.0/permissions_auditor/templates/permissions_auditor/admin/
+-rw-rw-rw-   0        0        0     5831 2023-04-12 22:14:44.000000 django-permissions-auditor-1.1.0/permissions_auditor/templates/permissions_auditor/admin/permission_detail.html
+-rw-rw-rw-   0        0        0     6876 2020-12-21 19:24:09.000000 django-permissions-auditor-1.1.0/permissions_auditor/templates/permissions_auditor/admin/views_index.html
+drwxrwxrwx   0        0        0        0 2023-04-12 22:45:39.744845 django-permissions-auditor-1.1.0/permissions_auditor/tests/
+-rw-rw-rw-   0        0        0        0 2018-12-19 16:13:53.000000 django-permissions-auditor-1.1.0/permissions_auditor/tests/__init__.py
+-rw-rw-rw-   0        0        0      649 2019-12-31 15:08:45.000000 django-permissions-auditor-1.1.0/permissions_auditor/tests/base.py
+drwxrwxrwx   0        0        0        0 2023-04-12 22:45:39.776093 django-permissions-auditor-1.1.0/permissions_auditor/tests/fixtures/
+-rw-rw-rw-   0        0        0        0 2019-01-04 15:15:29.000000 django-permissions-auditor-1.1.0/permissions_auditor/tests/fixtures/__init__.py
+-rw-rw-rw-   0        0        0      146 2019-12-31 15:08:45.000000 django-permissions-auditor-1.1.0/permissions_auditor/tests/fixtures/base_views.py
+-rw-rw-rw-   0        0        0     3096 2019-12-31 15:08:45.000000 django-permissions-auditor-1.1.0/permissions_auditor/tests/fixtures/decorator_views.py
+-rw-rw-rw-   0        0        0     1784 2019-12-31 15:08:45.000000 django-permissions-auditor-1.1.0/permissions_auditor/tests/fixtures/mixin_views.py
+-rw-rw-rw-   0        0        0     1454 2022-01-10 17:44:39.000000 django-permissions-auditor-1.1.0/permissions_auditor/tests/fixtures/urls.py
+-rw-rw-rw-   0        0        0     3924 2023-04-12 22:33:57.000000 django-permissions-auditor-1.1.0/permissions_auditor/tests/fixtures/views.py
+-rw-rw-rw-   0        0        0    11414 2019-12-31 15:08:45.000000 django-permissions-auditor-1.1.0/permissions_auditor/tests/test_auth_decorator_processors.py
+-rw-rw-rw-   0        0        0     6324 2023-04-12 22:33:57.000000 django-permissions-auditor-1.1.0/permissions_auditor/tests/test_auth_mixin_processors.py
+-rw-rw-rw-   0        0        0     2567 2023-04-12 22:33:57.000000 django-permissions-auditor-1.1.0/permissions_auditor/tests/test_base_processors.py
+-rw-rw-rw-   0        0        0     5343 2020-12-22 17:19:33.000000 django-permissions-auditor-1.1.0/permissions_auditor/tests/test_core.py
+-rw-rw-rw-   0        0        0      393 2019-12-31 15:08:17.000000 django-permissions-auditor-1.1.0/permissions_auditor/tests/test_management.py
+-rw-rw-rw-   0        0        0     1132 2020-09-22 15:42:45.000000 django-permissions-auditor-1.1.0/permissions_auditor/tests/test_settings.py
+-rw-rw-rw-   0        0        0       42 2023-04-12 22:45:39.776093 django-permissions-auditor-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1784 2023-04-12 22:41:18.000000 django-permissions-auditor-1.1.0/setup.py
```

### Comparing `django-permissions-auditor-1.0.5/LICENSE` & `django-permissions-auditor-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-permissions-auditor-1.0.5/PKG-INFO` & `django-permissions-auditor-1.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 Metadata-Version: 2.1
 Name: django-permissions-auditor
-Version: 1.0.5
+Version: 1.1.0
 Summary: django-permissions-auditor is a tool to audit access control on your django app.
 Home-page: https://github.com/AACEngineering/django-permissions-auditor
 Author: AAC Engineering
 License: MIT
-Description: django-permissions-auditor
-        ==========================
-        
-        ![Build](https://github.com/AACEngineering/django-permissions-auditor/workflows/Test/badge.svg)
-        [![codecov](https://codecov.io/gh/AACEngineering/django-permissions-auditor/branch/master/graph/badge.svg)](https://codecov.io/gh/AACEngineering/django-permissions-auditor)
-        [![](https://img.shields.io/pypi/v/django-permissions-auditor.svg)](https://pypi.org/project/django-permissions-auditor/)
-        [![](https://readthedocs.org/projects/django-permissions-auditor/badge/?version=latest&style=flat)](https://django-permissions-auditor.readthedocs.io/en/latest/)
-        
-        
-        https://django-permissions-auditor.readthedocs.io/en/latest/
-        
-        
-        Admin site for auditing and managing permissions for views in your Django app.
-        
-        
-        ![Screenshot](docs/img/admin_views.png?raw=true "Screenshot")
-        
-        
-        Automatically parse Django views in your project and pull out the permissions required to view them. Easily extensible to work with custom permission schemes.
-        
-        
-        ![Screenshot](docs/img/admin_permissions.png?raw=true "Screenshot")
-        
 Keywords: django,admin,permissions,audit,auditor
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management :: Link Checking
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+django-permissions-auditor
+==========================
+
+![Build](https://github.com/AACEngineering/django-permissions-auditor/workflows/Test/badge.svg)
+[![codecov](https://codecov.io/gh/AACEngineering/django-permissions-auditor/branch/master/graph/badge.svg)](https://codecov.io/gh/AACEngineering/django-permissions-auditor)
+[![](https://img.shields.io/pypi/v/django-permissions-auditor.svg)](https://pypi.org/project/django-permissions-auditor/)
+[![](https://readthedocs.org/projects/django-permissions-auditor/badge/?version=latest&style=flat)](https://django-permissions-auditor.readthedocs.io/en/latest/)
+
+
+https://django-permissions-auditor.readthedocs.io/en/latest/
+
+
+Admin site for auditing and managing permissions for views in your Django app.
+
+
+![Screenshot](docs/img/admin_views.png?raw=true "Screenshot")
+
+
+Automatically parse Django views in your project and pull out the permissions required to view them. Easily extensible to work with custom permission schemes.
+
+
+![Screenshot](docs/img/admin_permissions.png?raw=true "Screenshot")
```

### Comparing `django-permissions-auditor-1.0.5/README.md` & `django-permissions-auditor-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `django-permissions-auditor-1.0.5/django_permissions_auditor.egg-info/PKG-INFO` & `django-permissions-auditor-1.1.0/django_permissions_auditor.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 Metadata-Version: 2.1
 Name: django-permissions-auditor
-Version: 1.0.5
+Version: 1.1.0
 Summary: django-permissions-auditor is a tool to audit access control on your django app.
 Home-page: https://github.com/AACEngineering/django-permissions-auditor
 Author: AAC Engineering
 License: MIT
-Description: django-permissions-auditor
-        ==========================
-        
-        ![Build](https://github.com/AACEngineering/django-permissions-auditor/workflows/Test/badge.svg)
-        [![codecov](https://codecov.io/gh/AACEngineering/django-permissions-auditor/branch/master/graph/badge.svg)](https://codecov.io/gh/AACEngineering/django-permissions-auditor)
-        [![](https://img.shields.io/pypi/v/django-permissions-auditor.svg)](https://pypi.org/project/django-permissions-auditor/)
-        [![](https://readthedocs.org/projects/django-permissions-auditor/badge/?version=latest&style=flat)](https://django-permissions-auditor.readthedocs.io/en/latest/)
-        
-        
-        https://django-permissions-auditor.readthedocs.io/en/latest/
-        
-        
-        Admin site for auditing and managing permissions for views in your Django app.
-        
-        
-        ![Screenshot](docs/img/admin_views.png?raw=true "Screenshot")
-        
-        
-        Automatically parse Django views in your project and pull out the permissions required to view them. Easily extensible to work with custom permission schemes.
-        
-        
-        ![Screenshot](docs/img/admin_permissions.png?raw=true "Screenshot")
-        
 Keywords: django,admin,permissions,audit,auditor
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management :: Link Checking
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+django-permissions-auditor
+==========================
+
+![Build](https://github.com/AACEngineering/django-permissions-auditor/workflows/Test/badge.svg)
+[![codecov](https://codecov.io/gh/AACEngineering/django-permissions-auditor/branch/master/graph/badge.svg)](https://codecov.io/gh/AACEngineering/django-permissions-auditor)
+[![](https://img.shields.io/pypi/v/django-permissions-auditor.svg)](https://pypi.org/project/django-permissions-auditor/)
+[![](https://readthedocs.org/projects/django-permissions-auditor/badge/?version=latest&style=flat)](https://django-permissions-auditor.readthedocs.io/en/latest/)
+
+
+https://django-permissions-auditor.readthedocs.io/en/latest/
+
+
+Admin site for auditing and managing permissions for views in your Django app.
+
+
+![Screenshot](docs/img/admin_views.png?raw=true "Screenshot")
+
+
+Automatically parse Django views in your project and pull out the permissions required to view them. Easily extensible to work with custom permission schemes.
+
+
+![Screenshot](docs/img/admin_permissions.png?raw=true "Screenshot")
```

### Comparing `django-permissions-auditor-1.0.5/django_permissions_auditor.egg-info/SOURCES.txt` & `django-permissions-auditor-1.1.0/django_permissions_auditor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-permissions-auditor-1.0.5/permissions_auditor/admin.py` & `django-permissions-auditor-1.1.0/permissions_auditor/admin.py`

 * *Files identical despite different names*

### Comparing `django-permissions-auditor-1.0.5/permissions_auditor/apps.py` & `django-permissions-auditor-1.1.0/permissions_auditor/apps.py`

 * *Files identical despite different names*

### Comparing `django-permissions-auditor-1.0.5/permissions_auditor/core.py` & `django-permissions-auditor-1.1.0/permissions_auditor/core.py`

 * *Files identical despite different names*

### Comparing `django-permissions-auditor-1.0.5/permissions_auditor/defaults.py` & `django-permissions-auditor-1.1.0/permissions_auditor/defaults.py`

 * *Files identical despite different names*

### Comparing `django-permissions-auditor-1.0.5/permissions_auditor/forms.py` & `django-permissions-auditor-1.1.0/permissions_auditor/forms.py`

 * *Files identical despite different names*

### Comparing `django-permissions-auditor-1.0.5/permissions_auditor/management/commands/check_view_permissions.py` & `django-permissions-auditor-1.1.0/permissions_auditor/management/commands/check_view_permissions.py`

 * *Files identical despite different names*

### Comparing `django-permissions-auditor-1.0.5/permissions_auditor/processors/auth_decorators.py` & `django-permissions-auditor-1.1.0/permissions_auditor/processors/auth_decorators.py`

 * *Files identical despite different names*

### Comparing `django-permissions-auditor-1.0.5/permissions_auditor/processors/auth_mixins.py` & `django-permissions-auditor-1.1.0/permissions_auditor/processors/auth_mixins.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Processors for django auth mixins."""
 
 import inspect
 
 from django.conf import ImproperlyConfigured
 
-from .base import BaseFileredMixinProcessor
+from .base import BaseFilteredMixinProcessor
 
 
-class PermissionRequiredMixinProcessor(BaseFileredMixinProcessor):
+class PermissionRequiredMixinProcessor(BaseFilteredMixinProcessor):
     """
-    Processes views that directly inherit from
+    Processes views that inherit from
     ``django.contrib.auth.mixins.PermissionRequiredMixin``.
 
     .. hint::
         If the ``has_permission()`` function is overridden, any docstrings on that
         function will be displayed in the additional info column.
     """
 
@@ -37,29 +37,29 @@
 
             if docstring is None or docstring.startswith('Override this method'):
                 docstring = 'Custom (no docstring found)'
 
         return docstring
 
 
-class LoginRequiredMixinProcessor(BaseFileredMixinProcessor):
+class LoginRequiredMixinProcessor(BaseFilteredMixinProcessor):
     """
-    Processes views that directly inherit from
+    Processes views that inherit from
     ``django.contrib.auth.mixins.LoginRequiredMixin``.
     """
 
     class_filter = 'django.contrib.auth.mixins.LoginRequiredMixin'
 
     def get_login_required(self, view):
         return True
 
 
-class UserPassesTestMixinProcessor(BaseFileredMixinProcessor):
+class UserPassesTestMixinProcessor(BaseFilteredMixinProcessor):
     """
-    Processes views that directly inherit from
+    Processes views that inherit from
     ``django.contrib.auth.mixins.UserPassesTestMixin``.
 
     .. hint::
         If the function returned by ``get_test_func()`` is overridden, any docstrings
         on that function will be displayed in the additional info column.
 
     .. note::
```

### Comparing `django-permissions-auditor-1.0.5/permissions_auditor/processors/base.py` & `django-permissions-auditor-1.1.0/permissions_auditor/processors/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,32 +149,32 @@
 
             if 'view_func' in closures:
                 return self._has_func_decorator(closures['view_func'], func_name)
 
         return False
 
 
-class BaseFileredMixinProcessor(BaseCBVProcessor):
+class BaseFilteredMixinProcessor(BaseCBVProcessor):
     """
     Base class for parsing mixins on class based views.
     Set ``class_filter`` to filter the class names the processor applies to.
     ONLY checks top level base classes.
 
     :var class_filter: initial value: ``None``
     """
     class_filter = None
 
     def can_process(self, view):
         if not super().can_process(view):
             return False
 
-        view_bases = [cls.__module__ + '.' + cls.__name__ for cls in view.__bases__]
+        view_parents = [cls.__module__ + '.' + cls.__name__ for cls in view.__mro__]
 
         for cls_filter in self.get_class_filter():
-            if cls_filter in view_bases:
+            if cls_filter in view_parents:
                 return True
 
         return False
 
     def get_class_filter(self):
         """
         Override this method to override the class_names attribute.
```

### Comparing `django-permissions-auditor-1.0.5/permissions_auditor/templates/permissions_auditor/admin/permission_detail.html` & `django-permissions-auditor-1.1.0/permissions_auditor/templates/permissions_auditor/admin/permission_detail.html`

 * *Files identical despite different names*

### Comparing `django-permissions-auditor-1.0.5/permissions_auditor/templates/permissions_auditor/admin/views_index.html` & `django-permissions-auditor-1.1.0/permissions_auditor/templates/permissions_auditor/admin/views_index.html`

 * *Files identical despite different names*

### Comparing `django-permissions-auditor-1.0.5/permissions_auditor/tests/base.py` & `django-permissions-auditor-1.1.0/permissions_auditor/tests/base.py`

 * *Files identical despite different names*

### Comparing `django-permissions-auditor-1.0.5/permissions_auditor/tests/fixtures/decorator_views.py` & `django-permissions-auditor-1.1.0/permissions_auditor/tests/fixtures/decorator_views.py`

 * *Files identical despite different names*

### Comparing `django-permissions-auditor-1.0.5/permissions_auditor/tests/fixtures/mixin_views.py` & `django-permissions-auditor-1.1.0/permissions_auditor/tests/fixtures/mixin_views.py`

 * *Files identical despite different names*

### Comparing `django-permissions-auditor-1.0.5/permissions_auditor/tests/fixtures/urls.py` & `django-permissions-auditor-1.1.0/permissions_auditor/tests/fixtures/urls.py`

 * *Files identical despite different names*

### Comparing `django-permissions-auditor-1.0.5/permissions_auditor/tests/fixtures/views.py` & `django-permissions-auditor-1.1.0/permissions_auditor/tests/fixtures/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,24 +17,32 @@
     pass
 
 
 class LoginRequiredView(LoginRequiredMixin, View):
     pass
 
 
+class InheritedLoginRequiredView(LoginRequiredView):
+    pass
+
+
 class LoginRequiredMethodDecoratorView(View):
     @method_decorator(login_required)
     def dispatch(self, request, *args, **kwargs):
         return super().dispatch(request, *args, **kwargs)
 
 
 class PermissionRequiredView(PermissionRequiredMixin, View):
     permission_required = 'tests.test_perm'
 
 
+class InheritedPermissionRequiredView(PermissionRequiredView):
+    pass
+
+
 class PermissionRequiredMultiView(PermissionRequiredMixin, View):
     permission_required = ('tests.test_perm', 'tests.test_perm2')
 
 
 class PermissionRequiredViewNoPerm(PermissionRequiredMixin, View):
 
     def has_permission(self):
@@ -70,14 +78,19 @@
 
 
 class UserPassesTestView(UserPassesTestMixin, View):
     def test_func(self):
         return True
 
 
+class InheritedUserPassesTestView(UserPassesTestView):
+    def test_func(self):
+        return True
+
+
 class UserPassesTestViewDocstring(UserPassesTestMixin, View):
     def test_func(self):
         """Custom docstrings should be detected."""
         return True
 
 
 class UserPassesTestViewNoDocstring(UserPassesTestMixin, View):
```

### Comparing `django-permissions-auditor-1.0.5/permissions_auditor/tests/test_auth_decorator_processors.py` & `django-permissions-auditor-1.1.0/permissions_auditor/tests/test_auth_decorator_processors.py`

 * *Files identical despite different names*

### Comparing `django-permissions-auditor-1.0.5/permissions_auditor/tests/test_auth_mixin_processors.py` & `django-permissions-auditor-1.1.0/permissions_auditor/tests/test_auth_mixin_processors.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,17 @@
             views.UserPassesTestView, views.UserPassesTestViewCustomFunc,
             views.UserPassesTestViewDocstring, views.UserPassesTestViewNoDocstring
         ])
 
     def test_cb_loginrequiredview(self):
         self.assertCanProcessView(views.LoginRequiredView, **self.expected_results)
 
+    def test_cb_inheritedloginrequiredview(self):
+        self.assertCanProcessView(views.InheritedLoginRequiredView, **self.expected_results)
+
 
 class TestPermissionRequiredMixinProcessor(MixinProcessorTestCaseMixin, ProcessorTestCase):
 
     def setUp(self):
         self.processor = auth_mixins.PermissionRequiredMixinProcessor()
 
     def test_cannot_process(self):
@@ -51,14 +54,20 @@
 
     def test_cb_permissionsrequiredview(self):
         self.assertCanProcessView(
             views.PermissionRequiredView,
             permissions=['tests.test_perm'], login_required=True, docstring=None
         )
 
+    def test_cb_inherit_permissionsrequiredview(self):
+        self.assertCanProcessView(
+            views.InheritedPermissionRequiredView,
+            permissions=['tests.test_perm'], login_required=True, docstring=None
+        )
+
     def test_cb_permissionsrequiredview_no_perm(self):
         """
         Views that override has_permission() and do not set permission_required should be processed.
         """
         self.assertCanProcessView(
             views.PermissionRequiredViewNoPerm,
             permissions=[], login_required=True, docstring='The user\'s first name must be Bob'
@@ -108,14 +117,20 @@
 
     def test_cb_userpassestestview(self):
         self.assertCanProcessView(
             views.UserPassesTestView,
             permissions=[], login_required=None, docstring='Custom (no docstring found)'
         )
 
+    def test_cb_inheriteduserpassestestview(self):
+        self.assertCanProcessView(
+            views.InheritedUserPassesTestView,
+            permissions=[], login_required=None, docstring='Custom (no docstring found)'
+        )
+
     def test_cb_userpassestestview_docstring(self):
         """Views that implement test_func() and have a docstring should be retrieved."""
         self.assertCanProcessView(
             views.UserPassesTestViewDocstring,
             permissions=[], login_required=None, docstring='Custom docstrings should be detected.'
         )
```

### Comparing `django-permissions-auditor-1.0.5/permissions_auditor/tests/test_base_processors.py` & `django-permissions-auditor-1.1.0/permissions_auditor/tests/test_base_processors.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     def test_can_process_function(self):
         self.assertCannotProcess([views.base_view])
 
 
 class BaseFilteredMixinProcessorTest(ProcessorTestCase):
     def setUp(self):
-        self.processor = base.BaseFileredMixinProcessor()
+        self.processor = base.BaseFilteredMixinProcessor()
 
     def test_no_class_filter_raises_exception(self):
         with self.assertRaises(ImproperlyConfigured):
             self.assertCannotProcess([views.PermissionRequiredView])
 
     def test_can_process_filtered_class(self):
         self.processor.class_filter = 'django.contrib.auth.mixins.PermissionRequiredMixin'
```

### Comparing `django-permissions-auditor-1.0.5/permissions_auditor/tests/test_core.py` & `django-permissions-auditor-1.1.0/permissions_auditor/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `django-permissions-auditor-1.0.5/permissions_auditor/tests/test_settings.py` & `django-permissions-auditor-1.1.0/permissions_auditor/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django-permissions-auditor-1.0.5/setup.py` & `django-permissions-auditor-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,33 +14,34 @@
     author='AAC Engineering',
     url='https://github.com/AACEngineering/django-permissions-auditor',
     license='MIT',
     packages=find_packages(exclude=['example']),
     include_package_data=True,
     python_requires='>=3.5',
     install_requires=[
-        'django>=2.1'
-        'setuptools'
+        'django>=2.1',
+        'setuptools',
     ],
     zip_safe=False,
     test_suite='runtests.runtests',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Framework :: Django',
         'Framework :: Django :: 2.2',
         'Framework :: Django :: 3.2',
-        'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
         'Topic :: Internet :: WWW/HTTP :: Site Management',
         'Topic :: Internet :: WWW/HTTP :: Site Management :: Link Checking',
     ],
     keywords='django,admin,permissions,audit,auditor',
 )
```

