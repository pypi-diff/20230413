# Comparing `tmp/statefun-tasks-0.9.91.tar.gz` & `tmp/statefun-tasks-0.9.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statefun-tasks-0.9.91.tar", last modified: Mon Apr 10 17:02:11 2023, max compression
+gzip compressed data, was "statefun-tasks-0.9.92.tar", last modified: Thu Apr 13 15:26:02 2023, max compression
```

## Comparing `statefun-tasks-0.9.91.tar` & `statefun-tasks-0.9.92.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-10 17:02:11.090440 statefun-tasks-0.9.91/
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)    11357 2022-11-27 19:05:40.000000 statefun-tasks-0.9.91/LICENSE
--rw-rw-r--   0 kingfra   (1000) kingfra   (1000)     1386 2023-04-10 17:02:11.086439 statefun-tasks-0.9.91/PKG-INFO
--rw-rw-r--   0 kingfra   (1000) kingfra   (1000)      869 2023-04-10 17:01:43.000000 statefun-tasks-0.9.91/README.md
--rw-rw-r--   0 kingfra   (1000) kingfra   (1000)       38 2023-04-10 17:02:11.090440 statefun-tasks-0.9.91/setup.cfg
--rw-rw-r--   0 kingfra   (1000) kingfra   (1000)      944 2023-04-10 17:01:43.000000 statefun-tasks-0.9.91/setup.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-10 17:02:10.738443 statefun-tasks-0.9.91/statefun_tasks/
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)      924 2023-04-10 16:51:35.000000 statefun-tasks-0.9.91/statefun_tasks/__init__.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      585 2022-11-27 19:05:40.000000 statefun-tasks-0.9.91/statefun_tasks/builtin.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1004 2022-11-27 19:05:40.000000 statefun-tasks-0.9.91/statefun_tasks/builtin_tasks.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-10 17:02:10.798442 statefun-tasks-0.9.91/statefun_tasks/client/
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)      151 2022-11-27 19:05:40.000000 statefun-tasks-0.9.91/statefun_tasks/client/__init__.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)    17395 2022-11-27 19:05:40.000000 statefun-tasks-0.9.91/statefun_tasks/client/tasks_client.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)      864 2022-11-27 19:05:40.000000 statefun-tasks-0.9.91/statefun_tasks/client/types.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)    10552 2022-11-27 19:05:40.000000 statefun-tasks-0.9.91/statefun_tasks/context.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-10 17:02:10.822442 statefun-tasks-0.9.91/statefun_tasks/effects/
--rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)       84 2023-04-10 17:01:43.000000 statefun-tasks-0.9.91/statefun_tasks/effects/__init__.py
--rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)      339 2023-04-10 17:01:43.000000 statefun-tasks-0.9.91/statefun_tasks/effects/effect.py
--rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)      370 2023-04-10 17:01:43.000000 statefun-tasks-0.9.91/statefun_tasks/effects/pause_pipeline_effect.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-10 17:02:10.838442 statefun-tasks-0.9.91/statefun_tasks/events/
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)       43 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/events/__init__.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     6622 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/events/event_handlers.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-10 17:02:10.846442 statefun-tasks-0.9.91/statefun_tasks/extensions/
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)        0 2022-11-27 19:05:40.000000 statefun-tasks-0.9.91/statefun_tasks/extensions/__init__.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-10 17:02:10.866442 statefun-tasks-0.9.91/statefun_tasks/extensions/inline_tasks/
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)       65 2022-11-27 19:05:40.000000 statefun-tasks-0.9.91/statefun_tasks/extensions/inline_tasks/__init__.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     5248 2022-11-27 19:05:40.000000 statefun-tasks-0.9.91/statefun_tasks/extensions/inline_tasks/inline_tasks_impl.py
--rw-rw-r--   0 kingfra   (1000) kingfra   (1000)   115734 2023-04-10 17:01:43.000000 statefun-tasks-0.9.91/statefun_tasks/messages_pb2.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)     9212 2022-11-27 19:05:40.000000 statefun-tasks-0.9.91/statefun_tasks/pipeline.py
--rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)    17896 2023-03-03 19:15:45.000000 statefun-tasks-0.9.91/statefun_tasks/pipeline_builder.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-10 17:02:10.878441 statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)        0 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/__init__.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-10 17:02:10.942441 statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/handlers/
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      298 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/handlers/__init__.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     6795 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/handlers/begin_pipeline_handler.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1926 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/handlers/cancel_pipeline_handler.py
--rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)     6799 2023-04-10 17:01:43.000000 statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/handlers/continue_pipeline_handler.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     2969 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/handlers/end_pipeline_handler.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1658 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/handlers/pipeline_message_handler.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-10 17:02:11.006440 statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/helpers/
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      186 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/helpers/__init__.py
--rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)    11000 2023-03-03 19:15:45.000000 statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/helpers/pipeline_graph.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     6410 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/helpers/result_aggregator.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1995 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/helpers/result_emitter.py
--rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)    12023 2022-11-29 16:51:28.000000 statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/helpers/task_submitter.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)     7003 2022-11-27 19:05:40.000000 statefun-tasks-0.9.91/statefun_tasks/protobuf.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)     9345 2022-11-27 19:05:40.000000 statefun-tasks-0.9.91/statefun_tasks/serialisation.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)    16385 2023-04-10 12:06:04.000000 statefun-tasks-0.9.91/statefun_tasks/task_builder.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-10 17:02:11.022440 statefun-tasks-0.9.91/statefun_tasks/task_impl/
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)        0 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/task_impl/__init__.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-10 17:02:11.082440 statefun-tasks-0.9.91/statefun_tasks/task_impl/handlers/
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      265 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/task_impl/handlers/__init__.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      858 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/task_impl/handlers/child_pipeline_handler.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      537 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/task_impl/handlers/message_handler.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     3983 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/task_impl/handlers/task_action_handler.py
--rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)     4382 2023-04-10 17:01:43.000000 statefun-tasks-0.9.91/statefun_tasks/task_impl/handlers/task_request_handler.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1134 2022-11-27 19:05:41.000000 statefun-tasks-0.9.91/statefun_tasks/task_impl/handlers/task_response_handler.py
--rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)     7655 2023-04-10 17:01:43.000000 statefun-tasks-0.9.91/statefun_tasks/tasks.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     2483 2022-11-27 19:05:40.000000 statefun-tasks-0.9.91/statefun_tasks/type_helpers.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)    11331 2022-11-27 19:05:40.000000 statefun-tasks-0.9.91/statefun_tasks/types.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)     1793 2022-11-27 19:05:40.000000 statefun-tasks-0.9.91/statefun_tasks/utils.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-10 17:02:10.770442 statefun-tasks-0.9.91/statefun_tasks.egg-info/
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)     1386 2023-04-10 17:02:10.000000 statefun-tasks-0.9.91/statefun_tasks.egg-info/PKG-INFO
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)     2111 2023-04-10 17:02:10.000000 statefun-tasks-0.9.91/statefun_tasks.egg-info/SOURCES.txt
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)        1 2023-04-10 17:02:10.000000 statefun-tasks-0.9.91/statefun_tasks.egg-info/dependency_links.txt
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)       42 2023-04-10 17:02:10.000000 statefun-tasks-0.9.91/statefun_tasks.egg-info/requires.txt
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)       15 2023-04-10 17:02:10.000000 statefun-tasks-0.9.91/statefun_tasks.egg-info/top_level.txt
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-13 15:26:02.923625 statefun-tasks-0.9.92/
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)    11357 2022-11-27 19:05:40.000000 statefun-tasks-0.9.92/LICENSE
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)     1386 2023-04-13 15:26:02.919625 statefun-tasks-0.9.92/PKG-INFO
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)      869 2023-04-10 17:01:43.000000 statefun-tasks-0.9.92/README.md
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)       38 2023-04-13 15:26:02.923625 statefun-tasks-0.9.92/setup.cfg
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)      944 2023-04-13 15:25:59.000000 statefun-tasks-0.9.92/setup.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-13 15:26:02.779627 statefun-tasks-0.9.92/statefun_tasks/
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)      934 2023-04-13 15:25:59.000000 statefun-tasks-0.9.92/statefun_tasks/__init__.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      585 2022-11-27 19:05:40.000000 statefun-tasks-0.9.92/statefun_tasks/builtin.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1004 2022-11-27 19:05:40.000000 statefun-tasks-0.9.92/statefun_tasks/builtin_tasks.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-13 15:26:02.807626 statefun-tasks-0.9.92/statefun_tasks/client/
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)      151 2022-11-27 19:05:40.000000 statefun-tasks-0.9.92/statefun_tasks/client/__init__.py
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)    17395 2022-11-27 19:05:40.000000 statefun-tasks-0.9.92/statefun_tasks/client/tasks_client.py
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)      864 2022-11-27 19:05:40.000000 statefun-tasks-0.9.92/statefun_tasks/client/types.py
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)    10552 2022-11-27 19:05:40.000000 statefun-tasks-0.9.92/statefun_tasks/context.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-13 15:26:02.819626 statefun-tasks-0.9.92/statefun_tasks/effects/
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)       84 2023-04-10 17:01:43.000000 statefun-tasks-0.9.92/statefun_tasks/effects/__init__.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)      339 2023-04-10 17:01:43.000000 statefun-tasks-0.9.92/statefun_tasks/effects/effect.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)      370 2023-04-10 17:01:43.000000 statefun-tasks-0.9.92/statefun_tasks/effects/pause_pipeline_effect.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-13 15:26:02.831626 statefun-tasks-0.9.92/statefun_tasks/events/
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)       43 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/events/__init__.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     6622 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/events/event_handlers.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-13 15:26:02.839626 statefun-tasks-0.9.92/statefun_tasks/extensions/
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)        0 2022-11-27 19:05:40.000000 statefun-tasks-0.9.92/statefun_tasks/extensions/__init__.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-13 15:26:02.847626 statefun-tasks-0.9.92/statefun_tasks/extensions/inline_tasks/
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)       65 2022-11-27 19:05:40.000000 statefun-tasks-0.9.92/statefun_tasks/extensions/inline_tasks/__init__.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)     5596 2023-04-13 15:25:59.000000 statefun-tasks-0.9.92/statefun_tasks/extensions/inline_tasks/inline_tasks_impl.py
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)   115734 2023-04-10 17:01:43.000000 statefun-tasks-0.9.92/statefun_tasks/messages_pb2.py
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)     9212 2022-11-27 19:05:40.000000 statefun-tasks-0.9.92/statefun_tasks/pipeline.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)    17896 2023-03-03 19:15:45.000000 statefun-tasks-0.9.92/statefun_tasks/pipeline_builder.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-13 15:26:02.851626 statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)        0 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/__init__.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-13 15:26:02.871626 statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/handlers/
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      298 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/handlers/__init__.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     6795 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/handlers/begin_pipeline_handler.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1926 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/handlers/cancel_pipeline_handler.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)     6799 2023-04-10 17:01:43.000000 statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/handlers/continue_pipeline_handler.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     2969 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/handlers/end_pipeline_handler.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1658 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/handlers/pipeline_message_handler.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-13 15:26:02.891626 statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/helpers/
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      186 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/helpers/__init__.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)    11000 2023-03-03 19:15:45.000000 statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/helpers/pipeline_graph.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     6410 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/helpers/result_aggregator.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1995 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/helpers/result_emitter.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)    12023 2022-11-29 16:51:28.000000 statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/helpers/task_submitter.py
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)     7003 2022-11-27 19:05:40.000000 statefun-tasks-0.9.92/statefun_tasks/protobuf.py
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)     9345 2022-11-27 19:05:40.000000 statefun-tasks-0.9.92/statefun_tasks/serialisation.py
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)    16385 2023-04-10 12:06:04.000000 statefun-tasks-0.9.92/statefun_tasks/task_builder.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-13 15:26:02.895626 statefun-tasks-0.9.92/statefun_tasks/task_impl/
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)        0 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/task_impl/__init__.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-13 15:26:02.919625 statefun-tasks-0.9.92/statefun_tasks/task_impl/handlers/
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      265 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/task_impl/handlers/__init__.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      858 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/task_impl/handlers/child_pipeline_handler.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      537 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/task_impl/handlers/message_handler.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     3983 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/task_impl/handlers/task_action_handler.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)     4382 2023-04-10 17:01:43.000000 statefun-tasks-0.9.92/statefun_tasks/task_impl/handlers/task_request_handler.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1134 2022-11-27 19:05:41.000000 statefun-tasks-0.9.92/statefun_tasks/task_impl/handlers/task_response_handler.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)     7655 2023-04-10 17:01:43.000000 statefun-tasks-0.9.92/statefun_tasks/tasks.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     2483 2022-11-27 19:05:40.000000 statefun-tasks-0.9.92/statefun_tasks/type_helpers.py
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)    11331 2022-11-27 19:05:40.000000 statefun-tasks-0.9.92/statefun_tasks/types.py
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)     1793 2022-11-27 19:05:40.000000 statefun-tasks-0.9.92/statefun_tasks/utils.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-04-13 15:26:02.799626 statefun-tasks-0.9.92/statefun_tasks.egg-info/
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)     1386 2023-04-13 15:26:02.000000 statefun-tasks-0.9.92/statefun_tasks.egg-info/PKG-INFO
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)     2111 2023-04-13 15:26:02.000000 statefun-tasks-0.9.92/statefun_tasks.egg-info/SOURCES.txt
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)        1 2023-04-13 15:26:02.000000 statefun-tasks-0.9.92/statefun_tasks.egg-info/dependency_links.txt
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)       42 2023-04-13 15:26:02.000000 statefun-tasks-0.9.92/statefun_tasks.egg-info/requires.txt
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)       15 2023-04-13 15:26:02.000000 statefun-tasks-0.9.92/statefun_tasks.egg-info/top_level.txt
```

### Comparing `statefun-tasks-0.9.91/LICENSE` & `statefun-tasks-0.9.92/LICENSE`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.91/PKG-INFO` & `statefun-tasks-0.9.92/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statefun-tasks
-Version: 0.9.91
+Version: 0.9.92
 Summary: Tasks API for Stateful Functions on Flink
 Home-page: https://fransking.github.io/flink-statefun-tasks
 Author: Frans King & Luke Ashworth
 Author-email: frans.king@sbbsystems.com
 License: https://www.apache.org/licenses/LICENSE-2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `statefun-tasks-0.9.91/README.md` & `statefun-tasks-0.9.92/README.md`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.91/setup.py` & `statefun-tasks-0.9.92/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 install_requires = [
     'apache-flink-statefun>=3.2.0',
     'kafka-python'
 ]
 
 setuptools.setup(
     name="statefun-tasks",
-    version="0.9.91",
+    version="0.9.92",
     author="Frans King & Luke Ashworth",
     author_email="frans.king@sbbsystems.com",
     description="Tasks API for Stateful Functions on Flink",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://fransking.github.io/flink-statefun-tasks",
     packages=['statefun_tasks'] + [f'statefun_tasks.{package}' for package in setuptools.find_packages('statefun_tasks')],
```

