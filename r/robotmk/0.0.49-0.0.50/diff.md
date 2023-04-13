# Comparing `tmp/robotmk-0.0.49.tar.gz` & `tmp/robotmk-0.0.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotmk-0.0.49.tar", last modified: Wed Apr 12 16:13:10 2023, max compression
+gzip compressed data, was "robotmk-0.0.50.tar", last modified: Thu Apr 13 05:37:59 2023, max compression
```

## Comparing `robotmk-0.0.49.tar` & `robotmk-0.0.50.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0      110 2023-04-12 16:12:46.194371 robotmk-0.0.49/.bumpversion.cfg
--rw-r--r--   0        0        0      284 2023-04-04 11:07:18.122518 robotmk-0.0.49/.cli.env
--rw-r--r--   0        0        0       40 2023-02-24 13:10:55.692823 robotmk-0.0.49/README.md
--rw-r--r--   0        0        0      739 2023-04-12 16:12:36.358474 robotmk-0.0.49/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-28 07:41:38.789867 robotmk-0.0.49/src/_confitree/__init__.py
--rw-r--r--   0        0        0     5092 2023-03-02 13:49:11.086894 robotmk-0.0.49/src/_confitree/confitree.py
--rw-r--r--   0        0        0      512 2023-03-04 11:44:09.697687 robotmk-0.0.49/src/_confitree/robotmk.yml
--rwxr-xr-x   0        0        0      635 2023-02-24 13:10:55.692823 robotmk-0.0.49/src/_robotmk/__init__.py
--rwxr-xr-x   0        0        0      533 2023-02-24 13:10:55.692823 robotmk-0.0.49/src/_robotmk/__main__.py
--rwxr-xr-x   0        0        0     2249 2023-03-03 09:34:49.997849 robotmk-0.0.49/src/_robotmk/cli.py
--rwxr-xr-x   0        0        0      754 2023-02-24 13:10:55.696823 robotmk-0.0.49/src/_robotmk/modes/__init__.py
--rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.49/src/_robotmk/modes/agent/__init__.py
--rwxr-xr-x   0        0        0    11155 2023-02-24 13:10:55.696823 robotmk-0.0.49/src/_robotmk/modes/agent/agent.py
--rwxr-xr-x   0        0        0     1152 2023-02-24 13:10:55.696823 robotmk-0.0.49/src/_robotmk/modes/agent/cli.py
--rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.49/src/_robotmk/modes/output/__init__.py
--rwxr-xr-x   0        0        0      100 2023-02-24 13:10:55.696823 robotmk-0.0.49/src/_robotmk/modes/output/cli.py
--rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.49/src/_robotmk/modes/robot/__init__.py
--rwxr-xr-x   0        0        0       99 2023-02-24 13:10:55.696823 robotmk-0.0.49/src/_robotmk/modes/robot/cli.py
--rwxr-xr-x   0        0        0      308 2023-02-24 13:10:55.696823 robotmk-0.0.49/src/_robotmk/modes/robotmk.py
--rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.49/src/_robotmk/modes/specialagent/__init__.py
--rwxr-xr-x   0        0        0      106 2023-02-24 13:10:55.696823 robotmk-0.0.49/src/_robotmk/modes/specialagent/cli.py
--rw-r--r--   0        0        0    25966 2023-03-09 10:38:47.105752 robotmk-0.0.49/src/categories.json
--rw-r--r--   0        0        0     2161 2023-03-09 11:10:22.787194 robotmk-0.0.49/src/click_tutorial.py
--rw-r--r--   0        0        0       92 2023-04-12 16:12:46.194371 robotmk-0.0.49/src/robotmk/__init__.py
--rw-r--r--   0        0        0     5514 2023-03-30 06:57:58.218217 robotmk-0.0.49/src/robotmk/cli/cli.py
--rw-r--r--   0        0        0     3033 2023-03-16 11:52:36.253603 robotmk-0.0.49/src/robotmk/cli/defaultgroup.py
--rw-r--r--   0        0        0       64 2023-03-30 15:36:25.625426 robotmk-0.0.49/src/robotmk/config/__init__.py
--rw-r--r--   0        0        0    15122 2023-04-12 15:30:56.411240 robotmk-0.0.49/src/robotmk/config/config.py
--rw-r--r--   0        0        0     2498 2023-03-30 14:32:11.107185 robotmk-0.0.49/src/robotmk/config/yml.py
--rw-r--r--   0        0        0      178 2023-03-14 15:49:36.083594 robotmk-0.0.49/src/robotmk/context/__init__.py
--rw-r--r--   0        0        0     2293 2023-03-30 15:57:46.648634 robotmk-0.0.49/src/robotmk/context/abstract.py
--rw-r--r--   0        0        0      644 2023-03-29 10:27:39.457231 robotmk-0.0.49/src/robotmk/context/context.py
--rw-r--r--   0        0        0        0 2023-03-10 09:07:26.579374 robotmk-0.0.49/src/robotmk/context/local/__init__.py
--rw-r--r--   0        0        0     1211 2023-04-04 10:17:17.443557 robotmk-0.0.49/src/robotmk/context/local/cli.py
--rw-r--r--   0        0        0     2091 2023-03-29 11:50:24.791476 robotmk-0.0.49/src/robotmk/context/local/local.py
--rw-r--r--   0        0        0        0 2023-03-16 12:36:31.416463 robotmk-0.0.49/src/robotmk/context/server/__init__.py
--rw-r--r--   0        0        0      501 2023-04-04 10:17:35.143381 robotmk-0.0.49/src/robotmk/context/server/cli.py
--rw-r--r--   0        0        0        0 2023-03-16 12:36:40.036375 robotmk-0.0.49/src/robotmk/context/server/server.py
--rw-r--r--   0        0        0        0 2023-03-10 09:07:27.895361 robotmk-0.0.49/src/robotmk/context/specialagent/__init__.py
--rw-r--r--   0        0        0     1172 2023-04-04 10:17:56.403169 robotmk-0.0.49/src/robotmk/context/specialagent/cli.py
--rw-r--r--   0        0        0     1899 2023-03-29 11:50:21.439532 robotmk-0.0.49/src/robotmk/context/specialagent/specialagent.py
--rw-r--r--   0        0        0        0 2023-03-10 09:07:29.079350 robotmk-0.0.49/src/robotmk/context/suite/__init__.py
--rw-r--r--   0        0        0     3728 2023-04-04 10:54:27.529704 robotmk-0.0.49/src/robotmk/context/suite/cli.py
--rw-r--r--   0        0        0      125 2023-04-01 20:18:16.209113 robotmk-0.0.49/src/robotmk/context/suite/strategies/__init__.py
--rw-r--r--   0        0        0     5991 2023-04-12 16:06:33.770403 robotmk-0.0.49/src/robotmk/context/suite/strategies/run.py
--rw-r--r--   0        0        0     4293 2023-04-04 11:45:02.256091 robotmk-0.0.49/src/robotmk/context/suite/suite.py
--rw-r--r--   0        0        0      136 2023-04-01 18:27:58.571962 robotmk-0.0.49/src/robotmk/context/suite/target/__init__.py
--rw-r--r--   0        0        0     8422 2023-04-12 15:48:14.953328 robotmk-0.0.49/src/robotmk/context/suite/target/rcc.py
--rw-r--r--   0        0        0      315 2023-03-30 05:55:28.600317 robotmk-0.0.49/src/robotmk/context/suite/target/remote.py
--rw-r--r--   0        0        0       49 2023-04-03 17:11:56.923310 robotmk-0.0.49/src/robotmk/context/suite/target/robotframework/__init__.py
--rw-r--r--   0        0        0     5559 2023-04-09 16:52:38.817097 robotmk-0.0.49/src/robotmk/context/suite/target/robotframework/retry.py
--rw-r--r--   0        0        0     6448 2023-04-09 16:54:03.952360 robotmk-0.0.49/src/robotmk/context/suite/target/robotframework/robotframework.py
--rw-r--r--   0        0        0     4662 2023-04-09 17:05:22.342438 robotmk-0.0.49/src/robotmk/context/suite/target/robotframework/state.py
--rw-r--r--   0        0        0     2732 2023-04-12 16:06:53.534180 robotmk-0.0.49/src/robotmk/context/suite/target/target.py
--rw-r--r--   0        0        0        0 2023-03-16 16:00:58.422756 robotmk-0.0.49/src/robotmk/executor/__init__.py
--rw-r--r--   0        0        0      438 2023-03-21 06:35:39.773943 robotmk-0.0.49/src/robotmk/executor/abstract.py
--rw-r--r--   0        0        0     2013 2023-03-20 12:52:41.400361 robotmk-0.0.49/src/robotmk/executor/scheduler.py
--rw-r--r--   0        0        0      287 2023-03-20 12:52:46.348308 robotmk-0.0.49/src/robotmk/executor/sequencer.py
--rw-r--r--   0        0        0      552 2023-03-21 11:00:25.331460 robotmk-0.0.49/src/robotmk/executor/suiterunner.py
--rw-r--r--   0        0        0     2027 2023-04-04 10:56:24.192653 robotmk-0.0.49/src/robotmk/logger.py
--rw-r--r--   0        0        0     3463 2023-04-03 08:53:57.612055 robotmk-0.0.49/src/robotmk/main.py
--rw-r--r--   0        0        0        0 2023-03-04 11:04:47.025603 robotmk-0.0.49/tests/__init__.py
--rw-r--r--   0        0        0       25 2023-04-12 14:35:21.918852 robotmk-0.0.49/tests/config/robotmk.env
--rw-r--r--   0        0        0     2075 2023-04-04 09:03:29.524056 robotmk-0.0.49/tests/config/robotmk.yml
--rw-r--r--   0        0        0     9958 2023-04-12 15:08:57.203733 robotmk-0.0.49/tests/config/test_config.py
--rw-r--r--   0        0        0      300 2023-03-14 15:05:35.715975 robotmk-0.0.49/tests/context/local/robotmk.yml
--rw-r--r--   0        0        0     1265 2023-03-16 08:41:25.311423 robotmk-0.0.49/tests/context/local/test_local_cli.py
--rw-r--r--   0        0        0      746 2023-03-14 15:06:49.651217 robotmk-0.0.49/tests/context/specialagent/test_specialagent_cli.py
--rw-r--r--   0        0        0     2075 2023-04-04 10:39:17.810567 robotmk-0.0.49/tests/context/suite/robotmk.yml
--rw-r--r--   0        0        0      427 2023-04-04 10:41:57.860986 robotmk-0.0.49/tests/context/suite/test_suite.py
--rw-r--r--   0        0        0      842 2023-04-03 10:50:55.769100 robotmk-0.0.49/tests/context/suite/test_suite_cli.py
--rw-r--r--   0        0        0      991 2023-03-14 11:06:07.698634 robotmk-0.0.49/tests/context/test_cli.py
--rw-r--r--   0        0        0      945 2023-03-20 10:00:06.880076 robotmk-0.0.49/tests/yml/robotmk.yml
--rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 robotmk-0.0.49/PKG-INFO
+-rw-r--r--   0        0        0      110 2023-04-13 05:37:52.711274 robotmk-0.0.50/.bumpversion.cfg
+-rw-r--r--   0        0        0      284 2023-04-04 11:07:18.122518 robotmk-0.0.50/.cli.env
+-rw-r--r--   0        0        0       40 2023-02-24 13:10:55.692823 robotmk-0.0.50/README.md
+-rw-r--r--   0        0        0      739 2023-04-12 16:12:36.358474 robotmk-0.0.50/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-28 07:41:38.789867 robotmk-0.0.50/src/_confitree/__init__.py
+-rw-r--r--   0        0        0     5092 2023-03-02 13:49:11.086894 robotmk-0.0.50/src/_confitree/confitree.py
+-rw-r--r--   0        0        0      512 2023-03-04 11:44:09.697687 robotmk-0.0.50/src/_confitree/robotmk.yml
+-rwxr-xr-x   0        0        0      635 2023-02-24 13:10:55.692823 robotmk-0.0.50/src/_robotmk/__init__.py
+-rwxr-xr-x   0        0        0      533 2023-02-24 13:10:55.692823 robotmk-0.0.50/src/_robotmk/__main__.py
+-rwxr-xr-x   0        0        0     2249 2023-03-03 09:34:49.997849 robotmk-0.0.50/src/_robotmk/cli.py
+-rwxr-xr-x   0        0        0      754 2023-02-24 13:10:55.696823 robotmk-0.0.50/src/_robotmk/modes/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.50/src/_robotmk/modes/agent/__init__.py
+-rwxr-xr-x   0        0        0    11155 2023-02-24 13:10:55.696823 robotmk-0.0.50/src/_robotmk/modes/agent/agent.py
+-rwxr-xr-x   0        0        0     1152 2023-02-24 13:10:55.696823 robotmk-0.0.50/src/_robotmk/modes/agent/cli.py
+-rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.50/src/_robotmk/modes/output/__init__.py
+-rwxr-xr-x   0        0        0      100 2023-02-24 13:10:55.696823 robotmk-0.0.50/src/_robotmk/modes/output/cli.py
+-rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.50/src/_robotmk/modes/robot/__init__.py
+-rwxr-xr-x   0        0        0       99 2023-02-24 13:10:55.696823 robotmk-0.0.50/src/_robotmk/modes/robot/cli.py
+-rwxr-xr-x   0        0        0      308 2023-02-24 13:10:55.696823 robotmk-0.0.50/src/_robotmk/modes/robotmk.py
+-rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.50/src/_robotmk/modes/specialagent/__init__.py
+-rwxr-xr-x   0        0        0      106 2023-02-24 13:10:55.696823 robotmk-0.0.50/src/_robotmk/modes/specialagent/cli.py
+-rw-r--r--   0        0        0    25966 2023-03-09 10:38:47.105752 robotmk-0.0.50/src/categories.json
+-rw-r--r--   0        0        0     2161 2023-03-09 11:10:22.787194 robotmk-0.0.50/src/click_tutorial.py
+-rw-r--r--   0        0        0       92 2023-04-13 05:37:52.711274 robotmk-0.0.50/src/robotmk/__init__.py
+-rw-r--r--   0        0        0     5514 2023-03-30 06:57:58.218217 robotmk-0.0.50/src/robotmk/cli/cli.py
+-rw-r--r--   0        0        0     3033 2023-03-16 11:52:36.253603 robotmk-0.0.50/src/robotmk/cli/defaultgroup.py
+-rw-r--r--   0        0        0       64 2023-03-30 15:36:25.625426 robotmk-0.0.50/src/robotmk/config/__init__.py
+-rw-r--r--   0        0        0    15053 2023-04-13 05:21:28.444796 robotmk-0.0.50/src/robotmk/config/config.py
+-rw-r--r--   0        0        0     2498 2023-03-30 14:32:11.107185 robotmk-0.0.50/src/robotmk/config/yml.py
+-rw-r--r--   0        0        0      178 2023-03-14 15:49:36.083594 robotmk-0.0.50/src/robotmk/context/__init__.py
+-rw-r--r--   0        0        0     2293 2023-03-30 15:57:46.648634 robotmk-0.0.50/src/robotmk/context/abstract.py
+-rw-r--r--   0        0        0      644 2023-03-29 10:27:39.457231 robotmk-0.0.50/src/robotmk/context/context.py
+-rw-r--r--   0        0        0        0 2023-03-10 09:07:26.579374 robotmk-0.0.50/src/robotmk/context/local/__init__.py
+-rw-r--r--   0        0        0     1211 2023-04-04 10:17:17.443557 robotmk-0.0.50/src/robotmk/context/local/cli.py
+-rw-r--r--   0        0        0     2091 2023-03-29 11:50:24.791476 robotmk-0.0.50/src/robotmk/context/local/local.py
+-rw-r--r--   0        0        0        0 2023-03-16 12:36:31.416463 robotmk-0.0.50/src/robotmk/context/server/__init__.py
+-rw-r--r--   0        0        0      501 2023-04-04 10:17:35.143381 robotmk-0.0.50/src/robotmk/context/server/cli.py
+-rw-r--r--   0        0        0        0 2023-03-16 12:36:40.036375 robotmk-0.0.50/src/robotmk/context/server/server.py
+-rw-r--r--   0        0        0        0 2023-03-10 09:07:27.895361 robotmk-0.0.50/src/robotmk/context/specialagent/__init__.py
+-rw-r--r--   0        0        0     1172 2023-04-04 10:17:56.403169 robotmk-0.0.50/src/robotmk/context/specialagent/cli.py
+-rw-r--r--   0        0        0     1899 2023-03-29 11:50:21.439532 robotmk-0.0.50/src/robotmk/context/specialagent/specialagent.py
+-rw-r--r--   0        0        0        0 2023-03-10 09:07:29.079350 robotmk-0.0.50/src/robotmk/context/suite/__init__.py
+-rw-r--r--   0        0        0     3728 2023-04-04 10:54:27.529704 robotmk-0.0.50/src/robotmk/context/suite/cli.py
+-rw-r--r--   0        0        0      125 2023-04-01 20:18:16.209113 robotmk-0.0.50/src/robotmk/context/suite/strategies/__init__.py
+-rw-r--r--   0        0        0     6576 2023-04-13 05:28:33.289623 robotmk-0.0.50/src/robotmk/context/suite/strategies/run.py
+-rw-r--r--   0        0        0     4293 2023-04-04 11:45:02.256091 robotmk-0.0.50/src/robotmk/context/suite/suite.py
+-rw-r--r--   0        0        0      136 2023-04-01 18:27:58.571962 robotmk-0.0.50/src/robotmk/context/suite/target/__init__.py
+-rw-r--r--   0        0        0     4608 2023-04-13 05:35:37.852792 robotmk-0.0.50/src/robotmk/context/suite/target/rcc.py
+-rw-r--r--   0        0        0      315 2023-03-30 05:55:28.600317 robotmk-0.0.50/src/robotmk/context/suite/target/remote.py
+-rw-r--r--   0        0        0       49 2023-04-03 17:11:56.923310 robotmk-0.0.50/src/robotmk/context/suite/target/robotframework/__init__.py
+-rw-r--r--   0        0        0     5559 2023-04-09 16:52:38.817097 robotmk-0.0.50/src/robotmk/context/suite/target/robotframework/retry.py
+-rw-r--r--   0        0        0     6448 2023-04-09 16:54:03.952360 robotmk-0.0.50/src/robotmk/context/suite/target/robotframework/robotframework.py
+-rw-r--r--   0        0        0     4662 2023-04-09 17:05:22.342438 robotmk-0.0.50/src/robotmk/context/suite/target/robotframework/state.py
+-rw-r--r--   0        0        0     2768 2023-04-13 05:33:55.966022 robotmk-0.0.50/src/robotmk/context/suite/target/target.py
+-rw-r--r--   0        0        0        0 2023-03-16 16:00:58.422756 robotmk-0.0.50/src/robotmk/executor/__init__.py
+-rw-r--r--   0        0        0      438 2023-03-21 06:35:39.773943 robotmk-0.0.50/src/robotmk/executor/abstract.py
+-rw-r--r--   0        0        0     2013 2023-03-20 12:52:41.400361 robotmk-0.0.50/src/robotmk/executor/scheduler.py
+-rw-r--r--   0        0        0      287 2023-03-20 12:52:46.348308 robotmk-0.0.50/src/robotmk/executor/sequencer.py
+-rw-r--r--   0        0        0      552 2023-03-21 11:00:25.331460 robotmk-0.0.50/src/robotmk/executor/suiterunner.py
+-rw-r--r--   0        0        0     2027 2023-04-04 10:56:24.192653 robotmk-0.0.50/src/robotmk/logger.py
+-rw-r--r--   0        0        0     3463 2023-04-03 08:53:57.612055 robotmk-0.0.50/src/robotmk/main.py
+-rw-r--r--   0        0        0        0 2023-03-04 11:04:47.025603 robotmk-0.0.50/tests/__init__.py
+-rw-r--r--   0        0        0       25 2023-04-12 14:35:21.918852 robotmk-0.0.50/tests/config/robotmk.env
+-rw-r--r--   0        0        0     2075 2023-04-04 09:03:29.524056 robotmk-0.0.50/tests/config/robotmk.yml
+-rw-r--r--   0        0        0     9958 2023-04-12 15:08:57.203733 robotmk-0.0.50/tests/config/test_config.py
+-rw-r--r--   0        0        0      300 2023-03-14 15:05:35.715975 robotmk-0.0.50/tests/context/local/robotmk.yml
+-rw-r--r--   0        0        0     1265 2023-03-16 08:41:25.311423 robotmk-0.0.50/tests/context/local/test_local_cli.py
+-rw-r--r--   0        0        0      746 2023-03-14 15:06:49.651217 robotmk-0.0.50/tests/context/specialagent/test_specialagent_cli.py
+-rw-r--r--   0        0        0     2075 2023-04-04 10:39:17.810567 robotmk-0.0.50/tests/context/suite/robotmk.yml
+-rw-r--r--   0        0        0      427 2023-04-04 10:41:57.860986 robotmk-0.0.50/tests/context/suite/test_suite.py
+-rw-r--r--   0        0        0      842 2023-04-03 10:50:55.769100 robotmk-0.0.50/tests/context/suite/test_suite_cli.py
+-rw-r--r--   0        0        0      991 2023-03-14 11:06:07.698634 robotmk-0.0.50/tests/context/test_cli.py
+-rw-r--r--   0        0        0      945 2023-03-20 10:00:06.880076 robotmk-0.0.50/tests/yml/robotmk.yml
+-rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 robotmk-0.0.50/PKG-INFO
```

### Comparing `robotmk-0.0.49/pyproject.toml` & `robotmk-0.0.50/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/src/_confitree/confitree.py` & `robotmk-0.0.50/src/_confitree/confitree.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/src/_confitree/robotmk.yml` & `robotmk-0.0.50/src/_confitree/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/src/_robotmk/__init__.py` & `robotmk-0.0.50/src/_robotmk/__init__.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/src/_robotmk/__main__.py` & `robotmk-0.0.50/src/_robotmk/__main__.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/src/_robotmk/cli.py` & `robotmk-0.0.50/src/_robotmk/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/src/_robotmk/modes/__init__.py` & `robotmk-0.0.50/src/_robotmk/modes/__init__.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/src/_robotmk/modes/agent/agent.py` & `robotmk-0.0.50/src/_robotmk/modes/agent/agent.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/src/_robotmk/modes/agent/cli.py` & `robotmk-0.0.50/src/_robotmk/modes/agent/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/src/categories.json` & `robotmk-0.0.50/src/categories.json`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/src/click_tutorial.py` & `robotmk-0.0.50/src/click_tutorial.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/src/robotmk/cli/cli.py` & `robotmk-0.0.50/src/robotmk/cli/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/src/robotmk/cli/defaultgroup.py` & `robotmk-0.0.50/src/robotmk/cli/defaultgroup.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/src/robotmk/config/config.py` & `robotmk-0.0.50/src/robotmk/config/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -346,47 +346,44 @@
             return vdict
 
         # Remove the ROBOTMK_ prefix
         varname = o_varname.replace(self.envvar_prefix + "_", "")
         _str2dict(varname, value, vdict)
         return vdict
 
-    def to_environment(self, d=None, prefix=""):
+    def to_environment(self, d=None, prefix="", environ=None):
         """Converts a given dict/value or self.configdict to environment variables.
 
-        The rules are:
+        If environ is given, the environment variables are added to the given dict.
+        Otherwise the environment variables are added to the current environment.
+
+        The conversion rules are:
         - there is no case conversion
         - underscores within key names are replaced by double underscores
         - the prefix is added to the environment variable name
         - dicts are converted to nested environment variables
         - lists get a number appended to their key name"""
         if d is None:
             d = self.configdict
-        if isinstance(d, dict):
+        if isinstance(d, dict):  # DICT conversion
             for key, value in d.items():
                 safe_key = key.replace("_", "__")
                 new_prefix = f"{prefix}_{safe_key}"
-                self.to_environment(value, prefix=new_prefix)
-
-                # elif isinstance(value, list):
-                #     for i, item in enumerate(value):
-                #         new_prefix = f"{prefix}_{safe_key}_{i}"
-                #         self.to_environment(item, prefix=new_prefix)
-                # else:
-                #     varname = f"{self.envvar_prefix}{prefix}_{safe_key}"
-                #     print(f"{varname} = {value}")
-                #     os.environ[varname] = str(value)
-        elif isinstance(d, list):
+                self.to_environment(value, prefix=new_prefix, environ=environ)
+        elif isinstance(d, list):  # LIST conversion
             for i, item in enumerate(d):
                 new_prefix = f"{prefix}_{i}"
-                self.to_environment(item, prefix=new_prefix)
-        else:
+                self.to_environment(item, prefix=new_prefix, environ=environ)
+        else:  # VALUE conversion
             varname = f"{self.envvar_prefix}{prefix}"
-            # print(f"{varname} = {d}")
-            os.environ[varname] = str(d)
+            print(f"{varname} = {d}")
+            if environ is None:
+                os.environ[varname] = str(d)
+            else:
+                environ[varname] = str(d)
 
     def to_yml(self, file=None) -> Union[str, None]:
         """Dumps the config to a file returns it."""
         if file:
             try:
                 with open(file, "w") as f:
                     yaml.dump(self.configdict, f)
```

