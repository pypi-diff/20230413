# Comparing `tmp/inventory-monitor-4.0.5.tar.gz` & `tmp/inventory-monitor-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inventory-monitor-4.0.5.tar", last modified: Wed Apr  5 08:42:02 2023, max compression
+gzip compressed data, was "inventory-monitor-4.1.0.tar", last modified: Thu Apr 13 10:44:59 2023, max compression
```

## Comparing `inventory-monitor-4.0.5.tar` & `inventory-monitor-4.1.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 08:42:02.090916 inventory-monitor-4.0.5/
--rw-r--r--   0 root         (0) root         (0)       66 2022-08-17 08:16:04.000000 inventory-monitor-4.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      186 2023-04-05 08:42:02.090916 inventory-monitor-4.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      150 2022-11-11 11:56:29.000000 inventory-monitor-4.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 08:42:02.086916 inventory-monitor-4.0.5/inventory_monitor/
--rw-r--r--   0 root         (0) root         (0)      315 2023-04-05 08:40:22.000000 inventory-monitor-4.0.5/inventory_monitor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 08:42:02.086916 inventory-monitor-4.0.5/inventory_monitor/api/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-16 10:45:32.000000 inventory-monitor-4.0.5/inventory_monitor/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7025 2023-04-04 11:53:46.000000 inventory-monitor-4.0.5/inventory_monitor/api/serializers.py
--rw-r--r--   0 root         (0) root         (0)      476 2023-02-28 13:24:51.000000 inventory-monitor-4.0.5/inventory_monitor/api/urls.py
--rw-r--r--   0 root         (0) root         (0)     1606 2023-02-28 13:24:51.000000 inventory-monitor-4.0.5/inventory_monitor/api/views.py
--rw-r--r--   0 root         (0) root         (0)    16616 2023-03-27 12:08:03.000000 inventory-monitor-4.0.5/inventory_monitor/filtersets.py
--rw-r--r--   0 root         (0) root         (0)    19322 2023-03-27 12:16:44.000000 inventory-monitor-4.0.5/inventory_monitor/forms.py
--rw-r--r--   0 root         (0) root         (0)      459 2022-09-05 08:34:29.000000 inventory-monitor-4.0.5/inventory_monitor/graphql.py
--rw-r--r--   0 root         (0) root         (0)     1247 2023-02-28 13:24:51.000000 inventory-monitor-4.0.5/inventory_monitor/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 08:42:02.090916 inventory-monitor-4.0.5/inventory_monitor/migrations/
--rw-r--r--   0 root         (0) root         (0)     2329 2022-09-01 10:14:20.000000 inventory-monitor-4.0.5/inventory_monitor/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)     3198 2022-11-02 08:30:17.000000 inventory-monitor-4.0.5/inventory_monitor/migrations/0002_contractor_contract.py
--rw-r--r--   0 root         (0) root         (0)     1811 2022-11-11 11:48:13.000000 inventory-monitor-4.0.5/inventory_monitor/migrations/0003_alter_contract_price_invmonfileattachment.py
--rw-r--r--   0 root         (0) root         (0)      342 2022-11-11 11:48:53.000000 inventory-monitor-4.0.5/inventory_monitor/migrations/0004_delete_invmonfileattachment.py
--rw-r--r--   0 root         (0) root         (0)     1840 2022-11-22 11:20:11.000000 inventory-monitor-4.0.5/inventory_monitor/migrations/0005_invoice.py
--rw-r--r--   0 root         (0) root         (0)      409 2022-12-01 11:16:30.000000 inventory-monitor-4.0.5/inventory_monitor/migrations/0006_invoice_project.py
--rw-r--r--   0 root         (0) root         (0)     5622 2023-02-28 13:24:51.000000 inventory-monitor-4.0.5/inventory_monitor/migrations/0007_component_alter_contract_custom_field_data_and_more.py
--rw-r--r--   0 root         (0) root         (0)      436 2023-02-28 13:24:51.000000 inventory-monitor-4.0.5/inventory_monitor/migrations/0008_componentservice_comments.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-02-28 13:24:51.000000 inventory-monitor-4.0.5/inventory_monitor/migrations/0009_alter_component_items.py
--rw-r--r--   0 root         (0) root         (0)     1446 2023-03-27 12:15:02.000000 inventory-monitor-4.0.5/inventory_monitor/migrations/0010_componentimport_alter_component_options_and_more.py
--rw-r--r--   0 root         (0) root         (0)      721 2023-03-27 12:09:05.000000 inventory-monitor-4.0.5/inventory_monitor/migrations/0011_alter_component_options_and_more.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-04-03 15:32:31.000000 inventory-monitor-4.0.5/inventory_monitor/migrations/0012_probe_creation_time.py
--rw-r--r--   0 root         (0) root         (0)      479 2023-04-04 12:29:41.000000 inventory-monitor-4.0.5/inventory_monitor/migrations/0013_alter_probe_creation_time.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-22 08:26:09.000000 inventory-monitor-4.0.5/inventory_monitor/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12803 2023-04-04 12:29:25.000000 inventory-monitor-4.0.5/inventory_monitor/models.py
--rw-r--r--   0 root         (0) root         (0)     1050 2023-03-27 12:54:38.000000 inventory-monitor-4.0.5/inventory_monitor/navigation.py
--rw-r--r--   0 root         (0) root         (0)     1447 2023-02-28 13:24:51.000000 inventory-monitor-4.0.5/inventory_monitor/search.py
--rw-r--r--   0 root         (0) root         (0)     5070 2023-04-05 08:31:19.000000 inventory-monitor-4.0.5/inventory_monitor/tables.py
--rw-r--r--   0 root         (0) root         (0)     2337 2023-04-05 08:34:53.000000 inventory-monitor-4.0.5/inventory_monitor/template_content.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 08:42:02.086916 inventory-monitor-4.0.5/inventory_monitor/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 08:42:02.090916 inventory-monitor-4.0.5/inventory_monitor/templates/inventory_monitor/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-15 12:39:23.000000 inventory-monitor-4.0.5/inventory_monitor/templates/inventory_monitor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5195 2023-03-27 12:07:28.000000 inventory-monitor-4.0.5/inventory_monitor/templates/inventory_monitor/component.html
--rw-r--r--   0 root         (0) root         (0)     2988 2023-02-28 13:24:51.000000 inventory-monitor-4.0.5/inventory_monitor/templates/inventory_monitor/componentservice.html
--rw-r--r--   0 root         (0) root         (0)     6537 2023-02-28 13:24:51.000000 inventory-monitor-4.0.5/inventory_monitor/templates/inventory_monitor/contract.html
--rw-r--r--   0 root         (0) root         (0)     2109 2023-02-28 13:24:51.000000 inventory-monitor-4.0.5/inventory_monitor/templates/inventory_monitor/contractor.html
--rw-r--r--   0 root         (0) root         (0)     1558 2022-10-19 08:26:09.000000 inventory-monitor-4.0.5/inventory_monitor/templates/inventory_monitor/device_probes_include.html
--rw-r--r--   0 root         (0) root         (0)      155 2023-03-27 13:55:51.000000 inventory-monitor-4.0.5/inventory_monitor/templates/inventory_monitor/import_component_button.html
--rw-r--r--   0 root         (0) root         (0)     2238 2022-11-23 07:44:17.000000 inventory-monitor-4.0.5/inventory_monitor/templates/inventory_monitor/inventory_item_duplicates_include.html
--rw-r--r--   0 root         (0) root         (0)     2301 2023-02-28 13:24:51.000000 inventory-monitor-4.0.5/inventory_monitor/templates/inventory_monitor/invoice.html
--rw-r--r--   0 root         (0) root         (0)     5690 2023-04-04 12:47:57.000000 inventory-monitor-4.0.5/inventory_monitor/templates/inventory_monitor/probe.html
--rw-r--r--   0 root         (0) root         (0)     4097 2023-03-27 12:19:41.000000 inventory-monitor-4.0.5/inventory_monitor/urls.py
--rw-r--r--   0 root         (0) root         (0)    11064 2023-04-05 08:30:46.000000 inventory-monitor-4.0.5/inventory_monitor/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 08:42:02.086916 inventory-monitor-4.0.5/inventory_monitor.egg-info/
--rw-r--r--   0 root         (0) root         (0)      186 2023-04-05 08:42:02.000000 inventory-monitor-4.0.5/inventory_monitor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2250 2023-04-05 08:42:02.000000 inventory-monitor-4.0.5/inventory_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-05 08:42:02.000000 inventory-monitor-4.0.5/inventory_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-15 09:55:56.000000 inventory-monitor-4.0.5/inventory_monitor.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-05 08:42:02.000000 inventory-monitor-4.0.5/inventory_monitor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-05 08:42:02.090916 inventory-monitor-4.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      286 2023-04-05 08:40:16.000000 inventory-monitor-4.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:44:59.058448 inventory-monitor-4.1.0/
+-rw-r--r--   0 root         (0) root         (0)       66 2022-08-17 08:16:04.000000 inventory-monitor-4.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      186 2023-04-13 10:44:59.058448 inventory-monitor-4.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      150 2022-11-11 11:56:29.000000 inventory-monitor-4.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:44:59.030448 inventory-monitor-4.1.0/inventory_monitor/
+-rw-r--r--   0 root         (0) root         (0)      315 2023-04-13 10:44:43.000000 inventory-monitor-4.1.0/inventory_monitor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:44:59.038448 inventory-monitor-4.1.0/inventory_monitor/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-16 10:45:32.000000 inventory-monitor-4.1.0/inventory_monitor/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7025 2023-04-04 11:53:46.000000 inventory-monitor-4.1.0/inventory_monitor/api/serializers.py
+-rw-r--r--   0 root         (0) root         (0)      476 2023-02-28 13:24:51.000000 inventory-monitor-4.1.0/inventory_monitor/api/urls.py
+-rw-r--r--   0 root         (0) root         (0)     1606 2023-02-28 13:24:51.000000 inventory-monitor-4.1.0/inventory_monitor/api/views.py
+-rw-r--r--   0 root         (0) root         (0)    16616 2023-03-27 12:08:03.000000 inventory-monitor-4.1.0/inventory_monitor/filtersets.py
+-rw-r--r--   0 root         (0) root         (0)    19322 2023-03-27 12:16:44.000000 inventory-monitor-4.1.0/inventory_monitor/forms.py
+-rw-r--r--   0 root         (0) root         (0)      459 2022-09-05 08:34:29.000000 inventory-monitor-4.1.0/inventory_monitor/graphql.py
+-rw-r--r--   0 root         (0) root         (0)     1412 2023-04-13 10:44:43.000000 inventory-monitor-4.1.0/inventory_monitor/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:44:59.046448 inventory-monitor-4.1.0/inventory_monitor/migrations/
+-rw-r--r--   0 root         (0) root         (0)     2329 2022-09-01 10:14:20.000000 inventory-monitor-4.1.0/inventory_monitor/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)     3198 2022-11-02 08:30:17.000000 inventory-monitor-4.1.0/inventory_monitor/migrations/0002_contractor_contract.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2022-11-11 11:48:13.000000 inventory-monitor-4.1.0/inventory_monitor/migrations/0003_alter_contract_price_invmonfileattachment.py
+-rw-r--r--   0 root         (0) root         (0)      342 2022-11-11 11:48:53.000000 inventory-monitor-4.1.0/inventory_monitor/migrations/0004_delete_invmonfileattachment.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2022-11-22 11:20:11.000000 inventory-monitor-4.1.0/inventory_monitor/migrations/0005_invoice.py
+-rw-r--r--   0 root         (0) root         (0)      409 2022-12-01 11:16:30.000000 inventory-monitor-4.1.0/inventory_monitor/migrations/0006_invoice_project.py
+-rw-r--r--   0 root         (0) root         (0)     5622 2023-02-28 13:24:51.000000 inventory-monitor-4.1.0/inventory_monitor/migrations/0007_component_alter_contract_custom_field_data_and_more.py
+-rw-r--r--   0 root         (0) root         (0)      436 2023-02-28 13:24:51.000000 inventory-monitor-4.1.0/inventory_monitor/migrations/0008_componentservice_comments.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-02-28 13:24:51.000000 inventory-monitor-4.1.0/inventory_monitor/migrations/0009_alter_component_items.py
+-rw-r--r--   0 root         (0) root         (0)     1446 2023-03-27 12:15:02.000000 inventory-monitor-4.1.0/inventory_monitor/migrations/0010_componentimport_alter_component_options_and_more.py
+-rw-r--r--   0 root         (0) root         (0)      721 2023-03-27 12:09:05.000000 inventory-monitor-4.1.0/inventory_monitor/migrations/0011_alter_component_options_and_more.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-04-03 15:32:31.000000 inventory-monitor-4.1.0/inventory_monitor/migrations/0012_probe_creation_time.py
+-rw-r--r--   0 root         (0) root         (0)      479 2023-04-04 12:29:41.000000 inventory-monitor-4.1.0/inventory_monitor/migrations/0013_alter_probe_creation_time.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-22 08:26:09.000000 inventory-monitor-4.1.0/inventory_monitor/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12803 2023-04-13 10:38:29.000000 inventory-monitor-4.1.0/inventory_monitor/models.py
+-rw-r--r--   0 root         (0) root         (0)     1050 2023-03-27 12:54:38.000000 inventory-monitor-4.1.0/inventory_monitor/navigation.py
+-rw-r--r--   0 root         (0) root         (0)     1447 2023-02-28 13:24:51.000000 inventory-monitor-4.1.0/inventory_monitor/search.py
+-rw-r--r--   0 root         (0) root         (0)     5070 2023-04-05 08:31:19.000000 inventory-monitor-4.1.0/inventory_monitor/tables.py
+-rw-r--r--   0 root         (0) root         (0)     2049 2023-04-13 10:44:43.000000 inventory-monitor-4.1.0/inventory_monitor/template_content.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:44:59.018448 inventory-monitor-4.1.0/inventory_monitor/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:44:59.054448 inventory-monitor-4.1.0/inventory_monitor/templates/inventory_monitor/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-15 12:39:23.000000 inventory-monitor-4.1.0/inventory_monitor/templates/inventory_monitor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5195 2023-03-27 12:07:28.000000 inventory-monitor-4.1.0/inventory_monitor/templates/inventory_monitor/component.html
+-rw-r--r--   0 root         (0) root         (0)     2988 2023-02-28 13:24:51.000000 inventory-monitor-4.1.0/inventory_monitor/templates/inventory_monitor/componentservice.html
+-rw-r--r--   0 root         (0) root         (0)     6537 2023-02-28 13:24:51.000000 inventory-monitor-4.1.0/inventory_monitor/templates/inventory_monitor/contract.html
+-rw-r--r--   0 root         (0) root         (0)     2109 2023-02-28 13:24:51.000000 inventory-monitor-4.1.0/inventory_monitor/templates/inventory_monitor/contractor.html
+-rw-r--r--   0 root         (0) root         (0)     1558 2023-04-13 10:27:02.000000 inventory-monitor-4.1.0/inventory_monitor/templates/inventory_monitor/device_probes_include.html
+-rw-r--r--   0 root         (0) root         (0)      155 2023-03-27 13:55:51.000000 inventory-monitor-4.1.0/inventory_monitor/templates/inventory_monitor/import_component_button.html
+-rw-r--r--   0 root         (0) root         (0)     2238 2022-11-23 07:44:17.000000 inventory-monitor-4.1.0/inventory_monitor/templates/inventory_monitor/inventory_item_duplicates_include.html
+-rw-r--r--   0 root         (0) root         (0)     2301 2023-02-28 13:24:51.000000 inventory-monitor-4.1.0/inventory_monitor/templates/inventory_monitor/invoice.html
+-rw-r--r--   0 root         (0) root         (0)     5690 2023-04-04 12:47:57.000000 inventory-monitor-4.1.0/inventory_monitor/templates/inventory_monitor/probe.html
+-rw-r--r--   0 root         (0) root         (0)     4097 2023-03-27 12:19:41.000000 inventory-monitor-4.1.0/inventory_monitor/urls.py
+-rw-r--r--   0 root         (0) root         (0)    11064 2023-04-05 08:30:46.000000 inventory-monitor-4.1.0/inventory_monitor/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 10:44:59.034448 inventory-monitor-4.1.0/inventory_monitor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      186 2023-04-13 10:44:59.000000 inventory-monitor-4.1.0/inventory_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2250 2023-04-13 10:44:59.000000 inventory-monitor-4.1.0/inventory_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 10:44:59.000000 inventory-monitor-4.1.0/inventory_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-15 09:55:56.000000 inventory-monitor-4.1.0/inventory_monitor.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-13 10:44:59.000000 inventory-monitor-4.1.0/inventory_monitor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 10:44:59.058448 inventory-monitor-4.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      286 2023-04-13 10:44:43.000000 inventory-monitor-4.1.0/setup.py
```

### Comparing `inventory-monitor-4.0.5/inventory_monitor/api/serializers.py` & `inventory-monitor-4.1.0/inventory_monitor/api/serializers.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-4.0.5/inventory_monitor/api/views.py` & `inventory-monitor-4.1.0/inventory_monitor/api/views.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-4.0.5/inventory_monitor/filtersets.py` & `inventory-monitor-4.1.0/inventory_monitor/filtersets.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-4.0.5/inventory_monitor/forms.py` & `inventory-monitor-4.1.0/inventory_monitor/forms.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-4.0.5/inventory_monitor/helpers.py` & `inventory-monitor-4.1.0/inventory_monitor/helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,16 @@
     Args:
         number (decimal): number to format
 
     Returns:
         str: Formatted number
     """
     if number:
-        return '{:,}'.format(number).replace(',', ' ') + " Kč"
+        res = number.to_integral() if number == number.to_integral() else number.normalize()
+        return f"{res:,}".replace(',', ' ') + " Kč"
     else:
         return '---'
 
 
 class NumberColumn(django_tables2.Column):
     """Create a column that displays a number with a thousands separator.
 
