# Comparing `tmp/asana-3.2.0.tar.gz` & `tmp/asana-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/python-asana/python-asana/dist/.tmp-0_z0c5oy/asana-3.2.0.tar", last modified: Fri Mar 24 17:25:31 2023, max compression
+gzip compressed data, was "/home/runner/work/python-asana/python-asana/dist/.tmp-tepx3kjb/asana-3.2.1.tar", last modified: Thu Apr 13 16:54:49 2023, max compression
```

## Comparing `asana-3.2.0.tar` & `asana-3.2.1.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:25:31.000000 asana-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 17:25:20.000000 asana-3.2.0/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 17:25:20.000000 asana-3.2.0/CONTRIBUTORS
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-03-24 17:25:20.000000 asana-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-24 17:25:20.000000 asana-3.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-03-24 17:25:31.000000 asana-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-03-24 17:25:20.000000 asana-3.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:25:31.000000 asana-3.2.0/asana/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-24 17:25:20.000000 asana-3.2.0/asana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-03-24 17:25:20.000000 asana-3.2.0/asana/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-03-24 17:25:20.000000 asana-3.2.0/asana/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-03-24 17:25:20.000000 asana-3.2.0/asana/page_iterator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:25:31.000000 asana-3.2.0/asana/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/audit_log_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/batch_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/custom_field_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:25:31.000000 asana-3.2.0/asana/resources/gen/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/audit_log_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/batch_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/custom_field_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    12487 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/goal_relationships.py
--rw-r--r--   0 runner    (1001) docker     (123)    14536 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/goals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/organization_exports.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/portfolio_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)    16355 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/project_briefs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/project_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/project_statuses.py
--rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/project_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    27462 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/status_updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/stories.py
--rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    43387 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/team_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/teams.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/time_periods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/typeahead.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/user_task_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/workspace_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/gen/workspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/goal_relationships.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/goals.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/organization_exports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/portfolio_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/project_briefs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/project_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/project_statuses.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/project_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/sections.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/status_updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/stories.py
--rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    20218 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/team_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/teams.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/time_periods.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/typeahead.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/user_task_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/workspace_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-03-24 17:25:20.000000 asana-3.2.0/asana/resources/workspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-24 17:25:20.000000 asana-3.2.0/asana/session.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-24 17:25:20.000000 asana-3.2.0/asana/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:25:31.000000 asana-3.2.0/asana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-03-24 17:25:31.000000 asana-3.2.0/asana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-03-24 17:25:31.000000 asana-3.2.0/asana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 17:25:31.000000 asana-3.2.0/asana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-24 17:25:31.000000 asana-3.2.0/asana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-24 17:25:31.000000 asana-3.2.0/asana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 17:25:31.000000 asana-3.2.0/asana.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-24 17:25:31.000000 asana-3.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1321 2023-03-24 17:25:20.000000 asana-3.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 17:25:31.000000 asana-3.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18990 2023-03-24 17:25:20.000000 asana-3.2.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-03-24 17:25:20.000000 asana-3.2.0/tests/test_client_attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-03-24 17:25:20.000000 asana-3.2.0/tests/test_client_audit_log_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-03-24 17:25:20.000000 asana-3.2.0/tests/test_client_custom_field_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-03-24 17:25:20.000000 asana-3.2.0/tests/test_client_custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-03-24 17:25:20.000000 asana-3.2.0/tests/test_client_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-24 17:25:20.000000 asana-3.2.0/tests/test_client_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-03-24 17:25:20.000000 asana-3.2.0/tests/test_client_organization_exports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-03-24 17:25:20.000000 asana-3.2.0/tests/test_client_portfolio_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-03-24 17:25:20.000000 asana-3.2.0/tests/test_client_portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-03-24 17:25:20.000000 asana-3.2.0/tests/test_client_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-03-24 17:25:20.000000 asana-3.2.0/tests/test_client_sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-03-24 17:25:20.000000 asana-3.2.0/tests/test_client_stories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-03-24 17:25:20.000000 asana-3.2.0/tests/test_client_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-03-24 17:25:20.000000 asana-3.2.0/tests/test_client_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-24 17:25:20.000000 asana-3.2.0/tests/test_client_teams.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-03-24 17:25:20.000000 asana-3.2.0/tests/test_client_user_task_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-03-24 17:25:20.000000 asana-3.2.0/tests/test_client_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-03-24 17:25:20.000000 asana-3.2.0/tests/test_client_webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-03-24 17:25:20.000000 asana-3.2.0/tests/test_client_workspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-03-24 17:25:20.000000 asana-3.2.0/tests/test_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:54:49.000000 asana-3.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 16:54:39.000000 asana-3.2.1/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 16:54:39.000000 asana-3.2.1/CONTRIBUTORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-13 16:54:39.000000 asana-3.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 16:54:39.000000 asana-3.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-04-13 16:54:49.000000 asana-3.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-04-13 16:54:39.000000 asana-3.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:54:49.000000 asana-3.2.1/asana/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-13 16:54:39.000000 asana-3.2.1/asana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14070 2023-04-13 16:54:39.000000 asana-3.2.1/asana/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-13 16:54:39.000000 asana-3.2.1/asana/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-04-13 16:54:39.000000 asana-3.2.1/asana/page_iterator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:54:49.000000 asana-3.2.1/asana/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/audit_log_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/batch_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/custom_field_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:54:49.000000 asana-3.2.1/asana/resources/gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/audit_log_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/batch_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/custom_field_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12487 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/goal_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14536 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/goals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/organization_exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/portfolio_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16355 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/portfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/project_briefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/project_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/project_statuses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/project_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27462 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/status_updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/stories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43387 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/team_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/time_periods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/typeahead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/user_task_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/workspace_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/gen/workspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/goal_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/goals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/organization_exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/portfolio_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/portfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/project_briefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/project_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/project_statuses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/project_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/status_updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/stories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20218 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/team_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/time_periods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/typeahead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/user_task_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/workspace_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-04-13 16:54:39.000000 asana-3.2.1/asana/resources/workspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-13 16:54:39.000000 asana-3.2.1/asana/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 16:54:39.000000 asana-3.2.1/asana/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:54:49.000000 asana-3.2.1/asana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-04-13 16:54:49.000000 asana-3.2.1/asana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-04-13 16:54:49.000000 asana-3.2.1/asana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 16:54:49.000000 asana-3.2.1/asana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-13 16:54:49.000000 asana-3.2.1/asana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 16:54:49.000000 asana-3.2.1/asana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 16:54:49.000000 asana-3.2.1/asana.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-13 16:54:49.000000 asana-3.2.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1321 2023-04-13 16:54:39.000000 asana-3.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:54:49.000000 asana-3.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18990 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_audit_log_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_custom_field_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_organization_exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_portfolio_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_portfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_stories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_user_task_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_client_workspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-13 16:54:39.000000 asana-3.2.1/tests/test_errors.py
```

### Comparing `asana-3.2.0/LICENSE` & `asana-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/PKG-INFO` & `asana-3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asana
-Version: 3.2.0
+Version: 3.2.1
 Summary: Asana API client
 Home-page: http://github.com/asana/python-asana
 Author: Asana, Inc
 License: MIT
 Keywords: asana
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `asana-3.2.0/README.md` & `asana-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/client.py` & `asana-3.2.1/asana/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,16 +77,20 @@
         options = self._merge_options(options)
         url = options['base_url'] + path
         retry_count = 0
         request_options = self._parse_request_options(options)
         self._add_version_header(request_options)
         while True:
             try:
-                response = getattr(self.session, method)(
-                    url, auth=self.auth, **request_options)
+                try:
+                    response = getattr(self.session, method)(
+                        url, auth=self.auth, **request_options)
+                except requests.exceptions.Timeout:
+                    raise error.RetryableAsanaError()
+
                 self._log_asana_change_header(request_options['headers'], response.headers)
                 if response.status_code in STATUS_MAP:
                     raise STATUS_MAP[response.status_code](response)
                 elif 500 <= response.status_code < 600:
                     # Any unhandled 500 is a server error.
                     raise error.ServerError(response)
                 else:
```