### Comparing `statefun-tasks-0.9.91/statefun_tasks/__init__.py` & `statefun-tasks-0.9.92/statefun_tasks/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,8 +20,8 @@
     PipelineInProgress, YieldTaskInvocation, MessageSizeExceeded
     
 from statefun_tasks.type_helpers import flink_value_type_for, add_flink_value_type_for
 
 
 # protobuf message types
 from statefun_tasks.messages_pb2 import TaskRequest, TaskResult, TaskException, TaskActionRequest, TaskActionResult, \
-    TaskActionException, TaskAction, TaskStatus, TaskDeferral, PausedTask, ChildPipeline, Address, TaskInfo, DeferredTask
+    TaskActionException, TaskAction, TaskStatus, TaskDeferral, PausedTask, Pipeline, ChildPipeline, Address, TaskInfo, DeferredTask
```

### Comparing `statefun-tasks-0.9.91/statefun_tasks/builtin.py` & `statefun-tasks-0.9.92/statefun_tasks/builtin.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.91/statefun_tasks/builtin_tasks.py` & `statefun-tasks-0.9.92/statefun_tasks/builtin_tasks.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.91/statefun_tasks/client/tasks_client.py` & `statefun-tasks-0.9.92/statefun_tasks/client/tasks_client.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.91/statefun_tasks/client/types.py` & `statefun-tasks-0.9.92/statefun_tasks/client/types.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.91/statefun_tasks/context.py` & `statefun-tasks-0.9.92/statefun_tasks/context.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.91/statefun_tasks/events/event_handlers.py` & `statefun-tasks-0.9.92/statefun_tasks/events/event_handlers.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.91/statefun_tasks/extensions/inline_tasks/inline_tasks_impl.py` & `statefun-tasks-0.9.92/statefun_tasks/extensions/inline_tasks/inline_tasks_impl.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,27 +33,36 @@
         if __with_state:
             fn_args.append(state)
 
         fn_args.extend(args)
 
         safer_locals = {'fn': fn, 'args': fn_args, 'kwargs': kwargs}
 
