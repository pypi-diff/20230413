# Comparing `tmp/uptick_datawarehouse-0.2.5.tar.gz` & `tmp/uptick_datawarehouse-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uptick_datawarehouse-0.2.5.tar", max compression
+gzip compressed data, was "uptick_datawarehouse-0.2.6.tar", max compression
```

## Comparing `uptick_datawarehouse-0.2.5.tar` & `uptick_datawarehouse-0.2.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       24 2023-01-13 01:44:11.272938 uptick_datawarehouse-0.2.5/public_readme.md
--rw-r--r--   0        0        0      526 2023-02-09 01:18:54.783761 uptick_datawarehouse-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      200 2023-01-13 01:48:03.658500 uptick_datawarehouse-0.2.5/uptick_datawarehouse/model_settings.py
--rw-r--r--   0        0        0        0 2023-01-12 03:28:28.929168 uptick_datawarehouse-0.2.5/uptick_datawarehouse/subscriptionmanager/__init__.py
--rw-r--r--   0        0        0      191 2023-01-13 01:47:26.046172 uptick_datawarehouse-0.2.5/uptick_datawarehouse/subscriptionmanager/apps.py
--rw-r--r--   0        0        0      271 2023-01-12 03:28:28.929570 uptick_datawarehouse-0.2.5/uptick_datawarehouse/subscriptionmanager/migrations/0001_schema.py
--rw-r--r--   0        0        0    14332 2023-01-21 02:47:03.096787 uptick_datawarehouse-0.2.5/uptick_datawarehouse/subscriptionmanager/migrations/0002_changesummary_chargesummary_paymentmethodsummary_recurringcreditsummary_revenueforecastsummary_subsc.py
--rw-r--r--   0        0        0      699 2023-01-23 04:43:50.589352 uptick_datawarehouse-0.2.5/uptick_datawarehouse/subscriptionmanager/migrations/0003_auto_20230123_0443.py
--rw-r--r--   0        0        0        0 2023-01-12 03:28:28.930097 uptick_datawarehouse-0.2.5/uptick_datawarehouse/subscriptionmanager/migrations/__init__.py
--rw-r--r--   0        0        0    12040 2023-01-23 04:43:41.277818 uptick_datawarehouse-0.2.5/uptick_datawarehouse/subscriptionmanager/models.py
--rw-r--r--   0        0        0        0 2023-01-12 03:28:28.930464 uptick_datawarehouse-0.2.5/uptick_datawarehouse/superblocks/__init__.py
--rw-r--r--   0        0        0      175 2023-01-13 01:47:39.075510 uptick_datawarehouse-0.2.5/uptick_datawarehouse/superblocks/apps.py
--rw-r--r--   0        0        0      263 2023-01-12 03:28:28.930815 uptick_datawarehouse-0.2.5/uptick_datawarehouse/superblocks/migrations/0001_schema.py
--rw-r--r--   0        0        0        0 2023-01-12 03:28:28.930876 uptick_datawarehouse-0.2.5/uptick_datawarehouse/superblocks/migrations/__init__.py
--rw-r--r--   0        0        0        0 2023-01-12 03:28:28.932203 uptick_datawarehouse-0.2.5/uptick_datawarehouse/vitally/__init__.py
--rw-r--r--   0        0        0      167 2023-01-13 01:47:43.709643 uptick_datawarehouse-0.2.5/uptick_datawarehouse/vitally/apps.py
--rw-r--r--   0        0        0      259 2023-01-12 03:28:28.932792 uptick_datawarehouse-0.2.5/uptick_datawarehouse/vitally/migrations/0001_schema.py
--rw-r--r--   0        0        0        0 2023-01-12 03:28:28.932871 uptick_datawarehouse-0.2.5/uptick_datawarehouse/vitally/migrations/__init__.py
--rw-r--r--   0        0        0        0 2023-01-12 03:28:28.933549 uptick_datawarehouse-0.2.5/uptick_datawarehouse/workforce/__init__.py
--rw-r--r--   0        0        0      171 2023-01-13 01:47:49.225586 uptick_datawarehouse-0.2.5/uptick_datawarehouse/workforce/apps.py
--rw-r--r--   0        0        0      289 2023-01-12 03:28:28.934044 uptick_datawarehouse-0.2.5/uptick_datawarehouse/workforce/migrations/0001_schema.py
--rw-r--r--   0        0        0    10093 2023-01-21 03:00:22.637434 uptick_datawarehouse-0.2.5/uptick_datawarehouse/workforce/migrations/0002_initial.py
--rw-r--r--   0        0        0      396 2023-02-05 23:37:37.374239 uptick_datawarehouse-0.2.5/uptick_datawarehouse/workforce/migrations/0003_serverusage_contractor_addons_used.py
--rw-r--r--   0        0        0        0 2023-01-12 03:28:28.934250 uptick_datawarehouse-0.2.5/uptick_datawarehouse/workforce/migrations/__init__.py
--rw-r--r--   0        0        0     7204 2023-02-05 23:37:23.643244 uptick_datawarehouse-0.2.5/uptick_datawarehouse/workforce/models.py
--rw-r--r--   0        0        0      993 1970-01-01 00:00:00.000000 uptick_datawarehouse-0.2.5/setup.py
--rw-r--r--   0        0        0      415 1970-01-01 00:00:00.000000 uptick_datawarehouse-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0       24 2023-01-13 01:44:11.272938 uptick_datawarehouse-0.2.6/public_readme.md
+-rw-r--r--   0        0        0      526 2023-04-13 02:39:22.843405 uptick_datawarehouse-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      200 2023-01-13 01:48:03.658500 uptick_datawarehouse-0.2.6/uptick_datawarehouse/model_settings.py
+-rw-r--r--   0        0        0        0 2023-01-12 03:28:28.929168 uptick_datawarehouse-0.2.6/uptick_datawarehouse/subscriptionmanager/__init__.py
+-rw-r--r--   0        0        0      191 2023-01-13 01:47:26.046172 uptick_datawarehouse-0.2.6/uptick_datawarehouse/subscriptionmanager/apps.py
+-rw-r--r--   0        0        0      271 2023-01-12 03:28:28.929570 uptick_datawarehouse-0.2.6/uptick_datawarehouse/subscriptionmanager/migrations/0001_schema.py
+-rw-r--r--   0        0        0    14332 2023-01-21 02:47:03.096787 uptick_datawarehouse-0.2.6/uptick_datawarehouse/subscriptionmanager/migrations/0002_changesummary_chargesummary_paymentmethodsummary_recurringcreditsummary_revenueforecastsummary_subsc.py
+-rw-r--r--   0        0        0      699 2023-01-23 04:43:50.589352 uptick_datawarehouse-0.2.6/uptick_datawarehouse/subscriptionmanager/migrations/0003_auto_20230123_0443.py
+-rw-r--r--   0        0        0        0 2023-01-12 03:28:28.930097 uptick_datawarehouse-0.2.6/uptick_datawarehouse/subscriptionmanager/migrations/__init__.py
+-rw-r--r--   0        0        0    12040 2023-01-23 04:43:41.277818 uptick_datawarehouse-0.2.6/uptick_datawarehouse/subscriptionmanager/models.py
+-rw-r--r--   0        0        0        0 2023-01-12 03:28:28.930464 uptick_datawarehouse-0.2.6/uptick_datawarehouse/superblocks/__init__.py
+-rw-r--r--   0        0        0      175 2023-01-13 01:47:39.075510 uptick_datawarehouse-0.2.6/uptick_datawarehouse/superblocks/apps.py
+-rw-r--r--   0        0        0      263 2023-01-12 03:28:28.930815 uptick_datawarehouse-0.2.6/uptick_datawarehouse/superblocks/migrations/0001_schema.py
+-rw-r--r--   0        0        0        0 2023-01-12 03:28:28.930876 uptick_datawarehouse-0.2.6/uptick_datawarehouse/superblocks/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-12 03:28:28.932203 uptick_datawarehouse-0.2.6/uptick_datawarehouse/vitally/__init__.py
+-rw-r--r--   0        0        0      167 2023-01-13 01:47:43.709643 uptick_datawarehouse-0.2.6/uptick_datawarehouse/vitally/apps.py
+-rw-r--r--   0        0        0      259 2023-01-12 03:28:28.932792 uptick_datawarehouse-0.2.6/uptick_datawarehouse/vitally/migrations/0001_schema.py
+-rw-r--r--   0        0        0        0 2023-01-12 03:28:28.932871 uptick_datawarehouse-0.2.6/uptick_datawarehouse/vitally/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-12 03:28:28.933549 uptick_datawarehouse-0.2.6/uptick_datawarehouse/workforce/__init__.py
+-rw-r--r--   0        0        0      171 2023-01-13 01:47:49.225586 uptick_datawarehouse-0.2.6/uptick_datawarehouse/workforce/apps.py
+-rw-r--r--   0        0        0      289 2023-01-12 03:28:28.934044 uptick_datawarehouse-0.2.6/uptick_datawarehouse/workforce/migrations/0001_schema.py
+-rw-r--r--   0        0        0    10093 2023-01-21 03:00:22.637434 uptick_datawarehouse-0.2.6/uptick_datawarehouse/workforce/migrations/0002_initial.py
+-rw-r--r--   0        0        0      396 2023-02-05 23:37:37.374239 uptick_datawarehouse-0.2.6/uptick_datawarehouse/workforce/migrations/0003_serverusage_contractor_addons_used.py
+-rw-r--r--   0        0        0      945 2023-04-12 07:38:38.179175 uptick_datawarehouse-0.2.6/uptick_datawarehouse/workforce/migrations/0004_customreportsummary.py
+-rw-r--r--   0        0        0        0 2023-01-12 03:28:28.934250 uptick_datawarehouse-0.2.6/uptick_datawarehouse/workforce/migrations/__init__.py
+-rw-r--r--   0        0        0     7736 2023-04-13 02:32:18.166779 uptick_datawarehouse-0.2.6/uptick_datawarehouse/workforce/models.py
+-rw-r--r--   0        0        0      415 1970-01-01 00:00:00.000000 uptick_datawarehouse-0.2.6/PKG-INFO
```

### Comparing `uptick_datawarehouse-0.2.5/pyproject.toml` & `uptick_datawarehouse-0.2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uptick-datawarehouse"
-version = "0.2.5"
+version = "0.2.6"
 description = ""
 authors = ["william chu <william.chu@uptickhq.com>"]
 readme = "public_readme.md"
 
 packages = [{ include = "app" }, { include = "uptick_datawarehouse" }]
 exclude = ["app"]
