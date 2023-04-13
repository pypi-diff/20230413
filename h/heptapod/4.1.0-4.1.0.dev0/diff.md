# Comparing `tmp/heptapod-4.1.0.tar.gz` & `tmp/heptapod-4.1.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heptapod-4.1.0.tar", last modified: Thu Apr 13 17:17:31 2023, max compression
+gzip compressed data, was "heptapod-4.1.0.dev0.tar", last modified: Fri Mar 31 21:30:01 2023, max compression
```

## Comparing `heptapod-4.1.0.tar` & `heptapod-4.1.0.dev0.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-04-13 17:17:31.714311 heptapod-4.1.0/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    18092 2023-04-12 09:47:23.000000 heptapod-4.1.0/LICENSE
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       33 2023-04-12 09:47:23.000000 heptapod-4.1.0/MANIFEST.in
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3832 2023-04-13 17:17:31.714311 heptapod-4.1.0/PKG-INFO
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3145 2023-04-12 09:47:23.000000 heptapod-4.1.0/README.md
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-04-13 17:17:31.709311 heptapod-4.1.0/heptapod/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        6 2023-04-13 17:16:52.000000 heptapod-4.1.0/heptapod/VERSION
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      403 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/__init__.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-04-13 17:17:31.709311 heptapod-4.1.0/heptapod/gitlab/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/gitlab/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7113 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/gitlab/branch.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2447 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/gitlab/change.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    15489 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/gitlab/hooks.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3979 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/gitlab/prune_reasons.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      940 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/gitlab/tag.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-04-13 17:17:31.710311 heptapod-4.1.0/heptapod/gitlab/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/gitlab/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1214 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/gitlab/tests/test_change.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4275 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/gitlab/tests/test_hooks_inner.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    15612 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/gitlab/tests/test_hooks_integration.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      672 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/heptapod.example.hgrc
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-04-13 17:17:31.710311 heptapod-4.1.0/heptapod/hooks/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/hooks/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       77 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/hooks/check_publish.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      927 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/hooks/dev_util.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      661 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/hooks/gitlab_mirror.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6758 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/hooks/perm.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      722 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/hooks/subrepos.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-04-13 17:17:31.711311 heptapod-4.1.0/heptapod/hooks/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/hooks/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2760 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/hooks/tests/test_check_publish.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2098 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/hooks/tests/test_check_write.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1228 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/hooks/tests/test_dev_utils.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      962 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/hooks/tests/test_gitlab_mirror.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      548 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/hooks/tests/utils.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1156 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/obsutil.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1365 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/patch.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2209 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/required.hgrc
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-04-13 17:17:31.711311 heptapod-4.1.0/heptapod/testhelpers/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      475 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/testhelpers/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3730 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/testhelpers/git.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4960 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/testhelpers/gitlab.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3090 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/testhelpers/hg.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-04-13 17:17:31.711311 heptapod-4.1.0/heptapod/testhelpers/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/testhelpers/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1760 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/testhelpers/tests/test_git.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      799 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/testhelpers/tests/test_gitlab.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2700 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/testhelpers/tests/test_repo_wrapper.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-04-13 17:17:31.712311 heptapod-4.1.0/heptapod/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      456 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/tests/test_harness.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      597 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/tests/test_package.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1201 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/tests/test_patch.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1062 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/tests/test_util.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5965 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/tests/test_wsgi.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2356 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/tests/test_wsgi_webtest.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1072 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/util.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    10310 2023-04-12 09:47:23.000000 heptapod-4.1.0/heptapod/wsgi.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-04-13 17:17:31.709311 heptapod-4.1.0/heptapod.egg-info/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3832 2023-04-13 17:17:31.000000 heptapod-4.1.0/heptapod.egg-info/PKG-INFO
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2804 2023-04-13 17:17:31.000000 heptapod-4.1.0/heptapod.egg-info/SOURCES.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        1 2023-04-13 17:17:31.000000 heptapod-4.1.0/heptapod.egg-info/dependency_links.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      168 2023-04-13 17:17:31.000000 heptapod-4.1.0/heptapod.egg-info/requires.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       18 2023-04-13 17:17:31.000000 heptapod-4.1.0/heptapod.egg-info/top_level.txt
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-04-13 17:17:31.712311 heptapod-4.1.0/hgext3rd/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      157 2023-04-12 09:47:23.000000 heptapod-4.1.0/hgext3rd/__init__.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-04-13 17:17:31.712311 heptapod-4.1.0/hgext3rd/heptapod/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17105 2023-04-12 09:47:23.000000 heptapod-4.1.0/hgext3rd/heptapod/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2582 2023-04-12 09:47:23.000000 heptapod-4.1.0/hgext3rd/heptapod/branch.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9096 2023-04-12 09:47:23.000000 heptapod-4.1.0/hgext3rd/heptapod/git.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4163 2023-04-12 09:47:23.000000 heptapod-4.1.0/hgext3rd/heptapod/keep_around.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4177 2023-04-12 09:47:23.000000 heptapod-4.1.0/hgext3rd/heptapod/no_git.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5068 2023-04-12 09:47:23.000000 heptapod-4.1.0/hgext3rd/heptapod/special_ref.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    48933 2023-04-12 09:47:23.000000 heptapod-4.1.0/hgext3rd/heptapod/state_maintainer.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1305 2023-04-12 09:47:23.000000 heptapod-4.1.0/hgext3rd/heptapod/tag.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-04-13 17:17:31.713311 heptapod-4.1.0/hgext3rd/heptapod/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2023-04-12 09:47:23.000000 heptapod-4.1.0/hgext3rd/heptapod/tests/__init__.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-04-13 17:17:31.714311 heptapod-4.1.0/hgext3rd/heptapod/tests/git/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      126 2023-04-12 09:47:23.000000 heptapod-4.1.0/hgext3rd/heptapod/tests/git/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17184 2023-04-12 09:47:23.000000 heptapod-4.1.0/hgext3rd/heptapod/tests/git/test_inner.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      935 2023-04-12 09:47:23.000000 heptapod-4.1.0/hgext3rd/heptapod/tests/git/test_inner_subrepos.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    57377 2023-04-12 09:47:23.000000 heptapod-4.1.0/hgext3rd/heptapod/tests/git/test_integration.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-04-13 17:17:31.714311 heptapod-4.1.0/hgext3rd/heptapod/tests/no_git/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2023-04-12 09:47:23.000000 heptapod-4.1.0/hgext3rd/heptapod/tests/no_git/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2012 2023-04-12 09:47:23.000000 heptapod-4.1.0/hgext3rd/heptapod/tests/no_git/test_inner.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    43109 2023-04-12 09:47:23.000000 heptapod-4.1.0/hgext3rd/heptapod/tests/no_git/test_integration.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3955 2023-04-12 09:47:23.000000 heptapod-4.1.0/hgext3rd/heptapod/tests/test_backups.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     8265 2023-04-12 09:47:23.000000 heptapod-4.1.0/hgext3rd/heptapod/tests/test_commands_misc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3778 2023-04-12 09:47:23.000000 heptapod-4.1.0/hgext3rd/heptapod/tests/test_config.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1287 2023-04-12 09:47:23.000000 heptapod-4.1.0/hgext3rd/heptapod/tests/test_default_branch.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2489 2023-04-12 09:47:23.000000 heptapod-4.1.0/hgext3rd/heptapod/tests/test_exchange.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      735 2023-04-12 09:47:23.000000 heptapod-4.1.0/hgext3rd/heptapod/tests/test_initial_import_mode.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1870 2023-04-12 09:47:23.000000 heptapod-4.1.0/hgext3rd/heptapod/tests/test_keep_arounds.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1221 2023-04-12 09:47:23.000000 heptapod-4.1.0/hgext3rd/heptapod/tests/test_patch_runsystem.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6714 2023-04-12 09:47:23.000000 heptapod-4.1.0/hgext3rd/heptapod/tests/test_pull_force_topic.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3160 2023-04-12 09:47:23.000000 heptapod-4.1.0/hgext3rd/heptapod/tests/test_special_ref.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3606 2023-04-12 09:47:23.000000 heptapod-4.1.0/hgext3rd/heptapod/tests/test_typed_refs.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      910 2023-04-12 09:47:23.000000 heptapod-4.1.0/hgext3rd/heptapod/tests/utils.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3093 2023-04-12 09:47:23.000000 heptapod-4.1.0/hgext3rd/heptapod/topic.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6697 2023-04-12 09:47:23.000000 heptapod-4.1.0/hgext3rd/heptapod/typed_ref.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      168 2023-04-12 09:47:23.000000 heptapod-4.1.0/install-requirements.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       38 2023-04-13 17:17:31.714311 heptapod-4.1.0/setup.cfg
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1144 2023-04-12 09:47:23.000000 heptapod-4.1.0/setup.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-03-31 21:30:01.582936 heptapod-4.1.0.dev0/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    18092 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/LICENSE
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       33 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/MANIFEST.in
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3837 2023-03-31 21:30:01.582936 heptapod-4.1.0.dev0/PKG-INFO
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3145 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/README.md
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-03-31 21:30:01.577936 heptapod-4.1.0.dev0/heptapod/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       10 2023-03-31 19:21:11.000000 heptapod-4.1.0.dev0/heptapod/VERSION
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      403 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/__init__.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-03-31 21:30:01.578936 heptapod-4.1.0.dev0/heptapod/gitlab/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/gitlab/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7113 2023-03-31 19:21:11.000000 heptapod-4.1.0.dev0/heptapod/gitlab/branch.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2447 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/gitlab/change.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    15101 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/gitlab/hooks.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3979 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/gitlab/prune_reasons.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      940 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/gitlab/tag.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-03-31 21:30:01.578936 heptapod-4.1.0.dev0/heptapod/gitlab/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/gitlab/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1214 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/gitlab/tests/test_change.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4275 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/gitlab/tests/test_hooks_inner.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    15612 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/gitlab/tests/test_hooks_integration.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      672 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/heptapod.example.hgrc
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-03-31 21:30:01.579936 heptapod-4.1.0.dev0/heptapod/hooks/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/hooks/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       77 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/hooks/check_publish.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      927 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/hooks/dev_util.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      661 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/hooks/gitlab_mirror.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6758 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/hooks/perm.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      722 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/hooks/subrepos.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-03-31 21:30:01.579936 heptapod-4.1.0.dev0/heptapod/hooks/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/hooks/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2760 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/hooks/tests/test_check_publish.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2098 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/hooks/tests/test_check_write.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1228 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/hooks/tests/test_dev_utils.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      962 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/hooks/tests/test_gitlab_mirror.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      548 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/hooks/tests/utils.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1156 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/obsutil.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1365 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/patch.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2209 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/required.hgrc
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-03-31 21:30:01.579936 heptapod-4.1.0.dev0/heptapod/testhelpers/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      475 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/testhelpers/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3730 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/testhelpers/git.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4960 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/testhelpers/gitlab.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3090 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/testhelpers/hg.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-03-31 21:30:01.579936 heptapod-4.1.0.dev0/heptapod/testhelpers/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/testhelpers/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1760 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/testhelpers/tests/test_git.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      799 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/testhelpers/tests/test_gitlab.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2700 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/testhelpers/tests/test_repo_wrapper.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-03-31 21:30:01.580936 heptapod-4.1.0.dev0/heptapod/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      456 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/tests/test_harness.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      597 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/tests/test_package.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1201 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/tests/test_patch.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1062 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/tests/test_util.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5965 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/tests/test_wsgi.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2356 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/tests/test_wsgi_webtest.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1072 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/util.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    10310 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/heptapod/wsgi.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-03-31 21:30:01.577936 heptapod-4.1.0.dev0/heptapod.egg-info/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3837 2023-03-31 21:30:01.000000 heptapod-4.1.0.dev0/heptapod.egg-info/PKG-INFO
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2804 2023-03-31 21:30:01.000000 heptapod-4.1.0.dev0/heptapod.egg-info/SOURCES.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        1 2023-03-31 21:30:01.000000 heptapod-4.1.0.dev0/heptapod.egg-info/dependency_links.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      150 2023-03-31 21:30:01.000000 heptapod-4.1.0.dev0/heptapod.egg-info/requires.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       18 2023-03-31 21:30:01.000000 heptapod-4.1.0.dev0/heptapod.egg-info/top_level.txt
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-03-31 21:30:01.580936 heptapod-4.1.0.dev0/hgext3rd/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      157 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/hgext3rd/__init__.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-03-31 21:30:01.581936 heptapod-4.1.0.dev0/hgext3rd/heptapod/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    16759 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/hgext3rd/heptapod/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2582 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/hgext3rd/heptapod/branch.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9096 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/hgext3rd/heptapod/git.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4163 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/hgext3rd/heptapod/keep_around.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4177 2023-03-31 19:21:11.000000 heptapod-4.1.0.dev0/hgext3rd/heptapod/no_git.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5068 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/hgext3rd/heptapod/special_ref.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    48933 2023-03-31 19:26:08.000000 heptapod-4.1.0.dev0/hgext3rd/heptapod/state_maintainer.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1305 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/hgext3rd/heptapod/tag.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-03-31 21:30:01.582936 heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/__init__.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-03-31 21:30:01.582936 heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/git/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      126 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/git/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17184 2023-03-31 19:45:37.000000 heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/git/test_inner.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      935 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/git/test_inner_subrepos.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    57377 2023-03-31 19:22:02.000000 heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/git/test_integration.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2023-03-31 21:30:01.582936 heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/no_git/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/no_git/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2012 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/no_git/test_inner.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    43109 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/no_git/test_integration.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3955 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/test_backups.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     8265 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/test_commands_misc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3778 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/test_config.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1287 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/test_default_branch.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2489 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/test_exchange.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      735 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/test_initial_import_mode.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1870 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/test_keep_arounds.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1221 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/test_patch_runsystem.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6714 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/test_pull_force_topic.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3160 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/test_special_ref.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3606 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/test_typed_refs.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      910 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/utils.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3093 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/hgext3rd/heptapod/topic.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6697 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/hgext3rd/heptapod/typed_ref.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      150 2023-03-31 19:49:07.000000 heptapod-4.1.0.dev0/install-requirements.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       38 2023-03-31 21:30:01.582936 heptapod-4.1.0.dev0/setup.cfg
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1144 2023-03-26 20:03:39.000000 heptapod-4.1.0.dev0/setup.py
```

### Comparing `heptapod-4.1.0/LICENSE` & `heptapod-4.1.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/PKG-INFO` & `heptapod-4.1.0.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heptapod
-Version: 4.1.0
+Version: 4.1.0.dev0
 Summary: Heptapod server-side Mercurial hooks, extension, etc.
 Home-page: https://foss.heptapod.net/heptapod/py-heptapod
 Author: Georges Racinet
 Author-email: georges.racinet@octobus.net
 License: GPLv2+
 Keywords: hg mercurial heptapod gitlab
 Platform: UNKNOWN