-        # sample restrictions on loaded code
-        # ----------------------------------
-        #
-        # safer_builtins = {**fn.__globals__['__builtins__']}
-        # fn.__globals__['__builtins__'] = safer_builtins
-        # del safer_builtins['exit']
+        # sample restrictions on loaded code to prevent accidents but not malicious behaviour
+        # don't accept pickled code from untrusted sources
+        safer_builtins = {**fn.__builtins__} if hasattr(fn, '__builtins__') else {**fn.__globals__['__builtins__']}  # Python >= 3.10 uses fn.__builtins__
+
+        if 'exit' in safer_builtins:
+            del safer_builtins['exit']
+
+        if 'quit' in safer_builtins:
+            del safer_builtins['quit']
 
         # safer_open = open
         # def safer_open(file, *sargs, **skwargs):
-        #     # you might check and raise error if file not in valid list of files for example...
-        #     open(file, *sargs, **skwargs)
+        #     raise OSError("Not allowed")
         # safer_builtins['open'] = safer_open
 
+        if hasattr(fn, '__builtins__'):
+            # Python >= 3.10
+            fn.__builtins__.clear()
+            fn.__builtins__.update(**safer_builtins)
+        else:
+            fn.__globals__['__builtins__'] = safer_builtins
+
         exec('__res = fn(*args, **kwargs)', {}, safer_locals)
         res = safer_locals['__res']
 
         if asyncio.iscoroutinefunction(fn):
             res = await res
 
         if __with_state:
```

### Comparing `statefun-tasks-0.9.91/statefun_tasks/messages_pb2.py` & `statefun-tasks-0.9.92/statefun_tasks/messages_pb2.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.91/statefun_tasks/pipeline.py` & `statefun-tasks-0.9.92/statefun_tasks/pipeline.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.91/statefun_tasks/pipeline_builder.py` & `statefun-tasks-0.9.92/statefun_tasks/pipeline_builder.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/handlers/begin_pipeline_handler.py` & `statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/handlers/begin_pipeline_handler.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/handlers/cancel_pipeline_handler.py` & `statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/handlers/cancel_pipeline_handler.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/handlers/continue_pipeline_handler.py` & `statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/handlers/continue_pipeline_handler.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/handlers/end_pipeline_handler.py` & `statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/handlers/end_pipeline_handler.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/handlers/pipeline_message_handler.py` & `statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/handlers/pipeline_message_handler.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/helpers/pipeline_graph.py` & `statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/helpers/pipeline_graph.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/helpers/result_aggregator.py` & `statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/helpers/result_aggregator.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/helpers/result_emitter.py` & `statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/helpers/result_emitter.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.91/statefun_tasks/pipeline_impl/helpers/task_submitter.py` & `statefun-tasks-0.9.92/statefun_tasks/pipeline_impl/helpers/task_submitter.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.91/statefun_tasks/protobuf.py` & `statefun-tasks-0.9.92/statefun_tasks/protobuf.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.91/statefun_tasks/serialisation.py` & `statefun-tasks-0.9.92/statefun_tasks/serialisation.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.91/statefun_tasks/task_builder.py` & `statefun-tasks-0.9.92/statefun_tasks/task_builder.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.91/statefun_tasks/task_impl/handlers/child_pipeline_handler.py` & `statefun-tasks-0.9.92/statefun_tasks/task_impl/handlers/child_pipeline_handler.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.91/statefun_tasks/task_impl/handlers/message_handler.py` & `statefun-tasks-0.9.92/statefun_tasks/task_impl/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.91/statefun_tasks/task_impl/handlers/task_action_handler.py` & `statefun-tasks-0.9.92/statefun_tasks/task_impl/handlers/task_action_handler.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.91/statefun_tasks/task_impl/handlers/task_request_handler.py` & `statefun-tasks-0.9.92/statefun_tasks/task_impl/handlers/task_request_handler.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.91/statefun_tasks/task_impl/handlers/task_response_handler.py` & `statefun-tasks-0.9.92/statefun_tasks/task_impl/handlers/task_response_handler.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.91/statefun_tasks/tasks.py` & `statefun-tasks-0.9.92/statefun_tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.91/statefun_tasks/type_helpers.py` & `statefun-tasks-0.9.92/statefun_tasks/type_helpers.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.91/statefun_tasks/types.py` & `statefun-tasks-0.9.92/statefun_tasks/types.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.91/statefun_tasks/utils.py` & `statefun-tasks-0.9.92/statefun_tasks/utils.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.91/statefun_tasks.egg-info/PKG-INFO` & `statefun-tasks-0.9.92/statefun_tasks.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statefun-tasks
-Version: 0.9.91
+Version: 0.9.92
 Summary: Tasks API for Stateful Functions on Flink
 Home-page: https://fransking.github.io/flink-statefun-tasks
 Author: Frans King & Luke Ashworth
 Author-email: frans.king@sbbsystems.com
 License: https://www.apache.org/licenses/LICENSE-2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `statefun-tasks-0.9.91/statefun_tasks.egg-info/SOURCES.txt` & `statefun-tasks-0.9.92/statefun_tasks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