@@ -26,15 +27,16 @@
 
     Returns:
         str: Formatted number
     """
 
     def render(self, value):
         if value:
-            return '{:,}'.format(value).replace(',', ' ') + " Kč"
+            res = value.to_integral() if value == value.to_integral() else value.normalize()
+            return f"{res:,}".replace(',', ' ') + " Kč"
         else:
             return '---'
 
 
 TEMPLATE_SERVICES_END = """
 {% for service in record.services.all %}
     {% if service.service_end %}
```

### Comparing `inventory-monitor-4.0.5/inventory_monitor/migrations/0001_initial.py` & `inventory-monitor-4.1.0/inventory_monitor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-4.0.5/inventory_monitor/migrations/0002_contractor_contract.py` & `inventory-monitor-4.1.0/inventory_monitor/migrations/0002_contractor_contract.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-4.0.5/inventory_monitor/migrations/0003_alter_contract_price_invmonfileattachment.py` & `inventory-monitor-4.1.0/inventory_monitor/migrations/0003_alter_contract_price_invmonfileattachment.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-4.0.5/inventory_monitor/migrations/0005_invoice.py` & `inventory-monitor-4.1.0/inventory_monitor/migrations/0005_invoice.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-4.0.5/inventory_monitor/migrations/0007_component_alter_contract_custom_field_data_and_more.py` & `inventory-monitor-4.1.0/inventory_monitor/migrations/0007_component_alter_contract_custom_field_data_and_more.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-4.0.5/inventory_monitor/migrations/0010_componentimport_alter_component_options_and_more.py` & `inventory-monitor-4.1.0/inventory_monitor/migrations/0010_componentimport_alter_component_options_and_more.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-4.0.5/inventory_monitor/migrations/0011_alter_component_options_and_more.py` & `inventory-monitor-4.1.0/inventory_monitor/migrations/0011_alter_component_options_and_more.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-4.0.5/inventory_monitor/models.py` & `inventory-monitor-4.1.0/inventory_monitor/models.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-4.0.5/inventory_monitor/navigation.py` & `inventory-monitor-4.1.0/inventory_monitor/navigation.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-4.0.5/inventory_monitor/search.py` & `inventory-monitor-4.1.0/inventory_monitor/search.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-4.0.5/inventory_monitor/tables.py` & `inventory-monitor-4.1.0/inventory_monitor/tables.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-4.0.5/inventory_monitor/template_content.py` & `inventory-monitor-4.1.0/inventory_monitor/template_content.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,33 @@
 from dcim.models import InventoryItem
