# Comparing `tmp/m-abc-anhnt-1.0.0.tar.gz` & `tmp/m-abc-anhnt-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m-abc-anhnt-1.0.0.tar", last modified: Thu Apr 13 04:27:13 2023, max compression
+gzip compressed data, was "m-abc-anhnt-1.0.1.tar", last modified: Thu Apr 13 04:38:41 2023, max compression
```

## Comparing `m-abc-anhnt-1.0.0.tar` & `m-abc-anhnt-1.0.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-13 04:27:13.042844 m-abc-anhnt-1.0.0/
--rw-rw-r--   0 mobio     (1000) mobio     (1000)     2031 2023-04-13 04:27:13.042844 m-abc-anhnt-1.0.0/PKG-INFO
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1135 2023-04-13 03:44:34.000000 m-abc-anhnt-1.0.0/README.md
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-13 04:27:13.038844 m-abc-anhnt-1.0.0/m_abac/
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-13 04:27:13.042844 m-abc-anhnt-1.0.0/m_abac/adapter/
--rw-r--r--   0 mobio     (1000) mobio     (1000)      267 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/adapter/__init__.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      435 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/adapter/adapter.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)    15511 2023-04-10 10:55:45.000000 m-abc-anhnt-1.0.0/m_abac/adapter/elasticsearch_adapter.py
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-13 04:27:13.042844 m-abc-anhnt-1.0.0/m_abac/policy/
--rw-r--r--   0 mobio     (1000) mobio     (1000)       44 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/__init__.py
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-13 04:27:13.042844 m-abc-anhnt-1.0.0/m_abac/policy/conditions/
--rw-r--r--   0 mobio     (1000) mobio     (1000)        0 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/__init__.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      662 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/base.py
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-13 04:27:13.042844 m-abc-anhnt-1.0.0/m_abac/policy/conditions/boolean/
--rw-r--r--   0 mobio     (1000) mobio     (1000)       39 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/boolean/__init__.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1127 2023-03-22 08:58:07.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/boolean/base.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1107 2023-03-22 08:58:07.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/boolean/check_bool.py
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-13 04:27:13.042844 m-abc-anhnt-1.0.0/m_abac/policy/conditions/collection/
--rw-r--r--   0 mobio     (1000) mobio     (1000)      323 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/collection/__init__.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      629 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/collection/all_in.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      654 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/collection/all_not_in.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      638 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/collection/any_in.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      664 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/collection/any_not_in.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1341 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/collection/base.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      754 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/collection/is_empty.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      602 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/collection/is_in.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      774 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/collection/is_not_empty.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      728 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/collection/is_not_in.py
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-13 04:27:13.042844 m-abc-anhnt-1.0.0/m_abac/policy/conditions/date_time/
--rw-r--r--   0 mobio     (1000) mobio     (1000)      243 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/date_time/__init__.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     2520 2023-03-28 05:00:01.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/date_time/base.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1345 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/date_time/date_eq.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1367 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/date_time/date_gt.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1389 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/date_time/date_gte.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1358 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/date_time/date_lt.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1380 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/date_time/date_lte.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1363 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/date_time/date_neq.py
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-13 04:27:13.042844 m-abc-anhnt-1.0.0/m_abac/policy/conditions/day/
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      197 2023-03-28 07:06:43.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/day/__init__.py
--rw-rw-r--   0 mobio     (1000) mobio     (1000)     1839 2023-03-28 05:06:28.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/day/base.py
--rw-rw-r--   0 mobio     (1000) mobio     (1000)     1004 2023-03-28 05:06:28.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/day/day_eq.py
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      975 2023-03-28 06:54:31.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/day/day_gt.py
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      977 2023-03-28 06:59:38.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/day/day_gte.py
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      974 2023-03-28 06:59:38.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/day/day_lt.py
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      977 2023-03-28 07:02:53.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/day/day_lte.py
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      978 2023-03-28 07:03:16.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/day/day_neq.py
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-13 04:27:13.042844 m-abc-anhnt-1.0.0/m_abac/policy/conditions/ip_address/
--rw-r--r--   0 mobio     (1000) mobio     (1000)       82 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/ip_address/__init__.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1691 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/ip_address/base.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      737 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/ip_address/in_subnet.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      746 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/ip_address/not_in_subnet.py
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-13 04:27:13.042844 m-abc-anhnt-1.0.0/m_abac/policy/conditions/numeric/
--rw-r--r--   0 mobio     (1000) mobio     (1000)      188 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/numeric/__init__.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1450 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/numeric/base.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      853 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/numeric/eq.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      871 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/numeric/gt.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      895 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/numeric/gte.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      863 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/numeric/lt.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      886 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/numeric/lte.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)      869 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/numeric/neq.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1934 2023-03-28 07:06:43.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/schema.py
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-13 04:27:13.042844 m-abc-anhnt-1.0.0/m_abac/policy/conditions/string/
--rw-r--r--   0 mobio     (1000) mobio     (1000)      307 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/string/__init__.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1497 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/string/base.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1213 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/string/contains.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1245 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/string/ends_with.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1203 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/string/equals.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1227 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/string/not_contains.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1214 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/string/not_equals.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1498 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/string/regex_match.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1264 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/conditions/string/starts_with.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     1601 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.0/m_abac/policy/exceptions.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     5812 2023-03-23 03:58:21.000000 m-abc-anhnt-1.0.0/m_abac/policy/policy.py
--rw-r--r--   0 mobio     (1000) mobio     (1000)     3259 2023-04-10 10:55:45.000000 m-abc-anhnt-1.0.0/m_abac/policy/utils.py
-drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-13 04:27:13.042844 m-abc-anhnt-1.0.0/m_abc_anhnt.egg-info/
--rw-rw-r--   0 mobio     (1000) mobio     (1000)     2031 2023-04-13 04:27:13.000000 m-abc-anhnt-1.0.0/m_abc_anhnt.egg-info/PKG-INFO
--rw-rw-r--   0 mobio     (1000) mobio     (1000)     2721 2023-04-13 04:27:13.000000 m-abc-anhnt-1.0.0/m_abc_anhnt.egg-info/SOURCES.txt
--rw-rw-r--   0 mobio     (1000) mobio     (1000)        1 2023-04-13 04:27:13.000000 m-abc-anhnt-1.0.0/m_abc_anhnt.egg-info/dependency_links.txt
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      100 2023-04-13 04:27:13.000000 m-abc-anhnt-1.0.0/m_abc_anhnt.egg-info/requires.txt
--rw-rw-r--   0 mobio     (1000) mobio     (1000)        7 2023-04-13 04:27:13.000000 m-abc-anhnt-1.0.0/m_abc_anhnt.egg-info/top_level.txt
--rw-rw-r--   0 mobio     (1000) mobio     (1000)      104 2022-12-15 03:46:40.000000 m-abc-anhnt-1.0.0/pyproject.toml
--rw-rw-r--   0 mobio     (1000) mobio     (1000)       38 2023-04-13 04:27:13.042844 m-abc-anhnt-1.0.0/setup.cfg
--rw-r--r--   0 mobio     (1000) mobio     (1000)     9699 2023-04-13 04:26:13.000000 m-abc-anhnt-1.0.0/setup.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-13 04:38:41.676147 m-abc-anhnt-1.0.1/
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)     2031 2023-04-13 04:38:41.676147 m-abc-anhnt-1.0.1/PKG-INFO
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1135 2023-04-13 03:44:34.000000 m-abc-anhnt-1.0.1/README.md
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-13 04:38:41.672147 m-abc-anhnt-1.0.1/m_abac/
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-13 04:38:41.672147 m-abc-anhnt-1.0.1/m_abac/adapter/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      267 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/adapter/__init__.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      435 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/adapter/adapter.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)    15511 2023-04-10 10:55:45.000000 m-abc-anhnt-1.0.1/m_abac/adapter/elasticsearch_adapter.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-13 04:38:41.672147 m-abc-anhnt-1.0.1/m_abac/policy/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)       44 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/__init__.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-13 04:38:41.672147 m-abc-anhnt-1.0.1/m_abac/policy/conditions/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)        0 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/__init__.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      662 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/base.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-13 04:38:41.672147 m-abc-anhnt-1.0.1/m_abac/policy/conditions/boolean/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)       39 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/boolean/__init__.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1127 2023-03-22 08:58:07.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/boolean/base.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1107 2023-03-22 08:58:07.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/boolean/check_bool.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-13 04:38:41.676147 m-abc-anhnt-1.0.1/m_abac/policy/conditions/collection/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      323 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/collection/__init__.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      629 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/collection/all_in.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      654 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/collection/all_not_in.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      638 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/collection/any_in.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      664 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/collection/any_not_in.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1341 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/collection/base.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      754 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/collection/is_empty.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      602 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/collection/is_in.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      774 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/collection/is_not_empty.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      728 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/collection/is_not_in.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-13 04:38:41.676147 m-abc-anhnt-1.0.1/m_abac/policy/conditions/date_time/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      243 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/date_time/__init__.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     2520 2023-03-28 05:00:01.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/date_time/base.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1345 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/date_time/date_eq.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1367 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/date_time/date_gt.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1389 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/date_time/date_gte.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1358 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/date_time/date_lt.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1380 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/date_time/date_lte.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1363 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/date_time/date_neq.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-13 04:38:41.676147 m-abc-anhnt-1.0.1/m_abac/policy/conditions/day/
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      197 2023-03-28 07:06:43.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/day/__init__.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)     1839 2023-03-28 05:06:28.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/day/base.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)     1004 2023-03-28 05:06:28.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/day/day_eq.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      975 2023-03-28 06:54:31.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/day/day_gt.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      977 2023-03-28 06:59:38.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/day/day_gte.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      974 2023-03-28 06:59:38.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/day/day_lt.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      977 2023-03-28 07:02:53.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/day/day_lte.py
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      978 2023-03-28 07:03:16.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/day/day_neq.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-13 04:38:41.676147 m-abc-anhnt-1.0.1/m_abac/policy/conditions/ip_address/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)       82 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/ip_address/__init__.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1691 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/ip_address/base.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      737 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/ip_address/in_subnet.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      746 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/ip_address/not_in_subnet.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-13 04:38:41.676147 m-abc-anhnt-1.0.1/m_abac/policy/conditions/numeric/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      188 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/numeric/__init__.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1450 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/numeric/base.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      853 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/numeric/eq.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      871 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/numeric/gt.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      895 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/numeric/gte.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      863 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/numeric/lt.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      886 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/numeric/lte.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      869 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/numeric/neq.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1934 2023-03-28 07:06:43.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/schema.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-13 04:38:41.676147 m-abc-anhnt-1.0.1/m_abac/policy/conditions/string/
+-rw-r--r--   0 mobio     (1000) mobio     (1000)      307 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/string/__init__.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1497 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/string/base.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1213 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/string/contains.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1245 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/string/ends_with.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1203 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/string/equals.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1227 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/string/not_contains.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1214 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/string/not_equals.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1498 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/string/regex_match.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1264 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/conditions/string/starts_with.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     1601 2023-03-21 07:52:15.000000 m-abc-anhnt-1.0.1/m_abac/policy/exceptions.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     5812 2023-03-23 03:58:21.000000 m-abc-anhnt-1.0.1/m_abac/policy/policy.py
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     3259 2023-04-10 10:55:45.000000 m-abc-anhnt-1.0.1/m_abac/policy/utils.py
+drwxrwxr-x   0 mobio     (1000) mobio     (1000)        0 2023-04-13 04:38:41.676147 m-abc-anhnt-1.0.1/m_abc_anhnt.egg-info/
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)     2031 2023-04-13 04:38:41.000000 m-abc-anhnt-1.0.1/m_abc_anhnt.egg-info/PKG-INFO
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)     2721 2023-04-13 04:38:41.000000 m-abc-anhnt-1.0.1/m_abc_anhnt.egg-info/SOURCES.txt
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)        1 2023-04-13 04:38:41.000000 m-abc-anhnt-1.0.1/m_abc_anhnt.egg-info/dependency_links.txt
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      100 2023-04-13 04:38:41.000000 m-abc-anhnt-1.0.1/m_abc_anhnt.egg-info/requires.txt
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)        7 2023-04-13 04:38:41.000000 m-abc-anhnt-1.0.1/m_abc_anhnt.egg-info/top_level.txt
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)      104 2022-12-15 03:46:40.000000 m-abc-anhnt-1.0.1/pyproject.toml
+-rw-rw-r--   0 mobio     (1000) mobio     (1000)       38 2023-04-13 04:38:41.676147 m-abc-anhnt-1.0.1/setup.cfg
+-rw-r--r--   0 mobio     (1000) mobio     (1000)     9768 2023-04-13 04:38:30.000000 m-abc-anhnt-1.0.1/setup.py
```

### Comparing `m-abc-anhnt-1.0.0/PKG-INFO` & `m-abc-anhnt-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-abc-anhnt
-Version: 1.0.0
+Version: 1.0.1
 Summary: Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Keywords: mobio,mobio-engine,m-abac