### Comparing `asana-3.2.0/asana/error.py` & `asana-3.2.1/asana/error.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/page_iterator.py` & `asana-3.2.1/asana/page_iterator.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/__init__.py` & `asana-3.2.1/asana/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/attachments.py` & `asana-3.2.1/asana/resources/attachments.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/audit_log_api.py` & `asana-3.2.1/asana/resources/audit_log_api.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/custom_field_settings.py` & `asana-3.2.1/asana/resources/custom_field_settings.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/custom_fields.py` & `asana-3.2.1/asana/resources/custom_fields.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/events.py` & `asana-3.2.1/asana/resources/events.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/__init__.py` & `asana-3.2.1/asana/resources/gen/__init__.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/attachments.py` & `asana-3.2.1/asana/resources/gen/attachments.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/audit_log_api.py` & `asana-3.2.1/asana/resources/gen/audit_log_api.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/batch_api.py` & `asana-3.2.1/asana/resources/gen/batch_api.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/custom_field_settings.py` & `asana-3.2.1/asana/resources/gen/custom_field_settings.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/custom_fields.py` & `asana-3.2.1/asana/resources/gen/custom_fields.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/events.py` & `asana-3.2.1/asana/resources/gen/events.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/goal_relationships.py` & `asana-3.2.1/asana/resources/gen/goal_relationships.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/goals.py` & `asana-3.2.1/asana/resources/gen/goals.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/jobs.py` & `asana-3.2.1/asana/resources/gen/jobs.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/memberships.py` & `asana-3.2.1/asana/resources/gen/memberships.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/message.py` & `asana-3.2.1/asana/resources/gen/message.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/organization_exports.py` & `asana-3.2.1/asana/resources/gen/organization_exports.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/portfolio_memberships.py` & `asana-3.2.1/asana/resources/gen/portfolio_memberships.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/portfolios.py` & `asana-3.2.1/asana/resources/gen/portfolios.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/project_briefs.py` & `asana-3.2.1/asana/resources/gen/project_briefs.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/project_memberships.py` & `asana-3.2.1/asana/resources/gen/project_memberships.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/project_statuses.py` & `asana-3.2.1/asana/resources/gen/project_statuses.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/project_templates.py` & `asana-3.2.1/asana/resources/gen/project_templates.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/projects.py` & `asana-3.2.1/asana/resources/gen/projects.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/sections.py` & `asana-3.2.1/asana/resources/gen/sections.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/status_updates.py` & `asana-3.2.1/asana/resources/gen/status_updates.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/stories.py` & `asana-3.2.1/asana/resources/gen/stories.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/tags.py` & `asana-3.2.1/asana/resources/gen/tags.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/tasks.py` & `asana-3.2.1/asana/resources/gen/tasks.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/team_memberships.py` & `asana-3.2.1/asana/resources/gen/team_memberships.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/teams.py` & `asana-3.2.1/asana/resources/gen/teams.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/time_periods.py` & `asana-3.2.1/asana/resources/gen/time_periods.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/typeahead.py` & `asana-3.2.1/asana/resources/gen/typeahead.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/user_task_lists.py` & `asana-3.2.1/asana/resources/gen/user_task_lists.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/users.py` & `asana-3.2.1/asana/resources/gen/users.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/webhooks.py` & `asana-3.2.1/asana/resources/gen/webhooks.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/workspace_memberships.py` & `asana-3.2.1/asana/resources/gen/workspace_memberships.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/gen/workspaces.py` & `asana-3.2.1/asana/resources/gen/workspaces.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/organization_exports.py` & `asana-3.2.1/asana/resources/organization_exports.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/portfolio_memberships.py` & `asana-3.2.1/asana/resources/portfolio_memberships.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/portfolios.py` & `asana-3.2.1/asana/resources/portfolios.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/project_memberships.py` & `asana-3.2.1/asana/resources/project_memberships.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/project_statuses.py` & `asana-3.2.1/asana/resources/project_statuses.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/projects.py` & `asana-3.2.1/asana/resources/projects.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/sections.py` & `asana-3.2.1/asana/resources/sections.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/stories.py` & `asana-3.2.1/asana/resources/stories.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/tags.py` & `asana-3.2.1/asana/resources/tags.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/tasks.py` & `asana-3.2.1/asana/resources/tasks.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/teams.py` & `asana-3.2.1/asana/resources/teams.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/user_task_lists.py` & `asana-3.2.1/asana/resources/user_task_lists.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/users.py` & `asana-3.2.1/asana/resources/users.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/webhooks.py` & `asana-3.2.1/asana/resources/webhooks.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/resources/workspaces.py` & `asana-3.2.1/asana/resources/workspaces.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana/session.py` & `asana-3.2.1/asana/session.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/asana.egg-info/PKG-INFO` & `asana-3.2.1/asana.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asana
-Version: 3.2.0
+Version: 3.2.1
 Summary: Asana API client
 Home-page: http://github.com/asana/python-asana
 Author: Asana, Inc
 License: MIT
 Keywords: asana
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `asana-3.2.0/asana.egg-info/SOURCES.txt` & `asana-3.2.1/asana.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/setup.py` & `asana-3.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/tests/test_client.py` & `asana-3.2.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/tests/test_client_attachments.py` & `asana-3.2.1/tests/test_client_attachments.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/tests/test_client_audit_log_api.py` & `asana-3.2.1/tests/test_client_audit_log_api.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/tests/test_client_custom_field_settings.py` & `asana-3.2.1/tests/test_client_custom_field_settings.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/tests/test_client_custom_fields.py` & `asana-3.2.1/tests/test_client_custom_fields.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/tests/test_client_events.py` & `asana-3.2.1/tests/test_client_events.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/tests/test_client_organization_exports.py` & `asana-3.2.1/tests/test_client_organization_exports.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/tests/test_client_portfolio_memberships.py` & `asana-3.2.1/tests/test_client_portfolio_memberships.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/tests/test_client_portfolios.py` & `asana-3.2.1/tests/test_client_portfolios.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/tests/test_client_projects.py` & `asana-3.2.1/tests/test_client_projects.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/tests/test_client_sections.py` & `asana-3.2.1/tests/test_client_sections.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/tests/test_client_stories.py` & `asana-3.2.1/tests/test_client_stories.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/tests/test_client_tags.py` & `asana-3.2.1/tests/test_client_tags.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/tests/test_client_tasks.py` & `asana-3.2.1/tests/test_client_tasks.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/tests/test_client_user_task_lists.py` & `asana-3.2.1/tests/test_client_user_task_lists.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/tests/test_client_users.py` & `asana-3.2.1/tests/test_client_users.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/tests/test_client_webhooks.py` & `asana-3.2.1/tests/test_client_webhooks.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/tests/test_client_workspaces.py` & `asana-3.2.1/tests/test_client_workspaces.py`

 * *Files identical despite different names*

### Comparing `asana-3.2.0/tests/test_errors.py` & `asana-3.2.1/tests/test_errors.py`

 * *Files identical despite different names*