-from django.db.models import Count, OuterRef, Subquery
 from extras.plugins import PluginTemplateExtension
 
 from .models import Probe
 
-# from django.conf import settings
-# plugin_settings = settings.PLUGINS_CONFIG.get('inventory_monitor', {})
+from django.conf import settings
+plugin_settings = settings.PLUGINS_CONFIG.get('inventory_monitor', {})
+import_component_url = plugin_settings.get(
+    "import_component_url", '/extras/scripts/component_import.ImportComponent/')
 
 
 class DeviceProbeList(PluginTemplateExtension):
     model = 'dcim.device'
 
     def right_page(self):
         obj = self.context['object']
 
-        # Latest inventory overall
-        # latest_inventory_pks = Probe.objects.all()\
-        #    .distinct('serial')\
-        #    .order_by('serial', '-time')\
-        #    .values('pk')
-
-        # Latest inventory per device
-        latest_inventory_pks = Probe.objects.all().order_by(
-            'serial', 'device_id', '-time').distinct('serial', 'device_id').values('pk')
-
-        device_probes = Probe.objects.filter(device=obj, pk__in=latest_inventory_pks)\
-            .prefetch_related('tags', 'device')
+        device_probes = Probe.objects.all()\
+            .order_by('serial', 'device_id', '-time')\
+            .distinct('serial', 'device_id')\
+            .filter(device=obj).prefetch_related('tags', 'device')
 
         return self.render(
             'inventory_monitor/device_probes_include.html',
             extra_context={
-                'device_probes': device_probes.order_by('-time')[:10],
+                'device_probes': device_probes[:10],
                 'total_device_probes_count': device_probes.count(),
             }
         )
 
 
 class InventoryItemDuplicates(PluginTemplateExtension):
     model = 'dcim.inventoryitem'
