# Comparing `tmp/pretix_plugin_attendance_certificate-0.1.3.tar.gz` & `tmp/pretix_plugin_attendance_certificate-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix_plugin_attendance_certificate-0.1.3.tar", last modified: Wed Apr 12 16:15:47 2023, max compression
+gzip compressed data, was "pretix_plugin_attendance_certificate-0.1.4.tar", last modified: Thu Apr 13 14:00:06 2023, max compression
```

## Comparing `pretix_plugin_attendance_certificate-0.1.3.tar` & `pretix_plugin_attendance_certificate-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     1070 2023-04-12 16:15:36.189731 pretix_plugin_attendance_certificate-0.1.3/LICENSE
--rw-r--r--   0        0        0      161 2023-04-12 16:15:36.189731 pretix_plugin_attendance_certificate-0.1.3/README.md
--rw-r--r--   0        0        0     1100 2023-04-12 16:15:36.189731 pretix_plugin_attendance_certificate-0.1.3/pretix_attendance_certificate/__init__.py
--rw-r--r--   0        0        0      313 2023-04-12 16:15:36.189731 pretix_plugin_attendance_certificate-0.1.3/pretix_attendance_certificate/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-04-12 16:15:36.189731 pretix_plugin_attendance_certificate-0.1.3/pretix_attendance_certificate/locale/de_Informal/.gitkeep
--rw-r--r--   0        0        0      313 2023-04-12 16:15:36.189731 pretix_plugin_attendance_certificate-0.1.3/pretix_attendance_certificate/locale/de_Informal/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1960 2023-04-12 16:15:36.189731 pretix_plugin_attendance_certificate-0.1.3/pretix_attendance_certificate/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-04-12 16:15:36.189731 pretix_plugin_attendance_certificate-0.1.3/pretix_attendance_certificate/migrations/__init__.py
--rw-r--r--   0        0        0     1380 2023-04-12 16:15:36.189731 pretix_plugin_attendance_certificate-0.1.3/pretix_attendance_certificate/models.py
--rw-r--r--   0        0        0     1516 2023-04-12 16:15:36.189731 pretix_plugin_attendance_certificate-0.1.3/pretix_attendance_certificate/render.py
--rw-r--r--   0        0        0     1997 2023-04-12 16:15:36.193731 pretix_plugin_attendance_certificate-0.1.3/pretix_attendance_certificate/signals.py
--rw-r--r--   0        0        0        0 2023-04-12 16:15:36.193731 pretix_plugin_attendance_certificate-0.1.3/pretix_attendance_certificate/static/pretix_attendance_certificate/.gitkeep
--rw-r--r--   0        0        0      779 2023-04-12 16:15:36.193731 pretix_plugin_attendance_certificate-0.1.3/pretix_attendance_certificate/static/pretix_attendance_certificate/empty_attendance_certificate.pdf
--rw-r--r--   0        0        0     2615 2023-04-12 16:15:36.193731 pretix_plugin_attendance_certificate-0.1.3/pretix_attendance_certificate/tasks.py
--rw-r--r--   0        0        0        0 2023-04-12 16:15:36.193731 pretix_plugin_attendance_certificate-0.1.3/pretix_attendance_certificate/templates/pretix_attendance_certificate/.gitkeep
--rw-r--r--   0        0        0      117 2023-04-12 16:15:36.193731 pretix_plugin_attendance_certificate-0.1.3/pretix_attendance_certificate/templates/pretix_attendance_certificate/send_form_fragment_attendance_certificate.html
--rw-r--r--   0        0        0      495 2023-04-12 16:15:36.193731 pretix_plugin_attendance_certificate-0.1.3/pretix_attendance_certificate/urls.py
--rw-r--r--   0        0        0        0 2023-04-12 16:15:36.193731 pretix_plugin_attendance_certificate-0.1.3/pretix_attendance_certificate/views/__init__.py
--rw-r--r--   0        0        0     3611 2023-04-12 16:15:36.193731 pretix_plugin_attendance_certificate-0.1.3/pretix_attendance_certificate/views/editor.py
--rw-r--r--   0        0        0     1967 2023-04-12 16:15:36.193731 pretix_plugin_attendance_certificate-0.1.3/pretix_attendance_certificate/views/emails.py
--rw-r--r--   0        0        0      706 2023-04-12 16:15:47.269608 pretix_plugin_attendance_certificate-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-12 16:15:36.193731 pretix_plugin_attendance_certificate-0.1.3/tests/conftest.py
--rw-r--r--   0        0        0      385 1970-01-01 00:00:00.000000 pretix_plugin_attendance_certificate-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-13 13:59:48.137488 pretix_plugin_attendance_certificate-0.1.4/LICENSE
+-rw-r--r--   0        0        0      161 2023-04-13 13:59:48.137488 pretix_plugin_attendance_certificate-0.1.4/README.md
+-rw-r--r--   0        0        0     1100 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/__init__.py
+-rw-r--r--   0        0        0      313 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/locale/de_Informal/.gitkeep
+-rw-r--r--   0        0        0      313 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/locale/de_Informal/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1960 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/migrations/__init__.py
+-rw-r--r--   0        0        0     1380 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/models.py
+-rw-r--r--   0        0        0     1516 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/render.py
+-rw-r--r--   0        0        0     2478 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/signals.py
+-rw-r--r--   0        0        0        0 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/static/pretix_attendance_certificate/.gitkeep
+-rw-r--r--   0        0        0      779 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/static/pretix_attendance_certificate/empty_attendance_certificate.pdf
+-rw-r--r--   0        0        0     2615 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/tasks.py
+-rw-r--r--   0        0        0        0 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/templates/pretix_attendance_certificate/.gitkeep
+-rw-r--r--   0        0        0       90 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/templates/pretix_attendance_certificate/history_fragment_attendance_certificate.html
+-rw-r--r--   0        0        0      117 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/templates/pretix_attendance_certificate/send_form_fragment_attendance_certificate.html
+-rw-r--r--   0        0        0      495 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/urls.py
+-rw-r--r--   0        0        0        0 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/views/__init__.py
+-rw-r--r--   0        0        0     3611 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/views/editor.py
+-rw-r--r--   0        0        0     2319 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/views/emails.py
+-rw-r--r--   0        0        0      706 2023-04-13 14:00:06.657369 pretix_plugin_attendance_certificate-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-13 13:59:48.141488 pretix_plugin_attendance_certificate-0.1.4/tests/conftest.py
+-rw-r--r--   0        0        0      385 1970-01-01 00:00:00.000000 pretix_plugin_attendance_certificate-0.1.4/PKG-INFO
```

### Comparing `pretix_plugin_attendance_certificate-0.1.3/LICENSE` & `pretix_plugin_attendance_certificate-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.3/pretix_attendance_certificate/__init__.py` & `pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/__init__.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.3/pretix_attendance_certificate/migrations/0001_initial.py` & `pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.3/pretix_attendance_certificate/models.py` & `pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/models.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.3/pretix_attendance_certificate/render.py` & `pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/render.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.3/pretix_attendance_certificate/signals.py` & `pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/signals.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,29 +24,41 @@
             "url": reverse(
                 "plugins:pretix_attendance_certificate:edit",
                 kwargs={
                     "event": request.event.slug,
                     "organizer": request.event.organizer.slug,
                 },
             ),