### Comparing `robotmk-0.0.49/src/robotmk/config/yml.py` & `robotmk-0.0.50/src/robotmk/config/yml.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/src/robotmk/context/abstract.py` & `robotmk-0.0.50/src/robotmk/context/abstract.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/src/robotmk/context/context.py` & `robotmk-0.0.50/src/robotmk/context/context.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/src/robotmk/context/local/cli.py` & `robotmk-0.0.50/src/robotmk/context/local/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/src/robotmk/context/local/local.py` & `robotmk-0.0.50/src/robotmk/context/local/local.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/src/robotmk/context/specialagent/cli.py` & `robotmk-0.0.50/src/robotmk/context/specialagent/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/src/robotmk/context/specialagent/specialagent.py` & `robotmk-0.0.50/src/robotmk/context/specialagent/specialagent.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/src/robotmk/context/suite/cli.py` & `robotmk-0.0.50/src/robotmk/context/suite/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/src/robotmk/context/suite/suite.py` & `robotmk-0.0.50/src/robotmk/context/suite/suite.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/src/robotmk/context/suite/target/robotframework/retry.py` & `robotmk-0.0.50/src/robotmk/context/suite/target/robotframework/retry.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/src/robotmk/context/suite/target/robotframework/robotframework.py` & `robotmk-0.0.50/src/robotmk/context/suite/target/robotframework/robotframework.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/src/robotmk/context/suite/target/robotframework/state.py` & `robotmk-0.0.50/src/robotmk/context/suite/target/robotframework/state.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/src/robotmk/context/suite/target/target.py` & `robotmk-0.0.50/src/robotmk/context/suite/target/target.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,17 +51,18 @@
         suiteuname: str,
         config: dict,
         logger: RobotmkLogger,
     ):
         super().__init__(suiteuname, config, logger)
 
         # Store RCC and RF logs in separate folders
