# Comparing `tmp/ezmsg-3.3.0.tar.gz` & `tmp/ezmsg-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezmsg-3.3.0.tar", last modified: Wed Mar 29 20:03:00 2023, max compression
+gzip compressed data, was "ezmsg-3.3.1.tar", last modified: Thu Apr 13 18:59:02 2023, max compression
```

## Comparing `ezmsg-3.3.0.tar` & `ezmsg-3.3.1.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:03:00.201652 ezmsg-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-03-29 20:02:50.000000 ezmsg-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-03-29 20:03:00.201652 ezmsg-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-03-29 20:02:50.000000 ezmsg-3.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:03:00.173652 ezmsg-3.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:03:00.177652 ezmsg-3.3.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-29 20:02:50.000000 ezmsg-3.3.0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:03:00.181652 ezmsg-3.3.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-29 20:02:50.000000 ezmsg-3.3.0/examples/ezmsg_attach.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-03-29 20:02:50.000000 ezmsg-3.3.0/examples/ezmsg_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-03-29 20:02:50.000000 ezmsg-3.3.0/examples/ezmsg_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-03-29 20:02:50.000000 ezmsg-3.3.0/examples/ezmsg_intro.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-03-29 20:02:50.000000 ezmsg-3.3.0/examples/ezmsg_normalterm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-03-29 20:02:50.000000 ezmsg-3.3.0/examples/ezmsg_stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-03-29 20:02:50.000000 ezmsg-3.3.0/examples/ezmsg_toy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:03:00.173652 ezmsg-3.3.0/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:03:00.181652 ezmsg-3.3.0/extensions/ezmsg-sigproc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:03:00.173652 ezmsg-3.3.0/extensions/ezmsg-sigproc/ezmsg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:03:00.185652 ezmsg-3.3.0/extensions/ezmsg-sigproc/ezmsg/sigproc/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-29 20:02:50.000000 ezmsg-3.3.0/extensions/ezmsg-sigproc/ezmsg/sigproc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-29 20:02:50.000000 ezmsg-3.3.0/extensions/ezmsg-sigproc/ezmsg/sigproc/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-03-29 20:02:50.000000 ezmsg-3.3.0/extensions/ezmsg-sigproc/ezmsg/sigproc/butterworthfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-03-29 20:02:50.000000 ezmsg-3.3.0/extensions/ezmsg-sigproc/ezmsg/sigproc/decimate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-03-29 20:02:50.000000 ezmsg-3.3.0/extensions/ezmsg-sigproc/ezmsg/sigproc/downsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-03-29 20:02:50.000000 ezmsg-3.3.0/extensions/ezmsg-sigproc/ezmsg/sigproc/ewmfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-03-29 20:02:50.000000 ezmsg-3.3.0/extensions/ezmsg-sigproc/ezmsg/sigproc/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-03-29 20:02:50.000000 ezmsg-3.3.0/extensions/ezmsg-sigproc/ezmsg/sigproc/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-03-29 20:02:50.000000 ezmsg-3.3.0/extensions/ezmsg-sigproc/ezmsg/sigproc/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-03-29 20:02:50.000000 ezmsg-3.3.0/extensions/ezmsg-sigproc/ezmsg/sigproc/spectral.py
--rw-r--r--   0 runner    (1001) docker     (123)    12929 2023-03-29 20:02:50.000000 ezmsg-3.3.0/extensions/ezmsg-sigproc/ezmsg/sigproc/synth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-03-29 20:02:50.000000 ezmsg-3.3.0/extensions/ezmsg-sigproc/ezmsg/sigproc/window.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-29 20:02:50.000000 ezmsg-3.3.0/extensions/ezmsg-sigproc/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:03:00.185652 ezmsg-3.3.0/extensions/ezmsg-sigproc/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-03-29 20:02:50.000000 ezmsg-3.3.0/extensions/ezmsg-sigproc/tests/test_butterworth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-03-29 20:02:50.000000 ezmsg-3.3.0/extensions/ezmsg-sigproc/tests/test_downsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-03-29 20:02:50.000000 ezmsg-3.3.0/extensions/ezmsg-sigproc/tests/test_window.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-03-29 20:02:50.000000 ezmsg-3.3.0/extensions/ezmsg-sigproc/tests/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:03:00.185652 ezmsg-3.3.0/extensions/ezmsg-websocket/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:03:00.185652 ezmsg-3.3.0/extensions/ezmsg-websocket/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-03-29 20:02:50.000000 ezmsg-3.3.0/extensions/ezmsg-websocket/examples/ezmsg_websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:03:00.173652 ezmsg-3.3.0/extensions/ezmsg-websocket/ezmsg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:03:00.185652 ezmsg-3.3.0/extensions/ezmsg-websocket/ezmsg/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-29 20:02:50.000000 ezmsg-3.3.0/extensions/ezmsg-websocket/ezmsg/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-29 20:02:50.000000 ezmsg-3.3.0/extensions/ezmsg-websocket/ezmsg/websocket/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-03-29 20:02:50.000000 ezmsg-3.3.0/extensions/ezmsg-websocket/ezmsg/websocket/units.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-29 20:02:50.000000 ezmsg-3.3.0/extensions/ezmsg-websocket/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:03:00.185652 ezmsg-3.3.0/extensions/ezmsg-zmq/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:03:00.173652 ezmsg-3.3.0/extensions/ezmsg-zmq/ezmsg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:03:00.185652 ezmsg-3.3.0/extensions/ezmsg-zmq/ezmsg/zmq/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-29 20:02:50.000000 ezmsg-3.3.0/extensions/ezmsg-zmq/ezmsg/zmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-29 20:02:50.000000 ezmsg-3.3.0/extensions/ezmsg-zmq/ezmsg/zmq/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-03-29 20:02:50.000000 ezmsg-3.3.0/extensions/ezmsg-zmq/ezmsg/zmq/units.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-29 20:02:50.000000 ezmsg-3.3.0/extensions/ezmsg-zmq/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:03:00.177652 ezmsg-3.3.0/ezmsg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:03:00.193652 ezmsg-3.3.0/ezmsg/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/core/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/core/addressable.py
--rw-r--r--   0 runner    (1001) docker     (123)     8952 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/core/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/core/backendprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/core/backpressure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/core/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/core/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/core/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/core/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/core/graphcontext.py
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/core/graphserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/core/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/core/messagecache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/core/messagemarshal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/core/netprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)    10175 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/core/pubclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/core/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/core/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/core/shmserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/core/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/core/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/core/subclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/core/unit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:03:00.193652 ezmsg-3.3.0/ezmsg/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/testing/debuglog.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/testing/lfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/testing/multiplier.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/testing/terminate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:03:00.197652 ezmsg-3.3.0/ezmsg/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/util/debuglog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/util/messagecodec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/util/messagegate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/util/messagelogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/util/messagequeue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/util/messagereplay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:03:00.197652 ezmsg-3.3.0/ezmsg/util/messages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/util/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/util/messages/axisarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/util/rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/util/terminate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:03:00.197652 ezmsg-3.3.0/ezmsg/version/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-29 20:02:50.000000 ezmsg-3.3.0/ezmsg/version/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:03:00.189652 ezmsg-3.3.0/ezmsg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-03-29 20:03:00.000000 ezmsg-3.3.0/ezmsg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-03-29 20:03:00.000000 ezmsg-3.3.0/ezmsg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 20:03:00.000000 ezmsg-3.3.0/ezmsg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-29 20:03:00.000000 ezmsg-3.3.0/ezmsg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-29 20:03:00.000000 ezmsg-3.3.0/ezmsg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-29 20:03:00.000000 ezmsg-3.3.0/ezmsg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-29 20:02:50.000000 ezmsg-3.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-03-29 20:03:00.201652 ezmsg-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 20:02:50.000000 ezmsg-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:03:00.201652 ezmsg-3.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-03-29 20:02:50.000000 ezmsg-3.3.0/tests/test_addressable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-03-29 20:02:50.000000 ezmsg-3.3.0/tests/test_attach.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-03-29 20:02:50.000000 ezmsg-3.3.0/tests/test_axisarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-03-29 20:02:50.000000 ezmsg-3.3.0/tests/test_connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-03-29 20:02:50.000000 ezmsg-3.3.0/tests/test_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-03-29 20:02:50.000000 ezmsg-3.3.0/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-03-29 20:02:50.000000 ezmsg-3.3.0/tests/test_perf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-03-29 20:02:50.000000 ezmsg-3.3.0/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-03-29 20:02:50.000000 ezmsg-3.3.0/tests/test_shm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-03-29 20:02:50.000000 ezmsg-3.3.0/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-29 20:02:50.000000 ezmsg-3.3.0/tests/test_test.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 20:02:50.000000 ezmsg-3.3.0/tests/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.974635 ezmsg-3.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-13 18:58:53.000000 ezmsg-3.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-13 18:59:02.974635 ezmsg-3.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-13 18:58:53.000000 ezmsg-3.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.946634 ezmsg-3.3.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.954635 ezmsg-3.3.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-13 18:58:53.000000 ezmsg-3.3.1/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.958635 ezmsg-3.3.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-13 18:58:53.000000 ezmsg-3.3.1/examples/ezmsg_attach.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-04-13 18:58:53.000000 ezmsg-3.3.1/examples/ezmsg_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-13 18:58:53.000000 ezmsg-3.3.1/examples/ezmsg_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-04-13 18:58:53.000000 ezmsg-3.3.1/examples/ezmsg_intro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-13 18:58:53.000000 ezmsg-3.3.1/examples/ezmsg_normalterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-04-13 18:58:53.000000 ezmsg-3.3.1/examples/ezmsg_stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-04-13 18:58:53.000000 ezmsg-3.3.1/examples/ezmsg_toy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.950635 ezmsg-3.3.1/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.958635 ezmsg-3.3.1/extensions/ezmsg-sigproc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.950635 ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.962635 ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/butterworthfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/decimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/downsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/ewmfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10100 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/spectral.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12929 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/synth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/window.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.962635 ezmsg-3.3.1/extensions/ezmsg-sigproc/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/tests/test_butterworth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/tests/test_downsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/tests/test_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.962635 ezmsg-3.3.1/extensions/ezmsg-websocket/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.962635 ezmsg-3.3.1/extensions/ezmsg-websocket/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-websocket/examples/ezmsg_websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.950635 ezmsg-3.3.1/extensions/ezmsg-websocket/ezmsg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.962635 ezmsg-3.3.1/extensions/ezmsg-websocket/ezmsg/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-websocket/ezmsg/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-websocket/ezmsg/websocket/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-websocket/ezmsg/websocket/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-websocket/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.966635 ezmsg-3.3.1/extensions/ezmsg-zmq/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.950635 ezmsg-3.3.1/extensions/ezmsg-zmq/ezmsg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.966635 ezmsg-3.3.1/extensions/ezmsg-zmq/ezmsg/zmq/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-zmq/ezmsg/zmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-zmq/ezmsg/zmq/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-zmq/ezmsg/zmq/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-zmq/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.950635 ezmsg-3.3.1/ezmsg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.970635 ezmsg-3.3.1/ezmsg/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/addressable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10343 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/backendprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/backpressure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/graphcontext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/graphserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/messagecache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/messagemarshal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/netprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10175 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/pubclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/shmserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/subclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.970635 ezmsg-3.3.1/ezmsg/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/testing/debuglog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/testing/lfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/testing/multiplier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/testing/terminate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.970635 ezmsg-3.3.1/ezmsg/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/util/debuglog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/util/messagecodec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/util/messagegate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/util/messagelogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/util/messagequeue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/util/messagereplay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.970635 ezmsg-3.3.1/ezmsg/util/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/util/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/util/messages/axisarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/util/rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/util/terminate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.970635 ezmsg-3.3.1/ezmsg/version/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/version/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.966635 ezmsg-3.3.1/ezmsg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-13 18:59:02.000000 ezmsg-3.3.1/ezmsg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-13 18:59:02.000000 ezmsg-3.3.1/ezmsg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:59:02.000000 ezmsg-3.3.1/ezmsg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-13 18:59:02.000000 ezmsg-3.3.1/ezmsg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-13 18:59:02.000000 ezmsg-3.3.1/ezmsg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-13 18:59:02.000000 ezmsg-3.3.1/ezmsg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-13 18:58:53.000000 ezmsg-3.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-13 18:59:02.974635 ezmsg-3.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 18:58:53.000000 ezmsg-3.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.974635 ezmsg-3.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-13 18:58:53.000000 ezmsg-3.3.1/tests/test_addressable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-04-13 18:58:53.000000 ezmsg-3.3.1/tests/test_attach.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-04-13 18:58:53.000000 ezmsg-3.3.1/tests/test_axisarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-13 18:58:53.000000 ezmsg-3.3.1/tests/test_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-13 18:58:53.000000 ezmsg-3.3.1/tests/test_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-04-13 18:58:53.000000 ezmsg-3.3.1/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-04-13 18:58:53.000000 ezmsg-3.3.1/tests/test_perf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-04-13 18:58:53.000000 ezmsg-3.3.1/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-13 18:58:53.000000 ezmsg-3.3.1/tests/test_shm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-13 18:58:53.000000 ezmsg-3.3.1/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 18:58:53.000000 ezmsg-3.3.1/tests/test_test.py
```

### Comparing `ezmsg-3.3.0/LICENSE` & `ezmsg-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/PKG-INFO` & `ezmsg-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezmsg
-Version: 3.3.0
+Version: 3.3.1
 Summary: A simple DAG-based computation model
 Home-page: https://github.com/iscoe/ezmsg
 Author: Griffin Milsap
 Author-email: griffin.milsap@jhuapl.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `ezmsg-3.3.0/README.md` & `ezmsg-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/docs/source/conf.py` & `ezmsg-3.3.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/examples/ezmsg_configs.py` & `ezmsg-3.3.1/examples/ezmsg_configs.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/examples/ezmsg_count.py` & `ezmsg-3.3.1/examples/ezmsg_count.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             )
             count = count + 1
 
             if count >= self.SETTINGS.num_msgs:
                 raise ez.Complete
 
 
-class CountSystem(ez.System):
+class CountSystem(ez.Collection):
     COUNT = Count()
     TERM = TerminateTest()
 
     SUB1 = DebugLog(DebugLogSettings(name="SUB1"))
     SUB2 = DebugLog(DebugLogSettings(name="SUB2"))
 
     def network(self) -> ez.NetworkDefinition:
@@ -57,8 +57,8 @@
 
 
 if __name__ == "__main__":
     # import multiprocessing
     # multiprocessing.set_start_method('spawn', force=True)
 
     system = CountSystem()
-    ez.run_system(system)
+    ez.run(SYSTEM = system)
```

