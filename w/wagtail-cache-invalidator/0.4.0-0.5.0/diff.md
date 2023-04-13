# Comparing `tmp/wagtail-cache-invalidator-0.4.0.tar.gz` & `tmp/wagtail-cache-invalidator-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-cache-invalidator-0.4.0.tar", last modified: Fri Nov 25 13:24:09 2022, max compression
+gzip compressed data, was "wagtail-cache-invalidator-0.5.0.tar", last modified: Thu Apr 13 12:34:49 2023, max compression
```

## Comparing `wagtail-cache-invalidator-0.4.0.tar` & `wagtail-cache-invalidator-0.5.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-11-25 13:24:09.863777 wagtail-cache-invalidator-0.4.0/
--rw-r--r--   0 robmoorman   (501) staff       (20)      164 2022-08-18 07:16:51.000000 wagtail-cache-invalidator-0.4.0/MANIFEST.in
--rw-r--r--   0 robmoorman   (501) staff       (20)      285 2022-11-25 13:24:09.863378 wagtail-cache-invalidator-0.4.0/PKG-INFO
--rw-r--r--   0 robmoorman   (501) staff       (20)       38 2022-11-25 13:24:09.863920 wagtail-cache-invalidator-0.4.0/setup.cfg
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-11-25 13:24:09.857199 wagtail-cache-invalidator-0.4.0/src/
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-11-25 13:24:09.861170 wagtail-cache-invalidator-0.4.0/src/wagtail_cache_invalidator/
--rw-r--r--   0 robmoorman   (501) staff       (20)       87 2022-08-18 07:16:51.000000 wagtail-cache-invalidator-0.4.0/src/wagtail_cache_invalidator/__init__.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      178 2022-08-18 07:16:51.000000 wagtail-cache-invalidator-0.4.0/src/wagtail_cache_invalidator/admin_urls.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      406 2022-08-19 11:53:10.000000 wagtail-cache-invalidator-0.4.0/src/wagtail_cache_invalidator/apps.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      547 2022-11-25 13:22:25.000000 wagtail-cache-invalidator-0.4.0/src/wagtail_cache_invalidator/forms.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-11-25 13:24:09.862379 wagtail-cache-invalidator-0.4.0/src/wagtail_cache_invalidator/migrations/
--rw-r--r--   0 robmoorman   (501) staff       (20)     1551 2022-08-18 07:16:51.000000 wagtail-cache-invalidator-0.4.0/src/wagtail_cache_invalidator/migrations/0001_initial.py
--rw-r--r--   0 robmoorman   (501) staff       (20)     1808 2022-08-19 12:37:18.000000 wagtail-cache-invalidator-0.4.0/src/wagtail_cache_invalidator/migrations/0002_cachesettings.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      560 2022-11-25 13:22:48.000000 wagtail-cache-invalidator-0.4.0/src/wagtail_cache_invalidator/migrations/0003_purgecachesite.py
--rw-r--r--   0 robmoorman   (501) staff       (20)        0 2022-08-18 07:16:51.000000 wagtail-cache-invalidator-0.4.0/src/wagtail_cache_invalidator/migrations/__init__.py
--rw-r--r--   0 robmoorman   (501) staff       (20)     3468 2022-11-25 13:22:25.000000 wagtail-cache-invalidator-0.4.0/src/wagtail_cache_invalidator/models.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      154 2022-08-19 12:05:05.000000 wagtail-cache-invalidator-0.4.0/src/wagtail_cache_invalidator/settings.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      710 2022-08-19 12:05:13.000000 wagtail-cache-invalidator-0.4.0/src/wagtail_cache_invalidator/signal_handlers.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-11-25 13:24:09.857656 wagtail-cache-invalidator-0.4.0/src/wagtail_cache_invalidator/templates/
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-11-25 13:24:09.862606 wagtail-cache-invalidator-0.4.0/src/wagtail_cache_invalidator/templates/ wagtailcacheinvalidator/
--rw-r--r--   0 robmoorman   (501) staff       (20)     2051 2022-11-25 13:12:14.000000 wagtail-cache-invalidator-0.4.0/src/wagtail_cache_invalidator/templates/ wagtailcacheinvalidator/purge.html
--rw-r--r--   0 robmoorman   (501) staff       (20)      947 2022-08-19 12:53:55.000000 wagtail-cache-invalidator-0.4.0/src/wagtail_cache_invalidator/utils.py
--rw-r--r--   0 robmoorman   (501) staff       (20)     1623 2022-08-18 07:16:51.000000 wagtail-cache-invalidator-0.4.0/src/wagtail_cache_invalidator/views.py
--rw-r--r--   0 robmoorman   (501) staff       (20)     2652 2022-08-18 07:16:51.000000 wagtail-cache-invalidator-0.4.0/src/wagtail_cache_invalidator/wagtail_hooks.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-11-25 13:24:09.862960 wagtail-cache-invalidator-0.4.0/src/wagtail_cache_invalidator.egg-info/
--rw-r--r--   0 robmoorman   (501) staff       (20)      743 2022-11-25 13:24:09.000000 wagtail-cache-invalidator-0.4.0/src/wagtail_cache_invalidator.egg-info/SOURCES.txt
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-04-13 12:34:49.846361 wagtail-cache-invalidator-0.5.0/
+-rw-r--r--   0 robmoorman   (501) staff       (20)      164 2022-08-18 07:16:51.000000 wagtail-cache-invalidator-0.5.0/MANIFEST.in
+-rw-r--r--   0 robmoorman   (501) staff       (20)      285 2023-04-13 12:34:49.845875 wagtail-cache-invalidator-0.5.0/PKG-INFO
+-rw-r--r--   0 robmoorman   (501) staff       (20)       38 2023-04-13 12:34:49.846499 wagtail-cache-invalidator-0.5.0/setup.cfg
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-04-13 12:34:49.836440 wagtail-cache-invalidator-0.5.0/src/
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-04-13 12:34:49.841432 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/
+-rw-r--r--   0 robmoorman   (501) staff       (20)       87 2022-08-18 07:16:51.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/__init__.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      178 2022-08-18 07:16:51.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/admin_urls.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      406 2022-08-19 11:53:10.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/apps.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      547 2022-11-25 13:22:25.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/forms.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-04-13 12:34:49.844411 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/migrations/
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1550 2023-04-13 11:29:31.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/migrations/0001_initial.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1807 2023-04-13 11:29:31.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/migrations/0002_cachesettings.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      559 2023-04-13 11:29:31.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/migrations/0003_purgecachesite.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)        0 2022-08-18 07:16:51.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/migrations/__init__.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)     3746 2023-04-13 11:48:09.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/models.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      200 2023-04-13 11:37:45.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/settings.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1033 2023-04-13 12:24:47.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/signal_handlers.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      356 2023-04-13 11:37:51.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/signals.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-04-13 12:34:49.836924 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/templates/
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-04-13 12:34:49.844790 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/templates/ wagtailcacheinvalidator/
+-rw-r--r--   0 robmoorman   (501) staff       (20)     2051 2022-11-25 13:12:14.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/templates/ wagtailcacheinvalidator/purge.html
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1107 2023-04-13 11:57:44.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/utils.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1623 2022-08-18 07:16:51.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/views.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)     2652 2022-08-18 07:16:51.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/wagtail_hooks.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-04-13 12:34:49.845395 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator.egg-info/
+-rw-r--r--   0 robmoorman   (501) staff       (20)      784 2023-04-13 12:34:49.000000 wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator.egg-info/SOURCES.txt
```

### Comparing `wagtail-cache-invalidator-0.4.0/src/wagtail_cache_invalidator/forms.py` & `wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/forms.py`

 * *Files identical despite different names*

### Comparing `wagtail-cache-invalidator-0.4.0/src/wagtail_cache_invalidator/migrations/0001_initial.py` & `wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import django.db.models.deletion
 from django.conf import settings
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = []
 
     operations = [
         migrations.CreateModel(
             name="InvalidationRequest",
```

### Comparing `wagtail-cache-invalidator-0.4.0/src/wagtail_cache_invalidator/migrations/0002_cachesettings.py` & `wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/migrations/0002_cachesettings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 3.2.12 on 2022-08-19 12:37
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("wagtailcore", "0066_collection_management_permissions"),
         ("wagtailcacheinvalidator", "0001_initial"),
     ]
 
     operations = [
         migrations.CreateModel(
```

### Comparing `wagtail-cache-invalidator-0.4.0/src/wagtail_cache_invalidator/migrations/0003_purgecachesite.py` & `wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/migrations/0003_purgecachesite.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 4.1.3 on 2022-11-25 13:22
 
 from django.db import migrations
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("wagtailcore", "0078_referenceindex"),
         ("wagtailcacheinvalidator", "0002_cachesettings"),
     ]
 
     operations = [
         migrations.CreateModel(
```

### Comparing `wagtail-cache-invalidator-0.4.0/src/wagtail_cache_invalidator/models.py` & `wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,16 @@
     MultiFieldPanel,
     ObjectList,
     TabbedInterface,
 )
 from wagtail.contrib.settings.models import BaseSetting, register_setting
 from wagtail.core.models import Site
 
+from wagtail_cache_invalidator import signals
+from wagtail_cache_invalidator.settings import ASYNC
 from wagtail_cache_invalidator.utils import purge_urls_from_cache
 
 PURGE_ALL_HELP_TXT = _("Purge all cache for this site when pages are (un)published")
 
 
 class PurgeCacheSite(Site):
     class Meta:
@@ -107,8 +109,13 @@
     if action == "post_add":
         for site in instance.sites.all():
             urls = []
             root_url = site.root_url
             for path in instance.urls.splitlines():
                 url = root_url + path
                 urls.append(url)
-            purge_urls_from_cache(site, urls)
+            if ASYNC:
+                signals.purge_urls_from_cache.send(
+                    sender=sender, site_id=site.id, urls=urls
+                )
+            else:
+                purge_urls_from_cache(site.id, urls)
```

### Comparing `wagtail-cache-invalidator-0.4.0/src/wagtail_cache_invalidator/templates/ wagtailcacheinvalidator/purge.html` & `wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/templates/ wagtailcacheinvalidator/purge.html`

 * *Files identical despite different names*

### Comparing `wagtail-cache-invalidator-0.4.0/src/wagtail_cache_invalidator/utils.py` & `wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,26 +2,32 @@
     purge_page_from_cache as wagtail_purge_page_from_cache,
 )
 from wagtail.contrib.frontend_cache.utils import (
     purge_urls_from_cache as wagtail_purge_urls_from_cache,
 )
 
 
-def purge_urls_from_cache(site, urls):
+def purge_urls_from_cache(site_id, urls):
+    from wagtail.models import Site
+
     from wagtail_cache_invalidator.models import CacheSettings
 
+    site = Site.objects.get(id=site_id)
     cache_settings = CacheSettings.for_site(site)
     backend_settings = cache_settings.backend_settings
 
     wagtail_purge_urls_from_cache(urls, backend_settings=backend_settings)
 
 
-def purge_page_from_cache(page):
+def purge_page_from_cache(page_id):
+    from wagtail.models import Page
+
     from wagtail_cache_invalidator.models import CacheSettings
 
+    page = Page.objects.get(id=page_id)
     site = page.get_site()
     cache_settings = CacheSettings.for_site(site)
     backend_settings = cache_settings.backend_settings
 
     if cache_settings.purge_all:
         wagtail_purge_urls_from_cache(["/*"], backend_settings=backend_settings)
     else:
```

### Comparing `wagtail-cache-invalidator-0.4.0/src/wagtail_cache_invalidator/views.py` & `wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-cache-invalidator-0.4.0/src/wagtail_cache_invalidator/wagtail_hooks.py` & `wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cache-invalidator-0.4.0/src/wagtail_cache_invalidator.egg-info/SOURCES.txt` & `wagtail-cache-invalidator-0.5.0/src/wagtail_cache_invalidator.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 src/wagtail_cache_invalidator/__init__.py
 src/wagtail_cache_invalidator/admin_urls.py
 src/wagtail_cache_invalidator/apps.py
 src/wagtail_cache_invalidator/forms.py
 src/wagtail_cache_invalidator/models.py
 src/wagtail_cache_invalidator/settings.py
 src/wagtail_cache_invalidator/signal_handlers.py
+src/wagtail_cache_invalidator/signals.py
 src/wagtail_cache_invalidator/utils.py
 src/wagtail_cache_invalidator/views.py
 src/wagtail_cache_invalidator/wagtail_hooks.py
 src/wagtail_cache_invalidator/migrations/0001_initial.py
 src/wagtail_cache_invalidator/migrations/0002_cachesettings.py
 src/wagtail_cache_invalidator/migrations/0003_purgecachesite.py
 src/wagtail_cache_invalidator/migrations/__init__.py
```