```

### Comparing `m-abc-anhnt-1.0.0/README.md` & `m-abc-anhnt-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/adapter/elasticsearch_adapter.py` & `m-abc-anhnt-1.0.1/m_abac/adapter/elasticsearch_adapter.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/base.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/base.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/boolean/base.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/boolean/base.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/boolean/check_bool.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/boolean/check_bool.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/collection/all_in.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/collection/all_in.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/collection/all_not_in.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/collection/all_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/collection/any_in.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/collection/any_in.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/collection/any_not_in.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/collection/any_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/collection/base.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/collection/base.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/collection/is_empty.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/collection/is_empty.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/collection/is_in.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/collection/is_in.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/collection/is_not_empty.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/collection/is_not_empty.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/collection/is_not_in.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/collection/is_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/date_time/base.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/date_time/base.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/date_time/date_eq.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/date_time/date_eq.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/date_time/date_gt.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/date_time/date_gt.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/date_time/date_gte.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/date_time/date_gte.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/date_time/date_lt.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/date_time/date_lt.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/date_time/date_lte.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/date_time/date_lte.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/date_time/date_neq.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/date_time/date_neq.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/day/base.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/day/base.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/day/day_eq.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/day/day_eq.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/day/day_gt.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/day/day_gt.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/day/day_gte.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/day/day_gte.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/day/day_lt.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/day/day_lt.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/day/day_lte.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/day/day_lte.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/day/day_neq.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/day/day_neq.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/ip_address/base.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/ip_address/base.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/ip_address/in_subnet.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/ip_address/in_subnet.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/ip_address/not_in_subnet.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/ip_address/not_in_subnet.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/numeric/base.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/numeric/base.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/numeric/eq.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/numeric/eq.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/numeric/gt.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/numeric/gt.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/numeric/gte.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/numeric/gte.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/numeric/lt.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/numeric/lt.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/numeric/lte.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/numeric/lte.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/numeric/neq.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/numeric/neq.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/schema.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/schema.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/string/base.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/string/base.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/string/contains.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/string/contains.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/string/ends_with.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/string/ends_with.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/string/equals.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/string/equals.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/string/not_contains.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/string/not_contains.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/string/not_equals.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/string/not_equals.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/string/regex_match.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/string/regex_match.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/conditions/string/starts_with.py` & `m-abc-anhnt-1.0.1/m_abac/policy/conditions/string/starts_with.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/exceptions.py` & `m-abc-anhnt-1.0.1/m_abac/policy/exceptions.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/policy.py` & `m-abc-anhnt-1.0.1/m_abac/policy/policy.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abac/policy/utils.py` & `m-abc-anhnt-1.0.1/m_abac/policy/utils.py`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/m_abc_anhnt.egg-info/PKG-INFO` & `m-abc-anhnt-1.0.1/m_abc_anhnt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-abc-anhnt
-Version: 1.0.0
+Version: 1.0.1
 Summary: Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Keywords: mobio,mobio-engine,m-abac
```