### Comparing `ezmsg-3.3.0/examples/ezmsg_intro.py` & `ezmsg-3.3.1/examples/ezmsg_intro.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/examples/ezmsg_normalterm.py` & `ezmsg-3.3.1/examples/ezmsg_normalterm.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 
 class ToySystemSettings(ez.Settings):
     num_msgs: int
     output_fn: str
 
 
-class ToySystem(ez.System):
+class ToySystem(ez.Collection):
     SETTINGS: ToySystemSettings
 
     # Publishers
     SIMPLE_PUB = MessageGenerator()
 
     # Subscribers
     SIMPLE_SUB = MessageReceiver()
@@ -105,15 +105,15 @@
     test_filename = "./test.txt"
     num_messages = 5
     with open(test_filename, "w") as f:
         ...
     system = ToySystem(
         ToySystemSettings(num_msgs=num_messages, output_fn=test_filename)
     )
-    ez.run_system(system)
+    ez.run(SYSTEM = system)
 
     results = []
     with open(test_filename, "r") as file:
         lines = file.readlines()
         for line in lines:
             results.append(json.loads(line))
     os.remove(test_filename)
```

### Comparing `ezmsg-3.3.0/examples/ezmsg_stop.py` & `ezmsg-3.3.1/examples/ezmsg_stop.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 
 class ToySystemSettings(ez.Settings):
     num_msgs: int
     output_fn: str
 
 