-            "active": url.namespace == "plugins:pretix_attendance_certificate",
+            "active": False,
             "icon": "id-card",
             "children": [
                 {
+                    "label": _("Editor"),
+                    "url": reverse(
+                        "plugins:pretix_attendance_certificate:edit",
+                        kwargs={
+                            "event": request.event.slug,
+                            "organizer": request.event.organizer.slug,
+                        },
+                    ),
+                    "active": url.namespace == "plugins:pretix_attendance_certificate"
+                    and url.url_name == "edit",
+                },
+                {
                     "label": _("Send out certificates"),
                     "url": reverse(
                         "plugins:pretix_attendance_certificate:send",
                         kwargs={
                             "event": request.event.slug,
                             "organizer": request.event.organizer.slug,
                         },
                     ),
                     "active": url.namespace == "plugins:pretix_attendance_certificate"
                     and url.url_name == "send",
-                }
+                },
             ],
         }
     ]
 
 
 @receiver(
     sendmail_view_classes, dispatch_uid="pretix_attendance_certificate_sendmail_view"
```

### Comparing `pretix_plugin_attendance_certificate-0.1.3/pretix_attendance_certificate/static/pretix_attendance_certificate/empty_attendance_certificate.pdf` & `pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/static/pretix_attendance_certificate/empty_attendance_certificate.pdf`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.3/pretix_attendance_certificate/tasks.py` & `pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/tasks.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.3/pretix_attendance_certificate/views/editor.py` & `pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/views/editor.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.3/pretix_attendance_certificate/views/emails.py` & `pretix_plugin_attendance_certificate-0.1.4/pretix_attendance_certificate/views/emails.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from django.urls import reverse
+from django.template.loader import get_template
 from django.contrib.humanize.templatetags.humanize import intcomma
 from django.utils.translation import gettext_lazy as _, ngettext
 
 from pretix.plugins.sendmail.views import BaseSenderView
 from pretix.plugins.sendmail.forms import BaseMailForm
 from pretix.base.models import OrderPosition, Order
 
@@ -53,7 +54,18 @@
         ) % {
             "number": intcomma(cnt or 0),
         }
 
     def get_task_kwargs(self, form, objects):
         kwargs = super().get_task_kwargs(form, objects)
         return kwargs
+
+    @classmethod
+    def show_history_meta_data(cls, logentry, _cache_store):
+        tpl = get_template(
+            "pretix_attendance_certificate/history_fragment_attendance_certificate.html"
+        )
+        return tpl.render(
+            {
+                "log": logentry,
+            }
+        )
```

### Comparing `pretix_plugin_attendance_certificate-0.1.3/pyproject.toml` & `pretix_plugin_attendance_certificate-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "pretix-plugin-attendance-certificate"
-version = "0.1.3"
+version = "0.1.4"
 description = "Create attendance certificates"
 authors = [
     { name = "Python Italia" },
 ]
 dependencies = []
 requires-python = ">=3.9,<4.0"
 readme = "README.md"
```