### Comparing `m-abc-anhnt-1.0.0/m_abc_anhnt.egg-info/SOURCES.txt` & `m-abc-anhnt-1.0.1/m_abc_anhnt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m-abc-anhnt-1.0.0/setup.py` & `m-abc-anhnt-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from setuptools import find_namespace_packages, setup
+from setuptools import find_namespace_packages, setup, find_packages
 import os
 
 
 class Readme(object):
     __readme_path = "README.md"
 
     @staticmethod
@@ -70,15 +70,15 @@
     # options={"bdist_wheel": {"universal": True}},
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.0.0',  # Required
+    version='1.0.1',  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
@@ -149,15 +149,16 @@
     #
     # Alternatively, if you just want to distribute a single Python file, use
     # the `py_modules` argument instead as follows, which will expect a file
     # called `my_module.py` to exist:
     #
     #   py_modules=["my_module"],
     #
-    packages=find_namespace_packages(include=["m_abac.*"]),  # Required
+    # packages=find_namespace_packages(include=["m_abac.*"]),  # Required
+    packages = find_packages(include=['m_abac.*']),
     # namespace_packages=["mobio"],  # Optional
     # Specify which Python versions you support. In contrast to the
     # 'Programming Language' classifiers above, 'pip install' will check this
     # and refuse to install the project if the version does not match. See
     # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
     python_requires=">=3",
     # This field lists other packages that your project depends on to run.
```