-class ToySystem(ez.System):
+class ToySystem(ez.Collection):
     SETTINGS: ToySystemSettings
 
     # Publishers
     SIMPLE_PUB = MessageGenerator()
 
     # Subscribers
     SIMPLE_SUB = MessageReceiver()
@@ -99,15 +99,15 @@
     test_filename = "./test.txt"
     num_messages = 5
     with open(test_filename, "w") as f:
         ...
     system = ToySystem(
         ToySystemSettings(num_msgs=num_messages, output_fn=test_filename)
     )
-    ez.run_system(system)
+    ez.run(SYSTEM = system)
 
     results = []
     with open(test_filename, "r") as file:
         lines = file.readlines()
         for line in lines:
             results.append(json.loads(line))
     os.remove(test_filename)
```

### Comparing `ezmsg-3.3.0/examples/ezmsg_toy.py` & `ezmsg-3.3.1/examples/ezmsg_toy.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,14 @@
 
 if __name__ == "__main__":
     # import multiprocessing as mp
     # mp.set_start_method( 'fork', force = True )
 
     system = TestSystem(TestSystemSettings(name="A"))
 
-    ez.run_system(
-        system,
-        # name = 'TOY',
+    ez.run(
+        SYSTEM = system,
         # connections = [
         #     ( system.PING.OUTPUT, 'PING_OUTPUT' ),
         #     ( 'FOO_SUB', system.FOOSUB.INPUT )
         # ]
     )
```

### Comparing `ezmsg-3.3.0/extensions/ezmsg-sigproc/ezmsg/sigproc/butterworthfilter.py` & `ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/butterworthfilter.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/extensions/ezmsg-sigproc/ezmsg/sigproc/decimate.py` & `ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/decimate.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/extensions/ezmsg-sigproc/ezmsg/sigproc/downsample.py` & `ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/downsample.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/extensions/ezmsg-sigproc/ezmsg/sigproc/ewmfilter.py` & `ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/ewmfilter.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/extensions/ezmsg-sigproc/ezmsg/sigproc/filter.py` & `ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/filter.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/extensions/ezmsg-sigproc/ezmsg/sigproc/messages.py` & `ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/messages.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/extensions/ezmsg-sigproc/ezmsg/sigproc/sampler.py` & `ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,15 +237,15 @@
 
 
 class SamplerTestSystemSettings(ez.Settings):
     sampler_settings: SamplerSettings
     trigger_settings: TriggerGeneratorSettings
 
 
-class SamplerTestSystem(ez.System):
+class SamplerTestSystem(ez.Collection):
     SETTINGS: SamplerTestSystemSettings
 
     OSC = Oscillator()
     SAMPLER = Sampler()
     TRIGGER = TriggerGenerator()
     DEBUG = DebugLog()
 
@@ -280,8 +280,8 @@
         trigger_settings=TriggerGeneratorSettings(
             period=(1.0, 2.0), prewait=0.5, publish_period=5.0
         ),
     )
 
     system = SamplerTestSystem(settings)
 
-    ez.run_system(system)
+    ez.run(SYSTEM = system)
```

### Comparing `ezmsg-3.3.0/extensions/ezmsg-sigproc/ezmsg/sigproc/spectral.py` & `ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/spectral.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/extensions/ezmsg-sigproc/ezmsg/sigproc/synth.py` & `ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/synth.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/extensions/ezmsg-sigproc/ezmsg/sigproc/window.py` & `ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/window.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/extensions/ezmsg-sigproc/tests/test_butterworth.py` & `ezmsg-3.3.1/extensions/ezmsg-sigproc/tests/test_butterworth.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pytest
 import numpy as np
 
 import ezmsg.core as ez
 from ezmsg.util.messages.axisarray import AxisArray
 from ezmsg.util.messagegate import MessageGate, MessageGateSettings
 from ezmsg.util.messagelogger import MessageLogger, MessageLoggerSettings
-from ezmsg.util.messagecodec import MessageDecoder
+from ezmsg.util.messagecodec import message_log
 from ezmsg.sigproc.synth import WhiteNoise, WhiteNoiseSettings
 from ezmsg.sigproc.butterworthfilter import ButterworthFilter, ButterworthFilterSettings
 
 from util import get_test_fn
 from ezmsg.util.terminate import TerminateOnTimeout as TerminateTest
 from ezmsg.util.terminate import TerminateOnTimeoutSettings as TerminateTestSettings
 
@@ -23,15 +23,15 @@
     noise_settings: WhiteNoiseSettings
     gate_settings: MessageGateSettings
     butter_settings: ButterworthFilterSettings
     log_settings: MessageLoggerSettings
     term_settings: TerminateTestSettings
 
 
-class ButterworthSystem(ez.System):
+class ButterworthSystem(ez.Collection):
     NOISE = WhiteNoise()
     GATE = MessageGate()
     BUTTER = ButterworthFilter()
     LOG = MessageLogger()
     TERM = TerminateTest()
 
     SETTINGS: ButterworthSystemSettings
@@ -86,20 +86,19 @@
         butter_settings=ButterworthFilterSettings(order=5, cutoff=cutoff, cuton=cuton),
         log_settings=MessageLoggerSettings(output=test_filename),
         term_settings=TerminateTestSettings(time=1.0),
     )
 
     system = ButterworthSystem(settings)
 
-    ez.run_system(system)
+    ez.run(SYSTEM = system)
 
     messages: List[AxisArray] = []
-    with open(test_filename, "r") as file:
-        for line in file:
-            messages.append(json.loads(line, cls=MessageDecoder))
+    for msg in message_log(test_filename):
+        messages.append(msg)
 
     os.remove(test_filename)
 
     ez.logger.info(f"Analyzing recording of { len( messages ) } messages...")
 
     data = np.concatenate([msg.data for msg in messages], axis=0)
```

### Comparing `ezmsg-3.3.0/extensions/ezmsg-sigproc/tests/test_downsample.py` & `ezmsg-3.3.1/extensions/ezmsg-sigproc/tests/test_downsample.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pytest
 import numpy as np
 
 import ezmsg.core as ez
 from ezmsg.util.messages.axisarray import AxisArray
 from ezmsg.util.messagegate import MessageGate, MessageGateSettings
 from ezmsg.util.messagelogger import MessageLogger, MessageLoggerSettings
-from ezmsg.util.messagecodec import MessageDecoder
+from ezmsg.util.messagecodec import message_log
 from ezmsg.sigproc.downsample import Downsample, DownsampleSettings
 from ezmsg.sigproc.synth import Oscillator, OscillatorSettings
 
 from util import get_test_fn
 from ezmsg.util.terminate import TerminateOnTimeout as TerminateTest
 from ezmsg.util.terminate import TerminateOnTimeoutSettings as TerminateTestSettings
 from ezmsg.util.debuglog import DebugLog
@@ -24,15 +24,15 @@
     num_msgs: int
     osc_settings: OscillatorSettings
     down_settings: DownsampleSettings
     log_settings: MessageLoggerSettings
     term_settings: TerminateTestSettings
 
 
-class DownsampleSystem(ez.System):
+class DownsampleSystem(ez.Collection):
     OSC = Oscillator()
     GATE = MessageGate()
     DOWN = Downsample()
     LOG = MessageLogger()
     TERM = TerminateTest()
 
     DEBUG = DebugLog()
@@ -86,20 +86,19 @@
         down_settings=DownsampleSettings(factor=factor),
         log_settings=MessageLoggerSettings(output=test_filename),
         term_settings=TerminateTestSettings(time=1.0),
     )
 
     system = DownsampleSystem(settings)
 
-    ez.run_system(system)
+    ez.run(SYSTEM = system)
 
     messages: List[AxisArray] = []