```

### Comparing `heptapod-4.1.0/README.md` & `heptapod-4.1.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/gitlab/branch.py` & `heptapod-4.1.0.dev0/heptapod/gitlab/branch.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/gitlab/change.py` & `heptapod-4.1.0.dev0/heptapod/gitlab/change.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/gitlab/hooks.py` & `heptapod-4.1.0.dev0/heptapod/gitlab/hooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 # Copyright 2019-2020 Georges Racinet <georges.racinet@octobus.net>
 #
 # This software may be used and distributed according to the terms of the
 # GNU General Public License version 2 or any later version.
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 from base64 import b64encode
-import datetime
 import json
 import logging
 from mercurial import (
     hg,
     pycompat,
 )
 import os
 import re
 import requests
 from requests.exceptions import RequestException
 import requests_unixsocket
 
-import jwcrypto.jwk as jwk
-import python_jwt as jwt
-
-
 logger = logging.getLogger(__name__)
 
 ACTOR_RX_SYMBS = (
     (re.compile(r'key-(\d+)$'), 'key_id'),
     (re.compile(r'user-(\d+)$'), 'user_id'),
     (re.compile(r'username-(.*)$'), 'username'),
 )
@@ -259,26 +254,20 @@
 
     def gitlab_internal_api_request(
             self, meth,
             subpath, params, **kwargs):  # pragma: no cover
         logger.debug("Sending %s to %r, params=%r",
                      meth, subpath, params)
         params['secret_token'] = self.gitlab_secret
