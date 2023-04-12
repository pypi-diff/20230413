# Comparing `tmp/django_q2-1.5.1.tar.gz` & `tmp/django_q2-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_q2-1.5.1.tar", max compression
+gzip compressed data, was "django_q2-1.5.2.tar", max compression
```

## Comparing `django_q2-1.5.1.tar` & `django_q2-1.5.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0    62249 2023-04-02 15:54:08.606774 django_q2-1.5.1/CHANGELOG.md
--rw-r--r--   0        0        0     1088 2023-04-02 15:54:08.606774 django_q2-1.5.1/LICENSE
--rw-r--r--   0        0        0     7050 2023-04-02 15:54:08.606774 django_q2-1.5.1/README.rst
--rw-r--r--   0        0        0      169 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/__init__.py
--rw-r--r--   0        0        0     4547 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/admin.py
--rw-r--r--   0        0        0      289 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/apps.py
--rw-r--r--   0        0        0     5161 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/brokers/__init__.py
--rw-r--r--   0        0        0     3243 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/brokers/aws_sqs.py
--rw-r--r--   0        0        0     1404 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/brokers/ironmq.py
--rw-r--r--   0        0        0     2327 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/brokers/mongo.py
--rw-r--r--   0        0        0     2767 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/brokers/orm.py
--rw-r--r--   0        0        0     1951 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/brokers/redis_broker.py
--rw-r--r--   0        0        0    31002 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/cluster.py
--rw-r--r--   0        0        0     9270 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/conf.py
--rw-r--r--   0        0        0     2707 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/core_signing.py
--rw-r--r--   0        0        0     7253 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/humanhash.py
--rw-r--r--   0        0        0    11421 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    11403 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    11241 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/locale/tr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/management/commands/__init__.py
--rw-r--r--   0        0        0     1283 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/management/commands/qcluster.py
--rw-r--r--   0        0        0     1566 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/management/commands/qinfo.py
--rw-r--r--   0        0        0      889 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/management/commands/qmemory.py
--rw-r--r--   0        0        0      609 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/management/commands/qmonitor.py
--rw-r--r--   0        0        0     4886 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/migrations/0001_initial.py
--rw-r--r--   0        0        0      629 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/migrations/0002_auto_20150630_1624.py
--rw-r--r--   0        0        0     1213 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/migrations/0003_auto_20150708_1326.py
--rw-r--r--   0        0        0      823 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/migrations/0004_auto_20150710_1043.py
--rw-r--r--   0        0        0      524 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/migrations/0005_auto_20150718_1506.py
--rw-r--r--   0        0        0     1088 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/migrations/0006_auto_20150805_1817.py
--rw-r--r--   0        0        0      888 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/migrations/0007_ormq.py
--rw-r--r--   0        0        0      348 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/migrations/0008_auto_20160224_1026.py
--rw-r--r--   0        0        0      467 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/migrations/0009_auto_20171009_0915.py
--rw-r--r--   0        0        0      882 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/migrations/0010_auto_20200610_0856.py
--rw-r--r--   0        0        0     1113 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/migrations/0011_auto_20200628_1055.py
--rw-r--r--   0        0        0      603 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/migrations/0012_auto_20200702_1608.py
--rw-r--r--   0        0        0      389 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/migrations/0013_task_attempt_count.py
--rw-r--r--   0        0        0      426 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/migrations/0014_schedule_cluster.py
--rw-r--r--   0        0        0      958 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/migrations/0015_alter_schedule_schedule_type.py
--rw-r--r--   0        0        0      655 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/migrations/0016_schedule_intended_date_kwarg.py
--rw-r--r--   0        0        0     1211 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/migrations/0017_task_cluster_alter.py
--rw-r--r--   0        0        0        0 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/migrations/__init__.py
--rw-r--r--   0        0        0    11724 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/models.py
--rw-r--r--   0        0        0    18239 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/monitor.py
--rw-r--r--   0        0        0     2905 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/queues.py
--rw-r--r--   0        0        0     1206 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/signals.py
--rw-r--r--   0        0        0      989 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/signing.py
--rw-r--r--   0        0        0     3632 2023-04-02 15:54:08.606774 django_q2-1.5.1/django_q/status.py
--rw-r--r--   0        0        0    22128 2023-04-02 15:54:08.610774 django_q2-1.5.1/django_q/tasks.py
--rw-r--r--   0        0        0        0 2023-04-02 15:54:08.610774 django_q2-1.5.1/django_q/tests/__init__.py
--rw-r--r--   0        0        0     3101 2023-04-02 15:54:08.610774 django_q2-1.5.1/django_q/tests/settings.py
--rw-r--r--   0        0        0      712 2023-04-02 15:54:08.610774 django_q2-1.5.1/django_q/tests/tasks.py
--rw-r--r--   0        0        0     3018 2023-04-02 15:54:08.610774 django_q2-1.5.1/django_q/tests/test_admin.py
--rw-r--r--   0        0        0     8658 2023-04-02 15:54:08.610774 django_q2-1.5.1/django_q/tests/test_brokers.py
--rw-r--r--   0        0        0     6812 2023-04-02 15:54:08.610774 django_q2-1.5.1/django_q/tests/test_cached.py
--rw-r--r--   0        0        0    24279 2023-04-02 15:54:08.610774 django_q2-1.5.1/django_q/tests/test_cluster.py
--rw-r--r--   0        0        0      531 2023-04-02 15:54:08.610774 django_q2-1.5.1/django_q/tests/test_commands.py
--rw-r--r--   0        0        0     1231 2023-04-02 15:54:08.610774 django_q2-1.5.1/django_q/tests/test_monitor.py
--rw-r--r--   0        0        0    14840 2023-04-02 15:54:08.610774 django_q2-1.5.1/django_q/tests/test_scheduler.py
--rw-r--r--   0        0        0        0 2023-04-02 15:54:08.610774 django_q2-1.5.1/django_q/tests/testing_utilities/__init__.py
--rw-r--r--   0        0        0      918 2023-04-02 15:54:08.610774 django_q2-1.5.1/django_q/tests/testing_utilities/multiple_database_routers.py
--rw-r--r--   0        0        0      126 2023-04-02 15:54:08.610774 django_q2-1.5.1/django_q/tests/urls.py
--rw-r--r--   0        0        0     2369 2023-04-02 15:54:08.610774 django_q2-1.5.1/django_q/utils.py
--rw-r--r--   0        0        0     2736 2023-04-02 15:54:08.614774 django_q2-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     9555 1970-01-01 00:00:00.000000 django_q2-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0    62496 2023-04-12 23:40:17.343231 django_q2-1.5.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1088 2023-04-12 23:40:17.343231 django_q2-1.5.2/LICENSE
+-rw-r--r--   0        0        0     7073 2023-04-12 23:40:17.343231 django_q2-1.5.2/README.rst
+-rw-r--r--   0        0        0      169 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/__init__.py
+-rw-r--r--   0        0        0     4547 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/admin.py
+-rw-r--r--   0        0        0      289 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/apps.py
+-rw-r--r--   0        0        0     5161 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/brokers/__init__.py
+-rw-r--r--   0        0        0     3243 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/brokers/aws_sqs.py
+-rw-r--r--   0        0        0     1404 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/brokers/ironmq.py
+-rw-r--r--   0        0        0     2327 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/brokers/mongo.py
+-rw-r--r--   0        0        0     2767 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/brokers/orm.py
+-rw-r--r--   0        0        0     1951 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/brokers/redis_broker.py
+-rw-r--r--   0        0        0    31002 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/cluster.py
+-rw-r--r--   0        0        0     9270 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/conf.py
+-rw-r--r--   0        0        0     2711 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/core_signing.py
+-rw-r--r--   0        0        0     7253 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/humanhash.py
+-rw-r--r--   0        0        0    11421 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    11403 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    11241 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/locale/tr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/management/commands/__init__.py
+-rw-r--r--   0        0        0     1283 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/management/commands/qcluster.py
+-rw-r--r--   0        0        0     1566 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/management/commands/qinfo.py
+-rw-r--r--   0        0        0      889 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/management/commands/qmemory.py
+-rw-r--r--   0        0        0      609 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/management/commands/qmonitor.py
+-rw-r--r--   0        0        0     4886 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0001_initial.py
+-rw-r--r--   0        0        0      629 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0002_auto_20150630_1624.py
+-rw-r--r--   0        0        0     1213 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0003_auto_20150708_1326.py
+-rw-r--r--   0        0        0      823 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0004_auto_20150710_1043.py
+-rw-r--r--   0        0        0      524 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0005_auto_20150718_1506.py
+-rw-r--r--   0        0        0     1088 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0006_auto_20150805_1817.py
+-rw-r--r--   0        0        0      888 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0007_ormq.py
+-rw-r--r--   0        0        0      348 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0008_auto_20160224_1026.py
+-rw-r--r--   0        0        0      467 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0009_auto_20171009_0915.py
+-rw-r--r--   0        0        0      882 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0010_auto_20200610_0856.py
+-rw-r--r--   0        0        0     1113 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0011_auto_20200628_1055.py
+-rw-r--r--   0        0        0      603 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0012_auto_20200702_1608.py
+-rw-r--r--   0        0        0      389 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0013_task_attempt_count.py
+-rw-r--r--   0        0        0      426 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0014_schedule_cluster.py
+-rw-r--r--   0        0        0      958 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0015_alter_schedule_schedule_type.py
+-rw-r--r--   0        0        0      655 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0016_schedule_intended_date_kwarg.py
+-rw-r--r--   0        0        0     1211 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/0017_task_cluster_alter.py
+-rw-r--r--   0        0        0        0 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/migrations/__init__.py
+-rw-r--r--   0        0        0    11724 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/models.py
+-rw-r--r--   0        0        0    18239 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/monitor.py
+-rw-r--r--   0        0        0     2905 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/queues.py
+-rw-r--r--   0        0        0     1206 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/signals.py
+-rw-r--r--   0        0        0      989 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/signing.py
+-rw-r--r--   0        0        0     3632 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/status.py
+-rw-r--r--   0        0        0    22128 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/tasks.py
+-rw-r--r--   0        0        0        0 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/tests/__init__.py
+-rw-r--r--   0        0        0     3101 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/tests/settings.py
+-rw-r--r--   0        0        0      712 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/tests/tasks.py
+-rw-r--r--   0        0        0     3018 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/tests/test_admin.py
+-rw-r--r--   0        0        0     8658 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/tests/test_brokers.py
+-rw-r--r--   0        0        0     6812 2023-04-12 23:40:17.343231 django_q2-1.5.2/django_q/tests/test_cached.py
+-rw-r--r--   0        0        0    24279 2023-04-12 23:40:17.347231 django_q2-1.5.2/django_q/tests/test_cluster.py
+-rw-r--r--   0        0        0      531 2023-04-12 23:40:17.347231 django_q2-1.5.2/django_q/tests/test_commands.py
+-rw-r--r--   0        0        0     1231 2023-04-12 23:40:17.347231 django_q2-1.5.2/django_q/tests/test_monitor.py
+-rw-r--r--   0        0        0    14840 2023-04-12 23:40:17.347231 django_q2-1.5.2/django_q/tests/test_scheduler.py
+-rw-r--r--   0        0        0        0 2023-04-12 23:40:17.347231 django_q2-1.5.2/django_q/tests/testing_utilities/__init__.py
+-rw-r--r--   0        0        0      918 2023-04-12 23:40:17.347231 django_q2-1.5.2/django_q/tests/testing_utilities/multiple_database_routers.py
+-rw-r--r--   0        0        0      126 2023-04-12 23:40:17.347231 django_q2-1.5.2/django_q/tests/urls.py
+-rw-r--r--   0        0        0     2369 2023-04-12 23:40:17.347231 django_q2-1.5.2/django_q/utils.py
+-rw-r--r--   0        0        0     2736 2023-04-12 23:40:17.351232 django_q2-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     9578 1970-01-01 00:00:00.000000 django_q2-1.5.2/PKG-INFO
```

### Comparing `django_q2-1.5.1/CHANGELOG.md` & `django_q2-1.5.2/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 ## [Unreleased](https://github.com/GDay/django-q2/tree/HEAD)
 