```

### Comparing `uptick_datawarehouse-0.2.5/uptick_datawarehouse/subscriptionmanager/migrations/0002_changesummary_chargesummary_paymentmethodsummary_recurringcreditsummary_revenueforecastsummary_subsc.py` & `uptick_datawarehouse-0.2.6/uptick_datawarehouse/subscriptionmanager/migrations/0002_changesummary_chargesummary_paymentmethodsummary_recurringcreditsummary_revenueforecastsummary_subsc.py`

 * *Files identical despite different names*

### Comparing `uptick_datawarehouse-0.2.5/uptick_datawarehouse/subscriptionmanager/migrations/0003_auto_20230123_0443.py` & `uptick_datawarehouse-0.2.6/uptick_datawarehouse/subscriptionmanager/migrations/0003_auto_20230123_0443.py`

 * *Files identical despite different names*

### Comparing `uptick_datawarehouse-0.2.5/uptick_datawarehouse/subscriptionmanager/models.py` & `uptick_datawarehouse-0.2.6/uptick_datawarehouse/subscriptionmanager/models.py`

 * *Files identical despite different names*

### Comparing `uptick_datawarehouse-0.2.5/uptick_datawarehouse/workforce/migrations/0002_initial.py` & `uptick_datawarehouse-0.2.6/uptick_datawarehouse/workforce/migrations/0002_initial.py`

 * *Files identical despite different names*

### Comparing `uptick_datawarehouse-0.2.5/uptick_datawarehouse/workforce/models.py` & `uptick_datawarehouse-0.2.6/uptick_datawarehouse/workforce/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -128,14 +128,28 @@
     class Meta:
         managed = model_settings.DATAWAREHOUSE_MANAGED_MODELS
         app_label = 'workforce'
         default_permissions = ()
         db_table = 'workforce"."customer_onboarding_actions'
 
 
+class CustomReportSummary(models.Model):
+    """Custom reports are collected to support running regression tests."""
+    tenant = models.CharField(db_index=True, max_length=200)
+    last_synced = models.DateTimeField(db_index=True)
+    custom_report_pk = models.PositiveIntegerField(db_index=True)
+    query = models.TextField()
+
+    class Meta:
+        managed = model_settings.DATAWAREHOUSE_MANAGED_MODELS
+        app_label = 'workforce'
+        default_permissions = ()
+        db_table = 'workforce"."customer_custom_reports'
+
+
 class UsageMetrics(models.Model):
     tenant = models.CharField(db_index=True, max_length=200)
     count_name = models.CharField(db_index=True, max_length=200)
     stat_count = models.BigIntegerField()
     as_of = models.DateTimeField(db_index=True)
 
     class Meta:
```