-        payload = dict(iss='gitlab-shell')
-        key = jwk.JWK.from_password(self.gitlab_secret)
-        jwt_token = jwt.generate_jwt(payload, key, 'HS256',
-                                     datetime.timedelta(minutes=1))
-        headers = {'Gitlab-Shell-Api-Request': jwt_token}
         with requests_unixsocket.monkeypatch():
             return requests.request(
                 meth,
                 '/'.join((self.gitlab_internal_api_endpoint,
                           subpath)),
                 data=params,
-                headers=headers,
                 **kwargs)
 
     def __call__(self, changes):
         """Call GitLab Hook for the given changes.
 
         :return: numeric return code, output and error.
```

### Comparing `heptapod-4.1.0/heptapod/gitlab/prune_reasons.py` & `heptapod-4.1.0.dev0/heptapod/gitlab/prune_reasons.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/gitlab/tag.py` & `heptapod-4.1.0.dev0/heptapod/gitlab/tag.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/gitlab/tests/test_change.py` & `heptapod-4.1.0.dev0/heptapod/gitlab/tests/test_change.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/gitlab/tests/test_hooks_inner.py` & `heptapod-4.1.0.dev0/heptapod/gitlab/tests/test_hooks_inner.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/gitlab/tests/test_hooks_integration.py` & `heptapod-4.1.0.dev0/heptapod/gitlab/tests/test_hooks_integration.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/heptapod.example.hgrc` & `heptapod-4.1.0.dev0/heptapod/heptapod.example.hgrc`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/hooks/dev_util.py` & `heptapod-4.1.0.dev0/heptapod/hooks/dev_util.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/hooks/gitlab_mirror.py` & `heptapod-4.1.0.dev0/heptapod/hooks/gitlab_mirror.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/hooks/perm.py` & `heptapod-4.1.0.dev0/heptapod/hooks/perm.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/hooks/subrepos.py` & `heptapod-4.1.0.dev0/heptapod/hooks/subrepos.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/hooks/tests/test_check_publish.py` & `heptapod-4.1.0.dev0/heptapod/hooks/tests/test_check_publish.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/hooks/tests/test_check_write.py` & `heptapod-4.1.0.dev0/heptapod/hooks/tests/test_check_write.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/hooks/tests/test_dev_utils.py` & `heptapod-4.1.0.dev0/heptapod/hooks/tests/test_dev_utils.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/hooks/tests/test_gitlab_mirror.py` & `heptapod-4.1.0.dev0/heptapod/hooks/tests/test_gitlab_mirror.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/hooks/tests/utils.py` & `heptapod-4.1.0.dev0/heptapod/hooks/tests/utils.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/obsutil.py` & `heptapod-4.1.0.dev0/heptapod/obsutil.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/patch.py` & `heptapod-4.1.0.dev0/heptapod/patch.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/required.hgrc` & `heptapod-4.1.0.dev0/heptapod/required.hgrc`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/testhelpers/git.py` & `heptapod-4.1.0.dev0/heptapod/testhelpers/git.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/testhelpers/gitlab.py` & `heptapod-4.1.0.dev0/heptapod/testhelpers/gitlab.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/testhelpers/hg.py` & `heptapod-4.1.0.dev0/heptapod/testhelpers/hg.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/testhelpers/tests/test_git.py` & `heptapod-4.1.0.dev0/heptapod/testhelpers/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/testhelpers/tests/test_gitlab.py` & `heptapod-4.1.0.dev0/heptapod/testhelpers/tests/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/testhelpers/tests/test_repo_wrapper.py` & `heptapod-4.1.0.dev0/heptapod/testhelpers/tests/test_repo_wrapper.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/tests/test_package.py` & `heptapod-4.1.0.dev0/heptapod/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/tests/test_patch.py` & `heptapod-4.1.0.dev0/heptapod/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/tests/test_util.py` & `heptapod-4.1.0.dev0/heptapod/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/tests/test_wsgi.py` & `heptapod-4.1.0.dev0/heptapod/tests/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/tests/test_wsgi_webtest.py` & `heptapod-4.1.0.dev0/heptapod/tests/test_wsgi_webtest.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/util.py` & `heptapod-4.1.0.dev0/heptapod/util.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod/wsgi.py` & `heptapod-4.1.0.dev0/heptapod/wsgi.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/heptapod.egg-info/PKG-INFO` & `heptapod-4.1.0.dev0/heptapod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heptapod
-Version: 4.1.0
+Version: 4.1.0.dev0
 Summary: Heptapod server-side Mercurial hooks, extension, etc.
 Home-page: https://foss.heptapod.net/heptapod/py-heptapod
 Author: Georges Racinet
 Author-email: georges.racinet@octobus.net
 License: GPLv2+
 Keywords: hg mercurial heptapod gitlab
 Platform: UNKNOWN
```

### Comparing `heptapod-4.1.0/heptapod.egg-info/SOURCES.txt` & `heptapod-4.1.0.dev0/heptapod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/hgext3rd/heptapod/__init__.py` & `heptapod-4.1.0.dev0/hgext3rd/heptapod/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,26 +37,18 @@
 from . import (
     topic as topicmod,
     git,
     no_git,
 )
 from .branch import DEFAULT_GITLAB_BRANCH_FILE_NAME
 
+
 # these have conditional imports and subsequent `None` testing in
 # (urllib3 and/or requests). In other words, hgdemandimport breaks `requests`
-demandimport.IGNORES.update([
-    'brotli',
-    'simplejson',
-    # used in JWT token generation. With `demandimport`, we get errors such as
-    #  ValueError: module object for
-    #  'cryptography.hazmat.primitives.asymmetric.types' substituted
-    #  in sys.modules during a lazy load
-    'cryptography.hazmat.primitives.asymmetric.types',
-    'cryptography.hazmat.primitives.ciphers.algorithms',
-])
+demandimport.IGNORES.update([b'brotli', b'simplejson'])
 
 try:
     from hgext3rd import hggit
     # forcing demandimport to import it
     hggit.__doc__  # pragma no cover
 except ImportError:  # pragma no cover (fallback for hg-git < 0.11)
     try:
```

### Comparing `heptapod-4.1.0/hgext3rd/heptapod/branch.py` & `heptapod-4.1.0.dev0/hgext3rd/heptapod/branch.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/hgext3rd/heptapod/git.py` & `heptapod-4.1.0.dev0/hgext3rd/heptapod/git.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/hgext3rd/heptapod/keep_around.py` & `heptapod-4.1.0.dev0/hgext3rd/heptapod/keep_around.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/hgext3rd/heptapod/no_git.py` & `heptapod-4.1.0.dev0/hgext3rd/heptapod/no_git.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/hgext3rd/heptapod/special_ref.py` & `heptapod-4.1.0.dev0/hgext3rd/heptapod/special_ref.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/hgext3rd/heptapod/state_maintainer.py` & `heptapod-4.1.0.dev0/hgext3rd/heptapod/state_maintainer.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/hgext3rd/heptapod/tag.py` & `heptapod-4.1.0.dev0/hgext3rd/heptapod/tag.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/hgext3rd/heptapod/tests/git/test_inner.py` & `heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/git/test_inner.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/hgext3rd/heptapod/tests/git/test_inner_subrepos.py` & `heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/git/test_inner_subrepos.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/hgext3rd/heptapod/tests/git/test_integration.py` & `heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/git/test_integration.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/hgext3rd/heptapod/tests/no_git/test_inner.py` & `heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/no_git/test_inner.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/hgext3rd/heptapod/tests/no_git/test_integration.py` & `heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/no_git/test_integration.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/hgext3rd/heptapod/tests/test_backups.py` & `heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/test_backups.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/hgext3rd/heptapod/tests/test_commands_misc.py` & `heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/test_commands_misc.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/hgext3rd/heptapod/tests/test_config.py` & `heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/hgext3rd/heptapod/tests/test_default_branch.py` & `heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/test_default_branch.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/hgext3rd/heptapod/tests/test_exchange.py` & `heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/test_exchange.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/hgext3rd/heptapod/tests/test_initial_import_mode.py` & `heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/test_initial_import_mode.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/hgext3rd/heptapod/tests/test_keep_arounds.py` & `heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/test_keep_arounds.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/hgext3rd/heptapod/tests/test_patch_runsystem.py` & `heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/test_patch_runsystem.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/hgext3rd/heptapod/tests/test_pull_force_topic.py` & `heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/test_pull_force_topic.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/hgext3rd/heptapod/tests/test_special_ref.py` & `heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/test_special_ref.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/hgext3rd/heptapod/tests/test_typed_refs.py` & `heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/test_typed_refs.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/hgext3rd/heptapod/tests/utils.py` & `heptapod-4.1.0.dev0/hgext3rd/heptapod/tests/utils.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/hgext3rd/heptapod/topic.py` & `heptapod-4.1.0.dev0/hgext3rd/heptapod/topic.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/hgext3rd/heptapod/typed_ref.py` & `heptapod-4.1.0.dev0/hgext3rd/heptapod/typed_ref.py`

 * *Files identical despite different names*

### Comparing `heptapod-4.1.0/setup.py` & `heptapod-4.1.0.dev0/setup.py`

 * *Files identical despite different names*