+## [v1.5.2](https://github.com/GDay/django-q2/tree/v1.5.2) (2023-04-13)
+
+**Merged pull requests:**
+
+- Added Django 4.2 to the test matrix, fixed deprecation warning https://github.com/GDay/django-q2/pull/89
+- Updated docs to show support for 4.2
+
 ## [v1.5.1](https://github.com/GDay/django-q2/tree/v1.5.1) (2023-04-02)
 
 - Fix release to pipy due to changed org name
 
 ## [v1.5.0](https://github.com/GDay/django-q2/tree/v1.5.0) (2023-04-02)
 
 **Merged pull requests:**
```

### Comparing `django_q2-1.5.1/LICENSE` & `django_q2-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/README.rst` & `django_q2-1.5.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 Requirements
 ~~~~~~~~~~~~
 
 -  `Django <https://www.djangoproject.com>`__ > = 3.2
 -  `Django-picklefield <https://github.com/gintas/django-picklefield>`__
 
-Tested with: Python 3.8, 3.9, 3.10, 3.11 Django 3.2.X and 4.1.X
+Tested with: Python 3.8, 3.9, 3.10 and 3.11. Works with Django 3.2.X, 4.1.X and 4.2.X.
 
 Brokers
 ~~~~~~~
 - `Redis <https://django-q2.readthedocs.org/en/latest/brokers.html#redis>`__
 - `IronMQ <https://django-q2.readthedocs.org/en/latest/brokers.html#ironmq>`__
 - `Amazon SQS <https://django-q2.readthedocs.org/en/latest/brokers.html#amazon-sqs>`__
 - `MongoDB <https://django-q2.readthedocs.org/en/latest/brokers.html#mongodb>`__