-        self.config.set(
-            "common.logdir", "%s/%s" % (self.config.get("common.logdir"), str(self))
-        )
+        # TODO: relly needed?
+        # self.config.set(
+        #     "common.logdir", "%s/%s" % (self.config.get("common.logdir"), str(self))
+        # )
 
         self.path = Path(self.config.get("common.robotdir")).joinpath(
             self.config.get("suitecfg.path")
         )
         self.run_strategy = RunStrategyFactory(self).create()
         # list of subprocess' results and console output
         self.console_results = {}
```

### Comparing `robotmk-0.0.49/src/robotmk/executor/scheduler.py` & `robotmk-0.0.50/src/robotmk/executor/scheduler.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/src/robotmk/executor/suiterunner.py` & `robotmk-0.0.50/src/robotmk/executor/suiterunner.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/src/robotmk/logger.py` & `robotmk-0.0.50/src/robotmk/logger.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/src/robotmk/main.py` & `robotmk-0.0.50/src/robotmk/main.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/tests/config/robotmk.yml` & `robotmk-0.0.50/tests/config/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/tests/config/test_config.py` & `robotmk-0.0.50/tests/config/test_config.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/tests/context/local/test_local_cli.py` & `robotmk-0.0.50/tests/context/local/test_local_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/tests/context/specialagent/test_specialagent_cli.py` & `robotmk-0.0.50/tests/context/specialagent/test_specialagent_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/tests/context/suite/robotmk.yml` & `robotmk-0.0.50/tests/context/suite/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/tests/context/suite/test_suite_cli.py` & `robotmk-0.0.50/tests/context/suite/test_suite_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/tests/context/test_cli.py` & `robotmk-0.0.50/tests/context/test_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/tests/yml/robotmk.yml` & `robotmk-0.0.50/tests/yml/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.49/PKG-INFO` & `robotmk-0.0.50/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotmk
-Version: 0.0.49
+Version: 0.0.50
 Summary: Robot Framework test execution and result parsing for Check_MK
 Keywords: robotmk,checkmk,robotframework,automation,monitoring
 Author-email: Simon Meggle <simon.meggle@elabit.de>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: click
 Requires-Dist: psutil
```