-    with open(test_filename, "r") as file:
-        for line in file:
-            messages.append(json.loads(line, cls=MessageDecoder))
+    for msg in message_log(test_filename):
+        messages.append(msg)
 
     os.remove(test_filename)
 
     ez.logger.info(f"Analyzing recording of { len( messages ) } messages...")
 
     fs: Optional[float] = None
     dims: Optional[List[str]] = None
```

### Comparing `ezmsg-3.3.0/extensions/ezmsg-sigproc/tests/test_window.py` & `ezmsg-3.3.1/extensions/ezmsg-sigproc/tests/test_window.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pytest
 import numpy as np
 import ezmsg.core as ez
 
 from ezmsg.util.messages.axisarray import AxisArray
 from ezmsg.util.messagegate import MessageGate, MessageGateSettings
 from ezmsg.util.messagelogger import MessageLogger, MessageLoggerSettings
-from ezmsg.util.messagecodec import MessageDecoder
+from ezmsg.util.messagecodec import message_log
 from ezmsg.sigproc.synth import Counter, CounterSettings
 from ezmsg.sigproc.window import Window, WindowSettings
 
 from util import get_test_fn
 from ezmsg.util.terminate import TerminateOnTimeout as TerminateTest
 from ezmsg.util.terminate import TerminateOnTimeoutSettings as TerminateTestSettings
 from ezmsg.util.debuglog import DebugLog
@@ -26,15 +26,15 @@
     num_msgs: int
     counter_settings: CounterSettings
     window_settings: WindowSettings
     log_settings: MessageLoggerSettings
     term_settings: TerminateTestSettings = field(default_factory=TerminateTestSettings)
 
 
-class WindowSystem(ez.System):
+class WindowSystem(ez.Collection):
     COUNTER = Counter()
     GATE = MessageGate()
     WIN = Window()
     LOG = MessageLogger()
     TERM = TerminateTest()
 
     DEBUG = DebugLog()
@@ -90,20 +90,19 @@
         window_settings=WindowSettings(window_dur=win_dur, window_shift=win_shift),
         log_settings=MessageLoggerSettings(output=test_filename),
         term_settings=TerminateTestSettings(time=1.0),  # sec
     )
 
     system = WindowSystem(settings)
 
-    ez.run_system(system)
+    ez.run(SYSTEM = system)
 
     messages: List[AxisArray] = []
-    with open(test_filename, "r") as file:
-        for line in file:
-            messages.append(json.loads(line, cls=MessageDecoder))
+    for msg in message_log(test_filename):
+        messages.append(msg)
 
     os.remove(test_filename)
 
     ez.logger.info(f"Analyzing recording of { len( messages ) } messages...")
 
     fs: Optional[float] = None
     dims: Optional[List[str]] = None
```

### Comparing `ezmsg-3.3.0/extensions/ezmsg-sigproc/tests/util.py` & `ezmsg-3.3.1/extensions/ezmsg-sigproc/tests/util.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/extensions/ezmsg-websocket/examples/ezmsg_websocket.py` & `ezmsg-3.3.1/extensions/ezmsg-websocket/examples/ezmsg_websocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
 
 class WebsocketSystemSettings(ez.Settings):
     host: str
     port: int
 
 
-class WebsocketSystem(ez.System):
+class WebsocketSystem(ez.Collection):
     SETTINGS: WebsocketSystemSettings
 
     OSC = LFO()
     SERVER = WebsocketServer()
     JSON = JSONAdapter()
     OUT = DebugOutput()
     CLIENT = WebsocketClient()
@@ -100,8 +100,8 @@
 if __name__ == "__main__":
     host = "127.0.0.1"
     port = 5038
 
     # Run the websocket system
     system = WebsocketSystem()
     system.apply_settings(WebsocketSystemSettings(host=host, port=port))
-    ez.run_system(system)
+    ez.run(SYSTEM = system)
```

### Comparing `ezmsg-3.3.0/extensions/ezmsg-websocket/ezmsg/websocket/units.py` & `ezmsg-3.3.1/extensions/ezmsg-websocket/ezmsg/websocket/units.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/extensions/ezmsg-zmq/ezmsg/zmq/units.py` & `ezmsg-3.3.1/extensions/ezmsg-zmq/ezmsg/zmq/units.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/ezmsg/core/__init__.py` & `ezmsg-3.3.1/ezmsg/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/ezmsg/core/addressable.py` & `ezmsg-3.3.1/ezmsg/core/addressable.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/ezmsg/core/backend.py` & `ezmsg-3.3.1/ezmsg/core/backend.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import logging
+import typing
 
 from socket import socket
 from multiprocessing import Event, Barrier
 from multiprocessing.synchronize import Event as EventType
 from multiprocessing.synchronize import Barrier as BarrierType
 from multiprocessing.connection import wait, Connection
 
@@ -19,32 +20,32 @@
 from .graphcontext import GraphContext
 from .backendprocess import (
     BackendProcess,
     DefaultBackendProcess,
     new_threaded_event_loop,
 )
 
-from typing import List, Callable, Tuple, Optional, Type, Set, Union, Sequence
+from .util import either_dict_or_kwargs
 
 logger = logging.getLogger("ezmsg")
 
 
 class ExecutionContext:
-    processes: List[BackendProcess]
+    processes: typing.List[BackendProcess]
     term_ev: EventType
     start_barrier: BarrierType
-    connections: List[Tuple[str, str]]
+    connections: typing.List[typing.Tuple[str, str]]
 
     def __init__(
         self,
-        processes: List[List[Unit]],
+        processes: typing.List[typing.List[Unit]],
         graph_service: GraphService,
         shm_service: SHMService,
-        connections: List[Tuple[str, str]] = [],
-        backend_process: Type[BackendProcess] = DefaultBackendProcess,
+        connections: typing.List[typing.Tuple[str, str]] = [],
+        backend_process: typing.Type[BackendProcess] = DefaultBackendProcess,
     ) -> None:
         if not processes:
             raise ValueError("Cannot create an execution context for zero processes")
 
         self.connections = connections
 
         self.term_ev = Event()
@@ -62,70 +63,68 @@
             )
             for process_units in processes
         ]
 
     @classmethod
     def setup(
         cls,
-        components: List[Component],
+        components: typing.Mapping[str, Component],
         graph_service: GraphService,
         shm_service: SHMService,
-        name: Optional[str] = None,
-        connections: Optional[NetworkDefinition] = None,
-        backend_process: Type[BackendProcess] = DefaultBackendProcess,
+        root_name: typing.Optional[str] = None,
+        connections: typing.Optional[NetworkDefinition] = None,
+        process_components: typing.Optional[typing.Collection[Component]] = None,
+        backend_process: typing.Type[BackendProcess] = DefaultBackendProcess,
         force_single_process: bool = False,
-    ) -> Optional["ExecutionContext"]:
-        graph_connections: List[Tuple[str, str]] = []
+    ) -> typing.Optional["ExecutionContext"]:
+        graph_connections: typing.List[typing.Tuple[str, str]] = []
 
-        for component in components:
+        for name, component in components.items():
             component._set_name(name)
-            component._set_location()
+            component._set_location([root_name] if root_name is not None else [])
 
         if connections is not None:
             for from_topic, to_topic in connections:
                 if isinstance(from_topic, Stream):
                     from_topic = from_topic.address
                 if isinstance(to_topic, Stream):
                     to_topic = to_topic.address
                 graph_connections.append((from_topic, to_topic))
 
         def crawl_components(
-            component: Component, callback: Callable[[Component], None]
+            component: Component, callback: typing.Callable[[Component], None]
         ) -> None:
-            search: List[Component] = [component]
+            search: typing.List[Component] = [component]
             while len(search):
                 comp = search.pop()
                 search += list(comp.components.values())
                 callback(comp)
 
         def gather_edges(comp: Component):
             if isinstance(comp, Collection):
                 for from_stream, to_stream in comp.network():
                     if isinstance(from_stream, Stream):
                         from_stream = from_stream.address
                     if isinstance(to_stream, Stream):
                         to_stream = to_stream.address
                     graph_connections.append((from_stream, to_stream))
 