```

### Comparing `django_q2-1.5.1/django_q/admin.py` & `django_q2-1.5.2/django_q/admin.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/brokers/__init__.py` & `django_q2-1.5.2/django_q/brokers/__init__.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/brokers/aws_sqs.py` & `django_q2-1.5.2/django_q/brokers/aws_sqs.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/brokers/ironmq.py` & `django_q2-1.5.2/django_q/brokers/ironmq.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/brokers/mongo.py` & `django_q2-1.5.2/django_q/brokers/mongo.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/brokers/orm.py` & `django_q2-1.5.2/django_q/brokers/orm.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/brokers/redis_broker.py` & `django_q2-1.5.2/django_q/brokers/redis_broker.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/cluster.py` & `django_q2-1.5.2/django_q/cluster.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/conf.py` & `django_q2-1.5.2/django_q/conf.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/core_signing.py` & `django_q2-1.5.2/django_q/core_signing.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     """
     Reverse of dumps(), raise BadSignature if signature fails.
 
     The serializer is expected to accept a bytestring.
     """
     # TimestampSigner.unsign() returns str but base64 and zlib compression
     # operate on bytes.
-    base64d = force_bytes(TimestampSigner(key, salt=salt).unsign(s, max_age=max_age))
+    base64d = force_bytes(TimestampSigner(key=key, salt=salt).unsign(s, max_age=max_age))
     decompress = False
     if base64d[:1] == b".":
         # It's compressed; uncompress it first
         base64d = base64d[1:]
         decompress = True
     data = b64_decode(base64d)
     if decompress:
```

### Comparing `django_q2-1.5.1/django_q/humanhash.py` & `django_q2-1.5.2/django_q/humanhash.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/locale/de/LC_MESSAGES/django.po` & `django_q2-1.5.2/django_q/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/locale/fr/LC_MESSAGES/django.po` & `django_q2-1.5.2/django_q/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/locale/tr/LC_MESSAGES/django.po` & `django_q2-1.5.2/django_q/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/management/commands/qcluster.py` & `django_q2-1.5.2/django_q/management/commands/qcluster.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/management/commands/qinfo.py` & `django_q2-1.5.2/django_q/management/commands/qinfo.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/management/commands/qmemory.py` & `django_q2-1.5.2/django_q/management/commands/qmemory.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/management/commands/qmonitor.py` & `django_q2-1.5.2/django_q/management/commands/qmonitor.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/migrations/0001_initial.py` & `django_q2-1.5.2/django_q/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/migrations/0002_auto_20150630_1624.py` & `django_q2-1.5.2/django_q/migrations/0002_auto_20150630_1624.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/migrations/0003_auto_20150708_1326.py` & `django_q2-1.5.2/django_q/migrations/0003_auto_20150708_1326.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/migrations/0004_auto_20150710_1043.py` & `django_q2-1.5.2/django_q/migrations/0004_auto_20150710_1043.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/migrations/0005_auto_20150718_1506.py` & `django_q2-1.5.2/django_q/migrations/0005_auto_20150718_1506.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/migrations/0006_auto_20150805_1817.py` & `django_q2-1.5.2/django_q/migrations/0006_auto_20150805_1817.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/migrations/0007_ormq.py` & `django_q2-1.5.2/django_q/migrations/0007_ormq.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/migrations/0010_auto_20200610_0856.py` & `django_q2-1.5.2/django_q/migrations/0010_auto_20200610_0856.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/migrations/0011_auto_20200628_1055.py` & `django_q2-1.5.2/django_q/migrations/0011_auto_20200628_1055.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/migrations/0012_auto_20200702_1608.py` & `django_q2-1.5.2/django_q/migrations/0012_auto_20200702_1608.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/migrations/0015_alter_schedule_schedule_type.py` & `django_q2-1.5.2/django_q/migrations/0015_alter_schedule_schedule_type.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/migrations/0016_schedule_intended_date_kwarg.py` & `django_q2-1.5.2/django_q/migrations/0016_schedule_intended_date_kwarg.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/migrations/0017_task_cluster_alter.py` & `django_q2-1.5.2/django_q/migrations/0017_task_cluster_alter.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/models.py` & `django_q2-1.5.2/django_q/models.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/monitor.py` & `django_q2-1.5.2/django_q/monitor.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/queues.py` & `django_q2-1.5.2/django_q/queues.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/signals.py` & `django_q2-1.5.2/django_q/signals.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/signing.py` & `django_q2-1.5.2/django_q/signing.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/status.py` & `django_q2-1.5.2/django_q/status.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/tasks.py` & `django_q2-1.5.2/django_q/tasks.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/tests/settings.py` & `django_q2-1.5.2/django_q/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/tests/tasks.py` & `django_q2-1.5.2/django_q/tests/tasks.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/tests/test_admin.py` & `django_q2-1.5.2/django_q/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/tests/test_brokers.py` & `django_q2-1.5.2/django_q/tests/test_brokers.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/tests/test_cached.py` & `django_q2-1.5.2/django_q/tests/test_cached.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/tests/test_cluster.py` & `django_q2-1.5.2/django_q/tests/test_cluster.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/tests/test_commands.py` & `django_q2-1.5.2/django_q/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/tests/test_monitor.py` & `django_q2-1.5.2/django_q/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/tests/test_scheduler.py` & `django_q2-1.5.2/django_q/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/tests/testing_utilities/multiple_database_routers.py` & `django_q2-1.5.2/django_q/tests/testing_utilities/multiple_database_routers.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/django_q/utils.py` & `django_q2-1.5.2/django_q/utils.py`

 * *Files identical despite different names*

### Comparing `django_q2-1.5.1/pyproject.toml` & `django_q2-1.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-q2"
-version = "1.5.1"
+version = "1.5.2"
 packages = [
     { include = "django_q" },
 ]
 description = "A multiprocessing distributed task queue for Django"
 authors = ["Stan Triepels <django-q2@stantriepels.com>", "Ilan Steemers <koed00@gmail.com>"]
 maintainers = ["Stan Triepels <django-q2@stantriepels.com>"]
 license = "MIT"