@@ -57,13 +50,13 @@
 
 class ImportComponentScriptButton(PluginTemplateExtension):
     model = 'inventory_monitor.component'
 
     def list_buttons(self):
         return self.render('inventory_monitor/import_component_button.html',
                            extra_context={
-                               'url': '/extras/scripts/component_import.ImportComponent/'}
+                               'url': import_component_url}
                            )
 
 
 template_extensions = [DeviceProbeList,
                        InventoryItemDuplicates, ImportComponentScriptButton]
```

### Comparing `inventory-monitor-4.0.5/inventory_monitor/templates/inventory_monitor/component.html` & `inventory-monitor-4.1.0/inventory_monitor/templates/inventory_monitor/component.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-4.0.5/inventory_monitor/templates/inventory_monitor/componentservice.html` & `inventory-monitor-4.1.0/inventory_monitor/templates/inventory_monitor/componentservice.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-4.0.5/inventory_monitor/templates/inventory_monitor/contract.html` & `inventory-monitor-4.1.0/inventory_monitor/templates/inventory_monitor/contract.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-4.0.5/inventory_monitor/templates/inventory_monitor/contractor.html` & `inventory-monitor-4.1.0/inventory_monitor/templates/inventory_monitor/contractor.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-4.0.5/inventory_monitor/templates/inventory_monitor/device_probes_include.html` & `inventory-monitor-4.1.0/inventory_monitor/templates/inventory_monitor/device_probes_include.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-4.0.5/inventory_monitor/templates/inventory_monitor/inventory_item_duplicates_include.html` & `inventory-monitor-4.1.0/inventory_monitor/templates/inventory_monitor/inventory_item_duplicates_include.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-4.0.5/inventory_monitor/templates/inventory_monitor/invoice.html` & `inventory-monitor-4.1.0/inventory_monitor/templates/inventory_monitor/invoice.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-4.0.5/inventory_monitor/templates/inventory_monitor/probe.html` & `inventory-monitor-4.1.0/inventory_monitor/templates/inventory_monitor/probe.html`

 * *Files identical despite different names*

### Comparing `inventory-monitor-4.0.5/inventory_monitor/urls.py` & `inventory-monitor-4.1.0/inventory_monitor/urls.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-4.0.5/inventory_monitor/views.py` & `inventory-monitor-4.1.0/inventory_monitor/views.py`

 * *Files identical despite different names*

### Comparing `inventory-monitor-4.0.5/inventory_monitor.egg-info/SOURCES.txt` & `inventory-monitor-4.1.0/inventory_monitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