-        for component in components:
+        for component in components.values():
             if isinstance(component, Collection):
                 crawl_components(component, gather_edges)
 
-        processes = []
-        for component in components:
-            if isinstance(component, Collection):
-                processes += collect_processes(component)
+        processes = collect_processes(components.values(), process_components)
 
+        for component in components.values():
+            if isinstance(component, Collection):
                 def configure_collections(comp: Component):
                     if isinstance(comp, Collection):
                         comp.configure()
 
                 crawl_components(component, configure_collections)
-            elif isinstance(component, Unit):
-                processes += [[component]]
 
         if force_single_process:
             processes = [[u for pu in processes for u in pu]]
 
         try:
             return cls(
                 processes,
@@ -138,42 +137,49 @@
             return None
 
 
 def run_system(
     system: Collection,
     num_buffers: int = 32,
     init_buf_size: int = DEFAULT_SHM_SIZE,
-    backend_process: Type[BackendProcess] = DefaultBackendProcess,
+    backend_process: typing.Type[BackendProcess] = DefaultBackendProcess,
 ) -> None:
     """Deprecated; just use run any component (unit, collection)"""
-    run(system, backend_process=backend_process)
+    run(SYSTEM = system, backend_process = backend_process)
 
 
 def run(
-    components: Union[Component, List[Component]],
-    name: Optional[str] = None,
-    connections: Optional[NetworkDefinition] = None,
-    backend_process: Type[BackendProcess] = DefaultBackendProcess,
-    graph_address: Optional[AddressType] = None,
+    components: typing.Optional[typing.Mapping[str, Component]] = None,
+    root_name: typing.Optional[str] = None,
+    connections: typing.Optional[NetworkDefinition] = None,
+    process_components: typing.Optional[typing.Collection[Component]] = None,
+    backend_process: typing.Type[BackendProcess] = DefaultBackendProcess,
+    graph_address: typing.Optional[AddressType] = None,
     force_single_process: bool = False,
+    **components_kwargs: Component
 ) -> None:
     graph_service = GraphService(graph_address)
     shm_service = SHMService()
 
-    if isinstance(components, Component):
-        components = [components]
+    if components is not None and isinstance(components, Component):
+        components = {"SYSTEM": components}
+        logger.warning("Passing a single Component without naming the Component is now Deprecated.")
+    components = either_dict_or_kwargs(components, components_kwargs, "run")
+    if components is None:
+        raise ValueError("Must supply at least one component to run")
 
     with new_threaded_event_loop() as loop:
 
         execution_context = ExecutionContext.setup(
             components,
             graph_service,
             shm_service,
-            name,
+            root_name,
             connections,
+            process_components,
             backend_process,
             force_single_process,
         )
 
         if execution_context is None:
             return
         
@@ -189,20 +195,21 @@
 
         async def setup_graph() -> None:
             for edge in execution_context.connections:
                 await graph_context.connect(*edge)
 
         asyncio.run_coroutine_threadsafe(setup_graph(), loop).result()
 
+        if len(execution_context.processes) > 1:
+            logger.info(f"Running in {len(execution_context.processes)} processes.")
+            
         main_process = execution_context.processes[0]
         other_processes = execution_context.processes[1:]
 
-        sentinels: Set[Union[Connection, socket, int]] = set()
-        if other_processes:
-            logger.info(f"Spinning up {len(other_processes)} extra processes.")
+        sentinels: typing.Set[typing.Union[Connection, socket, int]] = set()
 
         for proc in other_processes:
             proc.start()
             sentinels.add(proc.sentinel)
 
         def join_all_other_processes():
             while len(sentinels):
@@ -234,36 +241,63 @@
         finally:
             join_all_other_processes()
             asyncio.run_coroutine_threadsafe(
                 cleanup_graph(graph_context), loop
             ).result()
 
 
-def collect_processes(collection: Collection) -> List[List[Unit]]:
-    process_units, units = _collect_processes(collection)
+def collect_processes(
+    collection: typing.Union[Collection, typing.Iterable[Component]],
+    process_components: typing.Optional[typing.Collection[Component]] = None
+) -> typing.List[typing.List[Unit]]:
+    
+    if isinstance(collection, Collection):
+        process_units, units = _collect_processes(
+            collection._components.values(), 
+            collection.process_components()
+        )
+
+    else:
+        process_units, units = _collect_processes(
+            collection, 
+            process_components if process_components is not None else tuple()
+        )
+
     if len(units):
-        process_units = process_units + [units]
+        process_units = [units] + process_units 
+
     return process_units
 
 
-def _collect_processes(collection: Collection) -> Tuple[List[List[Unit]], List[Unit]]:
-    process_units: List[List[Unit]] = []
-    units: List[Unit] = []
-    for comp in collection._components.values():
+def _collect_processes(
+    comps: typing.Iterable[Component],
+    process_components: typing.Collection[Component]
+) -> typing.Tuple[typing.List[typing.List[Unit]], typing.List[Unit]]:
+    process_units: typing.List[typing.List[Unit]] = []
+    units: typing.List[Unit] = []
+    
+    for comp in comps:
+
         if isinstance(comp, Collection):
-            r_process_units, r_units = _collect_processes(comp)
+            r_process_units, r_units = _collect_processes(
+                comp.components.values(), 
+                comp.process_components()
+            )
+
             process_units = process_units + r_process_units
-            if comp in collection.process_components():
+            if comp in process_components:
                 if len(r_units) > 0:
                     process_units = process_units + [r_units]
             else:
                 if len(r_units) > 0:
                     units = units + r_units
+
         elif isinstance(comp, Unit):
-            if comp in collection.process_components():
+            if comp in process_components:
                 process_units.append([comp])
             else:
                 if hasattr(comp, PROCESS_ATTR):
                     process_units.append([comp])
                 else:
                     units.append(comp)
+
     return process_units, units
```

### Comparing `ezmsg-3.3.0/ezmsg/core/backendprocess.py` & `ezmsg-3.3.1/ezmsg/core/backendprocess.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/ezmsg/core/backpressure.py` & `ezmsg-3.3.1/ezmsg/core/backpressure.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/ezmsg/core/collection.py` & `ezmsg-3.3.1/ezmsg/core/collection.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,25 @@
+import typing
 from copy import deepcopy
 
 from .stream import Stream
 from .component import ComponentMeta, Component
 from .settings import Settings
 
-from typing import Any, Dict, Iterable, Tuple, Optional, Union
 
-
-NetworkDefinition = Iterable[Tuple[Union[Stream, str], Union[Stream, str]]]
+NetworkDefinition = typing.Iterable[typing.Tuple[typing.Union[Stream, str], typing.Union[Stream, str]]]
 
 
 class CollectionMeta(ComponentMeta):
     def __init__(
-        cls, name: str, bases: Tuple[type, ...], fields: Dict[str, Any], **kwargs: Any
+        cls, 
+        name: str, 
+        bases: typing.Tuple[type, ...], 
+        fields: typing.Dict[str, typing.Any], 
+        **kwargs: typing.Any
     ) -> None:
         super(CollectionMeta, cls).__init__(name, bases, fields)
 
         cls.__components__ = {}
 
         for base in bases:
             if hasattr(base, "__components__"):
@@ -29,23 +32,23 @@
                 field_value._set_name(field_name)
                 cls.__components__[field_name] = field_value
 
 
 class Collection(Component, metaclass=CollectionMeta):
     """Collections can contain subunits and connect them together"""
 
-    def __init__(self, settings: Optional[Settings] = None):
+    def __init__(self, settings: typing.Optional[Settings] = None):
         super(Collection, self).__init__(settings)
 
         self._components = deepcopy(self.__class__.__components__)
         for comp_name, comp in self.components.items():
             setattr(self, comp_name, comp)
 
     def configure(self) -> None:
         """This is where to percolate apply_settings to subnodes"""
         ...
 
     def network(self) -> NetworkDefinition:
         return ()
 
-    def process_components(self) -> Tuple[Component, ...]:
+    def process_components(self) -> typing.Collection[Component]:
         return (self,)
```

### Comparing `ezmsg-3.3.0/ezmsg/core/command.py` & `ezmsg-3.3.1/ezmsg/core/command.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/ezmsg/core/component.py` & `ezmsg-3.3.1/ezmsg/core/component.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/ezmsg/core/dag.py` & `ezmsg-3.3.1/ezmsg/core/dag.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/ezmsg/core/graphcontext.py` & `ezmsg-3.3.1/ezmsg/core/graphcontext.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/ezmsg/core/graphserver.py` & `ezmsg-3.3.1/ezmsg/core/graphserver.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/ezmsg/core/message.py` & `ezmsg-3.3.1/ezmsg/core/message.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/ezmsg/core/messagecache.py` & `ezmsg-3.3.1/ezmsg/core/messagecache.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/ezmsg/core/messagemarshal.py` & `ezmsg-3.3.1/ezmsg/core/messagemarshal.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/ezmsg/core/netprotocol.py` & `ezmsg-3.3.1/ezmsg/core/netprotocol.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/ezmsg/core/pubclient.py` & `ezmsg-3.3.1/ezmsg/core/pubclient.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/ezmsg/core/server.py` & `ezmsg-3.3.1/ezmsg/core/server.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/ezmsg/core/settings.py` & `ezmsg-3.3.1/ezmsg/core/settings.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/ezmsg/core/shmserver.py` & `ezmsg-3.3.1/ezmsg/core/shmserver.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/ezmsg/core/state.py` & `ezmsg-3.3.1/ezmsg/core/state.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/ezmsg/core/stream.py` & `ezmsg-3.3.1/ezmsg/core/stream.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/ezmsg/core/subclient.py` & `ezmsg-3.3.1/ezmsg/core/subclient.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/ezmsg/core/unit.py` & `ezmsg-3.3.1/ezmsg/core/unit.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/ezmsg/testing/__init__.py` & `ezmsg-3.3.1/ezmsg/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/ezmsg/testing/lfo.py` & `ezmsg-3.3.1/ezmsg/testing/lfo.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/ezmsg/testing/multiplier.py` & `ezmsg-3.3.1/ezmsg/testing/multiplier.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/ezmsg/util/debuglog.py` & `ezmsg-3.3.1/ezmsg/util/debuglog.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/ezmsg/util/messagecodec.py` & `ezmsg-3.3.1/ezmsg/util/messagecodec.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 import json
+import time
 import base64
+import typing
 import importlib
 
 from pathlib import Path
-from dataclasses import is_dataclass, fields
+from dataclasses import dataclass, is_dataclass, fields
 from functools import reduce
 
-from typing import Optional, Any, Dict, Iterable, Generator
-
 try:
     import numpy as np
     import numpy.typing as npt
 except ImportError:
     np = None
 
 TYPE = "_type"
+TIMESTAMP_ATTR = "_log_timestamp"
 NDARRAY_TYPE = "_ndarray"
 NDARRAY_DTYPE = "dtype"
 NDARRAY_SHAPE = "shape"
 NDARRAY_DATA = "data"
 
+@dataclass
+class LogStart:
+    ...
+
 
-def type_str(obj: Any) -> str:
+def type_str(obj: typing.Any) -> str:
     t = type(obj)
     name = getattr(t, "__qualname__", t.__name__)
     return f"{t.__module__}:{name}"
 
 
 def import_type(typestr: str) -> type:
     module, name = typestr.split(":")
@@ -35,63 +40,81 @@
     if not isinstance(ty, type):
         raise ImportError(f"{typestr} does not resolve to type")
 
     return ty
 
 
 class MessageEncoder(json.JSONEncoder):
-    def default(self, obj: Any):
+    def default(self, obj: typing.Any):
         if is_dataclass(obj):
+            ts = getattr(obj, TIMESTAMP_ATTR, time.time())
             return {
-                **{f.name: getattr(obj, f.name) for f in fields(obj)},
-                **{TYPE: type_str(obj)},
+                **{f.name: getattr(obj, f.name) for f in fields(obj)}, 
+                **{TYPE: type_str(obj), TIMESTAMP_ATTR: ts}
             }
 
         elif np and isinstance(obj, np.ndarray):
             contig_obj = np.ascontiguousarray(obj)
             buf = base64.b64encode(contig_obj.data)
             return {
                 TYPE: NDARRAY_TYPE,
                 NDARRAY_DTYPE: str(obj.dtype),
                 NDARRAY_DATA: buf.decode("ascii"),
                 NDARRAY_SHAPE: obj.shape,
             }
 
         return json.JSONEncoder.default(self, obj)
 
+class StampedMessage(typing.NamedTuple):
+    msg: typing.Any
+    timestamp: typing.Optional[float]
 
-class MessageDecoder(json.JSONDecoder):
+class MessageTimestampDecoder(json.JSONDecoder):
     def __init__(self, *args, **kwargs):
         json.JSONDecoder.__init__(self, object_hook=self.object_hook, *args, **kwargs)
 
-    def object_hook(self, obj: Dict[str, Any]) -> Any:
-        obj_type: Optional[str] = obj.get(TYPE)
-
-        if obj_type is None:
-            return obj
-
-        if np and obj_type == NDARRAY_TYPE:
-            data_bytes: Optional[str] = obj.get(NDARRAY_DATA)
-            data_shape: Optional[Iterable[int]] = obj.get(NDARRAY_SHAPE)
-            data_dtype: Optional[npt.DTypeLike] = obj.get(NDARRAY_DTYPE)
-
-            if (
-                isinstance(data_bytes, str)
-                and data_shape is not None
-                and data_dtype is not None
-            ):
-                buf = base64.b64decode(data_bytes.encode("ascii"))
-                return np.frombuffer(buf, dtype=data_dtype).reshape(data_shape)
-
-        else:
-            cls = import_type(obj_type)
-            del obj[TYPE]
-            return cls(**obj)
-
+    def object_hook(self, obj: typing.Dict[str, typing.Any]) -> typing.Any:
+        obj_type: typing.Optional[str] = obj.get(TYPE)
+        timestamp: typing.Optional[float] = obj.get(TIMESTAMP_ATTR)
+
+        out_obj: typing.Any = obj
+
+        if obj_type is not None:
+            if np and obj_type == NDARRAY_TYPE:
+                data_bytes: typing.Optional[str] = obj.get(NDARRAY_DATA)
+                data_shape: typing.Optional[typing.Iterable[int]] = obj.get(NDARRAY_SHAPE)
+                data_dtype: typing.Optional[npt.DTypeLike] = obj.get(NDARRAY_DTYPE)
+
+                if (
+                    isinstance(data_bytes, str)
+                    and data_shape is not None
+                    and data_dtype is not None
+                ):
+                    buf = base64.b64decode(data_bytes.encode("ascii"))
+                    out_obj = np.frombuffer(buf, dtype=data_dtype).reshape(data_shape)
+
+            else:
+                cls = import_type(obj_type)
+                del obj[TYPE]
+                if TIMESTAMP_ATTR in obj: 
+                    del obj[TIMESTAMP_ATTR]
+                out_obj = cls(**obj)
+                setattr(out_obj, TIMESTAMP_ATTR, timestamp)
+
+        return out_obj
+    
+class MessageDecoder(MessageTimestampDecoder):
+    """ Just in case there are side-effects from adding the timestamp attribute """
+    def object_hook(self, obj: typing.Dict[str, typing.Any]) -> typing.Any:
+        obj = super().object_hook(obj)
+        if hasattr(obj, TIMESTAMP_ATTR):
+            delattr(obj, TIMESTAMP_ATTR)
         return obj
+    
 
-
-def message_log(fname: Path) -> Generator[Any, None, None]:
+def message_log(fname: Path) -> typing.Generator[typing.Any, None, None]:
     with open(fname, "r") as f:
         for l in f:
             obj = json.loads(l, cls=MessageDecoder)
+            if isinstance(obj, LogStart):
+                continue
             yield obj
```

### Comparing `ezmsg-3.3.0/ezmsg/util/messagegate.py` & `ezmsg-3.3.1/ezmsg/util/messagegate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
+import typing
 from dataclasses import dataclass
-import ezmsg.core as ez
 
-from typing import Any, AsyncGenerator, Optional
+import ezmsg.core as ez
 
 
 @dataclass
 class GateMessage:
     open: bool
 
 
 class MessageGateSettings(ez.Settings):
     start_open: bool = False
     default_open: bool = False
 
     # Automatically change back to default state after X messages
-    default_after: Optional[int] = None
+    default_after: typing.Optional[int] = None
 
 
 class MessageGateState(ez.State):
-    gate_open: Optional[bool] = None
+    gate_open: typing.Optional[bool] = None
     msgs: int = 0  # Messages since last gate change
 
 
 class MessageGate(ez.Unit):
     SETTINGS: MessageGateSettings
     STATE: MessageGateState
 
     INPUT_GATE = ez.InputStream(GateMessage)
 
-    INPUT = ez.InputStream(Any)
-    OUTPUT = ez.OutputStream(Any)
+    INPUT = ez.InputStream(typing.Any)
+    OUTPUT = ez.OutputStream(typing.Any)
 
     def initialize(self) -> None:
         self.STATE.gate_open = self.SETTINGS.start_open
 
     def set_gate(self, set_open: bool) -> None:
         if self.STATE.gate_open != set_open:
             self.STATE.msgs = 0
@@ -41,19 +41,19 @@
 
     @ez.subscriber(INPUT_GATE)
     async def on_gate(self, msg: GateMessage) -> None:
         self.set_gate(msg.open)
 
     @ez.subscriber(INPUT)
     @ez.publisher(OUTPUT)
-    async def on_input(self, msg: Any) -> AsyncGenerator:
+    async def on_input(self, msg: typing.Any) -> typing.AsyncGenerator:
         self.STATE.msgs += 1
 
         if self.STATE.gate_open:
             yield (self.OUTPUT, msg)
 
         if (  # Auto-revert to default state if necessary
             (self.SETTINGS.default_after is not None)
             and (self.STATE.gate_open != self.SETTINGS.default_open)
             and (self.STATE.msgs >= self.SETTINGS.default_after)
         ):
-            self.set_gate(self.SETTINGS.default_open)
+            self.set_gate(self.SETTINGS.default_open)
```

### Comparing `ezmsg-3.3.0/ezmsg/util/messagelogger.py` & `ezmsg-3.3.1/ezmsg/util/messagelogger.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 from io import TextIOWrapper
 from dataclasses import field
 from pathlib import Path
 
 import ezmsg.core as ez
 
-from .messagecodec import MessageEncoder
+from .messagecodec import MessageEncoder, LogStart
 
 from typing import Optional, Any, Dict, AsyncGenerator, Any
 
-
+    
 class MessageLoggerSettings(ez.Settings):
     output: Optional[Path] = None
 
 
 class MessageLoggerState(ez.State):
     output_files: Dict[Path, TextIOWrapper] = field(default_factory=dict)
 
@@ -34,15 +34,19 @@
         """Returns file path if file successfully opened, otherwise None"""
         if filepath in self.STATE.output_files:
             # If the file is already open, we return None
             return None
 
         if not filepath.parent.exists():
             filepath.parent.mkdir(parents=True, exist_ok=True)
-        self.STATE.output_files[filepath] = open(filepath, mode="w")
+        output_f = open(filepath, mode="w")
+        strmessage: str = json.dumps(LogStart(), cls=MessageEncoder)
+        output_f.write(f"{strmessage}\n")
+        output_f.flush()
+        self.STATE.output_files[filepath] = output_f
 
         return filepath
 
     def close_file(self, filepath: Path) -> Optional[Path]:
         """Returns file path if file successfully closed, otherwise None"""
         if filepath not in self.STATE.output_files:
             # We haven't opened this file
```

### Comparing `ezmsg-3.3.0/ezmsg/util/messagequeue.py` & `ezmsg-3.3.1/ezmsg/util/messagequeue.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/ezmsg/util/messages/axisarray.py` & `ezmsg-3.3.1/ezmsg/util/messages/axisarray.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from contextlib import contextmanager
 from dataclasses import field, dataclass, replace
 
 import numpy as np
 import numpy.typing as npt
 
+from ezmsg.core.util import either_dict_or_kwargs
 
 @dataclass
 class AxisArray:
     data: npt.NDArray
     dims: typing.List[str]
     axes: typing.Dict[str, "AxisArray.Axis"] = field(default_factory=dict)
 
@@ -55,39 +56,62 @@
 
     def __post_init__(self):
         if len(self.dims) != self.data.ndim:
             raise ValueError("dims must be same length as data.shape")
         if len(self.dims) != len(set(self.dims)):
             raise ValueError("dims contains repeated dim names")
 
-    def isel(self, **indexers: slice) -> "AxisArray":
+    def isel(
+        self,
+        indexers: typing.Optional[typing.Any] = None,
+        **indexers_kwargs: typing.Any
+    ) -> "AxisArray":
+        
+        indexers = either_dict_or_kwargs(indexers, indexers_kwargs, 'isel')
+
         out_axes = {an: a for an, a in self.axes.items()}
         out_data = self.data
 
         for axis_name, ix in indexers.items():
-            if not isinstance(ix, slice):
-                raise ValueError("isel only supports slices for now")
+            if not isinstance(ix, (np.ndarray, int, slice)):
+                raise ValueError('isel only accepts arrays, ints, or slices')
             ax = self.ax(axis_name)
-            indices = np.arange(*ix.indices(len(ax)))
+            indices = np.arange(len(ax))
+
+            # There has to be a more efficient way to do this
+            if isinstance(ix, slice):
+                indices = indices[ix]
+            else:
+                ix = [ix] if isinstance(ix, int) else ix
+                indices = np.take(indices, ix, 0)
+
             if axis_name in out_axes:
                 out_axes[axis_name] = replace(ax.axis, offset=ax.axis.units(indices[0]))
             out_data = np.take(out_data, indices, ax.idx)
 
         return replace(self, data=out_data, axes=out_axes)
 
-    def sel(self, **indexers: slice) -> "AxisArray":
+    def sel(
+        self, 
+        indexers: typing.Optional[typing.Any] = None,
+        **indexers_kwargs: typing.Any
+    ) -> "AxisArray":
+        
+        indexers = either_dict_or_kwargs(indexers, indexers_kwargs, 'sel')
+
         out_indexers = dict()
         for axis_name, ix in indexers.items():
             axis = self.get_axis(axis_name)
             if not isinstance(ix, slice):
                 raise ValueError("sel only supports slices for now")
             start = int(axis.index(ix.start)) if ix.start is not None else None
             stop = int(axis.index(ix.stop)) if ix.stop is not None else None
             step = int(ix.step / axis.gain) if ix.step is not None else None
             out_indexers[axis_name] = slice(start, stop, step)
+            
         return self.isel(**out_indexers)
 
     @property
     def shape(self) -> typing.Tuple[int, ...]:
         """Shape of data"""
         return self.data.shape
```

### Comparing `ezmsg-3.3.0/ezmsg/util/rate.py` & `ezmsg-3.3.1/ezmsg/util/rate.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/ezmsg/util/terminate.py` & `ezmsg-3.3.1/ezmsg/util/terminate.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/ezmsg.egg-info/PKG-INFO` & `ezmsg-3.3.1/ezmsg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezmsg
-Version: 3.3.0
+Version: 3.3.1
 Summary: A simple DAG-based computation model
 Home-page: https://github.com/iscoe/ezmsg
 Author: Griffin Milsap
 Author-email: griffin.milsap@jhuapl.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `ezmsg-3.3.0/ezmsg.egg-info/SOURCES.txt` & `ezmsg-3.3.1/ezmsg.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 ezmsg/core/server.py
 ezmsg/core/settings.py
 ezmsg/core/shmserver.py
 ezmsg/core/state.py
 ezmsg/core/stream.py
 ezmsg/core/subclient.py
 ezmsg/core/unit.py
+ezmsg/core/util.py
 ezmsg/testing/__init__.py
 ezmsg/testing/debuglog.py
 ezmsg/testing/lfo.py
 ezmsg/testing/multiplier.py
 ezmsg/testing/terminate.py
 ezmsg/util/__init__.py
 ezmsg/util/debuglog.py
@@ -91,9 +92,8 @@
 tests/test_connections.py
 tests/test_dag.py
 tests/test_graph.py
 tests/test_perf.py
 tests/test_run.py
 tests/test_shm.py
 tests/test_state.py
-tests/test_test.py
-tests/test_unit.py
+tests/test_test.py
```

### Comparing `ezmsg-3.3.0/setup.cfg` & `ezmsg-3.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/tests/test_addressable.py` & `ezmsg-3.3.1/tests/test_addressable.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/tests/test_attach.py` & `ezmsg-3.3.1/tests/test_attach.py`

 * *Files 9% similar despite different names*

```diff
@@ -65,30 +65,40 @@
 class AttachTestProcess(Process):
     settings: TransmitReceiveSettings
 
     def __init__(self, settings: TransmitReceiveSettings) -> None:
         super().__init__()
         self.settings = settings
 
+TX_TOPIC = 'TX'
+RX_TOPIC = 'RX'
+ACK_TOPIC = 'ACK'
 
 class TransmitReceiveProcess(AttachTestProcess):
     def run(self) -> None:
-        ez.run(TransmitReceive(self.settings))
-
+        txrx = TransmitReceive(self.settings)
+        ez.run(
+            TXRX = txrx,
+            connections = (
+                (txrx.OUTPUT, TX_TOPIC),
+                (RX_TOPIC, txrx.INPUT),
+                (txrx.ACK, ACK_TOPIC),
+            )
+        )
 
 class AttachEchoProcess(AttachTestProcess):
     def run(self) -> None:
         for _ in range(self.settings.num_messages):
             echo = Echo()
             ez.run(
-                echo,
+                ECHO = echo,
                 connections=(
-                    ("TransmitReceive/OUTPUT", echo.INPUT),
-                    (echo.OUTPUT, "TransmitReceive/INPUT"),
-                    ("TransmitReceive/ACK", echo.ACK),
+                    (TX_TOPIC, echo.INPUT),
+                    (echo.OUTPUT, RX_TOPIC),
+                    (ACK_TOPIC, echo.ACK),
                 ),
             )
 
 
 @pytest.mark.asyncio
 async def test_attach(event_loop: asyncio.AbstractEventLoop):
     graph_service = ez.GraphService(address=ez.GraphService.default_address())
```

### Comparing `ezmsg-3.3.0/tests/test_axisarray.py` & `ezmsg-3.3.1/tests/test_axisarray.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,12 +118,10 @@
     offset = -50
     data = (np.arange(400) * gain) + offset
     aa = AxisArray(
         data, dims=["dim0"], axes=dict(dim0=AxisArray.Axis(gain=gain, offset=offset))
     )
 
     aa_sl = aa.sel(dim0=slice(None, -10.75, 1.5))  # slice based on axis info
-    print(aa_sl)
-
-
-if __name__ == "__main__":
-    test_sel()
+    aa_idx = aa.isel(dim0=-1) # index slice of last index
+    assert aa_idx.data == data[-1]
+
```

### Comparing `ezmsg-3.3.0/tests/test_connections.py` & `ezmsg-3.3.1/tests/test_connections.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,22 +23,22 @@
     def network(self) -> ez.NetworkDefinition:
         return (
             (self.INPUT1, self.LOG.INPUT),
             (self.INPUT2, self.LOG.INPUT),
         )
 
 
-class SplitSystem(ez.System):
+class SplitSystem(ez.Collection):
     SOURCE = Source()
     SPLIT = SplitCollection()
     TERM = TerminateTest()
 
     def network(self) -> ez.NetworkDefinition:
         return (
             (self.SOURCE.OUTPUT, self.TERM.INPUT),
             (self.SOURCE.OUTPUT, self.SPLIT.INPUT1),
             (self.SOURCE.OUTPUT, self.SPLIT.INPUT2),
         )
 
 
 if __name__ == "__main__":
-    ez.run_system(SplitSystem())
+    ez.run(SYSTEM = SplitSystem())
```

### Comparing `ezmsg-3.3.0/tests/test_dag.py` & `ezmsg-3.3.1/tests/test_dag.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/tests/test_graph.py` & `ezmsg-3.3.1/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/tests/test_perf.py` & `ezmsg-3.3.1/tests/test_perf.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,30 +33,32 @@
 def get_datestamp() -> str:
     return datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
 
 
 class LoadTestSettings(ez.Settings):
     duration: float = 30.0
     dynamic_size: int = 8
+    buffers: int = 32
 
 
 @dataclasses.dataclass
 class LoadTestSample:
     _timestamp: float
     counter: int
     dynamic_data: np.ndarray
 
 
 class LoadTestPublisher(ez.Unit):
     OUTPUT = ez.OutputStream(LoadTestSample)
     SETTINGS: LoadTestSettings
 
-    def setup(self) -> None:
+    def initialize(self) -> None:
         self.running = True
         self.counter = 0
+        self.OUTPUT.num_buffers = self.SETTINGS.buffers
 
     @ez.publisher(OUTPUT)
     async def publish(self) -> AsyncGenerator:
         ez.logger.info(f"Load test publisher started. (PID: {os.getpid()})")
         start_time = time.time()
         while self.running:
             current_time = time.time()
@@ -141,15 +143,15 @@
         ez.logger.info(
             f"Dropped samples: {dropped_samples} ({dropped_samples / (dropped_samples + num_samples)}%)",
         )
 
         raise ez.NormalTermination
 
 
-class LoadTest(ez.System):
+class LoadTest(ez.Collection):
     SETTINGS: LoadTestSettings
 
     PUBLISHER = LoadTestPublisher()
     SUBSCRIBER = LoadTestSubscriber()
 
     def configure(self) -> None:
         self.PUBLISHER.apply_settings(self.SETTINGS)
@@ -176,17 +178,18 @@
 @pytest.mark.parametrize("size", [2**i for i in range(5, 22, 4)])
 def test_performance(duration, size, buffers) -> None:
     ez.logger.info(f"Running load test for dynamic size: {size} bytes")
     system = LoadTest(
         LoadTestSettings(
             dynamic_size=int(size),
             duration=duration,
+            buffers=buffers
         )
     )
-    ez.run_system(system, num_buffers=buffers)
+    ez.run(SYSTEM = system)
 
 
 def run_many_dynamic_sizes(duration, buffers) -> None:
     for exp in range(5, 22, 4):
         test_performance(duration, 2**exp, buffers)
```

### Comparing `ezmsg-3.3.0/tests/test_run.py` & `ezmsg-3.3.1/tests/test_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
 
 class ToySystemSettings(ez.Settings):
     num_msgs: int
     output_fn: str
 
 
-class ToySystem(ez.System):
+class ToySystem(ez.Collection):
     SETTINGS: ToySystemSettings
 
     # Publishers
     SIMPLE_PUB = MessageGenerator()
 
     # Subscribers
     SIMPLE_SUB = MessageReceiver()
@@ -137,15 +137,15 @@
 
 @pytest.mark.parametrize("num_messages", [1, 5, 10])
 def test_local_system(toy_system_fixture, num_messages):
     test_filename = get_test_fn()
     system = toy_system_fixture(
         ToySystemSettings(num_msgs=num_messages, output_fn=test_filename)
     )
-    ez.run_system(system)
+    ez.run(SYSTEM = system)
 
     results = []
     with open(test_filename, "r") as file:
         lines = file.readlines()
         for line in lines:
             results.append(json.loads(line))
     os.remove(test_filename)
```

### Comparing `ezmsg-3.3.0/tests/test_shm.py` & `ezmsg-3.3.1/tests/test_shm.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.0/tests/test_state.py` & `ezmsg-3.3.1/tests/test_state.py`

 * *Files identical despite different names*