```

### Comparing `django_q2-1.5.1/PKG-INFO` & `django_q2-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-q2
-Version: 1.5.1
+Version: 1.5.2
 Summary: A multiprocessing distributed task queue for Django
 Home-page: https://django-q2.readthedocs.org
 License: MIT
 Keywords: django,distributed,multiprocessing,queue,scheduler
 Author: Stan Triepels
 Author-email: django-q2@stantriepels.com
 Maintainer: Stan Triepels
@@ -92,15 +92,15 @@
 
 Requirements
 ~~~~~~~~~~~~
 
 -  `Django <https://www.djangoproject.com>`__ > = 3.2
 -  `Django-picklefield <https://github.com/gintas/django-picklefield>`__
 
-Tested with: Python 3.8, 3.9, 3.10, 3.11 Django 3.2.X and 4.1.X
+Tested with: Python 3.8, 3.9, 3.10 and 3.11. Works with Django 3.2.X, 4.1.X and 4.2.X.
 
 Brokers
 ~~~~~~~
 - `Redis <https://django-q2.readthedocs.org/en/latest/brokers.html#redis>`__
 - `IronMQ <https://django-q2.readthedocs.org/en/latest/brokers.html#ironmq>`__
 - `Amazon SQS <https://django-q2.readthedocs.org/en/latest/brokers.html#amazon-sqs>`__
 - `MongoDB <https://django-q2.readthedocs.org/en/latest/brokers.html#mongodb>`__
```

